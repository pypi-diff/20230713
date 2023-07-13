# Comparing `tmp/colortool-0.4.3.tar.gz` & `tmp/colortool-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colortool-0.4.3.tar", last modified: Sat Apr 29 11:02:44 2023, max compression
+gzip compressed data, was "colortool-0.4.4.tar", last modified: Thu Jul 13 16:32:41 2023, max compression
```

## Comparing `colortool-0.4.3.tar` & `colortool-0.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:02:44.950162 colortool-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 11:02:44.950162 colortool-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-29 11:02:31.000000 colortool-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:02:44.950162 colortool-0.4.3/colortool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-29 11:02:44.000000 colortool-0.4.3/colortool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-29 11:02:44.000000 colortool-0.4.3/colortool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:02:44.000000 colortool-0.4.3/colortool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 11:02:44.000000 colortool-0.4.3/colortool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 11:02:44.000000 colortool-0.4.3/colortool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-29 11:02:31.000000 colortool-0.4.3/colortool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 11:02:31.000000 colortool-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 11:02:44.950162 colortool-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:32:41.238360 colortool-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-13 16:32:41.238360 colortool-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-13 16:32:23.000000 colortool-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:32:41.238360 colortool-0.4.4/colortool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-13 16:32:41.000000 colortool-0.4.4/colortool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 16:32:41.000000 colortool-0.4.4/colortool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:32:41.000000 colortool-0.4.4/colortool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 16:32:41.000000 colortool-0.4.4/colortool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:32:41.000000 colortool-0.4.4/colortool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-13 16:32:23.000000 colortool-0.4.4/colortool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-13 16:32:23.000000 colortool-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:32:41.238360 colortool-0.4.4/setup.cfg
```

### Comparing `colortool-0.4.3/PKG-INFO` & `colortool-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortool
-Version: 0.4.3
+Version: 0.4.4
 Summary: set of tools to work with different color formats
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/colortool
 Project-URL: issues, https://tandav.github.io/colortool/issues
 Project-URL: release notes, https://tandav.github.io/colortool/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -60,15 +60,15 @@
 'rgba(0, 255, 0, 0.5)'
 
 ```
 
 ```python
 ### convert RGBA color on RGB background to RGB color
 >>> Color.from_background_and_color_alpha(
-...     background=Color.from_hex(0x00FF00),
+...     background=Color(0x00FF00),
 ...     color=Color(0x000000,alpha=0.5),
 ... )
 Color(0x007F00)
 
 ```
 
 ### make color darker or lighter
@@ -77,16 +77,16 @@
 Color(0x007F00)
 >>> green.lighter(ratio=0.5) # lightness = lightness + (1 - lightness) * ratio
 Color(0x7FFF7F)
 
 ```
 ###  [determine the font color to be either black or white depending on the background color](https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/)
 ```python
->>> white = Color.from_hex(0xFFFFFF)
->>> black = Color.from_hex(0x000000)
+>>> white = Color(0xFFFFFF)
+>>> black = Color(0x000000)
 >>> white.font_color()
 Color(0x000000)
 >>> black.font_color()
 Color(0xFFFFFF)
 >>> green.font_color()
 Color(0x000000)
```

### Comparing `colortool-0.4.3/README.md` & `colortool-0.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 'rgba(0, 255, 0, 0.5)'
 
 ```
 
 ```python
 ### convert RGBA color on RGB background to RGB color
 >>> Color.from_background_and_color_alpha(
-...     background=Color.from_hex(0x00FF00),
+...     background=Color(0x00FF00),
 ...     color=Color(0x000000,alpha=0.5),
 ... )
 Color(0x007F00)
 
 ```
 
 ### make color darker or lighter
@@ -65,16 +65,16 @@
 Color(0x007F00)
 >>> green.lighter(ratio=0.5) # lightness = lightness + (1 - lightness) * ratio
 Color(0x7FFF7F)
 
 ```
 ###  [determine the font color to be either black or white depending on the background color](https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/)
 ```python
->>> white = Color.from_hex(0xFFFFFF)
->>> black = Color.from_hex(0x000000)
+>>> white = Color(0xFFFFFF)
+>>> black = Color(0x000000)
 >>> white.font_color()
 Color(0x000000)
 >>> black.font_color()
 Color(0xFFFFFF)
 >>> green.font_color()
 Color(0x000000)
```

### Comparing `colortool-0.4.3/colortool.egg-info/PKG-INFO` & `colortool-0.4.4/colortool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colortool
-Version: 0.4.3
+Version: 0.4.4
 Summary: set of tools to work with different color formats
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/colortool
 Project-URL: issues, https://tandav.github.io/colortool/issues
 Project-URL: release notes, https://tandav.github.io/colortool/releases
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -60,15 +60,15 @@
 'rgba(0, 255, 0, 0.5)'
 
 ```
 
 ```python
 ### convert RGBA color on RGB background to RGB color
 >>> Color.from_background_and_color_alpha(
-...     background=Color.from_hex(0x00FF00),
+...     background=Color(0x00FF00),
 ...     color=Color(0x000000,alpha=0.5),
 ... )
 Color(0x007F00)
 
 ```
 
 ### make color darker or lighter
@@ -77,16 +77,16 @@
 Color(0x007F00)
 >>> green.lighter(ratio=0.5) # lightness = lightness + (1 - lightness) * ratio
 Color(0x7FFF7F)
 
 ```
 ###  [determine the font color to be either black or white depending on the background color](https://css-tricks.com/switch-font-color-for-different-backgrounds-with-css/)
 ```python
->>> white = Color.from_hex(0xFFFFFF)
->>> black = Color.from_hex(0x000000)
+>>> white = Color(0xFFFFFF)
+>>> black = Color(0x000000)
 >>> white.font_color()
 Color(0x000000)
 >>> black.font_color()
 Color(0xFFFFFF)
 >>> green.font_color()
 Color(0x000000)
```

### Comparing `colortool-0.4.3/colortool.py` & `colortool-0.4.4/colortool.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import math
 import random
 import string
 import typing as tp
 
 from dsplib.scale import minmax_scaler
 
-__version__ = '0.4.3'
+__version__ = '0.4.4'
 
 Float3 = tp.Tuple[float, float, float]
 Float4 = tp.Tuple[float, float, float, float]
 Int3 = tp.Tuple[int, int, int]
 Int4 = tp.Tuple[int, int, int, int]
 Int3Float = tp.Tuple[int, int, int, float]
 
@@ -25,20 +25,44 @@
 class Color:
     """
     supported formats:
     hex, css_hex, rgb_int, rgb_float, hls
     """
 
     def __init__(self, color: int, alpha: float | None = None):
+        self.color = color
+        self.alpha = alpha
+
+    @property
+    def color(self) -> int:
+        return self._color
+
+    @color.setter
+    def color(self, color: int) -> None:
         if not 0 <= color <= 0xFFFFFF:
             raise ValueError('color must be in range [0, 0xFFFFFF]')
+        self._color = color
+
+    @color.getter
+    def color(self) -> int:
+        return self._color
+
+    @property
+    def alpha(self) -> float | None:
+        return self._alpha
+
+    @alpha.setter
+    def alpha(self, alpha: float | None) -> None:
         if alpha is not None and not 0 <= alpha <= 1:
             raise ValueError('alpha must be in range [0, 1]')
-        self.color = color
-        self.alpha = alpha
+        self._alpha = alpha
+
+    @alpha.getter
+    def alpha(self) -> float | None:
+        return self._alpha
 
     def __repr__(self) -> str:
         if self.alpha is None:
             return f'Color(0x{self.color:06X})'
         return f'Color(0x{self.color:06X}, alpha={self.alpha})'
 
     def __eq__(self, other: object) -> bool:
```

### Comparing `colortool-0.4.3/pyproject.toml` & `colortool-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "colortool"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "set of tools to work with different color formats"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
@@ -29,15 +29,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.4.3"
+current_version = "v0.4.4"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

