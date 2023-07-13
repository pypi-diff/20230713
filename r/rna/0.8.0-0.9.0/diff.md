# Comparing `tmp/rna-0.8.0-py3-none-any.whl.zip` & `tmp/rna-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 64637 bytes, number of entries: 29
--rw-r--r--  2.0 unx      369 b- defN 80-Jan-01 00:00 rna/__init__.py
+Zip file size: 65539 bytes, number of entries: 29
+-rw-r--r--  2.0 unx      376 b- defN 80-Jan-01 00:00 rna/__init__.py
 -rw-r--r--  2.0 unx     2043 b- defN 80-Jan-01 00:00 rna/__main__.py
--rw-r--r--  2.0 unx     8094 b- defN 80-Jan-01 00:00 rna/config.py
+-rw-r--r--  2.0 unx     9662 b- defN 80-Jan-01 00:00 rna/config.py
 -rw-r--r--  2.0 unx     3719 b- defN 80-Jan-01 00:00 rna/log.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 rna/parsing.py
 -rw-r--r--  2.0 unx     6313 b- defN 80-Jan-01 00:00 rna/path.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 rna/pattern/__init__.py
 -rw-r--r--  2.0 unx      502 b- defN 80-Jan-01 00:00 rna/pattern/backend.py
 -rw-r--r--  2.0 unx    13029 b- defN 80-Jan-01 00:00 rna/pattern/composite.py
 -rw-r--r--  2.0 unx     9003 b- defN 80-Jan-01 00:00 rna/pattern/decorator.py
 -rw-r--r--  2.0 unx     5951 b- defN 80-Jan-01 00:00 rna/pattern/link.py
 -rw-r--r--  2.0 unx      977 b- defN 80-Jan-01 00:00 rna/pattern/singleton.py
 -rw-r--r--  2.0 unx     9053 b- defN 80-Jan-01 00:00 rna/pattern/strategy.py
 -rw-r--r--  2.0 unx     1254 b- defN 80-Jan-01 00:00 rna/pattern/switch.py
--rw-r--r--  2.0 unx     3941 b- defN 80-Jan-01 00:00 rna/plotting/__init__.py
+-rw-r--r--  2.0 unx     3921 b- defN 80-Jan-01 00:00 rna/plotting/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rna/plotting/backends/__init__.py
--rw-r--r--  2.0 unx    40524 b- defN 80-Jan-01 00:00 rna/plotting/backends/matplotlib.py
--rw-r--r--  2.0 unx    11908 b- defN 80-Jan-01 00:00 rna/plotting/backends/pyqtgraph.py
+-rw-r--r--  2.0 unx    40615 b- defN 80-Jan-01 00:00 rna/plotting/backends/matplotlib.py
+-rw-r--r--  2.0 unx    12926 b- defN 80-Jan-01 00:00 rna/plotting/backends/pyqtgraph.py
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 rna/plotting/base.py
 -rw-r--r--  2.0 unx    11330 b- defN 80-Jan-01 00:00 rna/plotting/colors.py
--rw-r--r--  2.0 unx    16863 b- defN 80-Jan-01 00:00 rna/plotting/core.py
+-rw-r--r--  2.0 unx    17074 b- defN 80-Jan-01 00:00 rna/plotting/core.py
 -rw-r--r--  2.0 unx    35834 b- defN 80-Jan-01 00:00 rna/plotting/mplstyles/rna.mplstyle
 -rw-r--r--  2.0 unx     1020 b- defN 80-Jan-01 00:00 rna/plotting/mplstyles/tfields.mplstyle
--rw-r--r--  2.0 unx     6856 b- defN 80-Jan-01 00:00 rna/polymorphism.py
+-rw-r--r--  2.0 unx     6863 b- defN 80-Jan-01 00:00 rna/polymorphism.py
 -rw-r--r--  2.0 unx     3310 b- defN 80-Jan-01 00:00 rna/process.py
--rw-r--r--  2.0 unx     3178 b- defN 80-Jan-01 00:00 rna-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rna-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 rna-0.8.0.dist-info/LICENSE.rst
-?rw-r--r--  2.0 unx     2256 b- defN 16-Jan-01 00:00 rna-0.8.0.dist-info/RECORD
-29 files, 200565 bytes uncompressed, 61085 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 rna-0.9.0.dist-info/LICENSE.rst
+-rw-r--r--  2.0 unx     2916 b- defN 80-Jan-01 00:00 rna-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rna-0.9.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2256 b- defN 16-Jan-01 00:00 rna-0.9.0.dist-info/RECORD
+29 files, 203185 bytes uncompressed, 61987 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -69,20 +69,20 @@
 
 Filename: rna/polymorphism.py
 Comment: 
 
 Filename: rna/process.py
 Comment: 
 
-Filename: rna-0.8.0.dist-info/METADATA
+Filename: rna-0.9.0.dist-info/LICENSE.rst
 Comment: 
 
-Filename: rna-0.8.0.dist-info/WHEEL
+Filename: rna-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: rna-0.8.0.dist-info/LICENSE.rst
+Filename: rna-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: rna-0.8.0.dist-info/RECORD
+Filename: rna-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rna/__init__.py

```diff
@@ -1,14 +1,16 @@
 """Top-level package of rna."""
 
 __author__ = """Daniel Böckenhoff"""
 __email__ = "dboe@ipp.mpg.de"
-__version__ = "0.7.17"
+__version__ = "0.9.0"
 from . import log  # NOQA
 from . import path  # NOQA
 from . import process  # NOQA
 from . import parsing  # NOQA
 from . import pattern  # NOQA
 from . import polymorphism  # NOQA
-from . import plotting
 
-plotting.use("matplotlib")  # TODO: remove
+# TODO: deprecate
+# from . import plotting
+#
+# plotting.use("matplotlib")
```

## rna/config.py

```diff
@@ -27,15 +27,15 @@
 
 OPTION_NOT_FOUND = object()
 logger = logging.getLogger(__name__)
 
 
 class Dialect(Strategy):
     """
-    Abstract Class to be derived by specific dialects of a config files (.ini, .cfg, ...)
+    Abstract Class to be derived by specific dialects of a config file (.ini, .cfg, ...)
     """
 
     def __init__(self):
         super().__init__()
         self._config_cache = {}
 
     def _get_config(self, config_path) -> "configparser.ConfigParser":
@@ -144,54 +144,90 @@
             return yaml.safe_load(_file)
 
 
 def api(
     module: typing.Union[Module, str],
     *merge_configs: str,
     config_dir: typing.Optional[str] = None,
-    config_name: str = "config"
+    config_name: str = "config",
+    version_base: typing.Optional[str] = "1.1",
+    **compose_kwargs
 ) -> omegaconf.OmegaConf:
     """
     Provide an OmegaConfig object read from :param:`config_dir`/:param:`config_name`.yaml
 
     Args:
         module: Module or path to the __init__.py of the module
-         (intended use is to call this from the module's __init__.py
+          (intended use is to call this from the module's __init__.py
           and pass __file__ as argument).
         *merge_configs: paths to configs to be merged in the order given
         config_dir: main directory of hydra config
         config_name: name of main config to read (yaml extended)
+        version_base: base version of hydra config (e.g. 1.1)
+        **compose_kwargs: forwarded to hydra.compose
 
-    this function sets the following values to the OmegaConf object in addition to the read values:
+    # Environment variables
 
-        package.name - module name of package
-        package.path - directory of __init__.py
+    This function sets the following additional environment variables:
 
-        os.home - user home directory ("~")
-        os.user - user name used for login
-        os.sysname - operating system name
-        os.nodename - name of machine on network (implementation-defined)
-        os.release - operating system release
-        os.version - operating system version
-        os.machine - hardware identifier
-        os.platform - The name of the operating system dependent module imported.
-            The following names have currently been registered: 'posix', 'nt', 'java'
+    * package.name - module name of package
+    * package.path - directory of __init__.py
 
+    * os.home - user home directory ("~")
+    * os.user - user name used for login
+    * os.sysname - operating system name (e.g. 'Linux')
+    * os.nodename - name of machine on network (implementation-defined, e.g. 'jdoe_laptop')
+    * os.release - operating system release (e.g. '5.15.0-67-generic')
+    * os.version - operating system version (e.g. '#74~20.04.1-Ubuntu SMP Wed Feb 22 14:52:34 UTC 2023')
+    * os.machine - hardware identifier (e.g. 'x86_64')
+    * os.platform - The name of the operating system dependent module imported.
 
+    # Resolvers
 
-    omegaconf provides builtin
+    omegaconf provides [builtin resolvers](https://omegaconf.readthedocs.io/en/latest/custom_resolvers.html)
 
-        oc.env.NAME -> user name
-        oc.env.HOME -> user home
+    * oc.env
+    * oc.create
+    * oc.deprecated
+    * oc.decode
+    * oc.select
+    * oc.dict
 
-    Note: I encountered problems with oc.env.NAME and oc.env.HOME so this fuction additionally sets
+    This function registers a new OmegaConf resolver to be used in interpolation as
 
-    this function registers a new OmegaConf resolver to be used in interpolation as
+    * "${path:path/to/stuff}" -> rna.path.resolve
 
-        "${path:path/to/stuff}" -> rna.path.resolve
+    Notes:
+        * Schema valdiation is not out of box with hydra.ConfigStore: [see here](https://suneeta-mall.github.io/2022/03/15/hydra-pydantic-config-management-for-training-application.html#where-hydra-falls-short-)
+            Consider using pydantic on top of hydra
+
+            ..code-block:: python
+
+                import rna.config
+                from pydantic.dataclasses import dataclass
+                from omegaconf import OmegaConf
+
+                @dataclass
+                class Employee:
+                    name: str
+                    age: int
+
+
+                @dataclass
+                class Company:
+                    name: str
+                    employees: List[Employee]
+
+
+                cfg = rna.config.api(...)
+                company = Company(**OmegaConf.to_container(cfg.company))
+
+            I found that this practice is working nice but careful: It is discarding additional keywords from the config!
+
+        * Have a look at [hydra_zen](_modules/hydra_zen/structured_configs/_implementations.html)
 
     """
     if isinstance(module, types.ModuleType):
         module_name = module.__name__
         module_path = module.__path__[0]
     elif os.path.basename(module) == "__init__.py":
         module_name = module.split(os.path.sep)[-2]
@@ -204,16 +240,16 @@
 
     if config_dir is None:
         config_dir = os.path.join(module_path, "conf")
 
     omegaconf.OmegaConf.register_new_resolver("path", rna.path.resolve, replace=True)
 
     logger.info("Reading main config in %s with name %s", config_dir, config_name)
-    hydra.initialize_config_dir(config_dir)
-    cfg = hydra.compose(config_name=config_name)
+    hydra.initialize_config_dir(config_dir, version_base=version_base)
+    cfg = hydra.compose(config_name=config_name, **compose_kwargs)
     for path in merge_configs:
         if os.path.exists(path):
             logger.info("Merging with config from %s", path)
             cfg = omegaconf.OmegaConf.merge(cfg, omegaconf.OmegaConf.load(path))
 
     # Add dynamic variables
     with omegaconf.open_dict(cfg):
@@ -233,14 +269,18 @@
         cfg.os.sysname = uname.sysname
         cfg.os.nodename = uname.nodename
         cfg.os.release = uname.release
         cfg.os.version = uname.version
         cfg.os.machine = uname.machine
         cfg.os.platform = os.name
 
+    # free the globalHydra because you might want to include another api that uses this function
+    # You would get 'ValueError: GlobalHydra is already initialized' in that case
+    hydra.core.global_hydra.GlobalHydra.instance().clear()
+
     return cfg
 
 
 def fallback(obj, *attrs):
     """
     Get attributes from object, throwing out attrs before the last from right to left
     in case no omegaconf.errors.ConfigAttributeError was thrown"""
```

## rna/plotting/__init__.py

```diff
@@ -19,15 +19,15 @@
     Tell rna to use the pyqtgraph backend. Default is matplotlib
     >>> rna.plotting.use('pyqtgraph')
 
     Switching back to default for this test. The code below stays the same if you keep pyqtgraph.
     >>> rna.plotting.use('matplotlib')
 
     Get an axes element
-    >>> axes = rna.plotting.gca(3)
+    >>> axes = rna.plotting.add_subplot(dim=3)
 
     Plot the cube
     >>> artist = rna.plotting.plot_mesh(axes, cube, cube.maps[3], color=scalars,
     ...     cmap='plasma')
 
     # Plot a colorbar
     >>> cbar = rna.plotting.set_colorbar(axes, artist)  # TODO: Broken in pyqtgraph atm
@@ -48,14 +48,15 @@
     PlotKwargsFunctions,
 )
 
 
 # TODO: remove EXPOSED_BACKEND_METHOD in favor of check for ApiBackend member
 EXPOSED_BACKEND_METHODS = [
     "axes_dim",
+    "add_subplot",
     "gca",
     "is_axes",
     "show",
     "clear",
     "plot_mesh",
     "plot_tensor_map",
     "plot_array",
@@ -131,11 +132,8 @@
         ratio = (np.sqrt(5.0) - 1.0) / 2.0
     fig_width = width_pt * inches_per_pt * scale  # fig_width in inches
     fig_height = fig_width * ratio  # height in inches
     fig_size = (fig_width, fig_height)
     return fig_size
 
 
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod()
+use("matplotlib")
```

## rna/plotting/backends/matplotlib.py

```diff
@@ -13,14 +13,15 @@
 import matplotlib.collections as mcollections
 import matplotlib.dates as dates
 import matplotlib.patches as mplpatch
 import mpl_toolkits.mplot3d as plt3d
 import mpl_toolkits.axes_grid1 as pltg1
 import rna
 import numpy as np
+import warnings
 
 
 # ANIMATION
 
 try:
     FFMPEGWRITER = manimation.writers["ffmpeg"]
     FFMPEG = True
@@ -40,15 +41,15 @@
             comment (str)
             fps (int)
 
     Examples:
         >>> import numpy as np
         >>> import rna
         >>> from rna.plotting.backends.matplotlib import Writer
-        >>> axes = rna.plotting.gca()
+        >>> axes = rna.plotting.add_subplot()
         >>> writer = Writer()
         >>> pictures = np.array([[[1,1], [0,0]],
         ...                      [[0.5,1], [0,0.5]]])
         >>> with writer.saving():
         ...     for s in pictures:
         ...         artist = axes.imshow(s.T)
         ...         writer.grab_frame()
@@ -160,59 +161,61 @@
         plt.show()
 
     @staticmethod
     def axes_dim(axes):
         """
         Returns int: axes dimension
         """
-        if hasattr(axes, "get_zlim"):
+        if axes.name == "3d":
             return 3
         return 2
 
     @staticmethod
-    def gca(dim=None, **kwargs):
-        """
-        Forwarding to plt.gca but translating the dimension to projection
-        correct dimension
-
-        Examples:
-            >>> ax_2 = rna.plotting.gca(2)
-            >>> assert rna.plotting.axes_dim(ax_2) == 2
-            >>> ax_2_implicit = rna.plotting.gca()
-            >>> assert rna.plotting.axes_dim(ax_2_implicit) == 2
-            >>> assert ax_2 is ax_2_implicit
-
-            >>> ax_3 = rna.plotting.gca(3)
-            >>> assert rna.plotting.axes_dim(ax_3) == 3
-            >>> ax_3_implicit = rna.plotting.gca()
-            >>> assert rna.plotting.axes_dim(ax_3_implicit) == 3
-            >>> assert ax_3 is ax_3_implicit
-
-            >>> ax_2 = rna.plotting.gca(2)
-            >>> assert rna.plotting.axes_dim(ax_2) == 2
-
-        """
+    def add_subplot(dim=None, **kwargs):
         if dim is not None and "projection" not in kwargs:
             if dim == 2:
                 kwargs["projection"] = "rectilinear"
-                # the line above would already be good ...
-                # but there is a bug in matplotlib which ignores setting the default
-                axes = plt.gca(**kwargs)
-                if ApiBackendMatplotlib.axes_dim(axes) != dim:
-                    return plt.gcf().add_subplot(1, 1, 1, **kwargs)
-                else:
-                    return axes
             elif dim == 3:
                 kwargs["projection"] = "3d"
             else:
                 raise NotImplementedError(
                     "Dimension {dim} not implemented".format(**locals())
                 )
-        axes = plt.gca(**kwargs)
-        return axes
+        return plt.gcf().add_subplot(**kwargs)
+
+    @staticmethod
+    def gca(dim=None, **kwargs):
+        """
+        Forwarding to plt.add_subplot but translating the dimension to projection
+        correct dimension
+
+        """
+        # this is deprecated, use axes instead
+        warnings.warn("gca is deprecated, use add_suplot instead")
+        return ApiBackendMatplotlib.add_subplot(dim=dim, **kwargs)
+        # breakpoint()
+        # if dim is not None and "projection" not in kwargs:
+        #     if dim == 2:
+
+        #         kwargs["projection"] = "rectilinear"
+        #         # the line above would already be good ...
+        #         # but there is a bug in matplotlib which ignores setting the default
+        #         axes = plt.gca()
+        #         if ApiBackendMatplotlib.axes_dim(axes) != dim:
+        #             return plt.gcf().add_subplot(**kwargs)
+        #         else:
+        #             return axes
+        #     elif dim == 3:
+        #         kwargs["projection"] = "3d"
+        #     else:
+        #         raise NotImplementedError(
+        #             "Dimension {dim} not implemented".format(**locals())
+        #         )
+        # axes = plt.gca()
+        # return axes
 
     @staticmethod
     def is_axes(obj):
         return isinstance(obj, plt.Axes)
 
     def set_labels(self, axes, *labels):
         """
@@ -243,15 +246,15 @@
     ):
         """
         Note:
             Bug found in matplotlib:
                 when calling axes.clear(), the colorbar has to be removed by hand,
                 since it will not be removed by clear.
             >> import rna
-            >> axes = rna.plotting.gca()
+            >> axes = rna.plotting.add_subplot()
             >> artist = ...
             >> cbar = rna.plotting.set_colorbar(axes, artist)
             >> rna.plotting.save(...)
             >> cbar.remove()  # THIS IS IMPORTANT. Otherwise you will have problems
             # at the next call of savefig.
             >> axes.clear()
         """
@@ -390,15 +393,15 @@
 
 
         """
         # catch figure from axes or fig
         axes = kwargs.pop("axes", None)
         if axes is None:
             fig_default = plt.gcf()
-            axes = self.gca()
+            axes = self.add_subplot()
             if fig_default is None:
                 raise ValueError("fig_default may not be None")
         else:
             fig_default = axes.figure
         fig = kwargs.pop("fig", fig_default)
 
         # resize the figure to match a given width (in pt).
@@ -1099,15 +1102,15 @@
     @rna.plotting.plot_signature
     def set_formatter(
         self, axes, sub_axes=None, formatter=dates.DateFormatter("%d-%m-%y")
     ):
         """
         Examples:
             >>> from rna.plotting.backends.matplotlib import ApiBackendMatplotlib
-            >>> axes = ApiBackendMatplotlib().gca()
+            >>> axes = ApiBackendMatplotlib().add_subplot()
             >>> ApiBackendMatplotlib().set_formatter(axes)
         """
         if sub_axes is None:
             sub_axes = axes.xaxis
         sub_axes.set_major_formatter(formatter)
```

## rna/plotting/backends/pyqtgraph.py

```diff
@@ -15,14 +15,15 @@
                     -> WINDOW
 Axes    -> PlotItem (2D) / GLViewWidget (3D)
 Artist  -> GraphicsItem
 """
 import typing
 import logging
 import sys
+import warnings
 import numpy as np
 import pyqtgraph as pg
 import pyqtgraph.opengl
 import pyqtgraph.exporters
 import rna
 
 
@@ -39,15 +40,43 @@
     if isinstance(axes, pg.PlotItem):
         return 2
     if isinstance(axes, pg.opengl.GLViewWidget):
         return 3
     raise NotImplementedError("Dimension of {axes} not mapped".format(**locals()))
 
 
+def add_subplot(dim=None, **kwargs):
+    global WINDOW, VIEW
+    if dim is None:
+        dim = 2
+
+    if WINDOW is None:
+        pg.mkQApp()
+
+    if dim == 2:
+        VIEW = pg.PlotItem()  # -> GraphicsWidget -> (GraphicsItem, QgraphicsWidget)
+        WINDOW = pg.GraphicsLayoutWidget(title="rna 2D plot")  # show=False
+        WINDOW.addItem(VIEW)  # , row, col, rowspan, colspan)
+    elif dim == 3:
+        VIEW = pg.opengl.GLViewWidget()
+        WINDOW = pg.LayoutWidget()
+        WINDOW.addWidget(VIEW)
+    else:
+        raise NotImplementedError()
+
+    WINDOW.resize(800, 800)
+
+    return VIEW
+
+
 def gca(dim=None):
+    """
+    Returns a 2D or 3D plot view object depending on the value of the `dim` parameter.
+    The returned object is of type `pg.PlotItem` for 2D views, or `pg.opengl.GLViewWidget` for 3D views.
+    """
     global WINDOW, VIEW
 
     initiate = False
 
     if VIEW is not None:
         if dim is None:
             return VIEW
@@ -154,15 +183,20 @@
     def clear(axes):
         global WINDOW, VIEW
         VIEW.setParent(None)
         # WINDOW.removeWidget(VIEW)
         VIEW = None
 
     @staticmethod
+    def add_subplot(dim=None, **kwargs):
+        return add_subplot(dim=dim, **kwargs)
+
+    @staticmethod
     def gca(dim=None, **kwargs):
+        warnings.warn("gca is deprecated, use add_suplot instead")
         return gca(dim=dim, **kwargs)
 
     @staticmethod
     def is_axes(obj):
         return isinstance(obj, (pg.PlotItem, pg.opengl.GLViewWidget))
 
     @staticmethod
@@ -185,14 +219,15 @@
         Use matplotlib conventions to retrieve a pg.ColorMap
 
         Examples:
             >>> import rna
             >>> rna.plotting.use('pyqtgraph')
             >>> from rna.plotting.backends.pyqtgraph import ApiBackendPyqtgraph
             >>> cm = ApiBackendPyqtgraph.get_cmap('viridis')
+            >>> rna.plotting.use('matplotlib')  # reset for test suite to start at default
         """
         import matplotlib.pyplot as plt
 
         plt_map = plt.get_cmap(cm_name)
         colors = plt_map.colors
         colors = [c + [1.0] for c in colors]
         positions = np.linspace(0, 1, len(colors))
@@ -380,13 +415,7 @@
                 "-",
             )
         p.save()
         p.translate(x3 + b_label.height(), y1 + 0.5 * (y2 - y1) - b_label.width() / 2)
         p.rotate(90)
         p.drawText(0.0, 0.0, str(self.label))
         p.restore()
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod()
```

## rna/plotting/core.py

```diff
@@ -6,21 +6,27 @@
 import abc
 import pickle
 import rna.pattern.backend
 import rna
 import rna.pattern.decorator
 
 
-def _get_axes_from_input(backend, *data, **kwargs):
+def _get_axes_from_input(backend: "ApiBackend", *data, **kwargs):
+    """
+    Args:
+        backend: backend providing add_subplot, axes_dim and is_axes callable
+    """
     # 'ax' is the standard in matplotlib, seaborn etc. Sometimes passed, e.g. seaborn.Pairgrid.map...
     ax = kwargs.pop("ax", None)
     # 'axes' is self explanatory as a variable while ax is too short
     axes = kwargs.pop("axes", None)
     if ax and axes:
         raise ValueError("Axes defined twice (ax and axes)")
+    else:
+        axes = axes or ax
     dim = kwargs.pop("dim", None)
 
     if data:
         if backend.is_axes(data[0]):
             if axes is not None and axes is not data[0]:
                 raise ValueError("Conflicting axes passed as arg and kwarg")
             axes = data[0]
@@ -28,61 +34,66 @@
 
     if axes and dim:
         if dim != backend.axes_dim(axes):
             raise ValueError(
                 "Axes dimension and dim argument in conflict:" f"{backend.dim} vs {dim}"
             )
     if axes is None:
-        axes = backend.gca(dim=dim)
+        axes = backend.add_subplot(dim=dim)
     return axes, data, kwargs
 
 
 # pylint:disable=invalid-name,too-few-public-methods
 class plot_signature(rna.pattern.decorator.Decorator):
     """
-    This is a decorator which ensures that you pass an axes instance either
-        as first argument
-    or
-        as keyword arugment axes=<axes instance>
-    and/or
-        you specify the dimension of the axes object ot be generated dim=<dimension>
-    This decorator is applicable to both functions and methods.
+    This decorator enforces a signature for plot methods and functions.
+    The wrapped callable must then satisfy the following signature:
 
-    These wraped function requires an axes object as first argument but may be used as if it would
-    not exist.
+    >>> import rna.plotting
+    >>> @rna.plotting.plot_signature
+    ... def plot_something(axes, *args, **kwargs):
+    ...     artist = axes.plot(*args, **kwargs)
+    ...     # usually it is a good idea to return the artist(s) but this is not enforced
+    ...     return artist, axes
 
-    Notes:
-        * Consider https://stackoverflow.com/a/60832711/6233888 to add a backend kwarg
+    And can given exemplary inputs
 
-    Examples:
-        >>> import rna
-        >>> def my_plot_function(axes):
-        ...     return axes
-        >>> my_decorated_plot_function = rna.plotting.plot_signature(my_plot_function)
-
-        >>> axes = rna.plotting.gca(2)
-
-        Use it without the axes and you have an axes at hand
-        >>> assert my_decorated_plot_function() == axes
-
-        You can also pass an axes explicit, both as first argument and as named kwarg
-        >>> assert my_decorated_plot_function(rna.plotting.gca()) == axes
-        >>> assert my_decorated_plot_function(axes=rna.plotting.gca()) == axes
-
-        Or you give the dimension of the axes
-        >>> type(my_decorated_plot_function(dim=3))
-        <class 'matplotlib.axes._subplots.Axes3DSubplot'>
+    >>> data = ([1, 2, 3], [4, 5, 6])
+    >>> kwargs = {'color': 'r'}
+
+    Can be called lazy (without explicit axes object)
+
+    >>> artist, axes = plot_something(*data, **kwargs)
+
+    where the dimension of the generated axes can be controlled by the `dim` kwarg
+
+    >>> artist, axes_2 = plot_something(*data, dim=2, **kwargs)
+
+    The returned axes are new ones
+
+    >>> assert axes is not axes_2
+
+    Or more pythonic (expicit is better than implicit) in the following ways:
+
+    >>> artist, axes_3 = plot_something(axes, *data, **kwargs)
+    >>> artist, axes_4 = plot_something(*data, axes=axes, **kwargs)
+    >>> artist, axes_5 = plot_something(*data, ax=axes, **kwargs)
+
+    The returned axes are the ones given
 
+    >>> assert axes is axes_3 is axes_4 is axes_5
 
     """
 
     def _wrap(self, this, func, *args, **kwargs):
-        if this is None:
-            this = rna.plotting
-        axes, data, kwargs = _get_axes_from_input(this, *args, **kwargs)
+        if isinstance(this, ApiBackend):
+            backend = this
+        else:
+            backend = Api().backend
+        axes, data, kwargs = _get_axes_from_input(backend, *args, **kwargs)
         return func(axes, *data, **kwargs)
 
 
 class PlotKwargsFunctions:
     """
     Collection of staticmethod functions acting on kwargs passed to a plotting method.
     This provides a standardized signature of plotting functions.
@@ -307,26 +318,26 @@
         As a functionality of the Backend/Strategy pattern the backend is instantiated at
         access time
         >>> backend = api.backend
         >>> assert not isinstance(backend, str)
         >>> assert isinstance(backend, ApiBackendMatplotlib)
 
         Default dimension of the axis is 2
-        >>> backend.axes_dim(backend.gca())
+        >>> backend.axes_dim(backend.add_subplot())
         2
 
         You can select the correct axes object with the dimension key
-        >>> axes = ApiBackendMatplotlib.gca(dim=3)
+        >>> axes = ApiBackendMatplotlib.add_subplot(dim=3)
         >>> backend.axes_dim(axes)
         3
 
         Switching the backend keeps the top level behaviour the same
         >>> api = rna.plotting.Api()
         >>> api.backend = 'pyqtgraph'
-        >>> api.backend.axes_dim(api.backend.gca(dim=2))
+        >>> api.backend.axes_dim(api.backend.add_subplot(dim=2))
         2
 
     """
 
     STRATEGY_MODULE_BASE = "rna.plotting.backends"
 
     @plot_signature
@@ -382,15 +393,15 @@
         <rna.plotting.backends.matplotlib.ApiBackendMatplotlib object at ...>
 
         To use plot, implement _plot
         >>> class Demo(Api):
         ...     def _plot(self, **kwargs):
         ...         self.set_style()
         ...         labels = kwargs.pop("labels", ["x (m)", "y (m)", "z (m)"])
-        ...         ax = self.gca()
+        ...         ax = self.add_subplot()
         ...         artist = self.plot_tensor(ax, self.data, **kwargs)
         ...         self.set_labels(ax, *labels)
         ...         return artist
         >>> demo = Demo()
 
         >>> artists = demo.plot(np.array([[1,1], [2,2]]), color='r')
         >>> _ = demo.set_legend(artists)
```

## rna/polymorphism.py

```diff
@@ -174,15 +174,15 @@
 
 class Plottable:  # pylint: disable=too-few-public-methods
     """
     Polymorphism for object which can be plotted
     The polymorphisms lies in the method name *plot' and the suggested kwargs for this method.
     """
 
-    def plot(self, **kwargs):
+    def plot(self, *args, **kwargs):
         """
         Args:
             **kwargs:
                 axes: Most fundamental object of the plotting backend e.g. matplotlib.pyplot.Axes
                     Ideally the plot method implements multiple backends which are automatically
                     selected on the basis of the axes object.
                 color: color to plot this object. This is to unify the various different signatures
```

## Comparing `rna-0.8.0.dist-info/METADATA` & `rna-0.9.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 Metadata-Version: 2.1
 Name: rna
-Version: 0.8.0
+Version: 0.9.0
 Summary: Basic and essential code building blocks of all pythons
 Home-page: https://gitlab.mpcdf.mpg.de/dboe/rna
 License: MIT
 Keywords: plotting, matplotlib, pyqtgraph, backend, logging, path, argparse
 Author: Daniel Böckenhoff
 Author-email: dboe@ipp.mpg.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: config
 Provides-Extra: pyqtgraph
 Requires-Dist: hydra_core ; extra == "config"
 Requires-Dist: matplotlib
-Requires-Dist: numpy
+Requires-Dist: numpy (>=1.22)
 Requires-Dist: omegaconf ; extra == "config"
 Requires-Dist: pathlib ; python_version < "3.10"
 Requires-Dist: pyopengl ; extra == "pyqtgraph"
 Requires-Dist: pyqt5 ; extra == "pyqtgraph"
 Requires-Dist: pyqtgraph ; extra == "pyqtgraph"
 Project-URL: Documentation, https://dboe.pages.mpcdf.de/rna
 Project-URL: Repository, https://gitlab.mpcdf.mpg.de/dboe/rna
 Description-Content-Type: text/x-rst
 
-=====================
 library documentation
 =====================
 
 ..
     [shields-start]
 
 .. pypi
@@ -69,42 +63,42 @@
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
 ..
     [shields-end]
 
 Overview
-========
+--------
 
 ..
     [overview-start]
 
 Basic and essential code building blocks of all pythons
 
 ..
     [overview-end]
 
 Licensed under the ``MIT License``
 
 Resources
----------
+~~~~~~~~~
 
 ..
     [resources-start]
 
 * Source code: https://gitlab.mpcdf.mpg.de/dboe/rna
 * Documentation: https://dboe.pages.mpcdf.de/rna
 * Pypi: https://pypi.python.org/pypi/rna
 
 ..
     [resources-end]
 
 
 Features
---------
+~~~~~~~~
 
 ..
     [features-start]
 
 The following features should be highlighted:
 
 * TODO
```

## Comparing `rna-0.8.0.dist-info/LICENSE.rst` & `rna-0.9.0.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `rna-0.8.0.dist-info/RECORD` & `rna-0.9.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-rna/__init__.py,sha256=0U6Dptdi-OaOEYlXTRZS4SKqxCF2zH5ZgyJ4r_0G71U,369
+rna/__init__.py,sha256=IK63QIBIHaTQfZpqBkq6Mx2cEq6wF0CSYQJZZPVrXVQ,376
 rna/__main__.py,sha256=mtR-Xm1t-spFY94Z8EpzL0oIhIVMN1WdaTgjcx_AnFM,2043
-rna/config.py,sha256=q__zCyzFa12tdwOc8GBEuRnOsGgmL2_bdjkL_7AAPow,8094
+rna/config.py,sha256=RPGXlV5yODiMLktw7-618pno05LaeTyQhP5QT0-6h1I,9662
 rna/log.py,sha256=44uVamGRBYXLeLk9v3Ra4p4S-S3O_JGgxbBLXhfk-QE,3719
 rna/parsing.py,sha256=h6EQhKH5fZwrPrLmXuacNPtvZahsRv3oyzZtvJdNGw8,1970
 rna/path.py,sha256=8fwHnga4To1aMpfhveXgClRBx6iwKyZIbSzY1_aih58,6313
 rna/pattern/__init__.py,sha256=tQQs3jkLfEcHS3SDjgT0r6pgg6Y9nkcdYl_EwkfT0qI,71
 rna/pattern/backend.py,sha256=Na3IQgNGd3YzzJiUitVdfAmoxPD58eUDCZjjlRWVGaM,502
 rna/pattern/composite.py,sha256=ueA6LLIaGaE9cp6Hn9jrAVSVmEK0ZZ1ik-0Z0RuiDrU,13029
 rna/pattern/decorator.py,sha256=fa8-UzUE_AH_3F4-4zbYHIjTj2uHNG_mlAyQ9mAHJNk,9003
 rna/pattern/link.py,sha256=x4y44gfM7lxw5xRQL7-0_nAYFdclo8j2kta9SK1lUcY,5951
 rna/pattern/singleton.py,sha256=gRGqbte5-wH4Lux6cfwtm86pftySSPyP7eLRjRNhm54,977
 rna/pattern/strategy.py,sha256=1SBw63pZr7vZqsqN_Px6ExzZpq5yZSbQKt6vd0eZGtc,9053
 rna/pattern/switch.py,sha256=GzCUj_R157F0fKi5rkZj-5eTnmGNKWU0B44BBB9GROc,1254
-rna/plotting/__init__.py,sha256=pXMCUoNpKH7A2fo1jYhqk6K1hnnkJb9EKa8s9MJefaw,3941
+rna/plotting/__init__.py,sha256=Ib5BL3YJOBjol_hq4HVRG-U-1B1Lt_0okbX1fI30Zqo,3921
 rna/plotting/backends/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rna/plotting/backends/matplotlib.py,sha256=k_0cQFRNJWcoH-uSazt8BXB9L4HMV9rNk4o9dk4mr4U,40524
-rna/plotting/backends/pyqtgraph.py,sha256=ZNTvrZ-NCzibtRlbuGx4xAnbkOQ8B1mylUr1I3tjtOc,11908
+rna/plotting/backends/matplotlib.py,sha256=b3pYIQJaoCNBEACnnFc5t2I9DrPFc5Hd4aIiWi-TK24,40615
+rna/plotting/backends/pyqtgraph.py,sha256=tx47uz4qTF-pNhF6BToB5n3iBNqaK9rmpyZ8Oog892g,12926
 rna/plotting/base.py,sha256=0t0ASto4HopJkg6NYQZ_pI7y-GyOCLtsiTHRwGIuKvY,33
 rna/plotting/colors.py,sha256=v3RtCivheLK-QglCldgfPvHJaPt7ieL5WVoqOR-ykOw,11330
-rna/plotting/core.py,sha256=YD8CeOYWqSKyFlUrtApxKgtQNt7kTmdpPosgX2_INV8,16863
+rna/plotting/core.py,sha256=yG8CyweilglbF51Oo813OrNjdCxx_pc56yUFzG_d1vw,17074
 rna/plotting/mplstyles/rna.mplstyle,sha256=zn1pP0FdZWpx1tBzqxYhF78LYuAdODfnds6BOhKiaGQ,35834
 rna/plotting/mplstyles/tfields.mplstyle,sha256=_v2BEgmVHXRpwMAFO5vbzdGkmXywgUWPcX7hQbleBLk,1020
-rna/polymorphism.py,sha256=Yc9IZBweuh46QC--TdR_WjW-uS3Hq3vwoiQoACbu_o0,6856
+rna/polymorphism.py,sha256=vhueh7euBhX4cqVuGJtV6UD0_7krzVUOOnv262gqDVQ,6863
 rna/process.py,sha256=Sfx_2duhfRx5dBNVDq5xLbmrBrH8J5AjyL0a4jjvKes,3310
-rna-0.8.0.dist-info/METADATA,sha256=QeRrUF2GSxjEsbuRFL7ASQlCL0Ff6h4FVaFE13KZMwI,3178
-rna-0.8.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-rna-0.8.0.dist-info/LICENSE.rst,sha256=dHQrFF0bnLAGSkUSft19a0uglZwuUv5dryNMHAk893o,1076
-rna-0.8.0.dist-info/RECORD,,
+rna-0.9.0.dist-info/LICENSE.rst,sha256=dHQrFF0bnLAGSkUSft19a0uglZwuUv5dryNMHAk893o,1076
+rna-0.9.0.dist-info/METADATA,sha256=PchnmCqPjHlBC6YRLELq5XXj_CMilwsRdhSvjUQXJ5w,2916
+rna-0.9.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+rna-0.9.0.dist-info/RECORD,,
```

