# Comparing `tmp/plotly_resampler-0.9.0rc6.tar.gz` & `tmp/plotly_resampler-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc6.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.1.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc6.tar` & `plotly_resampler-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1115 2023-05-04 08:48:30.616798 plotly_resampler-0.9.0rc6/LICENSE
--rw-r--r--   0        0        0    11180 2023-05-14 08:56:23.448441 plotly_resampler-0.9.0rc6/README.md
--rw-r--r--   0        0        0      853 2023-06-14 07:46:24.712021 plotly_resampler-0.9.0rc6/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6934 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    11877 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3489 2023-05-30 12:53:12.547957 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3179 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     9063 2023-05-30 14:16:09.462114 plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23690 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    63030 2023-06-14 07:27:57.588994 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-05-15 07:51:36.039672 plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc6/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2857 2023-06-14 07:46:36.788373 plotly_resampler-0.9.0rc6/pyproject.toml
--rw-r--r--   0        0        0    12876 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-04 08:48:30.616798 plotly_resampler-0.9.1/LICENSE
+-rw-r--r--   0        0        0    11109 2023-07-13 11:20:48.439467 plotly_resampler-0.9.1/README.md
+-rw-r--r--   0        0        0      849 2023-07-13 11:21:13.751549 plotly_resampler-0.9.1/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-04 08:48:30.656798 plotly_resampler-0.9.1/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-04 08:48:30.656798 plotly_resampler-0.9.1/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    12405 2023-07-10 15:51:54.705188 plotly_resampler-0.9.1/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3489 2023-05-30 12:53:12.547957 plotly_resampler-0.9.1/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-04 08:48:30.656798 plotly_resampler-0.9.1/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     9063 2023-07-01 09:07:09.313561 plotly_resampler-0.9.1/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      478 2023-07-07 21:10:57.100805 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    18689 2023-07-10 15:52:38.845527 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    64097 2023-07-13 11:20:48.451467 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13666 2023-07-07 21:10:57.100805 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     7124 2023-07-04 12:27:42.402346 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/jupyter_dash_persistent_inline_output.py
+-rw-r--r--   0        0        0     5420 2023-07-07 21:10:57.100805 plotly_resampler-0.9.1/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4864 2023-07-07 21:10:57.104805 plotly_resampler-0.9.1/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     3035 2023-07-13 11:21:07.715529 plotly_resampler-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    12841 1970-01-01 00:00:00.000000 plotly_resampler-0.9.1/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc6/LICENSE` & `plotly_resampler-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/README.md` & `plotly_resampler-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 <p align="center">
     <a href="#readme">
-        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/logo.svg" width=65%>
+        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/logo.svg" width=65%>
     </a>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)](https://pypi.org/project/plotly-resampler/)
 [![support-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/pyversions/plotly-resampler)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/predict-idlab/plotly-resampler)
 [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
-[![Documentation](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)
 [![Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml)
+[![Documentation](https://img.shields.io/badge/read%20our%20docs!-informational)](https://predict-idlab.github.io/plotly-resampler/latest)
+
 
 
 <!-- [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler) -->
 
 > `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**
 
 [Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.
 
-![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)
+![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/basic_example.gif)
 
 In [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!
 
 <!-- These dynamic aggregation callbacks are realized with: -->
 <!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->
 <!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->
```

#### html2text {}

```diff
@@ -3,30 +3,29 @@
 (https://pypi.org/project/plotly-resampler/) [![support-version](https://
 img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/
 pyversions/plotly-resampler) [![codecov](https://img.shields.io/codecov/c/
 github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/
 predict-idlab/plotly-resampler) [![Downloads](https://pepy.tech/badge/plotly-
 resampler)](https://pepy.tech/project/plotly-resampler) [![PRs Welcome](https:/
 /img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
-plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://
-github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml) [!
-[Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/
-test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/
-workflows/test.yml)  > `plotly_resampler`: visualize large sequential data by
-**adding resampling functionality to Plotly figures** [Plotly](https://
-github.com/plotly/plotly.py) is an awesome interactive visualization library,
-however it can get pretty slow when a lot of data points are visualized (100
-000+ datapoints). This library solves this by downsampling (aggregating) the
-data respective to the view and then plotting the aggregated points. When you
-interact with the plot (panning, zooming, ...), callbacks are used to aggregate
-data and update the figure. ![basic example gif](https://
-raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
-_static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
-predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
+makeapullrequest.com) [![Testing](https://github.com/predict-idlab/plotly-
+resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-
+idlab/plotly-resampler/actions/workflows/test.yml) [![Documentation](https://
+img.shields.io/badge/read%20our%20docs!-informational)](https://predict-
+idlab.github.io/plotly-resampler/latest)  > `plotly_resampler`: visualize large
+sequential data by **adding resampling functionality to Plotly figures**
+[Plotly](https://github.com/plotly/plotly.py) is an awesome interactive
+visualization library, however it can get pretty slow when a lot of data points
+are visualized (100 000+ datapoints). This library solves this by downsampling
+(aggregating) the data respective to the view and then plotting the aggregated
+points. When you interact with the plot (panning, zooming, ...), callbacks are
+used to aggregate data and update the figure. ![basic example gif](https://
+raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/
+basic_example.gif) In [this Plotly-Resampler demo](https://github.com/predict-
+idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
 `110,000,000` data points are visualized!       ### Installation | [**pip**]
 (https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
 | ---| ----|
 What is the difference between plotly-resampler figures and plain plotly
 figures? `plotly-resampler` can be thought of as wrapper around plain plotly
 figures which adds visualization scalability to line-charts by dynamically
 aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/__init__.py` & `plotly_resampler-0.9.1/plotly_resampler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""**plotly\_resampler**: visualizing large sequences."""
+"""**plotly_resampler**: visualizing large sequences."""
 
 import contextlib
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc6"
+__version__ = "0.9.1"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/aggregators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # -*- coding: utf-8 -*-
 """Compatible implementation for various aggregation/downsample methods.
 
-.. |br| raw:: html
-
-   <br>
-
 """
 
 from __future__ import annotations
 
 __author__ = "Jonas Van Der Donckt"
 
 
@@ -40,42 +36,48 @@
 
     This is arguably the most widely used aggregation method. It is based on the
     effective area of a triangle (inspired from the line simplification domain).
     The algorithm has $O(n)$ complexity, however, for large datasets, it can be much
     slower than other algorithms (e.g. MinMax) due to the higher cost of calculating
     the areas of triangles.
 
-    Thesis: https://skemman.is/bitstream/1946/15343/3/SS_MSthesis.pdf |br|
-    Details on visual representativeness & stability: https://arxiv.org/abs/2304.00900
+    Thesis: [https://skemman.is/bitstream/1946/15343/3/SS_MSthesis.pdf](https://skemman.is/bitstream/1946/15343/3/SS_MSthesis.pdf) <br/>
+    Details on visual representativeness & stability: [https://arxiv.org/abs/2304.00900](https://arxiv.org/abs/2304.00900)
+
+    !!! tip
 
-    .. Tip::
         `LTTB` doesn't scale super-well when moving to really large datasets, so when
         dealing with more than 1 million samples, you might consider using
-        :class:`MinMaxLTTB <MinMaxLTTB>`.
+        [`MinMaxLTTB`][aggregation.aggregators.MinMaxLTTB].
 
 
-    Note
-    ----
-    * This class is mainly designed to operate on numerical data as LTTB calculates
-      distances on the values. |br|
-      When dealing with categories, the data is encoded into its numeric codes,
-      these codes are the indices of the category array.
-    * To aggregate category data with LTTB, your ``pd.Series`` must be of dtype
-      'category'. |br|
-      **Tip**: if there is an order in your categories, order them that way, LTTB uses
-      the ordered category codes values (see bullet above) to calculate distances and
-      make aggregation decisions.
-      .. code::
-        >>> import pandas as pd
-        >>> s = pd.Series(["a", "b", "c", "a"])
-        >>> cat_type = pd.CategoricalDtype(categories=["b", "c", "a"], ordered=True)
-        >>> s_cat = s.astype(cat_type)
-    * `LTTB` has no downsample kwargs, as it cannot be paralellized. Instead, you can
-      use the :class:`MinMaxLTTB <MinMaxLTTB>` downsampler, which performs
-      minmax preselection (in parallel if configured so), followed by LTTB.
+    !!! note
+
+        * This class is mainly designed to operate on numerical data as LTTB calculates
+          distances on the values. <br/>
+          When dealing with categories, the data is encoded into its numeric codes,
+          these codes are the indices of the category array.
+        * To aggregate category data with LTTB, your ``pd.Series`` must be of dtype
+          'category'. <br/>
+
+          **tip**:
+
+          if there is an order in your categories, order them that way, LTTB uses
+          the ordered category codes values (see bullet above) to calculate distances and
+          make aggregation decisions. <br/>
+          **code**:
+            ```python
+                >>> import pandas as pd
+                >>> s = pd.Series(["a", "b", "c", "a"])
+                >>> cat_type = pd.CategoricalDtype(categories=["b", "c", "a"], ordered=True)
+                >>> s_cat = s.astype(cat_type)
+            ```
+        * `LTTB` has no downsample kwargs, as it cannot be paralellized. Instead, you can
+          use the [`MinMaxLTTB`][aggregation.aggregators.MinMaxLTTB] downsampler, which performs
+          minmax preselection (in parallel if configured so), followed by LTTB.
 
     """
 
     def __init__(self):
         super().__init__(
             y_dtype_regex_list=[rf"{dtype}\d*" for dtype in ("float", "int", "uint")]
             + ["category", "bool"],
@@ -91,30 +93,32 @@
         return self.downsampler.downsample(*_to_tsdownsample_args(x, y), n_out=n_out)
 
 
 class MinMaxOverlapAggregator(DataPointSelector):
     """Aggregation method which performs binned min-max aggregation over 50% overlapping
     windows.
 
-    .. image:: _static/minmax_operator.png
+    ![minmax operator image](https://github.com/predict-idlab/plotly-resampler/blob/main/docs/sphinx/_static/minmax_operator.png)
 
     In the above image, **bin_size**: represents the size of *(len(series) / n_out)*.
     As the windows have 50% overlap and are consecutive, the min & max values are
     calculated on a windows with size (2x bin-size).
 
     This is *very* similar to the MinMaxAggregator, emperical results showed no
     observable difference between both approaches.
 
-    .. note::
+    !!! note
+
         This method is implemented in Python (leveraging numpy for vecotrization), but
         is **significantly slower than the MinMaxAggregator** (which is implemented in
-        the tsdownsample toolkit in Rust). |br|
+        the tsdownsample toolkit in Rust). <br/>
         As such, this class does not support any downsample kwargs.
 
-    .. note::
+    !!! note
+
         This downsampler supports all dtypes.
 
     """
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
@@ -152,21 +156,22 @@
 class MinMaxAggregator(DataPointSelector):
     """Aggregation method which performs binned min-max aggregation over fully
     overlapping windows.
 
     This is arguably the most computational efficient downsampling method, as it only
     performs (non-expensive) comparisons on the data in a single pass.
 
-    Details on visual representativeness & stability: https://arxiv.org/abs/2304.00900
+    Details on visual representativeness & stability: [https://arxiv.org/abs/2304.00900](https://arxiv.org/abs/2304.00900)
+
+    !!! note
 
-    .. note::
         This method is rather efficient when scaling to large data sizes and can be used
-        as a data-reduction step before feeding it to the :class:`LTTB <LTTB>`
-        algorithm, as :class:`MinMaxLTTB <MinMaxLTTB>` does with the
-        :class:`MinMaxOverlapAggregator <MinMaxOverlapAggregator>`.
+        as a data-reduction step before feeding it to the [`LTTB`][aggregation.aggregators.LTTB]
+        algorithm, as [`MinMaxLTTB`][aggregation.aggregators.MinMaxLTTB] does with the
+        [`MinMaxOverlapAggregator`][aggregation.aggregators.MinMaxOverlapAggregator].
 
     """
 
     def __init__(self, **downsample_kwargs):
         """
         Parameters
         ----------
@@ -188,34 +193,34 @@
         return self.downsampler.downsample(
             *_to_tsdownsample_args(x, y), n_out=n_out, **self.downsample_kwargs
         )
 
 
 class MinMaxLTTB(DataPointSelector):
     """Efficient version off LTTB by first reducing really large datasets with
-    the :class:`MinMaxAggregator <MinMaxAggregator>` and then further aggregating the
-    reduced result with :class:`LTTB <LTTB>`.
+    the [`MinMaxAggregator`][aggregation.aggregators.MinMaxAggregator] and then further aggregating the
+    reduced result with [`LTTB`][aggregation.aggregators.LTTB].
 
     Starting from 10M data points, this method performs the MinMax-prefetching of data
     points to enhance computational efficiency.
 
     Inventors: Jonas & Jeroen Van Der Donckt - 2022
 
-    Paper: pending
+    Paper: [https://arxiv.org/pdf/2305.00332.pdf](https://arxiv.org/pdf/2305.00332.pdf)
     """
 
     def __init__(self, minmax_ratio: int = 4, **downsample_kwargs):
         """
         Parameters
         ----------
         minmax_ratio: int, optional
             The ratio between the number of data points in the MinMax-prefetching and
             the number of data points that will be outputted by LTTB. By default, 4.
         **downsample_kwargs
-            Keyword arguments passed to the :class:`MinMaxLTTBDownsampler`.
+            Keyword arguments passed to the `MinMaxLTTBDownsampler`.
             - The `parallel` argument is set to False by default.
             - The `minmax_ratio` argument is set to 4 by default, which was empirically
               proven to be a good default.
 
         """
         self.minmaxlttb = MinMaxLTTBDownsampler()
         self.minmax_ratio = minmax_ratio
@@ -239,15 +244,15 @@
             **self.downsample_kwargs,
         )
 
 
 class EveryNthPoint(DataPointSelector):
     """Naive (but fast) aggregator method which returns every N'th point.
 
-    .. note::
+    !!! note
         This downsampler supports all dtypes.
     """
 
     def _arg_downsample(
         self,
         x: np.ndarray | None,
         y: np.ndarray,
@@ -255,21 +260,23 @@
     ) -> np.ndarray:
         return EveryNthDownsampler().downsample(y, n_out=n_out)
 
 
 class FuncAggregator(DataAggregator):
     """Aggregator instance which uses the passed aggregation func.
 
-    .. warning::
+    !!! warning
+
         The user has total control which `aggregation_func` is passed to this method,
         hence the user should be careful to not make copies of the data, nor write to
         the data. Furthermore, the user should beware of performance issues when
         using more complex aggregation functions.
 
-    .. attention::
+    !!! warning "Attention"
+
         The user has total control which `aggregation_func` is passed to this method,
         hence it is the users' responsibility to handle categorical and bool-based
         data types.
 
     """
 
     def __init__(
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/gap_handlers.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.1/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.1/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Abstract ``AbstractFigureAggregator`` interface for the concrete *Resampler* classes.
 
-.. |br| raw:: html
-
-   <br>
-
 """
 
 from __future__ import annotations
 
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
 
 import re
@@ -72,38 +68,40 @@
         convert_existing_traces: bool
             A bool indicating whether the high-frequency traces of the passed ``figure``
             should be resampled, by default True. Hence, when set to False, the
             high-frequency traces of the passed ``figure`` will not be resampled.
         default_n_shown_samples: int, optional
             The default number of samples that will be shown for each trace,
             by default 1000.\n
-            .. note::
-                * This can be overridden within the :func:`add_trace` method.
+            !!! note
+                * This can be overridden within the [`add_trace`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_trace] method.
                 * If a trace withholds fewer datapoints than this parameter,
                   the data will *not* be aggregated.
         default_downsampler: AbstractAggregator
             An instance which implements the AbstractSeriesDownsampler interface and
             will be used as default downsampler, by default ``MinMaxLTTB``. \n
-            .. note:: This can be overridden within the :func:`add_trace` method.
+            !!! note
+                This can be overridden within the [`add_trace`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_trace] method.
         default_gap_handler: GapHandler
             An instance which implements the AbstractGapHandler interface and will be
             used as default gap handler, by default ``MedDiffGapHandler``. \n
-            .. note:: This can be overridden within the :func:`add_trace` method.
+            !!! note
+                This can be overridden within the [`add_trace`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_trace] method.
         resampled_trace_prefix_suffix: str, optional
             A tuple which contains the ``prefix`` and ``suffix``, respectively, which
             will be added to the trace its legend-name when a resampled version of the
             trace is shown. By default, a bold, orange ``[R]`` is shown as prefix
             (no suffix is shown).
         show_mean_aggregation_size: bool, optional
             Whether the mean aggregation bin size will be added as a suffix to the trace
             its legend-name, by default True.
         convert_traces_kwargs: dict, optional
-            A dict of kwargs that will be passed to the :func:`add_traces` method and
+            A dict of kwargs that will be passed to the [`add_traces`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_traces] method and
             will be used to convert the existing traces. \n
-            .. note::
+            !!! note
                 This argument is only used when the passed ``figure`` contains data and
                 ``convert_existing_traces`` is set to True.
         verbose: bool, optional
             Whether some verbose messages will be printed or not, by default False.
 
         """
         self._hf_data: Dict[str, dict] = {}
@@ -157,20 +155,20 @@
         self._yaxis_list = self._re_matches(re.compile("yaxis\d*"), self._layout.keys())
         # edge case: an empty `go.Figure()` does not yet contain axes keys
         if not len(self._xaxis_list):
             self._xaxis_list = ["xaxis"]
             self._yaxis_list = ["yaxis"]
 
         # Make sure to reset the layout its range
-        self.update_layout(
-            {
-                axis: {"autorange": None, "range": None}
-                for axis in self._xaxis_list + self._yaxis_list
-            }
-        )
+        # self.update_layout(
+        #     {
+        #         axis: {"autorange": None, "range": None}
+        #         for axis in self._xaxis_list + self._yaxis_list
+        #     }
+        # )
 
     def _print(self, *values):
         """Helper method for printing if ``verbose`` is set to True."""
         if self._print_verbose:
             print(*values)
 
     def _query_hf_data(self, trace: dict) -> Optional[dict]:
@@ -452,14 +450,19 @@
                 if trace.get("yaxis") is None:
                     # TODO In versions up until v0.8.2 we made the assumption that yaxis
                     # = xaxis_filter_short. -> Why did we make this assumption?
                     y_axis = "y"  # + xaxis_filter[1:]
                 else:
                     y_axis = "yaxis" + trace.get("yaxis")[1:]
 
+                # Also check for overlaying traces - fixes #242
+                overlaying = figure["layout"].get(y_axis, {}).get("overlaying")
+                if overlaying:
+                    y_axis = "yaxis" + overlaying[1:]
+
                 # Next to the x-anchor, we also fetch the xaxis which matches the
                 # current trace (i.e. if this value is not None, the axis shares the
                 # x-axis with one or more traces).
                 # This is relevant when e.g. fig.update_traces(xaxis='x...') was called.
                 x_anchor_trace = figure["layout"].get(y_axis, {}).get("anchor")
                 if x_anchor_trace is not None:
                     xaxis_matches = (
@@ -502,15 +505,15 @@
                 updated_trace_indices.append(idx)
         return updated_trace_indices
 
     @staticmethod
     def _get_figure_class(constr: type) -> type:
         """Get the plotly figure class (constructor) for the given class (constructor).
 
-        .. Note::
+        !!! note
             This method will always return a plotly constructor, even when the given
             `constr` is decorated (after executing the ``register_plotly_resampler``
             function).
 
         Parameters
         ----------
         constr: type
@@ -526,36 +529,39 @@
 
         return _get_plotly_constr(constr)
 
     @property
     def hf_data(self):
         """Property to adjust the `data` component of the current graph
 
-        .. note::
+        !!! note
             The user has full responsibility to adjust ``hf_data`` properly.
 
 
-        Example:
-            >>> from plotly_resampler import FigureResampler
-            >>> fig = FigureResampler(go.Figure())
-            >>> fig.add_trace(...)
-            >>> # Adjust the y property of the above added trace
-            >>> fig.hf_data[-1]["y"] = - s ** 2
-            >>> fig.hf_data
-            [
-                {
-                    'max_n_samples': 1000,
-                    'x': RangeIndex(start=0, stop=11000000, step=1),
-                    'y': array([-0.01339909,  0.01390696,, ...,  0.25051913, 0.55876513]),
-                    'axis_type': 'linear',
-                    'downsampler': <plotly_resampler.aggregation.aggregators.LTTB at 0x7f786d5a9ca0>,
-                    'text': None,
-                    'hovertext': None
-                },
-            ]
+        ??? example
+
+            ```python
+                >>> from plotly_resampler import FigureResampler
+                >>> fig = FigureResampler(go.Figure())
+                >>> fig.add_trace(...)
+                >>> # Adjust the y property of the above added trace
+                >>> fig.hf_data[-1]["y"] = - s ** 2
+                >>> fig.hf_data
+                [
+                    {
+                        'max_n_samples': 1000,
+                        'x': RangeIndex(start=0, stop=11000000, step=1),
+                        'y': array([-0.01339909,  0.01390696,, ...,  0.25051913, 0.55876513]),
+                        'axis_type': 'linear',
+                        'downsampler': <plotly_resampler.aggregation.aggregators.LTTB at 0x7f786d5a9ca0>,
+                        'text': None,
+                        'hovertext': None
+                    },
+                ]
+            ```
         """
         return list(self._hf_data.values())
 
     def _parse_get_trace_props(
         self,
         trace: BaseTraceType,
         hf_x: Iterable = None,
@@ -596,15 +602,17 @@
         hf_x: np.ndarray = (
             # fmt: off
             (np.asarray(trace["x"]) if trace["x"] is not None else None)
             if hasattr(trace, "x") and hf_x is None
             # If we cast a tz-aware datetime64 array to `.values` we lose the tz-info 
             # and the UTC time will be displayed instead of the tz-localized time, 
             # hence we cast to a pd.DatetimeIndex, which preserves the tz-info
-            else pd.Index(hf_x) if pd.core.dtypes.common.is_datetime64tz_dtype(hf_x)
+            # As a matter of fact, to resolve #231, we also convert non-tz-aware 
+            # datetime64 arrays to an pd.Index
+            else pd.Index(hf_x) if pd.core.dtypes.common.is_datetime64_any_dtype(hf_x)
             else hf_x.values if isinstance(hf_x, pd.Series)
             else hf_x if isinstance(hf_x, pd.Index)
             else np.asarray(hf_x)
             # fmt: on
         )
 
         hf_y = (
@@ -892,23 +900,23 @@
                 - The type property specifies the trace type (e.g. scatter, bar,
                   area, etc.). If the dict has no 'type' property then scatter is
                   assumed.
                 - All remaining properties are passed to the constructor
                   of the specified trace type.
         max_n_samples : int, optional
             The maximum number of samples that will be shown by the trace.\n
-            .. note::
+            !!! note
                 If this variable is not set; ``_global_n_shown_samples`` will be used.
         downsampler: AbstractAggregator, optional
             The abstract series downsampler method.\n
-            .. note::
+            !!! note
                 If this variable is not set, ``_global_downsampler`` will be used.
         gap_handler: AbstractGapHandler, optional
             The abstract series gap handler method.\n
-            .. note::
+            !!! note
                 If this variable is not set, ``_global_gap_handler`` will be used.
         limit_to_view: boolean, optional
             If set to True, the trace's datapoints will be cut to the corresponding
             front-end view, even if the total number of samples is lower than
             ``max_n_samples``, By default False.\n
             Remark that setting this parameter to True ensures that low frequency traces
             are added to the ``hf_data`` property.
@@ -938,60 +946,61 @@
             False if you are sure that your data does not contain NaNs (or when the
             downsampler can handle NaNs, e.g., EveryNthPoint). This should considerably
             speed up the graph construction time.
         **trace_kwargs: dict
             Additional trace related keyword arguments.
             e.g.: row=.., col=..., secondary_y=...
 
-            .. seealso::
-                `Figure.add_trace <https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.add_trace>`_ docs.
+            !!! info "See Also"
+                [`Figure.add_trace`](https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.add_trace>) docs.
 
         Returns
         -------
         BaseFigure
             The Figure on which ``add_trace`` was called on; i.e. self.
 
-        Note
-        ----
-        Constructing traces with **very large data amounts** really takes some time.
-        To speed this up; use this :func:`add_trace` method and
+        !!! note
 
-        1. Create a trace with no data (empty lists)
-        2. pass the high frequency data to this method using the ``hf_x`` and ``hf_y``
-           parameters.
-
-        See the example below:
-
-            >>> from plotly.subplots import make_subplots
-            >>> s = pd.Series()  # a high-frequency series, with more than 1e7 samples
-            >>> fig = FigureResampler(go.Figure())
-            >>> fig.add_trace(go.Scattergl(x=[], y=[], ...), hf_x=s.index, hf_y=s)
-
-        .. todo::
-            * explain why adding x and y to a trace is so slow
-            * check and simplify the example above
-
-        Tip
-        ---
-        * If you **do not want to downsample** your data, set ``max_n_samples`` to the
-          the number of datapoints of your trace!
-
-        Attention
-        ---------
-        * The ``NaN`` values in either ``hf_y`` or ``trace.y`` will be omitted! We do
-          not allow ``NaN`` values in ``hf_x`` or ``trace.x``.
-        * ``hf_x``, ``hf_y``, ``hf_text``, and ``hf_hovertext`` are useful when you deal
-          with large amounts of data (as it can increase the speed of this add_trace()
-          method with ~30%). These arguments have priority over the trace's data and
-          (hover)text attributes.
-        * Low-frequency time-series data, i.e. traces that are not resampled, can hinder
-          the the automatic-zooming (y-scaling) as these will not be stored in the
-          back-end and thus not be scaled to the view.
-          To circumvent this, the ``limit_to_view`` argument can be set, resulting in
-          also storing the low-frequency series in the back-end.
+            Constructing traces with **very large data amounts** really takes some time.
+            To speed this up; use this [`add_trace`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_trace] method and
+
+            1. Create a trace with no data (empty lists)
+            2. pass the high frequency data to this method using the ``hf_x`` and ``hf_y``
+               parameters.
+
+            See the example below:
+                ```python
+                >>> from plotly.subplots import make_subplots
+                >>> s = pd.Series()  # a high-frequency series, with more than 1e7 samples
+                >>> fig = FigureResampler(go.Figure())
+                >>> fig.add_trace(go.Scattergl(x=[], y=[], ...), hf_x=s.index, hf_y=s)
+                ```
+
+            !!! todo
+                * explain why adding x and y to a trace is so slow
+                * check and simplify the example above
+
+        !!! tip
+
+            * If you **do not want to downsample** your data, set ``max_n_samples`` to the
+              the number of datapoints of your trace!
+
+        !!! warning
+
+            * The ``NaN`` values in either ``hf_y`` or ``trace.y`` will be omitted! We do
+              not allow ``NaN`` values in ``hf_x`` or ``trace.x``.
+            * ``hf_x``, ``hf_y``, ``hf_text``, and ``hf_hovertext`` are useful when you deal
+              with large amounts of data (as it can increase the speed of this add_trace()
+              method with ~30%). These arguments have priority over the trace's data and
+              (hover)text attributes.
+            * Low-frequency time-series data, i.e. traces that are not resampled, can hinder
+              the the automatic-zooming (y-scaling) as these will not be stored in the
+              back-end and thus not be scaled to the view.
+              To circumvent this, the ``limit_to_view`` argument can be set, resulting in
+              also storing the low-frequency series in the back-end.
 
         """
         # to comply with the plotly data input acceptance behavior
         if isinstance(trace, (list, tuple)):
             raise ValueError("Trace must be either a dict or a BaseTraceType")
 
         max_out_s = (
@@ -1077,16 +1086,17 @@
         gap_handlers: None | List[AbstractGapHandler] | AbstractGapHandler = None,
         limit_to_views: List[bool] | bool = False,
         check_nans: List[bool] | bool = True,
         **traces_kwargs,
     ):
         """Add traces to the figure.
 
-        .. note::
-            Make sure to look at the :func:`add_trace` function for more info about
+        !!! note
+
+            Make sure to look at the [`add_trace`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator.add_trace] function for more info about
             **speed optimization**, and dealing with not ``high-frequency`` data, but
             still want to resample / limit the data to the front-end view.
 
         Parameters
         ----------
         data : List[BaseTraceType  |  dict]
             A list of trace specifications to be added.
@@ -1097,15 +1107,14 @@
               - Dicts where:
 
                   - The 'type' property specifies the trace type (e.g.
                     'scatter', 'bar', 'area', etc.). If the dict has no 'type'
                     property then 'scatter' is assumed.
                   - All remaining properties are passed to the constructor
                     of the specified trace type.
-
         max_n_samples : None | List[int] | int, optional
               The maximum number of samples that will be shown for each trace.
               If a single integer is passed, all traces will use this number. If this
               variable is not set; ``_global_n_shown_samples`` will be used.
         downsamplers : None | List[AbstractAggregator] | AbstractAggregator, optional
             The downsampler that will be used to aggregate the traces. If a single
             aggregator is passed, all traces will use this aggregator.
@@ -1126,21 +1135,21 @@
             List of check_nans booleans for the added traces. If set to True, the
             trace's datapoints will be checked for NaNs. If a single boolean is passed,
             all to be added traces will use this value, by default True.\n
             As this is a costly operation, it is recommended to set this parameter to
             False if the data is known to contain no NaNs (or when the downsampler can
             handle NaNs, e.g., EveryNthPoint). This will considerably speed up the graph
             construction time.
-
         **traces_kwargs: dict
             Additional trace related keyword arguments.
             e.g.: rows=.., cols=..., secondary_ys=...
 
-            .. seealso::
-                `Figure.add_traces <https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.add_traces>`_ docs.
+            !!! info "See Also"
+
+                [`Figure.add_traces`](https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.add_traces>) docs.
 
         Returns
         -------
         BaseFigure
             The Figure on which ``add_traces`` was called on; i.e. self.
 
         """
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.1/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 class FigureWidgetResampler(
     AbstractFigureAggregator, go.FigureWidget, metaclass=_FigureWidgetResamplerM
 ):
     """Data aggregation functionality wrapper for ``go.FigureWidgets``.
 
-    .. attention::
+    !!! warning
 
         * This wrapper only works within ``jupyter``-based environments.
         * The ``.show()`` method returns a **static figure** on which the
           **dynamic resampling cannot be performed**. To allow dynamic resampling,
           you should just output the ``FigureWidgetResampler`` object in a cell.
 
     """
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.1/plotly_resampler/figure_resampler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 ### Checks for the figure type
 
 
 def is_figure(figure: Any) -> bool:
     """Check if the figure is a plotly go.Figure or a FigureResampler.
 
-    .. Note::
+    !!! note
+
         This method does not use isinstance(figure, go.Figure) as this will not work
         when go.Figure is decorated (after executing the
         ``register_plotly_resampler`` function).
 
     Parameters
     ----------
     figure : Any
@@ -35,15 +36,16 @@
     """
     return isinstance(figure, BaseFigure) and (not isinstance(figure, BaseFigureWidget))
 
 
 def is_figurewidget(figure: Any):
     """Check if the figure is a plotly go.FigureWidget or a FigureWidgetResampler.
 
-    .. Note::
+    !!! note
+
         This method does not use isinstance(figure, go.FigureWidget) as this will not
         work when go.FigureWidget is decorated (after executing the
         ``register_plotly_resampler`` function).
 
     Parameters
     ----------
     figure : Any
@@ -56,15 +58,16 @@
     """
     return isinstance(figure, BaseFigureWidget)
 
 
 def is_fr(figure: Any) -> bool:
     """Check if the figure is a FigureResampler.
 
-    .. Note::
+    !!! note
+
         This method will not return True if the figure is a plotly go.Figure.
 
     Parameters
     ----------
     figure : Any
         The figure to check.
 
@@ -77,15 +80,16 @@
 
     return isinstance(figure, FigureResampler)
 
 
 def is_fwr(figure: Any) -> bool:
     """Check if the figure is a FigureWidgetResampler.
 
-    .. Note::
+    !!! note
+
         This method will not return True if the figure is a plotly go.FigureWidget.
 
     Parameters
     ----------
     figure : Any
         The figure to check.
 
@@ -161,16 +165,16 @@
 
     Returns
     -------
     str
         The rounded timedelta as a string.
         If the timedelta is == 0, None is returned.
 
-    .. seealso::
-        :func:`timedelta_to_str`
+    !!! info "See Also"
+        [`timedelta_to_str`][figure_resampler.utils.timedelta_to_str]
 
     """
     for t_s in ("D", "H", "min", "s", "ms", "us", "ns"):
         if td > 0.95 * pd.Timedelta(f"1{t_s}"):
             return timedelta_to_str(td.round(t_s))
```

### Comparing `plotly_resampler-0.9.0rc6/plotly_resampler/registering.py` & `plotly_resampler-0.9.1/plotly_resampler/registering.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def _already_wrapped(constr):
     return constr.__name__.startswith(WRAPPED_PREFIX)
 
 
 def _get_plotly_constr(constr):
     """Return the constructor of the underlying plotly graph object and thus omit the
-    possibly wrapped :class:`AbstractFigureAggregator <plotly_resampler.figure_resampler.figure_resampler_interface.AbstractFigureAggregator>`
+    possibly wrapped [`AbstractFigureAggregator`][figure_resampler.figure_resampler_interface.AbstractFigureAggregator]
     instance.
 
     Parameters
     ----------
     constr : callable
         The constructor of a instantiated plotly-object.
 
@@ -80,21 +80,21 @@
 
 
 def register_plotly_resampler(mode="auto", **aggregator_kwargs):
     """Register plotly-resampler to plotly.graph_objects.
 
     This function results in the use of plotly-resampler under the hood.
 
-    .. Note::
+    !!! note
         We advise to use mode= ``widget`` when working in an IPython based environment
         as this will just behave as a ``go.FigureWidget``, but with dynamic aggregation.
         When using mode= ``auto`` or ``figure``; most figures will be wrapped as
-        :class:`FigureResampler <plotly_resampler.figure_resampler.FigureResampler>`,
+        [`FigureResampler`][figure_resampler.FigureResampler],
         on which
-        :func:`show_dash <plotly_resampler.figure_resampler.FigureResampler.show_dash>`
+        [`show_dash`][figure_resampler.FigureResampler.show_dash]
         needs to be called.
 
     Parameters
     ----------
     mode : str, optional
         The mode of the plotly-resampler.
         Possible values are: 'auto', 'figure', 'widget', None.
@@ -104,16 +104,16 @@
         If 'widget' is used, all plotly figure widgets are wrapped as
         FigureWidgetResampler objects (we advise to use this mode in IPython environment
         with a kernel).
         If None is used, wrapping is done as expected (go.Figure -> FigureResampler,
         go.FigureWidget -> FigureWidgetResampler).
     aggregator_kwargs : dict, optional
         The keyword arguments to pass to the plotly-resampler decorator its constructor.
-        See more details in :class:`FigureResampler <FigureResampler>` and
-        :class:`FigureWidgetResampler <FigureWidgetResampler>`.
+        See more details in [`FigureResampler`][figure_resampler.FigureResampler] and
+        [`FigureWidgetResampler`][figure_resampler.FigureWidgetResampler].
 
     """
     for constr_name, pr_class in PLOTLY_CONSTRUCTOR_WRAPPER.items():
         if (mode == "auto" and _is_ipython_env()) or mode == "widget":
             pr_class = FigureWidgetResampler
         elif mode == "figure":
             pr_class = FigureResampler
```

### Comparing `plotly_resampler-0.9.0rc6/pyproject.toml` & `plotly_resampler-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc6"
+version = "0.9.1"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
-documentation = "https://predict-idlab.github.io/plotly-resampler"
+documentation = "https://predict-idlab.github.io/plotly-resampler/latest"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
 packages = [
     { include = "plotly_resampler" }
 ]
 include = [
     # C extensions must be included in the wheel distributions
     {path = "plotly_resampler/aggregation/algorithms/*.so", format = "wheel"},
@@ -30,17 +30,17 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
-jupyter-dash = ">=0.4.2"
+jupyter-dash = { version = ">=0.4.2", optional = true }
 plotly = "^5.5.0"
-dash = "^2.2.0"
+dash = "^2.11.0"
 pandas = ">=1"
 trace-updater = ">=0.0.8"
 numpy = [
     { version = ">=1.14", python = "<3.11" },
     { version = ">=1.24", python = ">=3.11" }
 ]
 orjson = "^3.8.0"  # Faster json serialization
@@ -48,34 +48,38 @@
 Flask-Cors = { version = "^3.0.10", optional = true }
 # Lock kaleido dependency until https://github.com/plotly/Kaleido/issues/156 is resolved
 kaleido = {version = "0.2.1", optional = true}
 tsdownsample = "0.1.2"
 
 [tool.poetry.extras]
 # Optional dependencies
-inline_persistent = ["kaleido", "Flask-Cors"]
+inline_persistent = ["kaleido", "Flask-Cors", "jupyter-dash"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 selenium = "4.2.0"
 pytest-selenium = "^2.0.1"
 webdriver-manager = "^3.5.2"
 selenium-wire = "^5.0"
 pyarrow = "^10.0"
-Sphinx = "^4.4.0"
-pydata-sphinx-theme = "^0.13.3"
-sphinx-autodoc-typehints = "^1.17.0"
 ipywidgets = "^7.7.1"
 memory-profiler = "^0.60.0"
 line-profiler = "^4.0"
 ruff = "^0.0.262"
 black = "^22.6.0"
 pytest-lazy-fixture = "^0.6.3"
 # yep = "^0.4"  # c code profiling
+mkdocs = "^1.4.3"
+mkdocstrings = { version = "^0.20.0", extras = ["python"] }
+mkdocs-gen-files = "^0.5.0"
+mike = "^1.1.2"
+mkdocs-material = "^9.1.18"
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-section-index = "^0.3.5"
 
 # Linting
 [tool.ruff]
 select = ["E", "F", "I"]
 line-length = 88
 ignore = ["E501"] # Never enforce `E501` (line length violations).
 [tool.ruff.per-file-ignores]
```

### Comparing `plotly_resampler-0.9.0rc6/PKG-INFO` & `plotly_resampler-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc6
+Version: 0.9.1
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,50 +18,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: inline-persistent
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ; extra == "inline-persistent"
-Requires-Dist: dash (>=2.2.0,<3.0.0)
-Requires-Dist: jupyter-dash (>=0.4.2)
+Requires-Dist: dash (>=2.11.0,<3.0.0)
+Requires-Dist: jupyter-dash (>=0.4.2) ; extra == "inline-persistent"
 Requires-Dist: kaleido (==0.2.1) ; extra == "inline-persistent"
 Requires-Dist: numpy (>=1.14) ; python_version < "3.11"
 Requires-Dist: numpy (>=1.24) ; python_version >= "3.11"
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1)
 Requires-Dist: plotly (>=5.5.0,<6.0.0)
 Requires-Dist: trace-updater (>=0.0.8)
 Requires-Dist: tsdownsample (==0.1.2)
-Project-URL: Documentation, https://predict-idlab.github.io/plotly-resampler
+Project-URL: Documentation, https://predict-idlab.github.io/plotly-resampler/latest
 Project-URL: Repository, https://github.com/predict-idlab/plotly-resampler
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="#readme">
-        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/logo.svg" width=65%>
+        <img alt="Plotly-Resampler logo" src="https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/logo.svg" width=65%>
     </a>
 </p>
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)](https://pypi.org/project/plotly-resampler/)
 [![support-version](https://img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/pyversions/plotly-resampler)
 [![codecov](https://img.shields.io/codecov/c/github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/predict-idlab/plotly-resampler)
 [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://makeapullrequest.com)
-[![Documentation](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml)
 [![Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/workflows/test.yml)
+[![Documentation](https://img.shields.io/badge/read%20our%20docs!-informational)](https://predict-idlab.github.io/plotly-resampler/latest)
+
 
 
 <!-- [![Downloads](https://pepy.tech/badge/plotly-resampler)](https://pepy.tech/project/plotly-resampler) -->
 
 > `plotly_resampler`: visualize large sequential data by **adding resampling functionality to Plotly figures**
 
 [Plotly](https://github.com/plotly/plotly.py) is an awesome interactive visualization library, however it can get pretty slow when a lot of data points are visualized (100 000+ datapoints). This library solves this by downsampling (aggregating) the data respective to the view and then plotting the aggregated points. When you interact with the plot (panning, zooming, ...), callbacks are used to aggregate data and update the figure.
 
-![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/_static/basic_example.gif)
+![basic example gif](https://raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/basic_example.gif)
 
 In [this Plotly-Resampler demo](https://github.com/predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over `110,000,000` data points are visualized!
 
 <!-- These dynamic aggregation callbacks are realized with: -->
 <!-- * [Dash](https://github.com/plotly/dash) when a `go.Figure` object is wrapped with dynamic aggregation functionality, see example ⬆️. -->
 <!-- * The [FigureWidget.layout.on_change](https://plotly.com/python-api-reference/generated/plotly.html?highlight=on_change#plotly.basedatatypes.BasePlotlyType.on_change) method, when a `go.FigureWidget` is used within a `.ipynb` environment. -->
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc6 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.1 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: inline-persistent Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ;
-extra == "inline-persistent" Requires-Dist: dash (>=2.2.0,<3.0.0) Requires-
-Dist: jupyter-dash (>=0.4.2) Requires-Dist: kaleido (==0.2.1) ; extra ==
-"inline-persistent" Requires-Dist: numpy (>=1.14) ; python_version < "3.11"
-Requires-Dist: numpy (>=1.24) ; python_version >= "3.11" Requires-Dist: orjson
-(>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1) Requires-Dist: plotly
-(>=5.5.0,<6.0.0) Requires-Dist: trace-updater (>=0.0.8) Requires-Dist:
-tsdownsample (==0.1.2) Project-URL: Documentation, https://predict-
-idlab.github.io/plotly-resampler Project-URL: Repository, https://github.com/
-predict-idlab/plotly-resampler Description-Content-Type: text/markdown
+extra == "inline-persistent" Requires-Dist: dash (>=2.11.0,<3.0.0) Requires-
+Dist: jupyter-dash (>=0.4.2) ; extra == "inline-persistent" Requires-Dist:
+kaleido (==0.2.1) ; extra == "inline-persistent" Requires-Dist: numpy (>=1.14)
+; python_version < "3.11" Requires-Dist: numpy (>=1.24) ; python_version >=
+"3.11" Requires-Dist: orjson (>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1)
+Requires-Dist: plotly (>=5.5.0,<6.0.0) Requires-Dist: trace-updater (>=0.0.8)
+Requires-Dist: tsdownsample (==0.1.2) Project-URL: Documentation, https://
+predict-idlab.github.io/plotly-resampler/latest Project-URL: Repository, https:
+//github.com/predict-idlab/plotly-resampler Description-Content-Type: text/
+markdown
                             [Plotly-Resampler_logo]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)]
 (https://pypi.org/project/plotly-resampler/) [![support-version](https://
 img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/
 pyversions/plotly-resampler) [![codecov](https://img.shields.io/codecov/c/
 github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/
 predict-idlab/plotly-resampler) [![Downloads](https://pepy.tech/badge/plotly-
 resampler)](https://pepy.tech/project/plotly-resampler) [![PRs Welcome](https:/
 /img.shields.io/badge/PRs-welcome-brightgreen.svg?)](http://
-makeapullrequest.com) [![Documentation](https://github.com/predict-idlab/
-plotly-resampler/actions/workflows/deploy-docs.yml/badge.svg)](https://
-github.com/predict-idlab/plotly-resampler/actions/workflows/deploy-docs.yml) [!
-[Testing](https://github.com/predict-idlab/plotly-resampler/actions/workflows/
-test.yml/badge.svg)](https://github.com/predict-idlab/plotly-resampler/actions/
-workflows/test.yml)  > `plotly_resampler`: visualize large sequential data by
-**adding resampling functionality to Plotly figures** [Plotly](https://
-github.com/plotly/plotly.py) is an awesome interactive visualization library,
-however it can get pretty slow when a lot of data points are visualized (100
-000+ datapoints). This library solves this by downsampling (aggregating) the
-data respective to the view and then plotting the aggregated points. When you
-interact with the plot (panning, zooming, ...), callbacks are used to aggregate
-data and update the figure. ![basic example gif](https://
-raw.githubusercontent.com/predict-idlab/plotly-resampler/main/docs/sphinx/
-_static/basic_example.gif) In [this Plotly-Resampler demo](https://github.com/
-predict-idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
+makeapullrequest.com) [![Testing](https://github.com/predict-idlab/plotly-
+resampler/actions/workflows/test.yml/badge.svg)](https://github.com/predict-
+idlab/plotly-resampler/actions/workflows/test.yml) [![Documentation](https://
+img.shields.io/badge/read%20our%20docs!-informational)](https://predict-
+idlab.github.io/plotly-resampler/latest)  > `plotly_resampler`: visualize large
+sequential data by **adding resampling functionality to Plotly figures**
+[Plotly](https://github.com/plotly/plotly.py) is an awesome interactive
+visualization library, however it can get pretty slow when a lot of data points
+are visualized (100 000+ datapoints). This library solves this by downsampling
+(aggregating) the data respective to the view and then plotting the aggregated
+points. When you interact with the plot (panning, zooming, ...), callbacks are
+used to aggregate data and update the figure. ![basic example gif](https://
+raw.githubusercontent.com/predict-idlab/plotly-resampler/main/mkdocs/static/
+basic_example.gif) In [this Plotly-Resampler demo](https://github.com/predict-
+idlab/plotly-resampler/blob/main/examples/basic_example.ipynb) over
 `110,000,000` data points are visualized!       ### Installation | [**pip**]
 (https://pypi.org/project/plotly_resampler/) | `pip install plotly-resampler` |
 | ---| ----|
 What is the difference between plotly-resampler figures and plain plotly
 figures? `plotly-resampler` can be thought of as wrapper around plain plotly
 figures which adds visualization scalability to line-charts by dynamically
 aggregating the data w.r.t. the front-end view. `plotly-resampler` thus adds
```

