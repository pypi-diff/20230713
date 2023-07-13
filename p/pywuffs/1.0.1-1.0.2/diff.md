# Comparing `tmp/pywuffs-1.0.1.tar.gz` & `tmp/pywuffs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywuffs-1.0.1.tar", last modified: Thu Jul 13 20:17:48 2023, max compression
+gzip compressed data, was "pywuffs-1.0.2.tar", last modified: Thu Jul 13 20:30:25 2023, max compression
```

## Comparing `pywuffs-1.0.1.tar` & `pywuffs-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/
--rw-rw-r--   0 george    (1000) george    (1000)     1073 2023-06-17 09:34:15.000000 pywuffs-1.0.1/LICENSE
--rw-r--r--   0 george    (1000) george    (1000)       90 2023-07-13 20:14:12.000000 pywuffs-1.0.1/MANIFEST.in
--rw-rw-r--   0 george    (1000) george    (1000)      236 2023-07-13 20:17:48.820546 pywuffs-1.0.1/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)     2150 2023-07-13 19:51:11.000000 pywuffs-1.0.1/README.md
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/libs/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/libs/wuffs-mirror-release-c/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/libs/wuffs-mirror-release-c/release/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/libs/wuffs-mirror-release-c/release/c/
--rw-rw-r--   0 george    (1000) george    (1000)  1825556 2023-07-12 17:55:45.000000 pywuffs-1.0.1/libs/wuffs-mirror-release-c/release/c/wuffs-v0.3.c
--rw-r--r--   0 george    (1000) george    (1000)       53 2023-07-12 19:57:07.000000 pywuffs-1.0.1/pyproject.toml
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/pywuffs.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)      236 2023-07-13 20:17:48.000000 pywuffs-1.0.1/pywuffs.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      312 2023-07-13 20:17:48.000000 pywuffs-1.0.1/pywuffs.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-07-13 20:17:48.000000 pywuffs-1.0.1/pywuffs.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)        8 2023-07-13 20:17:48.000000 pywuffs-1.0.1/pywuffs.egg-info/top_level.txt
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-13 20:17:48.820546 pywuffs-1.0.1/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)     1583 2023-07-13 20:17:09.000000 pywuffs-1.0.1/setup.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/src/
--rw-rw-r--   0 george    (1000) george    (1000)    12919 2023-07-13 11:04:12.000000 pywuffs-1.0.1/src/wuffs-aux-image-wrapper.h
--rw-rw-r--   0 george    (1000) george    (1000)    16142 2023-07-13 11:04:15.000000 pywuffs-1.0.1/src/wuffs-bindings.cpp
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:17:48.820546 pywuffs-1.0.1/test/
--rw-rw-r--   0 george    (1000) george    (1000)    10549 2023-07-13 11:04:12.000000 pywuffs-1.0.1/test/test_aux_image_decoder.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.747840 pywuffs-1.0.2/
+-rw-rw-r--   0 george    (1000) george    (1000)     1073 2023-06-17 09:34:15.000000 pywuffs-1.0.2/LICENSE
+-rw-r--r--   0 george    (1000) george    (1000)       90 2023-07-13 20:14:12.000000 pywuffs-1.0.2/MANIFEST.in
+-rw-rw-r--   0 george    (1000) george    (1000)      236 2023-07-13 20:30:25.747840 pywuffs-1.0.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)     2115 2023-07-13 20:22:21.000000 pywuffs-1.0.2/README.md
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.743841 pywuffs-1.0.2/libs/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.743841 pywuffs-1.0.2/libs/wuffs-mirror-release-c/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.743841 pywuffs-1.0.2/libs/wuffs-mirror-release-c/release/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.747840 pywuffs-1.0.2/libs/wuffs-mirror-release-c/release/c/
+-rw-rw-r--   0 george    (1000) george    (1000)  1825556 2023-07-12 17:55:45.000000 pywuffs-1.0.2/libs/wuffs-mirror-release-c/release/c/wuffs-v0.3.c
+-rw-r--r--   0 george    (1000) george    (1000)       53 2023-07-12 19:57:07.000000 pywuffs-1.0.2/pyproject.toml
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.747840 pywuffs-1.0.2/pywuffs.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)      236 2023-07-13 20:30:25.000000 pywuffs-1.0.2/pywuffs.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      312 2023-07-13 20:30:25.000000 pywuffs-1.0.2/pywuffs.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-07-13 20:30:25.000000 pywuffs-1.0.2/pywuffs.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        8 2023-07-13 20:30:25.000000 pywuffs-1.0.2/pywuffs.egg-info/top_level.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-13 20:30:25.747840 pywuffs-1.0.2/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)     1583 2023-07-13 20:29:35.000000 pywuffs-1.0.2/setup.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.747840 pywuffs-1.0.2/src/
+-rw-rw-r--   0 george    (1000) george    (1000)    12919 2023-07-13 11:04:12.000000 pywuffs-1.0.2/src/wuffs-aux-image-wrapper.h
+-rw-rw-r--   0 george    (1000) george    (1000)    16166 2023-07-13 20:26:52.000000 pywuffs-1.0.2/src/wuffs-bindings.cpp
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 20:30:25.747840 pywuffs-1.0.2/test/
+-rw-rw-r--   0 george    (1000) george    (1000)    10549 2023-07-13 11:04:12.000000 pywuffs-1.0.2/test/test_aux_image_decoder.py
```

### Comparing `pywuffs-1.0.1/LICENSE` & `pywuffs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywuffs-1.0.1/README.md` & `pywuffs-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Current version of Wuffs library used in this project is **0.3.3**.
 
 ## Installation
 
 ### Using pip
 
 ```bash
-python3 -m pip install git+https://github.com/dev0x13/pywuffs.git
+python3 -m pip install pywuffs
 ```
 
 ### Using CMake
 
 CMake build support is mostly intended for development purposes, so the process might be
 not so smooth.
```

### Comparing `pywuffs-1.0.1/libs/wuffs-mirror-release-c/release/c/wuffs-v0.3.c` & `pywuffs-1.0.2/libs/wuffs-mirror-release-c/release/c/wuffs-v0.3.c`

 * *Files identical despite different names*

### Comparing `pywuffs-1.0.1/setup.py` & `pywuffs-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
         "pywuffs",
         ["src/wuffs-bindings.cpp"],
         include_dirs=["libs/wuffs-mirror-release-c/release"]
     ),
 ]
 
 setup(name="pywuffs",
-      version="1.0.1",
+      version="1.0.2",
       description="Python bindings for Wuffs the Library",
       author="Georgiy Manuilov",
       url="https://github.com/dev0x13/pywuffs",
       cmdclass={"build_ext": CustomBuildExt},
       ext_modules=ext_modules)
```

### Comparing `pywuffs-1.0.1/src/wuffs-aux-image-wrapper.h` & `pywuffs-1.0.2/src/wuffs-aux-image-wrapper.h`

 * *Files identical despite different names*

### Comparing `pywuffs-1.0.1/src/wuffs-bindings.cpp` & `pywuffs-1.0.2/src/wuffs-bindings.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
    * Base Wuffs API
    */
 
   // clang-format off
   py::class_<wuffs_base__more_information>(
       m, "wuffs_base__more_information",
       "Holds additional fields. The flavor field follows the base38 namespace "
-      "convention (https://github.com/google/wuffs/blob/main/doc/note/base38-and-fourcc.md)."
+      "convention (https://github.com/google/wuffs/blob/main/doc/note/base38-and-fourcc.md). "
       "The other fields' semantics depends on the flavor.")
       // clang-format on
       .def_readonly("flavor", &wuffs_base__more_information::flavor)
       .def_readonly("w", &wuffs_base__more_information::w)
       .def_readonly("x", &wuffs_base__more_information::x)
       .def_readonly("y", &wuffs_base__more_information::y)
       .def_readonly("z", &wuffs_base__more_information::z)
@@ -230,20 +230,20 @@
           "background_color will typically be overwritten when pixel_blend is "
           "PixelBlend.SRC, but might still be visible on partial "
           "(not total) success or when pixel_blend is PixelBlend.SRC_OVER and "
           "the decoded image is not fully opaque.")
       .def_readwrite(
           "max_incl_dimension",
           &wuffs_aux_wrap::ImageDecoderConfig::max_incl_dimension,
-          "int: Decoding fails (with DecodeImage_MaxInclDimensionExceeded) if "
+          "int: Decoding fails (with ImageDecoderErrors.MaxInclDimensionExceeded) if "
           "the image's width or height is greater than max_incl_dimension.")
       .def_readwrite(
           "max_incl_metadata_length",
           &wuffs_aux_wrap::ImageDecoderConfig::max_incl_metadata_length,
-          "int: Decoding fails (with DecodeImage_MaxInclDimensionExceeded) if "
+          "int: Decoding fails (with ImageDecoderErrors.MaxInclDimensionExceeded) if "
           "any opted-in (via flags bits) metadata is longer than "
           "max_incl_metadata_length.")
       .def_readwrite("enabled_decoders",
                      &wuffs_aux_wrap::ImageDecoderConfig::enabled_decoders,
                      "list: list of ImageDecoderType.")
       .def_readwrite(
           "pixel_format", &wuffs_aux_wrap::ImageDecoderConfig::pixel_format,
@@ -305,20 +305,19 @@
       " - On failure, the error_message is non-empty and pixbuf is "
       "empty.")
       .def_readonly("pixbuf", &wuffs_aux_wrap::ImageDecodingResult::pixbuf,
                     "np.array: decoded pixel buffer (uint8 Numpy array of [H, "
                     "W, C] shape).")
       .def_readonly("pixcfg", &wuffs_aux_wrap::ImageDecodingResult::pixcfg,
                     "wuffs_base__pixel_config: decoded pixel buffer config.")
-      .def_readonly(
-          "reported_metadata",
-          &wuffs_aux_wrap::ImageDecodingResult::reported_metadata,
-          "VectorMetadataEntry: a list-like object containing reported data "
-          "(only filled is any metadata was decoded and the "
-          "corresponding ImageDecoderFlag flag was set).")
+      .def_readonly("reported_metadata",
+                    &wuffs_aux_wrap::ImageDecodingResult::reported_metadata,
+                    "list: a list object containing reported data "
+                    "(only filled if any metadata was decoded and the "
+                    "corresponding ImageDecoderFlag flag was set).")
       .def_readonly("error_message",
                     &wuffs_aux_wrap::ImageDecodingResult::error_message,
                     "str: error message, empty on success, one of "
                     "ImageDecoderError on error.");
 
   py::class_<wuffs_aux_wrap::ImageDecoder>(aux_m, "ImageDecoder",
                                            "Image decoder class.")
```

### Comparing `pywuffs-1.0.1/test/test_aux_image_decoder.py` & `pywuffs-1.0.2/test/test_aux_image_decoder.py`

 * *Files identical despite different names*

