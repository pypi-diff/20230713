# Comparing `tmp/LongNet-0.3.6.tar.gz` & `tmp/LongNet-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.6.tar", last modified: Wed Jul 12 21:06:08 2023, max compression
+gzip compressed data, was "LongNet-0.3.7.tar", last modified: Wed Jul 12 21:56:59 2023, max compression
```

## Comparing `LongNet-0.3.6.tar` & `LongNet-0.3.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:05:54.000000 LongNet-0.3.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.928199 LongNet-0.3.6/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 21:05:54.000000 LongNet-0.3.6/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 21:06:08.000000 LongNet-0.3.6/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:06:08.932199 LongNet-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-12 21:05:54.000000 LongNet-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:06:08.932199 LongNet-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 21:05:54.000000 LongNet-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:06:08.932199 LongNet-0.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 21:05:54.000000 LongNet-0.3.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:56:50.000000 LongNet-0.3.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:56:59.763195 LongNet-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-12 21:56:50.000000 LongNet-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:56:59.763195 LongNet-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 21:56:50.000000 LongNet-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 21:56:50.000000 LongNet-0.3.7/test/test.py
```

### Comparing `LongNet-0.3.6/LICENSE` & `LongNet-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/attend.py` & `LongNet-0.3.7/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/attention.py` & `LongNet-0.3.7/LongNet/attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         # Initialize softmax for later use in weights
         self.softmax = nn.Softmax(dim=-1)
 
     # Function to get mask for casual attention
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
 
+
     # Forward function
     def forward(self, x):
         # Get batch size, sequence length and model dimension
         batch_size, seq_len, _ = x.shape
 
         # If using positional encoding, add it
         if self.use_xpos:
@@ -84,17 +85,32 @@
             # Calculate offset for this head
             offset = head_idx % self.dilation_rate
 
             # Apply offset and segment for this head
             x_ = x[:, offset::self.dilation_rate, :]
             x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
             
-            elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
+
+            
+            elements_attns = []
+            for idx in range(x_.shape[1]):
+                element      = x_[:, idx, :, :].to(dtype)
+                element_attn = attention(element, element, element)
+
+                elements_attns.append(element_attn)
+
             attn_output = torch.cat(elements_attns, dim=1)
 
+
+            #option2
+            # elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
+            # attn_output = torch.cat(elements_attns, dim=1)
+
+
+            
             # If using relative positional bias, add it
             if self.use_rel_pos_bias:
                 attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
             # If using casual attention, apply mask
             if self.casual:
                 mask = self.get_mask(attn_output.size(1), attn_output.size(1))
```

### Comparing `LongNet-0.3.6/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.3.7/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.3.7/LongNet/iterations/DilatedAttentionOP.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.3.7/LongNet/iterations/DilatedAttentionOld.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.3.7/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.3.7/LongNet/iterations/DynamicDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/MultiModal.py` & `LongNet-0.3.7/LongNet/iterations/MultiModal.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/iterations/topk.py` & `LongNet-0.3.7/LongNet/iterations/topk.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/training.py` & `LongNet-0.3.7/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet/utils.py` & `LongNet-0.3.7/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.7/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.6
+Version: 0.3.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.6/LongNet.egg-info/SOURCES.txt` & `LongNet-0.3.7/LongNet.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+LongNet/Transformer.py
 LongNet/__init__.py
 LongNet/attend.py
 LongNet/attention.py
 LongNet/model.py
 LongNet/training.py
 LongNet/utils.py
 LongNet.egg-info/PKG-INFO
```

### Comparing `LongNet-0.3.6/PKG-INFO` & `LongNet-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.6
+Version: 0.3.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.6/README.md` & `LongNet-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.6/setup.py` & `LongNet-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.6',
+  version = '0.3.7',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.3.6/test/test.py` & `LongNet-0.3.7/test/test.py`

 * *Files identical despite different names*

