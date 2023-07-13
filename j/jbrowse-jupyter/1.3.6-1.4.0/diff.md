# Comparing `tmp/jbrowse-jupyter-1.3.6.tar.gz` & `tmp/jbrowse-jupyter-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jbrowse-jupyter-1.3.6.tar", last modified: Sat Dec  3 01:22:07 2022, max compression
+gzip compressed data, was "jbrowse-jupyter-1.4.0.tar", last modified: Thu Jul 13 15:23:54 2023, max compression
```

## Comparing `jbrowse-jupyter-1.3.6.tar` & `jbrowse-jupyter-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    25264 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    29750 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      556 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)    29750 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       82 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      100 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/
--rw-r--r--   0 runner    (1001) docker     (122)     5647 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/dev_server.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7085 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    17853 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg38.json
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg38_cgv.json
--rw-r--r--   0 runner    (1001) docker     (122)     2658 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg19_cgv.json
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg19.json
--rw-r--r--   0 runner    (1001) docker     (122)    32725 2022-12-03 01:21:27.000000 jbrowse-jupyter-1.3.6/jbrowse_jupyter/jbrowse_config.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-03 01:22:07.000000 jbrowse-jupyter-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:54.770172 jbrowse-jupyter-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-07-13 15:23:54.770172 jbrowse-jupyter-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26140 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:54.766172 jbrowse-jupyter-1.4.0/jbrowse_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:54.770172 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg19_cgv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg38.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg38_cgv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/dev_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32728 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/jbrowse_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:23:54.770172 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26865 2023-07-13 15:23:54.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 15:23:54.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:23:54.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-13 15:23:54.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 15:23:54.000000 jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:23:54.770172 jbrowse-jupyter-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-13 15:23:05.000000 jbrowse-jupyter-1.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jbrowse-jupyter-1.3.6/setup.py` & `jbrowse-jupyter-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jbrowse-jupyter",
-    version="1.3.6",
+    version="1.4.0",
     author="Teresa De Jesus Martinez",
     author_email="tere486martinez@gmail.com",
     maintainer="Teresa De Jesus Martinez; JBrowse Team",
     maintainer_email="tere486martinez@gmail.com",
     description="Jupyter Notebooks extension for showing JBrowse views",
     license="Apache-2.0",
     include_package_data=True,
```

### Comparing `jbrowse-jupyter-1.3.6/README.md` & `jbrowse-jupyter-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,79 @@
 ![Pytest and flake8](https://github.com/GMOD/jbrowse-jupyter/actions/workflows/push.yml/badge.svg)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/b74e1acfbe2a85a49462b6844297f92f2b738155?urlpath=lab%2Ftree%2Fbinder%2Fbinder.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/binder_updates?labpath=binder%2Fbinder.ipynb)
 [![Downloads](https://pepy.tech/badge/jbrowse-jupyter)](https://pepy.tech/project/jbrowse-jupyter)
 [![made-with-sphinx-doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
 
-
 # [JBrowse Jupyter](https://gmod.github.io/jbrowse-jupyter/)
 
-JBrowse Jupyter is a python package that provides a python interface to JBrowse views.
+JBrowse Jupyter is a python package that provides a python interface to JBrowse
+views.
 
-The package provides a JBrowseConfig API to enable the creation of JBrowse state configuration objects. It also provides utility functions to create and embed Dash JBrowse components in jupyter notebooks and python applications.
+The package provides a JBrowseConfig API to enable the creation of JBrowse state
+configuration objects. It also provides utility functions to create and embed
+Dash JBrowse components in jupyter notebooks and python applications.
 
 ![demo-gif](https://user-images.githubusercontent.com/45598764/144863573-2bcd982b-1d18-4dc8-aa2f-fd8adf4985a2.gif)
 
-*You can open this browser.ipynb in colab* [here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
+_You can open this browser.ipynb in colab_
+[here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
 
 > ### Dash JBrowse
-> JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse), which is a collection of Dash components for JBrowse's embeddable React components.
 >
-> We utilize the Dash JBrowse package along with the [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) or the [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view) in any jupyter notebook.
+> JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse),
+> which is a collection of Dash components for JBrowse's embeddable React
+> components.
+>
+> We utilize the Dash JBrowse package along with the
+> [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed
+> [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view)
+> or the
+> [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view)
+> in any jupyter notebook.
 >
-> To learn more about the Dash JBrowse package, including how the Dash components can be used outside of Jupyter Notebooks, see [here](https://github.com/GMOD/dash_jbrowse).
+> To learn more about the Dash JBrowse package, including how the Dash
+> components can be used outside of Jupyter Notebooks, see
+> [here](https://github.com/GMOD/dash_jbrowse).
 
 ## Demos
-* Browser notebook demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
-* SK-BR-3 demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
+
+- Browser notebook demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
+- SK-BR-3 demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
 
 ## Documentation
+
 Additional details and tutorials can be found in our Sphinx documentation page.
 https://gmod.github.io/jbrowse-jupyter/docs/html/index.html
+
 ## Installation
+
 `jbrowse-jupyter` is freely available for download on the Python Package Index
 https://pypi.org/project/jbrowse-jupyter/
 
 ```
 $ pip install jbrowse-jupyter
 ```
 
 ## Quickstart
 
-For all of the following examples, make sure that the JBrowse Jupyter package has been installed into your environment (pipenv, venv, conda, etc.).
+For all of the following examples, make sure that the JBrowse Jupyter package
+has been installed into your environment (pipenv, venv, conda, etc.).
 
 ### In a Jupyter Notebook
 
-*Launching a Linear Genome View in Jupyter Notebook*
+_Launching a Linear Genome View in Jupyter Notebook_
 ![Launching hg38 LGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook.png)
 
-*Launching a Circular Genome View in Jupyter Notebook*
+_Launching a Circular Genome View in Jupyter Notebook_
 ![Launching hg19 CGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook2.png)
-*JBrowse Linear Genome view in python Dash application*
+_JBrowse Linear Genome view in python Dash application_
+
 ```python
 from dash import html, Dash
 from jbrowse_jupyter import create, create_component
 
 app = Dash(__name__)
 
 jbrowse_conf = create("LGV", genome="hg38")
@@ -64,20 +85,21 @@
 app.layout = html.Div(
     [component],
     id='test'
 )
 
 if __name__ == "__main__":
     app.run_server(port=8081, debug=True)
-    
+
 ```
 
 ### Using jupyter-server-proxy
 
-or using the [jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
+or using the
+[jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
 and the [jupyter-dash extension](https://github.com/plotly/jupyter-dash)
 
 ```
 $ pip install jupyter-server-proxy
 $ pip install jupyter-dash
 ```
 
@@ -100,370 +122,502 @@
 
 app.layout = html.Div(
     [component],
     id='test'
 )
 
 if __name__ == "__main__":
-    # the external mode should display a url proxied by jupyter-server-proxy, 
+    # the external mode should display a url proxied by jupyter-server-proxy,
     # very handy on jupyterlab behind jupyterhub as in departmental jupyterlab instances.
-    
+
     app.run_server(mode='external', debug=True, port=8999)
 
 ```
 
 ![Dash JBrowse LGV in python app](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/python_app.png)
-You can customize the Linear Genome View by modifying the `jbrowse_conf`. The `jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set an assembly, add tracks, set custom color palettes and more.
+You can customize the Linear Genome View by modifying the `jbrowse_conf`. The
+`jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set
+an assembly, add tracks, set custom color palettes and more.
 
-Find more information about the JBrowseConfig API [here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
+Find more information about the JBrowseConfig API
+[here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
 
 ## Other Examples
 
-You can find examples in the root of this repo or in the examples folder, 
-* `browser.py` - uses the Dash library to create a python application with the Dash JBrowse LinearGenomeView component
-* `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse LinearGenomeView component in a cell
-* `examples/cgv_examples.py` - uses the Dash library to create a python application with the Dash JBrowse CircularGenomeView component
-* `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse CircularGenomeView component in a cell
-* `local_support.ipynb` - jupyter notebook with tutorial on using your local data and passing it to JBrowse views
+You can find examples in the root of this repo or in the examples folder,
+
+- `browser.py` - uses the Dash library to create a python application with the
+  Dash JBrowse LinearGenomeView component
+- `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a
+  Dash JBrowse LinearGenomeView component in a cell
+- `examples/cgv_examples.py` - uses the Dash library to create a python
+  application with the Dash JBrowse CircularGenomeView component
+- `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library
+  to embed a Dash JBrowse CircularGenomeView component in a cell
+- `local_support.ipynb` - jupyter notebook with tutorial on using your local
+  data and passing it to JBrowse views
 
 ### To run a Python Dash application
+
 ```
 $ python browser.py
 ```
+
 ### To run a jupyter notebook
 
-Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install) installed.
+Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install)
+installed.
 
 ```
 # May look different if you have classic notebooks instead of jupyterlab
 jupyter-lab build
 jupyter-lab browser.ipynb
 ```
 
 ## Usage
-The `jbrowse-jupyter` package provides several utility functions to create and launch Dash JBrowse components in python applications and jupyter notebooks.
+
+The `jbrowse-jupyter` package provides several utility functions to create and
+launch Dash JBrowse components in python applications and jupyter notebooks.
 
 ### Configuring Components
-* `create`(view_type, **kwargs)- creates a JBrowseConfig configuration object given a view_type 
-    - view_type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
-    Additional params:
-        - genome: choose from one of our default genomes {hg19 or hg38} e.g `create`('LGV', genome="hg38")
-        OR 
-        - conf: use a conf object, you can manually edit and pass json object.
-        e.g `create`('LGV', conf={"my-conf": "object"})
-        > **Note**: you can manually create a conf following the https://jbrowse.org/jb2/docs/config_guide/
-        - if no genome or conf is passed, you will create an empty JBrowseConfig for that view type.
-    *defaults* if you pass no params, an empty JBrowse config for a LGV (LinearGenomeView) will be created
-* `create_component`(conf, **kwargs) - creates and returns a Dash JBrowse component -> 'CGV' or 'LGV'. This component can be used as any Dash component in Dash applications.
-  - conf: JBrowseConfig obj 
+
+- `create`(view_type, \*\*kwargs)- creates a JBrowseConfig configuration object
+  given a view_type
+  - view*type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
+    Additional params: - genome: choose from one of our default genomes {hg19 or
+    hg38} e.g `create`('LGV', genome="hg38") OR - conf: use a conf object, you
+    can manually edit and pass json object. e.g `create`('LGV', conf={"my-conf":
+    "object"}) > **Note**: you can manually create a conf following the
+    https://jbrowse.org/jb2/docs/config_guide/ - if no genome or conf is passed,
+    you will create an empty JBrowseConfig for that view type. \_defaults* if
+    you pass no params, an empty JBrowse config for a LGV (LinearGenomeView)
+    will be created
+- `create_component`(conf, \*\*kwargs) - creates and returns a Dash JBrowse
+  component -> 'CGV' or 'LGV'. This component can be used as any Dash component
+  in Dash applications.
+  - conf: JBrowseConfig obj
   - id: id for Dash components (opyional)
-  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
-  e.g `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
-* `launch`(conf, **kwargs) - launches a LinearGenomeView Dash component in a Jupyter cell
+  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed e.g
+    `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
+- `launch`(conf, \*\*kwargs) - launches a LinearGenomeView Dash component in a
+  Jupyter cell
   - id: id for Dash components
   - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
- > **Warning**: Only use `launch` in jupyter notebooks
+    > **Warning**: Only use `launch` in jupyter notebooks
 
 ### JBrowseConfig
+
 Quick overview of the JBrowseConfig API
 
-The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more.
+The JBrowseConfig API allows us to set an assembly, add tracks, set default
+sessions, set custom color themes, and more.
 
 JBrowseConfig().
-* `set_assembly`(assembly_data, aliases, refname_aliases)
-    - Sets the assembly subconfiguration
-    - for the refname_alias subconfiguration check out the
-    JBrowse [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing) 
-* `add_df_track`(track_data, name, **kwargs)
-    - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
-    - refName and name columns must be strings, start and end must be int
-    - if the score column is present, it will create a Quantitative track else it will create a Feature track.
-    - not available for CGV
-    - params:
-        * df – pandas DataFrame with the track data.
-        * name (str) – (optional) name for the track
-        * overwrite (str) – (optional) flag wether or not to overwrite existing track.
-        * track_id (str) - (optional) trackId for the track
-
-* `add_track`(data, **kwargs)
-    - adds a track configuration given a file with track data
-    - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed, bigwig file types.
-    - assumes an index exists within the same directory of the track data if no index url path is provided. 
-    - currently supporting Wiggle, Variant, Feature and Alignments tracks
-    - params:
-        * data (str) – track path or url
-        * name (str) – (optional) name for the track
-        * index (str) – (optional) index file for the track
-        * track_type (str) – (optional) track type. If none is passed, the api will infer one based on the file type
-        * overwrite (boolean) – (optional) overwrites existing track if it exists in list of tracks (default False)
-* `delete_track`(track_id)
-    - params:
-        * track_id (str) - trackId for the track to delete
-* `set_location`(location)
-    - initial location for when the browser first loads, syntax 'refName:start-end' 
-    - e.g 'chrom1:500-1000'
-    - not available for CGV
-* `set_default_session`(tracks_ids, display_assembly=True)
-    - sets the default session given a list of track ids
-    - params:
-        * tracks_ids - list[str] list of track ids to display
-        * display_assembly (boolean) – display the assembly reference sequence track. default=True
-* `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
-    - sets the theme in the configuration given up to 4 hexadecimal colors
-* `set_env`(notebook_host, notebook_port):
-    - Changes the port and the host for creating links to files found within the file tree of jupyter.
-    - The port and host should match those configured in your jupyter config.
-* `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
-    - adds a trix text search adapter
-    - not available for CGV
-* `get_config`() - returns the configuration object
+
+- `set_assembly`(assembly_data, aliases, refname_aliases)
+  - Sets the assembly subconfiguration
+  - for the refname_alias subconfiguration check out the JBrowse
+    [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing)
+- `add_df_track`(track_data, name, \*\*kwargs)
+
+  - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
+  - refName and name columns must be strings, start and end must be int
+  - if the score column is present, it will create a Quantitative track else it
+    will create a Feature track.
+  - not available for CGV
+  - params:
+    - df – pandas DataFrame with the track data.
+    - name (str) – (optional) name for the track
+    - overwrite (str) – (optional) flag whether or not to overwrite existing
+      track.
+    - track_id (str) - (optional) trackId for the track
+
+- `add_track`(data, \*\*kwargs)
+  - adds a track configuration given a file with track data
+  - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed,
+    bigwig file types.
+  - assumes an index exists within the same directory of the track data if no
+    index url path is provided.
+  - currently supporting Wiggle, Variant, Feature and Alignments tracks
+  - params:
+    - data (str) – track path or url
+    - name (str) – (optional) name for the track
+    - index (str) – (optional) index file for the track
+    - track_type (str) – (optional) track type. If none is passed, the api will
+      infer one based on the file type
+    - overwrite (boolean) – (optional) overwrites existing track if it exists in
+      list of tracks (default False)
+- `delete_track`(track_id)
+  - params:
+    - track_id (str) - trackId for the track to delete
+- `set_location`(location)
+  - initial location for when the browser first loads, syntax
+    'refName:start-end'
+  - e.g 'chrom1:500-1000'
+  - not available for CGV
+- `set_default_session`(tracks_ids, display_assembly=True)
+  - sets the default session given a list of track ids
+  - params:
+    - tracks_ids - list[str] list of track ids to display
+    - display_assembly (boolean) – display the assembly reference sequence
+      track. default=True
+- `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
+  - sets the theme in the configuration given up to 4 hexadecimal colors
+- `set_env`(notebook_host, notebook_port):
+  - Changes the port and the host for creating links to files found within the
+    file tree of jupyter.
+  - The port and host should match those configured in your jupyter config.
+- `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
+  - adds a trix text search adapter
+  - not available for CGV
+- `get_config`() - returns the configuration object
 <!-- These configurations can be used to create [Dash JBrowse's Linear Genome View](https://github.com/GMOD/dash_jbrowse) components which can be used in any python application and or jupyter notebook. -->
 
 <!-- The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more. -->
  <!-- For full details please reference the documentation. -->
 
 ![Circular Genome View Gif](https://user-images.githubusercontent.com/45598764/152484043-aeff48b5-a1f2-44f2-b7d9-131c2afd4e1a.gif)
 
-
-
 ## Local file support
+
 We currently support two ways of passing your local data to JBrowse Views.
 
-For our **Jupyter lab and Jupyter notebook** users, you can create urls by leveraging the Jupyter server where your notebook is running or you can provide paths relative to root of the file tree. You can also provide paths relative to the root of the Jupyter file tree. Examples of these can be found below or in the
-local_support.ipynb.
+For our **Jupyter lab and Jupyter notebook** users, you can create urls by
+leveraging the Jupyter server where your notebook is running or you can provide
+paths relative to root of the file tree. You can also provide paths relative to
+the root of the Jupyter file tree. Examples of these can be found below or in
+the local_support.ipynb.
+
+For those using **colab notebooks and binder** (will also work in Jupyter) you
+can use the JBrowse dev server. An example of how to use the JBrowse dev server
+can be found below.
 
-For those using **colab notebooks and binder** (will also work in Jupyter) you can use the JBrowse dev server. An example of how to use the JBrowse dev server can be found below.
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
 
-> **Note**: These solutions are recommended for your development environments and not supported in production.
 ### Jupyter Server
 
-Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create urls or paths to pass to JBrowse Jupyter view configs. 
+Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create
+urls or paths to pass to JBrowse Jupyter view configs.
 
-Once you have the data within the file tree where the notebook is running, then you will be able to format the urls or paths to pass to the API. (Note: you will need to serve your entire project where the notebook is running.)
+Once you have the data within the file tree where the notebook is running, then
+you will be able to format the urls or paths to pass to the API. (Note: you will
+need to serve your entire project where the notebook is running.)
 
-To verify that your data is in the correct place, you can navigate to *http://your-host:your-port/tree* . Make sure that you use the same port and host that is used in your jupyter configuration. 
+To verify that your data is in the correct place, you can navigate to
+_http://your-host:your-port/tree_ . Make sure that you use the same port and
+host that is used in your jupyter configuration.
 
-e.g http://localhost:8888/tree is the url your should navigate to if you are running your jupyter notebook in localhost in port 8888
+e.g http://localhost:8888/tree is the url your should navigate to if you are
+running your jupyter notebook in localhost in port 8888
 
-If you have a different port or host, you can change the port and host used by JBrowse with the use of the set_env(notebook_host, notebook_port). 
+If you have a different port or host, you can change the port and host used by
+JBrowse with the use of the set_env(notebook_host, notebook_port).
 
-Example:
-config = create("LGV)
-config.set_env("host", 9999).
+Example: config = create("LGV) config.set_env("host", 9999).
 
 #### Using Jupyter URLS
 
-In this example, the notebook is configured to run in localhost in port 8888. It is assumed that you have Jupyter lab installed in your venv.
+In this example, the notebook is configured to run in localhost in port 8888. It
+is assumed that you have Jupyter lab installed in your venv.
+
+File tree of the project:
 
-File tree of the project: 
 ```
 - example_dir/
     - example.ipynb
     - data1.gff.gz
     - data2.gff.gz.tbi
 ```
+
 Running Jupyter
+
 ```
 (venv)$ cd example_dir
 (venv)$ jupyter lab
 ```
 
-This will be the url that you should see at the top of your browser if you opened the example.ipynb
-http://localhost:8888/lab/tree/example.ipynb
+This will be the url that you should see at the top of your browser if you
+opened the example.ipynb http://localhost:8888/lab/tree/example.ipynb
+
+Urls for file `data1.gff.gz` and `data2.gff.gz.tbi` would be in the form
+`http://localhost:8888/files/<your_file_name>`.
 
-Urls for file `data1.gff.gz` and `data2.gff.gz.tbi`
-would be in the form `http://localhost:8888/files/<your_file_name>`.
-* `http://localhost:8888/files/data1.gff.gz`
-* `http://localhost:8888/files/data2.gff.gz.tbi`
-Note that you do not need to add lab or tree to this url.
+- `http://localhost:8888/files/data1.gff.gz`
+- `http://localhost:8888/files/data2.gff.gz.tbi` Note that you do not need to
+  add lab or tree to this url.
+
+You can use these urls. For example, you could add a track with these urls like
+this:
 
-You can use these urls. For example, you could add a track with thse urls like this:
 ```python
 
 config.add_track(
     "http://localhost:8888/files/data1.gff.gz", # track data
     index="http://localhost:8888/files/data2.gff.gz.tbi", # track index
     track_id="example-track", # track id
     name="track-name" # track name
 )
 ```
 
 Resources:
-* [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
-* [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
+
+- [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
+- [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
 
 #### Using Jupyter paths
-JBrowse also supports paths to files are within the Jupyter file tree (this only works if you are running your notebook in Jupyter lab or Jupyter notebook).
 
-You can repeat the steps in the previous section to ensure that your files are in the correct place. Instead of formatting the urls yourself, you can pass paths **relative to the root of the Jupyter file tree** .
+JBrowse also supports paths to files are within the Jupyter file tree (this only
+works if you are running your notebook in Jupyter lab or Jupyter notebook).
+
+You can repeat the steps in the previous section to ensure that your files are
+in the correct place. Instead of formatting the urls yourself, you can pass
+paths **relative to the root of the Jupyter file tree** .
 
 Using the same structure of the previous example...
 
-File tree of the project: 
+File tree of the project:
+
 ```
 - example_dir/
     - example.ipynb
     - data1.gff.gz
     - data2.gff.gz.tbi
 ```
+
 Running Jupyter
+
 ```
 (venv)$ cd example_dir
 (venv)$ jupyter lab
 ```
+
 A user could then specify paths to data1 and data2 like this
+
 ```python
 
 config.add_track(
     "/data1.gff.gz", # track data
     index="/data2.gff.gz.tbi", # track index
     track_id="example-track", # track id
     name="track-name" # track name
 )
 ```
 
 ### JBrowse dev server
-We also provide a simple http server configured with CORS that will allow you to serve your local files from a specified directory within your machine.
 
-> **Note** The use of local files or the dev server provided is not recommended for production environments. 
+We also provide a simple http server configured with CORS that will allow you to
+serve your local files from a specified directory within your machine.
+
+> **Note** The use of local files or the dev server provided is not recommended
+> for production environments.
 
 You can spin the dev server in two ways.
+
 1. Git clone this repo
-2. From the root of this repository, you will be able to run the python file named `serve.py`
-```$ python serve.py```
-3. You can choose your own port, host, and directory from which to serve your files. You can also press enter to choose all the defaults. 
-  - Default PORT: 8080
-  - Default host: localhost
-  - Default directory: the current working directory -> os.getcwd() is used
-
-4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-- For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+2. From the root of this repository, you will be able to run the python file
+   named `serve.py` `$ python serve.py`
+3. You can choose your own port, host, and directory from which to serve your
+   files. You can also press enter to choose all the defaults.
+
+- Default PORT: 8080
+- Default host: localhost
+- Default directory: the current working directory -> os.getcwd() is used
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
 
 Or you can make your own python file and run it to start the server.
 
 1. create a python file named dev_server.py and add the code below
 
 ```
 import os
 from jbrowse_jupyter import serve
 
 
 if __name__ == "__main__":
     serve(os.getcwd(), port=8080, host='localhost')
 ```
-2. Run the python file
-`$ python dev_server.py`
 
-3. This will spin up a python simple http server with cors enabled. You can take a look at our implementation of our dev server here: `jbrowse_jupyter/dev_server.py`
+2. Run the python file `$ python dev_server.py`
 
-4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-- For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+3. This will spin up a python simple http server with cors enabled. You can take
+   a look at our implementation of our dev server here:
+   `jbrowse_jupyter/dev_server.py`
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
 
 ## JBrowse Jupyter vs Other tools
 
-| Features        | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv | Gosling/Gos | D3GB | PygBrowse | Mango |
-| --------------- | ----------------   | ------------------   |  ----  | ----------- | ---- | --------- | ----  |
-| Binder support            | :heavy_check_mark: | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark: | :x:  | :x: | :x: |
-| Colab  support            | :heavy_check_mark: | :heavy_check_mark:   | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-| Custom Color Theming      | :heavy_check_mark: | :x:                  | :x:                | :heavy_check_mark: | :x: | :x: | :x: |
-| Deletion of tracks        | :heavy_check_mark: | :x:                  | :heavy_check_mark: | :x: | :x: | :x: | :x: |
-| Export view as SVG        | :heavy_check_mark: &ast; | :heavy_check_mark:   | :heavy_check_mark:| :x: | :x: | :x: | :heavy_check_mark:|
-| Local file support        | :heavy_check_mark: &ast;&ast; | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark:| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
-| Supports Circular Genome View | :heavy_check_mark: | :x: | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-| Ability to enable text searching from indexed files | :heavy_check_mark: | :x: | :x: | :x: | :x: | :x: | :x: |
-| Ability to add tracks from Dataframes  | :heavy_check_mark: | :x: | :x: | :x: | :x: | :heavy_check_mark: | :x:| 
-| Zooming in on regions of interest | :heavy_check_mark: &ast; | :heavy_check_mark:  | :heavy_check_mark: &ast;| :heavy_check_mark: &ast; | :heavy_check_mark: &ast;| :x: | :heavy_check_mark: &ast; |
-
-&ast; Feature is accessible via the component's UI and not by API.
-&ast;&ast; Path support for local files is only available when running notebook in Jupyter lab and Jupyter notebook. Local file support in colab and binder is available by running the JBrowse dev server to host your data and creating urls to pass to the JBrowse view. More information available in the [local file suport section of this readme](#Local-file-support)
-
-* For more features of the JBrowse and JBrowse embedded components checkout 
-[our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
-* Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/) 
-* igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
-* ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
-* D3GB [documentation](http://d3gb.usal.es/index.html)
-* PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
-* Gosling [documentaiton](https://github.com/gosling-lang/gosling.js)
-* Gos [documentation](https://gosling-lang.github.io/gos/)
-* Mango [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
+| Features                                            | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv                | Gosling/Gos           | D3GB                  | PygBrowse          | Mango                 |
+| --------------------------------------------------- | ------------------------ | -------------------- | --------------------- | --------------------- | --------------------- | ------------------ | --------------------- |
+| Binder support                                      | :heavy_check_mark:       | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Colab support                                       | :heavy_check_mark:       | :heavy_check_mark:   | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Custom Color Theming                                | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Deletion of tracks                                  | :heavy_check_mark:       | :x:                  | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :x:                   |
+| Export view as SVG                                  | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :heavy_check_mark:    |
+| Local file support                                  | :heavy_check_mark: \*\*  | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark: | :heavy_check_mark:    |
+| Supports Circular Genome View                       | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Ability to enable text searching from indexed files | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :x:                | :x:                   |
+| Ability to add tracks from Dataframes               | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :heavy_check_mark: | :x:                   |
+| Zooming in on regions of interest                   | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark: \* | :heavy_check_mark: \* | :heavy_check_mark: \* | :x:                | :heavy_check_mark: \* |
+
+\* Feature is accessible via the component's UI and not by API. \*\* Path
+support for local files is only available when running notebook in Jupyter lab
+and Jupyter notebook. Local file support in colab and binder is available by
+running the JBrowse dev server to host your data and creating urls to pass to
+the JBrowse view. More information available in the
+[local file support section of this readme](#Local-file-support)
+
+- For more features of the JBrowse and JBrowse embedded components checkout
+  [our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
+- Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/)
+- igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
+- ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
+- D3GB [documentation](http://d3gb.usal.es/index.html)
+- PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
+- Gosling [documentation](https://github.com/gosling-lang/gosling.js)
+- Gos [documentation](https://gosling-lang.github.io/gos/)
+- Mango
+  [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
 
 ## Resources
-* [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
-* [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) - interactive genome browser
-* [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) - storybook docs of React LGV
-* [Dash Applications](https://dash.plotly.com/layout) how to get started to custumize Dash applications.
-* [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html components to build the Dash aplication layout.
-* [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable embedding Dash components in jupyter notebooks.
-* [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components for JBrowse views. (JBrowse Linear Genome View)
+
+- [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
+- [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) -
+  interactive genome browser
+- [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) -
+  storybook docs of React LGV
+- [Dash Applications](https://dash.plotly.com/layout) how to get started to
+  custumize Dash applications.
+- [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html
+  components to build the Dash application layout.
+- [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable
+  embedding Dash components in jupyter notebooks.
+- [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components
+  for JBrowse views. (JBrowse Linear Genome View)
 
 ## Contributing
 
 See our [contributing guide](./CONTRIBUTING.md).
 
 ## Academic Use
+
 This package was written with funding from the [NHGRI](https://genome.gov/) as
 part of the JBrowse project. If you use it in an academic project that you
 publish, please cite the most recent JBrowse paper, which will be linked from
 [jbrowse.org](https://jbrowse.org/).
+
 ## Contact us
 
-We **really** love talking to our users. Please reach out with any thoughts you have on what we are building!
+We **really** love talking to our users. Please reach out with any thoughts you
+have on what we are building!
 
--   Report a bug or request a feature at
-    https://github.com/GMOD/jbrowse-jupyter/issues
--   Join our developers chat at https://gitter.im/GMOD/jbrowse2
--   Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
+- Report a bug or request a feature at
+  https://github.com/GMOD/jbrowse-jupyter/issues
+- Join our developers chat at https://gitter.im/GMOD/jbrowse2
+- Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
 
 ## FAQ
-* What file types are supported?
-    - We currently support:
-        * bam
-        * big wig
-        * big bed
-        * cram
-        * fasta indexed
-        * fasta gzipped
-        * gff3 tabix
-        * two bit
-        * vcf
-        * vcf gzipped
-
-* What track types are supported?
-    - We currently support:
-        * [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
-        * [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
-        * [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
-        * [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
-        * Feature Tracks
-
-    For the circular genome view (CGV), we only support variant tracks. Check out [track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for more information.
-* What views do you currently support?
-    - We currently support JBrowse's Linear Genome View and Circular Genome View. We hope to support more in the future.
-* How do I configure text searching?
-    - In order to configure text searching in your Linear Genome View, you must first create a text index. Follow the steps found [here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching). Then you must create and add a text search adapter to your config. 
-* How do I configure tracks to show up on first render?
-    - You can set a specific track/tracks to show up when the component first renders, and you can do this via the default session. You can set the default session via the JBrowseConfig API. `set_default_session`
-* How do I set a custom color theme palette to fit with my application?
-    - You can customize the color palette of the component through the use of `set_theme` function from the JBrowseConfig API. Below is an image of an LGV with a custom color palette. 
+
+### What file types are supported?
+
+We currently support:
+
+- bam
+- bigwig
+- bigbed
+- cram
+- indexed fasta
+- bgzip indexed fasta
+- gff3 tabix
+- twobit
+- vcf
+- vcf tabix
+
+### What track types are supported?
+
+We currently support:
+
+- [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
+- [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
+- [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
+- [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
+- Feature Tracks
+
+For the circular genome view (CGV), we only support variant tracks. Check out
+[track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for
+more information.
+
+### What views do you currently support?
+
+We currently support JBrowse's Linear Genome View and Circular Genome View. We
+hope to support more in the future.
+
+### How do I configure text searching?
+
+In order to configure text searching in your Linear Genome View, you must first
+create a text index. Follow the steps found
+[here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching).
+Then you must create and add a text search adapter to your config.
+
+### How do I configure tracks to show up on first render?
+
+You can set a specific track/tracks to show up when the component first renders,
+and you can do this via the default session. You can set the default session via
+the JBrowseConfig API. `set_default_session`
+
+### How do I set a custom color theme palette to fit with my application?
+
+You can customize the color palette of the component through the use of
+`set_theme` function from the JBrowseConfig API. Below is an image of an LGV
+with a custom color palette.
 ![Custom Palette](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/custom_palette.png)
 
-* Can I use local files/my own data?
-    - Yes, there are a couple of ways in which you can configure and use your own data from your local environment in jbrowse views. 
-        1. Make use of the jupyter notebook/lab server. Intended for those running their notebooks with jupyter lab or jupyter notebook.
-        2. Launch your own http server with CORS which will enable you to use local files. You can run our serve.py to launch our dev server. 
-    (Checkout our local_support.ipynb for tutorials on how to use your own data)
-
-> **Note**: These solutions are recommended for your development environments and not supported in production.
-* I am running a colab notebook/binder notebook and wish to use my local data, how can I do this? 
-    - You can run JBrowse dev server to serve local files to use in your JBrowse views. More information on the dev server can be found in the local file support section of this readme.
-
-* My paths are not working?
-    - If you are using paths, make sure you are in a jupyter environment (Jupyter lab or jupyter notebook). Additionally, make sure that the port and host match the ones in your config. If they are different, use the set_env(notebook_host, notebook_port) to change the default port and host used by JBrowse to configure paths in jupyter.
-
-* My data says it's is loading and never loads?
-    - If your view shows that it is loading and never loads, it could be a fetch error or CORS.
-        - the JBrowse Dev Server has CORS enabled.
-    - Make sure that your alias is correctly configured. Data that never loads could also indicate that the format is correct, but will not display anything for it if the assembly does not match.
-    - Data that never loads could also indicate that the port and host do not match where your data is hosted when using paths in jupyter envs
+### Can I use local files/my own data?
+
+Yes, there are a couple of ways in which you can configure and use your own data
+from your local environment in jbrowse views. 1. Make use of the jupyter
+notebook/lab server. Intended for those running their notebooks with jupyter lab
+or jupyter notebook. 2. Launch your own http server with CORS which will enable
+you to use local files. You can run our serve.py to launch our dev server.
+(Checkout our local_support.ipynb for tutorials on how to use your own data)
+
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
+
+### I am running a colab notebook/binder notebook and wish to use my local data, how can I do this?
+
+You can run JBrowse dev server to serve local files to use in your JBrowse
+views. More information on the dev server can be found in the local file support
+section of this readme.
+
+### My paths are not working?
+
+If you are using paths, make sure you are in a jupyter environment (Jupyter lab
+or jupyter notebook). Additionally, make sure that the port and host match the
+ones in your config. If they are different, use the set_env(notebook_host,
+notebook_port) to change the default port and host used by JBrowse to configure
+paths in jupyter.
+
+### My data says it's is loading and never loads?
+
+If your view shows that it is loading and never loads, it could be a fetch error
+or CORS. - the JBrowse Dev Server has CORS enabled.
+
+- Make sure that your alias is correctly configured. Data that never loads could
+  also indicate that the format is correct, but will not display anything for it
+  if the assembly does not match.
+- Data that never loads could also indicate that the port and host do not match
+  where your data is hosted when using paths in jupyter envs
```

### Comparing `jbrowse-jupyter-1.3.6/PKG-INFO` & `jbrowse-jupyter-1.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,488 +1,642 @@
 Metadata-Version: 2.1
 Name: jbrowse-jupyter
-Version: 1.3.6
+Version: 1.4.0
 Summary: Jupyter Notebooks extension for showing JBrowse views
 Home-page: https://github.com/GMOD/jbrowse-jupyter
 Author: Teresa De Jesus Martinez
 Author-email: tere486martinez@gmail.com
 Maintainer: Teresa De Jesus Martinez; JBrowse Team
 Maintainer-email: tere486martinez@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/GMOD/jbrowse-jupyter/issues
-Description: ![Pytest and flake8](https://github.com/GMOD/jbrowse-jupyter/actions/workflows/push.yml/badge.svg)
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/b74e1acfbe2a85a49462b6844297f92f2b738155?urlpath=lab%2Ftree%2Fbinder%2Fbinder.ipynb)
-        [![Downloads](https://pepy.tech/badge/jbrowse-jupyter)](https://pepy.tech/project/jbrowse-jupyter)
-        [![made-with-sphinx-doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
-        
-        
-        # [JBrowse Jupyter](https://gmod.github.io/jbrowse-jupyter/)
-        
-        JBrowse Jupyter is a python package that provides a python interface to JBrowse views.
-        
-        The package provides a JBrowseConfig API to enable the creation of JBrowse state configuration objects. It also provides utility functions to create and embed Dash JBrowse components in jupyter notebooks and python applications.
-        
-        ![demo-gif](https://user-images.githubusercontent.com/45598764/144863573-2bcd982b-1d18-4dc8-aa2f-fd8adf4985a2.gif)
-        
-        *You can open this browser.ipynb in colab* [here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
-        
-        > ### Dash JBrowse
-        > JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse), which is a collection of Dash components for JBrowse's embeddable React components.
-        >
-        > We utilize the Dash JBrowse package along with the [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) or the [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view) in any jupyter notebook.
-        >
-        > To learn more about the Dash JBrowse package, including how the Dash components can be used outside of Jupyter Notebooks, see [here](https://github.com/GMOD/dash_jbrowse).
-        
-        ## Demos
-        * Browser notebook demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
-        * SK-BR-3 demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
-        
-        ## Documentation
-        Additional details and tutorials can be found in our Sphinx documentation page.
-        https://gmod.github.io/jbrowse-jupyter/docs/html/index.html
-        ## Installation
-        `jbrowse-jupyter` is freely available for download on the Python Package Index
-        https://pypi.org/project/jbrowse-jupyter/
-        
-        ```
-        $ pip install jbrowse-jupyter
-        ```
-        
-        ## Quickstart
-        
-        For all of the following examples, make sure that the JBrowse Jupyter package has been installed into your environment (pipenv, venv, conda, etc.).
-        
-        ### In a Jupyter Notebook
-        
-        *Launching a Linear Genome View in Jupyter Notebook*
-        ![Launching hg38 LGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook.png)
-        
-        *Launching a Circular Genome View in Jupyter Notebook*
-        ![Launching hg19 CGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook2.png)
-        *JBrowse Linear Genome view in python Dash application*
-        ```python
-        from dash import html, Dash
-        from jbrowse_jupyter import create, create_component
-        
-        app = Dash(__name__)
-        
-        jbrowse_conf = create("LGV", genome="hg38")
-        
-        config = jbrowse_conf.get_config()
-        
-        component = create_component(config)
-        
-        app.layout = html.Div(
-            [component],
-            id='test'
-        )
-        
-        if __name__ == "__main__":
-            app.run_server(port=8081, debug=True)
-            
-        ```
-        
-        ### Using jupyter-server-proxy
-        
-        or using the [jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
-        and the [jupyter-dash extension](https://github.com/plotly/jupyter-dash)
-        
-        ```
-        $ pip install jupyter-server-proxy
-        $ pip install jupyter-dash
-        ```
-        
-        ```python
-        from jupyter_dash import JupyterDash
-        
-        from dash import html
-        from jbrowse_jupyter import create, create_component
-        import jupyter_server_proxy
-        
-        JupyterDash.infer_jupyter_proxy_config()
-        #JupyterDash()._server_proxy # true if the proxy works as expected
-        #JupyterDash().config # gives the proxy config
-        
-        app = JupyterDash(__name__)
-        jbrowse_conf = create("LGV", genome="hg38")
-        
-        config = jbrowse_conf.get_config()
-        component = create_component(config)
-        
-        app.layout = html.Div(
-            [component],
-            id='test'
-        )
-        
-        if __name__ == "__main__":
-            # the external mode should display a url proxied by jupyter-server-proxy, 
-            # very handy on jupyterlab behind jupyterhub as in departmental jupyterlab instances.
-            
-            app.run_server(mode='external', debug=True, port=8999)
-        
-        ```
-        
-        ![Dash JBrowse LGV in python app](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/python_app.png)
-        You can customize the Linear Genome View by modifying the `jbrowse_conf`. The `jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set an assembly, add tracks, set custom color palettes and more.
-        
-        Find more information about the JBrowseConfig API [here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
-        
-        ## Other Examples
-        
-        You can find examples in the root of this repo or in the examples folder, 
-        * `browser.py` - uses the Dash library to create a python application with the Dash JBrowse LinearGenomeView component
-        * `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse LinearGenomeView component in a cell
-        * `examples/cgv_examples.py` - uses the Dash library to create a python application with the Dash JBrowse CircularGenomeView component
-        * `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse CircularGenomeView component in a cell
-        * `local_support.ipynb` - jupyter notebook with tutorial on using your local data and passing it to JBrowse views
-        
-        ### To run a Python Dash application
-        ```
-        $ python browser.py
-        ```
-        ### To run a jupyter notebook
-        
-        Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install) installed.
-        
-        ```
-        # May look different if you have classic notebooks instead of jupyterlab
-        jupyter-lab build
-        jupyter-lab browser.ipynb
-        ```
-        
-        ## Usage
-        The `jbrowse-jupyter` package provides several utility functions to create and launch Dash JBrowse components in python applications and jupyter notebooks.
-        
-        ### Configuring Components
-        * `create`(view_type, **kwargs)- creates a JBrowseConfig configuration object given a view_type 
-            - view_type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
-            Additional params:
-                - genome: choose from one of our default genomes {hg19 or hg38} e.g `create`('LGV', genome="hg38")
-                OR 
-                - conf: use a conf object, you can manually edit and pass json object.
-                e.g `create`('LGV', conf={"my-conf": "object"})
-                > **Note**: you can manually create a conf following the https://jbrowse.org/jb2/docs/config_guide/
-                - if no genome or conf is passed, you will create an empty JBrowseConfig for that view type.
-            *defaults* if you pass no params, an empty JBrowse config for a LGV (LinearGenomeView) will be created
-        * `create_component`(conf, **kwargs) - creates and returns a Dash JBrowse component -> 'CGV' or 'LGV'. This component can be used as any Dash component in Dash applications.
-          - conf: JBrowseConfig obj 
-          - id: id for Dash components (opyional)
-          - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
-          e.g `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
-        * `launch`(conf, **kwargs) - launches a LinearGenomeView Dash component in a Jupyter cell
-          - id: id for Dash components
-          - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
-         > **Warning**: Only use `launch` in jupyter notebooks
-        
-        ### JBrowseConfig
-        Quick overview of the JBrowseConfig API
-        
-        The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more.
-        
-        JBrowseConfig().
-        * `set_assembly`(assembly_data, aliases, refname_aliases)
-            - Sets the assembly subconfiguration
-            - for the refname_alias subconfiguration check out the
-            JBrowse [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing) 
-        * `add_df_track`(track_data, name, **kwargs)
-            - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
-            - refName and name columns must be strings, start and end must be int
-            - if the score column is present, it will create a Quantitative track else it will create a Feature track.
-            - not available for CGV
-            - params:
-                * df – pandas DataFrame with the track data.
-                * name (str) – (optional) name for the track
-                * overwrite (str) – (optional) flag wether or not to overwrite existing track.
-                * track_id (str) - (optional) trackId for the track
-        
-        * `add_track`(data, **kwargs)
-            - adds a track configuration given a file with track data
-            - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed, bigwig file types.
-            - assumes an index exists within the same directory of the track data if no index url path is provided. 
-            - currently supporting Wiggle, Variant, Feature and Alignments tracks
-            - params:
-                * data (str) – track path or url
-                * name (str) – (optional) name for the track
-                * index (str) – (optional) index file for the track
-                * track_type (str) – (optional) track type. If none is passed, the api will infer one based on the file type
-                * overwrite (boolean) – (optional) overwrites existing track if it exists in list of tracks (default False)
-        * `delete_track`(track_id)
-            - params:
-                * track_id (str) - trackId for the track to delete
-        * `set_location`(location)
-            - initial location for when the browser first loads, syntax 'refName:start-end' 
-            - e.g 'chrom1:500-1000'
-            - not available for CGV
-        * `set_default_session`(tracks_ids, display_assembly=True)
-            - sets the default session given a list of track ids
-            - params:
-                * tracks_ids - list[str] list of track ids to display
-                * display_assembly (boolean) – display the assembly reference sequence track. default=True
-        * `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
-            - sets the theme in the configuration given up to 4 hexadecimal colors
-        * `set_env`(notebook_host, notebook_port):
-            - Changes the port and the host for creating links to files found within the file tree of jupyter.
-            - The port and host should match those configured in your jupyter config.
-        * `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
-            - adds a trix text search adapter
-            - not available for CGV
-        * `get_config`() - returns the configuration object
-        <!-- These configurations can be used to create [Dash JBrowse's Linear Genome View](https://github.com/GMOD/dash_jbrowse) components which can be used in any python application and or jupyter notebook. -->
-        
-        <!-- The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more. -->
-         <!-- For full details please reference the documentation. -->
-        
-        ![Circular Genome View Gif](https://user-images.githubusercontent.com/45598764/152484043-aeff48b5-a1f2-44f2-b7d9-131c2afd4e1a.gif)
-        
-        
-        
-        ## Local file support
-        We currently support two ways of passing your local data to JBrowse Views.
-        
-        For our **Jupyter lab and Jupyter notebook** users, you can create urls by leveraging the Jupyter server where your notebook is running or you can provide paths relative to root of the file tree. You can also provide paths relative to the root of the Jupyter file tree. Examples of these can be found below or in the
-        local_support.ipynb.
-        
-        For those using **colab notebooks and binder** (will also work in Jupyter) you can use the JBrowse dev server. An example of how to use the JBrowse dev server can be found below.
-        
-        > **Note**: These solutions are recommended for your development environments and not supported in production.
-        ### Jupyter Server
-        
-        Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create urls or paths to pass to JBrowse Jupyter view configs. 
-        
-        Once you have the data within the file tree where the notebook is running, then you will be able to format the urls or paths to pass to the API. (Note: you will need to serve your entire project where the notebook is running.)
-        
-        To verify that your data is in the correct place, you can navigate to *http://your-host:your-port/tree* . Make sure that you use the same port and host that is used in your jupyter configuration. 
-        
-        e.g http://localhost:8888/tree is the url your should navigate to if you are running your jupyter notebook in localhost in port 8888
-        
-        If you have a different port or host, you can change the port and host used by JBrowse with the use of the set_env(notebook_host, notebook_port). 
-        
-        Example:
-        config = create("LGV)
-        config.set_env("host", 9999).
-        
-        #### Using Jupyter URLS
-        
-        In this example, the notebook is configured to run in localhost in port 8888. It is assumed that you have Jupyter lab installed in your venv.
-        
-        File tree of the project: 
-        ```
-        - example_dir/
-            - example.ipynb
-            - data1.gff.gz
-            - data2.gff.gz.tbi
-        ```
-        Running Jupyter
-        ```
-        (venv)$ cd example_dir
-        (venv)$ jupyter lab
-        ```
-        
-        This will be the url that you should see at the top of your browser if you opened the example.ipynb
-        http://localhost:8888/lab/tree/example.ipynb
-        
-        Urls for file `data1.gff.gz` and `data2.gff.gz.tbi`
-        would be in the form `http://localhost:8888/files/<your_file_name>`.
-        * `http://localhost:8888/files/data1.gff.gz`
-        * `http://localhost:8888/files/data2.gff.gz.tbi`
-        Note that you do not need to add lab or tree to this url.
-        
-        You can use these urls. For example, you could add a track with thse urls like this:
-        ```python
-        
-        config.add_track(
-            "http://localhost:8888/files/data1.gff.gz", # track data
-            index="http://localhost:8888/files/data2.gff.gz.tbi", # track index
-            track_id="example-track", # track id
-            name="track-name" # track name
-        )
-        ```
-        
-        Resources:
-        * [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
-        * [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
-        
-        #### Using Jupyter paths
-        JBrowse also supports paths to files are within the Jupyter file tree (this only works if you are running your notebook in Jupyter lab or Jupyter notebook).
-        
-        You can repeat the steps in the previous section to ensure that your files are in the correct place. Instead of formatting the urls yourself, you can pass paths **relative to the root of the Jupyter file tree** .
-        
-        Using the same structure of the previous example...
-        
-        File tree of the project: 
-        ```
-        - example_dir/
-            - example.ipynb
-            - data1.gff.gz
-            - data2.gff.gz.tbi
-        ```
-        Running Jupyter
-        ```
-        (venv)$ cd example_dir
-        (venv)$ jupyter lab
-        ```
-        A user could then specify paths to data1 and data2 like this
-        ```python
-        
-        config.add_track(
-            "/data1.gff.gz", # track data
-            index="/data2.gff.gz.tbi", # track index
-            track_id="example-track", # track id
-            name="track-name" # track name
-        )
-        ```
-        
-        ### JBrowse dev server
-        We also provide a simple http server configured with CORS that will allow you to serve your local files from a specified directory within your machine.
-        
-        > **Note** The use of local files or the dev server provided is not recommended for production environments. 
-        
-        You can spin the dev server in two ways.
-        1. Git clone this repo
-        2. From the root of this repository, you will be able to run the python file named `serve.py`
-        ```$ python serve.py```
-        3. You can choose your own port, host, and directory from which to serve your files. You can also press enter to choose all the defaults. 
-          - Default PORT: 8080
-          - Default host: localhost
-          - Default directory: the current working directory -> os.getcwd() is used
-        
-        4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-        - For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-        e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
-        
-        Or you can make your own python file and run it to start the server.
-        
-        1. create a python file named dev_server.py and add the code below
-        
-        ```
-        import os
-        from jbrowse_jupyter import serve
-        
-        
-        if __name__ == "__main__":
-            serve(os.getcwd(), port=8080, host='localhost')
-        ```
-        2. Run the python file
-        `$ python dev_server.py`
-        
-        3. This will spin up a python simple http server with cors enabled. You can take a look at our implementation of our dev server here: `jbrowse_jupyter/dev_server.py`
-        
-        4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-        - For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-        e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
-        
-        ## JBrowse Jupyter vs Other tools
-        
-        | Features        | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv | Gosling/Gos | D3GB | PygBrowse | Mango |
-        | --------------- | ----------------   | ------------------   |  ----  | ----------- | ---- | --------- | ----  |
-        | Binder support            | :heavy_check_mark: | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark: | :x:  | :x: | :x: |
-        | Colab  support            | :heavy_check_mark: | :heavy_check_mark:   | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-        | Custom Color Theming      | :heavy_check_mark: | :x:                  | :x:                | :heavy_check_mark: | :x: | :x: | :x: |
-        | Deletion of tracks        | :heavy_check_mark: | :x:                  | :heavy_check_mark: | :x: | :x: | :x: | :x: |
-        | Export view as SVG        | :heavy_check_mark: &ast; | :heavy_check_mark:   | :heavy_check_mark:| :x: | :x: | :x: | :heavy_check_mark:|
-        | Local file support        | :heavy_check_mark: &ast;&ast; | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark:| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
-        | Supports Circular Genome View | :heavy_check_mark: | :x: | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-        | Ability to enable text searching from indexed files | :heavy_check_mark: | :x: | :x: | :x: | :x: | :x: | :x: |
-        | Ability to add tracks from Dataframes  | :heavy_check_mark: | :x: | :x: | :x: | :x: | :heavy_check_mark: | :x:| 
-        | Zooming in on regions of interest | :heavy_check_mark: &ast; | :heavy_check_mark:  | :heavy_check_mark: &ast;| :heavy_check_mark: &ast; | :heavy_check_mark: &ast;| :x: | :heavy_check_mark: &ast; |
-        
-        &ast; Feature is accessible via the component's UI and not by API.
-        &ast;&ast; Path support for local files is only available when running notebook in Jupyter lab and Jupyter notebook. Local file support in colab and binder is available by running the JBrowse dev server to host your data and creating urls to pass to the JBrowse view. More information available in the [local file suport section of this readme](#Local-file-support)
-        
-        * For more features of the JBrowse and JBrowse embedded components checkout 
-        [our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
-        * Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/) 
-        * igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
-        * ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
-        * D3GB [documentation](http://d3gb.usal.es/index.html)
-        * PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
-        * Gosling [documentaiton](https://github.com/gosling-lang/gosling.js)
-        * Gos [documentation](https://gosling-lang.github.io/gos/)
-        * Mango [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
-        
-        ## Resources
-        * [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
-        * [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) - interactive genome browser
-        * [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) - storybook docs of React LGV
-        * [Dash Applications](https://dash.plotly.com/layout) how to get started to custumize Dash applications.
-        * [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html components to build the Dash aplication layout.
-        * [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable embedding Dash components in jupyter notebooks.
-        * [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components for JBrowse views. (JBrowse Linear Genome View)
-        
-        ## Contributing
-        
-        See our [contributing guide](./CONTRIBUTING.md).
-        
-        ## Academic Use
-        This package was written with funding from the [NHGRI](https://genome.gov/) as
-        part of the JBrowse project. If you use it in an academic project that you
-        publish, please cite the most recent JBrowse paper, which will be linked from
-        [jbrowse.org](https://jbrowse.org/).
-        ## Contact us
-        
-        We **really** love talking to our users. Please reach out with any thoughts you have on what we are building!
-        
-        -   Report a bug or request a feature at
-            https://github.com/GMOD/jbrowse-jupyter/issues
-        -   Join our developers chat at https://gitter.im/GMOD/jbrowse2
-        -   Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
-        
-        ## FAQ
-        * What file types are supported?
-            - We currently support:
-                * bam
-                * big wig
-                * big bed
-                * cram
-                * fasta indexed
-                * fasta gzipped
-                * gff3 tabix
-                * two bit
-                * vcf
-                * vcf gzipped
-        
-        * What track types are supported?
-            - We currently support:
-                * [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
-                * [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
-                * [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
-                * [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
-                * Feature Tracks
-        
-            For the circular genome view (CGV), we only support variant tracks. Check out [track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for more information.
-        * What views do you currently support?
-            - We currently support JBrowse's Linear Genome View and Circular Genome View. We hope to support more in the future.
-        * How do I configure text searching?
-            - In order to configure text searching in your Linear Genome View, you must first create a text index. Follow the steps found [here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching). Then you must create and add a text search adapter to your config. 
-        * How do I configure tracks to show up on first render?
-            - You can set a specific track/tracks to show up when the component first renders, and you can do this via the default session. You can set the default session via the JBrowseConfig API. `set_default_session`
-        * How do I set a custom color theme palette to fit with my application?
-            - You can customize the color palette of the component through the use of `set_theme` function from the JBrowseConfig API. Below is an image of an LGV with a custom color palette. 
-        ![Custom Palette](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/custom_palette.png)
-        
-        * Can I use local files/my own data?
-            - Yes, there are a couple of ways in which you can configure and use your own data from your local environment in jbrowse views. 
-                1. Make use of the jupyter notebook/lab server. Intended for those running their notebooks with jupyter lab or jupyter notebook.
-                2. Launch your own http server with CORS which will enable you to use local files. You can run our serve.py to launch our dev server. 
-            (Checkout our local_support.ipynb for tutorials on how to use your own data)
-        
-        > **Note**: These solutions are recommended for your development environments and not supported in production.
-        * I am running a colab notebook/binder notebook and wish to use my local data, how can I do this? 
-            - You can run JBrowse dev server to serve local files to use in your JBrowse views. More information on the dev server can be found in the local file support section of this readme.
-        
-        * My paths are not working?
-            - If you are using paths, make sure you are in a jupyter environment (Jupyter lab or jupyter notebook). Additionally, make sure that the port and host match the ones in your config. If they are different, use the set_env(notebook_host, notebook_port) to change the default port and host used by JBrowse to configure paths in jupyter.
-        
-        * My data says it's is loading and never loads?
-            - If your view shows that it is loading and never loads, it could be a fetch error or CORS.
-                - the JBrowse Dev Server has CORS enabled.
-            - Make sure that your alias is correctly configured. Data that never loads could also indicate that the format is correct, but will not display anything for it if the assembly does not match.
-            - Data that never loads could also indicate that the port and host do not match where your data is hosted when using paths in jupyter envs
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Pytest and flake8](https://github.com/GMOD/jbrowse-jupyter/actions/workflows/push.yml/badge.svg)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/binder_updates?labpath=binder%2Fbinder.ipynb)
+[![Downloads](https://pepy.tech/badge/jbrowse-jupyter)](https://pepy.tech/project/jbrowse-jupyter)
+[![made-with-sphinx-doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
+
+# [JBrowse Jupyter](https://gmod.github.io/jbrowse-jupyter/)
+
+JBrowse Jupyter is a python package that provides a python interface to JBrowse
+views.
+
+The package provides a JBrowseConfig API to enable the creation of JBrowse state
+configuration objects. It also provides utility functions to create and embed
+Dash JBrowse components in jupyter notebooks and python applications.
+
+![demo-gif](https://user-images.githubusercontent.com/45598764/144863573-2bcd982b-1d18-4dc8-aa2f-fd8adf4985a2.gif)
+
+_You can open this browser.ipynb in colab_
+[here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
+
+> ### Dash JBrowse
+>
+> JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse),
+> which is a collection of Dash components for JBrowse's embeddable React
+> components.
+>
+> We utilize the Dash JBrowse package along with the
+> [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed
+> [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view)
+> or the
+> [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view)
+> in any jupyter notebook.
+>
+> To learn more about the Dash JBrowse package, including how the Dash
+> components can be used outside of Jupyter Notebooks, see
+> [here](https://github.com/GMOD/dash_jbrowse).
+
+## Demos
+
+- Browser notebook demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
+- SK-BR-3 demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
+
+## Documentation
+
+Additional details and tutorials can be found in our Sphinx documentation page.
+https://gmod.github.io/jbrowse-jupyter/docs/html/index.html
+
+## Installation
+
+`jbrowse-jupyter` is freely available for download on the Python Package Index
+https://pypi.org/project/jbrowse-jupyter/
+
+```
+$ pip install jbrowse-jupyter
+```
+
+## Quickstart
+
+For all of the following examples, make sure that the JBrowse Jupyter package
+has been installed into your environment (pipenv, venv, conda, etc.).
+
+### In a Jupyter Notebook
+
+_Launching a Linear Genome View in Jupyter Notebook_
+![Launching hg38 LGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook.png)
+
+_Launching a Circular Genome View in Jupyter Notebook_
+![Launching hg19 CGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook2.png)
+_JBrowse Linear Genome view in python Dash application_
+
+```python
+from dash import html, Dash
+from jbrowse_jupyter import create, create_component
+
+app = Dash(__name__)
+
+jbrowse_conf = create("LGV", genome="hg38")
+
+config = jbrowse_conf.get_config()
+
+component = create_component(config)
+
+app.layout = html.Div(
+    [component],
+    id='test'
+)
+
+if __name__ == "__main__":
+    app.run_server(port=8081, debug=True)
+
+```
+
+### Using jupyter-server-proxy
+
+or using the
+[jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
+and the [jupyter-dash extension](https://github.com/plotly/jupyter-dash)
+
+```
+$ pip install jupyter-server-proxy
+$ pip install jupyter-dash
+```
+
+```python
+from jupyter_dash import JupyterDash
+
+from dash import html
+from jbrowse_jupyter import create, create_component
+import jupyter_server_proxy
+
+JupyterDash.infer_jupyter_proxy_config()
+#JupyterDash()._server_proxy # true if the proxy works as expected
+#JupyterDash().config # gives the proxy config
+
+app = JupyterDash(__name__)
+jbrowse_conf = create("LGV", genome="hg38")
+
+config = jbrowse_conf.get_config()
+component = create_component(config)
+
+app.layout = html.Div(
+    [component],
+    id='test'
+)
+
+if __name__ == "__main__":
+    # the external mode should display a url proxied by jupyter-server-proxy,
+    # very handy on jupyterlab behind jupyterhub as in departmental jupyterlab instances.
+
+    app.run_server(mode='external', debug=True, port=8999)
+
+```
+
+![Dash JBrowse LGV in python app](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/python_app.png)
+You can customize the Linear Genome View by modifying the `jbrowse_conf`. The
+`jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set
+an assembly, add tracks, set custom color palettes and more.
+
+Find more information about the JBrowseConfig API
+[here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
+
+## Other Examples
+
+You can find examples in the root of this repo or in the examples folder,
+
+- `browser.py` - uses the Dash library to create a python application with the
+  Dash JBrowse LinearGenomeView component
+- `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a
+  Dash JBrowse LinearGenomeView component in a cell
+- `examples/cgv_examples.py` - uses the Dash library to create a python
+  application with the Dash JBrowse CircularGenomeView component
+- `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library
+  to embed a Dash JBrowse CircularGenomeView component in a cell
+- `local_support.ipynb` - jupyter notebook with tutorial on using your local
+  data and passing it to JBrowse views
+
+### To run a Python Dash application
+
+```
+$ python browser.py
+```
+
+### To run a jupyter notebook
+
+Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install)
+installed.
+
+```
+# May look different if you have classic notebooks instead of jupyterlab
+jupyter-lab build
+jupyter-lab browser.ipynb
+```
+
+## Usage
+
+The `jbrowse-jupyter` package provides several utility functions to create and
+launch Dash JBrowse components in python applications and jupyter notebooks.
+
+### Configuring Components
+
+- `create`(view_type, \*\*kwargs)- creates a JBrowseConfig configuration object
+  given a view_type
+  - view*type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
+    Additional params: - genome: choose from one of our default genomes {hg19 or
+    hg38} e.g `create`('LGV', genome="hg38") OR - conf: use a conf object, you
+    can manually edit and pass json object. e.g `create`('LGV', conf={"my-conf":
+    "object"}) > **Note**: you can manually create a conf following the
+    https://jbrowse.org/jb2/docs/config_guide/ - if no genome or conf is passed,
+    you will create an empty JBrowseConfig for that view type. \_defaults* if
+    you pass no params, an empty JBrowse config for a LGV (LinearGenomeView)
+    will be created
+- `create_component`(conf, \*\*kwargs) - creates and returns a Dash JBrowse
+  component -> 'CGV' or 'LGV'. This component can be used as any Dash component
+  in Dash applications.
+  - conf: JBrowseConfig obj
+  - id: id for Dash components (opyional)
+  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed e.g
+    `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
+- `launch`(conf, \*\*kwargs) - launches a LinearGenomeView Dash component in a
+  Jupyter cell
+  - id: id for Dash components
+  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
+    > **Warning**: Only use `launch` in jupyter notebooks
+
+### JBrowseConfig
+
+Quick overview of the JBrowseConfig API
+
+The JBrowseConfig API allows us to set an assembly, add tracks, set default
+sessions, set custom color themes, and more.
+
+JBrowseConfig().
+
+- `set_assembly`(assembly_data, aliases, refname_aliases)
+  - Sets the assembly subconfiguration
+  - for the refname_alias subconfiguration check out the JBrowse
+    [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing)
+- `add_df_track`(track_data, name, \*\*kwargs)
+
+  - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
+  - refName and name columns must be strings, start and end must be int
+  - if the score column is present, it will create a Quantitative track else it
+    will create a Feature track.
+  - not available for CGV
+  - params:
+    - df – pandas DataFrame with the track data.
+    - name (str) – (optional) name for the track
+    - overwrite (str) – (optional) flag whether or not to overwrite existing
+      track.
+    - track_id (str) - (optional) trackId for the track
+
+- `add_track`(data, \*\*kwargs)
+  - adds a track configuration given a file with track data
+  - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed,
+    bigwig file types.
+  - assumes an index exists within the same directory of the track data if no
+    index url path is provided.
+  - currently supporting Wiggle, Variant, Feature and Alignments tracks
+  - params:
+    - data (str) – track path or url
+    - name (str) – (optional) name for the track
+    - index (str) – (optional) index file for the track
+    - track_type (str) – (optional) track type. If none is passed, the api will
+      infer one based on the file type
+    - overwrite (boolean) – (optional) overwrites existing track if it exists in
+      list of tracks (default False)
+- `delete_track`(track_id)
+  - params:
+    - track_id (str) - trackId for the track to delete
+- `set_location`(location)
+  - initial location for when the browser first loads, syntax
+    'refName:start-end'
+  - e.g 'chrom1:500-1000'
+  - not available for CGV
+- `set_default_session`(tracks_ids, display_assembly=True)
+  - sets the default session given a list of track ids
+  - params:
+    - tracks_ids - list[str] list of track ids to display
+    - display_assembly (boolean) – display the assembly reference sequence
+      track. default=True
+- `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
+  - sets the theme in the configuration given up to 4 hexadecimal colors
+- `set_env`(notebook_host, notebook_port):
+  - Changes the port and the host for creating links to files found within the
+    file tree of jupyter.
+  - The port and host should match those configured in your jupyter config.
+- `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
+  - adds a trix text search adapter
+  - not available for CGV
+- `get_config`() - returns the configuration object
+<!-- These configurations can be used to create [Dash JBrowse's Linear Genome View](https://github.com/GMOD/dash_jbrowse) components which can be used in any python application and or jupyter notebook. -->
+
+<!-- The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more. -->
+ <!-- For full details please reference the documentation. -->
+
+![Circular Genome View Gif](https://user-images.githubusercontent.com/45598764/152484043-aeff48b5-a1f2-44f2-b7d9-131c2afd4e1a.gif)
+
+## Local file support
+
+We currently support two ways of passing your local data to JBrowse Views.
+
+For our **Jupyter lab and Jupyter notebook** users, you can create urls by
+leveraging the Jupyter server where your notebook is running or you can provide
+paths relative to root of the file tree. You can also provide paths relative to
+the root of the Jupyter file tree. Examples of these can be found below or in
+the local_support.ipynb.
+
+For those using **colab notebooks and binder** (will also work in Jupyter) you
+can use the JBrowse dev server. An example of how to use the JBrowse dev server
+can be found below.
+
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
+
+### Jupyter Server
+
+Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create
+urls or paths to pass to JBrowse Jupyter view configs.
+
+Once you have the data within the file tree where the notebook is running, then
+you will be able to format the urls or paths to pass to the API. (Note: you will
+need to serve your entire project where the notebook is running.)
+
+To verify that your data is in the correct place, you can navigate to
+_http://your-host:your-port/tree_ . Make sure that you use the same port and
+host that is used in your jupyter configuration.
+
+e.g http://localhost:8888/tree is the url your should navigate to if you are
+running your jupyter notebook in localhost in port 8888
+
+If you have a different port or host, you can change the port and host used by
+JBrowse with the use of the set_env(notebook_host, notebook_port).
+
+Example: config = create("LGV) config.set_env("host", 9999).
+
+#### Using Jupyter URLS
+
+In this example, the notebook is configured to run in localhost in port 8888. It
+is assumed that you have Jupyter lab installed in your venv.
+
+File tree of the project:
+
+```
+- example_dir/
+    - example.ipynb
+    - data1.gff.gz
+    - data2.gff.gz.tbi
+```
+
+Running Jupyter
+
+```
+(venv)$ cd example_dir
+(venv)$ jupyter lab
+```
+
+This will be the url that you should see at the top of your browser if you
+opened the example.ipynb http://localhost:8888/lab/tree/example.ipynb
+
+Urls for file `data1.gff.gz` and `data2.gff.gz.tbi` would be in the form
+`http://localhost:8888/files/<your_file_name>`.
+
+- `http://localhost:8888/files/data1.gff.gz`
+- `http://localhost:8888/files/data2.gff.gz.tbi` Note that you do not need to
+  add lab or tree to this url.
+
+You can use these urls. For example, you could add a track with these urls like
+this:
+
+```python
+
+config.add_track(
+    "http://localhost:8888/files/data1.gff.gz", # track data
+    index="http://localhost:8888/files/data2.gff.gz.tbi", # track index
+    track_id="example-track", # track id
+    name="track-name" # track name
+)
+```
+
+Resources:
+
+- [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
+- [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
+
+#### Using Jupyter paths
+
+JBrowse also supports paths to files are within the Jupyter file tree (this only
+works if you are running your notebook in Jupyter lab or Jupyter notebook).
+
+You can repeat the steps in the previous section to ensure that your files are
+in the correct place. Instead of formatting the urls yourself, you can pass
+paths **relative to the root of the Jupyter file tree** .
+
+Using the same structure of the previous example...
+
+File tree of the project:
+
+```
+- example_dir/
+    - example.ipynb
+    - data1.gff.gz
+    - data2.gff.gz.tbi
+```
+
+Running Jupyter
+
+```
+(venv)$ cd example_dir
+(venv)$ jupyter lab
+```
+
+A user could then specify paths to data1 and data2 like this
+
+```python
+
+config.add_track(
+    "/data1.gff.gz", # track data
+    index="/data2.gff.gz.tbi", # track index
+    track_id="example-track", # track id
+    name="track-name" # track name
+)
+```
+
+### JBrowse dev server
+
+We also provide a simple http server configured with CORS that will allow you to
+serve your local files from a specified directory within your machine.
+
+> **Note** The use of local files or the dev server provided is not recommended
+> for production environments.
+
+You can spin the dev server in two ways.
+
+1. Git clone this repo
+2. From the root of this repository, you will be able to run the python file
+   named `serve.py` `$ python serve.py`
+3. You can choose your own port, host, and directory from which to serve your
+   files. You can also press enter to choose all the defaults.
+
+- Default PORT: 8080
+- Default host: localhost
+- Default directory: the current working directory -> os.getcwd() is used
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+
+Or you can make your own python file and run it to start the server.
+
+1. create a python file named dev_server.py and add the code below
+
+```
+import os
+from jbrowse_jupyter import serve
+
+
+if __name__ == "__main__":
+    serve(os.getcwd(), port=8080, host='localhost')
+```
+
+2. Run the python file `$ python dev_server.py`
+
+3. This will spin up a python simple http server with cors enabled. You can take
+   a look at our implementation of our dev server here:
+   `jbrowse_jupyter/dev_server.py`
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+
+## JBrowse Jupyter vs Other tools
+
+| Features                                            | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv                | Gosling/Gos           | D3GB                  | PygBrowse          | Mango                 |
+| --------------------------------------------------- | ------------------------ | -------------------- | --------------------- | --------------------- | --------------------- | ------------------ | --------------------- |
+| Binder support                                      | :heavy_check_mark:       | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Colab support                                       | :heavy_check_mark:       | :heavy_check_mark:   | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Custom Color Theming                                | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Deletion of tracks                                  | :heavy_check_mark:       | :x:                  | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :x:                   |
+| Export view as SVG                                  | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :heavy_check_mark:    |
+| Local file support                                  | :heavy_check_mark: \*\*  | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark: | :heavy_check_mark:    |
+| Supports Circular Genome View                       | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Ability to enable text searching from indexed files | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :x:                | :x:                   |
+| Ability to add tracks from Dataframes               | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :heavy_check_mark: | :x:                   |
+| Zooming in on regions of interest                   | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark: \* | :heavy_check_mark: \* | :heavy_check_mark: \* | :x:                | :heavy_check_mark: \* |
+
+\* Feature is accessible via the component's UI and not by API. \*\* Path
+support for local files is only available when running notebook in Jupyter lab
+and Jupyter notebook. Local file support in colab and binder is available by
+running the JBrowse dev server to host your data and creating urls to pass to
+the JBrowse view. More information available in the
+[local file support section of this readme](#Local-file-support)
+
+- For more features of the JBrowse and JBrowse embedded components checkout
+  [our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
+- Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/)
+- igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
+- ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
+- D3GB [documentation](http://d3gb.usal.es/index.html)
+- PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
+- Gosling [documentation](https://github.com/gosling-lang/gosling.js)
+- Gos [documentation](https://gosling-lang.github.io/gos/)
+- Mango
+  [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
+
+## Resources
+
+- [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
+- [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) -
+  interactive genome browser
+- [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) -
+  storybook docs of React LGV
+- [Dash Applications](https://dash.plotly.com/layout) how to get started to
+  custumize Dash applications.
+- [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html
+  components to build the Dash application layout.
+- [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable
+  embedding Dash components in jupyter notebooks.
+- [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components
+  for JBrowse views. (JBrowse Linear Genome View)
+
+## Contributing
+
+See our [contributing guide](./CONTRIBUTING.md).
+
+## Academic Use
+
+This package was written with funding from the [NHGRI](https://genome.gov/) as
+part of the JBrowse project. If you use it in an academic project that you
+publish, please cite the most recent JBrowse paper, which will be linked from
+[jbrowse.org](https://jbrowse.org/).
+
+## Contact us
+
+We **really** love talking to our users. Please reach out with any thoughts you
+have on what we are building!
+
+- Report a bug or request a feature at
+  https://github.com/GMOD/jbrowse-jupyter/issues
+- Join our developers chat at https://gitter.im/GMOD/jbrowse2
+- Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
+
+## FAQ
+
+### What file types are supported?
+
+We currently support:
+
+- bam
+- bigwig
+- bigbed
+- cram
+- indexed fasta
+- bgzip indexed fasta
+- gff3 tabix
+- twobit
+- vcf
+- vcf tabix
+
+### What track types are supported?
+
+We currently support:
+
+- [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
+- [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
+- [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
+- [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
+- Feature Tracks
+
+For the circular genome view (CGV), we only support variant tracks. Check out
+[track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for
+more information.
+
+### What views do you currently support?
+
+We currently support JBrowse's Linear Genome View and Circular Genome View. We
+hope to support more in the future.
+
+### How do I configure text searching?
+
+In order to configure text searching in your Linear Genome View, you must first
+create a text index. Follow the steps found
+[here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching).
+Then you must create and add a text search adapter to your config.
+
+### How do I configure tracks to show up on first render?
+
+You can set a specific track/tracks to show up when the component first renders,
+and you can do this via the default session. You can set the default session via
+the JBrowseConfig API. `set_default_session`
+
+### How do I set a custom color theme palette to fit with my application?
+
+You can customize the color palette of the component through the use of
+`set_theme` function from the JBrowseConfig API. Below is an image of an LGV
+with a custom color palette.
+![Custom Palette](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/custom_palette.png)
+
+### Can I use local files/my own data?
+
+Yes, there are a couple of ways in which you can configure and use your own data
+from your local environment in jbrowse views. 1. Make use of the jupyter
+notebook/lab server. Intended for those running their notebooks with jupyter lab
+or jupyter notebook. 2. Launch your own http server with CORS which will enable
+you to use local files. You can run our serve.py to launch our dev server.
+(Checkout our local_support.ipynb for tutorials on how to use your own data)
+
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
+
+### I am running a colab notebook/binder notebook and wish to use my local data, how can I do this?
+
+You can run JBrowse dev server to serve local files to use in your JBrowse
+views. More information on the dev server can be found in the local file support
+section of this readme.
+
+### My paths are not working?
+
+If you are using paths, make sure you are in a jupyter environment (Jupyter lab
+or jupyter notebook). Additionally, make sure that the port and host match the
+ones in your config. If they are different, use the set_env(notebook_host,
+notebook_port) to change the default port and host used by JBrowse to configure
+paths in jupyter.
+
+### My data says it's is loading and never loads?
+
+If your view shows that it is loading and never loads, it could be a fetch error
+or CORS. - the JBrowse Dev Server has CORS enabled.
+
+- Make sure that your alias is correctly configured. Data that never loads could
+  also indicate that the format is correct, but will not display anything for it
+  if the assembly does not match.
+- Data that never loads could also indicate that the port and host do not match
+  where your data is hosted when using paths in jupyter envs
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/SOURCES.txt` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter.egg-info/PKG-INFO` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,488 +1,642 @@
 Metadata-Version: 2.1
 Name: jbrowse-jupyter
-Version: 1.3.6
+Version: 1.4.0
 Summary: Jupyter Notebooks extension for showing JBrowse views
 Home-page: https://github.com/GMOD/jbrowse-jupyter
 Author: Teresa De Jesus Martinez
 Author-email: tere486martinez@gmail.com
 Maintainer: Teresa De Jesus Martinez; JBrowse Team
 Maintainer-email: tere486martinez@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/GMOD/jbrowse-jupyter/issues
-Description: ![Pytest and flake8](https://github.com/GMOD/jbrowse-jupyter/actions/workflows/push.yml/badge.svg)
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/b74e1acfbe2a85a49462b6844297f92f2b738155?urlpath=lab%2Ftree%2Fbinder%2Fbinder.ipynb)
-        [![Downloads](https://pepy.tech/badge/jbrowse-jupyter)](https://pepy.tech/project/jbrowse-jupyter)
-        [![made-with-sphinx-doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
-        
-        
-        # [JBrowse Jupyter](https://gmod.github.io/jbrowse-jupyter/)
-        
-        JBrowse Jupyter is a python package that provides a python interface to JBrowse views.
-        
-        The package provides a JBrowseConfig API to enable the creation of JBrowse state configuration objects. It also provides utility functions to create and embed Dash JBrowse components in jupyter notebooks and python applications.
-        
-        ![demo-gif](https://user-images.githubusercontent.com/45598764/144863573-2bcd982b-1d18-4dc8-aa2f-fd8adf4985a2.gif)
-        
-        *You can open this browser.ipynb in colab* [here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
-        
-        > ### Dash JBrowse
-        > JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse), which is a collection of Dash components for JBrowse's embeddable React components.
-        >
-        > We utilize the Dash JBrowse package along with the [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) or the [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view) in any jupyter notebook.
-        >
-        > To learn more about the Dash JBrowse package, including how the Dash components can be used outside of Jupyter Notebooks, see [here](https://github.com/GMOD/dash_jbrowse).
-        
-        ## Demos
-        * Browser notebook demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
-        * SK-BR-3 demo - https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
-        
-        ## Documentation
-        Additional details and tutorials can be found in our Sphinx documentation page.
-        https://gmod.github.io/jbrowse-jupyter/docs/html/index.html
-        ## Installation
-        `jbrowse-jupyter` is freely available for download on the Python Package Index
-        https://pypi.org/project/jbrowse-jupyter/
-        
-        ```
-        $ pip install jbrowse-jupyter
-        ```
-        
-        ## Quickstart
-        
-        For all of the following examples, make sure that the JBrowse Jupyter package has been installed into your environment (pipenv, venv, conda, etc.).
-        
-        ### In a Jupyter Notebook
-        
-        *Launching a Linear Genome View in Jupyter Notebook*
-        ![Launching hg38 LGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook.png)
-        
-        *Launching a Circular Genome View in Jupyter Notebook*
-        ![Launching hg19 CGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook2.png)
-        *JBrowse Linear Genome view in python Dash application*
-        ```python
-        from dash import html, Dash
-        from jbrowse_jupyter import create, create_component
-        
-        app = Dash(__name__)
-        
-        jbrowse_conf = create("LGV", genome="hg38")
-        
-        config = jbrowse_conf.get_config()
-        
-        component = create_component(config)
-        
-        app.layout = html.Div(
-            [component],
-            id='test'
-        )
-        
-        if __name__ == "__main__":
-            app.run_server(port=8081, debug=True)
-            
-        ```
-        
-        ### Using jupyter-server-proxy
-        
-        or using the [jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
-        and the [jupyter-dash extension](https://github.com/plotly/jupyter-dash)
-        
-        ```
-        $ pip install jupyter-server-proxy
-        $ pip install jupyter-dash
-        ```
-        
-        ```python
-        from jupyter_dash import JupyterDash
-        
-        from dash import html
-        from jbrowse_jupyter import create, create_component
-        import jupyter_server_proxy
-        
-        JupyterDash.infer_jupyter_proxy_config()
-        #JupyterDash()._server_proxy # true if the proxy works as expected
-        #JupyterDash().config # gives the proxy config
-        
-        app = JupyterDash(__name__)
-        jbrowse_conf = create("LGV", genome="hg38")
-        
-        config = jbrowse_conf.get_config()
-        component = create_component(config)
-        
-        app.layout = html.Div(
-            [component],
-            id='test'
-        )
-        
-        if __name__ == "__main__":
-            # the external mode should display a url proxied by jupyter-server-proxy, 
-            # very handy on jupyterlab behind jupyterhub as in departmental jupyterlab instances.
-            
-            app.run_server(mode='external', debug=True, port=8999)
-        
-        ```
-        
-        ![Dash JBrowse LGV in python app](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/python_app.png)
-        You can customize the Linear Genome View by modifying the `jbrowse_conf`. The `jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set an assembly, add tracks, set custom color palettes and more.
-        
-        Find more information about the JBrowseConfig API [here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
-        
-        ## Other Examples
-        
-        You can find examples in the root of this repo or in the examples folder, 
-        * `browser.py` - uses the Dash library to create a python application with the Dash JBrowse LinearGenomeView component
-        * `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse LinearGenomeView component in a cell
-        * `examples/cgv_examples.py` - uses the Dash library to create a python application with the Dash JBrowse CircularGenomeView component
-        * `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library to embed a Dash JBrowse CircularGenomeView component in a cell
-        * `local_support.ipynb` - jupyter notebook with tutorial on using your local data and passing it to JBrowse views
-        
-        ### To run a Python Dash application
-        ```
-        $ python browser.py
-        ```
-        ### To run a jupyter notebook
-        
-        Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install) installed.
-        
-        ```
-        # May look different if you have classic notebooks instead of jupyterlab
-        jupyter-lab build
-        jupyter-lab browser.ipynb
-        ```
-        
-        ## Usage
-        The `jbrowse-jupyter` package provides several utility functions to create and launch Dash JBrowse components in python applications and jupyter notebooks.
-        
-        ### Configuring Components
-        * `create`(view_type, **kwargs)- creates a JBrowseConfig configuration object given a view_type 
-            - view_type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
-            Additional params:
-                - genome: choose from one of our default genomes {hg19 or hg38} e.g `create`('LGV', genome="hg38")
-                OR 
-                - conf: use a conf object, you can manually edit and pass json object.
-                e.g `create`('LGV', conf={"my-conf": "object"})
-                > **Note**: you can manually create a conf following the https://jbrowse.org/jb2/docs/config_guide/
-                - if no genome or conf is passed, you will create an empty JBrowseConfig for that view type.
-            *defaults* if you pass no params, an empty JBrowse config for a LGV (LinearGenomeView) will be created
-        * `create_component`(conf, **kwargs) - creates and returns a Dash JBrowse component -> 'CGV' or 'LGV'. This component can be used as any Dash component in Dash applications.
-          - conf: JBrowseConfig obj 
-          - id: id for Dash components (opyional)
-          - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
-          e.g `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
-        * `launch`(conf, **kwargs) - launches a LinearGenomeView Dash component in a Jupyter cell
-          - id: id for Dash components
-          - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
-         > **Warning**: Only use `launch` in jupyter notebooks
-        
-        ### JBrowseConfig
-        Quick overview of the JBrowseConfig API
-        
-        The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more.
-        
-        JBrowseConfig().
-        * `set_assembly`(assembly_data, aliases, refname_aliases)
-            - Sets the assembly subconfiguration
-            - for the refname_alias subconfiguration check out the
-            JBrowse [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing) 
-        * `add_df_track`(track_data, name, **kwargs)
-            - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
-            - refName and name columns must be strings, start and end must be int
-            - if the score column is present, it will create a Quantitative track else it will create a Feature track.
-            - not available for CGV
-            - params:
-                * df – pandas DataFrame with the track data.
-                * name (str) – (optional) name for the track
-                * overwrite (str) – (optional) flag wether or not to overwrite existing track.
-                * track_id (str) - (optional) trackId for the track
-        
-        * `add_track`(data, **kwargs)
-            - adds a track configuration given a file with track data
-            - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed, bigwig file types.
-            - assumes an index exists within the same directory of the track data if no index url path is provided. 
-            - currently supporting Wiggle, Variant, Feature and Alignments tracks
-            - params:
-                * data (str) – track path or url
-                * name (str) – (optional) name for the track
-                * index (str) – (optional) index file for the track
-                * track_type (str) – (optional) track type. If none is passed, the api will infer one based on the file type
-                * overwrite (boolean) – (optional) overwrites existing track if it exists in list of tracks (default False)
-        * `delete_track`(track_id)
-            - params:
-                * track_id (str) - trackId for the track to delete
-        * `set_location`(location)
-            - initial location for when the browser first loads, syntax 'refName:start-end' 
-            - e.g 'chrom1:500-1000'
-            - not available for CGV
-        * `set_default_session`(tracks_ids, display_assembly=True)
-            - sets the default session given a list of track ids
-            - params:
-                * tracks_ids - list[str] list of track ids to display
-                * display_assembly (boolean) – display the assembly reference sequence track. default=True
-        * `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
-            - sets the theme in the configuration given up to 4 hexadecimal colors
-        * `set_env`(notebook_host, notebook_port):
-            - Changes the port and the host for creating links to files found within the file tree of jupyter.
-            - The port and host should match those configured in your jupyter config.
-        * `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
-            - adds a trix text search adapter
-            - not available for CGV
-        * `get_config`() - returns the configuration object
-        <!-- These configurations can be used to create [Dash JBrowse's Linear Genome View](https://github.com/GMOD/dash_jbrowse) components which can be used in any python application and or jupyter notebook. -->
-        
-        <!-- The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more. -->
-         <!-- For full details please reference the documentation. -->
-        
-        ![Circular Genome View Gif](https://user-images.githubusercontent.com/45598764/152484043-aeff48b5-a1f2-44f2-b7d9-131c2afd4e1a.gif)
-        
-        
-        
-        ## Local file support
-        We currently support two ways of passing your local data to JBrowse Views.
-        
-        For our **Jupyter lab and Jupyter notebook** users, you can create urls by leveraging the Jupyter server where your notebook is running or you can provide paths relative to root of the file tree. You can also provide paths relative to the root of the Jupyter file tree. Examples of these can be found below or in the
-        local_support.ipynb.
-        
-        For those using **colab notebooks and binder** (will also work in Jupyter) you can use the JBrowse dev server. An example of how to use the JBrowse dev server can be found below.
-        
-        > **Note**: These solutions are recommended for your development environments and not supported in production.
-        ### Jupyter Server
-        
-        Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create urls or paths to pass to JBrowse Jupyter view configs. 
-        
-        Once you have the data within the file tree where the notebook is running, then you will be able to format the urls or paths to pass to the API. (Note: you will need to serve your entire project where the notebook is running.)
-        
-        To verify that your data is in the correct place, you can navigate to *http://your-host:your-port/tree* . Make sure that you use the same port and host that is used in your jupyter configuration. 
-        
-        e.g http://localhost:8888/tree is the url your should navigate to if you are running your jupyter notebook in localhost in port 8888
-        
-        If you have a different port or host, you can change the port and host used by JBrowse with the use of the set_env(notebook_host, notebook_port). 
-        
-        Example:
-        config = create("LGV)
-        config.set_env("host", 9999).
-        
-        #### Using Jupyter URLS
-        
-        In this example, the notebook is configured to run in localhost in port 8888. It is assumed that you have Jupyter lab installed in your venv.
-        
-        File tree of the project: 
-        ```
-        - example_dir/
-            - example.ipynb
-            - data1.gff.gz
-            - data2.gff.gz.tbi
-        ```
-        Running Jupyter
-        ```
-        (venv)$ cd example_dir
-        (venv)$ jupyter lab
-        ```
-        
-        This will be the url that you should see at the top of your browser if you opened the example.ipynb
-        http://localhost:8888/lab/tree/example.ipynb
-        
-        Urls for file `data1.gff.gz` and `data2.gff.gz.tbi`
-        would be in the form `http://localhost:8888/files/<your_file_name>`.
-        * `http://localhost:8888/files/data1.gff.gz`
-        * `http://localhost:8888/files/data2.gff.gz.tbi`
-        Note that you do not need to add lab or tree to this url.
-        
-        You can use these urls. For example, you could add a track with thse urls like this:
-        ```python
-        
-        config.add_track(
-            "http://localhost:8888/files/data1.gff.gz", # track data
-            index="http://localhost:8888/files/data2.gff.gz.tbi", # track index
-            track_id="example-track", # track id
-            name="track-name" # track name
-        )
-        ```
-        
-        Resources:
-        * [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
-        * [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
-        
-        #### Using Jupyter paths
-        JBrowse also supports paths to files are within the Jupyter file tree (this only works if you are running your notebook in Jupyter lab or Jupyter notebook).
-        
-        You can repeat the steps in the previous section to ensure that your files are in the correct place. Instead of formatting the urls yourself, you can pass paths **relative to the root of the Jupyter file tree** .
-        
-        Using the same structure of the previous example...
-        
-        File tree of the project: 
-        ```
-        - example_dir/
-            - example.ipynb
-            - data1.gff.gz
-            - data2.gff.gz.tbi
-        ```
-        Running Jupyter
-        ```
-        (venv)$ cd example_dir
-        (venv)$ jupyter lab
-        ```
-        A user could then specify paths to data1 and data2 like this
-        ```python
-        
-        config.add_track(
-            "/data1.gff.gz", # track data
-            index="/data2.gff.gz.tbi", # track index
-            track_id="example-track", # track id
-            name="track-name" # track name
-        )
-        ```
-        
-        ### JBrowse dev server
-        We also provide a simple http server configured with CORS that will allow you to serve your local files from a specified directory within your machine.
-        
-        > **Note** The use of local files or the dev server provided is not recommended for production environments. 
-        
-        You can spin the dev server in two ways.
-        1. Git clone this repo
-        2. From the root of this repository, you will be able to run the python file named `serve.py`
-        ```$ python serve.py```
-        3. You can choose your own port, host, and directory from which to serve your files. You can also press enter to choose all the defaults. 
-          - Default PORT: 8080
-          - Default host: localhost
-          - Default directory: the current working directory -> os.getcwd() is used
-        
-        4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-        - For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-        e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
-        
-        Or you can make your own python file and run it to start the server.
-        
-        1. create a python file named dev_server.py and add the code below
-        
-        ```
-        import os
-        from jbrowse_jupyter import serve
-        
-        
-        if __name__ == "__main__":
-            serve(os.getcwd(), port=8080, host='localhost')
-        ```
-        2. Run the python file
-        `$ python dev_server.py`
-        
-        3. This will spin up a python simple http server with cors enabled. You can take a look at our implementation of our dev server here: `jbrowse_jupyter/dev_server.py`
-        
-        4. Now that the dev server is running you can use the url provided in the terminal to pass to your views. 
-        - For example: the url to the data you wish to pass to the JBrowse view config for the local dev server running on port 8080 on local host will look like this "http://localhost:8080/<your-file-name>"
-        e.g `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
-        
-        ## JBrowse Jupyter vs Other tools
-        
-        | Features        | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv | Gosling/Gos | D3GB | PygBrowse | Mango |
-        | --------------- | ----------------   | ------------------   |  ----  | ----------- | ---- | --------- | ----  |
-        | Binder support            | :heavy_check_mark: | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark: | :x:  | :x: | :x: |
-        | Colab  support            | :heavy_check_mark: | :heavy_check_mark:   | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-        | Custom Color Theming      | :heavy_check_mark: | :x:                  | :x:                | :heavy_check_mark: | :x: | :x: | :x: |
-        | Deletion of tracks        | :heavy_check_mark: | :x:                  | :heavy_check_mark: | :x: | :x: | :x: | :x: |
-        | Export view as SVG        | :heavy_check_mark: &ast; | :heavy_check_mark:   | :heavy_check_mark:| :x: | :x: | :x: | :heavy_check_mark:|
-        | Local file support        | :heavy_check_mark: &ast;&ast; | :heavy_check_mark:   | :heavy_check_mark: | :heavy_check_mark:| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
-        | Supports Circular Genome View | :heavy_check_mark: | :x: | :x: | :heavy_check_mark: | :x: | :x: | :x: |
-        | Ability to enable text searching from indexed files | :heavy_check_mark: | :x: | :x: | :x: | :x: | :x: | :x: |
-        | Ability to add tracks from Dataframes  | :heavy_check_mark: | :x: | :x: | :x: | :x: | :heavy_check_mark: | :x:| 
-        | Zooming in on regions of interest | :heavy_check_mark: &ast; | :heavy_check_mark:  | :heavy_check_mark: &ast;| :heavy_check_mark: &ast; | :heavy_check_mark: &ast;| :x: | :heavy_check_mark: &ast; |
-        
-        &ast; Feature is accessible via the component's UI and not by API.
-        &ast;&ast; Path support for local files is only available when running notebook in Jupyter lab and Jupyter notebook. Local file support in colab and binder is available by running the JBrowse dev server to host your data and creating urls to pass to the JBrowse view. More information available in the [local file suport section of this readme](#Local-file-support)
-        
-        * For more features of the JBrowse and JBrowse embedded components checkout 
-        [our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
-        * Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/) 
-        * igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
-        * ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
-        * D3GB [documentation](http://d3gb.usal.es/index.html)
-        * PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
-        * Gosling [documentaiton](https://github.com/gosling-lang/gosling.js)
-        * Gos [documentation](https://gosling-lang.github.io/gos/)
-        * Mango [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
-        
-        ## Resources
-        * [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
-        * [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) - interactive genome browser
-        * [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) - storybook docs of React LGV
-        * [Dash Applications](https://dash.plotly.com/layout) how to get started to custumize Dash applications.
-        * [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html components to build the Dash aplication layout.
-        * [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable embedding Dash components in jupyter notebooks.
-        * [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components for JBrowse views. (JBrowse Linear Genome View)
-        
-        ## Contributing
-        
-        See our [contributing guide](./CONTRIBUTING.md).
-        
-        ## Academic Use
-        This package was written with funding from the [NHGRI](https://genome.gov/) as
-        part of the JBrowse project. If you use it in an academic project that you
-        publish, please cite the most recent JBrowse paper, which will be linked from
-        [jbrowse.org](https://jbrowse.org/).
-        ## Contact us
-        
-        We **really** love talking to our users. Please reach out with any thoughts you have on what we are building!
-        
-        -   Report a bug or request a feature at
-            https://github.com/GMOD/jbrowse-jupyter/issues
-        -   Join our developers chat at https://gitter.im/GMOD/jbrowse2
-        -   Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
-        
-        ## FAQ
-        * What file types are supported?
-            - We currently support:
-                * bam
-                * big wig
-                * big bed
-                * cram
-                * fasta indexed
-                * fasta gzipped
-                * gff3 tabix
-                * two bit
-                * vcf
-                * vcf gzipped
-        
-        * What track types are supported?
-            - We currently support:
-                * [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
-                * [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
-                * [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
-                * [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
-                * Feature Tracks
-        
-            For the circular genome view (CGV), we only support variant tracks. Check out [track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for more information.
-        * What views do you currently support?
-            - We currently support JBrowse's Linear Genome View and Circular Genome View. We hope to support more in the future.
-        * How do I configure text searching?
-            - In order to configure text searching in your Linear Genome View, you must first create a text index. Follow the steps found [here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching). Then you must create and add a text search adapter to your config. 
-        * How do I configure tracks to show up on first render?
-            - You can set a specific track/tracks to show up when the component first renders, and you can do this via the default session. You can set the default session via the JBrowseConfig API. `set_default_session`
-        * How do I set a custom color theme palette to fit with my application?
-            - You can customize the color palette of the component through the use of `set_theme` function from the JBrowseConfig API. Below is an image of an LGV with a custom color palette. 
-        ![Custom Palette](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/custom_palette.png)
-        
-        * Can I use local files/my own data?
-            - Yes, there are a couple of ways in which you can configure and use your own data from your local environment in jbrowse views. 
-                1. Make use of the jupyter notebook/lab server. Intended for those running their notebooks with jupyter lab or jupyter notebook.
-                2. Launch your own http server with CORS which will enable you to use local files. You can run our serve.py to launch our dev server. 
-            (Checkout our local_support.ipynb for tutorials on how to use your own data)
-        
-        > **Note**: These solutions are recommended for your development environments and not supported in production.
-        * I am running a colab notebook/binder notebook and wish to use my local data, how can I do this? 
-            - You can run JBrowse dev server to serve local files to use in your JBrowse views. More information on the dev server can be found in the local file support section of this readme.
-        
-        * My paths are not working?
-            - If you are using paths, make sure you are in a jupyter environment (Jupyter lab or jupyter notebook). Additionally, make sure that the port and host match the ones in your config. If they are different, use the set_env(notebook_host, notebook_port) to change the default port and host used by JBrowse to configure paths in jupyter.
-        
-        * My data says it's is loading and never loads?
-            - If your view shows that it is loading and never loads, it could be a fetch error or CORS.
-                - the JBrowse Dev Server has CORS enabled.
-            - Make sure that your alias is correctly configured. Data that never loads could also indicate that the format is correct, but will not display anything for it if the assembly does not match.
-            - Data that never loads could also indicate that the port and host do not match where your data is hosted when using paths in jupyter envs
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Pytest and flake8](https://github.com/GMOD/jbrowse-jupyter/actions/workflows/push.yml/badge.svg)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GMOD/jbrowse-jupyter/binder_updates?labpath=binder%2Fbinder.ipynb)
+[![Downloads](https://pepy.tech/badge/jbrowse-jupyter)](https://pepy.tech/project/jbrowse-jupyter)
+[![made-with-sphinx-doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
+
+# [JBrowse Jupyter](https://gmod.github.io/jbrowse-jupyter/)
+
+JBrowse Jupyter is a python package that provides a python interface to JBrowse
+views.
+
+The package provides a JBrowseConfig API to enable the creation of JBrowse state
+configuration objects. It also provides utility functions to create and embed
+Dash JBrowse components in jupyter notebooks and python applications.
+
+![demo-gif](https://user-images.githubusercontent.com/45598764/144863573-2bcd982b-1d18-4dc8-aa2f-fd8adf4985a2.gif)
+
+_You can open this browser.ipynb in colab_
+[here](https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb)
+
+> ### Dash JBrowse
+>
+> JBrowse Jupyter uses [Dash JBrowse](https://github.com/GMOD/dash_jbrowse),
+> which is a collection of Dash components for JBrowse's embeddable React
+> components.
+>
+> We utilize the Dash JBrowse package along with the
+> [jupyter-dash](https://github.com/plotly/jupyter-dash) library to embed
+> [JBrowse React Linear Genome view](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view)
+> or the
+> [JBrowse React Circular Genome view](https://www.npmjs.com/package/@jbrowse/react-circular-genome-view)
+> in any jupyter notebook.
+>
+> To learn more about the Dash JBrowse package, including how the Dash
+> components can be used outside of Jupyter Notebooks, see
+> [here](https://github.com/GMOD/dash_jbrowse).
+
+## Demos
+
+- Browser notebook demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/browser.ipynb
+- SK-BR-3 demo -
+  https://colab.research.google.com/github/GMOD/jbrowse-jupyter/blob/main/skbr3.ipynb
+
+## Documentation
+
+Additional details and tutorials can be found in our Sphinx documentation page.
+https://gmod.github.io/jbrowse-jupyter/docs/html/index.html
+
+## Installation
+
+`jbrowse-jupyter` is freely available for download on the Python Package Index
+https://pypi.org/project/jbrowse-jupyter/
+
+```
+$ pip install jbrowse-jupyter
+```
+
+## Quickstart
+
+For all of the following examples, make sure that the JBrowse Jupyter package
+has been installed into your environment (pipenv, venv, conda, etc.).
+
+### In a Jupyter Notebook
+
+_Launching a Linear Genome View in Jupyter Notebook_
+![Launching hg38 LGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook.png)
+
+_Launching a Circular Genome View in Jupyter Notebook_
+![Launching hg19 CGV in python notebook](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/notebook2.png)
+_JBrowse Linear Genome view in python Dash application_
+
+```python
+from dash import html, Dash
+from jbrowse_jupyter import create, create_component
+
+app = Dash(__name__)
+
+jbrowse_conf = create("LGV", genome="hg38")
+
+config = jbrowse_conf.get_config()
+
+component = create_component(config)
+
+app.layout = html.Div(
+    [component],
+    id='test'
+)
+
+if __name__ == "__main__":
+    app.run_server(port=8081, debug=True)
+
+```
+
+### Using jupyter-server-proxy
+
+or using the
+[jupyter-server-proxy extension](https://github.com/jupyterhub/jupyter-server-proxy)
+and the [jupyter-dash extension](https://github.com/plotly/jupyter-dash)
+
+```
+$ pip install jupyter-server-proxy
+$ pip install jupyter-dash
+```
+
+```python
+from jupyter_dash import JupyterDash
+
+from dash import html
+from jbrowse_jupyter import create, create_component
+import jupyter_server_proxy
+
+JupyterDash.infer_jupyter_proxy_config()
+#JupyterDash()._server_proxy # true if the proxy works as expected
+#JupyterDash().config # gives the proxy config
+
+app = JupyterDash(__name__)
+jbrowse_conf = create("LGV", genome="hg38")
+
+config = jbrowse_conf.get_config()
+component = create_component(config)
+
+app.layout = html.Div(
+    [component],
+    id='test'
+)
+
+if __name__ == "__main__":
+    # the external mode should display a url proxied by jupyter-server-proxy,
+    # very handy on jupyterlab behind jupyterhub as in departmental jupyterlab instances.
+
+    app.run_server(mode='external', debug=True, port=8999)
+
+```
+
+![Dash JBrowse LGV in python app](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/python_app.png)
+You can customize the Linear Genome View by modifying the `jbrowse_conf`. The
+`jbrowse_conf` is an instance of our `JBrowseConfig`, and can be modified to set
+an assembly, add tracks, set custom color palettes and more.
+
+Find more information about the JBrowseConfig API
+[here](https://gmod.github.io/jbrowse-jupyter/docs/html/index.html)
+
+## Other Examples
+
+You can find examples in the root of this repo or in the examples folder,
+
+- `browser.py` - uses the Dash library to create a python application with the
+  Dash JBrowse LinearGenomeView component
+- `browser.ipynb` - jupyter notebook using the JupyterDash library to embed a
+  Dash JBrowse LinearGenomeView component in a cell
+- `examples/cgv_examples.py` - uses the Dash library to create a python
+  application with the Dash JBrowse CircularGenomeView component
+- `examples/cgv_examples.ipynb` - jupyter notebook using the JupyterDash library
+  to embed a Dash JBrowse CircularGenomeView component in a cell
+- `local_support.ipynb` - jupyter notebook with tutorial on using your local
+  data and passing it to JBrowse views
+
+### To run a Python Dash application
+
+```
+$ python browser.py
+```
+
+### To run a jupyter notebook
+
+Make sure you have [jupyter notebook or jupyterlab](https://jupyter.org/install)
+installed.
+
+```
+# May look different if you have classic notebooks instead of jupyterlab
+jupyter-lab build
+jupyter-lab browser.ipynb
+```
+
+## Usage
+
+The `jbrowse-jupyter` package provides several utility functions to create and
+launch Dash JBrowse components in python applications and jupyter notebooks.
+
+### Configuring Components
+
+- `create`(view_type, \*\*kwargs)- creates a JBrowseConfig configuration object
+  given a view_type
+  - view*type: Choose from a LGV or CGV e.g `create`('LGV') or `create`('CGV')
+    Additional params: - genome: choose from one of our default genomes {hg19 or
+    hg38} e.g `create`('LGV', genome="hg38") OR - conf: use a conf object, you
+    can manually edit and pass json object. e.g `create`('LGV', conf={"my-conf":
+    "object"}) > **Note**: you can manually create a conf following the
+    https://jbrowse.org/jb2/docs/config_guide/ - if no genome or conf is passed,
+    you will create an empty JBrowseConfig for that view type. \_defaults* if
+    you pass no params, an empty JBrowse config for a LGV (LinearGenomeView)
+    will be created
+- `create_component`(conf, \*\*kwargs) - creates and returns a Dash JBrowse
+  component -> 'CGV' or 'LGV'. This component can be used as any Dash component
+  in Dash applications.
+  - conf: JBrowseConfig obj
+  - id: id for Dash components (opyional)
+  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed e.g
+    `create_component`(cgv_with_conf.get_config(), dash_comp="CGV")
+- `launch`(conf, \*\*kwargs) - launches a LinearGenomeView Dash component in a
+  Jupyter cell
+  - id: id for Dash components
+  - dash_comp: 'CGV' or 'LGV', defaults to 'LGV' when none is passed
+    > **Warning**: Only use `launch` in jupyter notebooks
+
+### JBrowseConfig
+
+Quick overview of the JBrowseConfig API
+
+The JBrowseConfig API allows us to set an assembly, add tracks, set default
+sessions, set custom color themes, and more.
+
+JBrowseConfig().
+
+- `set_assembly`(assembly_data, aliases, refname_aliases)
+  - Sets the assembly subconfiguration
+  - for the refname_alias subconfiguration check out the JBrowse
+    [refname aliasing docs](https://jbrowse.org/jb2/docs/config_guide/#configuring-reference-name-aliasing)
+- `add_df_track`(track_data, name, \*\*kwargs)
+
+  - requires DataFrame to have columns ['refName', 'start', 'end', 'name']
+  - refName and name columns must be strings, start and end must be int
+  - if the score column is present, it will create a Quantitative track else it
+    will create a Feature track.
+  - not available for CGV
+  - params:
+    - df – pandas DataFrame with the track data.
+    - name (str) – (optional) name for the track
+    - overwrite (str) – (optional) flag whether or not to overwrite existing
+      track.
+    - track_id (str) - (optional) trackId for the track
+
+- `add_track`(data, \*\*kwargs)
+  - adds a track configuration given a file with track data
+  - currently supporting cram, bam, vcf gzipped, gff/gff3 gzipped, bigbed,
+    bigwig file types.
+  - assumes an index exists within the same directory of the track data if no
+    index url path is provided.
+  - currently supporting Wiggle, Variant, Feature and Alignments tracks
+  - params:
+    - data (str) – track path or url
+    - name (str) – (optional) name for the track
+    - index (str) – (optional) index file for the track
+    - track_type (str) – (optional) track type. If none is passed, the api will
+      infer one based on the file type
+    - overwrite (boolean) – (optional) overwrites existing track if it exists in
+      list of tracks (default False)
+- `delete_track`(track_id)
+  - params:
+    - track_id (str) - trackId for the track to delete
+- `set_location`(location)
+  - initial location for when the browser first loads, syntax
+    'refName:start-end'
+  - e.g 'chrom1:500-1000'
+  - not available for CGV
+- `set_default_session`(tracks_ids, display_assembly=True)
+  - sets the default session given a list of track ids
+  - params:
+    - tracks_ids - list[str] list of track ids to display
+    - display_assembly (boolean) – display the assembly reference sequence
+      track. default=True
+- `set_theme`(primary, secondary=None, tertiary=None, quaternary=None)
+  - sets the theme in the configuration given up to 4 hexadecimal colors
+- `set_env`(notebook_host, notebook_port):
+  - Changes the port and the host for creating links to files found within the
+    file tree of jupyter.
+  - The port and host should match those configured in your jupyter config.
+- `add_text_search_adapter`(ix, ixx, meta, adapter_id=None)
+  - adds a trix text search adapter
+  - not available for CGV
+- `get_config`() - returns the configuration object
+<!-- These configurations can be used to create [Dash JBrowse's Linear Genome View](https://github.com/GMOD/dash_jbrowse) components which can be used in any python application and or jupyter notebook. -->
+
+<!-- The JBrowseConfig API allows us to set an assembly, add tracks, set default sessions, set custom color themes, and more. -->
+ <!-- For full details please reference the documentation. -->
+
+![Circular Genome View Gif](https://user-images.githubusercontent.com/45598764/152484043-aeff48b5-a1f2-44f2-b7d9-131c2afd4e1a.gif)
+
+## Local file support
+
+We currently support two ways of passing your local data to JBrowse Views.
+
+For our **Jupyter lab and Jupyter notebook** users, you can create urls by
+leveraging the Jupyter server where your notebook is running or you can provide
+paths relative to root of the file tree. You can also provide paths relative to
+the root of the Jupyter file tree. Examples of these can be found below or in
+the local_support.ipynb.
+
+For those using **colab notebooks and binder** (will also work in Jupyter) you
+can use the JBrowse dev server. An example of how to use the JBrowse dev server
+can be found below.
+
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
+
+### Jupyter Server
+
+Jupyter Lab and Jupyter Notebook users can leverage the Jupyter server to create
+urls or paths to pass to JBrowse Jupyter view configs.
+
+Once you have the data within the file tree where the notebook is running, then
+you will be able to format the urls or paths to pass to the API. (Note: you will
+need to serve your entire project where the notebook is running.)
+
+To verify that your data is in the correct place, you can navigate to
+_http://your-host:your-port/tree_ . Make sure that you use the same port and
+host that is used in your jupyter configuration.
+
+e.g http://localhost:8888/tree is the url your should navigate to if you are
+running your jupyter notebook in localhost in port 8888
+
+If you have a different port or host, you can change the port and host used by
+JBrowse with the use of the set_env(notebook_host, notebook_port).
+
+Example: config = create("LGV) config.set_env("host", 9999).
+
+#### Using Jupyter URLS
+
+In this example, the notebook is configured to run in localhost in port 8888. It
+is assumed that you have Jupyter lab installed in your venv.
+
+File tree of the project:
+
+```
+- example_dir/
+    - example.ipynb
+    - data1.gff.gz
+    - data2.gff.gz.tbi
+```
+
+Running Jupyter
+
+```
+(venv)$ cd example_dir
+(venv)$ jupyter lab
+```
+
+This will be the url that you should see at the top of your browser if you
+opened the example.ipynb http://localhost:8888/lab/tree/example.ipynb
+
+Urls for file `data1.gff.gz` and `data2.gff.gz.tbi` would be in the form
+`http://localhost:8888/files/<your_file_name>`.
+
+- `http://localhost:8888/files/data1.gff.gz`
+- `http://localhost:8888/files/data2.gff.gz.tbi` Note that you do not need to
+  add lab or tree to this url.
+
+You can use these urls. For example, you could add a track with these urls like
+this:
+
+```python
+
+config.add_track(
+    "http://localhost:8888/files/data1.gff.gz", # track data
+    index="http://localhost:8888/files/data2.gff.gz.tbi", # track index
+    track_id="example-track", # track id
+    name="track-name" # track name
+)
+```
+
+Resources:
+
+- [Configuring the Jupyter Notebook server](https://jupyter-notebook.readthedocs.io/en/stable/config_overview.html#notebook-server)
+- [Getting started with Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html)
+
+#### Using Jupyter paths
+
+JBrowse also supports paths to files are within the Jupyter file tree (this only
+works if you are running your notebook in Jupyter lab or Jupyter notebook).
+
+You can repeat the steps in the previous section to ensure that your files are
+in the correct place. Instead of formatting the urls yourself, you can pass
+paths **relative to the root of the Jupyter file tree** .
+
+Using the same structure of the previous example...
+
+File tree of the project:
+
+```
+- example_dir/
+    - example.ipynb
+    - data1.gff.gz
+    - data2.gff.gz.tbi
+```
+
+Running Jupyter
+
+```
+(venv)$ cd example_dir
+(venv)$ jupyter lab
+```
+
+A user could then specify paths to data1 and data2 like this
+
+```python
+
+config.add_track(
+    "/data1.gff.gz", # track data
+    index="/data2.gff.gz.tbi", # track index
+    track_id="example-track", # track id
+    name="track-name" # track name
+)
+```
+
+### JBrowse dev server
+
+We also provide a simple http server configured with CORS that will allow you to
+serve your local files from a specified directory within your machine.
+
+> **Note** The use of local files or the dev server provided is not recommended
+> for production environments.
+
+You can spin the dev server in two ways.
+
+1. Git clone this repo
+2. From the root of this repository, you will be able to run the python file
+   named `serve.py` `$ python serve.py`
+3. You can choose your own port, host, and directory from which to serve your
+   files. You can also press enter to choose all the defaults.
+
+- Default PORT: 8080
+- Default host: localhost
+- Default directory: the current working directory -> os.getcwd() is used
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+
+Or you can make your own python file and run it to start the server.
+
+1. create a python file named dev_server.py and add the code below
+
+```
+import os
+from jbrowse_jupyter import serve
+
+
+if __name__ == "__main__":
+    serve(os.getcwd(), port=8080, host='localhost')
+```
+
+2. Run the python file `$ python dev_server.py`
+
+3. This will spin up a python simple http server with cors enabled. You can take
+   a look at our implementation of our dev server here:
+   `jbrowse_jupyter/dev_server.py`
+
+4. Now that the dev server is running you can use the url provided in the
+   terminal to pass to your views.
+
+- For example: the url to the data you wish to pass to the JBrowse view config
+  for the local dev server running on port 8080 on local host will look like
+  this "http://localhost:8080/<your-file-name>" e.g
+  `jbrowse_conf.add_track("http://localhost:8080/<your-file-name>", name="test-demo")`
+
+## JBrowse Jupyter vs Other tools
+
+| Features                                            | JBrowse/ JBrowse Jupyter | IGV.js /igv-notebook | ipyIgv                | Gosling/Gos           | D3GB                  | PygBrowse          | Mango                 |
+| --------------------------------------------------- | ------------------------ | -------------------- | --------------------- | --------------------- | --------------------- | ------------------ | --------------------- |
+| Binder support                                      | :heavy_check_mark:       | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Colab support                                       | :heavy_check_mark:       | :heavy_check_mark:   | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Custom Color Theming                                | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Deletion of tracks                                  | :heavy_check_mark:       | :x:                  | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :x:                   |
+| Export view as SVG                                  | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark:    | :x:                   | :x:                   | :x:                | :heavy_check_mark:    |
+| Local file support                                  | :heavy_check_mark: \*\*  | :heavy_check_mark:   | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark:    | :heavy_check_mark: | :heavy_check_mark:    |
+| Supports Circular Genome View                       | :heavy_check_mark:       | :x:                  | :x:                   | :heavy_check_mark:    | :x:                   | :x:                | :x:                   |
+| Ability to enable text searching from indexed files | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :x:                | :x:                   |
+| Ability to add tracks from Dataframes               | :heavy_check_mark:       | :x:                  | :x:                   | :x:                   | :x:                   | :heavy_check_mark: | :x:                   |
+| Zooming in on regions of interest                   | :heavy_check_mark: \*    | :heavy_check_mark:   | :heavy_check_mark: \* | :heavy_check_mark: \* | :heavy_check_mark: \* | :x:                | :heavy_check_mark: \* |
+
+\* Feature is accessible via the component's UI and not by API. \*\* Path
+support for local files is only available when running notebook in Jupyter lab
+and Jupyter notebook. Local file support in colab and binder is available by
+running the JBrowse dev server to host your data and creating urls to pass to
+the JBrowse view. More information available in the
+[local file support section of this readme](#Local-file-support)
+
+- For more features of the JBrowse and JBrowse embedded components checkout
+  [our documentation](https://jbrowse.org/jb2/docs/embedded_components/)
+- Igv.js [documentation](https://github.com/igvteam/igv.js/wiki/)
+- igv-notebook [documentation](https://github.com/igvteam/igv-notebook)
+- ipyIgv [documentation](https://github.com/QuantStack/ipyigv)
+- D3GB [documentation](http://d3gb.usal.es/index.html)
+- PygBrowse [documentation](https://github.com/phageghost/python-genome-browser)
+- Gosling [documentation](https://github.com/gosling-lang/gosling.js)
+- Gos [documentation](https://gosling-lang.github.io/gos/)
+- Mango
+  [documentation](https://bdg-mango.readthedocs.io/en/latest/jupyterWidgets/usage.html)
+
+## Resources
+
+- [JBrowse](https://jbrowse.org/jb2/) - the next generation genome browser
+- [JBrowse React Linear Genome View](https://www.npmjs.com/package/@jbrowse/react-linear-genome-view) -
+  interactive genome browser
+- [JBrowse React Linear Genome View Docs](https://jbrowse.org/storybook/lgv/main/?path=/story/getting-started--page) -
+  storybook docs of React LGV
+- [Dash Applications](https://dash.plotly.com/layout) how to get started to
+  custumize Dash applications.
+- [Dash HTML components](https://dash.plotly.com/dash-html-components) Dash html
+  components to build the Dash application layout.
+- [Dash Jupyter](https://github.com/plotly/jupyter-dash) library to enable
+  embedding Dash components in jupyter notebooks.
+- [Dash Jbrowse](https://github.com/GMOD/dash_jbrowse) suite of Dash components
+  for JBrowse views. (JBrowse Linear Genome View)
+
+## Contributing
+
+See our [contributing guide](./CONTRIBUTING.md).
+
+## Academic Use
+
+This package was written with funding from the [NHGRI](https://genome.gov/) as
+part of the JBrowse project. If you use it in an academic project that you
+publish, please cite the most recent JBrowse paper, which will be linked from
+[jbrowse.org](https://jbrowse.org/).
+
+## Contact us
+
+We **really** love talking to our users. Please reach out with any thoughts you
+have on what we are building!
+
+- Report a bug or request a feature at
+  https://github.com/GMOD/jbrowse-jupyter/issues
+- Join our developers chat at https://gitter.im/GMOD/jbrowse2
+- Send an email to our mailing list at `gmod-ajax@lists.sourceforge.net`
+
+## FAQ
+
+### What file types are supported?
+
+We currently support:
+
+- bam
+- bigwig
+- bigbed
+- cram
+- indexed fasta
+- bgzip indexed fasta
+- gff3 tabix
+- twobit
+- vcf
+- vcf tabix
+
+### What track types are supported?
+
+We currently support:
+
+- [AlignmentsTrack](https://jbrowse.org/jb2/docs/user_guide/#alignments-tracks)
+- [QuantitativeTrack](https://jbrowse.org/jb2/docs/user_guide/#bigwig-tracks)
+- [VariantTrack](https://jbrowse.org/jb2/docs/user_guide/#variant-tracks)
+- [ReferenceSequenceTrack](https://jbrowse.org/jb2/docs/user_guide/#sequence-track)
+- Feature Tracks
+
+For the circular genome view (CGV), we only support variant tracks. Check out
+[track types](https://jbrowse.org/jb2/docs/user_guide/#sequence-track) docs for
+more information.
+
+### What views do you currently support?
+
+We currently support JBrowse's Linear Genome View and Circular Genome View. We
+hope to support more in the future.
+
+### How do I configure text searching?
+
+In order to configure text searching in your Linear Genome View, you must first
+create a text index. Follow the steps found
+[here](https://jbrowse.org/jb2/docs/quickstart_cli/#indexing-feature-names-for-searching).
+Then you must create and add a text search adapter to your config.
+
+### How do I configure tracks to show up on first render?
+
+You can set a specific track/tracks to show up when the component first renders,
+and you can do this via the default session. You can set the default session via
+the JBrowseConfig API. `set_default_session`
+
+### How do I set a custom color theme palette to fit with my application?
+
+You can customize the color palette of the component through the use of
+`set_theme` function from the JBrowseConfig API. Below is an image of an LGV
+with a custom color palette.
+![Custom Palette](https://github.com/GMOD/jbrowse-jupyter/raw/main/images/custom_palette.png)
+
+### Can I use local files/my own data?
+
+Yes, there are a couple of ways in which you can configure and use your own data
+from your local environment in jbrowse views. 1. Make use of the jupyter
+notebook/lab server. Intended for those running their notebooks with jupyter lab
+or jupyter notebook. 2. Launch your own http server with CORS which will enable
+you to use local files. You can run our serve.py to launch our dev server.
+(Checkout our local_support.ipynb for tutorials on how to use your own data)
+
+> **Note**: These solutions are recommended for your development environments
+> and not supported in production.
+
+### I am running a colab notebook/binder notebook and wish to use my local data, how can I do this?
+
+You can run JBrowse dev server to serve local files to use in your JBrowse
+views. More information on the dev server can be found in the local file support
+section of this readme.
+
+### My paths are not working?
+
+If you are using paths, make sure you are in a jupyter environment (Jupyter lab
+or jupyter notebook). Additionally, make sure that the port and host match the
+ones in your config. If they are different, use the set_env(notebook_host,
+notebook_port) to change the default port and host used by JBrowse to configure
+paths in jupyter.
+
+### My data says it's is loading and never loads?
+
+If your view shows that it is loading and never loads, it could be a fetch error
+or CORS. - the JBrowse Dev Server has CORS enabled.
+
+- Make sure that your alias is correctly configured. Data that never loads could
+  also indicate that the format is correct, but will not display anything for it
+  if the assembly does not match.
+- Data that never loads could also indicate that the port and host do not match
+  where your data is hosted when using paths in jupyter envs
```

### Comparing `jbrowse-jupyter-1.3.6/LICENSE` & `jbrowse-jupyter-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/dev_server.py` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/dev_server.py`

 * *Files identical despite different names*

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/util.py` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dash import html
 from urllib.parse import urlparse
 from jupyter_dash import JupyterDash
 
 
 def is_url(filePath):
     """
-    Checks wether or not the file path
+    Checks whether or not the file path
     is a valid url.
     :param str filePath: file path/url
     :return: returns true if path matches pattern starting with
     http:// or https://
     :rtype: boolean
     """
     regex = re.compile(r'^https?:\/\/', re.IGNORECASE)
@@ -54,15 +54,15 @@
 
 def get_name_regex(assembly_file):
     """ Returns the name of the assembly based on the assembly data file"""
     return re.search(r'(\w+)\.(?:fa|fasta|fa\.gz)$', assembly_file).group(1)
 
 
 def get_default(name, view_type="LGV"):
-    """Returns the configuration oject given a genome name."""
+    """Returns the configuration object given a genome name."""
     base = pkg_resources.resource_filename("jbrowse_jupyter", "data")
     file_name = f'{base}/{name}.json'
     if view_type == "CGV":
         file_name = f'{base}/{name}_cgv.json'
     conf = {}
     with open(file_name) as json_data:
         conf = json.load(json_data)
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/tracks.py` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/tracks.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     notebook_port = kwargs.get('nb_port', "localhost")
     if in_colab:
         return location
     return f'http://{notebook_host}:{notebook_port}/files' + location
 
 
 def supported_track_type(track_type):
-    """Checks wether or not the given track type is supported."""
+    """Checks whether or not the given track type is supported."""
     return track_type in {
         "AlignmentsTrack",
         "QuantitativeTrack",
         "VariantTrack",
         "FeatureTrack",
     }
 
@@ -424,15 +424,15 @@
     if not (correct_numbers and correct_string):
         col_err = "One or more columns do not have the correct data type."
         raise TypeError(col_err)
 
 
 def check_columns(df):
     """
-    Checks wether dataframe contains the required columns.
+    Checks whether dataframe contains the required columns.
 
     :param df: the data frame with track data.
     :return: whether or not df contains all the required columns.
             required columns: refName, start, end, name, score (is optional)
     :rtype: boolean
     """
     required = ["refName", "start", "end", "name"]
@@ -460,15 +460,15 @@
 
 def get_track_data(df):
     """
     Retrieves the features from the data frame.
 
     :param df: the data frame with track data.
     :return: features
-    :rtype: ist[obj]
+    :rtype: list[obj]
     """
     required = ["refName", "start", "end", "name", "additional", "type"]
     df["type"] = ""
     df["additional"] = ""
     if "score" in df:
         required.append("score")
         if df.dtypes["score"] != int:
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg38.json` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg38.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 6% similar despite different names*

```diff
@@ -1,168 +1,133 @@
-00000000: 7b0a 2020 2020 2263 6f6e 6669 6775 7261  {.    "configura
-00000010: 7469 6f6e 223a 207b 7d2c 0a20 2020 2022  tion": {},.    "
-00000020: 6173 7365 6d62 6c79 223a 207b 0a20 2020  assembly": {.   
-00000030: 2020 2020 2022 6e61 6d65 223a 2022 4752       "name": "GR
-00000040: 4368 3338 222c 0a20 2020 2020 2020 2022  Ch38",.        "
-00000050: 7365 7175 656e 6365 223a 207b 0a20 2020  sequence": {.   
-00000060: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000070: 2022 5265 6665 7265 6e63 6553 6571 7565   "ReferenceSeque
-00000080: 6e63 6554 7261 636b 222c 0a20 2020 2020  nceTrack",.     
-00000090: 2020 2020 2020 2022 7472 6163 6b49 6422         "trackId"
-000000a0: 3a20 2247 5243 6833 382d 5265 6665 7265  : "GRCh38-Refere
-000000b0: 6e63 6553 6571 7565 6e63 6554 7261 636b  nceSequenceTrack
-000000c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000000d0: 6164 6170 7465 7222 3a20 7b0a 2020 2020  adapter": {.    
-000000e0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000000f0: 6522 3a20 2242 677a 6970 4661 7374 6141  e": "BgzipFastaA
-00000100: 6461 7074 6572 222c 0a20 2020 2020 2020  dapter",.       
-00000110: 2020 2020 2020 2020 2022 6661 7374 614c           "fastaL
-00000120: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
-00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000140: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
-00000150: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
-00000160: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
-00000170: 6f6d 6573 2f47 5243 6833 382f 6661 7374  omes/GRCh38/fast
-00000180: 612f 4752 4368 3338 2e66 612e 677a 220a  a/GRCh38.fa.gz".
-00000190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001a0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000001b0: 2020 2022 6661 694c 6f63 6174 696f 6e22     "faiLocation"
-000001c0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000001d0: 2020 2020 2020 2020 2275 7269 223a 2022          "uri": "
-000001e0: 6874 7470 733a 2f2f 7333 2e61 6d61 7a6f  https://s3.amazo
-000001f0: 6e61 7773 2e63 6f6d 2f6a 6272 6f77 7365  naws.com/jbrowse
-00000200: 2e6f 7267 2f67 656e 6f6d 6573 2f47 5243  .org/genomes/GRC
-00000210: 6833 382f 6661 7374 612f 4752 4368 3338  h38/fasta/GRCh38
-00000220: 2e66 612e 677a 2e66 6169 220a 2020 2020  .fa.gz.fai".    
-00000230: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00000240: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000250: 677a 694c 6f63 6174 696f 6e22 3a20 7b0a  gziLocation": {.
-00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000270: 2020 2020 2275 7269 223a 2022 6874 7470      "uri": "http
-00000280: 733a 2f2f 7333 2e61 6d61 7a6f 6e61 7773  s://s3.amazonaws
-00000290: 2e63 6f6d 2f6a 6272 6f77 7365 2e6f 7267  .com/jbrowse.org
-000002a0: 2f67 656e 6f6d 6573 2f47 5243 6833 382f  /genomes/GRCh38/
-000002b0: 6661 7374 612f 4752 4368 3338 2e66 612e  fasta/GRCh38.fa.
-000002c0: 677a 2e67 7a69 220a 2020 2020 2020 2020  gz.gzi".        
-000002d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000002e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000002f0: 7d2c 0a20 2020 2020 2020 2022 616c 6961  },.        "alia
-00000300: 7365 7322 3a20 5b0a 2020 2020 2020 2020  ses": [.        
-00000310: 2020 2020 2268 6733 3822 0a20 2020 2020      "hg38".     
-00000320: 2020 205d 2c0a 2020 2020 2020 2020 2272     ],.        "r
-00000330: 6566 4e61 6d65 416c 6961 7365 7322 3a20  efNameAliases": 
-00000340: 7b0a 2020 2020 2020 2020 2020 2020 2261  {.            "a
-00000350: 6461 7074 6572 223a 207b 0a20 2020 2020  dapter": {.     
-00000360: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000370: 223a 2022 5265 664e 616d 6541 6c69 6173  ": "RefNameAlias
-00000380: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
-00000390: 2020 2020 2020 2020 2020 226c 6f63 6174            "locat
-000003a0: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
-000003b0: 2020 2020 2020 2020 2020 2020 2275 7269              "uri
-000003c0: 223a 2022 6874 7470 733a 2f2f 7333 2e61  ": "https://s3.a
-000003d0: 6d61 7a6f 6e61 7773 2e63 6f6d 2f6a 6272  mazonaws.com/jbr
-000003e0: 6f77 7365 2e6f 7267 2f67 656e 6f6d 6573  owse.org/genomes
-000003f0: 2f47 5243 6833 382f 6867 3338 5f61 6c69  /GRCh38/hg38_ali
-00000400: 6173 6573 2e74 7874 220a 2020 2020 2020  ases.txt".      
-00000410: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000420: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000430: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
-00000440: 7472 6163 6b73 223a 205b 0a20 2020 2020  tracks": [.     
-00000450: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000460: 2022 7479 7065 223a 2022 4665 6174 7572   "type": "Featur
-00000470: 6554 7261 636b 222c 0a20 2020 2020 2020  eTrack",.       
-00000480: 2020 2020 2022 7472 6163 6b49 6422 3a20       "trackId": 
-00000490: 226e 6362 695f 7265 6673 6571 5f31 3039  "ncbi_refseq_109
-000004a0: 5f68 6733 3822 2c0a 2020 2020 2020 2020  _hg38",.        
-000004b0: 2020 2020 226e 616d 6522 3a20 224e 4342      "name": "NCB
-000004c0: 4920 5265 6653 6571 2028 4746 4633 5461  I RefSeq (GFF3Ta
-000004d0: 6269 7829 222c 0a20 2020 2020 2020 2020  bix)",.         
-000004e0: 2020 2022 6173 7365 6d62 6c79 4e61 6d65     "assemblyName
-000004f0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00000500: 2020 2020 2020 2247 5243 6833 3822 0a20        "GRCh38". 
-00000510: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00000520: 2020 2020 2020 2020 2020 2263 6174 6567            "categ
-00000530: 6f72 7922 3a20 5b0a 2020 2020 2020 2020  ory": [.        
-00000540: 2020 2020 2020 2020 2241 6e6e 6f74 6174          "Annotat
-00000550: 696f 6e22 0a20 2020 2020 2020 2020 2020  ion".           
-00000560: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00000570: 2261 6461 7074 6572 223a 207b 0a20 2020  "adapter": {.   
-00000580: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00000590: 7065 223a 2022 4766 6633 5461 6269 7841  pe": "Gff3TabixA
-000005a0: 6461 7074 6572 222c 0a20 2020 2020 2020  dapter",.       
-000005b0: 2020 2020 2020 2020 2022 6766 6647 7a4c           "gffGzL
-000005c0: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
-000005f0: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
-00000600: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
-00000610: 6f6d 6573 2f47 5243 6833 382f 6e63 6269  omes/GRCh38/ncbi
-00000620: 5f72 6566 7365 712f 4743 415f 3030 3030  _refseq/GCA_0000
-00000630: 3031 3430 352e 3135 5f47 5243 6833 385f  01405.15_GRCh38_
-00000640: 6675 6c6c 5f61 6e61 6c79 7369 735f 7365  full_analysis_se
-00000650: 742e 7265 6673 6571 5f61 6e6e 6f74 6174  t.refseq_annotat
-00000660: 696f 6e2e 736f 7274 6564 2e67 6666 2e67  ion.sorted.gff.g
-00000670: 7a22 0a20 2020 2020 2020 2020 2020 2020  z".             
-00000680: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000690: 2020 2020 2020 2269 6e64 6578 223a 207b        "index": {
-000006a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006b0: 2020 2020 2022 6c6f 6361 7469 6f6e 223a       "location":
-000006c0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000006d0: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
-000006e0: 3a20 2268 7474 7073 3a2f 2f73 332e 616d  : "https://s3.am
-000006f0: 617a 6f6e 6177 732e 636f 6d2f 6a62 726f  azonaws.com/jbro
-00000700: 7773 652e 6f72 672f 6765 6e6f 6d65 732f  wse.org/genomes/
-00000710: 4752 4368 3338 2f6e 6362 695f 7265 6673  GRCh38/ncbi_refs
-00000720: 6571 2f47 4341 5f30 3030 3030 3134 3035  eq/GCA_000001405
-00000730: 2e31 355f 4752 4368 3338 5f66 756c 6c5f  .15_GRCh38_full_
-00000740: 616e 616c 7973 6973 5f73 6574 2e72 6566  analysis_set.ref
-00000750: 7365 715f 616e 6e6f 7461 7469 6f6e 2e73  seq_annotation.s
-00000760: 6f72 7465 642e 6766 662e 677a 2e74 6269  orted.gff.gz.tbi
-00000770: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000780: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000790: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000007a0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000007b0: 7d0a 2020 2020 5d2c 0a20 2020 2022 6c6f  }.    ],.    "lo
-000007c0: 6361 7469 6f6e 223a 2022 3130 3a32 392c  cation": "10:29,
-000007d0: 3833 382c 3733 372e 2e32 392c 3833 382c  838,737..29,838,
-000007e0: 3831 3922 2c0a 2020 2020 2264 6566 6175  819",.    "defau
-000007f0: 6c74 5365 7373 696f 6e22 3a20 7b0a 2020  ltSession": {.  
-00000800: 2020 2020 2020 226e 616d 6522 3a20 224d        "name": "M
-00000810: 7920 7365 7373 696f 6e22 2c0a 2020 2020  y session",.    
-00000820: 2020 2020 2276 6965 7722 3a20 7b0a 2020      "view": {.  
-00000830: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-00000840: 226c 696e 6561 7247 656e 6f6d 6556 6965  "linearGenomeVie
-00000850: 7722 2c0a 2020 2020 2020 2020 2020 2020  w",.            
-00000860: 2274 7970 6522 3a20 224c 696e 6561 7247  "type": "LinearG
-00000870: 656e 6f6d 6556 6965 7722 2c0a 2020 2020  enomeView",.    
-00000880: 2020 2020 2020 2020 2274 7261 636b 7322          "tracks"
-00000890: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-000008a0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000008b0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000008c0: 3a20 2252 6566 6572 656e 6365 5365 7175  : "ReferenceSequ
-000008d0: 656e 6365 5472 6163 6b22 2c0a 2020 2020  enceTrack",.    
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2263 6f6e 6669 6775 7261 7469 6f6e 223a  "configuration":
-00000900: 2022 4752 4368 3338 2d52 6566 6572 656e   "GRCh38-Referen
-00000910: 6365 5365 7175 656e 6365 5472 6163 6b22  ceSequenceTrack"
-00000920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000930: 2020 2020 2020 2264 6973 706c 6179 7322        "displays"
-00000940: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00000950: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000980: 3a20 224c 696e 6561 7252 6566 6572 656e  : "LinearReferen
-00000990: 6365 5365 7175 656e 6365 4469 7370 6c61  ceSequenceDispla
-000009a0: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2263 6f6e 6669 6775 7261 7469 6f6e 223a  "configuration":
-000009d0: 2022 4752 4368 3338 2d52 6566 6572 656e   "GRCh38-Referen
-000009e0: 6365 5365 7175 656e 6365 5472 6163 6b2d  ceSequenceTrack-
-000009f0: 4c69 6e65 6172 5265 6665 7265 6e63 6553  LinearReferenceS
-00000a00: 6571 7565 6e63 6544 6973 706c 6179 220a  equenceDisplay".
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000a30: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
-00000a60: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00000a70: 7d0a                                     }.
+00000000: 7b0a 2020 2263 6f6e 6669 6775 7261 7469  {.  "configurati
+00000010: 6f6e 223a 207b 7d2c 0a20 2022 6173 7365  on": {},.  "asse
+00000020: 6d62 6c79 223a 207b 0a20 2020 2022 6e61  mbly": {.    "na
+00000030: 6d65 223a 2022 4752 4368 3338 222c 0a20  me": "GRCh38",. 
+00000040: 2020 2022 7365 7175 656e 6365 223a 207b     "sequence": {
+00000050: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+00000060: 5265 6665 7265 6e63 6553 6571 7565 6e63  ReferenceSequenc
+00000070: 6554 7261 636b 222c 0a20 2020 2020 2022  eTrack",.      "
+00000080: 7472 6163 6b49 6422 3a20 2247 5243 6833  trackId": "GRCh3
+00000090: 382d 5265 6665 7265 6e63 6553 6571 7565  8-ReferenceSeque
+000000a0: 6e63 6554 7261 636b 222c 0a20 2020 2020  nceTrack",.     
+000000b0: 2022 6164 6170 7465 7222 3a20 7b0a 2020   "adapter": {.  
+000000c0: 2020 2020 2020 2274 7970 6522 3a20 2242        "type": "B
+000000d0: 677a 6970 4661 7374 6141 6461 7074 6572  gzipFastaAdapter
+000000e0: 222c 0a20 2020 2020 2020 2022 6661 7374  ",.        "fast
+000000f0: 614c 6f63 6174 696f 6e22 3a20 7b0a 2020  aLocation": {.  
+00000100: 2020 2020 2020 2020 2275 7269 223a 2022          "uri": "
+00000110: 6874 7470 733a 2f2f 7333 2e61 6d61 7a6f  https://s3.amazo
+00000120: 6e61 7773 2e63 6f6d 2f6a 6272 6f77 7365  naws.com/jbrowse
+00000130: 2e6f 7267 2f67 656e 6f6d 6573 2f47 5243  .org/genomes/GRC
+00000140: 6833 382f 6661 7374 612f 4752 4368 3338  h38/fasta/GRCh38
+00000150: 2e66 612e 677a 220a 2020 2020 2020 2020  .fa.gz".        
+00000160: 7d2c 0a20 2020 2020 2020 2022 6661 694c  },.        "faiL
+00000170: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
+00000180: 2020 2020 2020 2275 7269 223a 2022 6874        "uri": "ht
+00000190: 7470 733a 2f2f 7333 2e61 6d61 7a6f 6e61  tps://s3.amazona
+000001a0: 7773 2e63 6f6d 2f6a 6272 6f77 7365 2e6f  ws.com/jbrowse.o
+000001b0: 7267 2f67 656e 6f6d 6573 2f47 5243 6833  rg/genomes/GRCh3
+000001c0: 382f 6661 7374 612f 4752 4368 3338 2e66  8/fasta/GRCh38.f
+000001d0: 612e 677a 2e66 6169 220a 2020 2020 2020  a.gz.fai".      
+000001e0: 2020 7d2c 0a20 2020 2020 2020 2022 677a    },.        "gz
+000001f0: 694c 6f63 6174 696f 6e22 3a20 7b0a 2020  iLocation": {.  
+00000200: 2020 2020 2020 2020 2275 7269 223a 2022          "uri": "
+00000210: 6874 7470 733a 2f2f 7333 2e61 6d61 7a6f  https://s3.amazo
+00000220: 6e61 7773 2e63 6f6d 2f6a 6272 6f77 7365  naws.com/jbrowse
+00000230: 2e6f 7267 2f67 656e 6f6d 6573 2f47 5243  .org/genomes/GRC
+00000240: 6833 382f 6661 7374 612f 4752 4368 3338  h38/fasta/GRCh38
+00000250: 2e66 612e 677a 2e67 7a69 220a 2020 2020  .fa.gz.gzi".    
+00000260: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
+00000270: 2020 7d2c 0a20 2020 2022 616c 6961 7365    },.    "aliase
+00000280: 7322 3a20 5b22 6867 3338 225d 2c0a 2020  s": ["hg38"],.  
+00000290: 2020 2272 6566 4e61 6d65 416c 6961 7365    "refNameAliase
+000002a0: 7322 3a20 7b0a 2020 2020 2020 2261 6461  s": {.      "ada
+000002b0: 7074 6572 223a 207b 0a20 2020 2020 2020  pter": {.       
+000002c0: 2022 7479 7065 223a 2022 5265 664e 616d   "type": "RefNam
+000002d0: 6541 6c69 6173 4164 6170 7465 7222 2c0a  eAliasAdapter",.
+000002e0: 2020 2020 2020 2020 226c 6f63 6174 696f          "locatio
+000002f0: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00000300: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
+00000310: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
+00000320: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
+00000330: 6f6d 6573 2f47 5243 6833 382f 6867 3338  omes/GRCh38/hg38
+00000340: 5f61 6c69 6173 6573 2e74 7874 220a 2020  _aliases.txt".  
+00000350: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+00000360: 2020 2020 7d0a 2020 7d2c 0a20 2022 7472      }.  },.  "tr
+00000370: 6163 6b73 223a 205b 0a20 2020 207b 0a20  acks": [.    {. 
+00000380: 2020 2020 2022 7479 7065 223a 2022 4665       "type": "Fe
+00000390: 6174 7572 6554 7261 636b 222c 0a20 2020  atureTrack",.   
+000003a0: 2020 2022 7472 6163 6b49 6422 3a20 226e     "trackId": "n
+000003b0: 6362 695f 7265 6673 6571 5f31 3039 5f68  cbi_refseq_109_h
+000003c0: 6733 3822 2c0a 2020 2020 2020 226e 616d  g38",.      "nam
+000003d0: 6522 3a20 224e 4342 4920 5265 6653 6571  e": "NCBI RefSeq
+000003e0: 2028 4746 4633 5461 6269 7829 222c 0a20   (GFF3Tabix)",. 
+000003f0: 2020 2020 2022 6173 7365 6d62 6c79 4e61       "assemblyNa
+00000400: 6d65 7322 3a20 5b22 4752 4368 3338 225d  mes": ["GRCh38"]
+00000410: 2c0a 2020 2020 2020 2263 6174 6567 6f72  ,.      "categor
+00000420: 7922 3a20 5b22 416e 6e6f 7461 7469 6f6e  y": ["Annotation
+00000430: 225d 2c0a 2020 2020 2020 2261 6461 7074  "],.      "adapt
+00000440: 6572 223a 207b 0a20 2020 2020 2020 2022  er": {.        "
+00000450: 7479 7065 223a 2022 4766 6633 5461 6269  type": "Gff3Tabi
+00000460: 7841 6461 7074 6572 222c 0a20 2020 2020  xAdapter",.     
+00000470: 2020 2022 6766 6647 7a4c 6f63 6174 696f     "gffGzLocatio
+00000480: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00000490: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
+000004a0: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
+000004b0: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
+000004c0: 6f6d 6573 2f47 5243 6833 382f 6e63 6269  omes/GRCh38/ncbi
+000004d0: 5f72 6566 7365 712f 4743 415f 3030 3030  _refseq/GCA_0000
+000004e0: 3031 3430 352e 3135 5f47 5243 6833 385f  01405.15_GRCh38_
+000004f0: 6675 6c6c 5f61 6e61 6c79 7369 735f 7365  full_analysis_se
+00000500: 742e 7265 6673 6571 5f61 6e6e 6f74 6174  t.refseq_annotat
+00000510: 696f 6e2e 736f 7274 6564 2e67 6666 2e67  ion.sorted.gff.g
+00000520: 7a22 0a20 2020 2020 2020 207d 2c0a 2020  z".        },.  
+00000530: 2020 2020 2020 2269 6e64 6578 223a 207b        "index": {
+00000540: 0a20 2020 2020 2020 2020 2022 6c6f 6361  .          "loca
+00000550: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
+00000560: 2020 2020 2022 7572 6922 3a20 2268 7474       "uri": "htt
+00000570: 7073 3a2f 2f73 332e 616d 617a 6f6e 6177  ps://s3.amazonaw
+00000580: 732e 636f 6d2f 6a62 726f 7773 652e 6f72  s.com/jbrowse.or
+00000590: 672f 6765 6e6f 6d65 732f 4752 4368 3338  g/genomes/GRCh38
+000005a0: 2f6e 6362 695f 7265 6673 6571 2f47 4341  /ncbi_refseq/GCA
+000005b0: 5f30 3030 3030 3134 3035 2e31 355f 4752  _000001405.15_GR
+000005c0: 4368 3338 5f66 756c 6c5f 616e 616c 7973  Ch38_full_analys
+000005d0: 6973 5f73 6574 2e72 6566 7365 715f 616e  is_set.refseq_an
+000005e0: 6e6f 7461 7469 6f6e 2e73 6f72 7465 642e  notation.sorted.
+000005f0: 6766 662e 677a 2e74 6269 220a 2020 2020  gff.gz.tbi".    
+00000600: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00000610: 7d0a 2020 2020 2020 7d0a 2020 2020 7d0a  }.      }.    }.
+00000620: 2020 5d2c 0a20 2022 6c6f 6361 7469 6f6e    ],.  "location
+00000630: 223a 2022 3130 3a32 392c 3833 382c 3733  ": "10:29,838,73
+00000640: 372e 2e32 392c 3833 382c 3831 3922 2c0a  7..29,838,819",.
+00000650: 2020 2264 6566 6175 6c74 5365 7373 696f    "defaultSessio
+00000660: 6e22 3a20 7b0a 2020 2020 226e 616d 6522  n": {.    "name"
+00000670: 3a20 224d 7920 7365 7373 696f 6e22 2c0a  : "My session",.
+00000680: 2020 2020 2276 6965 7722 3a20 7b0a 2020      "view": {.  
+00000690: 2020 2020 2269 6422 3a20 226c 696e 6561      "id": "linea
+000006a0: 7247 656e 6f6d 6556 6965 7722 2c0a 2020  rGenomeView",.  
+000006b0: 2020 2020 2274 7970 6522 3a20 224c 696e      "type": "Lin
+000006c0: 6561 7247 656e 6f6d 6556 6965 7722 2c0a  earGenomeView",.
+000006d0: 2020 2020 2020 2274 7261 636b 7322 3a20        "tracks": 
+000006e0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+000006f0: 2020 2020 2020 2274 7970 6522 3a20 2252        "type": "R
+00000700: 6566 6572 656e 6365 5365 7175 656e 6365  eferenceSequence
+00000710: 5472 6163 6b22 2c0a 2020 2020 2020 2020  Track",.        
+00000720: 2020 2263 6f6e 6669 6775 7261 7469 6f6e    "configuration
+00000730: 223a 2022 4752 4368 3338 2d52 6566 6572  ": "GRCh38-Refer
+00000740: 656e 6365 5365 7175 656e 6365 5472 6163  enceSequenceTrac
+00000750: 6b22 2c0a 2020 2020 2020 2020 2020 2264  k",.          "d
+00000760: 6973 706c 6179 7322 3a20 5b0a 2020 2020  isplays": [.    
+00000770: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000780: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000790: 224c 696e 6561 7252 6566 6572 656e 6365  "LinearReference
+000007a0: 5365 7175 656e 6365 4469 7370 6c61 7922  SequenceDisplay"
+000007b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000007c0: 2263 6f6e 6669 6775 7261 7469 6f6e 223a  "configuration":
+000007d0: 2022 4752 4368 3338 2d52 6566 6572 656e   "GRCh38-Referen
+000007e0: 6365 5365 7175 656e 6365 5472 6163 6b2d  ceSequenceTrack-
+000007f0: 4c69 6e65 6172 5265 6665 7265 6e63 6553  LinearReferenceS
+00000800: 6571 7565 6e63 6544 6973 706c 6179 220a  equenceDisplay".
+00000810: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000820: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00000830: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00000840: 7d0a 2020 7d0a 7d0a                      }.  }.}.
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg38_cgv.json` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg38_cgv.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,75 @@
-00000000: 7b0a 2020 2020 2263 6f6e 6669 6775 7261  {.    "configura
-00000010: 7469 6f6e 223a 207b 7d2c 0a20 2020 2022  tion": {},.    "
-00000020: 6173 7365 6d62 6c79 223a 207b 0a20 2020  assembly": {.   
-00000030: 2020 2020 2022 6e61 6d65 223a 2022 6867       "name": "hg
-00000040: 3338 222c 0a20 2020 2020 2020 2022 7365  38",.        "se
-00000050: 7175 656e 6365 223a 207b 0a20 2020 2020  quence": {.     
-00000060: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000070: 5265 6665 7265 6e63 6553 6571 7565 6e63  ReferenceSequenc
-00000080: 6554 7261 636b 222c 0a20 2020 2020 2020  eTrack",.       
-00000090: 2020 2020 2022 7472 6163 6b49 6422 3a20       "trackId": 
-000000a0: 2247 5243 6833 382d 5265 6665 7265 6e63  "GRCh38-Referenc
-000000b0: 6553 6571 7565 6e63 6554 7261 636b 222c  eSequenceTrack",
-000000c0: 0a20 2020 2020 2020 2020 2020 2022 6164  .            "ad
-000000d0: 6170 7465 7222 3a20 7b0a 2020 2020 2020  apter": {.      
-000000e0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000000f0: 3a20 2242 677a 6970 4661 7374 6141 6461  : "BgzipFastaAda
-00000100: 7074 6572 222c 0a20 2020 2020 2020 2020  pter",.         
-00000110: 2020 2020 2020 2022 6661 7374 614c 6f63         "fastaLoc
-00000120: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
-00000130: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00000140: 7269 223a 2022 6874 7470 733a 2f2f 6a62  ri": "https://jb
-00000150: 726f 7773 652e 6f72 672f 6765 6e6f 6d65  rowse.org/genome
-00000160: 732f 4752 4368 3338 2f66 6173 7461 2f68  s/GRCh38/fasta/h
-00000170: 6733 382e 7072 6566 6978 2e66 612e 677a  g38.prefix.fa.gz
-00000180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000190: 2020 2020 2020 2022 6c6f 6361 7469 6f6e         "location
-000001a0: 5479 7065 223a 2022 5572 694c 6f63 6174  Type": "UriLocat
-000001b0: 696f 6e22 0a20 2020 2020 2020 2020 2020  ion".           
-000001c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000001d0: 2020 2020 2020 2020 2266 6169 4c6f 6361          "faiLoca
-000001e0: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-000001f0: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
-00000200: 6922 3a20 2268 7474 7073 3a2f 2f6a 6272  i": "https://jbr
-00000210: 6f77 7365 2e6f 7267 2f67 656e 6f6d 6573  owse.org/genomes
-00000220: 2f47 5243 6833 382f 6661 7374 612f 6867  /GRCh38/fasta/hg
-00000230: 3338 2e70 7265 6669 782e 6661 2e67 7a2e  38.prefix.fa.gz.
-00000240: 6661 6922 2c0a 2020 2020 2020 2020 2020  fai",.          
-00000250: 2020 2020 2020 2020 2020 226c 6f63 6174            "locat
-00000260: 696f 6e54 7970 6522 3a20 2255 7269 4c6f  ionType": "UriLo
-00000270: 6361 7469 6f6e 220a 2020 2020 2020 2020  cation".        
-00000280: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000290: 2020 2020 2020 2020 2020 2022 677a 694c             "gziL
-000002a0: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
-000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002c0: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
-000002d0: 6a62 726f 7773 652e 6f72 672f 6765 6e6f  jbrowse.org/geno
-000002e0: 6d65 732f 4752 4368 3338 2f66 6173 7461  mes/GRCh38/fasta
-000002f0: 2f68 6733 382e 7072 6566 6978 2e66 612e  /hg38.prefix.fa.
-00000300: 677a 2e67 7a69 222c 0a20 2020 2020 2020  gz.gzi",.       
-00000310: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-00000320: 6361 7469 6f6e 5479 7065 223a 2022 5572  cationType": "Ur
-00000330: 694c 6f63 6174 696f 6e22 0a20 2020 2020  iLocation".     
-00000340: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000350: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000360: 2020 207d 2c0a 2020 2020 2020 2020 2261     },.        "a
-00000370: 6c69 6173 6573 223a 205b 0a20 2020 2020  liases": [.     
-00000380: 2020 2020 2020 2022 4752 4368 3338 220a         "GRCh38".
-00000390: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000003a0: 2020 2022 7265 664e 616d 6541 6c69 6173     "refNameAlias
-000003b0: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
-000003c0: 2020 2022 6164 6170 7465 7222 3a20 7b0a     "adapter": {.
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2274 7970 6522 3a20 2252 6566 4e61 6d65  "type": "RefName
-000003f0: 416c 6961 7341 6461 7074 6572 222c 0a20  AliasAdapter",. 
-00000400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000410: 6c6f 6361 7469 6f6e 223a 207b 0a20 2020  location": {.   
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
-00000440: 2f73 332e 616d 617a 6f6e 6177 732e 636f  /s3.amazonaws.co
-00000450: 6d2f 6a62 726f 7773 652e 6f72 672f 6765  m/jbrowse.org/ge
-00000460: 6e6f 6d65 732f 4752 4368 3338 2f68 6733  nomes/GRCh38/hg3
-00000470: 385f 616c 6961 7365 732e 7478 7422 2c0a  8_aliases.txt",.
-00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000490: 2020 2020 226c 6f63 6174 696f 6e54 7970      "locationTyp
-000004a0: 6522 3a20 2255 7269 4c6f 6361 7469 6f6e  e": "UriLocation
-000004b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000004c0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000004d0: 7d0a 2020 2020 2020 2020 7d0a 2020 2020  }.        }.    
-000004e0: 7d2c 0a20 2020 2022 7472 6163 6b73 223a  },.    "tracks":
-000004f0: 205b 5d2c 0a20 2020 2022 6465 6661 756c   [],.    "defaul
-00000500: 7453 6573 7369 6f6e 223a 207b 0a20 2020  tSession": {.   
-00000510: 2020 2020 2022 6e61 6d65 223a 2022 4d79       "name": "My
-00000520: 2073 6573 7369 6f6e 222c 0a20 2020 2020   session",.     
-00000530: 2020 2022 7669 6577 223a 207b 0a20 2020     "view": {.   
-00000540: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-00000550: 6369 7263 756c 6172 5669 6577 222c 0a20  circularView",. 
-00000560: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00000570: 223a 2022 4369 7263 756c 6172 5669 6577  ": "CircularView
-00000580: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000590: 6270 5065 7250 7822 3a20 3530 3030 3030  bpPerPx": 500000
-000005a0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-000005b0: 7472 6163 6b73 223a 205b 5d0a 2020 2020  tracks": [].    
-000005c0: 2020 2020 7d0a 2020 2020 7d0a 7d0a           }.    }.}.
+00000000: 7b0a 2020 2263 6f6e 6669 6775 7261 7469  {.  "configurati
+00000010: 6f6e 223a 207b 7d2c 0a20 2022 6173 7365  on": {},.  "asse
+00000020: 6d62 6c79 223a 207b 0a20 2020 2022 6e61  mbly": {.    "na
+00000030: 6d65 223a 2022 6867 3338 222c 0a20 2020  me": "hg38",.   
+00000040: 2022 7365 7175 656e 6365 223a 207b 0a20   "sequence": {. 
+00000050: 2020 2020 2022 7479 7065 223a 2022 5265       "type": "Re
+00000060: 6665 7265 6e63 6553 6571 7565 6e63 6554  ferenceSequenceT
+00000070: 7261 636b 222c 0a20 2020 2020 2022 7472  rack",.      "tr
+00000080: 6163 6b49 6422 3a20 2247 5243 6833 382d  ackId": "GRCh38-
+00000090: 5265 6665 7265 6e63 6553 6571 7565 6e63  ReferenceSequenc
+000000a0: 6554 7261 636b 222c 0a20 2020 2020 2022  eTrack",.      "
+000000b0: 6164 6170 7465 7222 3a20 7b0a 2020 2020  adapter": {.    
+000000c0: 2020 2020 2274 7970 6522 3a20 2242 677a      "type": "Bgz
+000000d0: 6970 4661 7374 6141 6461 7074 6572 222c  ipFastaAdapter",
+000000e0: 0a20 2020 2020 2020 2022 6661 7374 614c  .        "fastaL
+000000f0: 6f63 6174 696f 6e22 3a20 7b0a 2020 2020  ocation": {.    
+00000100: 2020 2020 2020 2275 7269 223a 2022 6874        "uri": "ht
+00000110: 7470 733a 2f2f 6a62 726f 7773 652e 6f72  tps://jbrowse.or
+00000120: 672f 6765 6e6f 6d65 732f 4752 4368 3338  g/genomes/GRCh38
+00000130: 2f66 6173 7461 2f68 6733 382e 7072 6566  /fasta/hg38.pref
+00000140: 6978 2e66 612e 677a 222c 0a20 2020 2020  ix.fa.gz",.     
+00000150: 2020 2020 2022 6c6f 6361 7469 6f6e 5479       "locationTy
+00000160: 7065 223a 2022 5572 694c 6f63 6174 696f  pe": "UriLocatio
+00000170: 6e22 0a20 2020 2020 2020 207d 2c0a 2020  n".        },.  
+00000180: 2020 2020 2020 2266 6169 4c6f 6361 7469        "faiLocati
+00000190: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
+000001a0: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
+000001b0: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
+000001c0: 6f6d 6573 2f47 5243 6833 382f 6661 7374  omes/GRCh38/fast
+000001d0: 612f 6867 3338 2e70 7265 6669 782e 6661  a/hg38.prefix.fa
+000001e0: 2e67 7a2e 6661 6922 2c0a 2020 2020 2020  .gz.fai",.      
+000001f0: 2020 2020 226c 6f63 6174 696f 6e54 7970      "locationTyp
+00000200: 6522 3a20 2255 7269 4c6f 6361 7469 6f6e  e": "UriLocation
+00000210: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
+00000220: 2020 2020 2022 677a 694c 6f63 6174 696f       "gziLocatio
+00000230: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00000240: 2275 7269 223a 2022 6874 7470 733a 2f2f  "uri": "https://
+00000250: 6a62 726f 7773 652e 6f72 672f 6765 6e6f  jbrowse.org/geno
+00000260: 6d65 732f 4752 4368 3338 2f66 6173 7461  mes/GRCh38/fasta
+00000270: 2f68 6733 382e 7072 6566 6978 2e66 612e  /hg38.prefix.fa.
+00000280: 677a 2e67 7a69 222c 0a20 2020 2020 2020  gz.gzi",.       
+00000290: 2020 2022 6c6f 6361 7469 6f6e 5479 7065     "locationType
+000002a0: 223a 2022 5572 694c 6f63 6174 696f 6e22  ": "UriLocation"
+000002b0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+000002c0: 207d 0a20 2020 207d 2c0a 2020 2020 2261   }.    },.    "a
+000002d0: 6c69 6173 6573 223a 205b 2247 5243 6833  liases": ["GRCh3
+000002e0: 3822 5d2c 0a20 2020 2022 7265 664e 616d  8"],.    "refNam
+000002f0: 6541 6c69 6173 6573 223a 207b 0a20 2020  eAliases": {.   
+00000300: 2020 2022 6164 6170 7465 7222 3a20 7b0a     "adapter": {.
+00000310: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000320: 2252 6566 4e61 6d65 416c 6961 7341 6461  "RefNameAliasAda
+00000330: 7074 6572 222c 0a20 2020 2020 2020 2022  pter",.        "
+00000340: 6c6f 6361 7469 6f6e 223a 207b 0a20 2020  location": {.   
+00000350: 2020 2020 2020 2022 7572 6922 3a20 2268         "uri": "h
+00000360: 7474 7073 3a2f 2f73 332e 616d 617a 6f6e  ttps://s3.amazon
+00000370: 6177 732e 636f 6d2f 6a62 726f 7773 652e  aws.com/jbrowse.
+00000380: 6f72 672f 6765 6e6f 6d65 732f 4752 4368  org/genomes/GRCh
+00000390: 3338 2f68 6733 385f 616c 6961 7365 732e  38/hg38_aliases.
+000003a0: 7478 7422 2c0a 2020 2020 2020 2020 2020  txt",.          
+000003b0: 226c 6f63 6174 696f 6e54 7970 6522 3a20  "locationType": 
+000003c0: 2255 7269 4c6f 6361 7469 6f6e 220a 2020  "UriLocation".  
+000003d0: 2020 2020 2020 7d0a 2020 2020 2020 7d0a        }.      }.
+000003e0: 2020 2020 7d0a 2020 7d2c 0a20 2022 7472      }.  },.  "tr
+000003f0: 6163 6b73 223a 205b 5d2c 0a20 2022 6465  acks": [],.  "de
+00000400: 6661 756c 7453 6573 7369 6f6e 223a 207b  faultSession": {
+00000410: 0a20 2020 2022 6e61 6d65 223a 2022 4d79  .    "name": "My
+00000420: 2073 6573 7369 6f6e 222c 0a20 2020 2022   session",.    "
+00000430: 7669 6577 223a 207b 0a20 2020 2020 2022  view": {.      "
+00000440: 6964 223a 2022 6369 7263 756c 6172 5669  id": "circularVi
+00000450: 6577 222c 0a20 2020 2020 2022 7479 7065  ew",.      "type
+00000460: 223a 2022 4369 7263 756c 6172 5669 6577  ": "CircularView
+00000470: 222c 0a20 2020 2020 2022 6270 5065 7250  ",.      "bpPerP
+00000480: 7822 3a20 3530 3030 3030 302c 0a20 2020  x": 5000000,.   
+00000490: 2020 2022 7472 6163 6b73 223a 205b 5d0a     "tracks": [].
+000004a0: 2020 2020 7d0a 2020 7d0a 7d0a                }.  }.}.
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg19_cgv.json` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg19_cgv.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 2% similar despite different names*

```diff
@@ -1,167 +1,136 @@
-00000000: 7b0a 2020 2020 2263 6f6e 6669 6775 7261  {.    "configura
-00000010: 7469 6f6e 223a 207b 7d2c 0a20 2020 2022  tion": {},.    "
-00000020: 6173 7365 6d62 6c79 223a 207b 0a20 2020  assembly": {.   
-00000030: 2020 2020 2022 6e61 6d65 223a 2022 6867       "name": "hg
-00000040: 3139 222c 0a20 2020 2020 2020 2022 616c  19",.        "al
-00000050: 6961 7365 7322 3a20 5b22 4752 4368 3337  iases": ["GRCh37
-00000060: 225d 2c0a 2020 2020 2020 2020 2273 6571  "],.        "seq
-00000070: 7565 6e63 6522 3a20 7b0a 2020 2020 2020  uence": {.      
-00000080: 2020 2020 2020 2274 7970 6522 3a20 2252        "type": "R
-00000090: 6566 6572 656e 6365 5365 7175 656e 6365  eferenceSequence
-000000a0: 5472 6163 6b22 2c0a 2020 2020 2020 2020  Track",.        
-000000b0: 2020 2020 2274 7261 636b 4964 223a 2022      "trackId": "
-000000c0: 5064 3857 6833 3065 6939 5222 2c0a 2020  Pd8Wh30ei9R",.  
-000000d0: 2020 2020 2020 2020 2020 2261 6461 7074            "adapt
-000000e0: 6572 223a 207b 0a20 2020 2020 2020 2020  er": {.         
-000000f0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000100: 4267 7a69 7046 6173 7461 4164 6170 7465  BgzipFastaAdapte
-00000110: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-00000120: 2020 2020 2266 6173 7461 4c6f 6361 7469      "fastaLocati
-00000130: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
-00000140: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
-00000150: 3a20 2268 7474 7073 3a2f 2f6a 6272 6f77  : "https://jbrow
-00000160: 7365 2e6f 7267 2f67 656e 6f6d 6573 2f68  se.org/genomes/h
-00000170: 6731 392f 6661 7374 612f 6867 3139 2e66  g19/fasta/hg19.f
-00000180: 612e 677a 222c 0a20 2020 2020 2020 2020  a.gz",.         
-00000190: 2020 2020 2020 2020 2020 2022 6c6f 6361             "loca
-000001a0: 7469 6f6e 5479 7065 223a 2022 5572 694c  tionType": "UriL
-000001b0: 6f63 6174 696f 6e22 0a20 2020 2020 2020  ocation".       
-000001c0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000001d0: 2020 2020 2020 2020 2020 2020 2266 6169              "fai
-000001e0: 4c6f 6361 7469 6f6e 223a 207b 0a20 2020  Location": {.   
-000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000200: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
-00000210: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
-00000220: 6f6d 6573 2f68 6731 392f 6661 7374 612f  omes/hg19/fasta/
-00000230: 6867 3139 2e66 612e 677a 2e66 6169 222c  hg19.fa.gz.fai",
-00000240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000250: 2020 2020 2022 6c6f 6361 7469 6f6e 5479       "locationTy
-00000260: 7065 223a 2022 5572 694c 6f63 6174 696f  pe": "UriLocatio
-00000270: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
-00000280: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000290: 2020 2020 2020 2267 7a69 4c6f 6361 7469        "gziLocati
-000002a0: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
-000002b0: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
-000002c0: 3a20 2268 7474 7073 3a2f 2f6a 6272 6f77  : "https://jbrow
-000002d0: 7365 2e6f 7267 2f67 656e 6f6d 6573 2f68  se.org/genomes/h
-000002e0: 6731 392f 6661 7374 612f 6867 3139 2e66  g19/fasta/hg19.f
-000002f0: 612e 677a 2e67 7a69 222c 0a20 2020 2020  a.gz.gzi",.     
-00000300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000310: 6c6f 6361 7469 6f6e 5479 7065 223a 2022  locationType": "
-00000320: 5572 694c 6f63 6174 696f 6e22 0a20 2020  UriLocation".   
-00000330: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00000340: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000350: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000360: 2272 6566 4e61 6d65 416c 6961 7365 7322  "refNameAliases"
-00000370: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000380: 2261 6461 7074 6572 223a 207b 0a20 2020  "adapter": {.   
-00000390: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000003a0: 7065 223a 2022 5265 664e 616d 6541 6c69  pe": "RefNameAli
-000003b0: 6173 4164 6170 7465 7222 2c0a 2020 2020  asAdapter",.    
-000003c0: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
-000003d0: 6174 696f 6e22 3a20 7b0a 2020 2020 2020  ation": {.      
-000003e0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-000003f0: 7269 223a 2022 6874 7470 733a 2f2f 7333  ri": "https://s3
-00000400: 2e61 6d61 7a6f 6e61 7773 2e63 6f6d 2f6a  .amazonaws.com/j
-00000410: 6272 6f77 7365 2e6f 7267 2f67 656e 6f6d  browse.org/genom
-00000420: 6573 2f68 6731 392f 6867 3139 5f61 6c69  es/hg19/hg19_ali
-00000430: 6173 6573 2e74 7874 222c 0a20 2020 2020  ases.txt",.     
-00000440: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000450: 6c6f 6361 7469 6f6e 5479 7065 223a 2022  locationType": "
-00000460: 5572 694c 6f63 6174 696f 6e22 0a20 2020  UriLocation".   
-00000470: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00000480: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000490: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
-000004a0: 2020 2274 7261 636b 7322 3a20 5b0a 2020    "tracks": [.  
-000004b0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000004c0: 2020 2020 2274 7970 6522 3a20 2256 6172      "type": "Var
-000004d0: 6961 6e74 5472 6163 6b22 2c0a 2020 2020  iantTrack",.    
-000004e0: 2020 2020 2020 2020 2274 7261 636b 4964          "trackId
-000004f0: 223a 2022 7061 6362 696f 5f73 765f 7663  ": "pacbio_sv_vc
-00000500: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
-00000510: 226e 616d 6522 3a20 2248 4730 3032 2050  "name": "HG002 P
-00000520: 6163 6269 6f20 5356 2028 5643 4629 222c  acbio SV (VCF)",
-00000530: 0a20 2020 2020 2020 2020 2020 2022 6173  .            "as
-00000540: 7365 6d62 6c79 4e61 6d65 7322 3a20 5b22  semblyNames": ["
-00000550: 6867 3139 225d 2c0a 2020 2020 2020 2020  hg19"],.        
-00000560: 2020 2020 2263 6174 6567 6f72 7922 3a20      "category": 
-00000570: 5b22 4749 4142 225d 2c0a 2020 2020 2020  ["GIAB"],.      
-00000580: 2020 2020 2020 2261 6461 7074 6572 223a        "adapter":
-00000590: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000005a0: 2020 2022 7479 7065 223a 2022 5663 6654     "type": "VcfT
-000005b0: 6162 6978 4164 6170 7465 7222 2c0a 2020  abixAdapter",.  
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-000005d0: 6366 477a 4c6f 6361 7469 6f6e 223a 207b  cfGzLocation": {
-000005e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000005f0: 2020 2020 2022 7572 6922 3a20 2268 7474       "uri": "htt
-00000600: 7073 3a2f 2f73 332e 616d 617a 6f6e 6177  ps://s3.amazonaw
-00000610: 732e 636f 6d2f 6a62 726f 7773 652e 6f72  s.com/jbrowse.or
-00000620: 672f 6765 6e6f 6d65 732f 6867 3139 2f70  g/genomes/hg19/p
-00000630: 6163 6269 6f2f 6873 3337 6435 2e48 4730  acbio/hs37d5.HG0
-00000640: 3032 2d53 6571 7565 6c49 492d 4343 532e  02-SequelII-CCS.
-00000650: 626e 642d 6f6e 6c79 2e73 762e 7663 662e  bnd-only.sv.vcf.
-00000660: 677a 222c 0a20 2020 2020 2020 2020 2020  gz",.           
-00000670: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
-00000680: 6f6e 5479 7065 223a 2022 5572 694c 6f63  onType": "UriLoc
-00000690: 6174 696f 6e22 0a20 2020 2020 2020 2020  ation".         
-000006a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000006b0: 2020 2020 2020 2020 2020 2269 6e64 6578            "index
-000006c0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000006d0: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
-000006e0: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000700: 7572 6922 3a20 2268 7474 7073 3a2f 2f73  uri": "https://s
-00000710: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
-00000720: 6a62 726f 7773 652e 6f72 672f 6765 6e6f  jbrowse.org/geno
-00000730: 6d65 732f 6867 3139 2f70 6163 6269 6f2f  mes/hg19/pacbio/
-00000740: 6873 3337 6435 2e48 4730 3032 2d53 6571  hs37d5.HG002-Seq
-00000750: 7565 6c49 492d 4343 532e 626e 642d 6f6e  uelII-CCS.bnd-on
-00000760: 6c79 2e73 762e 7663 662e 677a 2e74 6269  ly.sv.vcf.gz.tbi
-00000770: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000780: 2020 2020 2020 2020 2020 2022 6c6f 6361             "loca
-00000790: 7469 6f6e 5479 7065 223a 2022 5572 694c  tionType": "UriL
-000007a0: 6f63 6174 696f 6e22 0a20 2020 2020 2020  ocation".       
-000007b0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-000007c0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000007d0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000007e0: 2020 2020 2020 207d 0a20 2020 205d 2c0a         }.    ],.
-000007f0: 2020 2020 2264 6566 6175 6c74 5365 7373      "defaultSess
-00000800: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
-00000810: 226e 616d 6522 3a20 224d 7920 7365 7373  "name": "My sess
-00000820: 696f 6e22 2c0a 2020 2020 2020 2020 2276  ion",.        "v
-00000830: 6965 7722 3a20 7b0a 2020 2020 2020 2020  iew": {.        
-00000840: 2020 2020 2269 6422 3a20 2263 6972 6375      "id": "circu
-00000850: 6c61 7256 6965 7722 2c0a 2020 2020 2020  larView",.      
-00000860: 2020 2020 2020 2274 7970 6522 3a20 2243        "type": "C
-00000870: 6972 6375 6c61 7256 6965 7722 2c0a 2020  ircularView",.  
-00000880: 2020 2020 2020 2020 2020 2262 7050 6572            "bpPer
-00000890: 5078 223a 2035 3030 3030 3030 2c20 0a20  Px": 5000000, . 
-000008a0: 2020 2020 2020 2020 2020 2022 7472 6163             "trac
-000008b0: 6b73 223a 205b 7b0a 2020 2020 2020 2020  ks": [{.        
-000008c0: 2020 2020 2020 2020 2269 6422 3a20 2275          "id": "u
-000008d0: 5064 4c4b 4869 6b31 222c 0a20 2020 2020  PdLKHik1",.     
-000008e0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000008f0: 223a 2022 5661 7269 616e 7454 7261 636b  ": "VariantTrack
-00000900: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000910: 2020 2022 636f 6e66 6967 7572 6174 696f     "configuratio
-00000920: 6e22 3a20 2270 6163 6269 6f5f 7376 5f76  n": "pacbio_sv_v
-00000930: 6366 222c 0a20 2020 2020 2020 2020 2020  cf",.           
-00000940: 2020 2020 2022 6469 7370 6c61 7973 223a       "displays":
-00000950: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00000960: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2022 6964 223a 2022 7639 5156 4152 336f   "id": "v9QVAR3o
-00000990: 6142 222c 0a20 2020 2020 2020 2020 2020  aB",.           
-000009a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000009b0: 7065 223a 2022 4368 6f72 6456 6172 6961  pe": "ChordVaria
-000009c0: 6e74 4469 7370 6c61 7922 2c0a 2020 2020  ntDisplay",.    
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 2263 6f6e 6669 6775 7261 7469      "configurati
-000009f0: 6f6e 223a 2022 7061 6362 696f 5f73 765f  on": "pacbio_sv_
-00000a00: 7663 662d 4368 6f72 6456 6172 6961 6e74  vcf-ChordVariant
-00000a10: 4469 7370 6c61 7922 0a20 2020 2020 2020  Display".       
-00000a20: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00000a30: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000a40: 0a20 2020 2020 2020 2020 2020 207d 5d0a  .            }].
-00000a50: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00000a60: 7d0a                                     }.
+00000000: 7b0a 2020 2263 6f6e 6669 6775 7261 7469  {.  "configurati
+00000010: 6f6e 223a 207b 7d2c 0a20 2022 6173 7365  on": {},.  "asse
+00000020: 6d62 6c79 223a 207b 0a20 2020 2022 6e61  mbly": {.    "na
+00000030: 6d65 223a 2022 6867 3139 222c 0a20 2020  me": "hg19",.   
+00000040: 2022 616c 6961 7365 7322 3a20 5b22 4752   "aliases": ["GR
+00000050: 4368 3337 225d 2c0a 2020 2020 2273 6571  Ch37"],.    "seq
+00000060: 7565 6e63 6522 3a20 7b0a 2020 2020 2020  uence": {.      
+00000070: 2274 7970 6522 3a20 2252 6566 6572 656e  "type": "Referen
+00000080: 6365 5365 7175 656e 6365 5472 6163 6b22  ceSequenceTrack"
+00000090: 2c0a 2020 2020 2020 2274 7261 636b 4964  ,.      "trackId
+000000a0: 223a 2022 5064 3857 6833 3065 6939 5222  ": "Pd8Wh30ei9R"
+000000b0: 2c0a 2020 2020 2020 2261 6461 7074 6572  ,.      "adapter
+000000c0: 223a 207b 0a20 2020 2020 2020 2022 7479  ": {.        "ty
+000000d0: 7065 223a 2022 4267 7a69 7046 6173 7461  pe": "BgzipFasta
+000000e0: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
+000000f0: 2020 2266 6173 7461 4c6f 6361 7469 6f6e    "fastaLocation
+00000100: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+00000110: 7572 6922 3a20 2268 7474 7073 3a2f 2f6a  uri": "https://j
+00000120: 6272 6f77 7365 2e6f 7267 2f67 656e 6f6d  browse.org/genom
+00000130: 6573 2f68 6731 392f 6661 7374 612f 6867  es/hg19/fasta/hg
+00000140: 3139 2e66 612e 677a 222c 0a20 2020 2020  19.fa.gz",.     
+00000150: 2020 2020 2022 6c6f 6361 7469 6f6e 5479       "locationTy
+00000160: 7065 223a 2022 5572 694c 6f63 6174 696f  pe": "UriLocatio
+00000170: 6e22 0a20 2020 2020 2020 207d 2c0a 2020  n".        },.  
+00000180: 2020 2020 2020 2266 6169 4c6f 6361 7469        "faiLocati
+00000190: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
+000001a0: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
+000001b0: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
+000001c0: 6f6d 6573 2f68 6731 392f 6661 7374 612f  omes/hg19/fasta/
+000001d0: 6867 3139 2e66 612e 677a 2e66 6169 222c  hg19.fa.gz.fai",
+000001e0: 0a20 2020 2020 2020 2020 2022 6c6f 6361  .          "loca
+000001f0: 7469 6f6e 5479 7065 223a 2022 5572 694c  tionType": "UriL
+00000200: 6f63 6174 696f 6e22 0a20 2020 2020 2020  ocation".       
+00000210: 207d 2c0a 2020 2020 2020 2020 2267 7a69   },.        "gzi
+00000220: 4c6f 6361 7469 6f6e 223a 207b 0a20 2020  Location": {.   
+00000230: 2020 2020 2020 2022 7572 6922 3a20 2268         "uri": "h
+00000240: 7474 7073 3a2f 2f6a 6272 6f77 7365 2e6f  ttps://jbrowse.o
+00000250: 7267 2f67 656e 6f6d 6573 2f68 6731 392f  rg/genomes/hg19/
+00000260: 6661 7374 612f 6867 3139 2e66 612e 677a  fasta/hg19.fa.gz
+00000270: 2e67 7a69 222c 0a20 2020 2020 2020 2020  .gzi",.         
+00000280: 2022 6c6f 6361 7469 6f6e 5479 7065 223a   "locationType":
+00000290: 2022 5572 694c 6f63 6174 696f 6e22 0a20   "UriLocation". 
+000002a0: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+000002b0: 0a20 2020 207d 2c0a 2020 2020 2272 6566  .    },.    "ref
+000002c0: 4e61 6d65 416c 6961 7365 7322 3a20 7b0a  NameAliases": {.
+000002d0: 2020 2020 2020 2261 6461 7074 6572 223a        "adapter":
+000002e0: 207b 0a20 2020 2020 2020 2022 7479 7065   {.        "type
+000002f0: 223a 2022 5265 664e 616d 6541 6c69 6173  ": "RefNameAlias
+00000300: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
+00000310: 2020 226c 6f63 6174 696f 6e22 3a20 7b0a    "location": {.
+00000320: 2020 2020 2020 2020 2020 2275 7269 223a            "uri":
+00000330: 2022 6874 7470 733a 2f2f 7333 2e61 6d61   "https://s3.ama
+00000340: 7a6f 6e61 7773 2e63 6f6d 2f6a 6272 6f77  zonaws.com/jbrow
+00000350: 7365 2e6f 7267 2f67 656e 6f6d 6573 2f68  se.org/genomes/h
+00000360: 6731 392f 6867 3139 5f61 6c69 6173 6573  g19/hg19_aliases
+00000370: 2e74 7874 222c 0a20 2020 2020 2020 2020  .txt",.         
+00000380: 2022 6c6f 6361 7469 6f6e 5479 7065 223a   "locationType":
+00000390: 2022 5572 694c 6f63 6174 696f 6e22 0a20   "UriLocation". 
+000003a0: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+000003b0: 0a20 2020 207d 0a20 207d 2c0a 2020 2274  .    }.  },.  "t
+000003c0: 7261 636b 7322 3a20 5b0a 2020 2020 7b0a  racks": [.    {.
+000003d0: 2020 2020 2020 2274 7970 6522 3a20 2256        "type": "V
+000003e0: 6172 6961 6e74 5472 6163 6b22 2c0a 2020  ariantTrack",.  
+000003f0: 2020 2020 2274 7261 636b 4964 223a 2022      "trackId": "
+00000400: 7061 6362 696f 5f73 765f 7663 6622 2c0a  pacbio_sv_vcf",.
+00000410: 2020 2020 2020 226e 616d 6522 3a20 2248        "name": "H
+00000420: 4730 3032 2050 6163 6269 6f20 5356 2028  G002 Pacbio SV (
+00000430: 5643 4629 222c 0a20 2020 2020 2022 6173  VCF)",.      "as
+00000440: 7365 6d62 6c79 4e61 6d65 7322 3a20 5b22  semblyNames": ["
+00000450: 6867 3139 225d 2c0a 2020 2020 2020 2263  hg19"],.      "c
+00000460: 6174 6567 6f72 7922 3a20 5b22 4749 4142  ategory": ["GIAB
+00000470: 225d 2c0a 2020 2020 2020 2261 6461 7074  "],.      "adapt
+00000480: 6572 223a 207b 0a20 2020 2020 2020 2022  er": {.        "
+00000490: 7479 7065 223a 2022 5663 6654 6162 6978  type": "VcfTabix
+000004a0: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
+000004b0: 2020 2276 6366 477a 4c6f 6361 7469 6f6e    "vcfGzLocation
+000004c0: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+000004d0: 7572 6922 3a20 2268 7474 7073 3a2f 2f73  uri": "https://s
+000004e0: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000004f0: 6a62 726f 7773 652e 6f72 672f 6765 6e6f  jbrowse.org/geno
+00000500: 6d65 732f 6867 3139 2f70 6163 6269 6f2f  mes/hg19/pacbio/
+00000510: 6873 3337 6435 2e48 4730 3032 2d53 6571  hs37d5.HG002-Seq
+00000520: 7565 6c49 492d 4343 532e 626e 642d 6f6e  uelII-CCS.bnd-on
+00000530: 6c79 2e73 762e 7663 662e 677a 222c 0a20  ly.sv.vcf.gz",. 
+00000540: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
+00000550: 6f6e 5479 7065 223a 2022 5572 694c 6f63  onType": "UriLoc
+00000560: 6174 696f 6e22 0a20 2020 2020 2020 207d  ation".        }
+00000570: 2c0a 2020 2020 2020 2020 2269 6e64 6578  ,.        "index
+00000580: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+00000590: 6c6f 6361 7469 6f6e 223a 207b 0a20 2020  location": {.   
+000005a0: 2020 2020 2020 2020 2022 7572 6922 3a20           "uri": 
+000005b0: 2268 7474 7073 3a2f 2f73 332e 616d 617a  "https://s3.amaz
+000005c0: 6f6e 6177 732e 636f 6d2f 6a62 726f 7773  onaws.com/jbrows
+000005d0: 652e 6f72 672f 6765 6e6f 6d65 732f 6867  e.org/genomes/hg
+000005e0: 3139 2f70 6163 6269 6f2f 6873 3337 6435  19/pacbio/hs37d5
+000005f0: 2e48 4730 3032 2d53 6571 7565 6c49 492d  .HG002-SequelII-
+00000600: 4343 532e 626e 642d 6f6e 6c79 2e73 762e  CCS.bnd-only.sv.
+00000610: 7663 662e 677a 2e74 6269 222c 0a20 2020  vcf.gz.tbi",.   
+00000620: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
+00000630: 6f6e 5479 7065 223a 2022 5572 694c 6f63  onType": "UriLoc
+00000640: 6174 696f 6e22 0a20 2020 2020 2020 2020  ation".         
+00000650: 207d 0a20 2020 2020 2020 207d 0a20 2020   }.        }.   
+00000660: 2020 207d 0a20 2020 207d 0a20 205d 2c0a     }.    }.  ],.
+00000670: 2020 2264 6566 6175 6c74 5365 7373 696f    "defaultSessio
+00000680: 6e22 3a20 7b0a 2020 2020 226e 616d 6522  n": {.    "name"
+00000690: 3a20 224d 7920 7365 7373 696f 6e22 2c0a  : "My session",.
+000006a0: 2020 2020 2276 6965 7722 3a20 7b0a 2020      "view": {.  
+000006b0: 2020 2020 2269 6422 3a20 2263 6972 6375      "id": "circu
+000006c0: 6c61 7256 6965 7722 2c0a 2020 2020 2020  larView",.      
+000006d0: 2274 7970 6522 3a20 2243 6972 6375 6c61  "type": "Circula
+000006e0: 7256 6965 7722 2c0a 2020 2020 2020 2262  rView",.      "b
+000006f0: 7050 6572 5078 223a 2035 3030 3030 3030  pPerPx": 5000000
+00000700: 2c0a 2020 2020 2020 2274 7261 636b 7322  ,.      "tracks"
+00000710: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00000720: 2020 2020 2020 2020 2269 6422 3a20 2275          "id": "u
+00000730: 5064 4c4b 4869 6b31 222c 0a20 2020 2020  PdLKHik1",.     
+00000740: 2020 2020 2022 7479 7065 223a 2022 5661       "type": "Va
+00000750: 7269 616e 7454 7261 636b 222c 0a20 2020  riantTrack",.   
+00000760: 2020 2020 2020 2022 636f 6e66 6967 7572         "configur
+00000770: 6174 696f 6e22 3a20 2270 6163 6269 6f5f  ation": "pacbio_
+00000780: 7376 5f76 6366 222c 0a20 2020 2020 2020  sv_vcf",.       
+00000790: 2020 2022 6469 7370 6c61 7973 223a 205b     "displays": [
+000007a0: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+000007b0: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+000007c0: 223a 2022 7639 5156 4152 336f 6142 222c  ": "v9QVAR3oaB",
+000007d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000007e0: 7479 7065 223a 2022 4368 6f72 6456 6172  type": "ChordVar
+000007f0: 6961 6e74 4469 7370 6c61 7922 2c0a 2020  iantDisplay",.  
+00000800: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00000810: 6669 6775 7261 7469 6f6e 223a 2022 7061  figuration": "pa
+00000820: 6362 696f 5f73 765f 7663 662d 4368 6f72  cbio_sv_vcf-Chor
+00000830: 6456 6172 6961 6e74 4469 7370 6c61 7922  dVariantDisplay"
+00000840: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00000850: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00000860: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+00000870: 207d 0a20 207d 0a7d 0a                    }.  }.}.
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/data/hg19.json` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/data/hg19.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 10% similar despite different names*

```diff
@@ -1,136 +1,108 @@
-00000000: 7b0a 2020 2020 2263 6f6e 6669 6775 7261  {.    "configura
-00000010: 7469 6f6e 223a 207b 7d2c 0a20 2020 2022  tion": {},.    "
-00000020: 6173 7365 6d62 6c79 223a 207b 0a20 2020  assembly": {.   
-00000030: 2020 2020 2022 6e61 6d65 223a 2022 6867       "name": "hg
-00000040: 3139 222c 0a20 2020 2020 2020 2022 616c  19",.        "al
-00000050: 6961 7365 7322 3a20 5b0a 2020 2020 2020  iases": [.      
-00000060: 2020 2020 2020 2247 5243 6833 3722 0a20        "GRCh37". 
-00000070: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00000080: 2020 2273 6571 7565 6e63 6522 3a20 7b0a    "sequence": {.
-00000090: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000000a0: 6522 3a20 2252 6566 6572 656e 6365 5365  e": "ReferenceSe
-000000b0: 7175 656e 6365 5472 6163 6b22 2c0a 2020  quenceTrack",.  
-000000c0: 2020 2020 2020 2020 2020 2274 7261 636b            "track
-000000d0: 4964 223a 2022 6867 3139 2d52 6566 6572  Id": "hg19-Refer
-000000e0: 656e 6365 5365 7175 656e 6365 5472 6163  enceSequenceTrac
-000000f0: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
-00000100: 2261 6461 7074 6572 223a 207b 0a20 2020  "adapter": {.   
-00000110: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00000120: 7065 223a 2022 4267 7a69 7046 6173 7461  pe": "BgzipFasta
-00000130: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
-00000140: 2020 2020 2020 2020 2020 2266 6173 7461            "fasta
-00000150: 4c6f 6361 7469 6f6e 223a 207b 0a20 2020  Location": {.   
-00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000170: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
-00000180: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
-00000190: 6f6d 6573 2f68 6731 392f 6661 7374 612f  omes/hg19/fasta/
-000001a0: 6867 3139 2e66 612e 677a 220a 2020 2020  hg19.fa.gz".    
-000001b0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000001c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000001d0: 6661 694c 6f63 6174 696f 6e22 3a20 7b0a  faiLocation": {.
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001f0: 2020 2020 2275 7269 223a 2022 6874 7470      "uri": "http
-00000200: 733a 2f2f 6a62 726f 7773 652e 6f72 672f  s://jbrowse.org/
-00000210: 6765 6e6f 6d65 732f 6867 3139 2f66 6173  genomes/hg19/fas
-00000220: 7461 2f68 6731 392e 6661 2e67 7a2e 6661  ta/hg19.fa.gz.fa
-00000230: 6922 0a20 2020 2020 2020 2020 2020 2020  i".             
-00000240: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00000250: 2020 2020 2020 2267 7a69 4c6f 6361 7469        "gziLocati
-00000260: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
-00000270: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
-00000280: 3a20 2268 7474 7073 3a2f 2f6a 6272 6f77  : "https://jbrow
-00000290: 7365 2e6f 7267 2f67 656e 6f6d 6573 2f68  se.org/genomes/h
-000002a0: 6731 392f 6661 7374 612f 6867 3139 2e66  g19/fasta/hg19.f
-000002b0: 612e 677a 2e67 7a69 220a 2020 2020 2020  a.gz.gzi".      
-000002c0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000002d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000002e0: 2020 7d2c 0a20 2020 2020 2020 2022 7265    },.        "re
-000002f0: 664e 616d 6541 6c69 6173 6573 223a 207b  fNameAliases": {
-00000300: 0a20 2020 2020 2020 2020 2020 2022 6164  .            "ad
-00000310: 6170 7465 7222 3a20 7b0a 2020 2020 2020  apter": {.      
-00000320: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00000330: 3a20 2252 6566 4e61 6d65 416c 6961 7341  : "RefNameAliasA
-00000340: 6461 7074 6572 222c 0a20 2020 2020 2020  dapter",.       
-00000350: 2020 2020 2020 2020 2022 6c6f 6361 7469           "locati
-00000360: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
-00000370: 2020 2020 2020 2020 2020 2022 7572 6922             "uri"
-00000380: 3a20 2268 7474 7073 3a2f 2f73 332e 616d  : "https://s3.am
-00000390: 617a 6f6e 6177 732e 636f 6d2f 6a62 726f  azonaws.com/jbro
-000003a0: 7773 652e 6f72 672f 6765 6e6f 6d65 732f  wse.org/genomes/
-000003b0: 6867 3139 2f68 6731 395f 616c 6961 7365  hg19/hg19_aliase
-000003c0: 732e 7478 7422 0a20 2020 2020 2020 2020  s.txt".         
-000003d0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000003e0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000003f0: 0a20 2020 207d 2c0a 2020 2020 2274 7261  .    },.    "tra
-00000400: 636b 7322 3a20 5b0a 2020 2020 2020 2020  cks": [.        
-00000410: 7b0a 2020 2020 2020 2020 2020 2020 2274  {.            "t
-00000420: 7970 6522 3a20 2246 6561 7475 7265 5472  ype": "FeatureTr
-00000430: 6163 6b22 2c0a 2020 2020 2020 2020 2020  ack",.          
-00000440: 2020 2274 7261 636b 4964 223a 2022 7265    "trackId": "re
-00000450: 7065 6174 735f 6867 3139 222c 0a20 2020  peats_hg19",.   
-00000460: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00000470: 2022 5265 7065 6174 7322 2c0a 2020 2020   "Repeats",.    
-00000480: 2020 2020 2020 2020 2261 7373 656d 626c          "assembl
-00000490: 794e 616d 6573 223a 205b 2268 6731 3922  yNames": ["hg19"
-000004a0: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-000004b0: 6361 7465 676f 7279 223a 205b 2241 6e6e  category": ["Ann
-000004c0: 6f74 6174 696f 6e22 5d2c 0a20 2020 2020  otation"],.     
-000004d0: 2020 2020 2020 2022 6164 6170 7465 7222         "adapter"
-000004e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000004f0: 2020 2274 7970 6522 3a20 2242 6967 4265    "type": "BigBe
-00000500: 6441 6461 7074 6572 222c 0a20 2020 2020  dAdapter",.     
-00000510: 2020 2020 2020 2020 2022 6269 6742 6564           "bigBed
-00000520: 4c6f 6361 7469 6f6e 223a 207b 0a20 2020  Location": {.   
-00000530: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
-00000540: 6922 3a20 2268 7474 7073 3a2f 2f6a 6272  i": "https://jbr
-00000550: 6f77 7365 2e6f 7267 2f67 656e 6f6d 6573  owse.org/genomes
-00000560: 2f68 6731 392f 7265 7065 6174 732e 6262  /hg19/repeats.bb
-00000570: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000580: 2020 2022 6c6f 6361 7469 6f6e 5479 7065     "locationType
-00000590: 223a 2022 5572 694c 6f63 6174 696f 6e22  ": "UriLocation"
-000005a0: 0a20 2020 2020 2020 2020 2020 2020 207d  .              }
-000005b0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000005c0: 2020 2020 2020 2020 207d 0a20 2020 205d           }.    ]
-000005d0: 2c0a 2020 2020 2264 6566 6175 6c74 5365  ,.    "defaultSe
-000005e0: 7373 696f 6e22 3a20 7b0a 2020 2020 2020  ssion": {.      
-000005f0: 2020 226e 616d 6522 3a20 2274 6573 7422    "name": "test"
-00000600: 2c0a 2020 2020 2020 2020 2276 6965 7722  ,.        "view"
-00000610: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000620: 2269 6422 3a20 2261 5539 4e71 6a65 3155  "id": "aU9Nqje1U
-00000630: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000640: 7479 7065 223a 2022 4c69 6e65 6172 4765  type": "LinearGe
-00000650: 6e6f 6d65 5669 6577 222c 0a20 2020 2020  nomeView",.     
-00000660: 2020 2020 2020 2022 7472 6163 6b73 223a         "tracks":
-00000670: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00000680: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000690: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000006a0: 2022 5265 6665 7265 6e63 6553 6571 7565   "ReferenceSeque
-000006b0: 6e63 6554 7261 636b 222c 0a20 2020 2020  nceTrack",.     
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000006d0: 636f 6e66 6967 7572 6174 696f 6e22 3a20  configuration": 
-000006e0: 2268 6731 392d 5265 6665 7265 6e63 6553  "hg19-ReferenceS
-000006f0: 6571 7565 6e63 6554 7261 636b 222c 0a20  equenceTrack",. 
-00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000710: 2020 2022 6469 7370 6c61 7973 223a 205b     "displays": [
-00000720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000730: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000750: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00000760: 4c69 6e65 6172 5265 6665 7265 6e63 6553  LinearReferenceS
-00000770: 6571 7565 6e63 6544 6973 706c 6179 222c  equenceDisplay",
-00000780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000790: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-000007a0: 6e66 6967 7572 6174 696f 6e22 3a20 2268  nfiguration": "h
-000007b0: 6731 392d 5265 6665 7265 6e63 6553 6571  g19-ReferenceSeq
-000007c0: 7565 6e63 6554 7261 636b 2d4c 696e 6561  uenceTrack-Linea
-000007d0: 7252 6566 6572 656e 6365 5365 7175 656e  rReferenceSequen
-000007e0: 6365 4469 7370 6c61 7922 0a20 2020 2020  ceDisplay".     
-000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000800: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00000810: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00000820: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000830: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00000840: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
-00000850: 226c 6f63 6174 696f 6e22 3a20 2231 3a36  "location": "1:6
-00000860: 3836 3534 3639 342e 2e36 3836 3534 3733  8654694..6865473
-00000870: 3822 0a7d 0a                             8".}.
+00000000: 7b0a 2020 2263 6f6e 6669 6775 7261 7469  {.  "configurati
+00000010: 6f6e 223a 207b 7d2c 0a20 2022 6173 7365  on": {},.  "asse
+00000020: 6d62 6c79 223a 207b 0a20 2020 2022 6e61  mbly": {.    "na
+00000030: 6d65 223a 2022 6867 3139 222c 0a20 2020  me": "hg19",.   
+00000040: 2022 616c 6961 7365 7322 3a20 5b22 4752   "aliases": ["GR
+00000050: 4368 3337 225d 2c0a 2020 2020 2273 6571  Ch37"],.    "seq
+00000060: 7565 6e63 6522 3a20 7b0a 2020 2020 2020  uence": {.      
+00000070: 2274 7970 6522 3a20 2252 6566 6572 656e  "type": "Referen
+00000080: 6365 5365 7175 656e 6365 5472 6163 6b22  ceSequenceTrack"
+00000090: 2c0a 2020 2020 2020 2274 7261 636b 4964  ,.      "trackId
+000000a0: 223a 2022 6867 3139 2d52 6566 6572 656e  ": "hg19-Referen
+000000b0: 6365 5365 7175 656e 6365 5472 6163 6b22  ceSequenceTrack"
+000000c0: 2c0a 2020 2020 2020 2261 6461 7074 6572  ,.      "adapter
+000000d0: 223a 207b 0a20 2020 2020 2020 2022 7479  ": {.        "ty
+000000e0: 7065 223a 2022 4267 7a69 7046 6173 7461  pe": "BgzipFasta
+000000f0: 4164 6170 7465 7222 2c0a 2020 2020 2020  Adapter",.      
+00000100: 2020 2266 6173 7461 4c6f 6361 7469 6f6e    "fastaLocation
+00000110: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+00000120: 7572 6922 3a20 2268 7474 7073 3a2f 2f6a  uri": "https://j
+00000130: 6272 6f77 7365 2e6f 7267 2f67 656e 6f6d  browse.org/genom
+00000140: 6573 2f68 6731 392f 6661 7374 612f 6867  es/hg19/fasta/hg
+00000150: 3139 2e66 612e 677a 220a 2020 2020 2020  19.fa.gz".      
+00000160: 2020 7d2c 0a20 2020 2020 2020 2022 6661    },.        "fa
+00000170: 694c 6f63 6174 696f 6e22 3a20 7b0a 2020  iLocation": {.  
+00000180: 2020 2020 2020 2020 2275 7269 223a 2022          "uri": "
+00000190: 6874 7470 733a 2f2f 6a62 726f 7773 652e  https://jbrowse.
+000001a0: 6f72 672f 6765 6e6f 6d65 732f 6867 3139  org/genomes/hg19
+000001b0: 2f66 6173 7461 2f68 6731 392e 6661 2e67  /fasta/hg19.fa.g
+000001c0: 7a2e 6661 6922 0a20 2020 2020 2020 207d  z.fai".        }
+000001d0: 2c0a 2020 2020 2020 2020 2267 7a69 4c6f  ,.        "gziLo
+000001e0: 6361 7469 6f6e 223a 207b 0a20 2020 2020  cation": {.     
+000001f0: 2020 2020 2022 7572 6922 3a20 2268 7474       "uri": "htt
+00000200: 7073 3a2f 2f6a 6272 6f77 7365 2e6f 7267  ps://jbrowse.org
+00000210: 2f67 656e 6f6d 6573 2f68 6731 392f 6661  /genomes/hg19/fa
+00000220: 7374 612f 6867 3139 2e66 612e 677a 2e67  sta/hg19.fa.gz.g
+00000230: 7a69 220a 2020 2020 2020 2020 7d0a 2020  zi".        }.  
+00000240: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
+00000250: 2022 7265 664e 616d 6541 6c69 6173 6573   "refNameAliases
+00000260: 223a 207b 0a20 2020 2020 2022 6164 6170  ": {.      "adap
+00000270: 7465 7222 3a20 7b0a 2020 2020 2020 2020  ter": {.        
+00000280: 2274 7970 6522 3a20 2252 6566 4e61 6d65  "type": "RefName
+00000290: 416c 6961 7341 6461 7074 6572 222c 0a20  AliasAdapter",. 
+000002a0: 2020 2020 2020 2022 6c6f 6361 7469 6f6e         "location
+000002b0: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+000002c0: 7572 6922 3a20 2268 7474 7073 3a2f 2f73  uri": "https://s
+000002d0: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000002e0: 6a62 726f 7773 652e 6f72 672f 6765 6e6f  jbrowse.org/geno
+000002f0: 6d65 732f 6867 3139 2f68 6731 395f 616c  mes/hg19/hg19_al
+00000300: 6961 7365 732e 7478 7422 0a20 2020 2020  iases.txt".     
+00000310: 2020 207d 0a20 2020 2020 207d 0a20 2020     }.      }.   
+00000320: 207d 0a20 207d 2c0a 2020 2274 7261 636b   }.  },.  "track
+00000330: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
+00000340: 2020 2274 7970 6522 3a20 2246 6561 7475    "type": "Featu
+00000350: 7265 5472 6163 6b22 2c0a 2020 2020 2020  reTrack",.      
+00000360: 2274 7261 636b 4964 223a 2022 7265 7065  "trackId": "repe
+00000370: 6174 735f 6867 3139 222c 0a20 2020 2020  ats_hg19",.     
+00000380: 2022 6e61 6d65 223a 2022 5265 7065 6174   "name": "Repeat
+00000390: 7322 2c0a 2020 2020 2020 2261 7373 656d  s",.      "assem
+000003a0: 626c 794e 616d 6573 223a 205b 2268 6731  blyNames": ["hg1
+000003b0: 3922 5d2c 0a20 2020 2020 2022 6361 7465  9"],.      "cate
+000003c0: 676f 7279 223a 205b 2241 6e6e 6f74 6174  gory": ["Annotat
+000003d0: 696f 6e22 5d2c 0a20 2020 2020 2022 6164  ion"],.      "ad
+000003e0: 6170 7465 7222 3a20 7b0a 2020 2020 2020  apter": {.      
+000003f0: 2020 2274 7970 6522 3a20 2242 6967 4265    "type": "BigBe
+00000400: 6441 6461 7074 6572 222c 0a20 2020 2020  dAdapter",.     
+00000410: 2020 2022 6269 6742 6564 4c6f 6361 7469     "bigBedLocati
+00000420: 6f6e 223a 207b 0a20 2020 2020 2020 2020  on": {.         
+00000430: 2022 7572 6922 3a20 2268 7474 7073 3a2f   "uri": "https:/
+00000440: 2f6a 6272 6f77 7365 2e6f 7267 2f67 656e  /jbrowse.org/gen
+00000450: 6f6d 6573 2f68 6731 392f 7265 7065 6174  omes/hg19/repeat
+00000460: 732e 6262 222c 0a20 2020 2020 2020 2020  s.bb",.         
+00000470: 2022 6c6f 6361 7469 6f6e 5479 7065 223a   "locationType":
+00000480: 2022 5572 694c 6f63 6174 696f 6e22 0a20   "UriLocation". 
+00000490: 2020 2020 2020 207d 0a20 2020 2020 207d         }.      }
+000004a0: 0a20 2020 207d 0a20 205d 2c0a 2020 2264  .    }.  ],.  "d
+000004b0: 6566 6175 6c74 5365 7373 696f 6e22 3a20  efaultSession": 
+000004c0: 7b0a 2020 2020 226e 616d 6522 3a20 2274  {.    "name": "t
+000004d0: 6573 7422 2c0a 2020 2020 2276 6965 7722  est",.    "view"
+000004e0: 3a20 7b0a 2020 2020 2020 2269 6422 3a20  : {.      "id": 
+000004f0: 2261 5539 4e71 6a65 3155 222c 0a20 2020  "aU9Nqje1U",.   
+00000500: 2020 2022 7479 7065 223a 2022 4c69 6e65     "type": "Line
+00000510: 6172 4765 6e6f 6d65 5669 6577 222c 0a20  arGenomeView",. 
+00000520: 2020 2020 2022 7472 6163 6b73 223a 205b       "tracks": [
+00000530: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000540: 2020 2020 2022 7479 7065 223a 2022 5265       "type": "Re
+00000550: 6665 7265 6e63 6553 6571 7565 6e63 6554  ferenceSequenceT
+00000560: 7261 636b 222c 0a20 2020 2020 2020 2020  rack",.         
+00000570: 2022 636f 6e66 6967 7572 6174 696f 6e22   "configuration"
+00000580: 3a20 2268 6731 392d 5265 6665 7265 6e63  : "hg19-Referenc
+00000590: 6553 6571 7565 6e63 6554 7261 636b 222c  eSequenceTrack",
+000005a0: 0a20 2020 2020 2020 2020 2022 6469 7370  .          "disp
+000005b0: 6c61 7973 223a 205b 0a20 2020 2020 2020  lays": [.       
+000005c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000005d0: 2020 2020 2022 7479 7065 223a 2022 4c69       "type": "Li
+000005e0: 6e65 6172 5265 6665 7265 6e63 6553 6571  nearReferenceSeq
+000005f0: 7565 6e63 6544 6973 706c 6179 222c 0a20  uenceDisplay",. 
+00000600: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00000610: 6e66 6967 7572 6174 696f 6e22 3a20 2268  nfiguration": "h
+00000620: 6731 392d 5265 6665 7265 6e63 6553 6571  g19-ReferenceSeq
+00000630: 7565 6e63 6554 7261 636b 2d4c 696e 6561  uenceTrack-Linea
+00000640: 7252 6566 6572 656e 6365 5365 7175 656e  rReferenceSequen
+00000650: 6365 4469 7370 6c61 7922 0a20 2020 2020  ceDisplay".     
+00000660: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000670: 2020 205d 0a20 2020 2020 2020 207d 0a20     ].        }. 
+00000680: 2020 2020 205d 0a20 2020 207d 0a20 207d       ].    }.  }
+00000690: 2c0a 2020 226c 6f63 6174 696f 6e22 3a20  ,.  "location": 
+000006a0: 2231 3a36 3836 3534 3639 342e 2e36 3836  "1:68654694..686
+000006b0: 3534 3733 3822 0a7d 0a                   54738".}.
```

### Comparing `jbrowse-jupyter-1.3.6/jbrowse_jupyter/jbrowse_config.py` & `jbrowse-jupyter-1.4.0/jbrowse_jupyter/jbrowse_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         https://jbrowse.org/jb2/docs/config_guide/#assembly-config
 
         :param str assembly_data: url/path to the sequence data
         :param str name: (optional) name for the assembly,
             defaults to name generated from assembly_data file name
         :param list aliases: (optional) list of aliases for the assembly
         :param obj refname_aliases: (optional) config for refname aliases.
-        :param str overwrite: flag wether or not to overwrite
+        :param str overwrite: flag whether or not to overwrite
             existing assembly, default to False.
         :raises TypeError: Paths are only supported in jupyter.
         :raises TypeError: adapter used for file type is not supported or
             recognized
         """
         overwrite = kwargs.get('overwrite', False)
         indx = kwargs.get('index', "defaultIndex")
@@ -362,15 +362,15 @@
 
         e.g:
         add_df_track(df, "track_name")
 
         :param track_data: panda DataFrame with the track data.
         :param str name: name for the track.
         :param str track_id: (optional) trackId for the track
-        :param str overwrite: flag wether or not to overwrite existing track.
+        :param str overwrite: flag whether or not to overwrite existing track.
         :raises Exception: if assembly has not been configured.
         :raises TypeError: if track data is invalid
         :raises TypeError: if view is not LGV
         :raises TypeError: if track with that trackId already exists
             list of tracks
         """
         if not self.get_assembly():
@@ -573,15 +573,15 @@
             self.tracks_ids_map[track_id] = track_config
 
     def delete_track(self, track_id):
         """
         Deletes a track from the config.
 
         e.g:
-        delte_track("test_track_id")
+        delete_track("test_track_id")
 
         Will delete track with track_id test_track_id.
 
         :param str track_id: track_id to delete
 
         :raises TypeError: if track_id provided does not exist
         """
```

