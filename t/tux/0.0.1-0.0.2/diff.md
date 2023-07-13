# Comparing `tmp/tux-0.0.1.tar.gz` & `tmp/tux-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tux-0.0.1.tar", last modified: Wed Jul 12 04:41:27 2023, max compression
+gzip compressed data, was "tux-0.0.2.tar", last modified: Thu Jul 13 06:53:51 2023, max compression
```

## Comparing `tux-0.0.1.tar` & `tux-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-12 04:41:27.842571 tux-0.0.1/
--rw-rw-r--   0 hao       (1001) hao       (1002)      434 2023-07-12 04:41:27.842571 tux-0.0.1/PKG-INFO
--rw-rw-r--   0 hao       (1001) hao       (1002)       38 2023-07-12 04:41:27.842571 tux-0.0.1/setup.cfg
--rw-rw-r--   0 hao       (1001) hao       (1002)      835 2023-07-12 04:40:41.000000 tux-0.0.1/setup.py
-drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-12 04:41:27.842571 tux-0.0.1/tux/
--rw-rw-r--   0 hao       (1001) hao       (1002)     1446 2023-07-12 00:59:03.000000 tux-0.0.1/tux/__init__.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     8310 2023-07-12 00:49:16.000000 tux-0.0.1/tux/checkpoint.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     3330 2023-07-12 00:49:21.000000 tux-0.0.1/tux/config.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     6662 2023-07-12 00:49:16.000000 tux-0.0.1/tux/distributed.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     4500 2023-07-12 00:49:16.000000 tux-0.0.1/tux/jax_utils.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     1643 2023-07-12 00:49:16.000000 tux-0.0.1/tux/loss.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     1257 2023-07-12 00:49:16.000000 tux-0.0.1/tux/misc.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     7677 2023-07-12 00:58:37.000000 tux-0.0.1/tux/optimizers.py
--rw-rw-r--   0 hao       (1001) hao       (1002)      415 2023-07-12 00:28:04.000000 tux-0.0.1/tux/stats.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     1262 2023-07-12 00:49:16.000000 tux-0.0.1/tux/utils.py
--rw-rw-r--   0 hao       (1001) hao       (1002)     4645 2023-07-12 00:49:16.000000 tux-0.0.1/tux/wandb.py
-drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-12 04:41:27.842571 tux-0.0.1/tux.egg-info/
--rw-rw-r--   0 hao       (1001) hao       (1002)      434 2023-07-12 04:41:27.000000 tux-0.0.1/tux.egg-info/PKG-INFO
--rw-rw-r--   0 hao       (1001) hao       (1002)      307 2023-07-12 04:41:27.000000 tux-0.0.1/tux.egg-info/SOURCES.txt
--rw-rw-r--   0 hao       (1001) hao       (1002)        1 2023-07-12 04:41:27.000000 tux-0.0.1/tux.egg-info/dependency_links.txt
--rw-rw-r--   0 hao       (1001) hao       (1002)       88 2023-07-12 04:41:27.000000 tux-0.0.1/tux.egg-info/requires.txt
--rw-rw-r--   0 hao       (1001) hao       (1002)        4 2023-07-12 04:41:27.000000 tux-0.0.1/tux.egg-info/top_level.txt
+drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-13 06:53:51.966095 tux-0.0.2/
+-rw-rw-r--   0 hao       (1001) hao       (1002)      434 2023-07-13 06:53:51.966095 tux-0.0.2/PKG-INFO
+-rw-rw-r--   0 hao       (1001) hao       (1002)       38 2023-07-13 06:53:51.966095 tux-0.0.2/setup.cfg
+-rw-rw-r--   0 hao       (1001) hao       (1002)      835 2023-07-13 06:52:50.000000 tux-0.0.2/setup.py
+drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-13 06:53:51.966095 tux-0.0.2/tux/
+-rw-rw-r--   0 hao       (1001) hao       (1002)     1460 2023-07-13 06:19:10.000000 tux-0.0.2/tux/__init__.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     8636 2023-07-13 06:11:23.000000 tux-0.0.2/tux/checkpoint.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     3330 2023-07-12 00:49:21.000000 tux-0.0.2/tux/config.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     6662 2023-07-12 00:49:16.000000 tux-0.0.2/tux/distributed.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     4500 2023-07-12 00:49:16.000000 tux-0.0.2/tux/jax_utils.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     1643 2023-07-12 00:49:16.000000 tux-0.0.2/tux/loss.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     1257 2023-07-12 00:49:16.000000 tux-0.0.2/tux/misc.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     7677 2023-07-12 00:58:37.000000 tux-0.0.2/tux/optimizers.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)      415 2023-07-12 00:28:04.000000 tux-0.0.2/tux/stats.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     1417 2023-07-13 06:01:07.000000 tux-0.0.2/tux/utils.py
+-rw-rw-r--   0 hao       (1001) hao       (1002)     4722 2023-07-13 05:55:25.000000 tux-0.0.2/tux/wandb.py
+drwxrwxr-x   0 hao       (1001) hao       (1002)        0 2023-07-13 06:53:51.966095 tux-0.0.2/tux.egg-info/
+-rw-rw-r--   0 hao       (1001) hao       (1002)      434 2023-07-13 06:53:51.000000 tux-0.0.2/tux.egg-info/PKG-INFO
+-rw-rw-r--   0 hao       (1001) hao       (1002)      307 2023-07-13 06:53:51.000000 tux-0.0.2/tux.egg-info/SOURCES.txt
+-rw-rw-r--   0 hao       (1001) hao       (1002)        1 2023-07-13 06:53:51.000000 tux-0.0.2/tux.egg-info/dependency_links.txt
+-rw-rw-r--   0 hao       (1001) hao       (1002)       88 2023-07-13 06:53:51.000000 tux-0.0.2/tux.egg-info/requires.txt
+-rw-rw-r--   0 hao       (1001) hao       (1002)        4 2023-07-13 06:53:51.000000 tux-0.0.2/tux.egg-info/top_level.txt
```

### Comparing `tux-0.0.1/setup.py` & `tux-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='tux',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     description='Tools and Utils. Some tools and utils modified from many other code to fit my needs.',
     url='https://github.com/lhao499/tux',
     packages=find_packages(include=['tux']),
     python_requires=">=3.7",
     install_requires=[
         'absl-py',
```

### Comparing `tux-0.0.1/tux/__init__.py` & `tux-0.0.2/tux/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 from .loss import cross_entropy_loss, cross_entropy_loss_and_accuracy, mse_loss
 from .misc import (float_tensor_to_dtype, float_to_dtype,
                    get_float_dtype_by_name, get_gradient_checkpoint_policy)
 from .optimizers import (AdamWOptimizerFactory, get_weight_decay_mask, optax_add_scheduled_weight_decay,
                          OptimizerFactory, OptaxScheduledWeightDecayState, PalmOptimizerFactory)
 from .stats import average_metrics, global_norm
 from .utils import (Timer, array_to_text, load_pickle, open_file, save_pickle,
-                    text_to_array)
+                    text_to_array, check_exists)
 from .wandb import WandBLogger
```

### Comparing `tux-0.0.1/tux/checkpoint.py` & `tux-0.0.2/tux/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,20 @@
         if milestone:
             # Save a milestone checkpoint that will not be overwritten
             self.save_pickle(metadata, f'metadata_{step}.pkl')
             self.save_pickle(dataset, f'dataset_{step}.pkl')
             self.save_checkpoint(
                 checkpoint_state, f'{checkpoint_name}_{step}', checkpoint_gather_fns
             )
+            # Additionally save a checkpoint that can be overwritten for automatic resuming
+            self.save_pickle(metadata, 'metadata.pkl')
+            self.save_pickle(dataset, 'dataset.pkl')
+            self.save_checkpoint(
+                checkpoint_state, f'{checkpoint_name}', checkpoint_gather_fns
+            )
         else:
             # Save a normal checkpoint that can be overwritten
             self.save_pickle(metadata, 'metadata.pkl')
             self.save_pickle(dataset, 'dataset.pkl')
             self.save_checkpoint(
                 checkpoint_state, f'{checkpoint_name}', checkpoint_gather_fns
             )
```

### Comparing `tux-0.0.1/tux/config.py` & `tux-0.0.2/tux/config.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/distributed.py` & `tux-0.0.2/tux/distributed.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/jax_utils.py` & `tux-0.0.2/tux/jax_utils.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/loss.py` & `tux-0.0.2/tux/loss.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/misc.py` & `tux-0.0.2/tux/misc.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/optimizers.py` & `tux-0.0.2/tux/optimizers.py`

 * *Files identical despite different names*

### Comparing `tux-0.0.1/tux/utils.py` & `tux-0.0.2/tux/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -51,7 +51,14 @@
     return np.frombuffer(text.encode(encoding), dtype='uint8')
 
 
 def array_to_text(array, encoding='utf-8'):
     with BytesIO(array) as fin:
         text = fin.read().decode(encoding)
     return text
+
+
+def check_exists(path):
+    if path.startswith("gs://"):
+        return gcsfs.GCSFileSystem().exists(path)
+    else:
+        return os.path.exists(path)
```

### Comparing `tux-0.0.1/tux/wandb.py` & `tux-0.0.2/tux/wandb.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
         config.output_dir = "/tmp/"
         config.wandb_dir = ""
         config.profile_dir = ""
 
         config.online = False
 
+        config.reinit = False
+        config.resume = "allow"
+
         return update_config_dict(config, updates)
 
     def __init__(self, config, variant, enable=True):
         self.enable = enable
         self.config = self.get_default_config(config)
 
         if self.config.experiment_id is None or self.config.experiment_id == "":
@@ -84,15 +87,15 @@
         self._variant = flatten_config_dict(variant)
 
         if "hostname" not in self._variant:
             self._variant["hostname"] = gethostname()
 
         if self.enable:
             self.run = wandb.init(
-                reinit=True,
+                reinit=self.config.reinit,
                 config=self._variant,
                 project=self.config.project_id,
                 dir=self.config.wandb_dir,
                 id=self.config.experiment_id,
                 resume="allow",
                 notes=self.config.experiment_note,
                 entity=self.config.project_entity,
```

