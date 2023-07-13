# Comparing `tmp/zuko-0.2.1.tar.gz` & `tmp/zuko-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuko-0.2.1.tar", last modified: Wed Jun 14 13:08:38 2023, max compression
+gzip compressed data, was "zuko-0.2.2.tar", last modified: Thu Jul 13 20:54:20 2023, max compression
```

## Comparing `zuko-0.2.1.tar` & `zuko-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 13:08:38.141905 zuko-0.2.1/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.2.1/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     4140 2023-06-14 13:08:38.141905 zuko-0.2.1/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     3411 2023-04-10 15:30:49.000000 zuko-0.2.1/README.md
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-04-10 15:30:49.000000 zuko-0.2.1/requirements.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-06-14 13:08:38.145905 zuko-0.2.1/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-04-12 12:10:01.000000 zuko-0.2.1/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 13:08:38.141905 zuko-0.2.1/tests/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-02-07 15:31:17.000000 zuko-0.2.1/tests/test_distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2878 2023-04-10 09:40:37.000000 zuko-0.2.1/tests/test_flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-02-07 15:17:36.000000 zuko-0.2.1/tests/test_nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3066 2023-06-14 13:02:53.000000 zuko-0.2.1/tests/test_transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2490 2023-02-06 16:24:59.000000 zuko-0.2.1/tests/test_utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 13:08:38.141905 zuko-0.2.1/zuko/
--rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-06-14 13:04:20.000000 zuko-0.2.1/zuko/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    20798 2023-04-10 15:30:49.000000 zuko-0.2.1/zuko/distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    27983 2023-06-14 12:57:20.000000 zuko-0.2.1/zuko/flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9172 2023-03-20 17:08:26.000000 zuko-0.2.1/zuko/nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    23274 2023-06-14 12:50:36.000000 zuko-0.2.1/zuko/transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    12928 2023-05-24 11:29:11.000000 zuko-0.2.1/zuko/utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 13:08:38.141905 zuko-0.2.1/zuko.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     4140 2023-06-14 13:08:38.000000 zuko-0.2.1/zuko.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      399 2023-06-14 13:08:38.000000 zuko-0.2.1/zuko.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-06-14 13:08:38.000000 zuko-0.2.1/zuko.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-06-14 13:08:38.000000 zuko-0.2.1/zuko.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-06-14 13:08:38.000000 zuko-0.2.1/zuko.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.2.2/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4779 2023-07-13 20:54:20.248591 zuko-0.2.2/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4050 2023-07-09 10:11:29.000000 zuko-0.2.2/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-09 09:28:21.000000 zuko-0.2.2/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-07-13 20:54:20.248591 zuko-0.2.2/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-07-09 09:28:21.000000 zuko-0.2.2/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.244591 zuko-0.2.2/tests/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_distributions.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2975 2023-07-13 20:10:54.000000 zuko-0.2.2/tests/test_flows.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3066 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2792 2023-07-13 11:22:12.000000 zuko-0.2.2/tests/test_utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/zuko/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-07-13 20:13:15.000000 zuko-0.2.2/zuko/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    20798 2023-07-09 09:28:21.000000 zuko-0.2.2/zuko/distributions.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    34260 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/flows.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9073 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    27008 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    13559 2023-07-13 20:00:04.000000 zuko-0.2.2/zuko/utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/zuko.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4779 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      399 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/top_level.txt
```

### Comparing `zuko-0.2.1/LICENSE` & `zuko-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zuko-0.2.1/PKG-INFO` & `zuko-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.2.1
+Version: 0.2.2
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -39,36 +39,58 @@
 
 ```
 pip install git+https://github.com/francois-rozet/zuko
 ```
 
 ## Getting started
 
-Normalizing flows are provided in the `zuko.flows` module. To build one, supply the number of sample and context features as well as the transformations' hyperparameters. Then, feeding a context `y` to the flow returns a conditional distribution `p(x | y)` which can be evaluated and sampled from.
+Normalizing flows are provided in the `zuko.flows` module. To build one, supply the number of sample and context features as well as the transformations' hyperparameters. Then, feeding a context $c$ to the flow returns a conditional distribution $p(x | c)$ which can be evaluated and sampled from.
 
 ```python
 import torch
 import zuko
 
 # Neural spline flow (NSF) with 3 sample features and 5 context features
 flow = zuko.flows.NSF(3, 5, transforms=3, hidden_features=[128] * 3)
 
 # Train to maximize the log-likelihood
 optimizer = torch.optim.AdamW(flow.parameters(), lr=1e-3)
 
-for x, y in trainset:
-    loss = -flow(y).log_prob(x)  # -log p(x | y)
+for x, c in trainset:
+    loss = -flow(c).log_prob(x)  # -log p(x | c)
     loss = loss.mean()
 
     optimizer.zero_grad()
     loss.backward()
     optimizer.step()
 
-# Sample 64 points x ~ p(x | y*)
-x = flow(y_star).sample((64,))
+# Sample 64 points x ~ p(x | c*)
+x = flow(c_star).sample((64,))
+```
+
+Alternatively, flows can be built as custom `FlowModule` objects.
+
+```python
+from zuko.flows import FlowModule, MaskedAutoregressiveTransform, Unconditional
+from zuko.distributions import DiagNormal
+from zuko.transforms import PermutationTransform
+
+flow = FlowModule(
+    transforms=[
+        MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
+        Unconditional(PermutationTransform, torch.randperm(3), buffer=True),
+        MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
+    ],
+    base=Unconditional(
+        DiagNormal,
+        torch.zeros(3),
+        torch.ones(3),
+        buffer=True,
+    ),
+)
 ```
 
 For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
```

### Comparing `zuko-0.2.1/setup.cfg` & `zuko-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `zuko-0.2.1/tests/test_distributions.py` & `zuko-0.2.2/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.1/tests/test_flows.py` & `zuko-0.2.2/tests/test_transforms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,111 @@
-r"""Tests for the zuko.flows module."""
+r"""Tests for the zuko.transforms module."""
 
 import pytest
 import torch
 
 from torch import randn
-from zuko.flows import *
+from torch.distributions import *
+from zuko.transforms import *
 
 
-def test_flows(tmp_path):
-    flows = [
-        GMM(3, 5),
-        MAF(3, 5),
-        NSF(3, 5),
-        SOSPF(3, 5),
-        NAF(3, 5),
-        UNAF(3, 5),
-        CNF(3, 5),
+def test_univariate_transforms():
+    ts = [
+        IdentityTransform(),
+        CosTransform(),
+        SinTransform(),
+        SoftclipTransform(),
+        CircularShiftTransform(),
+        MonotonicAffineTransform(randn(256), randn(256)),
+        MonotonicRQSTransform(randn(256, 8), randn(256, 8), randn(256, 7)),
+        MonotonicTransform(lambda x: x**3),
+        UnconstrainedMonotonicTransform(lambda x: torch.exp(-x**2) + 1e-2, randn(256)),
+        SOSPolynomialTransform(randn(256, 2, 4), randn(256)),
     ]
 
-    for flow in flows:
-        # Evaluation of log_prob
-        x, y = randn(256, 3), randn(5)
-        log_p = flow(y).log_prob(x)
+    for t in ts:
+        # Call
+        if hasattr(t.domain, 'lower_bound'):
+            x = torch.linspace(t.domain.lower_bound + 1e-2, t.domain.upper_bound - 1e-2, 256)
+        else:
+            x = torch.linspace(-4.999, 4.999, 256)
 
-        assert log_p.shape == (256,), flow
-        assert log_p.requires_grad, flow
+        y = t(x)
 
-        flow.zero_grad(set_to_none=True)
-        loss = -log_p.mean()
-        loss.backward()
+        assert x.shape == y.shape, t
 
-        for p in flow.parameters():
-            assert p.grad is not None, flow
+        # Inverse
+        z = t.inv(y)
 
-        # Sampling
-        x = flow(y).sample((32,))
+        assert torch.allclose(x, z, atol=1e-4), t
 
-        assert x.shape == (32, 3), flow
+        # Jacobian
+        J = torch.autograd.functional.jacobian(t, x)
 
-        # Reparameterization trick
-        if flow(y).has_rsample:
-            x = flow(y).rsample()
+        assert (torch.triu(J, diagonal=+1) == 0).all(), t
+        assert (torch.tril(J, diagonal=-1) == 0).all(), t
 
-            flow.zero_grad(set_to_none=True)
-            loss = x.square().sum().sqrt()
-            loss.backward()
+        ladj = torch.diag(J).abs().log()
 
-            for p in flow.parameters():
-                assert p.grad is not None, flow
+        assert torch.allclose(t.log_abs_det_jacobian(x, y), ladj, atol=1e-4), t
 
-        # Invertibility
-        if isinstance(flow, FlowModule):
-            x, y = randn(256, 3), randn(256, 5)
-            t = flow(y).transform
-            z = t.inv(t(x))
+        # Compound call
+        y_comp, ladj_comp = t.call_and_ladj(x)
 
-            assert torch.allclose(x, z, atol=1e-4), flow
+        assert torch.allclose(y_comp, y, atol=1e-4), t
+        assert torch.allclose(ladj_comp, ladj, atol=1e-4), t
 
-        # Saving
-        torch.save(flow, tmp_path / 'flow.pth')
+        # Inverse Jacobian
+        J = torch.autograd.functional.jacobian(t.inv, y)
 
-        # Loading
-        flow_bis = torch.load(tmp_path / 'flow.pth')
+        assert (torch.triu(J, diagonal=+1) == 0).all(), t
+        assert (torch.tril(J, diagonal=-1) == 0).all(), t
 
-        x, y = randn(3), randn(5)
+        ladj = torch.diag(J).abs().log()
 
-        seed = torch.seed()
-        log_p = flow(y).log_prob(x)
-        torch.manual_seed(seed)
-        log_p_bis = flow_bis(y).log_prob(x)
+        assert torch.allclose(t.inv.log_abs_det_jacobian(y, z), ladj, atol=1e-4), t
 
-        assert torch.allclose(log_p, log_p_bis), flow
 
+def test_multivariate_transforms():
+    A, B = torch.randn(5, 16), torch.randn(16, 5)
+    f = lambda t, x: torch.sigmoid(x @ A) @ B
 
-def test_autoregressive_transforms():
-    ATs = [
-        MaskedAutoregressiveTransform,
-        NeuralAutoregressiveTransform,
-        UnconstrainedNeuralAutoregressiveTransform,
+    ts = [
+        FreeFormJacobianTransform(f, 0.0, 1.0),
+        LULinearTransform(randn(5, 5)),
+        PermutationTransform(torch.randperm(5)),
     ]
 
-    for AT in ATs:
-        # Without context
-        t = AT(3)
-        x = randn(3)
-        z = t()(x)
-
-        assert z.shape == x.shape, t
-        assert z.requires_grad, t
-        assert torch.allclose(t().inv(z), x, atol=1e-4), t
-
-        # With context
-        t = AT(3, 5)
-        x, y = randn(256, 3), randn(5)
-        z = t(y)(x)
-
-        assert z.shape == x.shape, t
-        assert z.requires_grad, t
-        assert torch.allclose(t(y).inv(z), x, atol=1e-4), t
-
-        # Passes
-
-        ## Fully autoregressive
-        t = AT(7)
-        x = randn(7)
-        J = torch.autograd.functional.jacobian(t(), x)
-
-        assert (torch.triu(J, diagonal=1) == 0).all(), t
-
-        ## Coupling
-        t = AT(7, passes=2)
-        x = randn(7)
-        J = torch.autograd.functional.jacobian(t(), x)
-
-        assert (torch.triu(J, diagonal=1) == 0).all(), t
-        assert (torch.tril(J[:4, :4], diagonal=-1) == 0).all(), t
-        assert (torch.tril(J[4:, 4:], diagonal=-1) == 0).all(), t
+    for t in ts:
+        # Shapes
+        x = randn(256, 5)
+        y = t(x)
+
+        assert x.shape == y.shape, t
+
+        # Inverse
+        z = t.inv(y)
+
+        assert torch.allclose(x, z, atol=1e-4), t
+
+        # Jacobian
+        x = randn(5)
+        y = t(x)
+
+        J = torch.autograd.functional.jacobian(t, x)
+        ladj = torch.linalg.slogdet(J).logabsdet
+
+        assert torch.allclose(t.log_abs_det_jacobian(x, y), ladj, atol=1e-4), t
+
+        # Compound call
+        y_comp, ladj_comp = t.call_and_ladj(x)
+
+        assert torch.allclose(y_comp, y, atol=1e-4), t
+        assert torch.allclose(ladj_comp, ladj, atol=1e-4), t
+
+        # Inverse Jacobian
+        z = t.inv(y)
+
+        J = torch.autograd.functional.jacobian(t.inv, y)
+        ladj = torch.linalg.slogdet(J).logabsdet
+
+        assert torch.allclose(t.inv.log_abs_det_jacobian(y, z), ladj, atol=1e-4), t
```

### Comparing `zuko-0.2.1/tests/test_nn.py` & `zuko-0.2.2/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.1/tests/test_utils.py` & `zuko-0.2.2/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,7 +90,23 @@
     # Gradients
     grad_x0, grad_t, grad_alpha = torch.autograd.grad(xt.sum(), (x0, t, alpha))
     g_x0, g_t, g_alpha = torch.autograd.grad(F(t, x0).sum(), (x0, t, alpha))
 
     assert torch.allclose(grad_x0, g_x0, atol=1e-4)
     assert torch.allclose(grad_t, g_t, atol=1e-4)
     assert torch.allclose(grad_alpha, g_alpha, atol=1e-4)
+
+
+def test_unpack():
+    # Normal
+    x = randn(26)
+    y, z = unpack(x, ((1, 2, 3), (4, 5)))
+
+    assert y.shape == (1, 2, 3)
+    assert z.shape == (4, 5)
+
+    # Batched
+    x = randn(7, 26)
+    y, z = unpack(x, ((1, 2, 3), (4, 5)))
+
+    assert y.shape == (7, 1, 2, 3)
+    assert z.shape == (7, 4, 5)
```

### Comparing `zuko-0.2.1/zuko/distributions.py` & `zuko-0.2.2/zuko/distributions.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.1/zuko/flows.py` & `zuko-0.2.2/zuko/flows.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,74 @@
-r"""Parameterized flows and autoregressive transformations."""
+r"""Parameterized flows and transformations."""
 
 __all__ = [
     'DistributionModule',
     'TransformModule',
     'FlowModule',
     'GMM',
+    'ElementWiseTransform',
     'MaskedAutoregressiveTransform',
     'MAF',
     'NSF',
     'NCSF',
     'SOSPF',
     'NeuralAutoregressiveTransform',
     'NAF',
     'UnconstrainedNeuralAutoregressiveTransform',
     'UNAF',
+    'GeneralCouplingTransform',
+    'GCF',
     'FFJTransform',
     'CNF',
 ]
 
 import abc
 import torch
 import torch.nn as nn
 
 from functools import partial
-from math import ceil, pi
+from math import ceil, pi, prod
 from textwrap import indent
-from torch import Tensor, LongTensor, Size
+from torch import Tensor, BoolTensor, LongTensor, Size
 from torch.distributions import *
 from typing import *
 
 from .distributions import *
 from .transforms import *
 from .nn import *
-from .utils import broadcast
+from .utils import broadcast, unpack
 
 
 class DistributionModule(nn.Module, abc.ABC):
     r"""Abstract distribution module."""
 
     @abc.abstractmethod
-    def forward(y: Tensor = None) -> Distribution:
+    def forward(c: Tensor = None) -> Distribution:
         r"""
         Arguments:
-            y: A context :math:`y`.
+            c: A context :math:`c`.
 
         Returns:
-            A distribution :math:`p(X | y)`.
+            A distribution :math:`p(X | c)`.
         """
 
         pass
 
 
 class TransformModule(nn.Module, abc.ABC):
     r"""Abstract transformation module."""
 
     @abc.abstractmethod
-    def forward(y: Tensor = None) -> Transform:
+    def forward(c: Tensor = None) -> Transform:
         r"""
         Arguments:
-            y: A context :math:`y`.
+            c: A context :math:`c`.
 
         Returns:
-            A transformation :math:`z = f(x | y)`.
+            A transformation :math:`y = f(x | c)`.
         """
 
         pass
 
 
 class FlowModule(DistributionModule):
     r"""Creates a normalizing flow module.
@@ -81,29 +84,29 @@
         base: DistributionModule,
     ):
         super().__init__()
 
         self.transforms = nn.ModuleList(transforms)
         self.base = base
 
-    def forward(self, y: Tensor = None) -> NormalizingFlow:
+    def forward(self, c: Tensor = None) -> NormalizingFlow:
         r"""
         Arguments:
-            y: A context :math:`y`.
+            c: A context :math:`c`.
 
         Returns:
-            A normalizing flow :math:`p(X | y)`.
+            A normalizing flow :math:`p(X | c)`.
         """
 
-        transform = ComposedTransform(*(t(y) for t in self.transforms))
+        transform = ComposedTransform(*(t(c) for t in self.transforms))
 
-        if y is None:
-            base = self.base(y)
+        if c is None:
+            base = self.base(c)
         else:
-            base = self.base(y).expand(y.shape[:-1])
+            base = self.base(c).expand(c.shape[:-1])
 
         return NormalizingFlow(transform, base)
 
 
 class Unconditional(nn.Module):
     r"""Creates a module that registers the positional arguments of a function.
     The function is evaluated during the forward pass and the result is returned.
@@ -133,44 +136,44 @@
                 self.register_parameter(f'_{i}', nn.Parameter(arg))
 
         self.kwargs = kwargs
 
     def __repr__(self) -> str:
         return repr(self.forward())
 
-    def forward(self, y: Tensor = None) -> Any:
+    def forward(self, c: Tensor = None) -> Any:
         return self.meta(
             *self._parameters.values(),
             *self._buffers.values(),
             **self.kwargs,
         )
 
 
 class Parameters(nn.ParameterList):
     r"""Creates a list of parameters."""
 
     def extra_repr(self) -> str:
         lines = [
-            f'({i}): tensor of shape {tuple(p.shape)}'
+            f'({i}): Tensor(shape={tuple(p.shape)})'
             for i, p in enumerate(self)
         ]
 
         return indent('\n'.join(lines), '  ')
 
 
 class GMM(DistributionModule):
     r"""Creates a Gaussian mixture model (GMM).
 
-    .. math:: p(X | y) = \sum_{i = 1}^K w_i(y) \, \mathcal{N}(X | \mu_i(y), \Sigma_i(y))
+    .. math:: p(X | c) = \sum_{i = 1}^K w_i(c) \, \mathcal{N}(X | \mu_i(c), \Sigma_i(c))
 
     Arguments:
         features: The number of features.
         context: The number of context features.
         components: The number of components :math:`K` in the mixture.
-        **kwargs: Keyword arguments passed to :class:`zuko.nn.MLP`.
+        kwargs: Keyword arguments passed to :class:`zuko.nn.MLP`.
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
         components: int = 2,
@@ -181,39 +184,107 @@
         shapes = [
             (components,),  # probabilities
             (components, features),  # mean
             (components, features),  # diagonal
             (components, features * (features - 1) // 2),  # off diagonal
         ]
 
-        self.shapes = list(map(Size, shapes))
-        self.sizes = [s.numel() for s in self.shapes]
+        self.shapes = shapes
+        self.total = sum(prod(s) for s in shapes)
 
         if context > 0:
-            self.hyper = MLP(context, sum(self.sizes), **kwargs)
+            self.hyper = MLP(context, self.total, **kwargs)
         else:
             self.phi = Parameters(torch.randn(*s) for s in shapes)
 
-    def forward(self, y: Tensor = None) -> Distribution:
-        if y is None:
+    def forward(self, c: Tensor = None) -> Distribution:
+        if c is None:
             phi = self.phi
         else:
-            phi = self.hyper(y)
-            phi = phi.split(self.sizes, -1)
-            phi = (p.unflatten(-1, s) for p, s in zip(phi, self.shapes))
+            phi = self.hyper(c)
+            phi = unpack(phi, self.shapes)
 
         logits, loc, diag, tril = phi
 
         scale = torch.diag_embed(diag.exp() + 1e-5)
         mask = torch.tril(torch.ones_like(scale, dtype=bool), diagonal=-1)
         scale = torch.masked_scatter(scale, mask, tril)
 
         return Mixture(MultivariateNormal(loc=loc, scale_tril=scale), logits)
 
 
+class ElementWiseTransform(TransformModule):
+    r"""Creates an element-wise transformation.
+
+    Arguments:
+        features: The number of features.
+        context: The number of context features.
+        univariate: The univariate transformation constructor.
+        shapes: The shapes of the univariate transformation parameters.
+        kwargs: Keyword arguments passed to :class:`zuko.nn.MLP`.
+
+    Example:
+        >>> t = ElementWiseTransform(3, 4)
+        >>> t
+        ElementWiseTransform(
+          (base): MonotonicAffineTransform()
+          (hyper): MLP(
+            (0): Linear(in_features=4, out_features=64, bias=True)
+            (1): ReLU()
+            (2): Linear(in_features=64, out_features=64, bias=True)
+            (3): ReLU()
+            (4): Linear(in_features=64, out_features=6, bias=True)
+          )
+        )
+        >>> x = torch.randn(3)
+        >>> x
+        tensor([2.1983,  -1.3182,  0.0329])
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
+        tensor([2.1983,  -1.3182,  0.0329])
+    """
+
+    def __init__(
+        self,
+        features: int,
+        context: int = 0,
+        univariate: Callable[..., Transform] = MonotonicAffineTransform,
+        shapes: Sequence[Size] = ((), ()),
+        **kwargs,
+    ):
+        super().__init__()
+
+        self.univariate = univariate
+        self.shapes = shapes
+        self.total = sum(prod(s) for s in shapes)
+
+        if context > 0:
+            self.hyper = MLP(context, features * self.total, **kwargs)
+        else:
+            self.phi = Parameters(torch.randn(features, *s) for s in shapes)
+
+    def extra_repr(self) -> str:
+        base = self.univariate(*map(torch.randn, self.shapes))
+
+        return '\n'.join([
+            f'(base): {base}',
+        ])
+
+    def forward(self, c: Tensor = None) -> Transform:
+        if c is None:
+            phi = self.phi
+        else:
+            phi = self.hyper(c)
+            phi = phi.unflatten(-1, (-1, self.total))
+            phi = unpack(phi, self.shapes)
+
+        return DependentTransform(self.univariate(*phi), 1)
+
+
 class MaskedAutoregressiveTransform(TransformModule):
     r"""Creates a masked autoregressive transformation.
 
     References:
         | Masked Autoregressive Flow for Density Estimation (Papamakarios et al., 2017)
         | https://arxiv.org/abs/1705.07057
 
@@ -241,17 +312,17 @@
             (3): ReLU()
             (4): MaskedLinear(in_features=64, out_features=6, bias=True)
           )
         )
         >>> x = torch.randn(3)
         >>> x
         tensor([-0.9485,  1.5290,  0.2018])
-        >>> y = torch.randn(4)
-        >>> z = t(y)(x)
-        >>> t(y).inv(z)
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
         tensor([-0.9485,  1.5290,  0.2018])
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
@@ -261,16 +332,16 @@
         shapes: Sequence[Size] = ((), ()),
         **kwargs,
     ):
         super().__init__()
 
         # Univariate transformation
         self.univariate = univariate
-        self.shapes = list(map(Size, shapes))
-        self.sizes = [s.numel() for s in self.shapes]
+        self.shapes = shapes
+        self.total = sum(prod(s) for s in shapes)
 
         # Adjacency
         self.register_buffer('order', None)
 
         if passes is None:
             passes = features
 
@@ -279,48 +350,45 @@
         else:
             order = torch.as_tensor(order)
 
         self.passes = min(max(passes, 1), features)
         self.order = torch.div(order, ceil(features / self.passes), rounding_mode='floor')
 
         in_order = torch.cat((self.order, torch.full((context,), -1)))
-        out_order = torch.repeat_interleave(self.order, sum(self.sizes))
+        out_order = torch.repeat_interleave(self.order, self.total)
         adjacency = out_order[:, None] > in_order
 
         # Hyper network
         self.hyper = MaskedMLP(adjacency, **kwargs)
 
     def extra_repr(self) -> str:
         base = self.univariate(*map(torch.randn, self.shapes))
         order = self.order.tolist()
 
         if len(order) > 10:
-            order = str(order[:5] + [...] + order[-5:]).replace('Ellipsis', '...')
+            order = order[:5] + [...] + order[-5:]
+            order = str(order).replace('Ellipsis', '...')
 
         return '\n'.join([
             f'(base): {base}',
             f'(order): {order}',
         ])
 
-    def meta(self, y: Tensor, x: Tensor) -> Transform:
-        if y is not None:
-            x = torch.cat(broadcast(x, y, ignore=1), dim=-1)
-
-        total = sum(self.sizes)
+    def meta(self, c: Tensor, x: Tensor) -> Transform:
+        if c is not None:
+            x = torch.cat(broadcast(x, c, ignore=1), dim=-1)
 
         phi = self.hyper(x)
-        phi = phi.unflatten(-1, (phi.shape[-1] // total, total))
-        phi = phi.split(self.sizes, -1)
-        phi = (p.unflatten(-1, s + (1,)) for p, s in zip(phi, self.shapes))
-        phi = (p.squeeze(-1) for p in phi)
+        phi = phi.unflatten(-1, (-1, self.total))
+        phi = unpack(phi, self.shapes)
 
-        return self.univariate(*phi)
+        return DependentTransform(self.univariate(*phi), 1)
 
-    def forward(self, y: Tensor = None) -> Transform:
-        return AutoregressiveTransform(partial(self.meta, y), self.passes)
+    def forward(self, c: Tensor = None) -> Transform:
+        return AutoregressiveTransform(partial(self.meta, c), self.passes)
 
 
 class MAF(FlowModule):
     r"""Creates a masked autoregressive flow (MAF).
 
     References:
         | Masked Autoregressive Flow for Density Estimation (Papamakarios et al., 2017)
@@ -372,19 +440,19 @@
                 (3): ReLU()
                 (4): MaskedLinear(in_features=64, out_features=6, bias=True)
               )
             )
           )
           (base): DiagNormal(loc: torch.Size([3]), scale: torch.Size([3]))
         )
-        >>> y = torch.randn(4)
-        >>> x = flow(y).sample()
+        >>> c = torch.randn(4)
+        >>> x = flow(c).sample()
         >>> x
         tensor([-1.7154, -0.4401,  0.7505])
-        >>> flow(y).log_prob(x)
+        >>> flow(c).log_prob(x)
         tensor(-4.4630, grad_fn=<AddBackward0>)
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
@@ -522,15 +590,15 @@
             context=context,
             univariate=SOSPolynomialTransform,
             shapes=[(polynomials, degree + 1), ()],
             **kwargs,
         )
 
         for i in reversed(range(len(self.transforms))):
-            self.transforms.insert(i, Unconditional(SoftclipTransform))
+            self.transforms.insert(i, Unconditional(SoftclipTransform, bound=6.0))
 
 
 class NeuralAutoregressiveTransform(MaskedAutoregressiveTransform):
     r"""Creates a neural autoregressive transformation.
 
     The monotonic neural network is parametrized by its internal positive weights,
     which are independent of the features and context. To modulate its behavior, it
@@ -568,17 +636,17 @@
             (3): TwoWayELU(alpha=1.0)
             (4): MonotonicLinear(in_features=64, out_features=1, bias=True)
           )
         )
         >>> x = torch.randn(3)
         >>> x
         tensor([-2.3267,  1.4581, -1.6776])
-        >>> y = torch.randn(4)
-        >>> z = t(y)(x)
-        >>> t(y).inv(z)
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
         tensor([-2.3267,  1.4581, -1.6776])
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
@@ -646,15 +714,15 @@
                 order=torch.randperm(features) if randperm else orders[i % 2],
                 **kwargs,
             )
             for i in range(transforms)
         ]
 
         for i in reversed(range(len(transforms))):
-            transforms.insert(i, Unconditional(SoftclipTransform))
+            transforms.insert(i, Unconditional(SoftclipTransform, bound=6.0))
 
         base = Unconditional(
             DiagNormal,
             torch.zeros(features),
             torch.ones(features),
             buffer=True,
         )
@@ -702,17 +770,17 @@
             (4): Linear(in_features=64, out_features=1, bias=True)
             (5): Softplus(beta=1, threshold=20)
           )
         )
         >>> x = torch.randn(3)
         >>> x
         tensor([-0.0103, -1.0871, -0.0667])
-        >>> y = torch.randn(4)
-        >>> z = t(y)(x)
-        >>> t(y).inv(z)
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
         tensor([-0.0103, -1.0871, -0.0667])
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
@@ -783,26 +851,170 @@
                 order=torch.randperm(features) if randperm else orders[i % 2],
                 **kwargs,
             )
             for i in range(transforms)
         ]
 
         for i in reversed(range(len(transforms))):
-            transforms.insert(i, Unconditional(SoftclipTransform))
+            transforms.insert(i, Unconditional(SoftclipTransform, bound=6.0))
 
         base = Unconditional(
             DiagNormal,
             torch.zeros(features),
             torch.ones(features),
             buffer=True,
         )
 
         super().__init__(transforms, base)
 
 
+class GeneralCouplingTransform(TransformModule):
+    r"""Creates a general coupling transformation.
+
+    References:
+        | NICE: Non-linear Independent Components Estimation (Dinh et al., 2014)
+        | https://arxiv.org/abs/1410.8516
+
+    Arguments:
+        features: The number of features.
+        context: The number of context features.
+        mask: The coupling mask. If :py:`None`, use a checkered mask.
+        univariate: The univariate transformation constructor.
+        shapes: The shapes of the univariate transformation parameters.
+        kwargs: Keyword arguments passed to :class:`zuko.nn.MLP`.
+
+    Example:
+        >>> t = GeneralCouplingTransform(3, 4)
+        >>> t
+        GeneralCouplingTransform(
+          (base): MonotonicAffineTransform()
+          (order): [0, 1, 0]
+          (hyper): MLP(
+            (0): Linear(in_features=5, out_features=64, bias=True)
+            (1): ReLU()
+            (2): Linear(in_features=64, out_features=64, bias=True)
+            (3): ReLU()
+            (4): Linear(in_features=64, out_features=4, bias=True)
+          )
+        )
+        >>> x = torch.randn(3)
+        >>> x
+        tensor([-0.8743,  0.6232,  1.2439])
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
+        tensor([-0.8743,  0.6232,  1.2439])
+    """
+
+    def __init__(
+        self,
+        features: int,
+        context: int = 0,
+        mask: BoolTensor = None,
+        univariate: Callable[..., Transform] = MonotonicAffineTransform,
+        shapes: Sequence[Size] = ((), ()),
+        **kwargs,
+    ):
+        super().__init__()
+
+        # Univariate transformation
+        self.univariate = univariate
+        self.shapes = shapes
+        self.total = sum(prod(s) for s in shapes)
+
+        # Mask
+        self.register_buffer('mask', None)
+
+        if mask is None:
+            self.mask = torch.arange(features) % 2 == 1
+        else:
+            self.mask = mask
+
+        features_a = self.mask.sum().item()
+        features_b = features - features_a
+
+        # Hyper network
+        self.hyper = MLP(features_a + context, features_b * self.total, **kwargs)
+
+    def extra_repr(self) -> str:
+        base = self.univariate(*map(torch.randn, self.shapes))
+        mask = self.mask.int().tolist()
+
+        if len(mask) > 10:
+            mask = mask[:5] + [...] + mask[-5:]
+            mask = str(mask).replace('Ellipsis', '...')
+
+        return '\n'.join([
+            f'(base): {base}',
+            f'(mask): {mask}',
+        ])
+
+    def meta(self, c: Tensor, x: Tensor) -> Transform:
+        if c is not None:
+            x = torch.cat(broadcast(x, c, ignore=1), dim=-1)
+
+        phi = self.hyper(x)
+        phi = phi.unflatten(-1, (-1, self.total))
+        phi = unpack(phi, self.shapes)
+
+        return DependentTransform(self.univariate(*phi), 1)
+
+    def forward(self, c: Tensor = None) -> Transform:
+        return CouplingTransform(partial(self.meta, c), self.mask)
+
+
+class GCF(FlowModule):
+    r"""Creates a general coupling flow (GCF).
+
+    Arguments:
+        features: The number of features.
+        context: The number of context features.
+        transforms: The number of coupling transformations.
+        randmask: Whether random coupling masks are used or not. If :py:`False`,
+            use alternating checkered masks.
+        features are in ascending (descending) order for even
+            (odd) transformations.
+        kwargs: Keyword arguments passed to :class:`GeneralCouplingTransform`.
+    """
+
+    def __init__(
+        self,
+        features: int,
+        context: int = 0,
+        transforms: int = 3,
+        randmask: bool = False,
+        **kwargs,
+    ):
+        temp = []
+
+        for i in range(transforms):
+            if randmask:
+                mask = torch.randperm(features) % 2 == i % 2
+            else:
+                mask = torch.arange(features) % 2 == i % 2
+
+            temp.append(
+                GeneralCouplingTransform(
+                    features=features,
+                    context=context,
+                    mask=mask,
+                    **kwargs,
+                )
+            )
+
+        base = Unconditional(
+            DiagNormal,
+            torch.zeros(features),
+            torch.ones(features),
+            buffer=True,
+        )
+
+        super().__init__(temp, base)
+
+
 class FFJTransform(TransformModule):
     r"""Creates a free-form Jacobian (FFJ) transformation.
 
     References:
         | FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl et al., 2018)
         | https://arxiv.org/abs/1810.01367
 
@@ -825,17 +1037,17 @@
             (3): ELU(alpha=1.0)
             (4): Linear(in_features=64, out_features=3, bias=True)
           )
         )
         >>> x = torch.randn(3)
         >>> x
         tensor([ 0.1777,  1.0139, -1.0370])
-        >>> y = torch.randn(4)
-        >>> z = t(y)(x)
-        >>> t(y).inv(z)
+        >>> c = torch.randn(4)
+        >>> y = t(c)(x)
+        >>> t(c).inv(y)
         tensor([ 0.1777,  1.0139, -1.0370])
     """
 
     def __init__(
         self,
         features: int,
         context: int = 0,
@@ -850,31 +1062,31 @@
         self.ode = MLP(features + context + 2 * freqs, features, **kwargs)
 
         self.register_buffer('times', torch.tensor((0.0, 1.0)))
         self.register_buffer('freqs', torch.arange(1, freqs + 1) * pi)
 
         self.exact = exact
 
-    def f(self, t: Tensor, x: Tensor, y: Tensor = None) -> Tensor:
+    def f(self, t: Tensor, x: Tensor, c: Tensor = None) -> Tensor:
         t = self.freqs * t[..., None]
         t = torch.cat((t.cos(), t.sin()), dim=-1)
 
-        if y is None:
+        if c is None:
             x = torch.cat(broadcast(t, x, ignore=1), dim=-1)
         else:
-            x = torch.cat(broadcast(t, x, y, ignore=1), dim=-1)
+            x = torch.cat(broadcast(t, x, c, ignore=1), dim=-1)
 
         return self.ode(x)
 
-    def forward(self, y: Tensor = None) -> Transform:
+    def forward(self, c: Tensor = None) -> Transform:
         return FreeFormJacobianTransform(
-            f=partial(self.f, y=y),
+            f=partial(self.f, c=c),
             t0=self.times[0],
             t1=self.times[1],
-            phi=self.parameters() if y is None else (y, *self.parameters()),
+            phi=self.parameters() if c is None else (c, *self.parameters()),
             exact=self.exact,
         )
 
 
 class CNF(FlowModule):
     r"""Creates a continuous normalizing flow (CNF) with free-form Jacobian
     transformations.
```

### Comparing `zuko-0.2.1/zuko/nn.py` & `zuko-0.2.2/zuko/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,17 +269,15 @@
         tensor([[0.8742, 0.9439, 0.9759],
                 [0.8969, 0.9716, 0.9866],
                 [1.0780, 1.1651, 1.2056],
                 [0.8596, 0.9400, 0.9502]])
     """
 
     def __init__(self, *args, **kwargs):
-        kwargs['activation'] = nn.ELU
+        kwargs['activation'] = TwoWayELU
         kwargs['normalize'] = False
 
         super().__init__(*args, **kwargs)
 
-        for i, layer in enumerate(self):
+        for layer in self:
             if isinstance(layer, nn.Linear):
                 layer.__class__ = MonotonicLinear
-            elif isinstance(layer, nn.ELU):
-                layer.__class__ = TwoWayELU
```

### Comparing `zuko-0.2.1/zuko/transforms.py` & `zuko-0.2.2/zuko/transforms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 r"""Parameterizable transformations."""
 
 __all__ = [
     'ComposedTransform',
+    'DependentTransform',
     'IdentityTransform',
     'CosTransform',
     'SinTransform',
     'SoftclipTransform',
     'CircularShiftTransform',
     'MonotonicAffineTransform',
     'MonotonicRQSTransform',
     'MonotonicTransform',
     'UnconstrainedMonotonicTransform',
     'SOSPolynomialTransform',
     'FreeFormJacobianTransform',
     'AutoregressiveTransform',
+    'CouplingTransform',
     'LULinearTransform',
     'PermutationTransform',
 ]
 
 import math
 import torch
 import torch.nn.functional as F
 
 from textwrap import indent
-from torch import Tensor, LongTensor, Size
+from torch import Tensor, BoolTensor, LongTensor, Size
 from torch.distributions import *
 from torch.distributions import constraints
 from torch.distributions.utils import _sum_rightmost
 from typing import *
 
 from .utils import bisection, broadcast, gauss_legendre, odeint
 
@@ -47,14 +49,16 @@
 
 Transform.call_and_ladj = _call_and_ladj
 
 
 class ComposedTransform(Transform):
     r"""Creates a transformation :math:`f(x) = f_n \circ \dots \circ f_0(x)`.
 
+    Optimized version of :class:`torch.distributions.transforms.ComposeTransform`.
+
     Arguments:
         transforms: A sequence of transformations :math:`f_i`.
     """
 
     def __init__(self, *transforms: Transform, **kwargs):
         super().__init__(**kwargs)
 
@@ -146,14 +150,74 @@
 
     def inverse_shape(self, shape: Size) -> Size:
         for t in reversed(self.transforms):
             shape = t.inverse_shape(shape)
         return shape
 
 
+class DependentTransform(Transform):
+    r"""Wraps a base transformation to treat right-most dimensions as dependent.
+
+    Optimized version of :class:`torch.distributions.transforms.IndependentTransform`.
+
+    Arguments:
+        base: The base transformation.
+        reinterpreted: The number of dimensions to treat as dependent.
+    """
+
+    def __init__(self, base: Transform, reinterpreted: int, **kwargs):
+        super().__init__(**kwargs)
+
+        self.base = base
+        self.reinterpreted = reinterpreted
+
+    def __repr__(self) -> str:
+        return f'{self.__class__.__name__}({self.base}, {self.reinterpreted})'
+
+    @property
+    def domain(self) -> constraints.Constraint:
+        return constraints.independent(self.base.domain, self.reinterpreted)
+
+    @property
+    def codomain(self) -> constraints.Constraint:
+        return constraints.independent(self.base.codomain, self.reinterpreted)
+
+    @property
+    def bijective(self) -> bool:
+        return self.base.bijective
+
+    def _call(self, x: Tensor) -> Tensor:
+        return self.base(x)
+
+    @property
+    def inv(self) -> Transform:
+        return DependentTransform(self.base.inv, self.reinterpreted)
+
+    def _inverse(self, y: Tensor) -> Tensor:
+        return self.base.inv(y)
+
+    def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
+        ladj = self.base.log_abs_det_jacobian(x, y)
+        ladj = _sum_rightmost(ladj, self.reinterpreted)
+
+        return ladj
+
+    def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        y, ladj = self.base.call_and_ladj(x)
+        ladj = ladj = _sum_rightmost(ladj, self.reinterpreted)
+
+        return y, ladj
+
+    def forward_shape(self, shape: Size) -> Size:
+        return self.base.forward_shape(shape)
+
+    def inverse_shape(self, shape: Size) -> Size:
+        return self.base.inverse_shape(shape)
+
+
 class IdentityTransform(Transform):
     r"""Creates a transformation :math:`f(x) = x`."""
 
     domain = constraints.real
     codomain = constraints.real
     bijective = True
     sign = +1
@@ -713,19 +777,83 @@
         x = torch.zeros_like(y)
         for _ in range(self.passes):
             x = self.meta(x).inv(y)
 
         return x
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
-        return self.meta(x).log_abs_det_jacobian(x, y).sum(dim=-1)
+        return self.meta(x).log_abs_det_jacobian(x, y)
 
     def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
         y, ladj = self.meta(x).call_and_ladj(x)
-        return y, ladj.sum(dim=-1)
+        return y, ladj
+
+
+class CouplingTransform(Transform):
+    r"""Transform via a coupling scheme.
+
+    .. math::
+        y_a & = x_a \\
+        y_b & = f(x_b; x_a)
+
+    Arguments:
+        meta: A meta function which returns a transformation :math:`f`.
+        mask: A coupling mask defining the split $x \mapsto (x_a, x_b)$.
+    """
+
+    domain = constraints.real_vector
+    codomain = constraints.real_vector
+    bijective = True
+
+    def __init__(
+        self,
+        meta: Callable[[Tensor], Transform],
+        mask: BoolTensor,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+
+        self.meta = meta
+        self.idx_a = mask.nonzero().squeeze(-1)
+        self.idx_b = (~mask).nonzero().squeeze(-1)
+
+    def split(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        return x[..., self.idx_a], x[..., self.idx_b]
+
+    def merge(self, x_a: Tensor, x_b: Tensor, shape: Size) -> Tensor:
+        x = x_a.new_empty(shape)
+        x[..., self.idx_a] = x_a
+        x[..., self.idx_b] = x_b
+
+        return x
+
+    def _call(self, x: Tensor) -> Tensor:
+        x_a, x_b = self.split(x)
+        y_b = self.meta(x_a)(x_b)
+
+        return self.merge(x_a, y_b, x.shape)
+
+    def _inverse(self, y: Tensor) -> Tensor:
+        y_a, y_b = self.split(y)
+        x_b = self.meta(y_a).inv(y_b)
+
+        return self.merge(y_a, x_b, y.shape)
+
+    def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
+        x_a, x_b = self.split(x)
+        _, y_b = self.split(y)
+
+        return self.meta(x_a).log_abs_det_jacobian(x_b, y_b)
+
+    def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        x_a, x_b = self.split(x)
+        y_b, ladj = self.meta(x_a).call_and_ladj(x_b)
+        y = self.merge(x_a, y_b, x.shape)
+
+        return y, ladj
 
 
 class LULinearTransform(Transform):
     r"""Creates a transformation :math:`f(x) = L U x`.
 
     Arguments:
         LU: A matrix whose lower and upper triangular parts are the non-zero elements
@@ -780,15 +908,16 @@
 
         self.order = order
 
     def __repr__(self) -> str:
         order = self.order.tolist()
 
         if len(order) > 10:
-            order = str(order[:5] + [...] + order[-5:]).replace('Ellipsis', '...')
+            order = order[:5] + [...] + order[-5:]
+            order = str(order).replace('Ellipsis', '...')
 
         return f'{self.__class__.__name__}({order})'
 
     def _call(self, x: Tensor) -> Tensor:
         return x[..., self.order]
 
     def _inverse(self, y: Tensor) -> Tensor:
```

### Comparing `zuko-0.2.1/zuko/utils.py` & `zuko-0.2.2/zuko/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 r"""General purpose helpers."""
 
 from __future__ import annotations
 
-__all__ = ['bisection', 'broadcast', 'gauss_legendre', 'odeint']
+__all__ = ['bisection', 'broadcast', 'gauss_legendre', 'odeint', 'unpack']
 
+import math
 import numpy as np
 import torch
 
 from functools import lru_cache
-from torch import Tensor
+from torch import Tensor, Size
 from typing import *
 
 
 def bisection(
     f: Callable[[Tensor], Tensor],
     y: Tensor,
     a: Union[float, Tensor],
@@ -290,32 +291,28 @@
         tensor([-3.7454, -0.4140,  0.2677])
     """
 
     if torch.is_tensor(x):
         g = None
     else:
         shapes = [y.shape for y in x]
-        sizes = [y.numel() for y in x]
 
         def pack(x: Sequence[Tensor]) -> Tensor:
             return torch.cat([y.flatten() for y in x])
 
-        def unpack(x: Tensor) -> Sequence[Tensor]:
-            return [y.reshape(s) for y, s in zip(x.split(sizes), shapes)]
-
         x = pack(x)
-        g = lambda t, x: pack(f(t, *unpack(x)))
+        g = lambda t, x: pack(f(t, *unpack(x, shapes)))
 
     t0 = torch.as_tensor(t0).to(x)
     t1 = torch.as_tensor(t1).to(x)
 
     if g is None:
         return AdaptiveCheckpointAdjoint.apply(f, x, t0, t1, *phi)
     else:
-        return unpack(AdaptiveCheckpointAdjoint.apply(g, x, t0, t1, *phi))
+        return unpack(AdaptiveCheckpointAdjoint.apply(g, x, t0, t1, *phi), shapes)
 
 
 def dopri45(
     f: Callable[[Tensor, Tensor], Tensor],
     x: Tensor,
     t: Tensor,
     dt: Tensor,
@@ -460,7 +457,36 @@
         # Initial time
         if ctx.needs_input_grad[2]:
             grad_t0 = f(t0, x0) * grad_x
         else:
             grad_t0 = None
 
         return (None, grad_x, grad_t0, grad_t1, *grad_phi)
+
+
+def unpack(x: Tensor, shapes: Sequence[Size]) -> List[Tensor]:
+    r"""Unpacks a packed tensor.
+
+    Arguments:
+        x: A packed tensor, with shape :math:`(*, D)`.
+        shapes: A sequence of shapes :math:`S_i`, corresponding to the total number of
+            elements :math:`D`.
+
+    Returns:
+        The unpacked tensors, with shapes :math:`(*, S_i)`.
+
+    Example:
+        >>> x = torch.randn(26)
+        >>> y, z = unpack(x, ((1, 2, 3), (4, 5)))
+        >>> y.shape
+        torch.Size([1, 2, 3])
+        >>> z.shape
+        torch.Size([4, 5])
+    """
+
+    sizes = [math.prod(s) for s in shapes]
+
+    x = x.split(sizes, -1)
+    x = (y.unflatten(-1, (*s, 1)) for y, s in zip(x, shapes))
+    x = (y.squeeze(-1) for y in x)
+
+    return list(x)
```

### Comparing `zuko-0.2.1/zuko.egg-info/PKG-INFO` & `zuko-0.2.2/zuko.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.2.1
+Version: 0.2.2
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -39,36 +39,58 @@
 
 ```
 pip install git+https://github.com/francois-rozet/zuko
 ```
 
 ## Getting started
 
-Normalizing flows are provided in the `zuko.flows` module. To build one, supply the number of sample and context features as well as the transformations' hyperparameters. Then, feeding a context `y` to the flow returns a conditional distribution `p(x | y)` which can be evaluated and sampled from.
+Normalizing flows are provided in the `zuko.flows` module. To build one, supply the number of sample and context features as well as the transformations' hyperparameters. Then, feeding a context $c$ to the flow returns a conditional distribution $p(x | c)$ which can be evaluated and sampled from.
 
 ```python
 import torch
 import zuko
 
 # Neural spline flow (NSF) with 3 sample features and 5 context features
 flow = zuko.flows.NSF(3, 5, transforms=3, hidden_features=[128] * 3)
 
 # Train to maximize the log-likelihood
 optimizer = torch.optim.AdamW(flow.parameters(), lr=1e-3)
 
-for x, y in trainset:
-    loss = -flow(y).log_prob(x)  # -log p(x | y)
+for x, c in trainset:
+    loss = -flow(c).log_prob(x)  # -log p(x | c)
     loss = loss.mean()
 
     optimizer.zero_grad()
     loss.backward()
     optimizer.step()
 
-# Sample 64 points x ~ p(x | y*)
-x = flow(y_star).sample((64,))
+# Sample 64 points x ~ p(x | c*)
+x = flow(c_star).sample((64,))
+```
+
+Alternatively, flows can be built as custom `FlowModule` objects.
+
+```python
+from zuko.flows import FlowModule, MaskedAutoregressiveTransform, Unconditional
+from zuko.distributions import DiagNormal
+from zuko.transforms import PermutationTransform
+
+flow = FlowModule(
+    transforms=[
+        MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
+        Unconditional(PermutationTransform, torch.randperm(3), buffer=True),
+        MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
+    ],
+    base=Unconditional(
+        DiagNormal,
+        torch.zeros(3),
+        torch.ones(3),
+        buffer=True,
+    ),
+)
 ```
 
 For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
```

