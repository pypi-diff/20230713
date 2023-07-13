# Comparing `tmp/lc-checkpoint-0.4.0.tar.gz` & `tmp/lc-checkpoint-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.4.0.tar", last modified: Mon Jul 10 12:45:59 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.5.0.tar", last modified: Thu Jul 13 07:52:22 2023, max compression
```

## Comparing `lc-checkpoint-0.4.0.tar` & `lc-checkpoint-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.806147 lc-checkpoint-0.4.0/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.4.0/LICENSE
--rw-r--r--   0 yeoshuheng   (501) staff       (20)     6026 2023-07-10 12:45:59.806259 lc-checkpoint-0.4.0/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     5680 2023-07-10 06:32:43.000000 lc-checkpoint-0.4.0/README.md
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.4.0/pyproject.toml
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      608 2023-07-10 12:45:59.806686 lc-checkpoint-0.4.0/setup.cfg
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.803390 lc-checkpoint-0.4.0/src/
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.804933 lc-checkpoint-0.4.0/src/lc_checkpoint/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.4.0/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6051 2023-07-10 06:19:30.000000 lc-checkpoint-0.4.0/src/lc_checkpoint/main.py
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-10 12:45:59.805969 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6026 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      262 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        1 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)       14 2023-07-10 12:45:59.000000 lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/top_level.txt
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.162656 lc-checkpoint-0.5.0/
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.5.0/LICENSE
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)     6044 2023-07-13 07:52:22.162727 lc-checkpoint-0.5.0/PKG-INFO
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     5698 2023-07-13 07:48:09.000000 lc-checkpoint-0.5.0/README.md
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.5.0/pyproject.toml
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      608 2023-07-13 07:52:22.163004 lc-checkpoint-0.5.0/setup.cfg
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.160790 lc-checkpoint-0.5.0/src/
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.161676 lc-checkpoint-0.5.0/src/lc_checkpoint/
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.5.0/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6081 2023-07-13 07:47:41.000000 lc-checkpoint-0.5.0/src/lc_checkpoint/main.py
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.162515 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6044 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      262 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        1 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)       14 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.4.0/LICENSE` & `lc-checkpoint-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.4.0/PKG-INFO` & `lc-checkpoint-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,17 +96,17 @@
             new_state_dict = model.state_dict()
             new_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in prev_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             δt = new_state_weights - prev_state_weights # Get delta
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
-            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
+            compressed_data, encoder = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
-            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
+            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i, encoder)
             save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
 
             # Print statistics
             running_loss += loss.item()
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
```

### Comparing `lc-checkpoint-0.4.0/README.md` & `lc-checkpoint-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
             new_state_dict = model.state_dict()
             new_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in prev_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             δt = new_state_weights - prev_state_weights # Get delta
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
-            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
+            compressed_data, encoder = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
-            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
+            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i, encoder)
             save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
 
             # Print statistics
             running_loss += loss.item()
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
```

### Comparing `lc-checkpoint-0.4.0/setup.cfg` & `lc-checkpoint-0.5.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lc-checkpoint
-version = 0.4.0
+version = 0.5.0
 author = Dedy Van Hauten
 author_email = dedy.van@ui.ac.id
 description = A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pypi.org/project/lc-checkpoint/
 classifiers =
```

### Comparing `lc-checkpoint-0.4.0/src/lc_checkpoint/main.py` & `lc-checkpoint-0.5.0/src/lc_checkpoint/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import math
 import numpy as np
 import torch.optim as optim
 import torch.nn as nn
 import dahuffman
 import torch
 
-__all__ = ['initialize', 'compress_data', 'decode_data', 'save_checkpoint', 'load_checkpoint', 'calculate_compression_rate']
+__all__ = ['initialize', 'compress_data', 'decode_data', 'restore_model',
+           'save_checkpoint', 'load_checkpoint', 'calculate_compression_rate']
 
 net = None
 optimizer = None
 criterion = None
 checkpoint_dir = None
 num_buckets = None
 num_bits = None
@@ -94,36 +95,35 @@
         
     new_δt = np.nan_to_num(new_δt, 0)
     
     # Encode new_δt using Huffman coding
     encoder = dahuffman.HuffmanCodec.from_data(new_δt)
     encoded = encoder.encode(new_δt)
 
-    return encoded
+    return encoded, encoder
 
-def decode_data(encoded):
-    codec = dahuffman.HuffmanCodec.from_data(encoded)
-    int_list = codec.decode(encoded)
+def decode_data(encoded, encoder):
+    int_list = encoder.decode(encoded)
     int_list = [int(x) for x in int_list]
     new_δt = np.array(int_list) / 100.0
     return new_δt
 
-def save_checkpoint(filename, compressed_data, epoch, iteration):
+def save_checkpoint(filename, compressed_data, epoch, iteration, encoder):
     # Save the compressed data and epoch number to a file
     if not os.path.exists('checkpoints/lc-checkpoint'):
         os.makedirs('checkpoints/lc-checkpoint')
     filename = os.path.join('checkpoints/lc-checkpoint', 'lc_checkpoint_epoch{}_iter{}.pt'.format(epoch, iteration))
     with open(filename, 'wb') as f:
-        pickle.dump((compressed_data, epoch), f)
+        pickle.dump((compressed_data, encoder, epoch), f)
 
 def load_checkpoint(filename):
     # Load the compressed data and epoch number from a file
     with open(filename, 'rb') as f:
-        compressed_data, epoch = pickle.load(f)
-    compressed_data = decode_data(compressed_data)  # decode the binary data
+        compressed_data, encoder, epoch = pickle.load(f)
+    compressed_data = decode_data(compressed_data, encoder)  # decode the binary data
     return compressed_data, epoch
 
 def calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets):
     num_elements = len(prev_state_dict)
     compression_rate = num_elements * math.log(num_buckets, 2) + num_buckets * num_bits
     return compression_rate
```

### Comparing `lc-checkpoint-0.4.0/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.4.0
+Version: 0.5.0
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,17 +96,17 @@
             new_state_dict = model.state_dict()
             new_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in new_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             prev_state_weights = np.concatenate([tensor.numpy().flatten() for tensor in prev_state_dict.values()])  # convert each tensor to a numpy array and concatenate them
             δt = new_state_weights - prev_state_weights # Get delta
             prev_state_dict = new_state_dict
 
             # Save the checkpoint
-            compressed_data = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
+            compressed_data, encoder = lc.compress_data(δt, num_bits=num_bits, k=num_buckets)
             save_start_time = time.time()  # record the start time
-            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i)
+            lc.save_checkpoint('checkpoint.pt', compressed_data, epoch, i, encoder)
             save_time = time.time() - save_start_time  # calculate the time taken to save the checkpoint
 
             # Print statistics
             running_loss += loss.item()
             if i % 1 == 0:    # print every 1 mini-batches
                 print('[Epoch: %d, Iteration: %5d] loss: %.3f' %
                       (epoch + 1, i + 1, running_loss / 1))
```

