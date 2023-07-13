# Comparing `tmp/bipl-0.3.2.tar.gz` & `tmp/bipl-0.3.3.tar.gz`

## Comparing `bipl-0.3.2.tar` & `bipl-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/_env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    14028 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/io/_util.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.3.2/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.2/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.2/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.2/hatch_build.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 bipl-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 bipl-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 bipl-0.3.3/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.3.3/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.3.3/hatch_build.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 bipl-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 bipl-0.3.3/PKG-INFO
```

### Comparing `bipl-0.3.2/src/bipl/io/__init__.py` & `bipl-0.3.3/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/io/_dzi.py` & `bipl-0.3.3/src/bipl/io/_dzi.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         qtag = {
             'jpeg': cv2.IMWRITE_JPEG_QUALITY,
             'webp': cv2.IMWRITE_WEBP_QUALITY,
         }.get(self.fmt)
         if qtag is None:
             raise RuntimeError(f'Unknown format: {self.fmt}')
 
-        bgr = rgb[..., ::-1]
+        bgr = cv2.cvtColor(rgb, cv2.COLOR_RGB2BGR)
         _, data = cv2.imencode(f'.{self.fmt}', bgr, [qtag, self.quality])
         return data.tobytes()
```

### Comparing `bipl-0.3.2/src/bipl/io/_gdal.py` & `bipl-0.3.3/src/bipl/io/_gdal.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/io/_libs.py` & `bipl-0.3.3/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/io/_openslide.py` & `bipl-0.3.3/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/io/_slide.py` & `bipl-0.3.3/src/bipl/io/_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 __all__ = ['Slide']
 
 import os
 from bisect import bisect_right
 from pathlib import Path
 from typing import final
+from warnings import warn
 
 import cv2
 import numpy as np
 from glow import memoize, shared_call, weak_memoize
 
 from bipl import env
 
@@ -20,14 +21,24 @@
 # TODO: inside Slide.open import ._slide.registry,
 # TODO: and in ._slide.registry do registration and DLL loading
 # TODO: to make Slide export not require DLL presence
 
 try:
     from ._gdal import Gdal
 except ImportError:
+    if not os.getenv('_BIPL_GDAL_NO_WARN'):
+        msg = 'No GDAL is available. Please '
+        if os.name == 'nt':
+            msg += ('acquire it manually from '
+                    'https://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal ')
+        else:
+            msg += ('install libgdal via your system package manager, '
+                    'and run "pip install gdal==`gdal-config --version`"')
+        warn(msg, stacklevel=1)
+        os.environ['_BIPL_GDAL_NO_WARN'] = '1'
     Gdal = None  # type: ignore[assignment,misc]
 
 _drv: type[Driver] | None
 for _drv, _regex in [  # LIFO, last driver takes priority
     (Gdal, r'^.*\.(tif|tiff)$'),
     (Openslide, r'^.*\.(bif|mrxs|ndpi|scn|svs|svsslide|tif|tiff|vms|vmu)$'),
     (Tiff, r'^.*\.(svs|tif|tiff)$'),
```

### Comparing `bipl-0.3.2/src/bipl/io/_slide_bases.py` & `bipl-0.3.3/src/bipl/io/_slide_bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
             # TODO: round/ceil/floor ?
             slice(round(s.start / self.scale), round(s.stop / self.scale))
             for s in slices
         ],
         # TODO: read base part-by-part, not all at once, if scale > 2(?)
         image = self.base[src_slices]
 
-        shape = *((s.stop - s.start) for s in slices),
-        return cv2.resize(image, shape[::-1], interpolation=cv2.INTER_AREA)
+        h, w = ((s.stop - s.start) for s in slices)
+        return cv2.resize(image, (w, h), interpolation=cv2.INTER_AREA)
 
 
 class Driver:
     @final
     @classmethod
     def register(cls, regex: str):
         """Registers type builder for extensions. Last call takes precedence"""
```

### Comparing `bipl-0.3.2/src/bipl/io/_tiff.py` & `bipl-0.3.3/src/bipl/io/_tiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,50 +201,51 @@
 
 
 # -------------------- item, lod & opener implementations --------------------
 @dataclass(frozen=True)
 class _ItemBase(Item):
     index: int
     tiff: Tiff
-    head: list[str]
-    meta: dict[str, str]  # unused
-    vendor: str
-    color: _ColorInfo
-    bg_color: np.ndarray
-    compression: _Compression
-    jpt: bytes = field(repr=False)
 
 
 @dataclass(frozen=True)
 class _Item(_ItemBase):
+    head: list[str]
+    vendor: str
+
     @property
     def key(self) -> str | None:
         if self.vendor == 'aperio' and self.index == 1:
             return 'thumbnail'
         for key in ('label', 'macro'):
             if any(key in s for s in self.head):
                 return key
         return None
 
     def __array__(self) -> np.ndarray:
         h, w = self.shape[:2]
-        bgra = np.empty((h, w, 4), dtype='u1')
+        rgba = np.empty((h, w, 4), dtype='u1')
 
         with self.tiff.ifd(self.index) as ptr:
-            ok = TIFF.TIFFReadRGBAImage(ptr, w, h, c_void_p(bgra.ctypes.data),
-                                        0)
+            ok = TIFF.TIFFReadRGBAImageOriented(ptr, w, h,
+                                                c_void_p(rgba.ctypes.data), 1,
+                                                0)
             assert ok
 
-        bgra = cv2.cvtColor(bgra, cv2.COLOR_mRGBA2RGBA)
+        rgba = cv2.cvtColor(rgba, cv2.COLOR_mRGBA2RGBA)
         # TODO: do we need to use bg_color to fill points where alpha = 0 ?
-        return bgra[..., 2::-1]
+        return rgba[..., :3]
 
 
 @dataclass(frozen=True)
 class _Lod(Lod, _ItemBase):
+    color: _ColorInfo
+    bg_color: np.ndarray
+    compression: _Compression
+    jpt: bytes = field(repr=False)
     tile: tuple[int, ...]
     tile_sizes: np.ndarray = field(repr=False)
 
     def _get_tile(self, y, x, ptr) -> SupportsArray:
         offset = TIFF.TIFFComputeTile(ptr, x, y, 0, 0)
         nbytes = int(self.tile_sizes[offset])
 
@@ -397,16 +398,15 @@
         # Whole level shape
         shape = (*tags.image_size, tags.spp)
         if len(shape) != 3:
             raise ValueError(f'Bad shape in TIFF: {shape}')
 
         # Tile shape, if applicable
         if not TIFF.TIFFIsTiled(self._ptr):  # Not yet supported
-            return _Item(shape, index, self, head, meta, vendor, tags.color,
-                         bg_color, tags.compression, jpt)
+            return _Item(shape, index, self, head, vendor)
 
         # Tile sizes
         tile = (*tags.tile_size, tags.spp)
         if len(tile) != 3:
             raise ValueError(f'Bad tile shape in TIFF: {tile}')
 
         tbc = np.empty([], 'u8')
@@ -414,13 +414,13 @@
         if TIFF.TIFFGetField(self._ptr, _Tag.TILE_BYTE_COUNTS, byref(tbc_ptr)):
             num_tiles = TIFF.TIFFNumberOfTiles(self._ptr)
             tbc = np.ctypeslib.as_array(tbc_ptr, [num_tiles]).copy()
             # TIFF._TIFFfree(tbc_ptr)  # TODO: ensure no segfault
             if (tbc == 0).any():
                 raise ValueError('Found 0s in tile size table')
 
-        return _Lod(shape, index, self, head, meta, vendor, tags.color,
-                    bg_color, tags.compression, jpt, spacing, tile, tbc)
+        return _Lod(shape, index, self, spacing, tags.color, bg_color,
+                    tags.compression, jpt, tile, tbc)
 
     def __getitem__(self, index: int) -> Item:
         with self.ifd(index):
             return self._get(index)
```

### Comparing `bipl-0.3.2/src/bipl/io/_util.py` & `bipl-0.3.3/src/bipl/io/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/ops/_mosaic.py` & `bipl-0.3.3/src/bipl/ops/_mosaic.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/src/bipl/ops/_util.py` & `bipl-0.3.3/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/LICENSE` & `bipl-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/README.md` & `bipl-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/hatch_build.py` & `bipl-0.3.3/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.3.2/pyproject.toml` & `bipl-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.3.2"
+version = "0.3.3"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -35,15 +35,15 @@
 ]
 
 dependencies = [
     "glow~=0.12.7",
     "imagecodecs",
     "lxml",
     "numpy~=1.21",
-    "opencv-python~=4.0",
+    "opencv-python-headless~=4.0",
     "pydantic~=1.2",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 gdal = [
     # For Windows, pick GDAL from here https://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal and install manually
```

### Comparing `bipl-0.3.2/PKG-INFO` & `bipl-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.3.2
+Version: 0.3.3
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
@@ -37,15 +37,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: glow~=0.12.7
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
 Requires-Dist: numpy~=1.21
-Requires-Dist: opencv-python~=4.0
+Requires-Dist: opencv-python-headless~=4.0
 Requires-Dist: pydantic~=1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: bipl[dev-core]; extra == 'dev'
 Requires-Dist: flake8-alphabetize; extra == 'dev'
 Requires-Dist: typing-extensions~=4.6; extra == 'dev'
 Provides-Extra: dev-core
```

