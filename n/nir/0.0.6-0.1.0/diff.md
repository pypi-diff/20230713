# Comparing `tmp/nir-0.0.6.tar.gz` & `tmp/nir-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nir-0.0.6.tar", last modified: Tue Jul 11 02:14:02 2023, max compression
+gzip compressed data, was "nir-0.1.0.tar", last modified: Thu Jul 13 00:57:55 2023, max compression
```

## Comparing `nir-0.0.6.tar` & `nir-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-11 02:14:02.646000 nir-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-11 02:13:53.000000 nir-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 02:13:53.000000 nir-0.0.6/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/nir/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 02:13:53.000000 nir-0.0.6/nir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-11 02:13:53.000000 nir-0.0.6/nir/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-11 02:13:53.000000 nir-0.0.6/nir/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 02:13:53.000000 nir-0.0.6/nir/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/nir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-11 02:13:53.000000 nir-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:14:02.646000 nir-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 02:13:53.000000 nir-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-11 02:13:53.000000 nir-0.0.6/tests/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-11 02:13:53.000000 nir-0.0.6/tests/test_readwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.739388 nir-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-13 00:57:55.739388 nir-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-13 00:57:46.000000 nir-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.735388 nir-0.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.735388 nir-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-13 00:57:46.000000 nir-0.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.739388 nir-0.1.0/nir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 00:57:46.000000 nir-0.1.0/nir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-13 00:57:46.000000 nir-0.1.0/nir/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-13 00:57:46.000000 nir-0.1.0/nir/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-13 00:57:46.000000 nir-0.1.0/nir/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.739388 nir-0.1.0/nir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-13 00:57:55.000000 nir-0.1.0/nir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 00:57:55.000000 nir-0.1.0/nir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:57:55.000000 nir-0.1.0/nir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 00:57:55.000000 nir-0.1.0/nir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 00:57:55.000000 nir-0.1.0/nir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-13 00:57:46.000000 nir-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:57:55.739388 nir-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:55.739388 nir-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:57:46.000000 nir-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-13 00:57:46.000000 nir-0.1.0/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-13 00:57:46.000000 nir-0.1.0/tests/test_readwrite.py
```

### Comparing `nir-0.0.6/PKG-INFO` & `nir-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.6
+Version: 0.1.0
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -57,30 +57,32 @@
 ## Frameworks that currently support NIR
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
-| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ✓ | ✓ |
 | [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
+| [snnTorch](https://github.com/jeshraghian/snntorch/) | ✓ | ⬚ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
 * [Sadique Sheik](https://github.com/sheiksadique)
+* [Peng Zhou](https://github.com/pengzhouzp)
 
 If you use NIR in your work, please cite the [following Zenodo reference](https://zenodo.org/record/8105042)
 
 ```
 @software{nir2023,
   author       = {Abreu, Steven and
                   Bauer, Felix and
```

### Comparing `nir-0.0.6/README.md` & `nir-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,30 +38,32 @@
 ## Frameworks that currently support NIR
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
-| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ✓ | ✓ |
 | [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
+| [snnTorch](https://github.com/jeshraghian/snntorch/) | ✓ | ⬚ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
 * [Sadique Sheik](https://github.com/sheiksadique)
+* [Peng Zhou](https://github.com/pengzhouzp)
 
 If you use NIR in your work, please cite the [following Zenodo reference](https://zenodo.org/record/8105042)
 
 ```
 @software{nir2023,
   author       = {Abreu, Steven and
                   Bauer, Felix and
```

### Comparing `nir-0.0.6/docs/source/conf.py` & `nir-0.1.0/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,29 +10,49 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath("../.."))
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "NIR"
 copyright = "2023, NIR team"
 author = "NIR team"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["myst_parser", "sphinx.ext.autodoc", "sphinx.ext.mathjax"]
+extensions = [
+    "myst_parser",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.autosummary",
+    "sphinx_external_toc",
+]
+external_toc_path = "toc.yml"
+
+myst_enable_extensions = [
+    "amsmath",
+    "dollarmath",
+]
+
+# Maps source configuration
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".txt": "markdown",
+    ".md": "markdown",
+}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -44,15 +64,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 # html_theme = 'alabaster'
 html_theme = "sphinx_book_theme"
 
 html_theme_options = {
-    "search_bar_text": "Search this book...",
+    "search_bar_text": "Search NIR docs...",
     "repository_url": "https://github.com/neuromorphs/nir",
     "repository_branch": "docs",
     "use_repository_button": True,
     "use_edit_page_button": False,
     "use_issues_button": True,
 }
```

### Comparing `nir-0.0.6/nir/ir.py` & `nir-0.1.0/nir/ir.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 import typing
 
 import numpy as np
 
 
-Edges = typing.NewType("Edges", typing.List[typing.Tuple[int, int]])
+Edges = typing.NewType("Edges", typing.List[typing.Tuple[str, str]])
 
 
 class NIRNode:
     """Base superclass of Neural Intermediate Representation Unit (NIR).
     All NIR primitives inherit from this class, but NIRNodes should never be
     instantiated.
     """
@@ -17,21 +17,32 @@
 @dataclass
 class NIRGraph(NIRNode):
     """Neural Intermediate Representation (NIR) Graph containing a number
     of nodes and edges.
 
     A graph of computational nodes and identity edges."""
 
-    nodes: typing.List[NIRNode]  # List of computational nodes
+    nodes: typing.Dict[str, NIRNode]  # List of computational nodes
     edges: Edges
 
+    @staticmethod
+    def from_list(*nodes: NIRNode) -> "NIRGraph":
+        """Create a sequential graph from a list of nodes by labelling them
+        after indices."""
+        return NIRGraph(
+            nodes={str(i): n for i, n in enumerate(nodes)},
+            edges=[(str(i), str(i + 1)) for i in range(len(nodes) - 1)],
+        )
+
 
 @dataclass
 class Affine(NIRNode):
-    r"""Affine transform:
+    r"""Affine transform that linearly maps and translates the input signal.
+
+    This is equivalent to the `Affine transformation <https://en.wikipedia.org/wiki/Affine_transformation>`_
 
     .. math::
         y(t) = W*x(t) + b
     """
     weight: np.ndarray  # Weight term
     bias: np.ndarray  # Bias term
 
@@ -55,14 +66,69 @@
     weight: np.ndarray  # Weight C_out * C_in * X * Y
     stride: int  # Stride
     padding: int  # Padding
     dilation: int  # Dilation
     groups: int  # Groups
     bias: np.ndarray  # Bias C_out
 
+    def __post_init__(self):
+        if isinstance(self.stride, int):
+            self.stride = (self.stride, self.stride)
+        if isinstance(self.padding, int):
+            self.padding = (self.padding, self.padding)
+        if isinstance(self.dilation, int):
+            self.dilation = (self.dilation, self.dilation)
+
+
+@dataclass
+class CubaLIF(NIRNode):
+    r"""Current based leaky integrate and-fire-neuron model.
+
+    The current based leaky integrate-and-fire neuron model
+    is defined by the following equations:
+
+    .. math::
+        \tau_{syn} \dot {I} = - I + w_{in} S
+
+    .. math::
+        \tau_{mem} \dot {v} = (v_{leak} - v) + R I
+
+    .. math::
+        z = \begin{cases}
+            1 & v > v_{threshold} \\
+            0 & else
+        \end{cases}
+
+    .. math::
+        v = \begin{cases}
+            v-v_{threshold} & z=1 \\
+            v & else
+        \end{cases}
+
+    Where :math:`\tau_{syn}` is the synaptic time constant,
+    :math:`\tau_{mem}` is the membrane time constant,
+    :math:`w_{in}` is the input current weight (elementwise),
+    :math:`v` is the membrane potential,
+    :math:`v_{leak}` is the leak voltage,
+    :math:`R` is the resistance,
+    :math:`v_{threshold}` is the firing threshold,
+    and :math:`S` is the input spike.
+    """
+
+    tau_syn: np.ndarray  # Time constant
+    tau_mem: np.ndarray  # Time constant
+    r: np.ndarray  # Resistance
+    v_leak: np.ndarray  # Leak voltage
+    v_threshold: np.ndarray  # Firing threshold
+    w_in: np.ndarray = 1.0  # Input current weight
+
+    def __post_init__(self):
+        # If w_in is a scalar, make it an array of same shape as v_threshold
+        self.w_in = np.ones_like(self.v_threshold) * self.w_in
+
 
 @dataclass
 class Delay(NIRNode):
     """Simple delay node.
 
     This node implements a simple delay:
 
@@ -70,14 +136,25 @@
         y(t) = x(t - \tau)
     """
 
     delay: np.ndarray  # Delay
 
 
 @dataclass
+class Flatten(NIRNode):
+    """Flatten node.
+
+    This node flattens its input tensor.
+    """
+
+    start_dim: int = 1  # First dimension to flatten
+    end_dim: int = -1  # Last dimension to flatten
+
+
+@dataclass
 class I(NIRNode):  # noqa: E742
     r"""Integrator
 
     The integrator neuron model is defined by the following equation:
 
     .. math::
         \dot{v} = R I
@@ -180,61 +257,35 @@
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
     v_threshold: np.ndarray  # Firing threshold
 
 
 @dataclass
-class CubaLIF(NIRNode):
-    r"""Current based leaky integrate and-fire-neuron model.
-
-    The current based leaky integrate-and-fire neuron model
-    is defined by the following equations:
-
-    .. math::
-        \tau_syn \ dot{I} = - I + S
-
-        \tau_mem \dot{v} = (v_{leak} - v) + R I
-
-    .. math::
-        z = \begin{cases}
-            1 & v > v_{thr} \\
-            0 & else
-        \end{cases}
-
-    .. math::
-        v = \begin{cases}
-            v-v_{thr} & z=1 \\
-            v & else
-        \end{cases}
+class Output(NIRNode):
+    """Output Node.
 
-    Where :math:`\tau_syn` is the synaptic time constant,
-    :math:`\tau_mem` is the membrane time constant,
-    :math:`v` is the membrane potential,
-    :math:`v_{leak}` is the leak voltage,
-    :math:`R` is the resistance,
-    :math:`v_{threshold}` is the firing threshold,
-    and :math:`S` is the input spike.
+    Defines an output of the graph.
     """
 
-    tau_syn: np.ndarray  # Time constant
-    tau_mem: np.ndarray  # Time constant
-    r: np.ndarray  # Resistance
-    v_leak: np.ndarray  # Leak voltage
-    v_threshold: np.ndarray  # Firing threshold
+    shape: int  # Size of output
 
 
 @dataclass
-class Output(NIRNode):
-    """Output Node.
+class Scale(NIRNode):
+    r"""Scales a signal by some values.
 
-    Defines an output of the graph.
+    This node is equivalent to the
+    `Hadamard product <https://en.wikipedia.org/wiki/Hadamard_product_(matrices)>`_.
+
+    .. math::
+        y(t) = x(t) \odot s
     """
 
-    pass
+    scale: np.ndarray  # Scaling factor
 
 
 @dataclass
 class Threshold(NIRNode):
     r"""Threshold node.
 
     This node implements the heaviside step function:
```

### Comparing `nir-0.0.6/nir/read.py` & `nir-0.1.0/nir/read.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,19 @@
             groups=node["groups"][()],
             bias=node["bias"][()],
         )
     elif node["type"][()] == b"Delay":
         return nir.Delay(
             delay=node["delay"][()],
         )
+    elif node["type"][()] == b"Flatten":
+        return nir.Flatten(
+            start_dim=node["start_dim"][()],
+            end_dim=node["end_dim"][()],
+        )
     elif node["type"][()] == b"I":
         return nir.I(
             r=node["r"][()],
         )
     elif node["type"][()] == b"IF":
         return nir.IF(
             r=node["r"][()],
@@ -70,19 +75,23 @@
             tau_syn=node["tau_syn"][()],
             r=node["r"][()],
             v_leak=node["v_leak"][()],
             v_threshold=node["v_threshold"][()],
         )
     elif node["type"][()] == b"NIRGraph":
         return nir.NIRGraph(
-            nodes=[read_node(n) for n in node["nodes"].values()],
+            nodes={k: read_node(n) for k, n in node["nodes"].items()},
             edges=node["edges"][()],
         )
     elif node["type"][()] == b"Output":
-        return nir.Output()
+        return nir.Output(shape=node["shape"][()])
+    elif node["type"][()] == b"Scale":
+        return nir.Scale(
+            scale=node["scale"][()],
+        )
     elif node["type"][()] == b"Threshold":
         return nir.Threshold(
             threshold=node["threshold"][()],
         )
     else:
         raise ValueError(f"Unknown unit type: {node['type'][()]}")
```

### Comparing `nir-0.0.6/nir/write.py` & `nir-0.1.0/nir/write.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,20 @@
             "padding": node.padding,
             "dilation": node.dilation,
             "groups": node.groups,
             "bias": node.bias,
         }
     elif isinstance(node, nir.Delay):
         return {"type": "Delay", "delay": node.delay}
+    elif isinstance(node, nir.Flatten):
+        return {
+            "type": "Flatten",
+            "start_dim": node.start_dim,
+            "end_dim": node.end_dim,
+        }
     elif isinstance(node, nir.I):
         return {"type": "I", "r": node.r}
     elif isinstance(node, nir.IF):
         return {"type": "IF", "r": node.r, "v_threshold": node.v_threshold}
     elif isinstance(node, nir.Input):
         return {
             "type": "Input",
@@ -73,20 +79,26 @@
             "r": node.r,
             "v_leak": node.v_leak,
             "v_threshold": node.v_threshold,
         }
     elif isinstance(node, nir.NIRGraph):
         return {
             "type": "NIRGraph",
-            "nodes": {i: _convert_node(n) for i, n in enumerate(node.nodes)},
+            "nodes": {k: _convert_node(n) for k, n in node.nodes.items()},
             "edges": node.edges,
         }
     elif isinstance(node, nir.Output):
         return {
             "type": "Output",
+            "shape": node.shape,
+        }
+    elif isinstance(node, nir.Scale):
+        return {
+            "type": "Scale",
+            "scale": node.scale,
         }
     elif isinstance(node, nir.Threshold):
         return {"type": "Threshold", "threshold": node.threshold}
     else:
         raise ValueError(f"Unknown node type: {node}")
```

### Comparing `nir-0.0.6/nir.egg-info/PKG-INFO` & `nir-0.1.0/nir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.6
+Version: 0.1.0
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -57,30 +57,32 @@
 ## Frameworks that currently support NIR
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
-| [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
+| [Rockpool](https://rockpool.ai) | ✓ | ✓ |
 | [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
+| [snnTorch](https://github.com/jeshraghian/snntorch/) | ✓ | ⬚ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
 * [Steven Abreu](https://github.com/stevenabreu7)
 * [Felix Bauer](https://github.com/bauerfe)
 * [Jason Eshraghian](https://github.com/jeshraghian)
 * [Matthias Jobst](https://github.com/matjobst)
 * [Gregor Lenz](https://github.com/biphasic)
 * [Jens Egholm Pedersen](https://github.com/jegp)
 * [Sadique Sheik](https://github.com/sheiksadique)
+* [Peng Zhou](https://github.com/pengzhouzp)
 
 If you use NIR in your work, please cite the [following Zenodo reference](https://zenodo.org/record/8105042)
 
 ```
 @software{nir2023,
   author       = {Abreu, Steven and
                   Bauer, Felix and
```

### Comparing `nir-0.0.6/pyproject.toml` & `nir-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nir"
-version = "0.0.6"
+version = "0.1.0"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsense.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
```

