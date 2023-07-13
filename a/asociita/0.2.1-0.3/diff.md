# Comparing `tmp/asociita-0.2.1.tar.gz` & `tmp/asociita-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.2.1.tar", max compression
+gzip compressed data, was "asociita-0.3.tar", max compression
```

## Comparing `asociita-0.2.1.tar` & `asociita-0.3.tar`

### file list

```diff
@@ -1,37 +1,76 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.2.1/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.2.1/asociita/__init__.py
--rw-r--r--   0        0        0     4435 2023-06-16 21:02:52.738641 asociita-0.2.1/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0    15339 2023-06-21 15:32:55.887413 asociita-0.2.1/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.2.1/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.2.1/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0    18039 2023-06-21 14:31:19.790585 asociita-0.2.1/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.2.1/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     8760 2023-06-21 09:00:59.361644 asociita-0.2.1/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6992 2023-06-21 09:00:53.701835 asociita-0.2.1/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    10764 2023-06-21 09:00:46.666073 asociita-0.2.1/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     4414 2023-06-16 21:28:46.480533 asociita-0.2.1/asociita/components/settings/settings.py
--rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.2.1/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.2.1/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.2.1/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.2.1/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.2.1/asociita/datasets/save_blueprint.py
--rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.2.1/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.2.1/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.2.1/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.2.1/asociita/exceptions/modelexception.py
--rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.2.1/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.2.1/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    16485 2023-06-16 11:50:05.308269 asociita-0.2.1/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.2.1/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.2.1/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6097 2023-06-21 09:19:46.159500 asociita-0.2.1/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.2.1/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.2.1/asociita/utils/handlers.py
--rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.2.1/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.2.1/asociita/utils/loggers.py
--rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.2.1/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.2.1/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.2.1/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-06-21 15:33:17.374686 asociita-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.3/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.3/asociita/__init__.py
+-rw-r--r--   0        0        0     2725 2023-07-11 10:54:45.641955 asociita-0.3/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-07-11 10:54:39.082119 asociita-0.3/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0    10487 2023-06-28 14:35:28.652094 asociita-0.3/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     6307 2023-06-16 21:39:14.145401 asociita-0.3/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    14784 2023-07-12 14:38:47.096029 asociita-0.3/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    15259 2023-06-22 18:08:42.554862 asociita-0.3/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.3/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.3/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0    18128 2023-07-04 14:39:59.993221 asociita-0.3/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     4015 2023-06-06 11:35:42.199705 asociita-0.3/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.3/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     6319 2023-07-12 15:33:59.530733 asociita-0.3/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     5593 2023-06-23 13:02:20.769158 asociita-0.3/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8984 2023-06-23 14:42:51.969346 asociita-0.3/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8902 2023-07-12 15:36:47.294347 asociita-0.3/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     7405 2023-06-23 13:02:09.173529 asociita-0.3/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11498 2023-06-23 14:42:45.977523 asociita-0.3/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     5098 2023-07-12 15:13:21.310949 asociita-0.3/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     4759 2023-07-12 14:39:39.170606 asociita-0.3/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     1663 2023-07-12 14:39:39.170606 asociita-0.3/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc
+-rw-r--r--   0        0        0    13715 2023-07-11 12:14:58.271395 asociita-0.3/asociita/components/settings/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0     6901 2023-07-12 15:13:18.167030 asociita-0.3/asociita/components/settings/evaluator_settings.py
+-rw-r--r--   0        0        0     5835 2023-07-12 14:39:37.466652 asociita-0.3/asociita/components/settings/fedopt_settings.py
+-rw-r--r--   0        0        0     1931 2023-07-12 14:39:31.446817 asociita-0.3/asociita/components/settings/init_settings.py
+-rw-r--r--   0        0        0    23141 2023-07-11 12:14:58.051401 asociita-0.3/asociita/components/settings/settings.py
+-rw-r--r--   0        0        0     2465 2023-06-07 13:17:41.861780 asociita-0.3/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1997 2023-06-07 14:35:08.514819 asociita-0.3/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-06-07 14:35:08.514819 asociita-0.3/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     2023 2023-06-07 14:35:08.314826 asociita-0.3/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc
+-rw-r--r--   0        0        0     1420 2023-06-07 14:35:08.514819 asociita-0.3/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc
+-rw-r--r--   0        0        0     4844 2023-06-12 11:32:41.024825 asociita-0.3/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc
+-rw-r--r--   0        0        0     5554 2023-06-14 13:55:29.401627 asociita-0.3/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.3/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.3/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.3/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.3/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.3/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.3/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.3/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      798 2023-06-05 13:07:28.160901 asociita-0.3/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc
+-rw-r--r--   0        0        0      442 2023-06-16 12:12:22.850903 asociita-0.3/asociita/exceptions/__pycache__/modelexception.cpython-310.pyc
+-rw-r--r--   0        0        0      990 2023-06-16 09:02:36.793602 asociita-0.3/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.3/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.3/asociita/exceptions/modelexception.py
+-rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.3/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0     1139 2023-05-29 09:36:33.144103 asociita-0.3/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc
+-rw-r--r--   0        0        0    13786 2023-06-26 13:50:33.898460 asociita-0.3/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc
+-rw-r--r--   0        0        0      557 2023-06-01 15:37:30.741582 asociita-0.3/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     4114 2023-06-14 08:05:54.914256 asociita-0.3/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.3/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    17170 2023-06-26 13:50:31.182553 asociita-0.3/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.3/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.3/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6202 2023-06-26 13:45:06.401533 asociita-0.3/asociita/utils/__pycache__/computations.cpython-310.pyc
+-rw-r--r--   0        0        0     1162 2023-05-29 09:36:33.148103 asociita-0.3/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     1575 2023-06-22 17:32:18.144898 asociita-0.3/asociita/utils/__pycache__/debugger.cpython-310.pyc
+-rw-r--r--   0        0        0     3695 2023-05-29 09:36:33.136103 asociita-0.3/asociita/utils/__pycache__/handlers.cpython-310.pyc
+-rw-r--r--   0        0        0     2009 2023-06-23 10:59:17.491655 asociita-0.3/asociita/utils/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     1309 2023-06-06 11:39:06.596624 asociita-0.3/asociita/utils/__pycache__/loggers.cpython-310.pyc
+-rw-r--r--   0        0        0     4876 2023-06-26 09:06:30.509538 asociita-0.3/asociita/utils/__pycache__/optimizers.cpython-310.pyc
+-rw-r--r--   0        0        0     4859 2023-06-05 13:07:02.649795 asociita-0.3/asociita/utils/__pycache__/orchestrations.cpython-310.pyc
+-rw-r--r--   0        0        0     1282 2023-05-29 09:36:33.148103 asociita-0.3/asociita/utils/__pycache__/showcase.cpython-310.pyc
+-rw-r--r--   0        0        0     5816 2023-06-26 13:44:42.626331 asociita-0.3/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.3/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     1388 2023-06-22 17:23:31.450734 asociita-0.3/asociita/utils/debugger.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.3/asociita/utils/handlers.py
+-rw-r--r--   0        0        0     1312 2023-06-23 10:58:27.961327 asociita-0.3/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.3/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     8064 2023-06-26 09:06:22.349796 asociita-0.3/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.3/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.3/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      676 2023-07-12 15:37:37.425037 asociita-0.3/pyproject.toml
+-rw-r--r--   0        0        0     3763 1970-01-01 00:00:00.000000 asociita-0.3/PKG-INFO
```

### Comparing `asociita-0.2.1/LICENSE` & `asociita-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/README.md` & `asociita-0.3/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/components/archiver/archive_manager.py` & `asociita-0.3/asociita/components/archiver/archive_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,16 @@
             # Paths and filenames for preserving metrics
             self.metrics_savepath = archive_manager["metrics_savepath"]
             self.orchestrator_metrics_file = archive_manager["orchestrator_filename"]
             self.clients_on_central_file = archive_manager["clients_on_central_filename"]
             self.central_on_local_file = archive_manager["central_on_local_filename"]
 
             # Paths for preserving models
-            self.orchestrator_save_path = archive_manager["orchestrator_model_save_path"]
-            self.nodes_save_path = archive_manager["nodes_model_save_path"]
+            self.orchestrator_save_path = archive_manager["orchestrator_model_savepath"]
+            self.nodes_save_path = archive_manager["nodes_model_savepath"]
 
         except ArchiverSettingsException:
             raise ArchiverSettingsException('The dictionary passed to the Archiver does not contain all the necessary key-words '/
                                             "The Dictionary should contain following key-items pairs: {orchestrator: bool," /
                                             "clients_on_central: bool, central_on_local: bool, save_results: bool, log_results: bool}")
         
         if logger != None:
```

### Comparing `asociita-0.2.1/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.3/asociita/components/evaluator/evaluation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 from asociita.exceptions.evaluatorexception import Sample_Evaluator_Init_Exception
 from asociita.utils.optimizers import Optimizers
 from collections import OrderedDict
 import copy
 import os
 import csv
 
-def write_metrics_dict(file: dict,
-                       path: str):
-    pass
-
 
 class Evaluation_Manager():
     """Evaluation Manager encapsulates the whole process of assessing the marginal
     clients' contributions, so the orchestrator code is free of any encumbrance
     connected to it. Evaluation Manager life-cycle is splitted into four different
     stages: initialization, preservation, tracking and finalization. Initialization
     requires a dictionary containing all the relevant settings. Preservation should
```

### Comparing `asociita-0.2.1/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.3/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/components/evaluator/or_evaluator.py` & `asociita-0.3/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/components/evaluator/sample_evaluator.py` & `asociita-0.3/asociita/components/evaluator/sample_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import math
 from multiprocessing import Pool, Manager
 from asociita.models.pytorch.federated_model import FederatedModel
 from collections import OrderedDict
 from _collections_abc import Generator
 from asociita.utils.optimizers import Optimizers
 
+
 def chunker(seq: iter, size: int) -> Generator:
     """Helper function for splitting an iterable into a number
     of chunks each of size n. If the iterable can not be splitted
     into an equal number of chunks of size n, chunker will return the
     left-overs as the last chunk.
         
     Parameters
@@ -24,14 +25,15 @@
     Returns
     -------
     Generator
         A generator object that can be iterated to obtain chunks of the original iterable.
     """
     return (seq[pos:pos + size] for pos in range(0, len(seq), size))
 
+
 def select_gradients(gradients: OrderedDict,
                      query: list,
                      in_place: bool = False):
     """Helper function for selecting gradients that of nodes that are
     in the query.
 
     Parameters
@@ -44,17 +46,17 @@
         No description
     Returns
     -------
     Generator
         A generator object that can be iterated to obtain chunks of the original iterable.
     """
     q_gradients = {}
-    if in_place == False:
-        gradients_copy = copy.deepcopy(gradients) #TODO: Inspect whether making copt is realy necc.
-    for id, grad in gradients_copy.items():
+    # if in_place == False:
+    #     gradients_copy = copy.deepcopy(gradients) #TODO: Inspect whether making copy is realy necc.
+    for id, grad in gradients.items():
         if id in query:
             q_gradients[id] = grad
     return q_gradients
 
 
 class Sample_Evaluator():
     """Sample evaluator is used to establish the marginal contribution of each sampled
@@ -128,15 +130,15 @@
             # Cloning the last optimizer
             marginal_optim = copy.deepcopy(optimizer)
 
             # Reconstrcuting the marginal model
             marginal_model = copy.deepcopy(previous_model)
             marginal_grad_avg = Aggregators.compute_average(marginal_gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
             marginal_weights = marginal_optim.fed_optimize(weights=marginal_model.get_weights(),
-                                                         delta=marginal_grad_avg)
+                                                           delta=marginal_grad_avg)
             marginal_model.update_weights(marginal_weights)
             marginal_model_score = marginal_model.evaluate_model()[1]
             self.partial_psi[iteration][node_id] = final_model_score - marginal_model_score
 
 
     def calculate_final_psi(self) -> tuple[dict[int: dict], dict[int: float]]:
         """Method used to sum up all the partial LOO scores to obtain
@@ -277,21 +279,21 @@
             self.partial_shapley[iteration][node] =  shap / (len(nodes_in_sample))
 
             if return_coalitions == True:
                 return recorded_values
         
 
     def update_shap_multip(self,
-                    gradients,
-                    nodes_in_sample,
-                    optimizer,
-                    iteration: int,
-                    previous_model,
-                    number_of_workers: int = 30,
-                    return_coalitions: bool = True):
+                           gradients: OrderedDict,
+                           nodes_in_sample: list,
+                           optimizer: Optimizers,
+                           iteration: int,
+                           previous_model: FederatedModel,
+                           number_of_workers: int = 30,
+                           return_coalitions: bool = True):
         """Method used to track_results after each training round.
         Update_shap_multip is a default method used to calculate
         Shapley round, as it uses a number of workers to complete a task.
     
         Given the graidnets, ids of the nodes included in sample,
         last version of the optimizer, previous version of the model
         and the updated version of the model, it calculates values of
@@ -323,27 +325,26 @@
         nodes_in_sample = [node.node_id for node in nodes_in_sample] 
         superset = Subsets.form_superset(nodes_in_sample, return_dict=False)
         # Operations counter to track the progress of the calculations.
         operation_counter = 0
         number_of_operations = 2 ** (len(nodes_in_sample)) - 1
         if len(superset) < number_of_workers:
             number_of_workers = len(superset)
+        chunked = chunker(seq = superset, size = number_of_workers)
         with Pool(number_of_workers) as pool:
-            chunked = chunker(seq = superset, size = number_of_workers)
             for chunk in chunked:
                 results = [pool.apply_async(self.establish_value, (coalition, 
-                                                                   copy.deepcopy(gradients),
-                                                                   copy.deepcopy(optimizer),
-                                                                   copy.deepcopy(previous_model))) for coalition in chunk]
+                                                                    copy.deepcopy(gradients),
+                                                                    copy.deepcopy(optimizer),
+                                                                    copy.deepcopy(previous_model))) for coalition in chunk]
                 for result in results:
                     coalition, score = result.get()
                     coalition_results[tuple(sorted(coalition))] = score
                 operation_counter += len(chunk)
                 print(f"Completed {operation_counter} out of {number_of_operations} operations")
-        
         print("Finished evaluating all of the coalitions. Commencing calculation of individual Shapley values.")
         for node in nodes_in_sample:
             shap = 0.0
             S = Subsets.select_subsets(coalitions = superset, searched_node = node)
             for s in S:
                 s_wo_i = tuple(sorted(s)) # Subset s without the agent i
                 s_copy = copy.deepcopy(s)
```

### Comparing `asociita-0.2.1/asociita/components/nodes/federated_node.py` & `asociita-0.3/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.3/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from asociita.utils.computations import Aggregators
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
 from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
 from asociita.components.archiver.archive_manager import Archive_Manager
 from asociita.components.settings.settings import Settings
+from asociita.utils.helpers import Helpers
 import datasets
 import copy
 from multiprocessing import Pool, Manager
 
 
 orchestrator_logger = Loggers.orchestrator_logger()
 from multiprocessing import set_start_method
@@ -101,60 +102,66 @@
         model_list = self.model_initialization(nodes_number=nodes_number,
                                                model=self.central_net)
         # Initializing nodes -> loading the data and models onto empty nodes.
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
                                                 data_list=nodes_data)
 
-
-        # 3. TRAINING PHASE ----- FEDOPT
-        with Manager() as manager:
-            queue = manager.Queue() # creates a shared queue
-            # create the pool of workers
-            with Pool(sample_size) as pool:
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    gradients = {}
-
-                    # Evaluation step: preserving the last version of the model and optimizer
-                    evaluation_manager.preserve_previous_model(previous_model = self.central_model)
-                    evaluation_manager.preserve_previous_optimizer(previous_optimizer = Optim)
-                    
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes, sampled_idx = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size,
-                                                 orchestrator_logger=orchestrator_logger,
-                                                 return_aux=True) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+        for iteration in range(iterations):
+            orchestrator_logger.info(f"Iteration {iteration}")
+            gradients = {}
+            # Evaluation step: preserving the last version of the model and optimizer
+            evaluation_manager.preserve_previous_model(previous_model = self.central_model)
+            evaluation_manager.preserve_previous_optimizer(previous_optimizer = Optim)
+            # Sampling nodes and asynchronously apply the function
+            sampled_nodes = sample_nodes(nodes_green, 
+                                         sample_size=sample_size, 
+                                         orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+            if self.batch_job:
+                for batch in Helpers.chunker(sampled_nodes, size=self.batch):
+                    with Pool(sample_size) as pool:
+                        results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in batch]
+                        # consume the results
+                        for result in results:
+                            node_id, model_weights = result.get()
+                            gradients[node_id] = copy.deepcopy(model_weights)
+            else:
+                with Pool(sample_size) as pool:
                     results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_gradients = result.get()
                         gradients[node_id] = copy.deepcopy(model_gradients)
-                    # Computing the average of gradients
-                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    # Upadting the weights using gradients and momentum
-                    updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
-                                                         delta=grad_avg)
-                    # Updating the central model
-                    self.central_model.update_weights(updated_weights)
-                    # Evaluation step: preserving the updated central model
-                    evaluation_manager.preserve_updated_model(updated_model = self.central_model)
-
-                    # Evaluation step: calculating all the marginal contributions
-                    evaluation_manager.track_results(gradients = gradients,
-                                                     nodes_in_sample = sampled_nodes,
-                                                     iteration = iteration)
-                    
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(updated_weights)
-                    
-                    # Passing results to the archiver -> only if so enabled in the settings.               
-                    if self.settings.enable_archiver == True:
-                        archive_manager.archive_training_results(iteration = iteration,
-                                                                central_model=self.central_model,
-                                                                nodes=nodes_green)
+            
+            # Computing the average
+            grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+            # Upadting the weights using gradients and momentum
+            updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
+                                                    delta=grad_avg)
+            # Evaluation step: preserving the updated central model
+            evaluation_manager.preserve_updated_model(updated_model = self.central_model)
+
+            # Evaluation step: calculating all the marginal contributions
+            evaluation_manager.track_results(gradients = gradients,
+                                             nodes_in_sample = sampled_nodes,
+                                             iteration = iteration)
+            
+            # Updating the orchestrator
+            self.central_model.update_weights(updated_weights)
+            # Updating the nodes
+            for node in nodes_green:
+                node.model.update_weights(updated_weights)         
+                   
+            # Passing results to the archiver -> only if so enabled in the settings.
+            if self.settings.enable_archiver == True:
+                archive_manager.archive_training_results(iteration = iteration,
+                                                        central_model=self.central_model,
+                                                        nodes=nodes_green)
+            
+            if self.full_debug == True:
+                log_gpu_memory(iteration=iteration)
+        
         
         # Evaluation step: Calling evaluation manager to preserve all steps
         results = evaluation_manager.finalize_tracking(path = archive_manager.metrics_savepath)
         orchestrator_logger.critical("Training complete")
         return 0
```

### Comparing `asociita-0.2.1/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.3/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import copy
 from asociita.components.orchestrator.generic_orchestrator import Orchestrator
 from asociita.utils.computations import Aggregators
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
 from asociita.components.archiver.archive_manager import Archive_Manager
-from multiprocessing import Pool, Manager
+from multiprocessing import Pool
 from asociita.components.settings.settings import Settings
-from torch import nn
+from asociita.utils.helpers import Helpers
+from asociita.utils.debugger import log_gpu_memory
 
 # set_start_method set to 'spawn' to ensure compatibility across platforms.
 orchestrator_logger = Loggers.orchestrator_logger()
 from multiprocessing import set_start_method
 set_start_method("spawn", force=True)
 
 
@@ -21,15 +22,16 @@
         It connects the nodes, maintain the knowledge about their state and manages the
         multithread pool. Fedopt orchestrator is a child class of the Generic Orchestrator.
         Unlike its parent, FedOpt Orchestrator performs a training using Federated Optimization
         - pseudo-gradients from the models and momentum."""
     
 
     def __init__(self, 
-                 settings: Settings) -> None:
+                 settings: Settings,
+                 **kwargs) -> None:
         """Orchestrator is initialized by passing an instance
         of the Settings object. Settings object contains all the relevant configurational
         settings that an instance of the Orchestrator object may need to complete the simulation.
         FedOpt orchestrator additionaly requires a configuration passed to the Optimizer upon
         its initialization.
         
         Parameters
@@ -39,15 +41,15 @@
             The FedOpt orchestrator additionaly requires the passed object to contain a 
             configuration for the Optimizer.
        
        Returns
        -------
        None
        """
-        super().__init__(settings)
+        super().__init__(settings, kwargs=kwargs)
     
 
     def train_protocol(self,
                 nodes_data: list[datasets.arrow_dataset.Dataset, 
                 datasets.arrow_dataset.Dataset]) -> None:
         """"Performs a full federated training according to the initialized
         settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
@@ -67,15 +69,15 @@
         -------
         int
             Returns 0 on the successful completion of the training.
         """
         # Initializing all the attributes using an instance of the Settings object.
         iterations = self.settings.iterations
         nodes_number = self.settings.number_of_nodes
-        local_warm_start = self.settings.local_warm_start
+        local_warm_start = self.settings.local_warm_start # Note: not implemented yet.
         nodes = [node for node in range(nodes_number)]
         sample_size = self.settings.sample_size
         
         # Initializing an instance of the Archiver class if enabled in the settings.
         if self.settings.enable_archiver == True:
             archive_manager = Archive_Manager(
                 archive_manager = self.settings.archiver_settings,
@@ -95,43 +97,52 @@
         
         # Initializing nodes -> loading the data and models onto empty nodes.
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
                                                 data_list=nodes_data)
 
         # 3. TRAINING PHASE ----- FEDOPT
-        with Manager() as manager:
-            queue = manager.Queue() # creates a shared queue
-            # create the pool of workers
-            with Pool(sample_size) as pool:
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    gradients = {}
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size,
-                                                 orchestrator_logger=orchestrator_logger,
-                                                 return_aux=False) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+        # create the pool of workers
+        for iteration in range(iterations):
+            orchestrator_logger.info(f"Iteration {iteration}")
+            gradients = {}
+            # Sampling nodes and asynchronously apply the function
+            sampled_nodes = sample_nodes(nodes_green, 
+                                         sample_size=sample_size, 
+                                         orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+            if self.batch_job:
+                for batch in Helpers.chunker(sampled_nodes, size=self.batch):
+                    with Pool(sample_size) as pool:
+                        results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in batch]
+                        # consume the results
+                        for result in results:
+                            node_id, model_weights = result.get()
+                            gradients[node_id] = copy.deepcopy(model_weights)
+            else:
+                with Pool(sample_size) as pool:
                     results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_gradients = result.get()
                         gradients[node_id] = copy.deepcopy(model_gradients)
-                    # Computing the average of gradients
-                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    # Upadting the weights using gradients and momentum
-                    updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
-                                                         delta=grad_avg)
-                    # Updating the orchestrator
-                    self.central_model.update_weights(updated_weights)
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(updated_weights)         
+            # Computing the average
+            grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+            # Upadting the weights using gradients and momentum
+            updated_weights = Optim.fed_optimize(weights=self.central_model.get_weights(),
+                                                    delta=grad_avg)
+            # Updating the orchestrator
+            self.central_model.update_weights(updated_weights)
+            # Updating the nodes
+            for node in nodes_green:
+                node.model.update_weights(updated_weights)         
                    
-                    # Passing results to the archiver -> only if so enabled in the settings.
-                    if self.settings.enable_archiver == True:
-                        archive_manager.archive_training_results(iteration = iteration,
-                                                                central_model=self.central_model,
-                                                                nodes=nodes_green)
+            # Passing results to the archiver -> only if so enabled in the settings.
+            if self.settings.enable_archiver == True:
+                archive_manager.archive_training_results(iteration = iteration,
+                                                        central_model=self.central_model,
+                                                        nodes=nodes_green)
+            
+            if self.full_debug == True:
+                log_gpu_memory(iteration=iteration)
 
         orchestrator_logger.critical("Training complete")
         return 0
```

### Comparing `asociita-0.2.1/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.3/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from asociita.components.nodes.federated_node import FederatedNode
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.computations import Aggregators
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import create_nodes, check_health, sample_nodes, train_nodes
 from asociita.components.archiver.archive_manager import Archive_Manager
 from asociita.components.settings.settings import Settings
-from multiprocessing import Pool, Manager
+from multiprocessing import Pool
 from torch import nn
+from asociita.utils.debugger import log_gpu_memory
+from asociita.utils.helpers import Helpers
 
 # set_start_method set to 'spawn' to ensure compatibility across platforms.
 orchestrator_logger = Loggers.orchestrator_logger()
 from multiprocessing import set_start_method
 set_start_method("spawn", force=True)
 
 
@@ -30,32 +32,36 @@
         """Orchestrator is initialized by passing an instance
         of the Settings object. Settings object contains all the relevant configurational
         settings that an instance of the Orchestrator object may need to complete the simulation.
         
         Parameters
         ----------
         settings : Settings
-            An instance of thesettings object cotaining all the settings 
+            An instance of the settings object cotaining all the settings 
             of the orchestrator.
         **kwargs : dict, optional
             Extra arguments to enable selected features of the Orchestrator.
             passing full_debug to **kwargs, allow to enter a full debug mode.
        
        Returns
        -------
        None
         """
         self.settings = settings
         self.model = None
         # Special option to enter a full debug mode.
-        if kwargs:
-            if kwargs.get("full_debug"):
-                self.full_debug = True
-            else:
-                self.full_debug = False
+        if kwargs.get("full_debug"):
+            self.full_debug = True
+        else:
+            self.full_debug = False
+        if kwargs.get("batch_job"):
+            self.batch_job = True
+            self.batch = kwargs["batch"]
+        else:
+            self.batch_job = False
     
     
     def prepare_orchestrator(self, 
                              model: nn,
                              validation_data: datasets.arrow_dataset.Dataset,
                              ) -> None:
         """Loads the orchestrator's test data and creates an instance
@@ -110,14 +116,15 @@
         ------
         NotImplemenetedError
             If local_warm_start is set to True.
         """
         if local_warm_start == True:
             raise NotImplementedError("Local warm start is not implemented yet.")
         else:
+            # Deep copy is nec. because the models will have different (non-shared) parameters
             model_list = [copy.deepcopy(model) for _ in range(nodes_number)]
         return model_list
 
 
     def nodes_initialization(self,
                              nodes_list: list[FederatedNode],
                              model_list: list[nn.Module],
@@ -176,15 +183,15 @@
         Returns:
         Int
             Returns 0 on the successful completion of the training."""
         
         # Initializing all the attributes using an instance of the Settings object.
         iterations = self.settings.iterations
         nodes_number = self.settings.number_of_nodes
-        local_warm_start = self.settings.local_warm_start
+        local_warm_start = self.settings.local_warm_start # Note: not implemeneted yet.
         nodes = [node for node in range(nodes_number)]
         sample_size = self.settings.sample_size
         
         # Initializing an instance of the Archiver class if enabled in the settings.
         if self.settings.enable_archiver == True:
             archive_manager = Archive_Manager(
                 archive_manager = self.settings.archiver_settings,
@@ -193,49 +200,57 @@
         # Creating (empty) federated nodes.
         nodes_green = create_nodes(nodes, 
                                    self.settings.nodes_settings)
 
 
         # Creating a list of models for the nodes.
         model_list = self.model_initialization(nodes_number=nodes_number,
-                                               model=self.central_net)
+                                               model=self.central_net) # return deep copies of nets.
         
         # Initializing nodes -> loading the data and models onto empty nodes.
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
                                                 model_list=model_list,
-                                                data_list=nodes_data)
-        
-        # TRAINING PHASE ----- FEDAVG
-        with Manager() as manager:
-            queue = manager.Queue() # creates a shared queue
-            # create the pool of workers
-            with Pool(sample_size) as pool: 
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    weights = {}
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size, 
-                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                                                data_list=nodes_data) # no deep copies of nets created at this stage
+    
+    # TRAINING PHASE ----- FEDAVG
+        # create the pool of workers
+        for iteration in range(iterations):
+            orchestrator_logger.info(f"Iteration {iteration}")
+            weights = {}
+            # Sampling nodes and asynchronously apply the function
+            sampled_nodes = sample_nodes(nodes_green, 
+                                            sample_size=sample_size, 
+                                            orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+            if self.batch_job:
+                for batch in Helpers.chunker(sampled_nodes, size=self.batch):
+                    with Pool(sample_size) as pool:
+                        results = [pool.apply_async(train_nodes, (node,)) for node in batch]
+                        # consume the results
+                        for result in results:
+                            node_id, model_weights = result.get()
+                            weights[node_id] = model_weights
+            else:
+                with Pool(sample_size) as pool:
                     results = [pool.apply_async(train_nodes, (node,)) for node in sampled_nodes]
                     # consume the results
                     for result in results:
                         node_id, model_weights = result.get()
-                        weights[node_id] = copy.deepcopy(model_weights)
-                    # Computing the average
-                    avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(avg)
-                    # Upadting the orchestrator
-                    self.central_model.update_weights(avg)
-
-                    # Passing results to the archiver -> only if so enabled in the settings.
-                    if self.settings.enable_archiver == True:
-                        archive_manager.archive_training_results(iteration = iteration,
-                                                                central_model=self.central_model,
-                                                                nodes=nodes_green)
-
+                        weights[node_id] = model_weights
+            # Computing the average
+            avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+            # Updating the nodes
+            for node in nodes_green:
+                node.model.update_weights(avg)
+            # Upadting the orchestrator
+            self.central_model.update_weights(avg)
+
+            # Passing results to the archiver -> only if so enabled in the settings.
+            if self.settings.enable_archiver == True:
+                archive_manager.archive_training_results(iteration = iteration,
+                                                        central_model=self.central_model,
+                                                        nodes=nodes_green)
+            if self.full_debug == True:
+                log_gpu_memory(iteration=iteration)
 
         orchestrator_logger.critical("Training complete")
         return 0
-                    
+
```

### Comparing `asociita-0.2.1/asociita/datasets/fetch_data.py` & `asociita-0.3/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/load_cifar.py` & `asociita-0.3/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/load_fmnist.py` & `asociita-0.3/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/load_mnist.py` & `asociita-0.3/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/save_blueprint.py` & `asociita-0.3/asociita/datasets/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/shard_splits.py` & `asociita-0.3/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/datasets/shard_transformation.py` & `asociita-0.3/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/models/pytorch/cifar10.py` & `asociita-0.3/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/models/pytorch/federated_model.py` & `asociita-0.3/asociita/models/pytorch/federated_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Libraries imports
-import sys, warnings, torch, gc, copy
+import torch, copy
 import numpy as np
 from datasets import arrow_dataset
 from collections import OrderedDict
 # Modules imports
 from collections import Counter
 from typing import Any, Generic, Mapping, TypeVar, Union
 #from sklearn.metrics import confusion_matrix, f1_score, precision_score, recall_score
@@ -41,31 +41,27 @@
             local_dataset (list[...]): local dataset that will be used with this set.
             node_name (int): identifier for the node that uses this container.
             features_name (int): name of key used to retrieve features, e.g. 'image'.
         -------------
         Returns:
             None
         """
-        self.device = None
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.cpu = torch.device("cpu")
         self.initial_model = None
         self.optimizer: optim.Optimizer = None
         
         # Checks for all the necessary elements:
         assert settings, "Could not find settings, please ensure that a valid dictionary containing settings was passed in a function call."
         assert net, "Could not find net object, please ensure that a valid nn.Module was passed in a function call."
         assert local_dataset, "Could not find local dataset that should be used with that model. Pleasure ensure that local dataset was passed in a function call."
         
-        self.net = copy.deepcopy(net)
+        self.net = net # No need to create a deep copy
         self.settings = settings
         self.node_name = node_name
-
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.net.to(self.device)
-        model_logger.info(f"Node {node_name} will use {self.device} as a device.")
-
         # If both, train and test data were provided
         if len(local_dataset) == 2:
             self.trainloader, self.testloader = self.prepare_data(local_dataset)
         # If only a test dataset was provided.
         elif len(local_dataset) == 1:
             self.testloader = self.prepare_data(local_dataset, only_test=True)
         else:
@@ -176,28 +172,31 @@
         Raises
         -------------
             Exception: if the model is not initialized it raises an exception
         Returns
         -------------
             _type_: weights of the network
         """
-        return copy.deepcopy(self.net.state_dict())
+        self.net.to(self.cpu) # Dupming weights on cpu.
+        return self.net.state_dict() # Try: to provide original weights, no copies.
     
 
     def get_gradients(self):
         
         assert self.initial_model != None, "Computing gradients require saving initial model first!"
+        self.net.to(self.cpu) # Dupming weights on cpu.
+        self.initial_model.to(self.cpu)
         weights_t1 = self.net.state_dict()
         weights_t2 = self.initial_model.state_dict()
         
         self.gradients = OrderedDict.fromkeys(weights_t1.keys(), 0)
         for key in weights_t1:
             self.gradients[key] =  weights_t1[key] - weights_t2[key]
-        
-        return copy.deepcopy(self.gradients)
+
+        return self.gradients # Try: to provide original weights, no copies
 
 
     def update_weights(self, avg_tensors) -> None:
         """This function updates the weights of the network.
         Raises
         ------
             Exception: _description_
@@ -254,26 +253,29 @@
             Tuple[float, float]: Loss and accuracy on the training set.
         """
 
         criterion = nn.CrossEntropyLoss()
         running_loss = 0.0
         total_correct = 0
         total = 0
-        #self.net = self.net.to(self.device)
+        
+        # Try: to place a net on the device during the training stage
+        self.net.to(self.device)
 
         self.net.train()
         for _, dic in enumerate(self.trainloader):
             data = dic['image']
             target = dic['label']
 
             self.optimizer.zero_grad()
 
             if isinstance(data, list):
                 data = data[0]
             
+            # Placing the data on the device
             data, target = data.to(self.device), target.to(self.device)
             # forward pass, backward pass and optimization
             outputs = self.net(data)
             _, predicted = torch.max(outputs.data, 1)
             correct = (predicted == target).float().sum()
 
             loss = criterion(outputs, target)
@@ -284,14 +286,15 @@
             self.optimizer.zero_grad()
             self.net.zero_grad()
             loss.backward()
             self.optimizer.step()
             self.optimizer.zero_grad()
             self.net.zero_grad()
         
+            # Emptying the cuda_cache
             if torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
 
         loss = running_loss / len(self.trainloader)
         accuracy = total_correct / total
         model_logger.info(f"Training on {self.node_name} results: loss: {loss}, accuracy: {accuracy}")
@@ -304,14 +307,17 @@
         Raises
         ------
             Exception: Raises an exception when Federated Learning is not initialized
         Returns
         -------
             Tuple[float, float]: loss and accuracy on the test set.
         """
+        # Try: to place net on device directly during the evaluation stage.
+        self.net.to(self.device)
+        
         with torch.no_grad():
             if self.net:
                 self.net.eval()
                 criterion = nn.CrossEntropyLoss()
                 test_loss = 0
                 correct = 0
                 total = 0
@@ -365,35 +371,42 @@
 
                 denominator = [sum(x) for x in zip(false_positives, true_negatives)]
                 false_positive_rate = [num/den for num, den in zip(false_positives, denominator)]
 
                 denominator = [sum(x) for x in zip(true_positives, false_negatives)]
                 true_positive_rate = [num/den for num, den in zip(true_positives, denominator)]
 
-                return (
-                    test_loss,
-                    accuracy,
-                    f1score,
-                    precision,
-                    recall,
-                    accuracy_per_class,
-                    true_positive_rate,
-                    false_positive_rate
+                # Emptying the cuda_cache
+                if torch.cuda.is_available():
+                    torch.cuda.empty_cache()
+
+        return (
+                test_loss,
+                accuracy,
+                f1score,
+                precision,
+                recall,
+                accuracy_per_class,
+                true_positive_rate,
+                false_positive_rate
                 )
 
     def quick_evaluate(self) -> tuple[float, float]:
         """Quicker version of the evaluate_model(function) 
         Validate the network on the local test set returning only the loss and accuracy.
             Raises
             ------
                 Exception: Raises an exception when Federated Learning is not initialized
             Returns
             -------
                 Tuple[float, float]: loss and accuracy on the test set.
             """
+        # Try: to place net on device directly during the evaluation stage.
+        self.net.to(self.device)
+        
         with torch.no_grad():
             if self.net:
                 self.net.eval()
                 criterion = nn.CrossEntropyLoss()
                 test_loss = 0
                 correct = 0
                 total = 0
@@ -407,19 +420,23 @@
                         total += target.size(0)
                         test_loss = criterion(output, target).item()
                         losses.append(test_loss)
                         pred = output.argmax(dim=1, keepdim=True)
                         correct += pred.eq(target.view_as(pred)).sum().item()
                     test_loss = np.mean(losses)
                     accuracy = correct / total
-
-                    return (
-                        test_loss,
-                        accuracy
-                    )
+                
+                # Emptying the cuda_cache
+                if torch.cuda.is_available():
+                    torch.cuda.empty_cache()
+
+        return (
+            test_loss,
+            accuracy
+            )
 
 
     def transform_func(self,
                        data):
         convert_tensor = transforms.ToTensor()
         data['image'] = [convert_tensor(img) for img in data['image']]
         return data
```

### Comparing `asociita-0.2.1/asociita/models/pytorch/mnist.py` & `asociita-0.3/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/utils/computations.py` & `asociita-0.3/asociita/utils/computations.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,32 @@
 import itertools
 from torch import Tensor
 
 class Aggregators:
     """Defines the Aggregators class."""
 
     @staticmethod
-    def compute_average(shared_data: dict) -> dict[Any, Any]:
+    def compute_average(gradients: dict) -> dict[Any, Any]:
         """This function computes the average of the weights.
         Args:
             shared_data (Dict): weights received from the other nodes of the cluster
         Returns
         -------
             OrderedDict: the average of the weights
         """
-        models = list(shared_data.values())
-        results: OrderedDict = OrderedDict()
-
-        for model in models:
-            for key in model:
+        results = OrderedDict()
+        for params in gradients.values():
+            for key in params:
                 if results.get(key) is None:
-                    if torch.cuda.is_available():
-                        model[key] = model[key].to("cuda:0")
-
-                    results[key] = model[key]
+                    results[key] = params[key]
                 else:
-                    if torch.cuda.is_available():
-                        model[key] = model[key].to("cuda:0")
-                    results[key] = results[key].add(model[key])
+                    results[key] += params[key]
 
         for key in results:
-            results[key] = torch.div(results[key], len(models))
+            results[key] = torch.div(results[key], len(gradients))
         return results
     
 
     @staticmethod
     def add_gradients(model_weights: OrderedDict, gradient: OrderedDict) -> OrderedDict:
         """Adds gradients to the central weights, concluding one round of Federated Training."""
         updated_weights = OrderedDict.fromkeys(model_weights.keys(), 0)
```

### Comparing `asociita-0.2.1/asociita/utils/custom_transformations.py` & `asociita-0.3/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/utils/handlers.py` & `asociita-0.3/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/utils/loggers.py` & `asociita-0.3/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/utils/optimizers.py` & `asociita-0.3/asociita/utils/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from collections import OrderedDict
-import numpy as np
 from torch import zeros
-from typing import Union
 import torch
 
 
 class Optimizers():
     def __init__(self,
                  weights: OrderedDict,
                  settings: dict) -> None:
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        # Seting up a device for the Optimizer. Please note, that the device must be the same as this
+        # that the nets were placed on. Otherwise, PyTorch will raise an exception trying to combine
+        # data placec on CPU and GPU.
+        self.device = torch.device("cpu")
         self.previous_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
         self.previous_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
         self.optimizer = settings['name']
         self.learning_rate = torch.tensor(settings['learning_rate'])
 
+        # Selecting a proper centralised optimizer and placing all the tensors on the same device.
         if self.optimizer == 'Simple':
             self.learning_rate = self.learning_rate.to(self.device)
         elif self.optimizer == "FedAdagard":
             self.b1 = torch.tensor(settings['b1'])
             self.tau = torch.tensor(settings['tau'])
             self.b1, self.tau, self.learning_rate = self.b1.to(self.device), self.tau.to(self.device), self.learning_rate.to(self.device)
         elif self.optimizer == "FedYogi" or self.optimizer == "FedAdam":
@@ -90,15 +92,15 @@
         for row_key in current_delta.keys():
             current_delta[row_key] = b1 * self.previous_delta[row_key] + (1 - b1) * delta[row_key]
         
         for row_key in current_momentum.keys():
             current_momentum[row_key] = self.previous_momentum[row_key] + (current_delta[row_key] ** 2)
 
         for row_key in updated_weights.keys():
-            updated_weights[row_key] = weights[row_key] + (learning_rate * (current_delta[row_key] / (torch.sqrt(current_momentum[row_key]) + tau)))
+            updated_weights[row_key] = (weights[row_key].to(self.device)) + (learning_rate * (current_delta[row_key] / (torch.sqrt(current_momentum[row_key]) + tau)))
         
         self.previous_delta = current_delta
         self.previous_momentum = current_momentum
 
         return updated_weights
```

### Comparing `asociita-0.2.1/asociita/utils/orchestrations.py` & `asociita-0.3/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/asociita/utils/showcase.py` & `asociita-0.3/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.2.1/pyproject.toml` & `asociita-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.2.1"
+version = "0.3"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.2.1/PKG-INFO` & `asociita-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.2.1
+Version: 0.3
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

