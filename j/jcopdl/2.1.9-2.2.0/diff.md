# Comparing `tmp/jcopdl-2.1.9.tar.gz` & `tmp/jcopdl-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcopdl-2.1.9.tar", last modified: Wed Jun 28 00:47:39 2023, max compression
+gzip compressed data, was "jcopdl-2.2.0.tar", last modified: Thu Jul 13 11:17:01 2023, max compression
```

## Comparing `jcopdl-2.1.9.tar` & `jcopdl-2.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.231292 jcopdl-2.1.9/
--rw-r--r--   0 bmduser    (501) staff       (20)     1513 2022-11-02 16:57:11.000000 jcopdl-2.1.9/LICENSE
--rw-r--r--   0 bmduser    (501) staff       (20)     1208 2023-06-28 00:47:39.231489 jcopdl-2.1.9/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      427 2022-11-02 16:57:11.000000 jcopdl-2.1.9/README.md
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.214013 jcopdl-2.1.9/jcopdl/
--rw-r--r--   0 bmduser    (501) staff       (20)       76 2023-03-14 10:27:13.000000 jcopdl-2.1.9/jcopdl/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)    12446 2023-06-28 00:38:10.000000 jcopdl-2.1.9/jcopdl/callback.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1346 2023-02-18 00:58:01.000000 jcopdl-2.1.9/jcopdl/eval.py
--rw-r--r--   0 bmduser    (501) staff       (20)      217 2022-12-16 20:36:07.000000 jcopdl-2.1.9/jcopdl/exception.py
--rw-r--r--   0 bmduser    (501) staff       (20)      225 2023-02-17 20:23:36.000000 jcopdl-2.1.9/jcopdl/io.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.218237 jcopdl-2.1.9/jcopdl/layers/
--rw-r--r--   0 bmduser    (501) staff       (20)      123 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/layers/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2194 2022-12-17 03:10:42.000000 jcopdl-2.1.9/jcopdl/layers/_base.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3329 2023-03-14 08:55:49.000000 jcopdl-2.1.9/jcopdl/layers/_block.py
--rw-r--r--   0 bmduser    (501) staff       (20)      888 2023-03-14 08:55:52.000000 jcopdl-2.1.9/jcopdl/layers/_layers.py
--rw-r--r--   0 bmduser    (501) staff       (20)     4803 2023-02-21 02:58:56.000000 jcopdl-2.1.9/jcopdl/metrics.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.221045 jcopdl-2.1.9/jcopdl/optim/
--rw-r--r--   0 bmduser    (501) staff       (20)       97 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/optim/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1474 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/optim/_lookahead.py
--rw-r--r--   0 bmduser    (501) staff       (20)      604 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/optim/_optimizer.py
--rw-r--r--   0 bmduser    (501) staff       (20)     4509 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/optim/_radam.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3869 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/optim/_ralamb.py
--rw-r--r--   0 bmduser    (501) staff       (20)    32048 2023-02-18 00:57:42.000000 jcopdl-2.1.9/jcopdl/snippet.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.223024 jcopdl-2.1.9/jcopdl/transforms/
--rw-r--r--   0 bmduser    (501) staff       (20)      779 2022-12-18 15:35:38.000000 jcopdl-2.1.9/jcopdl/transforms/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      509 2022-12-18 15:43:31.000000 jcopdl-2.1.9/jcopdl/transforms/augment.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1446 2022-12-18 15:49:06.000000 jcopdl-2.1.9/jcopdl/transforms/sequence.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.226852 jcopdl-2.1.9/jcopdl/utils/
--rw-r--r--   0 bmduser    (501) staff       (20)       43 2023-02-17 18:15:13.000000 jcopdl-2.1.9/jcopdl/utils/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)      228 2023-02-17 18:15:49.000000 jcopdl-2.1.9/jcopdl/utils/conv_calculator.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.230672 jcopdl-2.1.9/jcopdl/utils/dataloader/
--rw-r--r--   0 bmduser    (501) staff       (20)      215 2022-12-18 15:56:58.000000 jcopdl-2.1.9/jcopdl/utils/dataloader/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     4525 2022-12-18 15:49:43.000000 jcopdl-2.1.9/jcopdl/utils/dataloader/char_rnn.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3019 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/utils/dataloader/coco_detection.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1936 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/utils/dataloader/multilabel.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2889 2023-02-17 18:13:42.000000 jcopdl-2.1.9/jcopdl/utils/dataloader/time_series.py
--rw-r--r--   0 bmduser    (501) staff       (20)       92 2023-01-01 04:20:04.000000 jcopdl-2.1.9/jcopdl/utils/helper.py
--rw-r--r--   0 bmduser    (501) staff       (20)      862 2022-12-16 20:39:54.000000 jcopdl-2.1.9/jcopdl/utils/nb_check.py
--rw-r--r--   0 bmduser    (501) staff       (20)      419 2022-11-02 16:57:11.000000 jcopdl-2.1.9/jcopdl/utils/random_state.py
--rw-r--r--   0 bmduser    (501) staff       (20)      997 2022-12-18 15:56:20.000000 jcopdl-2.1.9/jcopdl/utils/sampler.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2195 2023-02-17 02:45:20.000000 jcopdl-2.1.9/jcopdl/visualization.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-28 00:47:39.216120 jcopdl-2.1.9/jcopdl.egg-info/
--rw-r--r--   0 bmduser    (501) staff       (20)     1208 2023-06-28 00:47:39.000000 jcopdl-2.1.9/jcopdl.egg-info/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      993 2023-06-28 00:47:39.000000 jcopdl-2.1.9/jcopdl.egg-info/SOURCES.txt
--rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-06-28 00:47:39.000000 jcopdl-2.1.9/jcopdl.egg-info/dependency_links.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       37 2023-06-28 00:47:39.000000 jcopdl-2.1.9/jcopdl.egg-info/requires.txt
--rw-r--r--   0 bmduser    (501) staff       (20)        7 2023-06-28 00:47:39.000000 jcopdl-2.1.9/jcopdl.egg-info/top_level.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-06-28 00:47:39.232628 jcopdl-2.1.9/setup.cfg
--rw-r--r--   0 bmduser    (501) staff       (20)     1086 2022-11-02 16:57:11.000000 jcopdl-2.1.9/setup.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.802538 jcopdl-2.2.0/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1513 2022-11-02 16:57:11.000000 jcopdl-2.2.0/LICENSE
+-rw-r--r--   0 bmduser    (501) staff       (20)     1208 2023-07-13 11:17:01.802651 jcopdl-2.2.0/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      427 2022-11-02 16:57:11.000000 jcopdl-2.2.0/README.md
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.793001 jcopdl-2.2.0/jcopdl/
+-rw-r--r--   0 bmduser    (501) staff       (20)       76 2023-07-13 11:16:55.000000 jcopdl-2.2.0/jcopdl/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)    12466 2023-07-13 10:13:12.000000 jcopdl-2.2.0/jcopdl/callback.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1441 2023-07-13 09:25:22.000000 jcopdl-2.2.0/jcopdl/eval.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      217 2022-12-16 20:36:07.000000 jcopdl-2.2.0/jcopdl/exception.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      133 2023-07-13 10:14:33.000000 jcopdl-2.2.0/jcopdl/io.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.796372 jcopdl-2.2.0/jcopdl/layers/
+-rw-r--r--   0 bmduser    (501) staff       (20)      184 2023-06-28 06:32:49.000000 jcopdl-2.2.0/jcopdl/layers/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2431 2023-06-28 04:46:21.000000 jcopdl-2.2.0/jcopdl/layers/_base.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3329 2023-06-28 06:31:14.000000 jcopdl-2.2.0/jcopdl/layers/_block.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1115 2023-06-28 06:32:51.000000 jcopdl-2.2.0/jcopdl/layers/_layers.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2031 2023-06-28 06:32:32.000000 jcopdl-2.2.0/jcopdl/layers/unet.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     4803 2023-02-21 02:58:56.000000 jcopdl-2.2.0/jcopdl/metrics.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.797924 jcopdl-2.2.0/jcopdl/optim/
+-rw-r--r--   0 bmduser    (501) staff       (20)       97 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/optim/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1474 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/optim/_lookahead.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      604 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/optim/_optimizer.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     4509 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/optim/_radam.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3869 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/optim/_ralamb.py
+-rw-r--r--   0 bmduser    (501) staff       (20)    32081 2023-07-13 10:22:02.000000 jcopdl-2.2.0/jcopdl/snippet.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.798888 jcopdl-2.2.0/jcopdl/transforms/
+-rw-r--r--   0 bmduser    (501) staff       (20)      819 2023-07-13 09:39:11.000000 jcopdl-2.2.0/jcopdl/transforms/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1336 2023-07-13 09:46:21.000000 jcopdl-2.2.0/jcopdl/transforms/augment.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1446 2022-12-18 15:49:06.000000 jcopdl-2.2.0/jcopdl/transforms/sequence.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.800746 jcopdl-2.2.0/jcopdl/utils/
+-rw-r--r--   0 bmduser    (501) staff       (20)       43 2023-02-17 18:15:13.000000 jcopdl-2.2.0/jcopdl/utils/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      228 2023-02-17 18:15:49.000000 jcopdl-2.2.0/jcopdl/utils/conv_calculator.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.802296 jcopdl-2.2.0/jcopdl/utils/dataloader/
+-rw-r--r--   0 bmduser    (501) staff       (20)      215 2022-12-18 15:56:58.000000 jcopdl-2.2.0/jcopdl/utils/dataloader/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     4525 2022-12-18 15:49:43.000000 jcopdl-2.2.0/jcopdl/utils/dataloader/char_rnn.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3019 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/utils/dataloader/coco_detection.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1936 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/utils/dataloader/multilabel.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2889 2023-02-17 18:13:42.000000 jcopdl-2.2.0/jcopdl/utils/dataloader/time_series.py
+-rw-r--r--   0 bmduser    (501) staff       (20)       92 2023-01-01 04:20:04.000000 jcopdl-2.2.0/jcopdl/utils/helper.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      862 2022-12-16 20:39:54.000000 jcopdl-2.2.0/jcopdl/utils/nb_check.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      419 2022-11-02 16:57:11.000000 jcopdl-2.2.0/jcopdl/utils/random_state.py
+-rw-r--r--   0 bmduser    (501) staff       (20)      997 2022-12-18 15:56:20.000000 jcopdl-2.2.0/jcopdl/utils/sampler.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2195 2023-07-13 09:23:38.000000 jcopdl-2.2.0/jcopdl/visualization.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-07-13 11:17:01.794740 jcopdl-2.2.0/jcopdl.egg-info/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1208 2023-07-13 11:17:01.000000 jcopdl-2.2.0/jcopdl.egg-info/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)     1015 2023-07-13 11:17:01.000000 jcopdl-2.2.0/jcopdl.egg-info/SOURCES.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-07-13 11:17:01.000000 jcopdl-2.2.0/jcopdl.egg-info/dependency_links.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       37 2023-07-13 11:17:01.000000 jcopdl-2.2.0/jcopdl.egg-info/requires.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)        7 2023-07-13 11:17:01.000000 jcopdl-2.2.0/jcopdl.egg-info/top_level.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-07-13 11:17:01.803095 jcopdl-2.2.0/setup.cfg
+-rw-r--r--   0 bmduser    (501) staff       (20)     1086 2022-11-02 16:57:11.000000 jcopdl-2.2.0/setup.py
```

### Comparing `jcopdl-2.1.9/LICENSE` & `jcopdl-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/PKG-INFO` & `jcopdl-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopdl
-Version: 2.1.9
+Version: 2.2.0
 Summary: J.COp DL is a deep Learning package to complement pytorch workflow
 Home-page: https://github.com/WiraDKP/jcopdl
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: deep learning dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopdl-2.1.9/jcopdl/callback.py` & `jcopdl-2.2.0/jcopdl/callback.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,19 +27,22 @@
     - Runtime Log and Reporting
 
 
     == Arguments ==
     model: torch.nn.Module
         A deep learning architecture using PyTorch nn.Module
 
-    model_config: dict
-        A dictionary with model parameters. It would be saved in callback.
+    configs: dict
+        A dictionary with any configurations value to be saved such as model configs, optimizer configs, scheduler configs, and training configs.        
 
-    metadata: dict
-        Any other value you would want to save in callback. Usually training and dataloader parameters.
+    optimizer: torch.optim
+        An optimizer using PyTorch torch.optim
+
+    scheduler: optim.lr_scheduler
+        A scheduler using PyTorch torch.optim.lr_scheduler
 
     checkpoint_every: int
         Number of epoch to save a checkpoint. Checkpoint would be deleted after the training finished.
 
     early_stop_patience: int
         number of patience tolerance before executing early stopping
 
@@ -48,15 +51,15 @@
 
     outdir: string
         path of output directory to save the weights, configs, and logs. You may also include subpath such as `outdir/model1` or `outdir/model2`
 
 
     == Example Usage ==
     # Initialization
-    callback = Callback(model, config, outdir="model")
+    callback = Callback(model, configs, optimizer, scheduler, outdir="model")
 
     # Add single metric plot
     callback.add_plot("test_cost", scale="semilogy")
 
     # Add multi-metric in single plot
     callback.add_plot(["train_cost", "test_cost"], scale="semilogy")
 
@@ -70,25 +73,24 @@
     # Logging
     callback.log("test_cost", value)
 
     # Early Stopping
     if callback.early_stopping("test_cost"):
         break
     """
-    def __init__(self, model, optimizer, model_config=None, optimizer_config=None, metadata=None, checkpoint_every=50, early_stop_patience=5, max_epoch=None, outdir="output"):
+    def __init__(self, model, configs=None, optimizer=None, scheduler=None, checkpoint_every=50, early_stop_patience=5, max_epoch=None, outdir="output"):
         self.outdir = Path(outdir)   
         self.outdir.mkdir(parents=True, exist_ok=True)
         
-        self._check_value(model, model_config, optimizer_config, metadata, max_epoch)
+        self._check_value(model, configs, max_epoch)
         
         self.model = model
         self.optimizer = optimizer
-        self.model_config = model_config
-        self.optimizer_config = optimizer_config
-        self.metadata = metadata
+        self.scheduler = scheduler
+        self.configs = configs
         
         self.checkpoint_every = checkpoint_every
         self.early_stop_patience = early_stop_patience
         self.best_metric = None
         self.best_epoch = None
 
         self.logs = {}
@@ -102,15 +104,15 @@
         self._graph_axes = None        
         self._graph_metrics = []
         self._graph_scales = []
 
         self._image_nb = None
         self._image_metrics = []
 
-    def early_stopping(self, sense, monitor, load_best_when_stop=True, n_row=10, plot=True, plot_image=True, figsize="auto"):
+    def early_stopping(self, sense, monitor, load_best_when_stop=True, n_log=10, plot=True, plot_image=True, figsize="auto"):
         """
         sense: {"maximize", "minimize"}
             Sense of the metric's.
             - use "minimize" if lower is better
             - use "maximize" if higher is better
 
         monitor: str
@@ -122,15 +124,15 @@
         
         if monitor not in self.logs:
             raise NotLoggedError(f'Metric {monitor} is not logged. Please use callback.log("{monitor}", value).')
 
         # Show report
         self.log("epoch", self.epoch)
         if IN_NOTEBOOK:
-            report_table = HTML(pd.DataFrame(self.logs).set_index("epoch").tail(n_row).to_html())
+            report_table = HTML(pd.DataFrame(self.logs).set_index("epoch").tail(n_log).to_html())
             if self._report_nb is None:
                 self._report_nb = display(report_table, display_id=True)
             else:
                 self._report_nb.update(report_table)
         else:
             report = f'Epoch {self.epoch:5}\n'
             report += " | ".join([f'{k.title():10} = {v[-1]:.4f}' for k, v in self.logs.items() if k != "epoch"])
@@ -178,15 +180,18 @@
 
         if plot_image:
             self._plot_images()
                 
         # Cleanup and load best when stop                
         if stop and load_best_when_stop:
             self.model = torch.load(self.outdir / "model_best.pth", map_location="cpu")
-            self.optimizer = torch.load(self.outdir / "optimizer_best.pth", map_location="cpu")
+            if self.optimizer is not None:
+                self.optimizer = torch.load(self.outdir / "optimizer_best.pth", map_location="cpu")
+            if self.scheduler is not None:
+                self.scheduler = torch.load(self.outdir / "scheduler_best.pth", map_location="cpu")
                 
         self.epoch += 1
         return stop
 
     def add_plot(self, metrics, scale="linear"):
         """
         Please make sure that the registered metrics is logged.
@@ -255,29 +260,33 @@
         if name not in self.logs:
             self.logs[name] = []
         self.logs[name].append(value)
 
     def log_image(self, name, pil_image):
         if name not in self.logs:
             self.logs[name] = []
-        log_path = self.outdir / "image_logs" / name / f"{self.epoch}.png"
+        log_path = self.outdir / "image_logs" / name / f"{self.epoch:0>5}.png"
         pil_image.save(log_path)
         self.logs[name].append(log_path)
 
     def reset_nb(self):
         self._report_nb = None
         self._graph_nb = None        
         self._image_nb = None
         
     def change_early_stop_patience(self, patience):
         self.early_stop_patience = patience
 
     def _save_best(self):
         torch.save(self.model, self.outdir / f'model_best.pth')
-        torch.save(self.optimizer, self.outdir / f'optimizer_best.pth')
+        if self.optimizer is not None:
+            torch.save(self.optimizer, self.outdir / f'optimizer_best.pth')
+        if self.scheduler is not None:
+            torch.save(self.scheduler, self.outdir / f'scheduler_best.pth')
+            
         try:
             pd.DataFrame(self.logs).to_csv(self.outdir / "logs.csv", index=None)
         except:
             torch.save(self.logs, self.outdir / "logs.pth")
 
     def _save_ckpt(self):
         ckpt_path = self.outdir / "checkpoint"
@@ -292,34 +301,28 @@
         }
 
         self._report_nb = None
         self._graph_nb = None
         self._image_nb = None
         self._graph_fig = None
         self._graph_axes = None
-        torch.save(self, ckpt_path / f'epoch_{self.epoch}.pth')
+        torch.save(self, ckpt_path / f'epoch_{self.epoch:0>5}.pth')
         
         self._report_nb = metadata["report_nb"]
         self._graph_nb = metadata["graph_nb"]
         self._image_nb = metadata["image_nb"]
         self._graph_fig = metadata["graph_fig"]
         self._graph_axes = metadata["graph_axes"]
         
 
-    def _check_value(self, model, model_config, optimizer_config, metadata, max_epoch):
+    def _check_value(self, model, configs, max_epoch):
         self.max_epoch = max_epoch if max_epoch is not None else np.inf
-        
-        if (model_config is not None) and isinstance(model_config, dict):
-            torch.save(model_config, self.outdir / "model_configs.pth")
-
-        if (optimizer_config is not None) and isinstance(optimizer_config, dict):
-            torch.save(optimizer_config, self.outdir / "optimizer_configs.pth")            
             
-        if (metadata is not None) and isinstance(metadata, dict):
-            torch.save(metadata, self.outdir / "metadata.pth")            
+        if (configs is not None) and isinstance(configs, dict):
+            torch.save(configs, self.outdir / "configs.pth")
 
         if model.__module__ == "__main__":            
             raise ModelError(f'Please write model in script (ex: model.py) and import it properly.\n>> from model import {model._get_name()}')
 
     @staticmethod
     def _plot(ax, x, y, scale, label):
         if scale == "linear":
```

### Comparing `jcopdl-2.1.9/jcopdl/eval.py` & `jcopdl-2.2.0/jcopdl/eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     for feature, target in tqdm(dataloader, desc=desc.title(), leave=False):
         feature, target = feature.to(device), target.to(device)
         output = model(feature)
         metric.add_batch(output, target)
     return metric.compute()
 
 
-def evaluate_prediction(dataloader, model, device):
+def evaluate_prediction(dataloader, model, device, viz_transform=None):
     model.eval()
     feature, target = next(iter(dataloader))
     feature, target = feature.to(device), target.to(device)
     output = model(feature)
     
     preds = output.argmax(1)
     classes = dataloader.dataset.classes
+    if viz_transform is not None:
+        feature = viz_transform(feature)
     image = visualize_prediction_batch(feature, target, preds, classes)
     return image
```

### Comparing `jcopdl-2.1.9/jcopdl/layers/_base.py` & `jcopdl-2.2.0/jcopdl/layers/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,31 @@
         self._activation_map = {
             "relu": nn.ReLU(),
             "lrelu": nn.LeakyReLU(),
             "sigmoid": nn.Sigmoid(),
             "tanh": nn.Tanh(),
             "elu": nn.ELU(),
             "selu": nn.SELU(),
+            "silu": nn.SiLU(),
+            "gelu": nn.GELU(),
             "lsoftmax": nn.LogSoftmax(dim=1),
+            "softmax": nn.Softmax(dim=1),
             "identity": nn.Identity(),
-            "softmax": nn.Softmax(dim=1)
+            "none": nn.Identity()
         } 
 
     def append_activation(self, activation):
         if isinstance(activation, str):
             if activation not in self._activation_map:
-                raise Exception(f"jcopdl supports these activations ({', '.join(self._activation_map.keys())}, None)")
+                raise Exception(f"jcopdl supports these activations ({', '.join(self._activation_map.keys())})")
             self.block.add_module(activation.title(), self._activation_map[activation])
         elif activation.__module__ == "torch.nn.modules.activation":
             self.block.add_module(activation._get_name(), activation)
+        elif activation is not None:
+            raise Exception(f"jcopdl supports these activations ({', '.join(self._activation_map.keys())})")
 
     def append_dropout(self, dropout):
         self.block.add_module("do", nn.Dropout(dropout))
 
     def append_dropout2d(self, dropout):
         self.block.add_module("do", nn.Dropout2d(dropout))
```

### Comparing `jcopdl-2.1.9/jcopdl/layers/_block.py` & `jcopdl-2.2.0/jcopdl/layers/_block.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/layers/_layers.py` & `jcopdl-2.2.0/jcopdl/layers/_layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,11 +7,15 @@
 
 def conv_block(c_in, c_out, kernel=3, stride=1, pad=1, bias=True, activation='relu', batch_norm=False, dropout=0,
                pool_type='maxpool', pool_kernel=2, pool_stride=2):
     return ConvBlock(c_in, c_out, kernel, stride, pad, bias, activation, batch_norm, dropout, pool_type, pool_kernel,
                      pool_stride)
 
 
+def conv_relu_block(c_in, c_out, kernel=3, stride=1, pad=1, bias=True, activation='relu', batch_norm=False, dropout=0):
+    return ConvBlock(c_in, c_out, kernel, stride, pad, bias, activation, batch_norm, dropout, pool=None)
+
+
 def tconv_block(c_in, c_out, kernel=4, stride=2, pad=1, bias=True, activation='relu', batch_norm=False, dropout=0,
                 pool_type=None, pool_kernel=2, pool_stride=2):
     return TConvBlock(c_in, c_out, kernel, stride, pad, bias, activation, batch_norm, dropout, pool_type, pool_kernel,
                       pool_stride)
```

### Comparing `jcopdl-2.1.9/jcopdl/metrics.py` & `jcopdl-2.2.0/jcopdl/metrics.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/optim/_lookahead.py` & `jcopdl-2.2.0/jcopdl/optim/_lookahead.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/optim/_optimizer.py` & `jcopdl-2.2.0/jcopdl/optim/_optimizer.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/optim/_radam.py` & `jcopdl-2.2.0/jcopdl/optim/_radam.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/optim/_ralamb.py` & `jcopdl-2.2.0/jcopdl/optim/_ralamb.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/snippet.py` & `jcopdl-2.2.0/jcopdl/snippet.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                         "train_set = datasets.ImageFolder(\"________\", transform=train_transform)",
                         "trainloader = DataLoader(train_set, batch_size=bs, shuffle=True)",
                         "",
                         "test_set = datasets.ImageFolder(\"________\", transform=test_transform)",
                         "testloader = DataLoader(test_set, batch_size=bs, shuffle=\"____\")",
                         "",
                         "",
-                        "metadata = {",
+                        "configs = {",
                         "    \"crop_size\": crop_size",
                         "}"
                     ]
                 },
                 {
                     "name": "CharRNN Dataset",
                     "snippet": [
@@ -61,15 +61,15 @@
                         "    transforms.TruncateSequence(200)",
                         "])",
                         "",
                         "trainloader = CharRNNDataloader(train_set, batch_size=16, batch_transform=transform, drop_last=True)",
                         "testloader = CharRNNDataloader(test_set, batch_size=16, batch_transform=transform, drop_last=True)",
                         "",
                         "",
-                        "metadata = {",
+                        "configs = {",
                         "    \"chars\": train_set.chars,",
                         "    \"classes\": train_set.classes,",
                         "    \"pad\": train_set.pad",
                         "}"
                     ]
                 }
             ]
@@ -91,22 +91,22 @@
                         "            linear_block(n2, output_size, activation=\"identity\")",
                         "        ),",
                         "    ",
                         "    def forward(self, x):",
                         "        return self.fc(x)",
                         "    ",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": train_set.n_features,",
                         "    \"n1\": 128,",
                         "    \"n2\": 64,",
                         "    \"output_size\": 1,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "ANN Classification Example",
                     "snippet": [
@@ -122,22 +122,22 @@
                         "            linear_block(n2, output_size, activation=\"lsoftmax\")",
                         "        ),",
                         "    ",
                         "    def forward(self, x):",
                         "        return self.fc(x)",
                         "    ",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": train_set.n_features,",
                         "    \"n1\": 128,",
                         "    \"n2\": 64,",
                         "    \"output_size\": 1,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "CNN Classification Example",
                     "snippet": [
@@ -158,19 +158,19 @@
                         "            linear_block(\"_____\", output_size, activation=\"lsoftmax\")",
                         "        )",
                         "        ",
                         "    def forward(self, x):",
                         "        return self.fc(self.conv(x))",
                         "    ",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"output_size\": len(train_set.classes),",
                         "    \"fc_dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to Many RNN Example",
                     "snippet": [
@@ -185,22 +185,22 @@
                         "        ",
                         "    def forward(self, x, hidden):        ",
                         "        x, hidden = self.rnn(x, hidden)",
                         "        x = self.fc(x)",
                         "        return x, hidden",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to One RNN Example",
                     "snippet": [
@@ -217,22 +217,22 @@
                         "        x, hidden = self.rnn(x, hidden)",
                         "        n_layers, n_batch, n_hidden = hidden.shape",
                         "        last_state = hidden.permute(1, 0, 2).reshape(-1, n_layers*n_hidden) # LBH -> BLH -> BF",
                         "        x = self.fc(last_state)",
                         "        return x, hidden",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to Many LSTM Example",
                     "snippet": [
@@ -247,22 +247,22 @@
                         "        ",
                         "    def forward(self, x, hidden):        ",
                         "        x, hidden = self.rnn(x, hidden)",
                         "        x = self.fc(x)",
                         "        return x, hidden",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to One LSTM Example",
                     "snippet": [
@@ -280,22 +280,22 @@
                         "        state = torch.cat([h, c], dim=2)",
                         "        n_layers, n_batch, n_2hidden = state.shape",
                         "        last_state = state.permute(1, 0, 2).reshape(-1, n_layers*n_2hidden) # LBH -> BLH -> BF",
                         "        x = self.fc(last_state)",
                         "        return x, (h, c)",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to Many GRU Example",
                     "snippet": [
@@ -310,22 +310,22 @@
                         "        ",
                         "    def forward(self, x, hidden):        ",
                         "        x, hidden = self.rnn(x, hidden)",
                         "        x = self.fc(x)",
                         "        return x, hidden",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 },
                 {
                     "name": "Many to One GRU Example",
                     "snippet": [
@@ -342,35 +342,35 @@
                         "        x, hidden = self.rnn(x, hidden)",
                         "        n_layers, n_batch, n_hidden = hidden.shape",
                         "        last_state = hidden.permute(1, 0, 2).reshape(-1, n_layers*n_hidden) # LBH -> BLH -> BF",
                         "        x = self.fc(last_state)",
                         "        return x, hidden",
                         "",
                         "",
-                        "model_config = {",
+                        "configs[\"model\"] = {",
                         "    \"input_size\": ________,",
                         "    \"output_size\": ________,",
                         "    \"hidden_size\": 64,",
                         "    \"num_layers\": 2,",
                         "    \"dropout\": 0",
                         "}",
-                        "optimizer_config = {",
+                        "configs[\"optimizer\"] = {",
                         "    \"lr\": 0.001",
                         "}"
                     ]
                 }
             ]
         },
         {
             "name": "Training Preparation (MCOC)",
             "snippet": [
-                "model = _______(**model_config).to(device)",
+                "model = _______(**configs[\"model\"]).to(device)",
                 "criterion = _______",
-                "optimizer = optim.AdamW(model.parameters(), **optimizer_config)",
-                "callback = Callback(model, optimizer, model_config, optimizer_config, metadata, outdir=\"output\")"
+                "optimizer = optim.AdamW(model.parameters(), **configs[\"optimizer\"])",
+                "callback = Callback(model, configs, optimizer, outdir=\"output\")"
             ]
         },
         {
             "name": "Add Plot to Callback",
             "sub-menu": [{
                     "name": "Cost",
                     "snippet": [
@@ -599,15 +599,16 @@
         {
             "name": "Load Model",
             "sub-menu": [{
                     "name": "Continue from Checkpoint",
                     "snippet": [
                         "from jcopdl.io import load_from_checkpoint",
                         "",                       
-                        "model, optimizer, callback = load_from_checkpoint(\"output/checkpoint/_________.pth\")",
+                        "checkpoint = load_from_checkpoint(\"output/checkpoint/_________.pth\")",
+                        "model, optimizer, scheduler, callback = checkpoint.model, checkpoint.optimizer, checkpoint.scheduler, checkpoint",
                         "criterion = _______"
                     ]
                 },{
                     "name": "Load best model",
                     "snippet": [
                         "import torch",
                         "device = torch.device(\"cuda:0\" if torch.cuda.is_available() else \"cpu\")",
@@ -615,17 +616,15 @@
                         "model = torch.load(\"output/model_best.pth\", map_location=\"cpu\").to(device)"
                     ]
                 },{
                     "name": "Load config, metadata, etc",
                     "snippet": [
                         "import torch",
                         "",
-                        "model_config = torch.load(\"output/model_configs.pth\")",
-                        "optimizer_config = torch.load(\"output/optimizer_configs.pth\")",
-                        "metadata = torch.load(\"output/metadata.pth\")"
+                        "configs = torch.load(\"output/configs.pth\")"
                     ]
                 }
             ]
         }
     ]
 }
```

### Comparing `jcopdl-2.1.9/jcopdl/transforms/__init__.py` & `jcopdl-2.2.0/jcopdl/transforms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .augment import Standardize
+from .augment import Standardize, NormalizeImageNet, DenormalizeImageNet
 from .sequence import OneHotEncode, TruncateSequence, PadSequence
 
 
 class Compose:
     """
     Composes several transforms together.
```

### Comparing `jcopdl-2.1.9/jcopdl/transforms/sequence.py` & `jcopdl-2.2.0/jcopdl/transforms/sequence.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/dataloader/char_rnn.py` & `jcopdl-2.2.0/jcopdl/utils/dataloader/char_rnn.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/dataloader/coco_detection.py` & `jcopdl-2.2.0/jcopdl/utils/dataloader/coco_detection.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/dataloader/multilabel.py` & `jcopdl-2.2.0/jcopdl/utils/dataloader/multilabel.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/dataloader/time_series.py` & `jcopdl-2.2.0/jcopdl/utils/dataloader/time_series.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/nb_check.py` & `jcopdl-2.2.0/jcopdl/utils/nb_check.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/utils/sampler.py` & `jcopdl-2.2.0/jcopdl/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl/visualization.py` & `jcopdl-2.2.0/jcopdl/visualization.py`

 * *Files identical despite different names*

### Comparing `jcopdl-2.1.9/jcopdl.egg-info/PKG-INFO` & `jcopdl-2.2.0/jcopdl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcopdl
-Version: 2.1.9
+Version: 2.2.0
 Summary: J.COp DL is a deep Learning package to complement pytorch workflow
 Home-page: https://github.com/WiraDKP/jcopdl
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: deep learning dl jcop indonesia
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Developers
```

### Comparing `jcopdl-2.1.9/jcopdl.egg-info/SOURCES.txt` & `jcopdl-2.2.0/jcopdl.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 jcopdl.egg-info/dependency_links.txt
 jcopdl.egg-info/requires.txt
 jcopdl.egg-info/top_level.txt
 jcopdl/layers/__init__.py
 jcopdl/layers/_base.py
 jcopdl/layers/_block.py
 jcopdl/layers/_layers.py
+jcopdl/layers/unet.py
 jcopdl/optim/__init__.py
 jcopdl/optim/_lookahead.py
 jcopdl/optim/_optimizer.py
 jcopdl/optim/_radam.py
 jcopdl/optim/_ralamb.py
 jcopdl/transforms/__init__.py
 jcopdl/transforms/augment.py
```

### Comparing `jcopdl-2.1.9/setup.py` & `jcopdl-2.2.0/setup.py`

 * *Files identical despite different names*

