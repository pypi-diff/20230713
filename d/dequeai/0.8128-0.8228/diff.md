# Comparing `tmp/dequeai-0.8128.tar.gz` & `tmp/dequeai-0.8228.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.8128.tar", last modified: Mon Jul 10 23:27:34 2023, max compression
+gzip compressed data, was "dequeai-0.8228.tar", last modified: Wed Jul 12 23:23:36 2023, max compression
```

## Comparing `dequeai-0.8128.tar` & `dequeai-0.8228.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:27:34.627504 dequeai-0.8128/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-10 23:27:34.627504 dequeai-0.8128/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:27:34.623504 dequeai-0.8128/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8128/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15433 2023-07-10 19:19:44.000000 dequeai-0.8128/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8128/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8128/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8128/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    15159 2023-07-10 23:27:01.000000 dequeai-0.8128/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8128/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8128/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8128/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8128/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8128/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 23:27:34.627504 dequeai-0.8128/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-10 23:27:34.000000 dequeai-0.8128/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-10 23:27:34.000000 dequeai-0.8128/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 23:27:34.000000 dequeai-0.8128/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-10 23:27:34.000000 dequeai-0.8128/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 23:27:34.000000 dequeai-0.8128/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 23:27:34.627504 dequeai-0.8128/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-10 23:27:14.000000 dequeai-0.8128/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 23:23:36.488532 dequeai-0.8228/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-12 23:23:36.488532 dequeai-0.8228/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 23:23:36.488532 dequeai-0.8228/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8228/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16590 2023-07-12 23:21:11.000000 dequeai-0.8228/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8228/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8228/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8228/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8228/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8228/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8228/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8228/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8228/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8228/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 23:23:36.488532 dequeai-0.8228/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-12 23:23:36.000000 dequeai-0.8228/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-12 23:23:36.000000 dequeai-0.8228/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 23:23:36.000000 dequeai-0.8228/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-12 23:23:36.000000 dequeai-0.8228/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 23:23:36.000000 dequeai-0.8228/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 23:23:36.488532 dequeai-0.8228/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-12 23:23:23.000000 dequeai-0.8228/setup.py
```

### Comparing `dequeai-0.8128/dequeai/datatypes.py` & `dequeai-0.8228/dequeai/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import json
 import time
 import dequeai.util as util
 import numpy as np
 from dequeai.util import DEQUE_IMAGE, DEQUE_HISTOGRAM, DEQUE_AUDIO, DEQUE_TEXT, DEQUE_TABLE, DEQUE_VIDEO, \
     DEQUE_BOUNDING_BOX, DEQUE_PLOT
 from dequeai.util import *
-#import altair
+
+
+# import altair
 
 
 class BoundingBox2D():
     _type = DEQUE_BOUNDING_BOX
 
     def __init__(self, coordinates, domain=None, scores=None, caption=None):
         self.coordinates = coordinates
@@ -53,14 +55,35 @@
                 self._process_image(d, mode)
 
                 if box_data is not None:
                     for b in box_data[i]:
                         if not isinstance(b, BoundingBox2D):
                             raise ValueError("All elements in box_data list must be BoundingBox2d objects")
                     self._box_data.append(box_data[i])
+        elif isinstance(data, np.ndarray):
+            if data.ndim == 3:
+                self._process_image(data, mode)
+                if box_data is not None:
+                    if not isinstance(box_data, list):
+                        raise ValueError("box_data must be a list of BoundingBox2d objects")
+                    for b in box_data:
+                        if not isinstance(b, BoundingBox2D):
+                            raise ValueError("All elements in box_data list must be BoundingBox2d objects")
+                    self._box_data.append(box_data)
+            elif data.ndim == 4:
+                for i, d in enumerate(data):
+                    self._process_image(d, mode)
+                    if box_data is not None:
+                        for b in box_data[i]:
+                            if not isinstance(b, BoundingBox2D):
+                                raise ValueError("All elements in box_data list must be BoundingBox2d objects")
+                        self._box_data.append(box_data[i])
+            else:
+                raise ValueError("numpy array must be 3 or 4 dimensional")
+
         else:
             self._process_image(data, mode)
 
             if box_data is not None:
                 if not isinstance(box_data, list):
                     raise ValueError("box_data must be a list of BoundingBox2d objects")
                 for b in box_data:
@@ -83,16 +106,14 @@
                 d = d.numpy()
             if d.ndim > 2:
                 d = d.squeeze()  # get rid of trivial dimensions as a convenience
             self._images.append(
                 self.to_uint8(d)
             )
 
-
-
     def _validate_size(self):
         pass
 
     def _tensor_to_numpy_image(self, torch_module, pic, mode):
 
         if not (isinstance(pic, torch_module.Tensor) or isinstance(pic, np.ndarray)):
             raise TypeError(f"pic should be Tensor or ndarray. Got {type(pic)}.")
@@ -282,14 +303,15 @@
         # "The maximum length of a histogram is %i" % cls.MAX_LENGTH
         # )
         # if len(histogram) + 1 != len(bins):
         # raise ValueError("len(bins) must be len(histogram) + 1")
 
         return cls(np_histogram=np_histogram)
 
+
 class Audio:
     _type = 'DEQUE_AUDIO'
 
     def __init__(self, data, sample_rate=None, caption=None):
         """Accepts a numpy array of audio data."""
         self._sample_rate = sample_rate
         self._caption = caption
@@ -325,15 +347,14 @@
         return self._sample_rate
 
     @property
     def caption(self):
         return self._caption
 
 
-
 class Video:
     _type = DEQUE_VIDEO
 
 
 class Text:
     _type = DEQUE_TEXT
 
@@ -392,15 +413,15 @@
 
         for row in data:
             if not isinstance(row, list):
                 raise TypeError("data argument must be a list (rows) of list (column values)")
 
             for column_val in row:
                 if not isinstance(column_val, (
-                Image, Audio, Video, Text, Histogram)) and not column_val.__class__.__module__ == 'builtins':
+                        Image, Audio, Video, Text, Histogram)) and not column_val.__class__.__module__ == 'builtins':
                     print("checking whether it is builtin datatype")
                     print(column_val.__class__.__module__)
                     print("checking whether it is deque datatype")
                     print(isinstance(column_val, (Image, Audio, Video, Text, Histogram)))
                     raise TypeError("Each column value must be a deque datatype or a builtin python type")
 
     def _validate_columns(self, columns):
@@ -432,36 +453,38 @@
         js_rep = self._altair_chart.to_json()
         return js_rep
 
     def to_vega_json(self):
         return self._vega_json
 
     def to_json(self):
-        return {"data":self._data,"plot_type":self._plot_type,"plot_attributes":self._plot_attributes,"vega_json":self._vega_json,"datatype":Plot._type}
+        return {"data": self._data, "plot_type": self._plot_type, "plot_attributes": self._plot_attributes,
+                "vega_json": self._vega_json, "datatype": Plot._type}
+
 
 if __name__ == "__main__":
     # bins = [0,1, 2, 3]
     # h = np.histogram([1,2,1], bins=bins)
     import matplotlib.pyplot as plt
 
     # plt.hist(h)
     # plt.hist(h, bins=bins)
     # plt.show()
     # dh = Histogram(np_histogram=h)
     # dh=Histogram.from_sequence(sequence=[0,2,1], num_bins=[0,1,2,3])
-    #import altair as alt
+    # import altair as alt
     import pandas as pd
 
     source = pd.DataFrame({
         'a': ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I'],
         'b': [28, 55, 43, 91, 81, 53, 19, 87, 52]
     })
 
-    #chart = alt.Chart(source).mark_bar().encode(
-     #   x='a',
-     #   y='b'
-    #)
+    # chart = alt.Chart(source).mark_bar().encode(
+    #   x='a',
+    #   y='b'
+    # )
 
-    #pl = Plot(altair_chart=chart)
-    #print(pl.to_vega_json())
+    # pl = Plot(altair_chart=chart)
+    # print(pl.to_vega_json())
```

### Comparing `dequeai-0.8128/dequeai/dequeai.py` & `dequeai-0.8228/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8128/dequeai/dequeai_model.py` & `dequeai-0.8228/dequeai/dequeai_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,31 +60,31 @@
                training_date: str, model_license: str, dependencies: list, pretrained: str,
                model_description: Optional[str] = None,
                limitations: Optional[str] = None, intended_users: Optional[str] = None,
                training_data_size: Optional[str] = None,
                training_data_size_units: Optional[str] = None, training_data_description: Optional[str] = None,
                training_data_source: Optional[str] = None,
                citation: Optional[str] = None):
-        self._model_name = model_name
-        self._task_category = task_category
-        self._task = task
-        self._model_architecture = model_architecture
-        self._model_description = model_description
-        self._model_version = model_version
-        self._limitations = limitations
-        self._intended_users = intended_users
-        self._training_data_size = training_data_size
-        self._training_data_size_units = training_data_size_units
-        self._training_data_description = training_data_description
-        self._training_data_source = training_data_source
-        self._training_date = training_date
-        self._license = model_license
-        self._citation = citation
-        self._dependencies = dependencies
-        self._pretrained = pretrained
+        self.model_name = model_name
+        self.task_category = task_category
+        self.task = task
+        self.model_architecture = model_architecture
+        self.model_description = model_description
+        self.model_version = model_version
+        self.limitations = limitations
+        self.intended_users = intended_users
+        self.training_data_size = training_data_size
+        self.training_data_size_units = training_data_size_units
+        self.training_data_description = training_data_description
+        self.training_data_source = training_data_source
+        self.training_date = training_date
+        self.license = model_license
+        self.citation = citation
+        self.dependencies = dependencies
+        self.pretrained = pretrained
 
         return self
 
     def to_dict(self):
         return self.__dict__
 
     def to_json(self):
@@ -94,181 +94,181 @@
         self.__dict__ = d
 
     def from_json(self, j):
         self.__dict__ = json.loads(j)
 
     @property
     def task_category(self) -> Optional[str]:
-        return self._task_category
+        return self.task_category
 
     @task_category.setter
     def task_category(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("task_category must be a string or None.")
-        self._task_category = value
+        self.task_category = value
 
     @property
     def task(self) -> Optional[str]:
-        return self._task
+        return self.task
 
     @task.setter
     def task(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("task must be a string or None.")
-        self._task = value
+        self.task = value
 
     @property
     def model_name(self) -> Optional[str]:
-        return self._model_name
+        return self.model_name
 
     @model_name.setter
     def model_name(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("model_name must be a string or None.")
-        self._model_name = value
+        self.model_name = value
 
     @property
     def model_architecture(self) -> Optional[str]:
-        return self._model_architecture
+        return self.model_architecture
 
     @model_architecture.setter
     def model_architecture(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("model_architecture must be a string or None.")
-        self._model_architecture = value
+        self.model_architecture = value
 
     @property
     def model_description(self) -> Optional[str]:
-        return self._model_description
+        return self.model_description
 
     @model_description.setter
     def model_description(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("model_description must be a string or None.")
-        self._model_description = value
+        self.model_description = value
 
     @property
     def model_version(self) -> Optional[str]:
         return self._model_version
 
     @model_version.setter
     def model_version(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("model_version must be a string or None.")
-        self._model_version = value
+        self.model_version = value
 
     @property
     def limitations(self) -> Optional[str]:
-        return self._limitations
+        return self.limitations
 
     @limitations.setter
     def limitations(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("limitations must be a string or None.")
-        self._limitations = value
+        self.limitations = value
 
     @property
     def intended_users(self) -> Optional[str]:
-        return self._intended_users
+        return self.intended_users
 
     @intended_users.setter
     def intended_users(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("intended_users must be a string or None.")
-        self._intended_users = value
+        self.intended_users = value
 
     @property
     def training_data_size(self) -> Optional[str]:
-        return self._training_data_size
+        return self.training_data_size
 
     @training_data_size.setter
     def training_data_size(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("training_data_size must be a string or None.")
-        self._training_data_size = value
+        self.training_data_size = value
 
     @property
     def training_data_size_units(self) -> Optional[str]:
-        return self._training_data_size_units
+        return self.training_data_size_units
 
     @training_data_size_units.setter
     def training_data_size_units(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("training_data_size_units must be a string or None.")
-        self._training_data_size_units = value
+        self.training_data_size_units = value
 
     @property
     def training_data_description(self) -> Optional[str]:
-        return self._training_data_description
+        return self.training_data_description
 
     @training_data_description.setter
     def training_data_description(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("training_data_description must be a string or None.")
-        self._training_data_description = value
+        self.training_data_description = value
 
     @property
     def training_data_source(self) -> Optional[str]:
-        return self._training_data_source
+        return self.training_data_source
 
     @training_data_source.setter
     def training_data_source(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("training_data_source must be a string or None.")
-        self._training_data_source = value
+        self.training_data_source = value
 
     @property
     def training_date(self) -> Optional[str]:
-        return self._training_date
+        return self.training_date
 
     @training_date.setter
     def training_date(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("training_date must be a string or None.")
-        self._training_date = value
+        self.training_date = value
 
     @property
     def citation(self) -> Optional[str]:
-        return self._citation
+        return self.citation
 
     @citation.setter
     def citation(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("citation must be a string or None.")
-        self._citation = value
+        self.citation = value
 
     @property
     def license(self) -> Optional[str]:
-        return self._license
+        return self.license
 
     @license.setter
     def license(self, value: Optional[str]) -> None:
         if value is not None and not isinstance(value, str):
             raise ValueError("license must be a string or None.")
-        self._license = value
+        self.license = value
 
     @property
     def dependencies(self) -> Optional[str]:
-        return self._dependencies
+        return self.dependencies
 
     @dependencies.setter
     def dependencies(self, value: Optional[str]) -> None:
         if value is not isinstance(value, list):
             raise ValueError("dependencies must be a list")
-        self._dependencies = value
+        self.dependencies = value
 
     @property
     def pretrained(self) -> Optional[str]:
-        return self._pretrained
+        return self.pretrained
 
     @pretrained.setter
     def pretrained(self, value: Optional[str]) -> None:
         if value is not isinstance(value, bool):
             raise ValueError("pretrained must be a boolean")
-        self._pretrained = value
+        self.pretrained = value
 
 
 
 
 class Model:
 
     def __init__(self):
```

### Comparing `dequeai-0.8128/dequeai/dequeai_run.py` & `dequeai-0.8228/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8128/dequeai/parsing_service.py` & `dequeai-0.8228/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8128/dequeai/rest_connect.py` & `dequeai-0.8228/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8128/dequeai/util.py` & `dequeai-0.8228/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8128/setup.py` & `dequeai-0.8228/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000008128',
+    version='0.000008228',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

