# Comparing `tmp/spark_rapids_ml-23.4.0-38_b251734-py3-none-any.whl.zip` & `tmp/spark_rapids_ml-23.6.0-100_04dffdf-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,22 @@
-Zip file size: 52237 bytes, number of entries: 16
--rw-r--r--  2.0 unx      615 b- defN 23-Apr-28 03:47 spark_rapids_ml/__init__.py
--rw-r--r--  2.0 unx     9944 b- defN 23-Apr-28 03:47 spark_rapids_ml/classification.py
--rw-r--r--  2.0 unx    13967 b- defN 23-Apr-28 03:47 spark_rapids_ml/clustering.py
--rw-r--r--  2.0 unx    29140 b- defN 23-Apr-28 03:47 spark_rapids_ml/core.py
--rw-r--r--  2.0 unx    13432 b- defN 23-Apr-28 03:47 spark_rapids_ml/feature.py
--rw-r--r--  2.0 unx    24378 b- defN 23-Apr-28 03:47 spark_rapids_ml/knn.py
--rw-r--r--  2.0 unx    14982 b- defN 23-Apr-28 03:47 spark_rapids_ml/params.py
--rw-r--r--  2.0 unx    22364 b- defN 23-Apr-28 03:47 spark_rapids_ml/regression.py
--rw-r--r--  2.0 unx    16334 b- defN 23-Apr-28 03:47 spark_rapids_ml/tree.py
--rw-r--r--  2.0 unx    12469 b- defN 23-Apr-28 03:47 spark_rapids_ml/utils.py
--rw-r--r--  2.0 unx      592 b- defN 23-Apr-28 03:47 spark_rapids_ml/common/__init__.py
--rw-r--r--  2.0 unx     6545 b- defN 23-Apr-28 03:47 spark_rapids_ml/common/cuml_context.py
--rw-r--r--  2.0 unx     8766 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1357 b- defN 23-Apr-28 06:15 spark_rapids_ml-23.4.0.dist-info/RECORD
-16 files, 174993 bytes uncompressed, 50005 bytes compressed:  71.4%
+Zip file size: 70100 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      615 b- defN 23-Jul-12 06:25 spark_rapids_ml/__init__.py
+-rw-r--r--  2.0 unx    18806 b- defN 23-Jul-12 06:25 spark_rapids_ml/classification.py
+-rw-r--r--  2.0 unx    14009 b- defN 23-Jul-12 06:25 spark_rapids_ml/clustering.py
+-rw-r--r--  2.0 unx    38441 b- defN 23-Jul-12 06:25 spark_rapids_ml/core.py
+-rw-r--r--  2.0 unx    13694 b- defN 23-Jul-12 06:25 spark_rapids_ml/feature.py
+-rw-r--r--  2.0 unx    24409 b- defN 23-Jul-12 06:25 spark_rapids_ml/knn.py
+-rw-r--r--  2.0 unx    16419 b- defN 23-Jul-12 06:25 spark_rapids_ml/params.py
+-rw-r--r--  2.0 unx    37608 b- defN 23-Jul-12 06:25 spark_rapids_ml/regression.py
+-rw-r--r--  2.0 unx    20969 b- defN 23-Jul-12 06:25 spark_rapids_ml/tree.py
+-rw-r--r--  2.0 unx     6731 b- defN 23-Jul-12 06:25 spark_rapids_ml/tuning.py
+-rw-r--r--  2.0 unx    14648 b- defN 23-Jul-12 06:25 spark_rapids_ml/utils.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Jul-12 06:25 spark_rapids_ml/common/__init__.py
+-rw-r--r--  2.0 unx     6545 b- defN 23-Jul-12 06:25 spark_rapids_ml/common/cuml_context.py
+-rw-r--r--  2.0 unx     6144 b- defN 23-Jul-12 06:25 spark_rapids_ml/metrics/MulticlassMetrics.py
+-rw-r--r--  2.0 unx     9495 b- defN 23-Jul-12 06:25 spark_rapids_ml/metrics/RegressionMetrics.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Jul-12 06:25 spark_rapids_ml/metrics/__init__.py
+-rw-r--r--  2.0 unx     8766 b- defN 23-Jul-12 10:13 spark_rapids_ml-23.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:13 spark_rapids_ml-23.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-12 10:13 spark_rapids_ml-23.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1733 b- defN 23-Jul-12 10:13 spark_rapids_ml-23.6.0.dist-info/RECORD
+20 files, 240324 bytes uncompressed, 67268 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -21,29 +21,41 @@
 
 Filename: spark_rapids_ml/regression.py
 Comment: 
 
 Filename: spark_rapids_ml/tree.py
 Comment: 
 
+Filename: spark_rapids_ml/tuning.py
+Comment: 
+
 Filename: spark_rapids_ml/utils.py
 Comment: 
 
 Filename: spark_rapids_ml/common/__init__.py
 Comment: 
 
 Filename: spark_rapids_ml/common/cuml_context.py
 Comment: 
 
-Filename: spark_rapids_ml-23.4.0.dist-info/METADATA
+Filename: spark_rapids_ml/metrics/MulticlassMetrics.py
+Comment: 
+
+Filename: spark_rapids_ml/metrics/RegressionMetrics.py
+Comment: 
+
+Filename: spark_rapids_ml/metrics/__init__.py
+Comment: 
+
+Filename: spark_rapids_ml-23.6.0.dist-info/METADATA
 Comment: 
 
-Filename: spark_rapids_ml-23.4.0.dist-info/WHEEL
+Filename: spark_rapids_ml-23.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: spark_rapids_ml-23.4.0.dist-info/top_level.txt
+Filename: spark_rapids_ml-23.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_rapids_ml-23.4.0.dist-info/RECORD
+Filename: spark_rapids_ml-23.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_rapids_ml/__init__.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "23.4.0"
+__version__ = "23.6.0"
```

## spark_rapids_ml/classification.py

```diff
@@ -9,37 +9,56 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
+
+from pyspark.ml.evaluation import Evaluator, MulticlassClassificationEvaluator
+
+from .metrics.MulticlassMetrics import MulticlassMetrics
 
 if TYPE_CHECKING:
-    import cudf
+    from pyspark.ml._typing import ParamMap
 
-import numpy as np
 import pandas as pd
-from pyspark import Row
+from pyspark import Row, keyword_only
 from pyspark.ml.classification import BinaryRandomForestClassificationSummary
 from pyspark.ml.classification import (
     RandomForestClassificationModel as SparkRandomForestClassificationModel,
 )
 from pyspark.ml.classification import (
     RandomForestClassificationSummary,
     _RandomForestClassifierParams,
 )
 from pyspark.ml.linalg import Vector
 from pyspark.ml.param.shared import HasProbabilityCol, HasRawPredictionCol
 from pyspark.sql import Column, DataFrame
 from pyspark.sql.functions import col
-from pyspark.sql.types import DoubleType, FloatType, IntegerType, IntegralType
+from pyspark.sql.types import (
+    DoubleType,
+    FloatType,
+    IntegerType,
+    IntegralType,
+    StructField,
+    StructType,
+)
 
-from .core import CumlT, alias, pred
+from .core import (
+    CumlT,
+    TransformInputType,
+    _ConstructFunc,
+    _EvaluateFunc,
+    _TransformFunc,
+    alias,
+    pred,
+    transform_evaluate,
+)
 from .tree import (
     _RandomForestClass,
     _RandomForestCumlParams,
     _RandomForestEstimator,
     _RandomForestModel,
 )
 from .utils import _get_spark_session
@@ -75,28 +94,105 @@
     _RFClassifierParams,
 ):
     """RandomForestClassifier implements a Random Forest classifier model which
     fits multiple decision tree classifiers in an ensemble. It supports both
     binary and multiclass labels. It implements cuML's GPU accelerated
     RandomForestClassifier algorithm based on cuML python library,
     and it can be used in PySpark Pipeline and PySpark ML meta algorithms like
-    :py:class:`~pyspark.ml.tuning.CrossValidator`/
-    :py:class:`~pyspark.ml.tuning.TrainValidationSplit`/
-    :py:class:`~pyspark.ml.classification.OneVsRest`
+    :py:class:`~pyspark.ml.tuning.CrossValidator`,
+    :py:class:`~pyspark.ml.tuning.TrainValidationSplit`,
+    :py:class:`~pyspark.ml.classification.OneVsRest`.
 
     The distributed algorithm uses an *embarrassingly-parallel* approach. For a
     forest with `N` trees being built on `w` workers, each worker simply builds `N/w`
     trees on the data it has available locally. In many cases, partitioning the
     data so that each worker builds trees on a subset of the total dataset works
     well, but it generally requires the data to be well-shuffled in advance.
 
     RandomForestClassifier automatically supports most of the parameters from both
-    :py:class:`~pyspark.ml.classification.RandomForestClassifier` and in the constructors of
-    :py:class:`cuml.ensemble.RandomForestClassifier`. And it can automatically map pyspark
-    parameters to cuML parameters.
+    :py:class:`~pyspark.ml.classification.RandomForestClassifier`
+    and :py:class:`cuml.ensemble.RandomForestClassifier`. And it can automatically
+    map pyspark parameters to cuML parameters.
+
+
+    Parameters
+    ----------
+
+    featuresCol:
+        The feature column names, spark-rapids-ml supports vector, array and columnar as the input.\n
+            * When the value is a string, the feature columns must be assembled into 1 column with vector or array type.
+            * When the value is a list of strings, the feature columns must be numeric types.
+    labelCol:
+        The label column name.
+    predictionCol:
+        The prediction column name.
+    probabilityCol
+        The column name for predicted class conditional probabilities.
+    rawPredictionCol:
+        The raw prediction column name.
+    maxDepth:
+        Maximum tree depth. Must be greater than 0.
+    maxBins:
+        Maximum number of bins used by the split algorithm per feature.
+    minInstancesPerNode:
+        The minimum number of samples (rows) in each leaf node.
+    impurity: str = "gini",
+        The criterion used to split nodes.\n
+            * ``'gini'`` for gini impurity
+            * ``'entropy'`` for information gain (entropy)
+    numTrees:
+        Total number of trees in the forest.
+    featureSubsetStrategy:
+        Ratio of number of features (columns) to consider per node split.\n
+        The supported options:\n
+            ``'auto'``:  If numTrees == 1, set to 'all', If numTrees > 1 (forest), set to 'sqrt'\n
+            ``'all'``: use all features\n
+            ``'onethird'``: use 1/3 of the features\n
+            ``'sqrt'``: use sqrt(number of features)\n
+            ``'log2'``: log2(number of features)\n
+            ``'n'``: when n is in the range (0, 1.0], use n * number of features. When n
+            is in the range (1, number of features), use n features.
+    seed:
+        Seed for the random number generator.
+    bootstrap:
+        Control bootstrapping.\n
+            * If ``True``, each tree in the forest is built on a bootstrapped
+              sample with replacement.
+            * If ``False``, the whole dataset is used to build each tree.
+    num_workers:
+        Number of cuML workers, where each cuML worker corresponds to one Spark task
+        running on one GPU. If not set, spark-rapids-ml tries to infer the number of
+        cuML workers (i.e. GPUs in cluster) from the Spark environment.
+    verbose:
+        Logging level.
+            * ``0`` - Disables all log messages.
+            * ``1`` - Enables only critical messages.
+            * ``2`` - Enables all messages up to and including errors.
+            * ``3`` - Enables all messages up to and including warnings.
+            * ``4 or False`` - Enables all messages up to and including information messages.
+            * ``5 or True`` - Enables all messages up to and including debug messages.
+            * ``6`` - Enables all messages up to and including trace messages.
+    n_streams:
+        Number of parallel streams used for forest building.
+        Please note that there is a bug running spark-rapids-ml on a node with multi-gpus
+        when n_streams > 1. See https://github.com/rapidsai/cuml/issues/5402.
+    min_samples_split:
+        The minimum number of samples required to split an internal node.\n
+         * If type ``int``, then ``min_samples_split`` represents the minimum
+           number.
+         * If type ``float``, then ``min_samples_split`` represents a fraction
+           and ``ceil(min_samples_split * n_rows)`` is the minimum number of
+           samples for each split.    max_samples:
+        Ratio of dataset rows used while fitting each tree.
+    max_leaves:
+        Maximum leaf nodes per tree. Soft constraint. Unlimited, if -1.
+    min_impurity_decrease:
+        Minimum decrease in impurity required for node to be split.
+    max_batch_size:
+        Maximum number of nodes that can be processed in a given batch.
 
     Examples
     --------
     >>> import numpy
     >>> from numpy import allclose
     >>> from pyspark.ml.linalg import Vectors
     >>> from pyspark.ml.feature import StringIndexer
@@ -134,23 +230,42 @@
     >>> model2.getNumTrees
     3
     >>> model.transform(test0).take(1) == model2.transform(test0).take(1)
     True
 
     """
 
-    def __init__(self, **kwargs: Any):
-        super().__init__(**kwargs)
-        self.set_params(**kwargs)
-
-    def setNumTrees(self, value: int) -> "RandomForestClassifier":
-        """
-        Sets the value of :py:attr:`numTrees`.
-        """
-        return self._set(numTrees=value)
+    @keyword_only
+    def __init__(
+        self,
+        *,
+        featuresCol: Union[str, List[str]] = "features",
+        labelCol: str = "label",
+        predictionCol: str = "prediction",
+        probabilityCol: str = "probability",
+        rawPredictionCol: str = "rawPrediction",
+        maxDepth: int = 5,
+        maxBins: int = 32,
+        minInstancesPerNode: int = 1,
+        impurity: str = "gini",
+        numTrees: int = 20,
+        featureSubsetStrategy: str = "auto",
+        seed: Optional[int] = None,
+        bootstrap: Optional[bool] = True,
+        num_workers: Optional[int] = None,
+        verbose: Union[int, bool] = False,
+        n_streams: int = 1,
+        min_samples_split: Union[int, float] = 2,
+        max_samples: float = 1.0,
+        max_leaves: int = -1,
+        min_impurity_decrease: float = 0.0,
+        max_batch_size: int = 4096,
+        **kwargs: Any,
+    ):
+        super().__init__(**self._input_kwargs)
 
     def _pre_process_label(
         self, dataset: DataFrame, feature_type: Union[Type[FloatType], Type[DoubleType]]
     ) -> Column:
         """Cuml RandomForestClassifier requires the int32 type of label column"""
         label_name = self.getLabelCol()
         label_datatype = dataset.schema[label_name].dataType
@@ -165,14 +280,24 @@
 
     def _create_pyspark_model(self, result: Row) -> "RandomForestClassificationModel":
         return RandomForestClassificationModel.from_row(result)
 
     def _is_classification(self) -> bool:
         return True
 
+    def _supportsTransformEvaluate(self, evaluator: Evaluator) -> bool:
+        if (
+            isinstance(evaluator, MulticlassClassificationEvaluator)
+            and evaluator.getMetricName()
+            in MulticlassMetrics.SUPPORTED_MULTI_CLASS_METRIC_NAMES
+        ):
+            return True
+
+        return False
+
 
 class RandomForestClassificationModel(
     _RandomForestClass,
     _RandomForestModel,
     _RandomForestCumlParams,
     _RFClassifierParams,
 ):
@@ -180,16 +305,16 @@
     Model fitted by :class:`RandomForestClassifier`.
     """
 
     def __init__(
         self,
         n_cols: int,
         dtype: str,
-        treelite_model: str,
-        model_json: List[str],
+        treelite_model: Union[str, List[str]],
+        model_json: Union[List[str], List[List[str]]],
         num_classes: int,
     ):
         super().__init__(
             dtype=dtype,
             n_cols=n_cols,
             treelite_model=treelite_model,
             model_json=model_json,
@@ -215,38 +340,14 @@
                 self.numFeatures,
                 self._num_classes,
             )
             self._rf_spark_model = SparkRandomForestClassificationModel(java_rf_model)
             self._copyValues(self._rf_spark_model)
         return self._rf_spark_model
 
-    def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
-        _construct_rf, _ = super()._get_cuml_transform_func(dataset)
-
-        def _predict(rf: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
-            data = {}
-            rf.update_labels = False
-            data[pred.prediction] = rf.predict(pdf)
-            probs = rf.predict_proba(pdf)
-            if isinstance(probs, pd.DataFrame):
-                # For 2302, when input is multi-cols, the output will be DataFrame
-                data[pred.probability] = pd.Series(probs.values.tolist())
-            else:
-                # should be np.ndarray
-                data[pred.probability] = pd.Series(list(probs))
-
-            return pd.DataFrame(data)
-
-        return _construct_rf, _predict
-
     def _is_classification(self) -> bool:
         return True
 
     @property
     def hasSummary(self) -> bool:
         """Indicates whether a training summary exists for this model instance."""
         return False
@@ -278,7 +379,133 @@
 
         Parameters
         ----------
         dataset : :py:class:`pyspark.sql.DataFrame`
             Test dataset to evaluate model on.
         """
         return self.cpu().evaluate(dataset)
+
+    def _get_cuml_transform_func(
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
+        _construct_rf, _, _ = super()._get_cuml_transform_func(dataset)
+
+        def _predict(rf: CumlT, pdf: TransformInputType) -> pd.Series:
+            data = {}
+            rf.update_labels = False
+            data[pred.prediction] = rf.predict(pdf)
+
+            if category == transform_evaluate.transform:
+                # transform_evaluate doesn't need probs for f1 score.
+                probs = rf.predict_proba(pdf)
+                if isinstance(probs, pd.DataFrame):
+                    # For 2302, when input is multi-cols, the output will be DataFrame
+                    data[pred.probability] = pd.Series(probs.values.tolist())
+                else:
+                    # should be np.ndarray
+                    data[pred.probability] = pd.Series(list(probs))
+
+            return pd.DataFrame(data)
+
+        def _evaluate(
+            input: TransformInputType,
+            transformed: TransformInputType,
+        ) -> pd.DataFrame:
+            # calculate the count of (label, prediction)
+            comb = pd.DataFrame(
+                {
+                    "label": input[alias.label],
+                    "prediction": transformed[pred.prediction],
+                }
+            )
+            confusion = (
+                comb.groupby(["label", "prediction"]).size().reset_index(name="total")
+            )
+            return confusion
+
+        return _construct_rf, _predict, _evaluate
+
+    def _transformEvaluate(
+        self,
+        dataset: DataFrame,
+        evaluator: Evaluator,
+        params: Optional["ParamMap"] = None,
+    ) -> List[float]:
+        """
+        Transforms and evaluates the input dataset with optional parameters in a single pass.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            a dataset that contains labels/observations and predictions
+        evaluator: :py:class:`pyspark.ml.evaluation.Evaluator`
+            an evaluator user intends to use
+        params : dict, optional
+            an optional param map that overrides embedded params
+
+        Returns
+        -------
+        list of float
+            metrics
+        """
+
+        if not isinstance(evaluator, MulticlassClassificationEvaluator):
+            raise NotImplementedError(f"{evaluator} is unsupported yet.")
+
+        if (
+            evaluator.getMetricName()
+            not in MulticlassMetrics.SUPPORTED_MULTI_CLASS_METRIC_NAMES
+        ):
+            raise NotImplementedError(
+                f"{evaluator.getMetricName()} is not supported yet."
+            )
+
+        if self.getLabelCol() not in dataset.schema.names:
+            raise RuntimeError("Label column is not existing.")
+
+        dataset = dataset.withColumnRenamed(self.getLabelCol(), alias.label)
+
+        schema = StructType(
+            [
+                StructField(pred.model_index, IntegerType()),
+                StructField("label", FloatType()),
+                StructField("prediction", FloatType()),
+                StructField("total", FloatType()),
+            ]
+        )
+
+        rows = super()._transform_evaluate_internal(dataset, schema).collect()
+
+        num_models = (
+            len(self._treelite_model) if isinstance(self._treelite_model, list) else 1
+        )
+
+        tp_by_class: List[Dict[float, float]] = [{} for _ in range(num_models)]
+        fp_by_class: List[Dict[float, float]] = [{} for _ in range(num_models)]
+        label_count_by_class: List[Dict[float, float]] = [{} for _ in range(num_models)]
+        label_count = [0 for _ in range(num_models)]
+
+        for i in range(num_models):
+            for j in range(self._num_classes):
+                tp_by_class[i][float(j)] = 0.0
+                label_count_by_class[i][float(j)] = 0.0
+                fp_by_class[i][float(j)] = 0.0
+
+        for row in rows:
+            label_count[row.model_index] += row.total
+            label_count_by_class[row.model_index][row.label] += row.total
+
+            if row.label == row.prediction:
+                tp_by_class[row.model_index][row.label] += row.total
+            else:
+                fp_by_class[row.model_index][row.prediction] += row.total
+
+        scores = []
+        for i in range(num_models):
+            metrics = MulticlassMetrics(
+                tp=tp_by_class[i],
+                fp=fp_by_class[i],
+                label=label_count_by_class[i],
+                label_count=label_count[i],
+            )
+            scores.append(metrics.evaluate(evaluator))
+        return scores
```

## spark_rapids_ml/clustering.py

```diff
@@ -10,28 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
-
-if TYPE_CHECKING:
-    import cudf
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
 from pyspark.ml.clustering import KMeansModel as SparkKMeansModel
 from pyspark.ml.clustering import _KMeansParams
 from pyspark.ml.linalg import Vector
 from pyspark.sql.dataframe import DataFrame
@@ -42,19 +29,23 @@
     Row,
     StringType,
     StructField,
     StructType,
 )
 
 from .core import (
-    CumlInputType,
     CumlT,
+    FitInputType,
+    _ConstructFunc,
     _CumlEstimator,
-    _CumlModelSupervised,
+    _CumlModelWithPredictionCol,
+    _EvaluateFunc,
+    _TransformFunc,
     param_alias,
+    transform_evaluate,
 )
 from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
 from .utils import (
     _ArrayOrder,
     _concat_and_free,
     _get_spark_session,
     get_logger,
@@ -265,39 +256,40 @@
         """
         raise ValueError("'weightCol' is not supported by cuML.")
 
     def _fit_array_order(self) -> _ArrayOrder:
         return "C"
 
     def _get_cuml_fit_func(
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         cls = self.__class__
 
         array_order = self._fit_array_order()
 
         def _cuml_fit(
-            dfs: CumlInputType,
+            dfs: FitInputType,
             params: Dict[str, Any],
         ) -> Dict[str, Any]:
+            import cupy as cp
             from cuml.cluster.kmeans_mg import KMeansMG as CumlKMeansMG
 
             kmeans_object = CumlKMeansMG(
                 handle=params[param_alias.handle],
                 output_type="cudf",
                 **params[param_alias.cuml_init],
             )
             df_list = [x for (x, _, _) in dfs]
             if isinstance(df_list[0], pd.DataFrame):
                 concated = pd.concat(df_list)
             else:
-                # should be list of np.ndarrays here
-                concated = _concat_and_free(
-                    cast(List[np.ndarray], df_list), order=array_order
-                )
+                # features are either cp or np arrays here
+                concated = _concat_and_free(df_list, order=array_order)
 
             kmeans_object.fit(
                 concated,
                 sample_weight=None,
             )
 
             logger = get_logger(cls)
@@ -327,15 +319,15 @@
             ]
         )
 
     def _create_pyspark_model(self, result: Row) -> "KMeansModel":
         return KMeansModel.from_row(result)
 
 
-class KMeansModel(KMeansClass, _CumlModelSupervised, _KMeansCumlParams):
+class KMeansModel(KMeansClass, _CumlModelWithPredictionCol, _KMeansCumlParams):
     """
     KMeans gpu model for clustering input vectors to learned k centers.
     Refer to the KMeans class for learning the k centers.
     """
 
     def __init__(
         self,
@@ -391,19 +383,16 @@
         ret_schema = "int"
         return ret_schema
 
     def _transform_array_order(self) -> _ArrayOrder:
         return "C"
 
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         cuml_alg_params = self.cuml_params.copy()
 
         cluster_centers_ = self.cluster_centers_
         dtype = self.dtype
         n_cols = self.n_cols
         array_order = self._transform_array_order()
 
@@ -422,8 +411,8 @@
 
         def _transform_internal(
             kmeans: CumlT, df: Union[pd.DataFrame, np.ndarray]
         ) -> pd.Series:
             res = list(kmeans.predict(df, normalize_weights=False).to_numpy())
             return pd.Series(res)
 
-        return _construct_kmeans, _transform_internal
+        return _construct_kmeans, _transform_internal, None
```

## spark_rapids_ml/core.py

```diff
@@ -11,34 +11,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import json
 import os
+import threading
 from abc import abstractmethod
 from collections import namedtuple
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
+    Generic,
     Iterator,
     List,
     Optional,
+    Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import numpy as np
 import pandas as pd
 from pyspark import RDD, TaskContext
 from pyspark.ml import Estimator, Model
+from pyspark.ml.evaluation import Evaluator
 from pyspark.ml.functions import array_to_vector, vector_to_array
 from pyspark.ml.linalg import VectorUDT
 from pyspark.ml.param.shared import (
     HasLabelCol,
     HasOutputCol,
     HasPredictionCol,
     HasProbabilityCol,
@@ -72,42 +76,66 @@
     _is_local,
     dtype_to_pyspark_type,
     get_logger,
 )
 
 if TYPE_CHECKING:
     import cudf
-    from cuml.cluster.kmeans_mg import KMeansMG
-    from cuml.decomposition.pca_mg import PCAMG
+    from pyspark.ml._typing import ParamMap
 
-    CumlT = TypeVar("CumlT", PCAMG, KMeansMG)
-else:
-    CumlT = Any
+CumlT = Any
 
 _SinglePdDataFrameBatchType = Tuple[
     pd.DataFrame, Optional[pd.DataFrame], Optional[pd.DataFrame]
 ]
 _SingleNpArrayBatchType = Tuple[np.ndarray, Optional[np.ndarray], Optional[np.ndarray]]
-# CumlInputType is type of [(feature, label), ...]
-CumlInputType = Union[List[_SinglePdDataFrameBatchType], List[_SingleNpArrayBatchType]]
 
+# FitInputType is type of [(feature, label), ...]
+FitInputType = Union[List[_SinglePdDataFrameBatchType], List[_SingleNpArrayBatchType]]
+
+# TransformInput type
+TransformInputType = Union["cudf.DataFrame", np.ndarray]
+
+# Function to construct cuml instances on the executor side
+_ConstructFunc = Callable[..., Union[CumlT, List[CumlT]]]
+
+# Function to do the inference using cuml instance constructed by _ConstructFunc
+_TransformFunc = Callable[[CumlT, TransformInputType], pd.DataFrame]
+
+# Function to do evaluation based on the prediction result got from _TransformFunc
+_EvaluateFunc = Callable[
+    [
+        TransformInputType,  # input dataset with label column
+        TransformInputType,  # inferred dataset with prediction column
+    ],
+    pd.DataFrame,
+]
 
 # Global constant for defining column alias
 Alias = namedtuple("Alias", ("data", "label", "row_number"))
 alias = Alias("cuml_values", "cuml_label", "unique_id")
 
 # Global prediction names
-Pred = namedtuple("Pred", ("prediction", "probability"))
-pred = Pred("prediction", "probability")
+Pred = namedtuple("Pred", ("prediction", "probability", "model_index"))
+pred = Pred("prediction", "probability", "model_index")
 
 # Global parameter alias used by core and subclasses.
 ParamAlias = namedtuple(
-    "ParamAlias", ("cuml_init", "handle", "num_cols", "part_sizes", "loop")
+    "ParamAlias",
+    ("cuml_init", "handle", "num_cols", "part_sizes", "loop", "fit_multiple_params"),
 )
-param_alias = ParamAlias("cuml_init", "handle", "num_cols", "part_sizes", "loop")
+param_alias = ParamAlias(
+    "cuml_init", "handle", "num_cols", "part_sizes", "loop", "fit_multiple_params"
+)
+
+CumlModel = TypeVar("CumlModel", bound="_CumlModel")
+
+# Global parameter used by core and subclasses.
+TransformEvaluate = namedtuple("TransformEvaluate", ("transform", "transform_evaluate"))
+transform_evaluate = TransformEvaluate("transform", "transform_evaluate")
 
 
 class _CumlEstimatorWriter(MLWriter):
     """
     Write the parameters of _CumlEstimator to the file
     """
 
@@ -135,14 +163,15 @@
     def __init__(self, cls: Type) -> None:
         super().__init__()
         self.estimator_cls = cls
 
     def load(self, path: str) -> "_CumlEstimator":
         metadata = DefaultParamsReader.loadMetadata(path, self.sc)
         cuml_estimator = self.estimator_cls()
+        cuml_estimator._resetUid(metadata["uid"])
         DefaultParamsReader.getAndSetParams(cuml_estimator, metadata)
         cuml_estimator._cuml_params = metadata["_cuml_params"]
         cuml_estimator._num_workers = metadata["_num_workers"]
         return cuml_estimator
 
 
 class _CumlModelWriter(MLWriter):
@@ -340,23 +369,25 @@
         Return (True, False) if only NCCL is required.
         Return (True, True) if UCX is required. Cuml UCX backend currently also requires NCCL.
         """
         return (True, False)
 
     @abstractmethod
     def _get_cuml_fit_func(
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         """
         Subclass must implement this function to return a cuml fit function that will be
         sent to executor to run.
 
         Eg,
 
-        def _get_cuml_fit_func(self, dataset: DataFrame):
+        def _get_cuml_fit_func(self, dataset: DataFrame, extra_params: Optional[List[Dict[str, Any]]] = None):
             ...
             def _cuml_fit(df: CumlInputType, params: Dict[str, Any]) -> Dict[str, Any]:
                 "" "
                 df:  a sequence of (X, Y)
                 params: a series of parameters stored in dictionary,
                     especially, the parameters of __init__ is stored in params[param_alias.init]
                 "" "
@@ -367,15 +398,18 @@
 
         _get_cuml_fit_func itself runs on the driver side, while the returned _cuml_fit will
         run on the executor side.
         """
         raise NotImplementedError()
 
     def _call_cuml_fit_func(
-        self, dataset: DataFrame, partially_collect: bool = True
+        self,
+        dataset: DataFrame,
+        partially_collect: bool = True,
+        paramMaps: Optional[Sequence["ParamMap"]] = None,
     ) -> RDD:
         """
         Fits a model to the input dataset. This is called by the default implementation of fit.
 
         Parameters
         ----------
         dataset : :py:class:`pyspark.sql.DataFrame`
@@ -396,31 +430,64 @@
         dataset = dataset.select(*select_cols)
 
         if dataset.rdd.getNumPartitions() != num_workers:
             dataset = self._repartition_dataset(dataset)
 
         is_local = _is_local(_get_spark_session().sparkContext)
 
+        cuda_managed_mem_enabled = (
+            _get_spark_session().conf.get("spark.rapids.ml.uvm.enabled", "false")
+            == "true"
+        )
+        if cuda_managed_mem_enabled:
+            get_logger(cls).info("CUDA managed memory enabled.")
+
+        # parameters passed to subclass
         params: Dict[str, Any] = {
             param_alias.cuml_init: self.cuml_params,
         }
 
-        cuml_fit_func = self._get_cuml_fit_func(dataset)
+        # Convert the paramMaps into cuml paramMaps
+        fit_multiple_params = []
+        if paramMaps is not None:
+            for paramMap in paramMaps:
+                tmp_fit_multiple_params = {}
+                for k, v in paramMap.items():
+                    name = self._get_cuml_param(k.name, False)
+                    assert name is not None
+                    tmp_fit_multiple_params[name] = self._get_cuml_mapping_value(
+                        name, v
+                    )
+                fit_multiple_params.append(tmp_fit_multiple_params)
+        params[param_alias.fit_multiple_params] = fit_multiple_params
+
+        cuml_fit_func = self._get_cuml_fit_func(
+            dataset, None if len(fit_multiple_params) == 0 else fit_multiple_params
+        )
         array_order = self._fit_array_order()
 
         cuml_verbose = self.cuml_params.get("verbose", False)
 
         (enable_nccl, require_ucx) = self._require_nccl_ucx()
 
         def _train_udf(pdf_iter: Iterator[pd.DataFrame]) -> pd.DataFrame:
             from pyspark import BarrierTaskContext
 
             logger = get_logger(cls)
             logger.info("Initializing cuml context")
 
+            import cupy as cp
+
+            if cuda_managed_mem_enabled:
+                import rmm
+                from rmm.allocators.cupy import rmm_cupy_allocator
+
+                rmm.reinitialize(managed_memory=True)
+                cp.cuda.set_allocator(rmm_cupy_allocator)
+
             _CumlCommon.initialize_cuml_logging(cuml_verbose)
 
             context = BarrierTaskContext.get()
             partition_id = context.partitionId()
 
             # set gpu device
             _CumlCommon.set_gpu_device(context, is_local)
@@ -432,17 +499,22 @@
                 # inputs = [(X, Optional(y)), (X, Optional(y))]
                 logger.info("Loading data into python worker memory")
                 inputs = []
                 sizes = []
                 for pdf in pdf_iter:
                     sizes.append(pdf.shape[0])
                     if multi_col_names:
-                        features = pdf[multi_col_names]
+                        features = np.array(pdf[multi_col_names], order=array_order)
                     else:
                         features = np.array(list(pdf[alias.data]), order=array_order)
+                    # experiments indicate it is faster to convert to numpy array and then to cupy array than directly
+                    # invoking cupy array on the list
+                    if cuda_managed_mem_enabled:
+                        features = cp.array(features)
+
                     label = pdf[alias.label] if alias.label in pdf.columns else None
                     row_number = (
                         pdf[alias.row_number]
                         if alias.row_number in pdf.columns
                         else None
                     )
                     inputs.append((features, label, row_number))
@@ -480,53 +552,166 @@
     def _fit_array_order(self) -> _ArrayOrder:
         """
         preferred array order for converting single column array type to numpy arrays: "C" or "F"
         """
         return "F"
 
 
+class _FitMultipleIterator(Generic[CumlModel]):
+    """
+    Used by default implementation of Estimator.fitMultiple to produce models in a thread safe
+    iterator. This class handles the gpu version of fitMultiple where all param maps should be
+    fit in a single pass.
+
+    Parameters
+    ----------
+    fitMultipleModels : function
+        Callable[[], CumlModel] which fits multiple models to a dataset in a single pass.
+    numModels : int
+        Number of models this iterator should produce.
+
+    Notes
+    -----
+    See :py:meth:`Estimator.fitMultiple` for more info.
+    """
+
+    def __init__(
+        self, fitMultipleModels: Callable[[], List[CumlModel]], numModels: int
+    ):
+        self.fitMultipleModels = fitMultipleModels
+        self.numModels = numModels
+        self.counter = 0
+        self.lock = threading.Lock()
+        self.models: List[CumlModel] = []
+
+    def __iter__(self) -> Iterator[Tuple[int, CumlModel]]:
+        return self
+
+    def __next__(self) -> Tuple[int, CumlModel]:
+        with self.lock:
+            index = self.counter
+            if index >= self.numModels:
+                raise StopIteration("No models remaining.")
+            if index == 0:
+                self.models = self.fitMultipleModels()
+                assert len(self.models) == self.numModels
+            self.counter += 1
+        return index, self.models[index]
+
+    def next(self) -> Tuple[int, CumlModel]:
+        return self.__next__()
+
+
 class _CumlEstimator(Estimator, _CumlCaller):
     """
     The common estimator to handle the fit callback (_fit). It should:
     1. set the default parameters
     2. validate the parameters
     3. prepare the dataset
     4. train and return CUML model
     5. create the pyspark model
     """
 
+    # used by keywords_only
+    _input_kwargs: Dict[str, Any]
+
     def __init__(self) -> None:
         super().__init__()
 
     @abstractmethod
     def _create_pyspark_model(self, result: Row) -> "_CumlModel":
         """
         Create the model according to the collected Row
         """
         raise NotImplementedError()
 
-    def _fit(self, dataset: DataFrame) -> "_CumlModel":
+    def _enable_fit_multiple_in_single_pass(self) -> bool:
+        """flag to indicate if fitMultiple in a single pass is supported.
+        If not, fallback to super().fitMultiple"""
+        return False
+
+    def fitMultiple(
+        self, dataset: DataFrame, paramMaps: Sequence["ParamMap"]
+    ) -> Iterator[Tuple[int, "_CumlModel"]]:
+        """
+        Fits multiple models to the input dataset for all param maps in a single pass.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            input dataset.
+        paramMaps : :py:class:`collections.abc.Sequence`
+            A Sequence of param maps.
+
+        Returns
+        -------
+        :py:class:`_FitMultipleIterator`
+            A thread safe iterable which contains one model for each param map. Each
+            call to `next(modelIterator)` will return `(index, model)` where model was fit
+            using `paramMaps[index]`. `index` values may not be sequential.
+        """
+
+        if self._enable_fit_multiple_in_single_pass():
+            estimator = self.copy()
+
+            def fitMultipleModels() -> List["_CumlModel"]:
+                return estimator._fit_internal(dataset, paramMaps)
+
+            return _FitMultipleIterator(fitMultipleModels, len(paramMaps))
+        else:
+            return super().fitMultiple(dataset, paramMaps)
+
+    def _fit_internal(
+        self, dataset: DataFrame, paramMaps: Optional[Sequence["ParamMap"]]
+    ) -> List["_CumlModel"]:
+        """Fit multiple models according to the parameters maps"""
         pipelined_rdd = self._call_cuml_fit_func(
-            dataset=dataset, partially_collect=True
+            dataset=dataset,
+            partially_collect=True,
+            paramMaps=paramMaps,
         )
-        ret = pipelined_rdd.collect()[0]
+        rows = pipelined_rdd.collect()
+
+        models: List["_CumlModel"] = [None]  # type: ignore
+        if paramMaps is not None:
+            models = [None] * len(paramMaps)  # type: ignore
+
+        for index in range(len(models)):
+            model = self._create_pyspark_model(rows[index])
+            model._num_workers = self._num_workers
+
+            if paramMaps is not None:
+                self._copyValues(model, paramMaps[index])
+            else:
+                self._copyValues(model)
+
+            self._copy_cuml_params(model)  # type: ignore
+
+            models[index] = model  # type: ignore
+
+        return models
 
-        model = self._create_pyspark_model(ret)
-        model._num_workers = self._num_workers
-        self._copyValues(model)
-        self._copy_cuml_params(model)  # type: ignore
-        return model
+    def _fit(self, dataset: DataFrame) -> "_CumlModel":
+        """fit only 1 model"""
+        return self._fit_internal(dataset, None)[0]
 
     def write(self) -> MLWriter:
         return _CumlEstimatorWriter(self)
 
     @classmethod
     def read(cls) -> MLReader:
         return _CumlEstimatorReader(cls)
 
+    def _supportsTransformEvaluate(self, evaluator: Evaluator) -> bool:
+        """If supporting _transformEvaluate in a single pass based on the evaluator
+
+        Please note that this function should only be used in CrossValidator for quick
+        fallback if unsupported."""
+        return False
+
 
 class _CumlEstimatorSupervised(_CumlEstimator, HasLabelCol):
     """
     Base class for Cuml Supervised machine learning.
     """
 
     def _pre_process_label(
@@ -606,38 +791,39 @@
         So please make sure if the constructor can accept all of them.
         """
         attr_dict = model_attributes.asDict()
         return cls(**attr_dict)
 
     @abstractmethod
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         """
-        Subclass must implement this function to return two functions,
+        Subclass must implement this function to return three functions,
         1. a function to construct cuml counterpart instance
         2. a function to transform the dataset
+        3. an optional function to evaluate.
 
         Eg,
 
         def _get_cuml_transform_func(self, dataset: DataFrame):
             ...
             def _construct_cuml_object() -> CumlT
                 ...
             def _cuml_transform(cuml_obj: CumlT, df: Union[pd.DataFrame, np.ndarray]) ->pd.DataFrame:
                 ...
+            def _evaluate(input_df: Union[pd.DataFrame, np.ndarray], transformed_df: Union[pd.DataFrame, np.ndarray]) -> pd.DataFrame:
+                ...
             ...
 
-            return _construct_cuml_object, _cuml_transform
+            # please note that if category is transform, the evaluate function will be ignored.
+            return _construct_cuml_object, _cuml_transform, _evaluate
 
         _get_cuml_transform_func itself runs on the driver side, while the returned
-        _construct_cuml_object and _cuml_transform will run on the executor side.
+        _construct_cuml_object and _cuml_transform, _evaluate will run on the executor side.
         """
         raise NotImplementedError()
 
     def _transform_array_order(self) -> _ArrayOrder:
         """
         preferred array order for converting single column array type to numpy arrays: "C" or "F"
         """
@@ -650,15 +836,21 @@
         construct the returning pandas dataframe
         """
         raise NotImplementedError()
 
     def _pre_process_data(
         self, dataset: DataFrame
     ) -> Tuple[DataFrame, List[str], bool]:
-        """Pre-handle the dataset before transform."""
+        """Pre-handle the dataset before transform.
+
+        Please note that, this function just transforms the input column if necessary, and
+        it will keep the unused columns.
+
+        return (dataset, list of feature names, bool value to indicate if it is multi-columns input)
+        """
         select_cols = []
         input_is_multi_cols = True
 
         input_col, input_cols = self._get_input_columns()
 
         if input_col is not None:
             if isinstance(dataset.schema[input_col].dataType, VectorUDT):
@@ -679,70 +871,118 @@
             select_cols.extend(input_cols)
         else:
             # should never get here
             raise Exception("Unable to determine input column(s).")
 
         return dataset, select_cols, input_is_multi_cols
 
-    def _transform(self, dataset: DataFrame) -> DataFrame:
-        """
-        Transforms the input dataset.
-
-        Parameters
-        ----------
-        dataset : :py:class:`pyspark.sql.DataFrame`
-            input dataset.
-
-        Returns
-        -------
-        :py:class:`pyspark.sql.DataFrame`
-            transformed dataset
-        """
+    def _transform_evaluate_internal(
+        self, dataset: DataFrame, schema: Union[StructType, str]
+    ) -> DataFrame:
+        """Internal API to support transform and evaluation in a single pass"""
         dataset, select_cols, input_is_multi_cols = self._pre_process_data(dataset)
 
         is_local = _is_local(_get_spark_session().sparkContext)
 
         # Get the functions which will be passed into executor to run.
         (
             construct_cuml_object_func,
             cuml_transform_func,
-        ) = self._get_cuml_transform_func(dataset)
+            evaluate_func,
+        ) = self._get_cuml_transform_func(
+            dataset, transform_evaluate.transform_evaluate
+        )
 
         array_order = self._transform_array_order()
 
         def _transform_udf(pdf_iter: Iterator[pd.DataFrame]) -> pd.DataFrame:
             from pyspark import TaskContext
 
             context = TaskContext.get()
 
             _CumlCommon.set_gpu_device(context, is_local, True)
 
             # Construct the cuml counterpart object
-            cuml_object = construct_cuml_object_func()
+            cuml_instance = construct_cuml_object_func()
+            cuml_objects = (
+                cuml_instance if isinstance(cuml_instance, list) else [cuml_instance]
+            )
 
-            # Transform the dataset
-            if input_is_multi_cols:
-                for pdf in pdf_iter:
-                    yield cuml_transform_func(cuml_object, pdf[select_cols])
-            else:
-                for pdf in pdf_iter:
-                    nparray = np.array(list(pdf[select_cols[0]]), order=array_order)
-                    yield cuml_transform_func(cuml_object, nparray)
+            # TODO try to concatenate all the data and do the transform.
+            for pdf in pdf_iter:
+                for index, cuml_object in enumerate(cuml_objects):
+                    # Transform the dataset
+                    if input_is_multi_cols:
+                        data = cuml_transform_func(cuml_object, pdf[select_cols])
+                    else:
+                        nparray = np.array(list(pdf[select_cols[0]]), order=array_order)
+                        data = cuml_transform_func(cuml_object, nparray)
+                    # Evaluate the dataset if necessary.
+                    if evaluate_func is not None:
+                        data = evaluate_func(pdf, data)
+                        data[pred.model_index] = index
+                    yield data
+
+        return dataset.mapInPandas(_transform_udf, schema=schema)  # type: ignore
 
-        return dataset.mapInPandas(
-            _transform_udf, schema=self._out_schema(dataset.schema)  # type: ignore
+    def _transform(self, dataset: DataFrame) -> DataFrame:
+        """
+        Transforms the input dataset.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            input dataset.
+
+        Returns
+        -------
+        :py:class:`pyspark.sql.DataFrame`
+            transformed dataset
+        """
+        return self._transform_evaluate_internal(
+            dataset, schema=self._out_schema(dataset.schema)
         )
 
     def write(self) -> MLWriter:
         return _CumlModelWriter(self)
 
     @classmethod
     def read(cls) -> MLReader:
         return _CumlModelReader(cls)
 
+    def _transformEvaluate(
+        self,
+        dataset: DataFrame,
+        evaluator: Evaluator,
+        params: Optional["ParamMap"] = None,
+    ) -> List[float]:
+        """
+        Transforms and evaluates the input dataset with optional parameters in a single pass.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            a dataset that contains labels/observations and predictions
+        evaluator: :py:class:`pyspark.ml.evaluation.Evaluator`
+            an evaluator user intends to use
+        params : dict, optional
+            an optional param map that overrides embedded params
+
+        Returns
+        -------
+        list of float
+            metrics
+        """
+        raise NotImplementedError()
+
+    @classmethod
+    def _combine(cls: Type["_CumlModel"], models: List["_CumlModel"]) -> "_CumlModel":
+        """Combine a list of same type models into a model"""
+        raise NotImplementedError()
+
 
 class _CumlModelWithColumns(_CumlModel):
     """Cuml base model for generating extra predicted columns"""
 
     def _is_single_pred(self, input_schema: StructType) -> bool:
         """Indicate if the transform is only predicting 1 column"""
         schema = self._out_schema(input_schema)
@@ -773,30 +1013,35 @@
 
         is_local = _is_local(_get_spark_session().sparkContext)
 
         # Get the functions which will be passed into executor to run.
         (
             construct_cuml_object_func,
             cuml_transform_func,
+            _,
         ) = self._get_cuml_transform_func(dataset)
 
         array_order = self._transform_array_order()
 
         @pandas_udf(self._out_schema(dataset.schema))  # type: ignore
         def predict_udf(iterator: Iterator[pd.DataFrame]) -> Iterator[pd.Series]:
             from pyspark import TaskContext
 
             context = TaskContext.get()
             _CumlCommon.set_gpu_device(context, is_local, True)
-            cuml_object = construct_cuml_object_func()
+            cuml_objects = construct_cuml_object_func()
+            cuml_object = (
+                cuml_objects[0] if isinstance(cuml_objects, list) else cuml_objects
+            )
             for pdf in iterator:
                 if not input_is_multi_cols:
                     data = np.array(list(pdf[select_cols[0]]), order=array_order)
                 else:
                     data = pdf[select_cols]
+                # for normal transform, we don't allow multiple models.
                 res = cuml_transform_func(cuml_object, data)
                 del data
                 yield res
 
         pred_name = self._get_prediction_name()
         pred_col = predict_udf(struct(*select_cols))
 
@@ -837,16 +1082,16 @@
             schema = f"{schema}, {pred.probability} array<{pyspark_type}>"
         else:
             schema = f"{pyspark_type}"
 
         return schema
 
 
-class _CumlModelSupervised(_CumlModelWithColumns, HasPredictionCol):
-    """Cuml base model for supervised machine learning Eg, RF/LR"""
+class _CumlModelWithPredictionCol(_CumlModelWithColumns, HasPredictionCol):
+    """Cuml base model with prediction col"""
 
     @property  # type: ignore[misc]
     def numFeatures(self) -> int:
         """
         Returns the number of features the model was trained on. If unknown, returns -1
         """
```

## spark_rapids_ml/feature.py

```diff
@@ -11,18 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import itertools
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
-
-if TYPE_CHECKING:
-    import cudf
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from pyspark.ml.common import _py2java
 from pyspark.ml.feature import PCAModel as SparkPCAModel
 from pyspark.ml.feature import _PCAParams
 from pyspark.ml.linalg import DenseMatrix, DenseVector
@@ -35,19 +32,23 @@
     Row,
     StringType,
     StructField,
     StructType,
 )
 
 from .core import (
-    CumlInputType,
     CumlT,
+    FitInputType,
+    _ConstructFunc,
     _CumlEstimator,
     _CumlModelWithColumns,
+    _EvaluateFunc,
+    _TransformFunc,
     param_alias,
+    transform_evaluate,
 )
 from .params import P, _CumlClass, _CumlParams
 from .utils import (
     PartitionDescriptor,
     _get_spark_session,
     dtype_to_pyspark_type,
     java_uid,
@@ -134,15 +135,15 @@
     >>> gpu_model.getK()
     1
     >>> print(gpu_model.mean)
     [2.0, 2.0]
     >>> print(gpu_model.pc)
     DenseMatrix([[0.70710678],
                  [0.70710678]])
-    >>> print(gpu_model.explainedVariance)
+    >>> print(gpu_model.explained_variance)
     [1.0]
     >>> gpu_pca.save("/tmp/pca")
 
     >>> # vector column input
     >>> from pyspark.ml.linalg import Vectors
     >>> data = [(Vectors.dense([1.0, 1.0]),),
     ...         (Vectors.dense([2.0, 2.0]),),
@@ -171,36 +172,41 @@
     def setK(self, value: int) -> "PCA":
         """
         Sets the value of :py:attr:`k`.
         """
         return self.set_params(k=value)
 
     def _get_cuml_fit_func(
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         def _cuml_fit(
-            dfs: CumlInputType,
+            dfs: FitInputType,
             params: Dict[str, Any],
         ) -> Dict[str, Any]:
             from cuml.decomposition.pca_mg import PCAMG as CumlPCAMG
 
             pca_object = CumlPCAMG(
                 handle=params[param_alias.handle],
                 output_type="cudf",
                 **params[param_alias.cuml_init],
             )
 
             pdesc = PartitionDescriptor.build(
                 params[param_alias.part_sizes], params[param_alias.num_cols]
             )
+            data_arrays = [x for x, _, _ in dfs]
+            # reverse list order to compensate for cuda managed memory LRU eviction
+            stride = -1
             pca_object.fit(
-                [x for x, _, _ in dfs],
+                data_arrays[::stride],
                 pdesc.m,
                 pdesc.n,
-                pdesc.parts_rank_size,
+                pdesc.parts_rank_size[::stride],
                 pdesc.rank,
                 _transform=False,
             )
 
             cpu_mean = pca_object.mean_.to_arrow().to_pylist()
             cpu_pc = pca_object.components_.to_numpy().tolist()
             cpu_explained_variance = (
@@ -333,19 +339,16 @@
             )
             self._pca_ml_model = SparkPCAModel(java_model)
             self._copyValues(self._pca_ml_model)
 
         return self._pca_ml_model
 
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         cuml_alg_params = self.cuml_params.copy()
 
         n_cols = self.n_cols
         dype = self.dtype
         components = self.components_
         mean = self.mean_
         singular_values = self.singular_values_
@@ -391,14 +394,14 @@
             res = pca_object.transform(df)
             # Spark does not remove the mean from the transformed data,
             # but cuML does, so need to add the mean back to match Spark results
             res += transformed_mean
 
             return pd.Series(list(res))
 
-        return _construct_pca, _transform_internal
+        return _construct_pca, _transform_internal, None
 
     def _out_schema(self, input_schema: StructType) -> Union[StructType, str]:
         assert self.dtype is not None
 
         pyspark_type = dtype_to_pyspark_type(self.dtype)
         return f"array<{pyspark_type}>"
```

## spark_rapids_ml/knn.py

```diff
@@ -11,28 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import asyncio
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
-
-if TYPE_CHECKING:
-    import cudf
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 import numpy as np
 import pandas as pd
 from pyspark.ml.functions import vector_to_array
 from pyspark.ml.linalg import VectorUDT
 from pyspark.ml.param.shared import (
     HasInputCol,
@@ -52,21 +39,25 @@
     LongType,
     Row,
     StructField,
     StructType,
 )
 
 from .core import (
-    CumlInputType,
     CumlT,
+    FitInputType,
+    _ConstructFunc,
     _CumlCaller,
     _CumlEstimatorSupervised,
     _CumlModel,
+    _EvaluateFunc,
+    _TransformFunc,
     alias,
     param_alias,
+    transform_evaluate,
 )
 from .params import P, _CumlClass, _CumlParams
 from .utils import _concat_and_free
 
 
 class NearestNeighborsClass(_CumlClass):
     @classmethod
@@ -295,15 +286,15 @@
         """
         This class overrides _fit and will not call _out_schema.
         """
         pass
 
     def _get_cuml_fit_func(  # type: ignore
         self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         """
         This class overrides _fit and will not call _get_cuml_fit_func.
         """
         pass
 
     def write(self) -> MLWriter:
         raise NotImplementedError(
@@ -436,23 +427,25 @@
         )
         knn_df = knn_rdd.toDF(
             schema=f"{query_id_col_name} {id_col_type}, indices array<{id_col_type}>, distances array<float>"
         ).sort(query_id_col_name)
 
         return (self._item_df_withid, query_df_withid, knn_df)
 
-    def _get_cuml_fit_func(  # type: ignore
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+    def _get_cuml_fit_func(
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         label_isdata = self._label_isdata
         label_isquery = self._label_isquery
         id_col_name = self.getIdCol()
 
         def _cuml_fit(
-            dfs: CumlInputType,
+            dfs: FitInputType,
             params: Dict[str, Any],
         ) -> Dict[str, Any]:
             from pyspark import BarrierTaskContext
 
             context = BarrierTaskContext.get()
             rank = context.partitionId()
 
@@ -564,19 +557,16 @@
 
     def _transform(self, dataset: DataFrame) -> DataFrame:
         raise NotImplementedError(
             "NearestNeighborsModel does not provide a transform function. Use 'kneighbors' instead."
         )
 
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         raise NotImplementedError(
             "'_CumlModel._get_cuml_transform_func' method is not implemented. Use 'kneighbors' instead."
         )
 
     def exactNearestNeighborsJoin(
         self,
         query_df: DataFrame,
```

## spark_rapids_ml/params.py

```diff
@@ -11,21 +11,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from abc import abstractmethod
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 from pyspark.ml.param import Param, Params, TypeConverters
 from pyspark.sql import SparkSession
 
 from .utils import _is_local
 
+if TYPE_CHECKING:
+    from pyspark.ml._typing import ParamMap
+
 P = TypeVar("P", bound="_CumlParams")
 
 
 class HasFeaturesCols(Params):
     """
     Mixin for param featuresCols: features column names for multi-column input.
     """
@@ -159,14 +172,36 @@
             else self._num_workers
         )
 
     @num_workers.setter
     def num_workers(self, value: int) -> None:
         self._num_workers = value
 
+    def copy(self: P, extra: Optional["ParamMap"] = None) -> P:
+        # override this function to update cuml_params if possible
+        instance: P = super().copy(extra)
+        cuml_params = instance.cuml_params.copy()
+
+        if isinstance(extra, dict):
+            for param, value in extra.items():
+                if isinstance(param, Param):
+                    name = instance._get_cuml_param(param.name, silent=False)
+                    if name is not None:
+                        cuml_params[name] = instance._get_cuml_mapping_value(
+                            name, value
+                        )
+                else:
+                    raise TypeError(
+                        "Expecting a valid instance of Param, but received: {}".format(
+                            param
+                        )
+                    )
+        instance._cuml_params = cuml_params
+        return instance
+
     def initialize_cuml_params(self) -> None:
         """
         Set the default values of cuML parameters to match their Spark equivalents.
         """
         # initialize cuml_params with defaults from cuML
         self._cuml_params = self._get_cuml_params_default()
 
@@ -334,14 +369,35 @@
                     )
         except Exception as e:
             # ignore any exceptions and just use default value
             print(e)
 
         return num_workers
 
+    def _get_cuml_param(self, spark_param: str, silent: bool = True) -> Optional[str]:
+        param_map = self._param_mapping()
+
+        if spark_param in param_map:
+            cuml_param = param_map[spark_param]
+            if cuml_param is None:
+                if not silent:
+                    # if Spark Param is mapped to None, raise error
+                    raise ValueError(
+                        f"Spark Param '{spark_param}' is not supported by cuML."
+                    )
+            elif cuml_param == "":
+                # if Spark Param is mapped to empty string, warn and continue
+                if not silent:
+                    print(f"WARNING: Spark Param '{spark_param}' is not used by cuML.")
+                cuml_param = None
+
+            return cuml_param
+        else:
+            return None
+
     def _set_cuml_param(
         self, spark_param: str, spark_value: Any, silent: bool = True
     ) -> None:
         """Set a cuml_params parameter for a given Spark Param and value.
 
         Parameters
         ----------
@@ -353,30 +409,33 @@
             Don't warn or raise errors, default=True.
 
         Raises
         ------
         ValueError
             If the Spark Param is explictly not supported.
         """
-        param_map = self._param_mapping()
-        if spark_param in param_map:
-            cuml_param = param_map[spark_param]
-            if cuml_param is None:
-                if not silent:
-                    # if Spark Param is mapped to None, raise error
-                    raise ValueError(
-                        f"Spark Param '{spark_param}' is not supported by cuML."
-                    )
-            elif cuml_param == "":
-                # if Spark Param is mapped to empty string, warn and continue
-                if not silent:
-                    print(f"WARNING: Spark Param '{spark_param}' is not used by cuML.")
+
+        cuml_param = self._get_cuml_param(spark_param, silent)
+
+        if cuml_param is not None:
+            # if Spark Param is mapped to cuML parameter, set cuml_params
+            self._set_cuml_value(cuml_param, spark_value)
+
+    def _get_cuml_mapping_value(self, k: str, v: Any) -> Any:
+        value_map = self._param_value_mapping()
+        if k not in value_map:
+            # no value mapping required
+            return v
+        else:
+            # value map exists
+            mapped_v = value_map[k](v)
+            if mapped_v is not None:
+                return mapped_v
             else:
-                # if Spark Param is mapped to cuML parameter, set cuml_params
-                self._set_cuml_value(cuml_param, spark_value)
+                raise ValueError(f"Value '{v}' for '{k}' param is unsupported")
 
     def _set_cuml_value(self, k: str, v: Any) -> None:
         """
         Set a cuml_params parameter with a (mapped) value.
 
         If the value originated from a Spark ML Param, and a value mapping exists, the parameter
         will be set to the mapped value.  Generally, this is only useful for string/enum types.
@@ -390,18 +449,9 @@
 
         Raises
         ------
         ValueError
             If a value mapping exists, but the mapped value is None, this means that there is
             no equivalent value for the cuML side, so an exception is raised.
         """
-        value_map = self._param_value_mapping()
-        if k not in value_map:
-            # no value mapping required
-            self._cuml_params[k] = v
-        else:
-            # value map exists
-            mapped_v = value_map[k](v)
-            if mapped_v:
-                self._cuml_params[k] = mapped_v
-            else:
-                raise ValueError(f"Value '{v}' for '{k}' param is unsupported")
+        value_map = self._get_cuml_mapping_value(k, v)
+        self._cuml_params[k] = value_map
```

## spark_rapids_ml/regression.py

```diff
@@ -19,23 +19,22 @@
     Dict,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
-if TYPE_CHECKING:
-    import cudf
-
 import numpy as np
 import pandas as pd
-from pyspark import Row
+from pyspark import Row, TaskContext, keyword_only
 from pyspark.ml.common import _py2java
+from pyspark.ml.evaluation import Evaluator, RegressionEvaluator
 from pyspark.ml.linalg import Vector, Vectors, _convert_to_vector
 from pyspark.ml.regression import LinearRegressionModel as SparkLinearRegressionModel
 from pyspark.ml.regression import LinearRegressionSummary
 from pyspark.ml.regression import (
     RandomForestRegressionModel as SparkRandomForestRegressionModel,
 )
 from pyspark.ml.regression import _LinearRegressionParams, _RandomForestRegressorParams
@@ -47,32 +46,126 @@
     IntegerType,
     StringType,
     StructField,
     StructType,
 )
 
 from .core import (
-    CumlInputType,
     CumlT,
+    FitInputType,
+    TransformInputType,
+    _ConstructFunc,
     _CumlEstimatorSupervised,
-    _CumlModelSupervised,
+    _CumlModel,
+    _CumlModelWithPredictionCol,
+    _EvaluateFunc,
+    _TransformFunc,
+    alias,
     param_alias,
+    pred,
+    transform_evaluate,
 )
+from .metrics.RegressionMetrics import RegressionMetrics, reg_metrics
 from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
 from .tree import (
     _RandomForestClass,
     _RandomForestCumlParams,
     _RandomForestEstimator,
     _RandomForestModel,
 )
 from .utils import PartitionDescriptor, _get_spark_session, cudf_to_cuml_array, java_uid
 
+if TYPE_CHECKING:
+    from pyspark.ml._typing import ParamMap
+
 T = TypeVar("T")
 
 
+class _RegressionModelEvaluationMixIn:
+    # https://github.com/python/mypy/issues/5868#issuecomment-437690894 to bypass mypy checking
+    _this_model: Union["RandomForestRegressionModel", "LinearRegressionModel"]
+
+    def _transform_evaluate(
+        self,
+        dataset: DataFrame,
+        evaluator: Evaluator,
+        num_models: int,
+        params: Optional["ParamMap"] = None,
+    ) -> List[float]:
+        """
+        Transforms and evaluates the input dataset with optional parameters in a single pass.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            a dataset that contains labels/observations and predictions
+        evaluator: :py:class:`pyspark.ml.evaluation.Evaluator`
+            an evaluator user intends to use
+        num_models: how many models are used to perform transform and evaluation in a single pass
+        params : dict, optional
+            an optional param map that overrides embedded params
+
+        Returns
+        -------
+        list of float
+            metrics
+        """
+
+        if not isinstance(evaluator, RegressionEvaluator):
+            raise NotImplementedError(f"{evaluator} is unsupported yet.")
+
+        if self._this_model.getLabelCol() not in dataset.schema.names:
+            raise RuntimeError("Label column is not existing.")
+
+        dataset = dataset.withColumnRenamed(self._this_model.getLabelCol(), alias.label)
+
+        schema = StructType(
+            [
+                StructField(pred.model_index, IntegerType()),
+                StructField(reg_metrics.mean, ArrayType(FloatType())),
+                StructField(reg_metrics.m2n, ArrayType(FloatType())),
+                StructField(reg_metrics.m2, ArrayType(FloatType())),
+                StructField(reg_metrics.l1, ArrayType(FloatType())),
+                StructField(reg_metrics.total_count, IntegerType()),
+            ]
+        )
+
+        rows = self._this_model._transform_evaluate_internal(dataset, schema).collect()
+
+        metrics = RegressionMetrics.from_rows(num_models, rows)
+        return [metric.evaluate(evaluator) for metric in metrics]
+
+    @staticmethod
+    def calculate_regression_metrics(
+        input: TransformInputType,
+        transformed: TransformInputType,
+    ) -> pd.DataFrame:
+        """calculate the metrics: mean/m2n/m2/l1 ...
+
+        input must have `alias.label` column"""
+
+        comb = pd.DataFrame(
+            {
+                "label": input[alias.label],
+                "prediction": transformed,
+            }
+        )
+        comb.insert(1, "label-prediction", comb["label"] - comb["prediction"])
+        total_cnt = comb.shape[0]
+        return pd.DataFrame(
+            data={
+                reg_metrics.mean: [comb.mean().to_list()],
+                reg_metrics.m2n: [(comb.var(ddof=0) * total_cnt).to_list()],
+                reg_metrics.m2: [comb.pow(2).sum().to_list()],
+                reg_metrics.l1: [comb.abs().sum().to_list()],
+                reg_metrics.total_count: total_cnt,
+            }
+        )
+
+
 class LinearRegressionClass(_CumlClass):
     @classmethod
     def _param_mapping(cls) -> Dict[str, Optional[str]]:
         return {
             "aggregationDepth": "",
             "elasticNetParam": "l1_ratio",
             "epsilon": "",
@@ -185,25 +278,69 @@
 
     * none (a.k.a. ordinary least squares)
     * L2 (ridge regression)
     * L1 (Lasso)
     * L2 + L1 (elastic net)
 
     LinearRegression automatically supports most of the parameters from both
-    :py:class:`~pyspark.ml.regression.LinearRegression` and in the constructors of
+    :py:class:`~pyspark.ml.regression.LinearRegression`,
     :py:class:`cuml.LinearRegression`, :py:class:`cuml.Ridge`, :py:class:`cuml.Lasso`
     and :py:class:`cuml.ElasticNet`. And it will automatically map pyspark parameters
     to cuML parameters.
 
-    Note
-    ----
+    Notes
+    -----
         Results for spark ML and spark rapids ml fit() will currently match in all regularization
         cases only if features and labels are standardized in the input dataframe.  Otherwise,
         they will match only if regParam = 0 or elastNetParam = 1.0 (aka Lasso).
 
+    Parameters
+    ----------
+
+    featuresCol:
+        The feature column names, spark-rapids-ml supports vector, array and columnar as the input.\n
+            * When the value is a string, the feature columns must be assembled into 1 column with vector or array type.
+            * When the value is a list of strings, the feature columns must be numeric types.
+    labelCol:
+        The label column name.
+    predictionCol:
+        The prediction column name.
+    maxIter:
+        Max number of iterations (>= 0).
+    regParam:
+        Regularization parameter (>= 0)
+    elasticNetParam:
+        The ElasticNet mixing parameter, in range [0, 1]. For alpha = 0,
+        the penalty is an L2 penalty. For alpha = 1, it is an L1 penalty.
+    tol:
+        The convergence tolerance for iterative algorithms (>= 0).
+    fitIntercept:
+        whether to fit an intercept term.
+    standardization:
+        Whether to standardize the training features before fitting the model.
+    solver:
+        The solver algorithm for optimization. If this is not set or empty, default value is 'auto'.\n
+        The supported options: 'auto', 'normal' and 'eig', all of them will be mapped to 'eig' in cuML.
+    loss:
+        The loss function to be optimized.
+        The supported options: 'squaredError'
+    num_workers:
+        Number of cuML workers, where each cuML worker corresponds to one Spark task
+        running on one GPU. If not set, spark-rapids-ml tries to infer the number of
+        cuML workers (i.e. GPUs in cluster) from the Spark environment.
+    verbose:
+        Logging level.
+            * ``0`` - Disables all log messages.
+            * ``1`` - Enables only critical messages.
+            * ``2`` - Enables all messages up to and including errors.
+            * ``3`` - Enables all messages up to and including warnings.
+            * ``4 or False`` - Enables all messages up to and including information messages.
+            * ``5 or True`` - Enables all messages up to and including debug messages.
+            * ``6`` - Enables all messages up to and including trace messages.
+
     Examples
     --------
     >>> from spark_rapids_ml.regression import LinearRegression, LinearRegressionModel
     >>> from pyspark.ml.linalg import Vectors
     >>>
     >>> df = spark.createDataFrame([
     ...     (6.5, Vectors.dense(1.0, 2.0)),
@@ -251,17 +388,35 @@
     +-----+----------+------------------+
     |  6.5|[1.0, 2.0]|               6.5|
     |  3.5|[0.0, 2.0]|3.4999999999999996|
     +-----+----------+------------------+
 
     """
 
-    def __init__(self, **kwargs: Any) -> None:
+    @keyword_only
+    def __init__(
+        self,
+        *,
+        featuresCol: Union[str, List[str]] = "features",
+        labelCol: str = "label",
+        predictionCol: str = "prediction",
+        maxIter: int = 100,
+        regParam: float = 0.0,
+        elasticNetParam: float = 0.0,
+        tol: float = 1e-6,
+        fitIntercept: bool = True,
+        standardization: bool = True,
+        solver: str = "auto",
+        loss: str = "squaredError",
+        num_workers: Optional[int] = None,
+        verbose: Union[int, bool] = False,
+        **kwargs: Any,
+    ):
         super().__init__()
-        self.set_params(**kwargs)
+        self.set_params(**self._input_kwargs)
 
     def setMaxIter(self, value: int) -> "LinearRegression":
         """
         Sets the value of :py:attr:`maxIter`.
         """
         return self.set_params(maxIter=value)
 
@@ -314,109 +469,129 @@
             raise RuntimeError(
                 "LinearRegression doesn't support training data with 1 column"
             )
 
         return select_cols, multi_col_names, dimension, feature_type
 
     def _get_cuml_fit_func(
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
         def _linear_regression_fit(
-            dfs: CumlInputType,
+            dfs: FitInputType,
             params: Dict[str, Any],
         ) -> Dict[str, Any]:
-            init_parameters = params[param_alias.cuml_init]
-
+            # Step 1, get the PartitionDescriptor
             pdesc = PartitionDescriptor.build(
                 params[param_alias.part_sizes], params[param_alias.num_cols]
             )
 
-            if init_parameters["alpha"] == 0:
-                # LR
-                from cuml.linear_model.linear_regression_mg import (
-                    LinearRegressionMG as CumlLinearRegression,
-                )
-
-                supported_params = [
-                    "algorithm",
-                    "fit_intercept",
-                    "normalize",
-                    "verbose",
-                ]
-            else:
-                if init_parameters["l1_ratio"] == 0:
-                    # LR + L2
-                    from cuml.linear_model.ridge_mg import (
-                        RidgeMG as CumlLinearRegression,
+            def _single_fit(init_parameters: Dict[str, Any]) -> Dict[str, Any]:
+                if init_parameters["alpha"] == 0:
+                    # LR
+                    from cuml.linear_model.linear_regression_mg import (
+                        LinearRegressionMG as CumlLinearRegression,
                     )
 
                     supported_params = [
-                        "alpha",
-                        "solver",
+                        "algorithm",
                         "fit_intercept",
                         "normalize",
                         "verbose",
                     ]
-                    # spark ML normalizes sample portion of objective by the number of examples
-                    # but cuml does not for RidgeRegression (l1_ratio=0).   Induce similar behavior
-                    # to spark ml by scaling up the reg parameter by the number of examples.
-                    # With this, spark ML and spark rapids ML results match closely when features
-                    # and label columns are all standardized.
-                    init_parameters = init_parameters.copy()
-                    if "alpha" in init_parameters.keys():
-                        print(f"pdesc.m {pdesc.m}")
-                        init_parameters["alpha"] *= (float)(pdesc.m)
-
                 else:
-                    # LR + L1, or LR + L1 + L2
-                    # Cuml uses Coordinate Descent algorithm to implement Lasso and ElasticNet
-                    # So combine Lasso and ElasticNet here.
-                    from cuml.solvers.cd_mg import CDMG as CumlLinearRegression
-
-                    # in this case, both spark ML and cuml CD normalize sample portion of
-                    # objective by the number of training examples, so no need to adjust
-                    # reg params
-
-                    supported_params = [
-                        "loss",
-                        "alpha",
-                        "l1_ratio",
-                        "fit_intercept",
-                        "max_iter",
-                        "normalize",
-                        "tol",
-                        "shuffle",
-                        "verbose",
-                    ]
-
-            # filter only supported params
-            init_parameters = {
-                k: v for k, v in init_parameters.items() if k in supported_params
-            }
+                    if init_parameters["l1_ratio"] == 0:
+                        # LR + L2
+                        from cuml.linear_model.ridge_mg import (
+                            RidgeMG as CumlLinearRegression,
+                        )
+
+                        supported_params = [
+                            "alpha",
+                            "solver",
+                            "fit_intercept",
+                            "normalize",
+                            "verbose",
+                        ]
+                        # spark ML normalizes sample portion of objective by the number of examples
+                        # but cuml does not for RidgeRegression (l1_ratio=0).   Induce similar behavior
+                        # to spark ml by scaling up the reg parameter by the number of examples.
+                        # With this, spark ML and spark rapids ML results match closely when features
+                        # and label columns are all standardized.
+                        init_parameters = init_parameters.copy()
+                        if "alpha" in init_parameters.keys():
+                            init_parameters["alpha"] *= (float)(pdesc.m)
+
+                    else:
+                        # LR + L1, or LR + L1 + L2
+                        # Cuml uses Coordinate Descent algorithm to implement Lasso and ElasticNet
+                        # So combine Lasso and ElasticNet here.
+                        from cuml.solvers.cd_mg import CDMG as CumlLinearRegression
+
+                        # in this case, both spark ML and cuml CD normalize sample portion of
+                        # objective by the number of training examples, so no need to adjust
+                        # reg params
+
+                        supported_params = [
+                            "loss",
+                            "alpha",
+                            "l1_ratio",
+                            "fit_intercept",
+                            "max_iter",
+                            "normalize",
+                            "tol",
+                            "shuffle",
+                            "verbose",
+                        ]
+
+                # filter only supported params
+                final_init_parameters = {
+                    k: v for k, v in init_parameters.items() if k in supported_params
+                }
+
+                linear_regression = CumlLinearRegression(
+                    handle=params[param_alias.handle],
+                    output_type="cudf",
+                    **final_init_parameters,
+                )
 
-            linear_regression = CumlLinearRegression(
-                handle=params[param_alias.handle],
-                output_type="cudf",
-                **init_parameters,
-            )
+                linear_regression.fit(
+                    dfs,
+                    pdesc.m,
+                    pdesc.n,
+                    pdesc.parts_rank_size,
+                    pdesc.rank,
+                )
 
-            linear_regression.fit(
-                dfs,
-                pdesc.m,
-                pdesc.n,
-                pdesc.parts_rank_size,
-                pdesc.rank,
-            )
+                return {
+                    "coef_": linear_regression.coef_.to_numpy().tolist(),
+                    "intercept_": linear_regression.intercept_,
+                    "dtype": linear_regression.dtype.name,
+                    "n_cols": linear_regression.n_cols,
+                }
 
-            return {
-                "coef_": [linear_regression.coef_.to_numpy().tolist()],
-                "intercept_": linear_regression.intercept_,
-                "dtype": linear_regression.dtype.name,
-                "n_cols": linear_regression.n_cols,
-            }
+            init_parameters = params[param_alias.cuml_init]
+            fit_multiple_params = params[param_alias.fit_multiple_params]
+            if len(fit_multiple_params) == 0:
+                fit_multiple_params.append({})
+
+            models = []
+            for i in range(len(fit_multiple_params)):
+                tmp_params = init_parameters.copy()
+                tmp_params.update(fit_multiple_params[i])
+                models.append(_single_fit(tmp_params))
+
+            models_dict = {}
+            tc = TaskContext.get()
+            assert tc is not None
+            if tc.partitionId() == 0:
+                for k in models[0].keys():
+                    models_dict[k] = [m[k] for m in models]
+            return models_dict
 
         return _linear_regression_fit
 
     def _out_schema(self) -> Union[StructType, str]:
         return StructType(
             [
                 StructField("coef_", ArrayType(DoubleType(), False), False),
@@ -425,33 +600,41 @@
                 StructField("dtype", StringType(), False),
             ]
         )
 
     def _create_pyspark_model(self, result: Row) -> "LinearRegressionModel":
         return LinearRegressionModel.from_row(result)
 
+    def _enable_fit_multiple_in_single_pass(self) -> bool:
+        return True
+
+    def _supportsTransformEvaluate(self, evaluator: Evaluator) -> bool:
+        return True if isinstance(evaluator, RegressionEvaluator) else False
+
 
 class LinearRegressionModel(
     LinearRegressionClass,
-    _CumlModelSupervised,
+    _CumlModelWithPredictionCol,
     _LinearRegressionCumlParams,
+    _RegressionModelEvaluationMixIn,
 ):
     """Model fitted by :class:`LinearRegression`."""
 
     def __init__(
         self,
-        coef_: List[float],
-        intercept_: float,
+        coef_: Union[List[float], List[List[float]]],
+        intercept_: Union[float, List[float]],
         n_cols: int,
         dtype: str,
     ) -> None:
         super().__init__(dtype=dtype, n_cols=n_cols, coef_=coef_, intercept_=intercept_)
         self.coef_ = coef_
         self.intercept_ = intercept_
         self._lr_ml_model: Optional[SparkLinearRegressionModel] = None
+        self._this_model = self
 
     def cpu(self) -> SparkLinearRegressionModel:
         """Return the PySpark ML LinearRegressionModel"""
         if self._lr_ml_model is None:
             sc = _get_spark_session().sparkContext
             assert sc._jvm is not None
 
@@ -467,28 +650,30 @@
 
     @property
     def coefficients(self) -> Vector:
         """
         Model coefficients.
         """
         # TBD: for large enough dimension, SparseVector is returned. Need to find out how to match
-        return Vectors.dense(self.coef_)
+        assert not isinstance(self.coef_[0], list)
+        return Vectors.dense(cast(list, self.coef_))
 
     @property
     def hasSummary(self) -> bool:
         """
         Indicates whether a training summary exists for this model instance.
         """
         return False
 
     @property
     def intercept(self) -> float:
         """
         Model intercept.
         """
+        assert not isinstance(self.intercept_, list)
         return self.intercept_
 
     @property
     def scale(self) -> float:
         """
         Since "huber" loss is not supported by cuML, just returns the value 1.0 for API compatibility.
         """
@@ -501,40 +686,88 @@
 
     def evaluate(self, dataset: DataFrame) -> LinearRegressionSummary:
         """cuML doesn't support evaluating.
         Fall back to PySpark ML LinearRegressionModel"""
         return self.cpu().evaluate(dataset)
 
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         coef_ = self.coef_
         intercept_ = self.intercept_
         n_cols = self.n_cols
         dtype = self.dtype
 
         def _construct_lr() -> CumlT:
             from cuml.linear_model.linear_regression_mg import LinearRegressionMG
 
-            lr = LinearRegressionMG(output_type="numpy")
-            lr.coef_ = cudf_to_cuml_array(np.array(coef_, order="F").astype(dtype))
-            lr.intercept_ = intercept_
-            lr.n_cols = n_cols
-            lr.dtype = np.dtype(dtype)
+            lrs = []
 
-            return lr
+            coefs = coef_ if isinstance(intercept_, list) else [coef_]
+            intercepts = intercept_ if isinstance(intercept_, list) else [intercept_]
 
-        def _predict(lr: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
+            for i in range(len(coefs)):
+                lr = LinearRegressionMG(output_type="numpy")
+                lr.coef_ = cudf_to_cuml_array(
+                    np.array(coefs[i], order="F").astype(dtype)
+                )
+                lr.intercept_ = intercepts[i]
+                lr.n_cols = n_cols
+                lr.dtype = np.dtype(dtype)
+                lrs.append(lr)
+
+            return lrs
+
+        def _predict(lr: CumlT, pdf: TransformInputType) -> pd.Series:
             ret = lr.predict(pdf)
             return pd.Series(ret)
 
-        return _construct_lr, _predict
+        return _construct_lr, _predict, self.calculate_regression_metrics
+
+    def _transform(self, dataset: DataFrame) -> DataFrame:
+        df = super()._transform(dataset)
+        return df.withColumn(
+            self.getPredictionCol(), df[self.getPredictionCol()].cast("double")
+        )
+
+    @classmethod
+    def _combine(
+        cls: Type["LinearRegressionModel"], models: List["LinearRegressionModel"]  # type: ignore
+    ) -> "LinearRegressionModel":
+        assert len(models) > 0 and all(isinstance(model, cls) for model in models)
+        first_model = models[0]
+
+        # Combine coef and intercepts
+        coefs = cast(list, [model.coef_ for model in models])
+        intercepts = cast(list, [model.intercept_ for model in models])
+
+        assert first_model.n_cols is not None
+        assert first_model.dtype is not None
+
+        lr_model = cls(
+            n_cols=first_model.n_cols,
+            dtype=first_model.dtype,
+            coef_=coefs,
+            intercept_=intercepts,
+        )
+        first_model._copyValues(lr_model)
+        first_model._copy_cuml_params(lr_model)
+
+        return lr_model
+
+    def _transformEvaluate(
+        self,
+        dataset: DataFrame,
+        evaluator: Evaluator,
+        params: Optional["ParamMap"] = None,
+    ) -> List[float]:
+        num_models = len(self.intercept_) if isinstance(self.intercept_, list) else 1
+        return self._transform_evaluate(
+            dataset=dataset, evaluator=evaluator, num_models=num_models, params=params
+        )
 
 
 class _RandomForestRegressorClass(_RandomForestClass):
     @classmethod
     def _param_value_mapping(
         cls,
     ) -> Dict[str, Callable[[str], Union[None, str, float, int]]]:
@@ -549,31 +782,103 @@
     _RandomForestRegressorClass,
     _RandomForestEstimator,
     _RandomForestCumlParams,
     _RandomForestRegressorParams,
 ):
     """RandomForestRegressor implements a Random Forest regressor model which
     fits multiple decision tree in an ensemble. It implements cuML's
-    GPU accelerated RandomForestRegressor algorithm based on cuML python library,\
+    GPU accelerated RandomForestRegressor algorithm based on cuML python library,
     and it can be used in PySpark Pipeline and PySpark ML meta algorithms like
-    :py:class:`~pyspark.ml.tuning.CrossValidator`/
-    :py:class:`~pyspark.ml.tuning.TrainValidationSplit`/
+    :py:class:`~pyspark.ml.tuning.CrossValidator`,
+    :py:class:`~pyspark.ml.tuning.TrainValidationSplit`,
     :py:class:`~pyspark.ml.classification.OneVsRest`
 
     The distributed algorithm uses an *embarrassingly-parallel* approach. For a
     forest with `N` trees being built on `w` workers, each worker simply builds `N/w`
     trees on the data it has available locally. In many cases, partitioning the
     data so that each worker builds trees on a subset of the total dataset works
     well, but it generally requires the data to be well-shuffled in advance.
 
     RandomForestRegressor automatically supports most of the parameters from both
-    :py:class:`~pyspark.ml.regression.RandomForestRegressor` and in the constructors of
+    :py:class:`~pyspark.ml.regression.RandomForestRegressor` and
     :py:class:`cuml.ensemble.RandomForestRegressor`. And it can automatically map
     pyspark parameters to cuML parameters.
 
+
+    Parameters
+    ----------
+
+    featuresCol:
+        The feature column names, spark-rapids-ml supports vector, array and columnar as the input.\n
+            * When the value is a string, the feature columns must be assembled into 1 column with vector or array type.
+            * When the value is a list of strings, the feature columns must be numeric types.
+    labelCol:
+        The label column name.
+    predictionCol:
+        The prediction column name.
+    maxDepth:
+        Maximum tree depth. Must be greater than 0.
+    maxBins:
+        Maximum number of bins used by the split algorithm per feature.
+    minInstancesPerNode:
+        The minimum number of samples (rows) in each leaf node.
+    impurity: str = "variance",
+        The criterion used to split nodes.
+    numTrees:
+        Total number of trees in the forest.
+    featureSubsetStrategy:
+        Ratio of number of features (columns) to consider per node split.\n
+        The supported options:\n
+            ``'auto'``:  If numTrees == 1, set to 'all', If numTrees > 1 (forest), set to 'onethird'\n
+            ``'all'``: use all features\n
+            ``'onethird'``: use 1/3 of the features\n
+            ``'sqrt'``: use sqrt(number of features)\n
+            ``'log2'``: log2(number of features)\n
+            ``'n'``: when n is in the range (0, 1.0], use n * number of features. When n
+            is in the range (1, number of features), use n features.
+    seed:
+        Seed for the random number generator.
+    bootstrap:
+        Control bootstrapping.\n
+            * If ``True``, each tree in the forest is built on a bootstrapped
+              sample with replacement.
+            * If ``False``, the whole dataset is used to build each tree.
+    num_workers:
+        Number of cuML workers, where each cuML worker corresponds to one Spark task
+        running on one GPU. If not set, spark-rapids-ml tries to infer the number of
+        cuML workers (i.e. GPUs in cluster) from the Spark environment.
+    verbose:
+        Logging level.
+            * ``0`` - Disables all log messages.
+            * ``1`` - Enables only critical messages.
+            * ``2`` - Enables all messages up to and including errors.
+            * ``3`` - Enables all messages up to and including warnings.
+            * ``4 or False`` - Enables all messages up to and including information messages.
+            * ``5 or True`` - Enables all messages up to and including debug messages.
+            * ``6`` - Enables all messages up to and including trace messages.
+    n_streams:
+        Number of parallel streams used for forest building.
+        Please note that there is a bug running spark-rapids-ml on a node with multi-gpus
+        when n_streams > 1. See https://github.com/rapidsai/cuml/issues/5402.
+    min_samples_split:
+        The minimum number of samples required to split an internal node.\n
+         * If type ``int``, then ``min_samples_split`` represents the minimum
+           number.
+         * If type ``float``, then ``min_samples_split`` represents a fraction
+           and ``ceil(min_samples_split * n_rows)`` is the minimum number of
+           samples for each split.    max_samples:
+        Ratio of dataset rows used while fitting each tree.
+    max_leaves:
+        Maximum leaf nodes per tree. Soft constraint. Unlimited, if -1.
+    min_impurity_decrease:
+        Minimum decrease in impurity required for node to be split.
+    max_batch_size:
+        Maximum number of nodes that can be processed in a given batch.
+
+
     Examples
     --------
     >>> from spark_rapids_ml.regression import RandomForestRegressor, RandomForestRegressionModel
     >>> from numpy import allclose
     >>> from pyspark.ml.linalg import Vectors
     >>> df = spark.createDataFrame([
     ...     (1.0, Vectors.dense(1.0)),
@@ -606,50 +911,78 @@
     >>> model.save(model_path)
     >>> model2 = RandomForestRegressionModel.load(model_path)
     >>> model.transform(test0).take(1) == model2.transform(test0).take(1)
     True
 
     """
 
-    def __init__(self, **kwargs: Any):
-        super().__init__()
-        self.set_params(**kwargs)
+    @keyword_only
+    def __init__(
+        self,
+        *,
+        featuresCol: Union[str, List[str]] = "features",
+        labelCol: str = "label",
+        predictionCol: str = "prediction",
+        maxDepth: int = 5,
+        maxBins: int = 32,
+        minInstancesPerNode: int = 1,
+        impurity: str = "variance",
+        numTrees: int = 20,
+        featureSubsetStrategy: str = "auto",
+        seed: Optional[int] = None,
+        bootstrap: Optional[bool] = True,
+        num_workers: Optional[int] = None,
+        verbose: Union[int, bool] = False,
+        n_streams: int = 1,
+        min_samples_split: Union[int, float] = 2,
+        max_samples: float = 1.0,
+        max_leaves: int = -1,
+        min_impurity_decrease: float = 0.0,
+        max_batch_size: int = 4096,
+        **kwargs: Any,
+    ):
+        super().__init__(**self._input_kwargs)
 
     def _is_classification(self) -> bool:
         return False
 
     def _create_pyspark_model(self, result: Row) -> "RandomForestRegressionModel":
         return RandomForestRegressionModel.from_row(result)
 
+    def _supportsTransformEvaluate(self, evaluator: Evaluator) -> bool:
+        return True if isinstance(evaluator, RegressionEvaluator) else False
+
 
 class RandomForestRegressionModel(
     _RandomForestRegressorClass,
     _RandomForestModel,
     _RandomForestCumlParams,
     _RandomForestRegressorParams,
+    _RegressionModelEvaluationMixIn,
 ):
     """
     Model fitted by :class:`RandomForestRegressor`.
     """
 
     def __init__(
         self,
         n_cols: int,
         dtype: str,
-        treelite_model: str,
-        model_json: List[str],
+        treelite_model: Union[str, List[str]],
+        model_json: Union[List[str], List[List[str]]] = [],  # type: ignore
     ):
         super().__init__(
             dtype=dtype,
             n_cols=n_cols,
             treelite_model=treelite_model,
             model_json=model_json,
         )
 
         self._rf_spark_model: Optional[SparkRandomForestRegressionModel] = None
+        self._this_model = self
 
     def cpu(self) -> SparkRandomForestRegressionModel:
         """Return the PySpark ML RandomForestRegressionModel"""
 
         if self._rf_spark_model is None:
             sc = _get_spark_session().sparkContext
             assert sc._jvm is not None
@@ -665,7 +998,44 @@
             )
             self._rf_spark_model = SparkRandomForestRegressionModel(java_rf_model)
             self._copyValues(self._rf_spark_model)
         return self._rf_spark_model
 
     def _is_classification(self) -> bool:
         return False
+
+    def _get_cuml_transform_func(
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
+        _construct_rf, _predict, _ = super()._get_cuml_transform_func(dataset, category)
+        return _construct_rf, _predict, self.calculate_regression_metrics
+
+    def _transformEvaluate(
+        self,
+        dataset: DataFrame,
+        evaluator: Evaluator,
+        params: Optional["ParamMap"] = None,
+    ) -> List[float]:
+        """
+        Transforms and evaluates the input dataset with optional parameters in a single pass.
+
+        Parameters
+        ----------
+        dataset : :py:class:`pyspark.sql.DataFrame`
+            a dataset that contains labels/observations and predictions
+        evaluator: :py:class:`pyspark.ml.evaluation.Evaluator`
+            an evaluator user intends to use
+        params : dict, optional
+            an optional param map that overrides embedded params
+
+        Returns
+        -------
+        list of float
+            metrics
+        """
+
+        num_models = (
+            len(self._treelite_model) if isinstance(self._treelite_model, list) else 1
+        )
+        return self._transform_evaluate(
+            dataset=dataset, evaluator=evaluator, num_models=num_models, params=params
+        )
```

## spark_rapids_ml/tree.py

```diff
@@ -14,28 +14,15 @@
 # limitations under the License.
 #
 import base64
 import json
 import math
 import pickle
 from abc import abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
-
-if TYPE_CHECKING:
-    import cudf
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast
 
 import numpy as np
 import pandas as pd
 from pyspark.ml.classification import DecisionTreeClassificationModel
 from pyspark.ml.classification import (
     RandomForestClassificationModel as SparkRandomForestClassificationModel,
 )
@@ -51,19 +38,24 @@
     IntegerType,
     StringType,
     StructField,
     StructType,
 )
 
 from .core import (
-    CumlInputType,
     CumlT,
+    FitInputType,
+    TransformInputType,
+    _ConstructFunc,
     _CumlEstimatorSupervised,
-    _CumlModelSupervised,
+    _CumlModelWithPredictionCol,
+    _EvaluateFunc,
+    _TransformFunc,
     param_alias,
+    transform_evaluate,
 )
 from .params import HasFeaturesCols, P, _CumlClass, _CumlParams
 from .utils import (
     _concat_and_free,
     _get_spark_session,
     _str_or_numerical,
     java_uid,
@@ -177,143 +169,236 @@
     def setLabelCol(self: P, value: str) -> P:
         """
         Sets the value of :py:attr:`labelCol`.
         """
         self._set(labelCol=value)  # type: ignore
         return self
 
+    def setPredictionCol(self: P, value: str) -> P:
+        """
+        Sets the value of :py:attr:`predictionCol`.
+        """
+        self._set(predictionCol=value)  # type: ignore
+        return self
+
+
+class _RandomForestEstimatorParams(_RandomForestCumlParams):
+    def __init__(self) -> None:
+        super().__init__()
+
+    # include setters used only in estimator classes (classifier and regressor) here
+    def setBootstrap(self: P, value: bool) -> P:
+        """
+        Sets the value of :py:attr:`bootstrap`.
+        """
+        return self.set_params(bootstrap=value)
+
+    def setFeatureSubsetStrategy(self: P, value: str) -> P:
+        """
+        Sets the value of :py:attr:`featureSubsetStrategy`.
+        """
+        return self.set_params(featureSubsetStrategy=value)
+
+    def setImpurity(self: P, value: str) -> P:
+        """
+        Sets the value of :py:attr:`impurity`.
+        """
+        return self.set_params(impurity=value)  # type: ignore
+
+    def setMaxBins(self: P, value: int) -> P:
+        """
+        Sets the value of :py:attr:`maxBins`.
+        """
+        return self.set_params(maxBins=value)
+
+    def setMaxDepth(self: P, value: int) -> P:
+        """
+        Sets the value of :py:attr:`maxDepth`.
+        """
+        return self.set_params(maxDepth=value)
+
+    def setMinInstancesPerNode(self: P, value: int) -> P:
+        """
+        Sets the value of :py:attr:`minInstancesPerNode`.
+        """
+        return self.set_params(minInstancesPerNode=value)
+
+    def setNumTrees(self: P, value: int) -> P:
+        """
+        Sets the value of :py:attr:`numTrees`.
+        """
+        return self.set_params(numTrees=value)
+
     def setSeed(self: P, value: int) -> P:
+        """
+        Sets the value of :py:attr:`seed`.
+        """
         if value > 0x07FFFFFFF:
             raise ValueError("cuML seed value must be a 32-bit integer.")
         return self.set_params(seed=value)
 
 
 class _RandomForestEstimator(
     _CumlEstimatorSupervised,
-    _RandomForestCumlParams,
+    _RandomForestEstimatorParams,
 ):
     def __init__(self, **kwargs: Any):
         super().__init__()
         self.set_params(**kwargs)
         if "n_streams" not in kwargs:
             # cuML will throw exception when running on a node with multi-gpus when n_streams > 0
             self._set_cuml_value("n_streams", 1)
 
     @abstractmethod
     def _is_classification(self) -> bool:
         """Indicate if it is regression or classification estimator"""
         raise NotImplementedError()
 
-    def _estimators_per_worker(self) -> List[int]:
+    def _estimators_per_worker(self, n_estimators: int) -> List[int]:
         """Calculate the number of trees each task should train according to n_estimators"""
-        n_estimators = self.cuml_params["n_estimators"]
         n_workers = self.num_workers
         if n_estimators < n_workers:
             raise ValueError("n_estimators cannot be lower than number of spark tasks.")
 
         n_est_per_worker = math.floor(n_estimators / n_workers)
         n_estimators_per_worker = [n_est_per_worker for i in range(n_workers)]
         remaining_est = n_estimators - (n_est_per_worker * n_workers)
         for i in range(remaining_est):
             n_estimators_per_worker[i] = n_estimators_per_worker[i] + 1
         return n_estimators_per_worker
 
     def _get_cuml_fit_func(
-        self, dataset: DataFrame
-    ) -> Callable[[CumlInputType, Dict[str, Any]], Dict[str, Any],]:
-        n_estimators_per_worker = self._estimators_per_worker()
+        self,
+        dataset: DataFrame,
+        extra_params: Optional[List[Dict[str, Any]]] = None,
+    ) -> Callable[[FitInputType, Dict[str, Any]], Dict[str, Any],]:
+        # Each element of n_estimators_of_all_params is a list value which
+        # is composed of n_estimators per worker.
+        n_estimators_of_all_params: List[List[int]] = []
+        total_trees: List[int] = []
+
+        all_params = [{}] if extra_params is None else extra_params
+
+        for params in all_params:
+            num_trees = (
+                self.cuml_params["n_estimators"]
+                if "n_estimators" not in params
+                else params["n_estimators"]
+            )
+            n_estimators_of_all_params.append(self._estimators_per_worker(num_trees))
+            total_trees.append(num_trees)
 
         is_classification = self._is_classification()
 
-        total_trees = self.cuml_params["n_estimators"]
-
         def _rf_fit(
-            dfs: CumlInputType,
+            dfs: FitInputType,
             params: Dict[str, Any],
         ) -> Dict[str, Any]:
+            X_list = [item[0] for item in dfs]
+            y_list = [item[1] for item in dfs]
+            if isinstance(X_list[0], pd.DataFrame):
+                X = pd.concat(X_list)
+                y = pd.concat(y_list)
+            else:
+                # features are either cp or np arrays here
+                X = _concat_and_free(X_list)
+                y = _concat_and_free(y_list)
+
+            if is_classification:
+                from cuml import RandomForestClassifier as cuRf
+            else:
+                from cuml import RandomForestRegressor as cuRf
+
             from pyspark import BarrierTaskContext
 
             context = BarrierTaskContext.get()
             part_id = context.partitionId()
 
-            rf_params = params[param_alias.cuml_init]
-            rf_params.pop("n_estimators")
+            def _single_fit(rf: cuRf) -> Dict[str, Any]:
+                # Fit a random forest model on the dataset (X, y)
+                rf.fit(X, y, convert_dtype=False)
+
+                # serialized_model is Dictionary type
+                serialized_model = rf._get_serialized_model()
+                pickled_model = pickle.dumps(serialized_model)
+                msg = base64.b64encode(pickled_model).decode("utf-8")
+                trees = rf.get_json()
+                data = {"model_bytes": msg, "model_json": trees}
+                messages = context.allGather(json.dumps(data))
+
+                # concatenate the random forest in the worker0
+                if part_id == 0:
+                    mod_bytes = []
+                    mod_jsons = []
+                    for msg in messages:
+                        data = json.loads(msg)
+                        mod_bytes.append(
+                            pickle.loads(base64.b64decode(data["model_bytes"]))
+                        )
+                        mod_jsons.append(data["model_json"])
+
+                    all_tl_mod_handles = [
+                        rf._tl_handle_from_bytes(i) for i in mod_bytes
+                    ]
+                    rf._concatenate_treelite_handle(all_tl_mod_handles)
+
+                    from cuml.fil.fil import TreeliteModel
+
+                    for tl_handle in all_tl_mod_handles:
+                        TreeliteModel.free_treelite_model(tl_handle)
+
+                    final_model_bytes = pickle.dumps(rf._get_serialized_model())
+                    final_model = base64.b64encode(final_model_bytes).decode("utf-8")
+                    result = {
+                        "treelite_model": final_model,
+                        "dtype": rf.dtype.name,
+                        "n_cols": rf.n_cols,
+                        "model_json": mod_jsons,
+                    }
+
+                    if is_classification:
+                        result["num_classes"] = rf.num_classes
 
-            if rf_params["max_features"] == "auto":
-                if total_trees == 1:
-                    rf_params["max_features"] = 1.0
+                    return result
                 else:
-                    rf_params["max_features"] = (
-                        "sqrt" if is_classification else (1 / 3.0)
-                    )
+                    return {}
 
-            if is_classification:
-                from cuml import RandomForestClassifier as cuRf
-            else:
-                from cuml import RandomForestRegressor as cuRf
+            rf_params = params[param_alias.cuml_init]
+            fit_multiple_params = params[param_alias.fit_multiple_params]
 
-            rf = cuRf(
-                n_estimators=n_estimators_per_worker[part_id],
-                output_type="cudf",
-                **rf_params,
-            )
+            if len(fit_multiple_params) == 0:
+                fit_multiple_params.append({})
 
-            X_list = [item[0] for item in dfs]
-            y_list = [item[1] for item in dfs]
-            if isinstance(X_list[0], pd.DataFrame):
-                X = pd.concat(X_list)
-                y = pd.concat(y_list)
-            else:
-                # should be list of np.ndarrays here
-                X = _concat_and_free(cast(List[np.ndarray], X_list))
-                y = _concat_and_free(cast(List[np.ndarray], y_list))
-
-            # Fit a random forest model on the dataset (X, y)
-            rf.fit(X, y, convert_dtype=False)
-
-            # serialized_model is Dictionary type
-            serialized_model = rf._get_serialized_model()
-            pickled_model = pickle.dumps(serialized_model)
-            msg = base64.b64encode(pickled_model).decode("utf-8")
-            trees = rf.get_json()
-            data = {"model_bytes": msg, "model_json": trees}
-            messages = context.allGather(json.dumps(data))
+            models = []
+            for i in range(len(fit_multiple_params)):
+                tmp_rf_params = rf_params.copy()
+                tmp_rf_params.update(fit_multiple_params[i])
+                tmp_rf_params.pop("n_estimators")
+
+                if tmp_rf_params["max_features"] == "auto":
+                    if total_trees[i] == 1:
+                        tmp_rf_params["max_features"] = 1.0
+                    else:
+                        tmp_rf_params["max_features"] = (
+                            "sqrt" if is_classification else (1 / 3.0)
+                        )
+                rf = cuRf(
+                    n_estimators=n_estimators_of_all_params[i][part_id],
+                    output_type="cudf",
+                    **tmp_rf_params,
+                )
+                models.append(_single_fit(rf))
+                del rf
+
+            models_dict = {}
 
-            # concatenate the random forest in the worker0
             if part_id == 0:
-                mod_bytes = []
-                mod_jsons = []
-                for msg in messages:
-                    data = json.loads(msg)
-                    mod_bytes.append(
-                        pickle.loads(base64.b64decode(data["model_bytes"]))
-                    )
-                    mod_jsons.append(data["model_json"])
-
-                all_tl_mod_handles = [rf._tl_handle_from_bytes(i) for i in mod_bytes]
-                rf._concatenate_treelite_handle(all_tl_mod_handles)
-
-                from cuml.fil.fil import TreeliteModel
-
-                for tl_handle in all_tl_mod_handles:
-                    TreeliteModel.free_treelite_model(tl_handle)
-
-                final_model_bytes = pickle.dumps(rf._get_serialized_model())
-                final_model = base64.b64encode(final_model_bytes).decode("utf-8")
-                result = {
-                    "treelite_model": [final_model],
-                    "dtype": rf.dtype.name,
-                    "n_cols": rf.n_cols,
-                    "model_json": [mod_jsons],
-                }
-                if is_classification:
-                    result["num_classes"] = rf.num_classes
-                return result
-            else:
-                return {}
+                for k in models[0].keys():
+                    models_dict[k] = [m[k] for m in models]
+            return models_dict
 
         return _rf_fit
 
     def _out_schema(self) -> Union[StructType, str]:
         fields = [
             StructField("treelite_model", StringType(), False),
             StructField("n_cols", IntegerType(), False),
@@ -324,25 +409,28 @@
             fields.append(StructField("num_classes", IntegerType(), False))
 
         return StructType(fields)
 
     def _require_nccl_ucx(self) -> Tuple[bool, bool]:
         return False, False
 
+    def _enable_fit_multiple_in_single_pass(self) -> bool:
+        return True
+
 
 class _RandomForestModel(
-    _CumlModelSupervised,
+    _CumlModelWithPredictionCol,
     _RandomForestCumlParams,
 ):
     def __init__(
         self,
         n_cols: int,
         dtype: str,
-        treelite_model: str,
-        model_json: List[str] = [],
+        treelite_model: Union[str, List[str]],
+        model_json: Union[List[str], List[List[str]]] = [],  # type: ignore
         num_classes: int = -1,  # only for classification
     ):
         if self._is_classification():
             super().__init__(
                 dtype=dtype,
                 n_cols=n_cols,
                 treelite_model=treelite_model,
@@ -418,18 +506,21 @@
 
     def _convert_to_java_trees(self, impurity: str) -> Tuple[Any, List[Any]]:
         """Convert cuml trees to Java decision tree model"""
         sc = _get_spark_session().sparkContext
         assert sc._jvm is not None
         assert sc._gateway is not None
 
+        # This function shouldn't be called for the multiple models scenario.
+        model_json = cast(List[str], self._model_json)
+
         # Convert cuml trees to Spark trees
         trees = [
             translate_trees(sc, impurity, trees)
-            for trees_json in self._model_json
+            for trees_json in model_json
             for trees in json.loads(trees_json)
         ]
 
         if self._is_classification():
             uid = java_uid(sc, "rfc")
             java_decision_tree_model_class = (
                 sc._jvm.org.apache.spark.ml.classification.DecisionTreeClassificationModel
@@ -457,36 +548,60 @@
         )
         for i in range(len(decision_trees)):
             java_trees[i] = decision_trees[i]
 
         return uid, java_trees
 
     def _get_cuml_transform_func(
-        self, dataset: DataFrame
-    ) -> Tuple[
-        Callable[..., CumlT],
-        Callable[[CumlT, Union["cudf.DataFrame", np.ndarray]], pd.DataFrame],
-    ]:
+        self, dataset: DataFrame, category: str = transform_evaluate.transform
+    ) -> Tuple[_ConstructFunc, _TransformFunc, Optional[_EvaluateFunc],]:
         treelite_model = self._treelite_model
-
         is_classification = self._is_classification()
 
         def _construct_rf() -> CumlT:
-            model = pickle.loads(base64.b64decode(treelite_model))
-
             if is_classification:
                 from cuml import RandomForestClassifier as cuRf
             else:
                 from cuml import RandomForestRegressor as cuRf
 
-            rf = cuRf()
-            rf._concatenate_treelite_handle([rf._tl_handle_from_bytes(model)])
+            rfs = []
+            treelite_models = (
+                treelite_model if isinstance(treelite_model, list) else [treelite_model]
+            )
+            for m in treelite_models:
+                model = pickle.loads(base64.b64decode(m))
+                rf = cuRf()
+                rf._concatenate_treelite_handle([rf._tl_handle_from_bytes(model)])
+                rfs.append(rf)
 
-            return rf
+            return rfs
 
-        def _predict(rf: CumlT, pdf: Union["cudf.DataFrame", np.ndarray]) -> pd.Series:
+        def _predict(rf: CumlT, pdf: TransformInputType) -> pd.Series:
             rf.update_labels = False
             ret = rf.predict(pdf)
             return pd.Series(ret)
 
         # TBD: figure out why RF algo's warns regardless of what np array order is set
-        return _construct_rf, _predict
+        return _construct_rf, _predict, None
+
+    def _transform(self, dataset: DataFrame) -> DataFrame:
+        df = super()._transform(dataset)
+        return df.withColumn(
+            self.getPredictionCol(), df[self.getPredictionCol()].cast("double")
+        )
+
+    @classmethod
+    def _combine(
+        cls: Type["_RandomForestModel"], models: List["_RandomForestModel"]  # type: ignore
+    ) -> "_RandomForestModel":
+        assert len(models) > 0 and all(isinstance(model, cls) for model in models)
+        first_model = models[0]
+        treelite_models = [model._treelite_model for model in models]
+        model_jsons = [model._model_json for model in models]
+        attrs = first_model.get_model_attributes()
+        assert attrs is not None
+        attrs["treelite_model"] = treelite_models
+        attrs["model_json"] = model_jsons
+        rf_model = cls(**attrs)
+        first_model._copyValues(rf_model)
+        first_model._copy_cuml_params(rf_model)
+        return rf_model
```

## spark_rapids_ml/utils.py

```diff
@@ -12,26 +12,55 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import inspect
 import logging
 import sys
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Set, Tuple, Union
 
 if TYPE_CHECKING:
     import cudf
+    import cupy as cp
 
 import numpy as np
 from pyspark import BarrierTaskContext, SparkContext, TaskContext
 from pyspark.sql import SparkSession
 
 _ArrayOrder = Literal["C", "F"]
 
 
+def _method_names_from_param(spark_param_name: str) -> List[str]:
+    """
+    Returns getter and setter method names, per Spark ML conventions, for passed in attribute.
+    """
+    cap = spark_param_name[0].upper() + spark_param_name[1:]
+    getter = f"get{cap}"
+    setter = f"set{cap}"
+    return [getter, setter]
+
+
+def _unsupported_methods_attributes(clazz: Any) -> Set[str]:
+    """
+    Returns set of methods and attributes not supported by spark-rapids-ml for passed in class
+    as determined from empty values in the dictionary returned by _param_mapping() invoked on the class.
+    """
+    if "_param_mapping" in [
+        member_name for member_name, _ in inspect.getmembers(clazz, inspect.ismethod)
+    ]:
+        param_map = clazz._param_mapping()
+        _unsupported_params = [k for k, v in param_map.items() if not v]
+        _unsupported_methods: List[str] = sum(
+            [_method_names_from_param(k) for k in _unsupported_params], []
+        )
+        return set(_unsupported_params + _unsupported_methods)
+    else:
+        return set()
+
+
 def _get_spark_session() -> SparkSession:
     """Get or create spark session.
     Note: This function can only be invoked from driver side."""
     if TaskContext.get() is not None:
         # safety check.
         raise RuntimeError(
             "_get_spark_session should not be invoked from executor side."
@@ -57,24 +86,45 @@
         except:
             _x = x
     return _x
 
 
 def _get_gpu_id(task_context: TaskContext) -> int:
     """Get the gpu id from the task resources"""
-    if task_context is None:
-        # safety check.
-        raise RuntimeError("_get_gpu_id should not be invoked from driver side.")
-    resources = task_context.resources()
-    if "gpu" not in resources:
-        raise RuntimeError(
-            "Couldn't get the gpu id, Please check the GPU resource configuration."
+    import os
+
+    if "CUDA_VISIBLE_DEVICES" in os.environ:
+        if os.environ["CUDA_VISIBLE_DEVICES"]:
+            num_assigned = len(os.environ["CUDA_VISIBLE_DEVICES"].split(","))
+            # when CUDA_VISIBLE_DEVICES is set and non-empty, use 0-th index entry
+            gpu_id = 0
+        else:
+            raise RuntimeError(
+                "Couldn't get gpu id since CUDA_VISIBLE_DEVICES is set to an empty string.  Please check the GPU resource configuration."
+            )
+    else:
+        if task_context is None:
+            # safety check.
+            raise RuntimeError("_get_gpu_id should not be invoked from driver side.")
+        resources = task_context.resources()
+        if "gpu" not in resources:
+            raise RuntimeError(
+                "Couldn't get the gpu id, Please check the GPU resource configuration."
+            )
+        num_assigned = len(resources["gpu"].addresses)
+        # return the first gpu id.
+        gpu_id = int(resources["gpu"].addresses[0].strip())
+
+    if num_assigned > 1:
+        logger = get_logger(_get_gpu_id)
+        logger.warn(
+            f"Task got assigned {num_assigned} GPUs but using only 1.  This could be a waste of GPU resources."
         )
-    # return the first gpu id.
-    return int(resources["gpu"].addresses[0].strip())
+
+    return gpu_id
 
 
 def _get_default_params_from_func(
     func: Callable, unsupported_set: List[str] = []
 ) -> Dict[str, Any]:
     """
     Returns a dictionary of parameters and their default value of function fn.
@@ -88,19 +138,19 @@
             parameter.default is not parameter.empty
             and parameter.name not in unsupported_set
         ):
             filtered_params_dict[parameter.name] = parameter.default
     return filtered_params_dict
 
 
-def _get_class_name(cls: type) -> str:
+def _get_class_or_callable_name(cls_or_callable: Union[type, Callable]) -> str:
     """
     Return the class name.
     """
-    return f"{cls.__module__}.{cls.__name__}"
+    return f"{cls_or_callable.__module__}.{cls_or_callable.__name__}"
 
 
 class PartitionDescriptor:
     """
     Partition descriptor
 
     m: total number of rows across all workers
@@ -136,31 +186,35 @@
         parts_rank_size = [item for pair in messages for item in json.loads(pair)]
         total_rows = sum(pair[1] for pair in parts_rank_size)
 
         return cls(total_rows, total_cols, rank, parts_rank_size)
 
 
 def _concat_and_free(
-    np_array_list: List[np.ndarray], order: _ArrayOrder = "F"
-) -> np.ndarray:
+    array_list: Union[List["cp.ndarray"], List[np.ndarray]], order: _ArrayOrder = "F"
+) -> Union["cp.ndarray", np.ndarray]:
     """
     concatenates a list of compatible numpy arrays into a 'order' ordered output array,
     in a memory efficient way.
     Note: frees list elements so do not reuse after calling.
     """
-    rows = sum(arr.shape[0] for arr in np_array_list)
-    if len(np_array_list[0].shape) > 1:
-        cols = np_array_list[0].shape[1]
+    import cupy as cp
+
+    array_module = cp if isinstance(array_list[0], cp.ndarray) else np
+
+    rows = sum(arr.shape[0] for arr in array_list)
+    if len(array_list[0].shape) > 1:
+        cols = array_list[0].shape[1]
         concat_shape: Tuple[int, ...] = (rows, cols)
     else:
         concat_shape = (rows,)
-    d_type = np_array_list[0].dtype
-    concated = np.empty(shape=concat_shape, order=order, dtype=d_type)
-    np.concatenate(np_array_list, out=concated)
-    del np_array_list[:]
+    d_type = array_list[0].dtype
+    concated = array_module.empty(shape=concat_shape, order=order, dtype=d_type)
+    array_module.concatenate(array_list, out=concated)
+    del array_list[:]
     return concated
 
 
 def cudf_to_cuml_array(gdf: Union["cudf.DataFrame", "cudf.Series"], order: str = "F"):  # type: ignore
     try:
         # Compatible with older cuml version (before 23.02)
         from cuml.common.input_utils import input_to_cuml_array
@@ -182,17 +236,19 @@
     elif dtype == np.int16:
         return "short"
     else:
         raise RuntimeError("Unsupported dtype, found ", dtype)
 
 
 # similar to https://github.com/dmlc/xgboost/blob/master/python-package/xgboost/spark/utils.py
-def get_logger(cls: type, level: str = "INFO") -> logging.Logger:
+def get_logger(
+    cls_or_callable: Union[type, Callable], level: str = "INFO"
+) -> logging.Logger:
     """Gets a logger by name, or creates and configures it for the first time."""
-    name = _get_class_name(cls)
+    name = _get_class_or_callable_name(cls_or_callable)
     logger = logging.getLogger(name)
 
     logger.setLevel(level)
     # If the logger is configured, skip the configure
     if not logger.handlers and not logging.getLogger().handlers:
         handler = logging.StreamHandler(sys.stderr)
         formatter = logging.Formatter(
```

## Comparing `spark_rapids_ml-23.4.0.dist-info/METADATA` & `spark_rapids_ml-23.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-rapids-ml
-Version: 23.4.0
+Version: 23.6.0
 Summary: Apache Spark integration with RAPIDS and cuML
 Author-email: Jinfeng Li <jinfeng@nvidia.com>, Bobby Wang <bobwang@nvidia.com>, Erik Ordentlich <eordentlich@nvidia.com>, Lee Yang <leey@nvidia.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,26 +20,26 @@
 
 ## Installation
 
 For simplicity, the following instructions just use Spark local mode, assuming a server with at least one GPU.
 
 First, install RAPIDS cuML per [these instructions](https://rapids.ai/start.html).
 ```bash
-conda create -n rapids-23.04 \
+conda create -n rapids-23.06 \
     -c rapidsai -c nvidia -c conda-forge \
-    cuml=23.04 python=3.8 cudatoolkit=11.5
+    cuml=23.06 python=3.9 cudatoolkit=11.5
 ```
 
 **Note**: while testing, we recommend using conda or docker to simplify installation and isolate your environment while experimenting.  Once you have a working environment, you can then try installing directly, if necessary.
 
 **Note**: you can select the latest version compatible with your environment from [rapids.ai](https://rapids.ai/start.html#get-rapids).
 
 Once you have the conda environment, activate it and install the required packages.
 ```bash
-conda activate rapids-23.04
+conda activate rapids-23.06
 
 # for development access to notebooks, tests, and benchmarks
 git clone --branch main https://github.com/NVIDIA/spark-rapids-ml.git
 cd spark-rapids-ml/python
 pip install -r requirements.txt
 pip install -e .
 
@@ -164,15 +164,15 @@
 - **cuML parameters** - there may be additional cuML-specific parameters which might be useful for optimizing GPU performance.  These can be supplied to the various class constructors, but they are _not_ exposed via getters and setters to avoid any confusion with the PySpark ML Params.  If needed, they can be observed via the `cuml_params` attribute.
 - **Algorithmic Results** - again, since the GPU implementations are entirely different from their PySpark ML CPU counterparts, there may be slight differences in the produced results.  This can be due to various reasons, including different optimizations, randomized initializations, or algorithm design.  While these differences should be relatively minor, they should still be reviewed in the context of your specific use case to see if they are within acceptable limits.
 
 **Example**
 ```python
 # from pyspark.ml.clustering import KMeans
 from spark_rapids_ml.clustering import KMeans
-form pyspark.ml.linalg import Vectors
+from pyspark.ml.linalg import Vectors
 
 data = [(Vectors.dense([0.0, 0.0]), 2.0), (Vectors.dense([1.0, 1.0]), 2.0),
         (Vectors.dense([9.0, 8.0]), 2.0), (Vectors.dense([8.0, 9.0]), 2.0)]
 df = spark.createDataFrame(data, ["features", "weighCol"]).repartition(1)
 
 # `k` is a Spark ML Param, `max_samples_per_batch` is a cuML parameter
 kmeans = KMeans(k=3, max_samples_per_batch=16384)
```

