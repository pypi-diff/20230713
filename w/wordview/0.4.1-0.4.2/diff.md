# Comparing `tmp/wordview-0.4.1.tar.gz` & `tmp/wordview-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.4.1.tar", max compression
+gzip compressed data, was "wordview-0.4.2.tar", max compression
```

## Comparing `wordview-0.4.1.tar` & `wordview-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1849 2023-06-29 13:33:48.786617 wordview-0.4.1/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-29 13:33:48.786617 wordview-0.4.1/LICENSE
--rw-r--r--   0        0        0     4342 2023-06-29 13:33:48.786617 wordview-0.4.1/README.rst
--rw-r--r--   0        0        0      873 2023-06-29 13:33:48.870618 wordview-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-29 13:33:48.870618 wordview-0.4.1/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/mwes/am.py
--rw-r--r--   0        0        0    11822 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-29 13:33:48.874618 wordview-0.4.1/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 wordview-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2107 2023-07-13 10:31:23.988287 wordview-0.4.2/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-07-13 10:31:23.988287 wordview-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4192 2023-07-13 10:31:23.988287 wordview-0.4.2/README.rst
+-rw-r--r--   0        0        0      893 2023-07-13 10:31:24.076289 wordview-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-07-13 10:31:24.076289 wordview-0.4.2/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/am.py
+-rw-r--r--   0        0        0    11970 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    12315 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8763 2023-07-13 10:31:24.080289 wordview-0.4.2/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 wordview-0.4.2/PKG-INFO
```

### Comparing `wordview-0.4.1/CHANGES.rst` & `wordview-0.4.2/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 0.4.2
+-------------
+- Better encapsulation.
+- Overall improvement and fix of several inconsistencies in docstring.
+- Allow quite a few plot configurations via kwargs.
+- Rm old code from the demo notebook.
+- Change cover.
+- Optimize figure creation.
+
 Version 0.4.1
 -------------
 - Update precommit hooks mypy and black versions
 
 Version 0.4.0
 -------------
 - Support for extracting variable length MWE given a user pattern of POS tags.
```

### Comparing `wordview-0.4.1/LICENSE` & `wordview-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/README.rst` & `wordview-0.4.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
-|text_analysis_cover|
+|cover|
 
 
 Usage
 ######
 
 Install the package via ``pip``:
 
@@ -95,12 +95,8 @@
 
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
-.. |cover| image:: docs/figs/abstract_cover_2.png
-.. |clustering_cover| image:: docs/figs/clustering_cover.png
-.. |text_analysis_cover| image:: docs/figs/text_analysis.png
-
-
+.. |cover| image:: docs/figs/cover.png
```

### Comparing `wordview-0.4.1/pyproject.toml` & `wordview-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.4.1"
+version = "0.4.2"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
 
@@ -23,15 +23,17 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3.0.0"
 pytest = ">=7.1"
 pytest-cov = ">=3.0.0"
 ipython = ">=8.4.0"
 sphinx = ">=v6.1.3"
-sphinx-rtd-theme= "1.2.1"
+sphinx-rtd-theme = "1.2.1"
+jupyter = "1.0.0"
+
 
 [tool.poetry.scripts]
 nltk_download_script = "bin.downloads:download_nltk_req"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wordview-0.4.1/wordview/anomaly/gaussianize.py` & `wordview-0.4.2/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/wordview/anomaly/normaldist.py` & `wordview-0.4.2/wordview/anomaly/normaldist.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 scale=np.std(self.item_value_df["guassian_values"]),
             )
             self.item_value_df["normal_prob"] = self.item_value_df[
                 "guassian_values"
             ].apply(lambda x: dist.pdf(x))
         else:
             logger.error(
-                "The provided values cannot be gaussanized. Please consider using another anomaly detection method."
+                "The provided values cannot be gaussianized. Please consider using another anomaly detection method."
             )
 
     def anomalous_items(
         self,
         manual: bool = False,
         z: int = 3,
         prob: float = 0.001,
```

### Comparing `wordview-0.4.1/wordview/clustering/cluster.py` & `wordview-0.4.2/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/wordview/mwes/am.py` & `wordview-0.4.2/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/wordview/mwes/mwe.py` & `wordview-0.4.2/wordview/mwes/mwe.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,15 +237,39 @@
                     else:
                         mwes.append(w1[0] + " " + w2[0])
         mwes_count_dic = Counter(mwes)
         return mwes_count_dic
 
 
 class HigherOrderMWEExtractor:
+    """Extract higher order MWEs from a list of tokens based on a given pattern."""
+
     def __init__(self, tokens: list[str], pattern: str) -> None:
+        """Initializes a new instance of HigherOrderMWEExtractor class.
+
+        Args:
+            tokens: A list of tokens.
+            pattern: A string pattern to match against the tokens. The pattern must be a string of the following form.
+
+        Examples of user-defined patterns:
+        - NP: {<DT>?<JJ>*<NN>} # Noun phrase
+        - VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
+        - PP: {<IN><NP>} # Prepositional phrase
+
+        You can use multiple and/or nested patterns, separated by a newline character:
+        pattern = '''
+        NP: {<DT>?<JJ>*<NN>} # Noun phrase
+        PROPN: {<NNP>+} # Proper noun
+        ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
+        ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase
+        '''
+
+        In this case, patterns of a clause are executed in order.  An earlier
+        pattern may introduce a chunk boundary that prevents a later pattern from executing.
+        """
         self.tokens = tokens
         self.pattern = pattern
         self._validate_input()
 
     def _validate_input(self) -> None:
         if not isinstance(self.tokens, list):
             raise TypeError(
@@ -266,37 +290,20 @@
                 'Input argument "pattern" must be a non-zero length string.'
             )
 
     def extract_higher_order_mwe_candidates(self) -> dict:
         """
         Extract variable-length MWE from tokenized input, using a user-defined POS regex pattern.
 
-        Parameters:
-            tokens (list[str]): A list of tuples containing the word and its corresponding part-of-speech tag.
-            pattern (str): A string containing a user-defined pattern for nltk.RegexpParser.
+        Args:
+            None
 
         Returns:
             match_counter (dict[str, dict[str, int]]): A counter dictionary with count of matched strings, grouped by pattern label.
                                                     An empty list if none were found.
-
-        Examples of user-defined patterns:
-        - NP: {<DT>?<JJ>*<NN>} # Noun phrase
-        - VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
-        - PP: {<IN><NP>} # Prepositional phrase
-
-        You can use multiple and/or nested patterns, separated by a newline character:
-        pattern = '''
-        NP: {<DT>?<JJ>*<NN>} # Noun phrase
-        PROPN: {<NNP>+} # Proper noun
-        ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
-        ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase
-        '''
-
-        In this case, patterns of a clause are executed in order.  An earlier
-        pattern may introduce a chunk boundary that prevents a later pattern from executing.
         """
 
         tagged_tokens: list[tuple[str, str]] = get_pos_tags(self.tokens)
         parser = RegexpParser(self.pattern)
         parsed_tokens = parser.parse(tagged_tokens)
 
         labels: list[str] = [
```

### Comparing `wordview-0.4.1/wordview/mwes/mwe_utils.py` & `wordview-0.4.2/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/wordview/preprocessing/cleaning.py` & `wordview-0.4.2/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.4.1/wordview/text_analysis/core.py` & `wordview-0.4.2/wordview/text_analysis/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 from plotly.subplots import make_subplots
 from tqdm import tqdm
 from wordcloud import WordCloud, get_single_color_func
 
 from wordview import logger
 
 
-def plotly_wordcloud(
-    token_count_dic: dict, settings: Dict = {"color": "deepskyblue", "max_words": 100}
-) -> plotly.graph_objects.Scattergl:
+def plotly_wordcloud(token_count_dic: dict, **kwargs) -> plotly.graph_objects.Scattergl:
     """Create a world cloud trace for plotly.
 
     Args:
         token_count_dic (Dict): Dictionary of token to its count
-        settings (Dict): wordcloud.WordCloud settings.
+        **kwargs:
 
     Returns:
         trace (plotly.graph_objects.Scatter)
     """
+    wc_settings: Dict = kwargs.get(
+        "wc_settings", {"color": "deepskyblue", "max_words": 100}
+    )
     wc = WordCloud(
-        color_func=get_single_color_func(settings["color"]),
-        max_words=settings["max_words"],
+        color_func=get_single_color_func(wc_settings["color"]),
+        max_words=wc_settings["max_words"],
     )
     wc.generate_from_frequencies(token_count_dic)
     word_list = []
     rel_freq_list = []
     freq_list = []
     fontsize_list = []
     position_list = []
@@ -79,23 +80,24 @@
         logger.error(
             f"While creating the word cloud, plotly.go returned the following error \
          \n{E}\nfor relative frequencies: {rel_freq_list}\nthat were mapped to {new_freq_list}"
         )
 
 
 def generate_label_plots(
-    df: pandas.DataFrame, label_cols: List[Tuple]
+    df: pandas.DataFrame, label_cols: List[Tuple], **kwargs
 ) -> plotly.graph_objects.Figure:
     """Generate histogram and bar plots for the labels in label_cols.
 
     Args:
-        figure (plotly.graph_objs.Figure): Figure object in which the plots are created.
         df (Pandas DataFrame): DataFrame that contains labels specified in label_cols.
         label_cols (list): list of tuples in the form of [('label_1', 'categorical/numerical'),
                            ('label_2', 'categorical/numerical'), ...]
+        **kwargs: Additional arguments to pass to plotly.Figure.update_layout(). For more details
+                  see https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.update_layout
 
     Returns:
         plotly.graph_objects.Figure
     """
 
     if len(label_cols) == 1:
         # with titles
@@ -128,14 +130,15 @@
         lab_trace2 = label_plot(
             df, label_col=label_cols[1][0], label_type=label_cols[1][1]
         )
         lab_trace3 = label_plot(
             df, label_col=label_cols[2][0], label_type=label_cols[2][1]
         )
         figure.append_trace(lab_trace1, 1, 1)
+
         figure.append_trace(lab_trace2, 1, 2)
         figure.append_trace(lab_trace3, 1, 3)
     elif len(label_cols) == 4:
         figure = make_subplots(rows=2, cols=2)
         lab_trace1 = label_plot(
             df, label_col=label_cols[0][0], label_type=label_cols[0][1]
         )
@@ -148,14 +151,15 @@
         lab_trace4 = label_plot(
             df, label_col=label_cols[3][0], label_type=label_cols[3][1]
         )
         figure.append_trace(lab_trace1, 1, 1)
         figure.append_trace(lab_trace2, 1, 2)
         figure.append_trace(lab_trace3, 2, 1)
         figure.append_trace(lab_trace4, 2, 2)
+    figure.update_layout(**kwargs)
     return figure
 
 
 def label_plot(
     df: pandas.DataFrame, label_col: str, label_type: str
 ) -> plotly.graph_objects.Histogram:
     """Create a plot for label_col in df, wrt to label_type.
@@ -166,27 +170,38 @@
         label_type (str): Represents the type of label and consequently specifies the type of plot.
                              It can be "numerical" or "categorical".
 
     Returns:
         trace (plotly.graph_objects.Histogram)
     """
     if label_type == "categorical":
-        values = df[label_col].unique().tolist()  # ['pos', 'neg', 'neutral']
-        counts = df[label_col].value_counts()  # 1212323
+        values = df[label_col].unique().tolist()  # E.g. ['pos', 'neg', 'neutral']
+        counts = df[label_col].value_counts()  # E.g. 1212323
         x = []
         y = []
         for v in values:
             x.append(v)
             y.append(counts[v])
-        trace = go.Bar(x=x, y=y, name=label_col)
+        trace = go.Bar(
+            x=x,
+            y=y,
+            name=label_col,
+            marker=dict(
+                color=y, coloraxis="coloraxis", line=dict(width=0.5, color="white")
+            ),
+        )
     elif label_type == "numerical":
         trace = go.Histogram(
             x=df[label_col],
             name=label_col,
-            marker=dict(line=dict(width=0.5, color="white")),
+            marker=dict(
+                color=df[label_col],
+                coloraxis="coloraxis",
+                line=dict(width=0.5, color="white"),
+            ),
         )
     else:
         raise ValueError(
             'label_col input argument must be set to either "categorical" or "numerical".'
         )
     return trace
```

### Comparing `wordview-0.4.1/wordview/text_analysis/wrapper.py` & `wordview-0.4.2/wordview/text_analysis/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,35 +46,33 @@
         self.token_count = self.analysis.token_count
         self.num_docs = self.analysis.doc_count
         self.median_doc_len = self.analysis.median_doc_len
         self.num_nns = len(self.analysis.nns)
         self.num_jjs = len(self.analysis.jjs)
         self.num_vbs = len(self.analysis.vs)
 
-    def create_dist_plots(self) -> Dict[str, go.Figure]:
+    def _create_dist_plots(self, **kwargs) -> Dict[str, go.Figure]:
         """Create distribution plots for items in `self.distributions`.
 
         Args:
-            None
+            **kwargs: Additional arguments to be passed to the plotly figure factory.
+                      For available settings see: https://plotly.com/python/reference/layout/
 
         Returns:
             Dictionary of distribution names to plotly go.Figure objects for that distribution.
         """
         res = {}
         if "doc_len" in self.distributions:
             fig_doc_len_dist = ff.create_distplot(
                 [self.analysis.doc_lengths], group_labels=["distplot"], colors=["blue"]
             )
             res["doc_len"] = fig_doc_len_dist
 
         if "word_frequency_zipf" in self.distributions:
             fig_w_freq = go.Figure()
-            # Alternative nice color scales that go together:
-            # Plotly3
-            # ice
             fig_w_freq.add_trace(
                 go.Scattergl(
                     x=self.analysis.zipf_x,
                     y=self.analysis.zipf_y_emp,
                     mode="markers",
                     marker=dict(
                         color=self.analysis.zipf_x,
@@ -87,107 +85,92 @@
                     x=self.analysis.zipf_x,
                     y=self.analysis.zipf_y_theory,
                     mode="markers",
                     marker=dict(color=self.analysis.zipf_x, colorscale="Reds"),
                 )
             )
             res["word_frequency_zipf"] = fig_w_freq
-
-        dist_plot_setup = {
-            # 'paper_bgcolor': '#007A78',
-            "showlegend": False
-        }
+        dist_plot_settings = kwargs.get("plot_settings", {"showlegend": False})
         for _, fig in res.items():
-            fig.update_layout(dist_plot_setup)
+            fig.update_layout(dist_plot_settings)
 
         return res
 
-    def show_distplot(self, distribution: str) -> None:
+    def show_distplot(self, distribution: str, **kwargs) -> None:
         """Shows distribution plots for `dist`.
 
         Args:
             dist (str): The distribution for which the plot is to be shown.
                         Can be either of: doc_len" or "word_frequency_zipf.
+            **kwargs: Additional arguments to be passed to self._create_dist_plots and then plotly figure factory.
+                      For available settings see: https://plotly.com/python/reference/layout/
 
         Returns:
             None
         """
-        self.create_dist_plots()[distribution].show()
+        self._create_dist_plots(**kwargs)[distribution].show()
 
-    def create_pos_plots(
-        self, go_plot_settings: Dict = {}, wc_settings: Dict = {}
-    ) -> Dict[str, go.Figure]:
+    def _create_pos_plots(
+        self,
+        pos: str,
+        **kwargs,
+    ) -> go.Figure:
         """Create plots for the POS tags specified in items in `self.pos_tags`.
 
         Args:
-            go_plot_settings (Dict): Color and other settings for the plotly.graph_objs figure.
-            wc_settings (Dict): Color, font and other settings for wordcloud.WordCloud.
+            pos (str): The POS tag for which the plot is to be shown.
 
         Returns:
             Dictionary of POS tags to plotly go.Figure objects.
 
         """
-        word_cloud_mandatory_settings = {
+        word_cloud_plot_mandatory_settings = {
             "showlegend": False,
             "xaxis_showgrid": False,
             "yaxis_showgrid": False,
             "xaxis_zeroline": False,
             "yaxis_zeroline": False,
             "yaxis_visible": False,
             "yaxis_showticklabels": False,
             "xaxis_visible": False,
             "xaxis_showticklabels": False,
         }
-        word_cloud_setting = {**word_cloud_mandatory_settings, **go_plot_settings}
-        res = {}
-        if "NN" in self.pos_tags:
-            res["noun_cloud"] = go.Figure(
-                plotly_wordcloud(
-                    token_count_dic=self.analysis.nns, settings=wc_settings
-                )
+        plot_settings = kwargs.get("plot_settings", {})
+        plot_settings = {**word_cloud_plot_mandatory_settings, **plot_settings}
+        if pos == "NN" and "NN" in self.pos_tags:
+            return go.Figure(
+                plotly_wordcloud(token_count_dic=self.analysis.nns, **kwargs)
+            ).update_layout(plot_settings)
+        elif pos == "JJ" and "JJ" in self.pos_tags:
+            return go.Figure(
+                plotly_wordcloud(token_count_dic=self.analysis.jjs, **kwargs)
+            ).update_layout(plot_settings)
+        elif pos == "VB" and "VB" in self.pos_tags:
+            return go.Figure(
+                plotly_wordcloud(token_count_dic=self.analysis.vs, **kwargs)
+            ).update_layout(plot_settings)
+        else:
+            raise ValueError(
+                f"Invalid value for pos: {pos}. Valid values are: {self.pos_tags}"
             )
-        if "JJ" in self.pos_tags:
-            res["adj_cloud"] = go.Figure(
-                plotly_wordcloud(
-                    token_count_dic=self.analysis.jjs, settings=wc_settings
-                )
-            )
-        if "VB" in self.pos_tags:
-            res["verb_cloud"] = go.Figure(
-                plotly_wordcloud(token_count_dic=self.analysis.vs, settings=wc_settings)
-            )
-        for _, fig in res.items():
-            fig.update_layout(word_cloud_setting)
-        return res
 
-    def show_word_clouds(
-        self, pos: str, go_plot_settings: Dict = {}, wc_settings: Dict = {}
-    ) -> None:
+    def show_word_clouds(self, pos: str, **kwargs) -> None:
         """Shows POS word clouds.
 
         Args:
             pos (str): Type of POS. Can be any of: [NN, JJ, VB].
-            go_plot_settings (Dict): Color and other settings for the word clouds.
-            wc_settings (Dict): Color, font and other settings for wordcloud.WordCloud.
+            **kwargs: Keyword arguments to be passed to self._create_pos_plots() and wordview.text_analysis.core.plotly_wordcloud().
+              This includes:
+                - plot_settings: Dictionary of form: for self._create_pos_plots(). For available settings see: https://plotly.com/python/reference/layout/.
+                - wc_settings: Dictionary of form: {"color": "<color>", "max_words": int} for core.plotly_wordcloud(). Accepted values are color strings as usable by PIL/Pillow.
 
         Returns:
             None
         """
-        if pos == "NN":
-            self.create_pos_plots(
-                go_plot_settings=go_plot_settings, wc_settings=wc_settings
-            )["noun_cloud"].show()
-        if pos == "JJ":
-            self.create_pos_plots(
-                go_plot_settings=go_plot_settings,
-            )["adj_cloud"].show()
-        if pos == "VB":
-            self.create_pos_plots(
-                go_plot_settings=go_plot_settings,
-            )["verb_cloud"].show()
+        self._create_pos_plots(pos=pos, **kwargs).show()
 
     def show_stats(self) -> None:
         """Print dataset statistics, including:
         Language/s
         Number of unique words
         Number of all words
         Number of documents
@@ -232,19 +215,20 @@
             df (pandas.DataFrame): DataFrame with one or more label column/s.
             label_columns (List): List of tuples (column_name, label_type) that specify a label column and its type (categorical or numerical).
 
         Returns:
             None
         """
         self.df = df
-        self.labels_fig = generate_label_plots(self.df, label_cols=label_columns)
+        self.label_columns = label_columns
 
-    def show_label_plots(self) -> None:
+    def show_label_plots(self, **kwargs) -> None:
         """Renders label plots for columns specified in `self.label_columns`.
 
         Args:
-            None
+            **kwargs: Additional arguments to be passed to generate_label_plots() to be used by plotly.Figure.update_layout(). For more details
+                  see https://plotly.com/python-api-reference/generated/plotly.graph_objects.Figure.html#plotly.graph_objects.Figure.update_layout
 
         Returns:
             None
         """
-        self.labels_fig.show()
+        generate_label_plots(self.df, label_cols=self.label_columns, **kwargs).show()
```

### Comparing `wordview-0.4.1/PKG-INFO` & `wordview-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.4.1
+Version: 0.4.2
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
-|text_analysis_cover|
+|cover|
 
 
 Usage
 ######
 
 Install the package via ``pip``:
 
@@ -120,13 +120,8 @@
 
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
-.. |cover| image:: docs/figs/abstract_cover_2.png
-.. |clustering_cover| image:: docs/figs/clustering_cover.png
-.. |text_analysis_cover| image:: docs/figs/text_analysis.png
-
-
-
+.. |cover| image:: docs/figs/cover.png
```

