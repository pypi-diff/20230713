# Comparing `tmp/wbDefcon-0.2.0.tar.gz` & `tmp/wbDefcon-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbDefcon-0.2.0.tar", last modified: Sun Jul  2 11:38:42 2023, max compression
+gzip compressed data, was "wbDefcon-0.2.2.tar", last modified: Thu Jul 13 09:49:35 2023, max compression
```

## Comparing `wbDefcon-0.2.0.tar` & `wbDefcon-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.018734 wbDefcon-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.010734 wbDefcon-0.2.0/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.012734 wbDefcon-0.2.0/Lib/wbDefcon/
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.013734 wbDefcon-0.2.0/Lib/wbDefcon/misc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/misc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6556 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/misc/glyphnamelist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.017734 wbDefcon-0.2.0/Lib/wbDefcon/objects/
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/color.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/component.py
--rw-rw-rw-   0 root         (0) root         (0)     5061 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/contour.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/dataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/features.py
--rw-rw-rw-   0 root         (0) root         (0)    10214 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/font.py
--rw-rw-rw-   0 root         (0) root         (0)    10367 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     5134 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/image.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/imageSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/info.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     3605 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/layerSet.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/point.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/objects/uniData.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.018734 wbDefcon-0.2.0/Lib/wbDefcon/pens/
--rw-rw-rw-   0 root         (0) root         (0)    10025 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/pens/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/pens/lineIntersectionPen.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/pens/marginPen.py
--rw-rw-rw-   0 root         (0) root         (0)    25654 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/pens/outlineTestPen.py
--rw-rw-rw-   0 root         (0) root         (0)     4228 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/pens/pointPen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.018734 wbDefcon-0.2.0/Lib/wbDefcon/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3050 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/tools/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/tools/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/tools/representations.py
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/Lib/wbDefcon/undomanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 11:38:42.013734 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-02 11:38:41.000000 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-02 11:38:42.000000 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 11:38:41.000000 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-07-02 11:38:41.000000 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-02 11:38:41.000000 wbDefcon-0.2.0/Lib/wbDefcon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-02 11:38:42.018734 wbDefcon-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-07-02 11:38:42.019734 wbDefcon-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-02 11:38:40.000000 wbDefcon-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.714314 wbDefcon-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.706314 wbDefcon-0.2.2/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.707314 wbDefcon-0.2.2/Lib/wbDefcon/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.709314 wbDefcon-0.2.2/Lib/wbDefcon/misc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/misc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6556 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/misc/glyphnamelist.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.712314 wbDefcon-0.2.2/Lib/wbDefcon/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/color.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     5061 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/dataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1799 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/features.py
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/font.py
+-rw-rw-rw-   0 root         (0) root         (0)    10367 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     5134 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/imageSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/layerSet.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/point.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/objects/uniData.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.713314 wbDefcon-0.2.2/Lib/wbDefcon/pens/
+-rw-rw-rw-   0 root         (0) root         (0)    10025 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/pens/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/pens/lineIntersectionPen.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/pens/marginPen.py
+-rw-rw-rw-   0 root         (0) root         (0)    25654 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/pens/outlineTestPen.py
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/pens/pointPen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.714314 wbDefcon-0.2.2/Lib/wbDefcon/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/tools/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/tools/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/tools/representations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/Lib/wbDefcon/undomanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:49:35.708314 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-13 09:49:35.000000 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-07-13 09:49:35.000000 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:49:35.000000 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-13 09:49:35.000000 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 09:49:35.000000 wbDefcon-0.2.2/Lib/wbDefcon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-13 09:49:35.714314 wbDefcon-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-07-13 09:49:35.715314 wbDefcon-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-13 09:49:34.000000 wbDefcon-0.2.2/setup.py
```

### Comparing `wbDefcon-0.2.0/LICENSE` & `wbDefcon-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/__init__.py` & `wbDefcon-0.2.2/Lib/wbDefcon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A set of objects that are suited to being the basis
 of the UFO-Workbench tool. This works on UFO files.
 """
-__version__ = "0.2.0"
+__version__ = "0.2.2"
 
 from defcon import registerRepresentationFactory, unregisterRepresentationFactory
 
 from .objects.font import Font
 from .objects.layerSet import LayerSet
 from .objects.layer import Layer
 from .objects.glyph import Glyph
```

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/misc/glyphnamelist.py` & `wbDefcon-0.2.2/Lib/wbDefcon/misc/glyphnamelist.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/anchor.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/anchor.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/color.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/color.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/component.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/component.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/contour.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/contour.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/features.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/features.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/font.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             glyphContourClass=Contour,
             glyphPointClass=Point,
             glyphComponentClass=Component,
             glyphAnchorClass=Anchor,
             glyphImageClass=Image,
         )
         self._doc: Optional[UfoDocument] = None
-        if not self._ufoFormatVersion:
+        if not isinstance(self._ufoFormatVersion, UFOFormatVersion):
             self._ufoFormatVersion = UFOFormatVersion.FORMAT_3_0
         if not self._ufoFileStructure:
             self._ufoFileStructure = UFOFileStructure.ZIP
 
     def __repr__(self) -> str:
         return f"<wbDefcon Font at 0x{id(self):04X}>"
 
@@ -122,15 +122,15 @@
         implement custom saving behavior.
         """
         # if not format version is given, use the existing.
         # if that doesn't exist, go to 3.
         if formatVersion is None:
             formatVersion = self._ufoFormatVersion[0]
         if formatVersion is None:
-            formatVersion = 3
+            formatVersion = UFOFormatVersion.FORMAT_3_0
         if structure is None:
             structure = self._ufoFileStructure
         saveAll = structure == UFOFileStructure.ZIP
         if not self.path:
             saveAll = True
         elif path and os.path.realpath(path) != os.path.realpath(self.path):
             saveAll = True
```

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/glyph.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/glyph.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/groups.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/groups.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/guideline.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/guideline.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/image.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/image.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/info.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/info.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/kerning.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/kerning.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/layer.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/layer.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/layerSet.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/layerSet.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/objects/point.py` & `wbDefcon-0.2.2/Lib/wbDefcon/objects/point.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/pens/__init__.py` & `wbDefcon-0.2.2/Lib/wbDefcon/pens/__init__.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/pens/lineIntersectionPen.py` & `wbDefcon-0.2.2/Lib/wbDefcon/pens/lineIntersectionPen.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/pens/marginPen.py` & `wbDefcon-0.2.2/Lib/wbDefcon/pens/marginPen.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/pens/outlineTestPen.py` & `wbDefcon-0.2.2/Lib/wbDefcon/pens/outlineTestPen.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/pens/pointPen.py` & `wbDefcon-0.2.2/Lib/wbDefcon/pens/pointPen.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/tools/conversion.py` & `wbDefcon-0.2.2/Lib/wbDefcon/tools/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-anchor
+conversion
 ===============================================================================
 
 Convert private robofont attributes to UFO-3 format and back
 """
 
 from ..objects.guideline import Guideline
```

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/tools/glyph.py` & `wbDefcon-0.2.2/Lib/wbDefcon/tools/glyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 glyph
 ===============================================================================
 """
 import re
 
-from fontToolsTools.feature import renameGlyphInFeatureText
+from feaASTools.renameGlyph import renameGlyphInFeatureText
 
 digits = re.compile(r"^[0-9]*$")
 
 
 def renameGlyph(
     glyph,
     newName,
@@ -51,15 +51,16 @@
                 groups = font.groups
                 for groupName in [g for g in groups if oldName in groups[g]]:
                     groups[groupName] = [
                         newName if n == oldName else n for n in groups[groupName]
                     ]
             if inKerning:
                 kerning = font.kerning
-                for pair in kerning:
+                pairs = tuple(kerning.keys())
+                for pair in pairs:
                     if oldName in pair:
                         value = kerning.pop(pair)
                         newPair = tuple(newName if n == oldName else n for n in pair)
                         kerning[newPair] = value
             if inFeatures:
                 featureText = font.features.text
                 if featureText:
```

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/tools/representations.py` & `wbDefcon-0.2.2/Lib/wbDefcon/tools/representations.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon/undomanager.py` & `wbDefcon-0.2.2/Lib/wbDefcon/undomanager.py`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon.egg-info/PKG-INFO` & `wbDefcon-0.2.2/Lib/wbDefcon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbDefcon
-Version: 0.2.0
+Version: 0.2.2
 Summary: Defcon for Workbench applications.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbDefcon/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon/-/issues
```

### Comparing `wbDefcon-0.2.0/Lib/wbDefcon.egg-info/SOURCES.txt` & `wbDefcon-0.2.2/Lib/wbDefcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbDefcon-0.2.0/PKG-INFO` & `wbDefcon-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbDefcon
-Version: 0.2.0
+Version: 0.2.2
 Summary: Defcon for Workbench applications.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbDefcon/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbDefcon/-/issues
```

### Comparing `wbDefcon-0.2.0/setup.cfg` & `wbDefcon-0.2.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.0
+current_version = 0.2.2
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -59,14 +59,15 @@
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	defcon>=0.10.2
 	fontParts>=0.11.0
+	feaASTools>=0.2.2
 	wbBase>=0.2.2
 
 [options.packages.find]
 where = Lib
 
 [tox:tox]
 min_version = 4.6
```

