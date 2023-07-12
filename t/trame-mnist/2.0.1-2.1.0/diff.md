# Comparing `tmp/trame-mnist-2.0.1.tar.gz` & `tmp/trame-mnist-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-mnist-2.0.1.tar", last modified: Mon May 30 23:21:30 2022, max compression
+gzip compressed data, was "trame-mnist-2.1.0.tar", last modified: Wed Jul 12 23:07:14 2023, max compression
```

## Comparing `trame-mnist-2.0.1.tar` & `trame-mnist-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.190652 trame-mnist-2.0.1/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     1504 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/LICENSE
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       36 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/MANIFEST.in
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     2856 2022-05-30 23:21:30.190753 trame-mnist-2.0.1/PKG-INFO
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     2084 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/README.rst
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     1150 2022-05-30 23:21:30.191388 trame-mnist-2.0.1/setup.cfg
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       38 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/setup.py
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.173332 trame-mnist-2.0.1/trame_mnist/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       49 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/__init__.py
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.181499 trame-mnist-2.0.1/trame_mnist/app/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       50 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/__init__.py
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.183214 trame-mnist-2.0.1/trame_mnist/app/engine/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       62 2022-05-30 16:12:02.000000 trame-mnist-2.0.1/trame_mnist/app/engine/__init__.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     5161 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/engine/charts.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     7240 2022-05-30 23:19:41.000000 trame-mnist-2.0.1/trame_mnist/app/engine/main.py
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.190488 trame-mnist-2.0.1/trame_mnist/app/engine/ml/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      492 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/__init__.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     5781 2022-05-30 16:50:28.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/common.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      886 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/prediction.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     1032 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/testing.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     1569 2022-05-30 16:22:43.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/training.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     1767 2022-02-18 03:03:59.000000 trame-mnist-2.0.1/trame_mnist/app/engine/ml/xai.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      662 2022-05-30 17:03:03.000000 trame-mnist-2.0.1/trame_mnist/app/jupyter.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      740 2022-05-30 16:50:28.000000 trame-mnist-2.0.1/trame_mnist/app/main.py
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)    13118 2022-05-30 16:50:28.000000 trame-mnist-2.0.1/trame_mnist/app/ui.py
-drwxr-xr-x   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        0 2022-05-30 23:21:30.177391 trame-mnist-2.0.1/trame_mnist.egg-info/
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)     2856 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/PKG-INFO
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      707 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)        1 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       50 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/entry_points.txt
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)      256 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/requires.txt
--rw-r--r--   0 sebastien.jourdain (849467605) KHQ\Domain Users (1034492881)       12 2022-05-30 23:21:30.000000 trame-mnist-2.0.1/trame_mnist.egg-info/top_level.txt
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1504 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/LICENSE
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       36 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/MANIFEST.in
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     2723 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/PKG-INFO
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1932 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/README.rst
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1147 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/setup.cfg
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       38 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/setup.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.570912 trame-mnist-2.1.0/trame_mnist/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       49 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/trame_mnist/app/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       50 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/trame_mnist/app/engine/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       62 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/__init__.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     6889 2023-07-12 22:57:25.000000 trame-mnist-2.1.0/trame_mnist/app/engine/charts.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     7240 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/main.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.574912 trame-mnist-2.1.0/trame_mnist/app/engine/ml/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      492 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/__init__.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     5854 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/common.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      886 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/prediction.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1032 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/testing.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1569 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/training.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1767 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/engine/ml/xai.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      662 2023-07-12 20:16:14.000000 trame-mnist-2.1.0/trame_mnist/app/jupyter.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      739 2023-07-12 22:57:25.000000 trame-mnist-2.1.0/trame_mnist/app/main.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)    14464 2023-07-12 23:03:06.000000 trame-mnist-2.1.0/trame_mnist/app/ui.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 23:07:14.570912 trame-mnist-2.1.0/trame_mnist.egg-info/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     2723 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      707 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        1 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       50 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      252 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/requires.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       12 2023-07-12 23:07:14.000000 trame-mnist-2.1.0/trame_mnist.egg-info/top_level.txt
```

### Comparing `trame-mnist-2.0.1/LICENSE` & `trame-mnist-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/PKG-INFO` & `trame-mnist-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: trame-mnist
-Version: 2.0.1
+Version: 2.1.0
 Summary: Visualization exploration for AI/XAI
+Home-page: UNKNOWN
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -49,16 +50,14 @@
 .. code-block:: console
 
     # Needed in order to get py3.9 with lzma
     # PYTHON_CONFIGURE_OPTS="--enable-framework" pyenv install 3.9.9
 
     conda create --name trame-mnist python=3.9
     conda activate trame-mnist
-    conda install "pytorch==1.9.1" "torchvision==0.10.1" -c pytorch
-    conda install scipy "scikit-learn==0.24.2" "scikit-image==0.18.3" -c conda-forge
 
     # For development when inside repo
     pip install -e .
 
     # For testing (no need to clone repo)
     pip install trame-mnist
 
@@ -84,7 +83,8 @@
   :width: 32%
 
 License
 --------
 
 **trame-mnist** is distributed under the OSI-approved BSD 3-clause License.
 
+
```

### Comparing `trame-mnist-2.0.1/README.rst` & `trame-mnist-2.1.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 .. code-block:: console
 
     # Needed in order to get py3.9 with lzma
     # PYTHON_CONFIGURE_OPTS="--enable-framework" pyenv install 3.9.9
 
     conda create --name trame-mnist python=3.9
     conda activate trame-mnist
-    conda install "pytorch==1.9.1" "torchvision==0.10.1" -c pytorch
-    conda install scipy "scikit-learn==0.24.2" "scikit-image==0.18.3" -c conda-forge
 
     # For development when inside repo
     pip install -e .
 
     # For testing (no need to clone repo)
     pip install trame-mnist
 
@@ -62,8 +60,8 @@
   :width: 32%
 .. |image_3| image:: https://github.com/Kitware/trame-mnist/raw/master/gallery/trame-mnist-04.jpg
   :width: 32%
 
 License
 --------
 
-**trame-mnist** is distributed under the OSI-approved BSD 3-clause License.
+**trame-mnist** is distributed under the OSI-approved BSD 3-clause License.
```

### Comparing `trame-mnist-2.0.1/setup.cfg` & `trame-mnist-2.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-mnist
-version = 2.0.1
+version = 2.1.0
 description = Visualization exploration for AI/XAI
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -23,26 +23,27 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
-	trame>=2.0.0rc2
-	altair==4.1.0
-	torch>=1.9.1
-	torchvision>=0.10.0,<=0.10.1
+	trame>=2.1.0
+	plotly==5.15.0
+	pandas
+	torch==1.10.0
+	torchvision==0.11.1
 	smqtk-classifier==0.19.0
-	smqtk-core==0.18.1
-	smqtk-dataprovider==0.16.0
-	smqtk-descriptors==0.18.1
-	smqtk-image-io==0.16.2
-	xaitk-saliency==0.4.0
-	scikit-learn==0.24.2
-	scikit-image==0.18.3
+	smqtk-core==0.19.0
+	smqtk-dataprovider==0.18.0
+	smqtk-descriptors==0.19.0
+	smqtk-image-io==0.17.1
+	xaitk-saliency==0.7.0
+	scikit-learn==1.3.0
+	scikit-image==0.21.0
 
 [options.entry_points]
 console_scripts = 
 	trame-mnist = trame_mnist:main
 
 [egg_info]
 tag_build =
```

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/main.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/main.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/ml/common.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/ml/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 
 MODEL_PATH = Path(DATA_DIR, "model_lenet-5.trained").resolve().absolute()
 
 TRANSFORM = transforms.Compose(
     [transforms.ToTensor(), transforms.Normalize((0,), (1,))]
 )
 
-DEVICE = torch.device("cpu")
+DEVICE = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
 
 
 def update_ml_device(cpu_only=True):
+    global DEVICE
     if not cpu_only and torch.cuda.is_available():
         DEVICE = torch.device("cuda")
         print(" ~~~ Using GPU ~~~ \n")
     else:
         print(" ~~~ Using CPU ~~~ \n")
```

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/ml/prediction.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/ml/prediction.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/ml/testing.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/ml/testing.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/ml/training.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/ml/training.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/engine/ml/xai.py` & `trame-mnist-2.1.0/trame_mnist/app/engine/ml/xai.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/jupyter.py` & `trame-mnist-2.1.0/trame_mnist/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-mnist-2.0.1/trame_mnist/app/main.py` & `trame-mnist-2.1.0/trame_mnist/app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,8 @@
     ui.initialize(server)
 
     # Start server
     server.start(**kwargs)
 
 
 if __name__ == "__main__":
-
     main()
```

### Comparing `trame-mnist-2.0.1/trame_mnist/app/ui.py` & `trame-mnist-2.1.0/trame_mnist/app/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from trame.ui.vuetify import SinglePageLayout
-from trame.widgets import vega, vuetify, html, trame
+from trame.widgets import plotly, vuetify, html, trame
 
 TITLE = "MNIST Exploration"
 
 
 def initialize(server):
     state, ctrl = server.state, server.controller
 
@@ -158,22 +158,32 @@
                             disabled=("training_running",),
                         )
 
                 # Training page
                 with vuetify.VCol(
                     v_if="view_mode == 'training' && model_state.epoch > 1"
                 ):
-                    chart_acc = vega.Figure(
-                        style="width: 100%;",
+                    # chart_acc = vega.Figure(
+                    #     style="width: 100%;",
+                    #     v_show="view_mode === 'training'",
+                    # )
+                    chart_acc = plotly.Figure(
+                        style="width: 100%; height: 100%;",
                         v_show="view_mode === 'training'",
+                        display_mode_bar=False,
                     )
                     ctrl.chart_acc_update = chart_acc.update
-                    chart_loss = vega.Figure(
-                        style="width: 100%;",
+                    # chart_loss = vega.Figure(
+                    #     style="width: 100%;",
+                    #     v_show="view_mode === 'training'",
+                    # )
+                    chart_loss = plotly.Figure(
+                        style="width: 100%; height: 100%;",
                         v_show="view_mode === 'training'",
+                        display_mode_bar=False,
                     )
                     ctrl.chart_loss_update = chart_loss.update
 
                 # Execution page
                 with vuetify.VRow(
                     v_if="view_mode == 'execution'",
                     classes="pa-3 ma-2",
@@ -206,17 +216,21 @@
                                             max_width=200,
                                             min_width=200,
                                             __properties=["v_bind", "v_on"],
                                         )
                                     html.Span("{{ prediction_label }}")
 
                     with vuetify.VCol(align_self="center", cols=8):
-                        chart_pred = vega.Figure(
-                            style="width: 100%; display: flex;",
+                        chart_pred = plotly.Figure(
+                            style="width: 100%; height: 100%;",
+                            display_mode_bar=False,
                         )
+                        # chart_pred = vega.Figure(
+                        #     style="width: 100%; display: flex;",
+                        # )
                         ctrl.chart_pred_update = chart_pred.update
 
                 # Execution page
                 with vuetify.VCol(v_if="view_mode == 'execution'"):
                     with vuetify.VRow(classes="px-0 ma-0"):
                         with vuetify.VCol(
                             v_for=("i in 10",), key="i", classes="pa-0 ma-0"
@@ -268,23 +282,35 @@
                 with vuetify.VRow(
                     v_if="view_mode == 'testing'",
                     classes="pa-3 ma-2 overflow-hidden",
                     align="center",
                     justify="center",
                     style="height: 100%; max-height: calc(100vh - 64px);",
                 ):
-                    chart_confusion_matrix = vega.Figure(
+                    # chart_confusion_matrix = vega.Figure(
+                    #     v_show="view_mode == 'testing' && testing_count",
+                    #     style="width: 50%;",
+                    #     key="`${testing_count}-matrix`",
+                    # )
+                    chart_confusion_matrix = plotly.Figure(
                         v_show="view_mode == 'testing' && testing_count",
-                        style="width: 50%;",
+                        style="width: 50%; heigh: 100%;",
+                        display_mode_bar=False,
                         key="`${testing_count}-matrix`",
                     )
                     ctrl.chart_confusion_matrix = chart_confusion_matrix.update
 
-                    chart_class_accuracy = vega.Figure(
+                    # chart_class_accuracy = vega.Figure(
+                    #     v_show="view_mode == 'testing' && testing_count",
+                    #     style="width: 50%;",
+                    #     key="`${testing_count}-class`",
+                    # )
+                    chart_class_accuracy = plotly.Figure(
                         v_show="view_mode == 'testing' && testing_count",
-                        style="width: 50%;",
+                        style="width: 50%; heigh: 100%;",
+                        display_mode_bar=False,
                         key="`${testing_count}-class`",
                     )
                     ctrl.chart_class_accuracy = chart_class_accuracy.update
 
         # Footer
         # layout.footer.hide()
```

### Comparing `trame-mnist-2.0.1/trame_mnist.egg-info/PKG-INFO` & `trame-mnist-2.1.0/trame_mnist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: trame-mnist
-Version: 2.0.1
+Version: 2.1.0
 Summary: Visualization exploration for AI/XAI
+Home-page: UNKNOWN
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
@@ -49,16 +50,14 @@
 .. code-block:: console
 
     # Needed in order to get py3.9 with lzma
     # PYTHON_CONFIGURE_OPTS="--enable-framework" pyenv install 3.9.9
 
     conda create --name trame-mnist python=3.9
     conda activate trame-mnist
-    conda install "pytorch==1.9.1" "torchvision==0.10.1" -c pytorch
-    conda install scipy "scikit-learn==0.24.2" "scikit-image==0.18.3" -c conda-forge
 
     # For development when inside repo
     pip install -e .
 
     # For testing (no need to clone repo)
     pip install trame-mnist
 
@@ -84,7 +83,8 @@
   :width: 32%
 
 License
 --------
 
 **trame-mnist** is distributed under the OSI-approved BSD 3-clause License.
 
+
```

### Comparing `trame-mnist-2.0.1/trame_mnist.egg-info/SOURCES.txt` & `trame-mnist-2.1.0/trame_mnist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

