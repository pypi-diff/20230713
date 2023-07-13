# Comparing `tmp/Willow-1.5.1.tar.gz` & `tmp/willow-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Willow-1.5.1.tar", last modified: Thu Jul  6 16:05:40 2023, max compression
+gzip compressed data, was "willow-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `Willow-1.5.1.tar` & `willow-1.6.tar`

### file list

```diff
@@ -1,39 +1,23 @@
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.298329 Willow-1.5.1/
--rw-r--r--   0 dan        (503) staff       (20)     1545 2022-07-01 10:58:39.000000 Willow-1.5.1/LICENSE
--rw-r--r--   0 dan        (503) staff       (20)      101 2022-07-01 10:58:39.000000 Willow-1.5.1/MANIFEST.in
--rw-r--r--   0 dan        (503) staff       (20)      975 2023-07-06 16:05:40.298450 Willow-1.5.1/PKG-INFO
--rw-r--r--   0 dan        (503) staff       (20)     3679 2023-07-06 13:57:05.000000 Willow-1.5.1/README.rst
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.285569 Willow-1.5.1/Willow.egg-info/
--rw-r--r--   0 dan        (503) staff       (20)      975 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/PKG-INFO
--rw-r--r--   0 dan        (503) staff       (20)      687 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (503) staff       (20)        1 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (503) staff       (20)        1 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/not-zip-safe
--rw-r--r--   0 dan        (503) staff       (20)      135 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/requires.txt
--rw-r--r--   0 dan        (503) staff       (20)        7 2023-07-06 16:05:40.000000 Willow-1.5.1/Willow.egg-info/top_level.txt
--rw-r--r--   0 dan        (503) staff       (20)       70 2023-07-06 16:05:40.298784 Willow-1.5.1/setup.cfg
--rw-r--r--   0 dan        (503) staff       (20)     1783 2023-07-06 15:55:46.000000 Willow-1.5.1/setup.py
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.293784 Willow-1.5.1/tests/
--rw-r--r--   0 dan        (503) staff       (20)     6880 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_image.py
--rw-r--r--   0 dan        (503) staff       (20)     2161 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_opencv.py
--rw-r--r--   0 dan        (503) staff       (20)    14800 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_pillow.py
--rw-r--r--   0 dan        (503) staff       (20)    14576 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_registry.py
--rw-r--r--   0 dan        (503) staff       (20)     7326 2023-07-06 14:34:06.000000 Willow-1.5.1/tests/test_svg_coordinate_transforms.py
--rw-r--r--   0 dan        (503) staff       (20)    16612 2023-07-06 14:34:06.000000 Willow-1.5.1/tests/test_svg_image.py
--rw-r--r--   0 dan        (503) staff       (20)    13893 2023-07-06 13:57:05.000000 Willow-1.5.1/tests/test_wand.py
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.294914 Willow-1.5.1/willow/
--rw-r--r--   0 dan        (503) staff       (20)     6148 2023-07-04 23:07:06.000000 Willow-1.5.1/willow/.DS_Store
--rw-r--r--   0 dan        (503) staff       (20)     1331 2023-07-06 14:49:48.000000 Willow-1.5.1/willow/__init__.py
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.283385 Willow-1.5.1/willow/data/
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.295135 Willow-1.5.1/willow/data/cascades/
--rw-r--r--   0 dan        (503) staff       (20)   837462 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/data/cascades/haarcascade_frontalface_alt2.xml
--rw-r--r--   0 dan        (503) staff       (20)     6496 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/image.py
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.297843 Willow-1.5.1/willow/plugins/
--rw-r--r--   0 dan        (503) staff       (20)        0 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/plugins/__init__.py
--rw-r--r--   0 dan        (503) staff       (20)     3867 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/opencv.py
--rw-r--r--   0 dan        (503) staff       (20)     9081 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/pillow.py
--rw-r--r--   0 dan        (503) staff       (20)     6880 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/plugins/wand.py
--rw-r--r--   0 dan        (503) staff       (20)    12614 2023-07-06 13:57:05.000000 Willow-1.5.1/willow/registry.py
--rw-r--r--   0 dan        (503) staff       (20)    11803 2023-07-06 14:34:06.000000 Willow-1.5.1/willow/svg.py
-drwxr-xr-x   0 dan        (503) staff       (20)        0 2023-07-06 16:05:40.298069 Willow-1.5.1/willow/utils/
--rw-r--r--   0 dan        (503) staff       (20)        0 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/utils/__init__.py
--rw-r--r--   0 dan        (503) staff       (20)       61 2022-07-01 10:58:40.000000 Willow-1.5.1/willow/utils/deprecation.py
+-rw-r--r--   0        0        0     1545 2023-07-13 18:09:19.277441 willow-1.6/LICENSE
+-rw-r--r--   0        0        0      101 2023-07-13 18:09:19.281442 willow-1.6/MANIFEST.in
+-rw-r--r--   0        0        0     3686 2023-07-13 18:09:19.281442 willow-1.6/README.md
+-rw-r--r--   0        0        0     2810 2023-07-13 18:09:19.281442 willow-1.6/pyproject.toml
+-rw-r--r--   0        0        0     1703 2023-07-13 18:09:19.297442 willow-1.6/willow/__init__.py
+-rw-r--r--   0        0        0   837462 2023-07-13 18:09:19.301442 willow-1.6/willow/data/cascades/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0        0        0     9210 2023-07-13 18:09:19.301442 willow-1.6/willow/image.py
+-rw-r--r--   0        0        0      219 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/__init__.py
+-rw-r--r--   0        0        0     1615 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/base.py
+-rw-r--r--   0        0        0      947 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/cwebp.py
+-rw-r--r--   0        0        0      508 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/gifsicle.py
+-rw-r--r--   0        0        0      600 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/jpegoptim.py
+-rw-r--r--   0        0        0      535 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/optipng.py
+-rw-r--r--   0        0        0      648 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/pngquant.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/__init__.py
+-rw-r--r--   0        0        0     3787 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/opencv.py
+-rw-r--r--   0        0        0    12289 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/pillow.py
+-rw-r--r--   0        0        0     9276 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/wand.py
+-rw-r--r--   0        0        0    15273 2023-07-13 18:09:19.301442 willow-1.6/willow/registry.py
+-rw-r--r--   0        0        0    11803 2023-07-13 18:09:19.301442 willow-1.6/willow/svg.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:09:19.301442 willow-1.6/willow/utils/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-13 18:09:19.301442 willow-1.6/willow/utils/deprecation.py
+-rw-r--r--   0        0        0     5601 1970-01-01 00:00:00.000000 willow-1.6/PKG-INFO
```

### Comparing `Willow-1.5.1/LICENSE` & `willow-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Willow-1.5.1/willow/__init__.py` & `willow-1.6/willow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-from willow.image import Image
+from willow.image import Image  # noqa: F401
 
 
 def setup():
     from xml.etree import ElementTree
-    from willow.registry import registry
 
     from willow.image import (
+        AvifImageFile,
+        BMPImageFile,
+        GIFImageFile,
+        HeicImageFile,
         JPEGImageFile,
         PNGImageFile,
-        GIFImageFile,
-        BMPImageFile,
-        RGBImageBuffer,
         RGBAImageBuffer,
+        RGBImageBuffer,
+        SvgImageFile,
         TIFFImageFile,
         WebPImageFile,
-        SvgImageFile,
-        HeicImageFile,
     )
-    from willow.plugins import pillow, wand, opencv
+    from willow.optimizers import Cwebp, Gifsicle, Jpegoptim, Optipng, Pngquant
+    from willow.plugins import opencv, pillow, wand
+    from willow.registry import registry
     from willow.svg import SvgImage
 
     registry.register_image_class(JPEGImageFile)
     registry.register_image_class(PNGImageFile)
     registry.register_image_class(GIFImageFile)
     registry.register_image_class(BMPImageFile)
     registry.register_image_class(TIFFImageFile)
     registry.register_image_class(WebPImageFile)
     registry.register_image_class(HeicImageFile)
     registry.register_image_class(RGBImageBuffer)
     registry.register_image_class(RGBAImageBuffer)
     registry.register_image_class(SvgImageFile)
     registry.register_image_class(SvgImage)
+    registry.register_image_class(AvifImageFile)
 
     registry.register_plugin(pillow)
     registry.register_plugin(wand)
     registry.register_plugin(opencv)
 
+    registry.register_optimizer(Cwebp)
+    registry.register_optimizer(Gifsicle)
+    registry.register_optimizer(Jpegoptim)
+    registry.register_optimizer(Optipng)
+    registry.register_optimizer(Pngquant)
+
     # Prevents etree from prefixing XML tag names with anonymous
     # namespaces, e.g. "<ns0:svg ..."
     ElementTree.register_namespace("", "http://www.w3.org/2000/svg")
 
 
 setup()
 
 
-__version__ = "1.5.1"
+__version__ = "1.6"
```

### Comparing `Willow-1.5.1/willow/data/cascades/haarcascade_frontalface_alt2.xml` & `willow-1.6/willow/data/cascades/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `Willow-1.5.1/willow/plugins/opencv.py` & `willow-1.6/willow/plugins/opencv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 import os
 
 from willow.image import Image, RGBImageBuffer
 
 
 def _cv2():
     try:
@@ -11,14 +9,15 @@
     except ImportError:
         from cv import cv2
     return cv2
 
 
 def _numpy():
     import numpy
+
     return numpy
 
 
 class BaseOpenCVImage(Image):
     def __init__(self, image, size):
         self.image = image
         self.size = size
@@ -46,15 +45,15 @@
         # Animation is not supported by OpenCV
         return False
 
 
 class OpenCVColorImage(BaseOpenCVImage):
     @classmethod
     def check(cls):
-        super(OpenCVColorImage, cls).check()
+        super().check()
         _numpy()
 
     @classmethod
     @Image.converter_from(RGBImageBuffer)
     def from_buffer_rgb(cls, image_buffer):
         """
         Converts a Color Image buffer into a numpy array suitable for use with OpenCV
@@ -81,45 +80,53 @@
         """
         numpy = _numpy()
         cv2 = _cv2()
         points = cv2.goodFeaturesToTrack(self.image, 20, 0.04, 1.0)
         if points is None:
             return []
         else:
-            points = numpy.reshape(points, (-1, 2))  # Numpy returns it with an extra third dimension
+            points = numpy.reshape(
+                points, (-1, 2)
+            )  # Numpy returns it with an extra third dimension
             return points.tolist()
 
     @Image.operation
-    def detect_faces(self, cascade_filename='haarcascade_frontalface_alt2.xml'):
+    def detect_faces(self, cascade_filename="haarcascade_frontalface_alt2.xml"):
         """
         Run OpenCV face detection on the image. Returns a list of coordinates representing a box around each face.
         """
         cv2 = _cv2()
         cascade_filename = self._find_cascade(cascade_filename)
         cascade = cv2.CascadeClassifier(cascade_filename)
         equalised_image = cv2.equalizeHist(self.image)
-        faces = cascade.detectMultiScale(equalised_image,
-                                         self.face_haar_scale,
-                                         self.face_min_neighbors,
-                                         self.face_haar_flags,
-                                         self.face_min_size)
-        return [(face[0],
-                 face[1],
-                 face[0] + face[2],
-                 face[1] + face[3],
-                 ) for face in faces]
+        faces = cascade.detectMultiScale(
+            equalised_image,
+            self.face_haar_scale,
+            self.face_min_neighbors,
+            self.face_haar_flags,
+            self.face_min_size,
+        )
+        return [
+            (
+                face[0],
+                face[1],
+                face[0] + face[2],
+                face[1] + face[3],
+            )
+            for face in faces
+        ]
 
     def _find_cascade(self, cascade_filename):
         """
         Find the requested OpenCV cascade file.  If a relative path was provided, check local cascades directory.
         """
         if not os.path.isabs(cascade_filename):
             cascade_filename = os.path.join(
                 os.path.dirname(os.path.dirname(__file__)),
-                'data/cascades',
+                "data/cascades",
                 cascade_filename,
             )
         return cascade_filename
 
     @classmethod
     @Image.converter_from(OpenCVColorImage)
     def from_color(cls, colour_image):
```

### Comparing `Willow-1.5.1/willow/plugins/pillow.py` & `willow-1.6/willow/plugins/wand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,319 @@
-from __future__ import absolute_import
-
-try:
-    from pillow_heif import HeifImagePlugin
-except ImportError:
-    pass
+import functools
+from ctypes import c_char_p, c_void_p
 
 from willow.image import (
+    AvifImageFile,
+    BadImageOperationError,
+    BMPImageFile,
+    GIFImageFile,
+    HeicImageFile,
     Image,
     JPEGImageFile,
     PNGImageFile,
-    GIFImageFile,
-    BMPImageFile,
+    RGBAImageBuffer,
+    RGBImageBuffer,
     TIFFImageFile,
     WebPImageFile,
-    HeicImageFile,
-    RGBImageBuffer,
-    RGBAImageBuffer,
-    BadImageOperationError,
 )
 
-class UnsupportedRotation(Exception): pass
 
-def _PIL_Image():
-    import PIL.Image
-    return PIL.Image
+class UnsupportedRotation(Exception):
+    pass
+
+
+def _wand_image():
+    import wand.image
+
+    return wand.image
+
+
+def _wand_color():
+    import wand.color
+
+    return wand.color
+
+
+def _wand_api():
+    import wand.api
+
+    return wand.api
 
 
-class PillowImage(Image):
+def _wand_version():
+    import wand.version
+
+    return wand.version
+
+
+class WandImage(Image):
     def __init__(self, image):
         self.image = image
 
     @classmethod
     def check(cls):
-        _PIL_Image()
+        _wand_image()
+        _wand_color()
+        _wand_api()
+        _wand_version()
+
+    def _clone(self):
+        return WandImage(self.image.clone())
 
     @classmethod
     def is_format_supported(cls, image_format):
-        formats = _PIL_Image().registered_extensions()
-        return image_format in formats.values()
+        return bool(_wand_version().formats(image_format))
 
     @Image.operation
     def get_size(self):
         return self.image.size
 
     @Image.operation
     def get_frame_count(self):
-        # Animation is not supported by PIL
-        return 1
+        return len(self.image.sequence)
 
     @Image.operation
     def has_alpha(self):
-        img = self.image
-        return img.mode in ('RGBA', 'LA') or (img.mode == 'P' and 'transparency' in img.info)
+        return self.image.alpha_channel
 
     @Image.operation
     def has_animation(self):
-        # Animation is not supported by PIL
-        return False
+        return self.image.animation
 
     @Image.operation
     def resize(self, size):
-        # Convert 1 and P images to RGB to improve resize quality
-        # (palleted images don't get antialiased or filtered when minified)
-        if self.image.mode in ['1', 'P']:
-            if self.has_alpha():
-                image = self.image.convert('RGBA')
-            else:
-                image = self.image.convert('RGB')
-        else:
-            image = self.image
-
-        # LANCZOS was previously known as ANTIALIAS
-        return PillowImage(image.resize(size, _PIL_Image().Resampling.LANCZOS))
+        clone = self._clone()
+        clone.image.resize(size[0], size[1])
+        return clone
 
     @Image.operation
     def crop(self, rect):
         left, top, right, bottom = rect
         width, height = self.image.size
         if (
-            left >= right or left >= width
+            left >= right
+            or left >= width
             or right <= 0
-            or top >= bottom or top >= height
+            or top >= bottom
+            or top >= height
             or bottom <= 0
         ):
-            raise BadImageOperationError("Invalid crop dimensions: %r" % (rect,))
+            raise BadImageOperationError(f"Invalid crop dimensions: {rect!r}")
 
-        # clamp to image boundaries
-        clamped_rect = (
-            max(0, left),
-            max(0, top),
-            min(right, width),
-            min(bottom, height),
+        clone = self._clone()
+        clone.image.crop(
+            # clamp to image boundaries
+            left=max(0, left),
+            top=max(0, top),
+            right=min(right, width),
+            bottom=min(bottom, height),
         )
-
-        return PillowImage(self.image.crop(clamped_rect))
+        return clone
 
     @Image.operation
     def rotate(self, angle):
-        """
-        Accept a multiple of 90 to pass to the underlying Pillow function
-        to rotate the image.
-        """
-
-        Image = _PIL_Image()
-        ORIENTATION_TO_TRANSPOSE = {
-            90: Image.Transpose.ROTATE_90,
-            180: Image.Transpose.ROTATE_180,
-            270: Image.Transpose.ROTATE_270,
-        }
-
-        modulo_angle = angle % 360
-
-        # is we're rotating a multiple of 360, it's the same as a no-op
-        if not modulo_angle:
-            return self
-
-        transpose_code = ORIENTATION_TO_TRANSPOSE.get(modulo_angle)
+        not_a_multiple_of_90 = angle % 90
 
-        if not transpose_code:
+        if not_a_multiple_of_90:
             raise UnsupportedRotation(
                 "Sorry - we only support right angle rotations - i.e. multiples of 90 degrees"
             )
 
-        # We call "transpose", as it rotates the image,
-        # updating the height and width, whereas using 'rotate'
-        # only changes the contents of the image.
-        rotated = self.image.transpose(transpose_code)
-
-        return PillowImage(rotated)
+        clone = self.image.clone()
+        clone.rotate(angle)
+        return WandImage(clone)
 
     @Image.operation
     def set_background_color_rgb(self, color):
         if not self.has_alpha():
             # Don't change image that doesn't have an alpha channel
             return self
 
         # Check type of color
         if not isinstance(color, (tuple, list)) or not len(color) == 3:
             raise TypeError("the 'color' argument must be a 3-element tuple or list")
 
-        # Convert non-RGB colour formats to RGB
-        # As we only allow the background color to be passed in as RGB, we
-        # convert the format of the original image to match.
-        image = self.image.convert('RGBA')
-
-        # Generate a new image with background colour and draw existing image on top of it
-        # The new image must temporarily be RGBA in order for alpha_composite to work
-        new_image = _PIL_Image().new('RGBA', self.image.size, (color[0], color[1], color[2], 255))
-
-        if hasattr(new_image, 'alpha_composite'):
-            new_image.alpha_composite(image)
-        else:
-            # Pillow < 4.2.0 fallback
-            # This method may be slower as the operation generates a new image
-            new_image = _PIL_Image().alpha_composite(new_image, image)
-
-        return PillowImage(new_image.convert('RGB'))
-
-    @Image.operation
-    def save_as_jpeg(self, f, quality=85, optimize=False, progressive=False):
-        if self.image.mode in ['1', 'P']:
-            image = self.image.convert('RGB')
-        else:
-            image = self.image
-
-        # Pillow only checks presence of optimize kwarg, not its value
-        kwargs = {}
-        if optimize:
-            kwargs['optimize'] = True
-        if progressive:
-            kwargs['progressive'] = True
+        clone = self._clone()
+
+        # Wand will perform the compositing at the point of setting alpha_channel to 'remove'
+        clone.image.background_color = _wand_color().Color(
+            "rgb({}, {}, {})".format(*color)
+        )
+        clone.image.alpha_channel = "remove"
+
+        if clone.image.alpha_channel:
+            # ImageMagick <=6 fails to set alpha_channel to False, so do it manually
+            clone.image.alpha_channel = False
+
+        return clone
+
+    @Image.operation
+    def save_as_jpeg(
+        self,
+        f,
+        quality: int = 85,
+        progressive: bool = False,
+        apply_optimizers: bool = True,
+        **kwargs,
+    ):
+        """
+        Save the image as a JPEG file.
+
+        :param f: the file or file-like object to save to
+        :param quality: the image quality
+        :param progressive: whether to save as progressive JPEG file.
+        :param apply_optimizers: controls whether to run any configured optimizer libraries
+        :return: JPEGImageFile
+        """
+        with self.image.convert("pjpeg" if progressive else "jpeg") as converted:
+            converted.compression_quality = quality
+            converted.save(file=f)
 
-        image.save(f, 'JPEG', quality=quality, **kwargs)
+        if apply_optimizers:
+            self.optimize(f, "jpeg")
         return JPEGImageFile(f)
 
     @Image.operation
-    def save_as_png(self, f, optimize=False):
-        # Pillow only checks presence of optimize kwarg, not its value
-        kwargs = {}
-        if optimize:
-            kwargs['optimize'] = True
+    def save_as_png(self, f, apply_optimizers: bool = True, **kwargs):
+        """
+        Save the image as a PNG file.
+
+        :param f: the file or file-like object to save to
+        :param apply_optimizers: controls whether to run any configured optimizer libraries
+        :return: PNGImageFile
+        """
+        with self.image.convert("png") as converted:
+            converted.save(file=f)
 
-        self.image.save(f, 'PNG', **kwargs)
+        if apply_optimizers:
+            self.optimize(f, "png")
         return PNGImageFile(f)
 
     @Image.operation
-    def save_as_gif(self, f):
-        image = self.image
-
-        # All gif files use either the L or P mode but we sometimes convert them
-        # to RGB/RGBA to improve the quality of resizing. We must make sure that
-        # they are converted back before saving.
-        if image.mode not in ['L', 'P']:
-            image = image.convert('P', palette=_PIL_Image().Palette.ADAPTIVE)
-
-        if 'transparency' in image.info:
-            image.save(f, 'GIF', transparency=image.info['transparency'])
-        else:
-            image.save(f, 'GIF')
+    def save_as_gif(self, f, apply_optimizers: bool = True):
+        with self.image.convert("gif") as converted:
+            converted.save(file=f)
 
+        if apply_optimizers:
+            self.optimize(f, "gif")
         return GIFImageFile(f)
 
     @Image.operation
-    def save_as_webp(self, f, quality=80, lossless=False):
-        self.image.save(f, 'WEBP', quality=quality, lossless=lossless)
+    def save_as_webp(
+        self,
+        f,
+        quality: int = 80,
+        lossless: bool = False,
+        apply_optimizers: bool = True,
+    ):
+        """
+        Save the image as a WEBP file.
+
+        :param f: the file or file-like object to save to
+        :param quality: the image quality
+        :param lossless: whether to save as lossless WEBP file.
+        :param apply_optimizers: controls whether to run any configured optimizer libraries.
+            Note that when lossless=True, this will be ignored.
+        :return: WebPImageFile
+        """
+        with self.image.convert("webp") as converted:
+            if lossless:
+                library = _wand_api().library
+                library.MagickSetOption.argtypes = [c_void_p, c_char_p, c_char_p]
+                library.MagickSetOption(
+                    converted.wand,
+                    b"webp:lossless",
+                    b"true",
+                )
+            else:
+                converted.compression_quality = quality
+            converted.save(file=f)
+        if not lossless and apply_optimizers:
+            self.optimize(f, "webp")
         return WebPImageFile(f)
 
     @Image.operation
-    def save_as_heic(self, f, quality=80, lossless=False):
-        if lossless:
-            self.image.save(f, 'HEIF', quality=-1, chroma=444)
-        else:
-            self.image.save(f, 'HEIF', quality=quality)
-        return HeicImageFile(f)
+    def save_as_avif(self, f, quality=80, lossless=False, apply_optimizers=True):
+        with self.image.convert("avif") as converted:
+            if lossless:
+                converted.compression_quality = 100
+                library = _wand_api().library
+                library.MagickSetOption.argtypes = [c_void_p, c_char_p, c_char_p]
+                library.MagickSetOption(
+                    converted.wand,
+                    b"heic:lossless",
+                    b"true",
+                )
+            else:
+                converted.compression_quality = quality
+            converted.save(file=f)
+
+        if not lossless and apply_optimizers:
+            self.optimize(f, "avif")
+
+        return AvifImageFile(f)
 
     @Image.operation
     def auto_orient(self):
-        # JPEG files can be orientated using an EXIF tag.
-        # Make sure this orientation is applied to the data
         image = self.image
 
-        if hasattr(image, '_getexif'):
-            try:
-                exif = image._getexif()
-            except Exception:
-                # Blanket cover all the ways _getexif can fail in.
-                exif = None
-            if exif is not None:
-                # 0x0112 = Orientation
-                orientation = exif.get(0x0112, 1)
-
-                if 1 <= orientation <= 8:
-                    Image = _PIL_Image()
-                    ORIENTATION_TO_TRANSPOSE = {
-                        1: (),
-                        2: (Image.Transpose.FLIP_LEFT_RIGHT,),
-                        3: (Image.Transpose.ROTATE_180,),
-                        4: (Image.Transpose.ROTATE_180, Image.Transpose.FLIP_LEFT_RIGHT),
-                        5: (Image.Transpose.ROTATE_270, Image.Transpose.FLIP_LEFT_RIGHT),
-                        6: (Image.Transpose.ROTATE_270,),
-                        7: (Image.Transpose.ROTATE_90, Image.Transpose.FLIP_LEFT_RIGHT),
-                        8: (Image.Transpose.ROTATE_90,),
-                    }
+        if image.orientation not in ["top_left", "undefined"]:
+            image = image.clone()
+            if hasattr(image, "auto_orient"):
+                # Wand 0.4.1 +
+                image.auto_orient()
+            else:
+                orientation_ops = {
+                    "top_right": [image.flop],
+                    "bottom_right": [functools.partial(image.rotate, degree=180.0)],
+                    "bottom_left": [image.flip],
+                    "left_top": [
+                        image.flip,
+                        functools.partial(image.rotate, degree=90.0),
+                    ],
+                    "right_top": [functools.partial(image.rotate, degree=90.0)],
+                    "right_bottom": [
+                        image.flop,
+                        functools.partial(image.rotate, degree=90.0),
+                    ],
+                    "left_bottom": [functools.partial(image.rotate, degree=270.0)],
+                }
+                fns = orientation_ops.get(image.orientation)
+
+                if fns:
+                    for fn in fns:
+                        fn()
 
-                    for transpose in ORIENTATION_TO_TRANSPOSE[orientation]:
-                        image = image.transpose(transpose)
+                    image.orientation = "top_left"
 
-        return PillowImage(image)
+        return WandImage(image)
 
     @Image.operation
-    def get_pillow_image(self):
+    def get_wand_image(self):
         return self.image
 
     @classmethod
-    @Image.converter_from(JPEGImageFile)
-    @Image.converter_from(PNGImageFile)
-    @Image.converter_from(GIFImageFile, cost=200)
-    @Image.converter_from(BMPImageFile)
-    @Image.converter_from(TIFFImageFile)
-    @Image.converter_from(WebPImageFile)
-    @Image.converter_from(HeicImageFile)
+    @Image.converter_from(JPEGImageFile, cost=150)
+    @Image.converter_from(PNGImageFile, cost=150)
+    @Image.converter_from(GIFImageFile, cost=150)
+    @Image.converter_from(BMPImageFile, cost=150)
+    @Image.converter_from(TIFFImageFile, cost=150)
+    @Image.converter_from(WebPImageFile, cost=150)
+    @Image.converter_from(HeicImageFile, cost=150)
+    @Image.converter_from(AvifImageFile, cost=150)
     def open(cls, image_file):
         image_file.f.seek(0)
-        image = _PIL_Image().open(image_file.f)
-        image.load()
+        image = _wand_image().Image(file=image_file.f)
+        image.wand = _wand_api().library.MagickCoalesceImages(image.wand)
 
         return cls(image)
 
     @Image.converter_to(RGBImageBuffer)
     def to_buffer_rgb(self):
-        image = self.image
-
-        if image.mode != 'RGB':
-            image = image.convert('RGB')
-
-        return RGBImageBuffer(image.size, image.tobytes())
+        return RGBImageBuffer(self.image.size, self.image.make_blob("RGB"))
 
     @Image.converter_to(RGBAImageBuffer)
     def to_buffer_rgba(self):
-        image = self.image
-
-        if image.mode != 'RGBA':
-            image = image.convert('RGBA')
-
-        return RGBAImageBuffer(image.size, image.tobytes())
+        return RGBImageBuffer(self.image.size, self.image.make_blob("RGBA"))
 
 
-willow_image_classes = [PillowImage]
+willow_image_classes = [WandImage]
```

### Comparing `Willow-1.5.1/willow/registry.py` & `willow-1.6/willow/registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 from collections import defaultdict
+from typing import TYPE_CHECKING, List
+
+if TYPE_CHECKING:
+    from .optimizers import OptimizerBase
 
 
 class UnrecognisedOperationError(LookupError):
     """
     Raised when the operation isn't in any of the known image classes.
     """
+
     pass
 
 
 class UnavailableOperationError(LookupError):
     """
     Raised when all the image classes the operation exists in are not available.
     (most likely due to a missing image library.)
     """
+
     pass
 
 
 class UnroutableOperationError(LookupError):
     """
     Raised when there is no way to convert the image into an image class that
     supports the operation.
     """
+
     pass
 
 
-class WillowRegistry(object):
+class WillowRegistry:
     def __init__(self):
         self._registered_image_classes = set()
-        self._unavailable_image_classes = dict()
+        self._unavailable_image_classes = {}
         self._registered_operations = defaultdict(dict)
-        self._registered_converters = dict()
-        self._registered_converter_costs = dict()
+        self._registered_converters = {}
+        self._registered_converter_costs = {}
+        self._registered_optimizers: List["OptimizerBase"] = []
 
     def register_operation(self, image_class, operation_name, func):
         self._registered_operations[image_class][operation_name] = func
 
     def register_converter(self, from_image_class, to_image_class, func, cost=None):
         self._registered_converters[from_image_class, to_image_class] = func
 
@@ -43,87 +51,162 @@
 
     def register_image_class(self, image_class):
         self._registered_image_classes.add(image_class)
 
         # Check the image class
         try:
             image_class.check()
-        except Exception as e:
+        except Exception as e:  # noqa: BLE001
             self._unavailable_image_classes[image_class] = e
 
         # Find and register operations/converters
         for attr in dir(image_class):
             val = getattr(image_class, attr)
-            if hasattr(val, '_willow_operation'):
+            if hasattr(val, "_willow_operation"):
                 self.register_operation(image_class, val.__name__, val)
-            elif hasattr(val, '_willow_converter_to'):
-                self.register_converter(image_class, val._willow_converter_to[0], val, cost=val._willow_converter_to[1])
-            elif hasattr(val, '_willow_converter_from'):
+            elif hasattr(val, "_willow_converter_to"):
+                self.register_converter(
+                    image_class,
+                    val._willow_converter_to[0],
+                    val,
+                    cost=val._willow_converter_to[1],
+                )
+            elif hasattr(val, "_willow_converter_from"):
                 for converter_from, cost in val._willow_converter_from:
                     self.register_converter(converter_from, image_class, val, cost=cost)
 
     def register_plugin(self, plugin):
-        image_classes = getattr(plugin, 'willow_image_classes', [])
-        operations = getattr(plugin, 'willow_operations', [])
-        converters = getattr(plugin, 'willow_converters', [])
+        image_classes = getattr(plugin, "willow_image_classes", [])
+        operations = getattr(plugin, "willow_operations", [])
+        converters = getattr(plugin, "willow_converters", [])
 
         for image_class in image_classes:
             self.register_image_class(image_class)
 
         for operation in operations:
             self.register_operation(operation[0], operation[1], operation[2])
 
         for converter in converters:
             self.register_converter(converter[0], converter[1], converter[2])
 
+    def register_optimizer(self, optimizer_class: "OptimizerBase"):
+        """Registers an optimizer class."""
+        try:
+            # try to check Django settings, if used in that context
+            from django.conf import settings
+
+            enabled_optimizers = getattr(settings, "WILLOW_OPTIMIZERS", False)
+        except ImportError:
+            # fall back to env vars.
+            import os
+
+            enabled_optimizers = os.environ.get("WILLOW_OPTIMIZERS", False)
+
+        if not enabled_optimizers:
+            # WILLOW_OPTIMIZERS is either not set, or is set to a false-y value, so skip registration
+            return
+
+        if isinstance(enabled_optimizers, str):
+            if enabled_optimizers.lower() == "false":
+                return
+            elif enabled_optimizers.lower() == "true":
+                enabled_optimizers = True
+            else:
+                enabled_optimizers = enabled_optimizers.split(",")
+
+        if enabled_optimizers is True:
+            add_optimizer = True
+        else:
+            add_optimizer = optimizer_class.library_name in enabled_optimizers
+
+        if (
+            add_optimizer
+            and optimizer_class.check_library()
+            and optimizer_class not in self._registered_optimizers
+        ):
+            self._registered_optimizers.append(optimizer_class)
+
     def get_operation(self, image_class, operation_name):
         return self._registered_operations[image_class][operation_name]
 
     def operation_exists(self, operation_name):
         for image_class_operations in self._registered_operations.values():
             if operation_name in image_class_operations:
                 return True
 
         return False
 
     def get_converter(self, from_image_class, to_image_class):
         return self._registered_converters[from_image_class, to_image_class]
 
     def get_converter_cost(self, from_image_class, to_image_class):
-        return self._registered_converter_costs.get((from_image_class, to_image_class), 100)
+        return self._registered_converter_costs.get(
+            (from_image_class, to_image_class), 100
+        )
 
     def get_image_classes(self, with_operation=None, available=None):
         image_classes = self._registered_image_classes.copy()
 
         if with_operation:
-            image_classes = set(filter(lambda image_class: image_class in self._registered_operations and with_operation in self._registered_operations[image_class], image_classes))
+            image_classes = set(
+                filter(
+                    lambda image_class: image_class in self._registered_operations
+                    and with_operation in self._registered_operations[image_class],
+                    image_classes,
+                )
+            )
 
             if not image_classes:
-                raise UnrecognisedOperationError("Could not find image class with the '{0}' operation".format(with_operation))
+                raise UnrecognisedOperationError(
+                    "Could not find image class with the '{}' operation".format(
+                        with_operation
+                    )
+                )
 
         if available:
             # Remove unavailable image classes
-            available_image_classes = image_classes - set(self._unavailable_image_classes.keys())
+            available_image_classes = image_classes - set(
+                self._unavailable_image_classes.keys()
+            )
 
             # Raise error if all image classes failed the check
             if not available_image_classes:
-                raise UnavailableOperationError('\n'.join([
-                    "The operation '{0}' is available in the following image classes but they all raised errors:".format(with_operation)
-                ] + [
-                    "{image_class_name}: {error_message}".format(
-                        image_class_name=image_class.__name__,
-                        error_message=str(self._unavailable_image_classes.get(image_class, "Unknown error"))
+                raise UnavailableOperationError(
+                    "\n".join(
+                        [
+                            "The operation '{}' is available in the following image classes but they all raised errors:".format(
+                                with_operation
+                            )
+                        ]
+                        + [
+                            "{image_class_name}: {error_message}".format(
+                                image_class_name=image_class.__name__,
+                                error_message=str(
+                                    self._unavailable_image_classes.get(
+                                        image_class, "Unknown error"
+                                    )
+                                ),
+                            )
+                            for image_class in image_classes
+                        ]
                     )
-                    for image_class in image_classes
-                ]))
+                )
 
             return available_image_classes
         else:
             return image_classes
 
+    def get_optimizers_for_format(self, image_format: str) -> List["OptimizerBase"]:
+        optimizers = []
+        for optimizer in self._registered_optimizers:
+            if optimizer.applies_to(image_format):
+                optimizers.append(optimizer)
+
+        return optimizers
+
     # Routing
 
     # In some cases, it may not be possible to convert directly between two
     # image classes, so we need to use one or more intermediate classes in order
     # to get to where we want to be.
 
     # For example, the OpenCV plugin doesn't load JPEG images, so the image
@@ -178,24 +261,29 @@
         # Implementation based on https://www.python.org/doc/essays/graphs/
         if start == end:
             return [path]
 
         if start in seen_classes:
             return []
 
-        if not start in self._registered_image_classes or start in self._unavailable_image_classes:
+        if (
+            start not in self._registered_image_classes
+            or start in self._unavailable_image_classes
+        ):
             return []
 
         paths = []
         for converter, next_class in self.get_converters_from(start):
             if next_class not in path:
                 newpaths = self.find_all_paths(
-                    next_class, end,
+                    next_class,
+                    end,
                     path + [(converter, next_class)],
-                    seen_classes.union({start}))
+                    seen_classes.union({start}),
+                )
 
                 paths.extend(newpaths)
 
         return paths
 
     def get_path_cost(self, start, path):
         """
@@ -311,30 +399,33 @@
             cls = from_class
             path = []
             cost = 0
         except LookupError:
             # Not implemented on the current class. Find the closest, available,
             # routable class that has it instead
             image_classes = self.get_image_classes(
-                with_operation=operation_name,
-                available=True)
+                with_operation=operation_name, available=True
+            )
 
             # Choose an image class
             # image_classes will always have a value here as get_image_classes raises
             # LookupError if there are no image classes available.
             cls, path, cost = self.find_closest_image_class(from_class, image_classes)
 
             if path is None:
                 raise UnroutableOperationError(
-                    "The operation '{0}' is available in the image class '{1}'"
-                    " but it can't be converted to from '{2}'".format(
+                    "The operation '{}' is available in the image class '{}'"
+                    " but it can't be converted to from '{}'".format(
                         operation_name,
-                        ', '.join(image_class.__name__ for image_class in image_classes),
-                        from_class.__name__
-                    ))
+                        ", ".join(
+                            image_class.__name__ for image_class in image_classes
+                        ),
+                        from_class.__name__,
+                    )
+                )
 
             # Get the operation function
             func = self.get_operation(cls, operation_name)
 
         return func, cls, path, cost
```

### Comparing `Willow-1.5.1/willow/svg.py` & `willow-1.6/willow/svg.py`

 * *Files identical despite different names*

