# Comparing `tmp/denoising-diffusion-pytorch-1.8.5.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.5.tar", last modified: Sun Jul  9 15:20:09 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.6.tar", last modified: Thu Jul 13 14:45:22 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.5.tar` & `denoising-diffusion-pytorch-1.8.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36837 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 15:20:09.000000 denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 15:20:09.984936 denoising-diffusion-pytorch-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-09 15:20:01.000000 denoising-diffusion-pytorch-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.217145 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36981 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.5/LICENSE` & `denoising-diffusion-pytorch-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/PKG-INFO` & `denoising-diffusion-pytorch-1.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.5
+Version: 1.8.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.5/README.md` & `denoising-diffusion-pytorch-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,16 @@
         dim_mults=(1, 2, 4, 8),
         channels = 3,
         resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16,
+        attn_dim_head = 32,
+        attn_heads = 4
     ):
         super().__init__()
 
         # classifier free guidance stuff
 
         self.cond_drop_prob = cond_drop_prob
 
@@ -330,15 +332,15 @@
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
                 Residual(PreNorm(dim_in, LinearAttention(dim_in))),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
         self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
-        self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim)))
+        self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim, dim_head = attn_dim_head, heads = attn_heads)))
         self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim, classes_emb_dim = classes_dim)
 
         for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim, classes_emb_dim = classes_dim),
```

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,14 +267,16 @@
         channels = 3,
         self_condition = False,
         resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
         learned_sinusoidal_dim = 16,
+        attn_dim_head = 32,
+        attn_heads = 4,
         full_attn = (False, False, False, True),
         flash_attn = False
     ):
         super().__init__()
 
         # determine dimensions
 
@@ -327,15 +329,15 @@
             is_last = ind >= (num_resolutions - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
             self.downs.append(nn.ModuleList([
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                attn_klass(dim_in),
+                attn_klass(dim_in, dim_head = attn_dim_head, heads = attn_heads),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
         self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
         self.mid_attn = FullAttention(mid_dim)
         self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
@@ -344,15 +346,15 @@
             is_last = ind == (len(in_out) - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
             self.ups.append(nn.ModuleList([
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                attn_klass(dim_out),
+                attn_klass(dim_out, dim_head = attn_dim_head, heads = attn_heads),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
```

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,17 @@
         dim_mults=(1, 2, 4, 8),
         channels = 3,
         self_condition = False,
         resnet_block_groups = 8,
         learned_variance = False,
         learned_sinusoidal_cond = False,
         random_fourier_features = False,
-        learned_sinusoidal_dim = 16
+        learned_sinusoidal_dim = 16,
+        attn_dim_head = 32,
+        attn_heads = 4
     ):
         super().__init__()
 
         # determine dimensions
 
         self.channels = channels
         self.self_condition = self_condition
@@ -317,15 +319,15 @@
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
                 Residual(PreNorm(dim_in, LinearAttention(dim_in))),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv1d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
         self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
-        self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim)))
+        self.mid_attn = Residual(PreNorm(mid_dim, Attention(mid_dim, dim_head = attn_dim_head, heads = attn_heads)))
         self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
 
         for ind, (dim_in, dim_out) in enumerate(reversed(in_out)):
             is_last = ind == (len(in_out) - 1)
 
             self.ups.append(nn.ModuleList([
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
```

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.5
+Version: 1.8.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.5/setup.py` & `denoising-diffusion-pytorch-1.8.6/setup.py`

 * *Files identical despite different names*

