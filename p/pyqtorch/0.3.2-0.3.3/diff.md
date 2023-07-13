# Comparing `tmp/pyqtorch-0.3.2.tar.gz` & `tmp/pyqtorch-0.3.3.tar.gz`

## Comparing `pyqtorch-0.3.2.tar` & `pyqtorch-0.3.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_converters.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/LICENSE
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/mkdocs.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    23548 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    12189 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_converters.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.3/PKG-INFO
```

### Comparing `pyqtorch-0.3.2/.pre-commit-config.yaml` & `pyqtorch-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/CODE_OF_CONDUCT.md` & `pyqtorch-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/CONTRIBUTING.md` & `pyqtorch-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/mkdocs.yml` & `pyqtorch-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.3.3/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/QAOA.ipynb` & `pyqtorch-0.3.3/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/essentials.ipynb` & `pyqtorch-0.3.3/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/fit_function.ipynb` & `pyqtorch-0.3.3/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/gate_composition.ipynb` & `pyqtorch-0.3.3/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/hamevo.md` & `pyqtorch-0.3.3/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.3.3/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/bench.py` & `pyqtorch-0.3.3/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.3.3/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.3.3/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.3.3/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.3.3/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/__init__.py` & `pyqtorch-0.3.3/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/ansatz.py` & `pyqtorch-0.3.3/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/embedding.py` & `pyqtorch-0.3.3/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/matrices.py` & `pyqtorch-0.3.3/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/matrices_sparse.py` & `pyqtorch-0.3.3/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/converters/store_ops.py` & `pyqtorch-0.3.3/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.3.3/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/__init__.py` & `pyqtorch-0.3.3/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/batched_operation.py` & `pyqtorch-0.3.3/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/circuit.py` & `pyqtorch-0.3.3/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/measurement.py` & `pyqtorch-0.3.3/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/operation.py` & `pyqtorch-0.3.3/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/core/utils.py` & `pyqtorch-0.3.3/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/__init__.py` & `pyqtorch-0.3.3/pyqtorch/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/abstract.py` & `pyqtorch-0.3.3/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/circuit.py` & `pyqtorch-0.3.3/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/hamevo.py` & `pyqtorch-0.3.3/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/parametric.py` & `pyqtorch-0.3.3/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/primitive.py` & `pyqtorch-0.3.3/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyqtorch/modules/utils.py` & `pyqtorch-0.3.3/pyqtorch/modules/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,21 @@
 import torch
 
 
 def normalize(wf: torch.Tensor) -> torch.Tensor:
     return wf / torch.sqrt((wf.abs() ** 2).sum())
 
 
-def is_normalized(state: torch.Tensor, atol: float = 1e-07) -> bool:
+def is_normalized(state: torch.Tensor, atol: float = 1e-15) -> bool:
     n_qubits = len(state.size()) - 1
     batch_size = state.size()[-1]
     state = state.reshape((2**n_qubits, batch_size))
-
-    def _is_normalized(state: torch.Tensor) -> torch.Tensor:
-        sum_probs: torch.Tensor = (state.abs() ** 2).sum(dim=0)
-        if not torch.allclose(sum_probs, torch.ones(batch_size), rtol=0.0, atol=atol):
-            breakpoint()
-        return True
-
-    return _is_normalized(state)  # type: ignore[no-any-return]
+    sum_probs = (state.abs() ** 2).sum(dim=0)
+    ones = torch.ones(batch_size)
+    return torch.allclose(sum_probs, ones, rtol=0.0, atol=atol)  # type:ignore[no-any-return]
 
 
 def is_diag(H: torch.Tensor) -> bool:
     """
     Returns True if Hamiltonian H is diagonal.
     """
     return len(torch.abs(torch.triu(H, diagonal=1)).to_sparse().coalesce().values()) == 0
@@ -38,19 +33,17 @@
 def overlap(state: torch.Tensor, other: torch.Tensor) -> torch.Tensor:
     n_qubits = len(state.size()) - 1
     batch_size = state.size()[-1]
     state = state.reshape((2**n_qubits, batch_size))
     other = other.reshape((2**n_qubits, batch_size))
     res = []
     for i in range(batch_size):
-        s = state[:, i]
-        o = other[:, i]
-        ovrlp = torch.real(torch.sum(torch.conj(s) * o))
+        ovrlp = torch.real(torch.sum(torch.conj(state[:, i]) * other[:, i]))
         res.append(ovrlp)
-    return torch.tensor(res)
+    return torch.stack(res)
 
 
 def rot_matrices(
     theta: torch.Tensor, P: torch.Tensor, I: torch.Tensor, batch_size: int  # noqa: E741
 ) -> torch.Tensor:
     """
     Returns:
@@ -151,11 +144,13 @@
     dtype: torch.dtype = torch.cdouble,
 ) -> torch.Tensor:
     def _rand(n_qubits: int) -> torch.Tensor:
         N = 2**n_qubits
         x = -torch.log(torch.rand(N))
         sumx = torch.sum(x)
         phases = torch.rand(N) * 2.0 * torch.pi
-        return (torch.sqrt(x / sumx) * torch.exp(1j * phases)).reshape(N, 1).type(dtype).to(device)
+        return normalize(
+            (torch.sqrt(x / sumx) * torch.exp(1j * phases)).reshape(N, 1).type(dtype).to(device)
+        )
 
     _state = torch.concat(tuple(_rand(n_qubits) for _ in range(batch_size)), dim=1)
     return _state.reshape([2] * n_qubits + [batch_size])
```

### Comparing `pyqtorch-0.3.2/tests/conftest.py` & `pyqtorch-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_batched_operations.py` & `pyqtorch-0.3.3/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_converters.py` & `pyqtorch-0.3.3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_module_hamevo.py` & `pyqtorch-0.3.3/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_modules.py` & `pyqtorch-0.3.3/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_notebooks.py` & `pyqtorch-0.3.3/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_operations.py` & `pyqtorch-0.3.3/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/tests/test_operations_hamevo.py` & `pyqtorch-0.3.3/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/.gitignore` & `pyqtorch-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/LICENSE` & `pyqtorch-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.3.2/pyproject.toml` & `pyqtorch-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.3.2"
+version = "0.3.3"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.3.2/PKG-INFO` & `pyqtorch-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.3.2
+Version: 0.3.3
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

