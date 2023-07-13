# Comparing `tmp/SPACEL-1.1.1.tar.gz` & `tmp/SPACEL-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPACEL-1.1.1.tar", last modified: Tue Jul 11 12:51:44 2023, max compression
+gzip compressed data, was "dist/SPACEL-1.1.2.tar", last modified: Thu Jul 13 01:20:57 2023, max compression
```

## Comparing `SPACEL-1.1.1.tar` & `SPACEL-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.027290 SPACEL-1.1.1/
--rw-r--r--   0 xuhao      (501) staff       (20)     3655 2023-07-11 12:51:44.026958 SPACEL-1.1.1/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)     3354 2023-07-11 12:50:36.000000 SPACEL-1.1.1/README.md
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.938820 SPACEL-1.1.1/SPACEL/
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.958498 SPACEL-1.1.1/SPACEL/Scube/
--rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.1/SPACEL/Scube/alignment.py
--rw-r--r--   0 xuhao      (501) staff       (20)    14330 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/gpr.py
--rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/plot.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4381 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Scube/utils_3d.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.996974 SPACEL-1.1.1/SPACEL/Splane/
--rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.1/SPACEL/Splane/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/graph.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.011126 SPACEL-1.1.1/SPACEL/Splane/kegra/
--rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/gnn.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/kegra/gnn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Splane/pygcn_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4225 2023-07-11 09:00:10.000000 SPACEL-1.1.1/SPACEL/Splane/utils.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:44.026063 SPACEL-1.1.1/SPACEL/Spoint/
--rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.1/SPACEL/Spoint/base_model.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_augmentation.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_downsample.py
--rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/data_utils.py
--rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/metrics.py
--rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/model.py
--rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/Spoint/spatial_simulation.py
--rw-r--r--   0 xuhao      (501) staff       (20)      745 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/__init__.py
--rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-11 12:50:36.000000 SPACEL-1.1.1/SPACEL/_version.py
--rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.1/SPACEL/setting.py
-drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-11 12:51:43.941235 SPACEL-1.1.1/SPACEL.egg-info/
--rw-r--r--   0 xuhao      (501) staff       (20)     3655 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/PKG-INFO
--rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/SOURCES.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/dependency_links.txt
--rw-r--r--   0 xuhao      (501) staff       (20)      120 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/requires.txt
--rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-11 12:51:43.000000 SPACEL-1.1.1/SPACEL.egg-info/top_level.txt
--rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-11 12:51:44.027378 SPACEL-1.1.1/setup.cfg
--rw-r--r--   0 xuhao      (501) staff       (20)      908 2023-07-11 12:48:07.000000 SPACEL-1.1.1/setup.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:57.091735 SPACEL-1.1.2/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4046 2023-07-13 01:20:57.091297 SPACEL-1.1.2/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)     3708 2023-07-12 13:44:19.000000 SPACEL-1.1.2/README.md
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:56.971259 SPACEL-1.1.2/SPACEL/
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:56.997592 SPACEL-1.1.2/SPACEL/Scube/
+-rw-r--r--   0 xuhao      (501) staff       (20)      151 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Scube/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    13309 2023-07-11 12:14:50.000000 SPACEL-1.1.2/SPACEL/Scube/alignment.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    16402 2023-07-13 00:51:58.000000 SPACEL-1.1.2/SPACEL/Scube/gpr.py
+-rw-r-----   0 xuhao      (501) staff       (20)     6191 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Scube/plot.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6635 2023-07-12 13:05:31.000000 SPACEL-1.1.2/SPACEL/Scube/utils_3d.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:57.051881 SPACEL-1.1.2/SPACEL/Splane/
+-rw-r--r--   0 xuhao      (501) staff       (20)      149 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    15183 2023-07-11 12:20:57.000000 SPACEL-1.1.2/SPACEL/Splane/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1627 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/graph.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:57.074444 SPACEL-1.1.2/SPACEL/Splane/kegra/
+-rw-r--r--   0 xuhao      (501) staff       (20)        0 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/kegra/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4662 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/kegra/gnn.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4658 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/kegra/gnn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     3688 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     2050 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Splane/pygcn_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4269 2023-07-12 12:05:55.000000 SPACEL-1.1.2/SPACEL/Splane/utils.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:57.090736 SPACEL-1.1.2/SPACEL/Spoint/
+-rw-r--r--   0 xuhao      (501) staff       (20)      138 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    27194 2023-07-11 09:03:42.000000 SPACEL-1.1.2/SPACEL/Spoint/base_model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1332 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/data_augmentation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4007 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/data_downsample.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     6788 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/data_utils.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     1017 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/metrics.py
+-rw-r--r--   0 xuhao      (501) staff       (20)     4998 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/model.py
+-rw-r--r--   0 xuhao      (501) staff       (20)    20829 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/Spoint/spatial_simulation.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      226 2023-07-12 13:29:08.000000 SPACEL-1.1.2/SPACEL/__init__.py
+-rw-r--r--   0 xuhao      (501) staff       (20)       32 2023-07-12 13:26:39.000000 SPACEL-1.1.2/SPACEL/_version.py
+-rw-r--r--   0 xuhao      (501) staff       (20)      719 2023-07-11 08:15:35.000000 SPACEL-1.1.2/SPACEL/setting.py
+drwxr-xr-x   0 xuhao      (501) staff       (20)        0 2023-07-13 01:20:56.972915 SPACEL-1.1.2/SPACEL.egg-info/
+-rw-r--r--   0 xuhao      (501) staff       (20)     4046 2023-07-13 01:20:56.000000 SPACEL-1.1.2/SPACEL.egg-info/PKG-INFO
+-rw-r--r--   0 xuhao      (501) staff       (20)      818 2023-07-13 01:20:56.000000 SPACEL-1.1.2/SPACEL.egg-info/SOURCES.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        1 2023-07-13 01:20:56.000000 SPACEL-1.1.2/SPACEL.egg-info/dependency_links.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)      120 2023-07-13 01:20:56.000000 SPACEL-1.1.2/SPACEL.egg-info/requires.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)        7 2023-07-13 01:20:56.000000 SPACEL-1.1.2/SPACEL.egg-info/top_level.txt
+-rw-r--r--   0 xuhao      (501) staff       (20)       38 2023-07-13 01:20:57.091844 SPACEL-1.1.2/setup.cfg
+-rw-r--r--   0 xuhao      (501) staff       (20)      908 2023-07-11 12:48:07.000000 SPACEL-1.1.2/setup.py
```

### Comparing `SPACEL-1.1.1/PKG-INFO` & `SPACEL-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: SPACEL
-Version: 1.1.1
-Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
-Home-page: https://github.com/QuKunLab/SPACEL
-Author: Hao Xu
-Author-email: xuhaoustc@mail.ustc.edu.cn
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
@@ -27,14 +17,21 @@
     * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
     * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.2 2023-07-12
+#### Fixed Bugs
+- Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
+- Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
+#### Features
+- Added function documentations for Scube related to the GPR model.
+
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
@@ -42,15 +39,15 @@
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
-conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 r-base r-fitdistrplus
+conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
 * Test if [PyTorch](https://pytorch.org) for GPU available:
 ```
 python
 >>> import torch
 >>> torch.cuda.is_available()
```

### Comparing `SPACEL-1.1.1/README.md` & `SPACEL-1.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: SPACEL
+Version: 1.1.2
+Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
+Home-page: https://github.com/QuKunLab/SPACEL
+Author: Hao Xu
+Author-email: xuhaoustc@mail.ustc.edu.cn
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
 
 ![](docs/_static/img/figure1.png "Overview")
 SPACEL (**SP**atial **A**rchitecture **C**haracterization by d**E**ep **L**earning) is a Python package of deep-learning-based methods for ST data analysis. SPACEL consists of three modules: 
@@ -17,14 +29,21 @@
     * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
     * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.2 2023-07-12
+#### Fixed Bugs
+- Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
+- Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
+#### Features
+- Added function documentations for Scube related to the GPR model.
+
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
@@ -32,15 +51,15 @@
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
-conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 r-base r-fitdistrplus
+conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
 * Test if [PyTorch](https://pytorch.org) for GPU available:
 ```
 python
 >>> import torch
 >>> torch.cuda.is_available()
@@ -50,7 +69,9 @@
 Note: If you want to run 3D expression GPR model in Scube, you need to install the [Open3D](http://www.open3d.org/docs/release/) python library first.
 
 ## Installation
 * Install `SPACEL`:
 ```
 pip install SPACEL
 ```
+
+
```

### Comparing `SPACEL-1.1.1/SPACEL/Scube/alignment.py` & `SPACEL-1.1.2/SPACEL/Scube/alignment.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Scube/gpr.py` & `SPACEL-1.1.2/SPACEL/Scube/gpr.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,16 +20,40 @@
 
     def forward(self, x):
         mean_x = self.mean_module(x)
         covar_x = self.covar_module(x)
         return gpytorch.distributions.MultivariateNormal(mean_x, covar_x)
 
 class GPRmodel():
+    """The GPR model class.
+
+    The GPR model class for prediction of 3D spatial transcriptomic data.
+
+    Attributes:
+        used_genes: A list of gene names used for selecting genes as input.
+        log_bf: The log Bayes factor (BF) value indicating the variation of each gene in 3D spatial data.
+        use_gpu: A boolean value indicating whether to use the GPU for training.
+        subset: An integer value indicating the number of spots/cells to be downsampled for training.
+        lengthscale_prior: The prior value of the lengthscale parameter in the Gaussian Process Regression (GPR) model.
+        outputscale_prior: The prior value of the outputscale parameter in the GPR model.
+        noise_prior: The prior value of the noise parameter in the GPR model.
+        output_dir: The path where the outputs will be saved.
+    """
+
     def __init__(self,expr,loc,loc_resample,used_genes,use_gpu=False,output_dir=None,**kwargs):
-        
+        """Initializes the instance of GPR model class.
+
+        Args:
+            expr: A matrix of expression values at each location in the spatial transcriptomic data.
+            loc: A matrix of coordinate values at each location in the spatial transcriptomic data.
+            loc_resample: A matrix of coordinate values at each location in the resampled data.
+            used_genes: A list of gene names used for selecting genes as input.
+            use_gpu: A boolean value indicating whether to use the GPU for training.
+            output_dir: The path where the outputs will be saved.
+        """
         if 'subset' not in kwargs.keys():
             self.subset = 10000
         else:
             self.subset = kwargs['subset']
             
         if 'lengthscale_prior' not in kwargs.keys():
             self.lengthscale_prior = None
@@ -81,16 +105,16 @@
 
         if bayesian_alter:
             if self.flat_model is None:
                 likelihood = gpytorch.likelihoods.GaussianLikelihood(
                     noise_prior=noise_prior
                 )
                 self.flat_model = ExactGPModel(self.train_x, self.train_y, likelihood, lengthscale_prior=lengthscale_prior,outputscale_prior=outputscale_prior)
-            # self.init_model(self.flat_model,lengthscale=torch.tensor(99999999))
-            self.init_model(self.flat_model,lengthscale=torch.inf)
+            # self.init_model(self.flat_model,lengthscale=torch.tensor(99999))
+            self.init_model(self.flat_model,lengthscale=torch.tensor(1000))
         else:
             if self.model is None:
                 likelihood = gpytorch.likelihoods.GaussianLikelihood(
                     noise_prior=noise_prior
                 )
                 self.model = ExactGPModel(self.train_x, self.train_y, likelihood, lengthscale_prior=lengthscale_prior,outputscale_prior=outputscale_prior)
             self.init_model(self.model)
@@ -112,72 +136,57 @@
             'covar_module.outputscale': outputscale,
             'mean_module.constant': constant
         }
 
         model.initialize(**hypers)
         model.train_targets = self.train_y
         model.zero_grad()
-        # print('outputscale: %.3f   lengthscale: %.3f   noise: %.3f' % (
-        #     model.covar_module.outputscale.item(),
-        #     model.covar_module.base_kernel.lengthscale.item(),
-        #     model.likelihood.noise.item()
-        # ))
     
     def train_single_model(self,model,lr=1,training_iter=500,save=False,save_path=None,optimize_method='Adam'):
         # Find optimal model hyperparameters
         model.train()
         model.likelihood.train()
         
         # "Loss" for GPs - the marginal log likelihood
         mll = gpytorch.mlls.ExactMarginalLogLikelihood(model.likelihood, model)
-        best_loss=np.inf
-        
+        best_loss = np.inf
+        best_model_state = model.state_dict()
         if optimize_method=='Adam':
             optimizer = torch.optim.Adam(model.parameters(),lr=lr)
             for i in range(training_iter):
                 optimizer.zero_grad()
                 output = model(self.train_x)
                 loss = -mll(output, self.train_y)
                 loss.backward()
                 optimizer.step()
-                # print('Iter %d/%d - Loss: %.3f   lengthscale: %.3f   noise: %.3f' % (
-                #     i + 1, training_iter, loss.item(),
-                #     model.covar_module.base_kernel.lengthscale.item(),
-                #     model.likelihood.noise.item()
-                # ))
+                print(loss.item())
                 if loss.item() < best_loss:
                     best_model_state = model.state_dict()
                     best_loss = loss.item()
+
         # Bugs need to be solved
         elif optimize_method=='LBGFS':
             optimizer = torch.optim.LBFGS(model.parameters(),line_search_fn='strong_wolfe', lr=lr)
             def closure():
                 optimizer.zero_grad()
                 output = model(self.train_x)
                 loss = -mll(output, self.train_y)
                 loss.backward()
                 return loss
             for i in range(training_iter):
                 loss = optimizer.step(closure)
-                # print('Iter %d/%d - Loss: %.3f   lengthscale: %.3f   noise: %.3f' % (
-                #     i + 1, training_iter, loss.item(),
-                #     model.covar_module.base_kernel.lengthscale.item(),
-                #     model.likelihood.noise.item()
-                # ))
                 if loss.item() < best_loss:
                     best_model_state = model.state_dict()
                     best_loss = loss.item()
         else:
             raise ValueError('Invalid optimize method: ', optimize_method)
 
         # Get into evaluation (predictive posterior) mode
         model.eval()
         model.likelihood.eval()
-        # for param_name, param in model.named_parameters():
-        #     print(f'Parameter name: {param_name:42} value = {param.item()}')
         if save:
             torch.save(best_model_state, save_path)
         print('Best model loss:', best_loss)
         return best_loss
     
     def optim_lengthscale(self,model,lr=1,l_range=torch.arange(1,12,1),optimize_method='Adam'):
 
@@ -203,26 +212,38 @@
                     output = model(self.train_x)
                     loss = -mll(output, self.train_y)
                     loss.backward()
                     return loss
                 loss = optimizer.step(closure)
             else:
                 raise ValueError('Invalid optimize method: ', optimize_method)
-            # print(' - Lengthscale weight: %.3f   Loss: %.3f' % (
-            #     lenthscale_alpha,
-            #     loss.item(),
-            # ))
             loss_list.append(loss.item())
         best_l_alpha = l_range[np.argmin(loss_list)]
         print('Initialize lenthscale alpha as %.3f' % best_l_alpha)
         self.init_model(model,lengthscale=best_l_alpha*self.train_y.std())
         model.eval()
         model.likelihood.eval()
     
     def train(self,lr=1,training_iter=500,save_model=True,save_pred=False,cal_bf=False,optim_l=False,optimize_method='Adam'):
+        """Training GPR model
+    
+        Training GPR model. 
+        
+        Args:
+            lr: The learning rate used in the training process.
+            training_iter: The number of iterations for the training.
+            save_model: A boolean value indicating whether to save the trained model. The default value is True.
+            save_pred: A boolean value indicating whether to save the prediction results.
+            cal_bf: A boolean value indicating whether to calculate the BF (Bayes factor) value.
+            optim_l: A boolean value indicating whether to optimize the initial length scale value.
+            optimize_method: The optimization method used in the training. It must be one of 'Adam' and 'LBGFS'. By default, it is set to 'Adam'.
+
+        Returns:
+            ``None``
+        """
         for g,g_i in zip(self.used_genes,self.g_ind):
             print(f'Modeling {g}')
             self.train_y = self.subset_y[:,g_i]
             self.prepare_gpr_model(lengthscale_prior=self.lengthscale_prior,outputscale_prior=self.outputscale_prior,noise_prior=self.noise_prior) 
             if self.use_gpu:
                 self.train_y = self.train_y.cuda()
                 self.model = self.model.cuda()
@@ -298,14 +319,31 @@
         save_path=None,
         save_pred=False,
         save_pred_path=None,
         save_dpi=150,
         return_expr=True,
         *args,**kwargs
     ):
+        """Plotting predicted expression values.
+    
+        Plotting the expression values predicted by the trained GPR model.
+        
+        Args:
+            gene: The name of the gene for prediction.
+            training_iter: The number of model iteration for prediction.
+            lr: The learning rate of the model for prediction.
+            data: The coordinate matrix for prediction.
+            save: A boolean value indicating whether to save the prediction figure.
+            save_path: The path where the outputs will be saved. The file extension must be one of the supported picture types.
+            save_dpi: The DPI (dots per inch) of the saved results.
+            return_expr: A boolean value indicating whether to return the prediction values.
+
+        Returns:
+            ``None`` or the prediction values.
+        """
         if data is None:
             data = self.loc_resample
         else:
             data = torch.tensor(data,dtype=torch.float32)
             if self.use_gpu:
                 data = data.cuda()
         # if pred_path is None:
```

### Comparing `SPACEL-1.1.1/SPACEL/Scube/plot.py` & `SPACEL-1.1.2/SPACEL/Scube/plot.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/base_model.py` & `SPACEL-1.1.2/SPACEL/Splane/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/graph.py` & `SPACEL-1.1.2/SPACEL/Splane/graph.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/kegra/gnn.py` & `SPACEL-1.1.2/SPACEL/Splane/kegra/gnn.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/kegra/gnn_utils.py` & `SPACEL-1.1.2/SPACEL/Splane/kegra/gnn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/model.py` & `SPACEL-1.1.2/SPACEL/Splane/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/pygcn_utils.py` & `SPACEL-1.1.2/SPACEL/Splane/pygcn_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Splane/utils.py` & `SPACEL-1.1.2/SPACEL/Splane/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
         unique_labels = np.unique(labels)
     num_classes = len(unique_labels)
     label_map = {label: i for i, label in enumerate(unique_labels)}
     encoded = np.eye(num_classes)[np.array([label_map[label] for label in labels])]
     return encoded, unique_labels
 
 def add_cell_type_composition(ad, prop_df=None, celltype_anno=None, all_celltypes=None):
-    """Initialize Splane model.
+    """Add cell type composition.
     
-    Build the model then set the data and paratemters. 
+    Adding cell type compostion to AnnData object of spatial transcriptomic data as Splane input. 
     
     Args:
         ad: A AnnData object of spatial transcriptomic data as Splane input.
         prop_df: A DataFrame of cell type composition used for spot-based spatial transcriptomic data.
-        celltype_anno`: A list containing the cell type annotations for each cell in the single-cell resolution spatial transcriptomic data. This parameter is not used if `prof_ad` is provided.
-        all_celltypes`: A list of all cell types present in all slices. This parameter is used when a single slice does not cover all cell types in the dataset.
+        celltype_anno: A list containing the cell type annotations for each cell in the single-cell resolution spatial transcriptomic data. This parameter is not used if `prof_ad` is provided.
+        all_celltypes: A list of all cell types present in all slices. This parameter is used when a single slice does not cover all cell types in the dataset.
+
     Returns:
         ``None``
     """
     if prop_df is not None:
         if all_celltypes is not None:
             prop_df.loc[:,np.setdiff1d(all_celltypes, prop_df.columns)] = 0
         ad.obs[prop_df.columns] = prop_df.values
```

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/base_model.py` & `SPACEL-1.1.2/SPACEL/Spoint/base_model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/data_augmentation.py` & `SPACEL-1.1.2/SPACEL/Spoint/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/data_downsample.py` & `SPACEL-1.1.2/SPACEL/Spoint/data_downsample.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/data_utils.py` & `SPACEL-1.1.2/SPACEL/Spoint/data_utils.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/metrics.py` & `SPACEL-1.1.2/SPACEL/Spoint/metrics.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/model.py` & `SPACEL-1.1.2/SPACEL/Spoint/model.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/Spoint/spatial_simulation.py` & `SPACEL-1.1.2/SPACEL/Spoint/spatial_simulation.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL/setting.py` & `SPACEL-1.1.2/SPACEL/setting.py`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/SPACEL.egg-info/PKG-INFO` & `SPACEL-1.1.2/SPACEL.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: SPACEL
-Version: 1.1.1
+Version: 1.1.2
 Summary: SPACEL: characterizing spatial transcriptome architectures by deep-learning
 Home-page: https://github.com/QuKunLab/SPACEL
 Author: Hao Xu
 Author-email: xuhaoustc@mail.ustc.edu.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/spacel/badge/?version=latest)](https://spacel.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/SPACEL)
 
 # SPACEL: characterizing spatial transcriptome architectures by deep-learning
@@ -27,14 +29,21 @@
     * [Splane tutorial: Identify uniform spatial domain on human breast cancer Visium dataset](docs/tutorials/identification_of_uniform_spatial_domain.ipynb)
     * [Scube tutorial: Alignment of consecutive ST slices on human brain MERFISH dataset](docs/tutorials/alignment_of_multiple_slices.ipynb)
     * [Scube tutorial: 3D expression modeling with gaussian process regression](docs/tutorials/3D_expression_modeling.ipynb)
 
 Read the [documentation](https://spacel.readthedocs.io) for more information.
 
 ## Latest updates
+### Version 1.1.2 2023-07-12
+#### Fixed Bugs
+- Removed `rpy2` from the pypi dependency of SPACEL. It now needs to be pre-installed when creating the environment through conda.
+- Fixed a bug in Scube where the `best_model_state` was not referenced before being used.
+#### Features
+- Added function documentations for Scube related to the GPR model.
+
 ### Version 1.1.1 2023-07-11
 #### Features
 * All code based on `Tensorflow` have been mirated to `PyTorch`, it does not have `Tensorflow` as dependency anymore.
 * The `Splane.utils.add_cell_type_composition` function has been implemented to facilitate the cell type composition predicted by deconvolution methods into Splane.
 * Spoint and Splane now support tqdm type output for improved progress tracking.
     
 ## Requirements
@@ -42,15 +51,15 @@
 To install `SPACEL`, you need to install [PyTorch](https://pytorch.org) with GPU support first. If you don't need GPU acceleration, you can just skip the installation for `cudnn` and `cudatoolkit`.
 * Create conda environment for `SPACEL`:
 ```
 conda env create -f environment.yml
 ```
 or
 ```
-conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 r-base r-fitdistrplus
+conda create -n SPACEL -c conda-forge -c default cudatoolkit=10.2 python=3.8 rpy2 r-base r-fitdistrplus
 ```
 You must choose correct `PyTorch`, `cudnn` and `cudatoolkit` version dependent on your graphic driver version. 
 * Test if [PyTorch](https://pytorch.org) for GPU available:
 ```
 python
 >>> import torch
 >>> torch.cuda.is_available()
@@ -60,7 +69,9 @@
 Note: If you want to run 3D expression GPR model in Scube, you need to install the [Open3D](http://www.open3d.org/docs/release/) python library first.
 
 ## Installation
 * Install `SPACEL`:
 ```
 pip install SPACEL
 ```
+
+
```

### Comparing `SPACEL-1.1.1/SPACEL.egg-info/SOURCES.txt` & `SPACEL-1.1.2/SPACEL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPACEL-1.1.1/setup.py` & `SPACEL-1.1.2/setup.py`

 * *Files identical despite different names*

