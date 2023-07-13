# Comparing `tmp/doy-1.1.tar.gz` & `tmp/doy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-1.1.tar", max compression
+gzip compressed data, was "doy-1.2.tar", max compression
```

## Comparing `doy-1.1.tar` & `doy-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.1/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.1/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.1/doy/__init__.py
--rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.1/doy/data.py
--rw-r--r--   0        0        0     1517 2023-07-12 11:50:17.468975 doy-1.1/doy/logger.py
--rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.1/doy/plotting.py
--rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.1/doy/progress.py
--rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.1/doy/rich_utils.py
--rw-r--r--   0        0        0     2685 2023-07-12 13:40:24.055859 doy-1.1/doy/utils.py
--rw-r--r--   0        0        0      360 2023-07-12 13:42:04.040694 doy-1.1/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.1/setup.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-1.2/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-1.2/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0      156 2023-06-06 17:00:27.147433 doy-1.2/doy/__init__.py
+-rw-r--r--   0        0        0      953 2023-06-06 15:22:52.582141 doy-1.2/doy/data.py
+-rw-r--r--   0        0        0     1482 2023-07-12 13:55:22.467360 doy-1.2/doy/logger.py
+-rw-r--r--   0        0        0     4293 2023-06-06 16:07:24.452360 doy-1.2/doy/plotting.py
+-rw-r--r--   0        0        0     2300 2023-06-13 16:15:43.417259 doy-1.2/doy/progress.py
+-rw-r--r--   0        0        0     2561 2023-06-06 16:24:05.628322 doy-1.2/doy/rich_utils.py
+-rw-r--r--   0        0        0     2948 2023-07-13 11:03:55.427841 doy-1.2/doy/utils.py
+-rw-r--r--   0        0        0      360 2023-07-13 11:04:06.411932 doy-1.2/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 doy-1.2/setup.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 doy-1.2/PKG-INFO
```

### Comparing `doy-1.1/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-1.2/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-1.1/doy/data.py` & `doy-1.2/doy/data.py`

 * *Files identical despite different names*

### Comparing `doy-1.1/doy/logger.py` & `doy-1.2/doy/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,9 +44,9 @@
         elif smoothing_method == "conv":
             return smooth_conv(self[key], smoothing_param)
         else:
             raise ValueError(
                 f"Unknown smoothing method: {smoothing_method}, should be 'ema' or 'conv'."
             )
 
-    def save(self, path: Union[str, os.PathLike]):
-        doy.dump({"data": self.data, "data_x": self.data_x}, path)
+    # def asdict(self):
+    #    return {"data": self.data, "data_x": self.data_x}
```

### Comparing `doy-1.1/doy/plotting.py` & `doy-1.2/doy/plotting.py`

 * *Files identical despite different names*

### Comparing `doy-1.1/doy/progress.py` & `doy-1.2/doy/progress.py`

 * *Files identical despite different names*

### Comparing `doy-1.1/doy/rich_utils.py` & `doy-1.2/doy/rich_utils.py`

 * *Files identical despite different names*

### Comparing `doy-1.1/doy/utils.py` & `doy-1.2/doy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,7 +95,15 @@
 
         return result[0] if is_scalar else result
 
     def plot(self):
         xs = np.arange(0, self.points[-1])
         plt.plot(xs, self(xs))
         plt.show()
+
+
+def normalize_into_range(lower, upper, v, ensure_in_range=False):
+    assert lower <= upper
+    if ensure_in_range and (v < lower or v > upper):
+        raise ValueError(f"Value {v} is not in range [{lower}, {upper}]")
+
+    return (v - lower) / (upper - lower)
```

### Comparing `doy-1.1/setup.py` & `doy-1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2', 'numpy', 'rich>=13.4.1', 'tqdm>=4.65.0', 'wandb>=0.15.5']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '1.1',
+    'version': '1.2',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `doy-1.1/PKG-INFO` & `doy-1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doy
-Version: 1.1
+Version: 1.2
 Summary: 
 Author: Dominik Schmidt
 Author-email: schmidtdominik30@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

