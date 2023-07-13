# Comparing `tmp/findpeaks-2.5.0.tar.gz` & `tmp/findpeaks-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpeaks-2.5.0.tar", last modified: Wed Jul 12 20:07:10 2023, max compression
+gzip compressed data, was "findpeaks-2.5.1.tar", last modified: Thu Jul 13 20:09:42 2023, max compression
```

## Comparing `findpeaks-2.5.0.tar` & `findpeaks-2.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.346871 findpeaks-2.5.0/
--rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.5.0/LICENSE
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8724 2023-07-12 20:07:10.344886 findpeaks-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.259363 findpeaks-2.5.0/findpeaks/
--rw-rw-rw-   0        0        0     2232 2023-07-12 20:00:25.000000 findpeaks-2.5.0/findpeaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.315778 findpeaks-2.5.0/findpeaks/data/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/data/__init__.py
--rw-rw-rw-   0        0        0    20069 2023-07-12 18:43:54.000000 findpeaks-2.5.0/findpeaks/examples.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.335315 findpeaks-2.5.0/findpeaks/filters/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/filters/__init__.py
--rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.5.0/findpeaks/filters/frost.py
--rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.5.0/findpeaks/filters/kuan.py
--rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.5.0/findpeaks/filters/lee.py
--rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.5.0/findpeaks/filters/lee_enhanced.py
--rw-rw-rw-   0        0        0    12835 2023-07-12 18:57:51.000000 findpeaks-2.5.0/findpeaks/filters/lee_sigma.py
--rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.5.0/findpeaks/filters/mean.py
--rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.5.0/findpeaks/filters/median.py
--rw-rw-rw-   0        0        0    54480 2023-07-12 19:49:33.000000 findpeaks-2.5.0/findpeaks/findpeaks.py
--rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.5.0/findpeaks/interpolate.py
--rw-rw-rw-   0        0        0    23627 2023-07-12 18:58:17.000000 findpeaks-2.5.0/findpeaks/stats.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.342878 findpeaks-2.5.0/findpeaks/tests/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/tests/__init__.py
--rw-rw-rw-   0        0        0     9288 2023-07-12 18:44:51.000000 findpeaks-2.5.0/findpeaks/tests/test_findpeaks.py
--rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/union_find.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.314142 findpeaks-2.5.0/findpeaks.egg-info/
--rw-rw-rw-   0        0        0     8724 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 20:07:10.346987 findpeaks-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-07-12 15:59:47.000000 findpeaks-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.345222 findpeaks-2.5.1/
+-rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8724 2023-07-13 20:09:42.345222 findpeaks-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.317641 findpeaks-2.5.1/findpeaks/
+-rw-rw-rw-   0        0        0     2232 2023-07-13 20:09:28.000000 findpeaks-2.5.1/findpeaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.333593 findpeaks-2.5.1/findpeaks/data/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.1/findpeaks/data/__init__.py
+-rw-rw-rw-   0        0        0    20214 2023-07-13 11:43:11.000000 findpeaks-2.5.1/findpeaks/examples.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.342599 findpeaks-2.5.1/findpeaks/filters/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.1/findpeaks/filters/__init__.py
+-rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.5.1/findpeaks/filters/frost.py
+-rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.5.1/findpeaks/filters/kuan.py
+-rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.5.1/findpeaks/filters/lee.py
+-rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.5.1/findpeaks/filters/lee_enhanced.py
+-rw-rw-rw-   0        0        0    12835 2023-07-12 18:57:51.000000 findpeaks-2.5.1/findpeaks/filters/lee_sigma.py
+-rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.5.1/findpeaks/filters/mean.py
+-rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.5.1/findpeaks/filters/median.py
+-rw-rw-rw-   0        0        0    54530 2023-07-13 11:41:57.000000 findpeaks-2.5.1/findpeaks/findpeaks.py
+-rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.5.1/findpeaks/interpolate.py
+-rw-rw-rw-   0        0        0    23627 2023-07-12 18:58:17.000000 findpeaks-2.5.1/findpeaks/stats.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.343581 findpeaks-2.5.1/findpeaks/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.1/findpeaks/tests/__init__.py
+-rw-rw-rw-   0        0        0     9288 2023-07-12 18:44:51.000000 findpeaks-2.5.1/findpeaks/tests/test_findpeaks.py
+-rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.5.1/findpeaks/union_find.py
+drwxrwxrwx   0        0        0        0 2023-07-13 20:09:42.332612 findpeaks-2.5.1/findpeaks.egg-info/
+-rw-rw-rw-   0        0        0     8724 2023-07-13 20:09:42.000000 findpeaks-2.5.1/findpeaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-07-13 20:09:42.000000 findpeaks-2.5.1/findpeaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 20:09:42.000000 findpeaks-2.5.1/findpeaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-13 20:09:42.000000 findpeaks-2.5.1/findpeaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 20:09:42.000000 findpeaks-2.5.1/findpeaks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 20:09:42.345222 findpeaks-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-12 15:59:47.000000 findpeaks-2.5.1/setup.py
```

### Comparing `findpeaks-2.5.0/LICENSE` & `findpeaks-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/PKG-INFO` & `findpeaks-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.5.0
+Version: 2.5.1
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.0.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.5.0 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.5.1 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.5.0.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/findpeaks/archive/2.5.1.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
 pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
 [Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
 findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
```

### Comparing `findpeaks-2.5.0/README.md` & `findpeaks-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/__init__.py` & `findpeaks-2.5.1/findpeaks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from findpeaks.filters.median import median_filter
 from findpeaks.filters.mean import mean_filter
 
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 
 # module level doc-string
 __doc__ = """
 findpeaks
 =====================================================================
 
 findpeaks is for the detection and vizualization of peaks and valleys in a 1D-vector and 2D-array.
```

### Comparing `findpeaks-2.5.0/findpeaks/examples.py` & `findpeaks-2.5.1/findpeaks/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,53 @@
 # print(findpeaks.__version__)
 
 # pip install opencv-python
 # import matplotlib.pyplot as plt
 # from findpeaks import findpeaks
 
 # %% New functionality:
-import findpeaks
+import findpeaks as fp
 import matplotlib.pyplot as plt
-img = findpeaks.import_example('2dpeaks_image')
+
+# Import example
+img = fp.import_example('2dpeaks_image')
 # Resize
-img = findpeaks.stats.resize(img, size=(300,300))
+img = fp.stats.resize(img, size=(150, 150))
 # Make grey image
-img = findpeaks.stats.togray(img)
+img = fp.stats.togray(img)
 # Scale between [0-255]
-img = findpeaks.stats.scale(img)
+img = fp.stats.scale(img)
 # Filter
-img_filtered = findpeaks.stats.lee_sigma_filter(img.copy(), win_size=7)
+img_filtered = fp.stats.lee_sigma_filter(img, win_size=17)
 
 plt.figure()
 fig, axs = plt.subplots(1,2)
 axs[0].imshow(img, cmap='gray'); axs[0].set_title('Input')
 axs[1].imshow(img_filtered, cmap='gray'); axs[1].set_title('Lee sigma filter')
 
 
-import findpeaks
-img = findpeaks.import_example('2dpeaks_image')
-
+# %%
+# Import library
 from findpeaks import findpeaks
-fp = findpeaks(method='topology', scale=True, denoise='lee_sigma', togray=True, params={'window': 31})
+
+# Set 
+fp = findpeaks(method='topology',
+               scale=True,
+               togray=True,
+               imsize=(150, 150),
+               denoise='lee_sigma',
+               params={'window': 17})
+
+# Import example image
+img = fp.import_example('2dpeaks_image')
+
 results = fp.fit(img)
-fp.plot_persistence()
-fp.plot()
+fp.plot_mesh()
+# fp.plot_persistence()
+fp.plot(limit=3)
 
 
 # %% Issue 18:
 from findpeaks import findpeaks
 
 fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, params={'window': 15})
 X = fp.import_example('2dpeaks')
```

### Comparing `findpeaks-2.5.0/findpeaks/filters/frost.py` & `findpeaks-2.5.1/findpeaks/filters/frost.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/kuan.py` & `findpeaks-2.5.1/findpeaks/filters/kuan.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/lee.py` & `findpeaks-2.5.1/findpeaks/filters/lee.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/lee_enhanced.py` & `findpeaks-2.5.1/findpeaks/filters/lee_enhanced.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/lee_sigma.py` & `findpeaks-2.5.1/findpeaks/filters/lee_sigma.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/mean.py` & `findpeaks-2.5.1/findpeaks/filters/mean.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/filters/median.py` & `findpeaks-2.5.1/findpeaks/filters/median.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/findpeaks.py` & `findpeaks-2.5.1/findpeaks/findpeaks.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         elif os.path.isfile(path):
             if verbose>=3: print('[findpeaks] >Import [%s]' %(path))
             X = cv2.imread(path)
         # Return
         return X
 
     # %% Plotting
-    def plot(self, legend=True, figsize=None, cmap=None, text=True, xlabel='x-axis', ylabel='y-axis'):
+    def plot(self, limit=None, legend=True, figsize=None, cmap=None, text=True, xlabel='x-axis', ylabel='y-axis'):
         """Plot results.
 
         Parameters
         ----------
         legend : bool, (default: True)
             Show the legend.
         figsize : (int, int), optional, default: (15, 8)
@@ -708,15 +708,15 @@
 
         figsize = figsize if figsize is not None else self.args['figsize']
 
         if self.args['type']=='peaks1d':
             fig_axis = self.plot1d(legend=legend, figsize=figsize, xlabel=xlabel, ylabel=ylabel)
         elif self.args['type']=='peaks2d':
             # fig_axis = self.plot2d(figsize=figsize)
-            fig_axis = self.plot_mask(figsize=figsize, cmap=cmap, text=text)
+            fig_axis = self.plot_mask(figsize=figsize, cmap=cmap, text=text, limit=limit)
         else:
             if self.verbose>=2: print('[findpeaks] >WARNING: Nothing to plot for %s' %(self.args['type']))
             return None
 
         # Return
         return fig_axis
 
@@ -768,15 +768,15 @@
                     min_peaks = df_interp['x'].loc[df_interp['valley']].values
                 if np.any('peak' in self.whitelist):
                     max_peaks = df_interp['x'].loc[df_interp['peak']].values
                 ax2 = _plot_original(df_interp['y'].values, df_interp['x'].values, df_interp['labx'].values, min_peaks.astype(int), max_peaks.astype(int), title=title + ' (interpolated)', figsize=figsize, legend=legend, xlabel=xlabel, ylabel=ylabel)
             # Return axis
             return (ax2, ax1)
 
-    def plot2d(self, figsize=None):
+    def plot2d(self, figsize=None, limit=None):
         """Plot the 2d results.
 
         Parameters
         ----------
         figsize : (int, int), (default: None)
             (width, height) in inches.
 
@@ -791,15 +791,15 @@
         ax_method, ax_mesh = None, None
         figsize = figsize if figsize is not None else self.args['figsize']
         # Plot preprocessing steps
         self.plot_preprocessing()
 
         # Setup figure
         if self.method=='mask':
-            ax_method = self.plot_mask(figsize=figsize)
+            ax_method = self.plot_mask(figsize=figsize, limit=limit)
         if self.method=='topology':
             # Plot topology/persistence
             ax_method = self.plot_persistence(figsize=figsize)
 
         # Plot mesh
         ax_mesh = self.plot_mesh(figsize=figsize)
```

### Comparing `findpeaks-2.5.0/findpeaks/interpolate.py` & `findpeaks-2.5.1/findpeaks/interpolate.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/stats.py` & `findpeaks-2.5.1/findpeaks/stats.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/tests/test_findpeaks.py` & `findpeaks-2.5.1/findpeaks/tests/test_findpeaks.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks/union_find.py` & `findpeaks-2.5.1/findpeaks/union_find.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/findpeaks.egg-info/PKG-INFO` & `findpeaks-2.5.1/findpeaks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.5.0
+Version: 2.5.1
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.0.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.5.0 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.5.1 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.5.0.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/findpeaks/archive/2.5.1.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
 pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
 [Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
 findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
```

### Comparing `findpeaks-2.5.0/findpeaks.egg-info/SOURCES.txt` & `findpeaks-2.5.1/findpeaks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findpeaks-2.5.0/setup.py` & `findpeaks-2.5.1/setup.py`

 * *Files identical despite different names*

