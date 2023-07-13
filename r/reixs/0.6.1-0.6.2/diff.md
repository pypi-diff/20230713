# Comparing `tmp/reixs-0.6.1.tar.gz` & `tmp/reixs-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.6.1.tar", last modified: Wed Jun 28 22:27:38 2023, max compression
+gzip compressed data, was "reixs-0.6.2.tar", last modified: Thu Jul 13 19:36:47 2023, max compression
```

## Comparing `reixs-0.6.1.tar` & `reixs-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:27:38.468990 reixs-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-28 22:27:27.000000 reixs-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-28 22:27:38.468990 reixs-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-28 22:27:27.000000 reixs-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-28 22:27:27.000000 reixs-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-28 22:27:38.468990 reixs-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:27:38.464990 reixs-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:27:38.468990 reixs-0.6.1/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    58552 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-28 22:27:27.000000 reixs-0.6.1/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:27:38.468990 reixs-0.6.1/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-28 22:27:38.000000 reixs-0.6.1/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-28 22:27:38.000000 reixs-0.6.1/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:27:38.000000 reixs-0.6.1/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-28 22:27:38.000000 reixs-0.6.1/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-28 22:27:38.000000 reixs-0.6.1/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 19:36:34.000000 reixs-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 19:36:47.434481 reixs-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-07-13 19:36:34.000000 reixs-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 19:36:34.000000 reixs-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 19:36:47.434481 reixs-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.418481 reixs-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    58598 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.6.1/LICENSE` & `reixs-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/PKG-INFO` & `reixs-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.6.1/README.md` & `reixs-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/setup.cfg` & `reixs-0.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.6.1
+version = 0.6.2
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls =
```

### Comparing `reixs-0.6.1/src/reixs/LoadData.py` & `reixs-0.6.2/src/reixs/LoadData.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         pos_y : float
         text : string
         **kwargs : dict, optional
             See bokeh manual for available options.
         """
         self.plot_labels.append([pos_x, pos_y, text, kwargs])
 
-    def plot(self, linewidth=4, title=None, xlabel=None, ylabel=None, plot_height=450, plot_width=700):
+    def plot(self, linewidth=4, title=None, xlabel=None, ylabel=None, plot_height=450, plot_width=700, y_axis_type='linear'):
         """
         Plot all data assosciated with class instance/object.
 
         Parameters
         ----------
         linewidth : int, optional
         title : string, optional
@@ -263,15 +263,15 @@
         # Get the colours for the glyphs.
         numlines = len(plot_data['scan'])
         plot_data['color'] = COLORP[0:numlines]
 
         source = ColumnDataSource(plot_data)
 
         # Set up the bokeh plot
-        p = figure(height=plot_height, width=plot_width,
+        p = figure(height=plot_height, width=plot_width,y_axis_type=y_axis_type,
                    tools="pan,wheel_zoom,box_zoom,reset,crosshair,save")
         p.multi_line(xs='x_stream', ys='y_stream', legend_group="legend",
                      line_width=linewidth, line_color='color', line_alpha=0.6,
                      hover_line_color='color', hover_line_alpha=1.0,
                      source=source)
 
         # Set up the information for hover box
```

### Comparing `reixs-0.6.1/src/reixs/ReadData.py` & `reixs-0.6.2/src/reixs/ReadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/add_subtract.py` & `reixs-0.6.2/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/beamline_info.py` & `reixs-0.6.2/src/reixs/beamline_info.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/mca.py` & `reixs-0.6.2/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/mesh.py` & `reixs-0.6.2/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/parser.py` & `reixs-0.6.2/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/rixs_readutil.py` & `reixs-0.6.2/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/rsxs_mcp.py` & `reixs-0.6.2/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/rsxs_readutil.py` & `reixs-0.6.2/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/sca.py` & `reixs-0.6.2/src/reixs/sca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/simplemath.py` & `reixs-0.6.2/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/spec_config.py` & `reixs-0.6.2/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/util.py` & `reixs-0.6.2/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs/xeol.py` & `reixs-0.6.2/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.1/src/reixs.egg-info/PKG-INFO` & `reixs-0.6.2/src/reixs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.6.1/src/reixs.egg-info/SOURCES.txt` & `reixs-0.6.2/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

