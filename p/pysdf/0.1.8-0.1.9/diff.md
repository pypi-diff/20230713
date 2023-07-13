# Comparing `tmp/pysdf-0.1.8.tar.gz` & `tmp/pysdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysdf-0.1.8.tar", last modified: Fri Aug 28 23:00:20 2020, max compression
+gzip compressed data, was "pysdf-0.1.9.tar", last modified: Thu Jul 13 03:50:53 2023, max compression
```

## Comparing `pysdf-0.1.8.tar` & `pysdf-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     1260 2020-08-21 03:35:05.000000 pysdf-0.1.8/LICENSE.txt
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)      310 2020-08-28 01:27:23.000000 pysdf-0.1.8/MANIFEST.in
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)      431 2020-08-28 23:00:20.000000 pysdf-0.1.8/PKG-INFO
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     7681 2020-08-27 05:31:24.000000 pysdf-0.1.8/README.md
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/include/
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/include/sdf/
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/include/sdf/internal/
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)    50018 2020-08-19 06:22:31.000000 pysdf-0.1.8/include/sdf/internal/RTree.h
--rwxrwxr-x   0 sxyu      (1000) sxyu      (1000)    73083 2020-08-19 06:22:34.000000 pysdf-0.1.8/include/sdf/internal/nanoflann.hpp
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     3761 2020-08-28 22:09:47.000000 pysdf-0.1.8/include/sdf/internal/sdf_util.hpp
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)    14766 2020-08-28 22:34:03.000000 pysdf-0.1.8/include/sdf/sdf.hpp
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     9557 2020-08-28 22:37:12.000000 pysdf-0.1.8/pybind.cpp
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/pysdf.egg-info/
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)      431 2020-08-28 23:00:20.000000 pysdf-0.1.8/pysdf.egg-info/PKG-INFO
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)      367 2020-08-28 23:00:20.000000 pysdf-0.1.8/pysdf.egg-info/SOURCES.txt
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)        1 2020-08-28 23:00:20.000000 pysdf-0.1.8/pysdf.egg-info/dependency_links.txt
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)        1 2020-08-21 03:50:50.000000 pysdf-0.1.8/pysdf.egg-info/not-zip-safe
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)        6 2020-08-28 23:00:20.000000 pysdf-0.1.8/pysdf.egg-info/top_level.txt
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)       79 2020-08-28 23:00:20.000000 pysdf-0.1.8/setup.cfg
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     6609 2020-08-28 22:26:53.000000 pysdf-0.1.8/setup.py
-drwxrwxr-x   0 sxyu      (1000) sxyu      (1000)        0 2020-08-28 23:00:20.000000 pysdf-0.1.8/src/
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)    11198 2020-08-28 22:40:54.000000 pysdf-0.1.8/src/renderer.cpp
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)    14925 2020-08-28 21:19:00.000000 pysdf-0.1.8/src/sdf.cpp
--rw-rw-r--   0 sxyu      (1000) sxyu      (1000)     1149 2020-08-28 01:11:28.000000 pysdf-0.1.8/src/util.cpp
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1260 2022-04-05 03:44:05.000000 pysdf-0.1.9/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      310 2022-04-05 03:44:05.000000 pysdf-0.1.9/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)      446 2023-07-13 03:50:53.264571 pysdf-0.1.9/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7835 2023-07-13 03:43:10.000000 pysdf-0.1.9/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/include/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/include/sdf/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/include/sdf/internal/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    50018 2022-04-05 03:44:05.000000 pysdf-0.1.9/include/sdf/internal/RTree.h
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    73083 2022-04-05 03:44:05.000000 pysdf-0.1.9/include/sdf/internal/nanoflann.hpp
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3761 2022-04-05 03:44:05.000000 pysdf-0.1.9/include/sdf/internal/sdf_util.hpp
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15287 2023-07-13 03:37:57.000000 pysdf-0.1.9/include/sdf/sdf.hpp
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10134 2023-07-13 03:41:34.000000 pysdf-0.1.9/pybind.cpp
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/pysdf.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      446 2023-07-13 03:50:53.000000 pysdf-0.1.9/pysdf.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      367 2023-07-13 03:50:53.000000 pysdf-0.1.9/pysdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-13 03:50:53.000000 pysdf-0.1.9/pysdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-13 03:36:28.000000 pysdf-0.1.9/pysdf.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-07-13 03:50:53.000000 pysdf-0.1.9/pysdf.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       79 2023-07-13 03:50:53.264571 pysdf-0.1.9/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6609 2023-07-13 03:43:25.000000 pysdf-0.1.9/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-13 03:50:53.264571 pysdf-0.1.9/src/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-13 03:35:59.000000 pysdf-0.1.9/src/renderer.cpp
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15298 2023-07-13 03:33:29.000000 pysdf-0.1.9/src/sdf.cpp
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1149 2022-04-05 03:44:05.000000 pysdf-0.1.9/src/util.cpp
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysdf-0.1.8/LICENSE.txt` & `pysdf-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysdf-0.1.8/README.md` & `pysdf-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 origin_nn = f.nn([0, 0, 0])
 
 # Misc: uniform surface point sampling
 random_surface_points = f.sample_surface(10000)
 
 # Misc: surface area
 the_surface_area = f.surface_area
+
+# All the functions also support an additional argument 'n_threads=<int>' to specify number of threads.
+# by default we use min(32, n_cpus) 
 ```
 To modify the vertices/faces, you can change
 `f.vertices_mutable` and `f.faces_mutable`, then call `f.update()` to 
 update the internal data structures.
 You can also use 
 `f.vertices` and `f.faces` to access vertices and faces (non-writable).
 
@@ -119,15 +122,15 @@
 - Vendored (no installation needed):
     - nanoflann
     - nushoin/RTree
 - Optional:
     - meshview https://github.com/sxyu/meshview for demo
 
 ## Build + Install
-`mkdir build && cmake .. && make -j4 && sudo make install`
+`mkdir build && cd build && cmake .. && make -j4 && sudo make install`
 
 ## Demo
 A demo program can optionally be built, if meshview is installed.
 To use it, run `./sdf-demo BASIC_OBJ_FILE`. Try the `sample-obj/*.obj` included in the project.
 
 ## Benchmark
```

### Comparing `pysdf-0.1.8/include/sdf/internal/RTree.h` & `pysdf-0.1.9/include/sdf/internal/RTree.h`

 * *Files identical despite different names*

### Comparing `pysdf-0.1.8/include/sdf/internal/nanoflann.hpp` & `pysdf-0.1.9/include/sdf/internal/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `pysdf-0.1.8/include/sdf/internal/sdf_util.hpp` & `pysdf-0.1.9/include/sdf/internal/sdf_util.hpp`

 * *Files identical despite different names*

### Comparing `pysdf-0.1.8/include/sdf/sdf.hpp` & `pysdf-0.1.9/include/sdf/sdf.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 #define SDF_SDF_F15B6437_01FD_4DBE_AB0D_BC1EE8ACC4C4
 
 #include <Eigen/Core>
 #include <cstdint>
 
 #include <memory>
 #include <vector>
+#include <thread>
 #ifdef __GNUC__
 #include <experimental/propagate_const>
 #endif
 #include <Eigen/Geometry>
 
 namespace sdf {
 
@@ -180,29 +181,31 @@
     // bounding box
     // @return approx SDF values at input points
     //
     // WARNING: if robust=false (from constructor), this WILL FAIL if the mesh
     // has self-intersections. In particular, the signs of points inside the
     // mesh may be flipped.
     Vector operator()(Eigen::Ref<const Points> points,
-                      bool trunc_aabb = false) const;
+                      bool trunc_aabb = false,
+                      int n_threads = std::thread::hardware_concurrency()) const;
 
     // Return exact nearest neighbor vertex index for each point (index as in
     // input verts)
-    Eigen::VectorXi nn(Eigen::Ref<const Points> points) const;
+    Eigen::VectorXi nn(Eigen::Ref<const Points> points, int n_threads = std::thread::hardware_concurrency()) const;
 
     // Return 1 for each point inside/on surface of the mesh and 0 for outside.
     //
     // @param points input points
     // @return indicator of whether each point is in OR on surface of mesh
     //
     // WARNING: if robust=false (from constructor), this WILL FAIL if the mesh
     // has self-intersections.
     Eigen::Matrix<bool, Eigen::Dynamic, 1> contains(
-        Eigen::Ref<const Points> points) const;
+        Eigen::Ref<const Points> points,
+        int n_threads = std::thread::hardware_concurrency()) const;
 
     // Call if vertex positions have been updated to rebuild the KD tree
     // and update face normals+areas
     void update();
 
     /*** MISC UTILITIES ***/
     // Sample 'num_points' points uniformly on surface, output (num_points, 3).
@@ -301,44 +304,44 @@
     ~Renderer();
 
     // *** PRIMARY INTERFACE ***
     // Render (height, width) depth map of the mesh.
     // @return Each pixel will be distance from z=0 plane and 0 if no object is
     // present.
     Eigen::Matrix<float, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_depth() const;
+    render_depth(int n_threads = std::thread::hardware_concurrency()) const;
 
     // Render (height, width) mask.
     // @return Each pixel is 1 where object is present, 0 else.
     Eigen::Matrix<bool, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_mask() const;
+    render_mask(int n_threads = std::thread::hardware_concurrency()) const;
 
     // Render (height, width) vertex map, i.e. vertex id nearest to raycast hit
     // at each pixel. Each pixel is -1 if empty space, index of vertex in verts
     // else
     // @param fill_outside if true, instead of returning -1 for empty space,
     // finds nearest-neighbor vertex in 2d and uses its index
     Eigen::Matrix<int, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_nn(bool fill_outside = false) const;
+    render_nn(bool fill_outside = false, int n_threads = std::thread::hardware_concurrency()) const;
 
     // Compute depth at 2D points
     // (render_depth for continuous points)
-    Vector operator()(Eigen::Ref<const Points2D> points) const;
+    Vector operator()(Eigen::Ref<const Points2D> points, int n_threads = std::thread::hardware_concurrency()) const;
 
     // Compute mask at 2D points (1 means inside)
     // (render_mask for continuous points)
     Eigen::Matrix<bool, Eigen::Dynamic, 1> contains(
-        Eigen::Ref<const Points2D> points) const;
+        Eigen::Ref<const Points2D> points, int n_threads = std::thread::hardware_concurrency()) const;
 
     // Compute vertex id hit by raycast at 2D points
     // (render_vertex for continuous points)
     // @param fill_outside if true, instead of returning -1 for empty space,
     // finds nearest-neighbor vertex in 2d and uses its index
     Eigen::VectorXi nn(Eigen::Ref<const Points2D> points,
-                       bool fill_outside = false) const;
+                       bool fill_outside = false, int n_threads = std::thread::hardware_concurrency()) const;
 
     // Call if vertex positions have been updated to rebuild the KD tree
     // and update face normals+areas
     void update();
 
     /*** DATA ACCESSORS ***/
     // Get faces
```

### Comparing `pysdf-0.1.8/pybind.cpp` & `pysdf-0.1.9/pybind.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 #include <pybind11/eigen.h>
 #include <iostream>
 #include <thread>
 
 namespace py = pybind11;
 using namespace sdf;
 
+static const int DEFAULT_NUM_THREADS = std::min(static_cast<int>(std::thread::hardware_concurrency()), 32);
+
 PYBIND11_MODULE(pysdf, m) {
     m.doc() =
         R"pbdoc(SDF: Convert triangle mesh to continuous signed distance function)pbdoc";
 
     py::class_<SDF>(m, "SDF")
         .def(py::init<Eigen::Ref<const Points>, Eigen::Ref<const Triangles>,
                       bool, bool>(),
              py::arg("verts"), py::arg("faces"), py::arg("robust") = true,
              py::arg("copy") = true)
         .def("__call__", &SDF::operator(),
              "Compute SDF on points (positive iff inside)", py::arg("points"),
-             py::arg("trunc_aabb") = false)
+             py::arg("trunc_aabb") = false, py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("calc", &SDF::operator(),
              "Compute SDF on points (positive iff inside), alias of __call__",
-             py::arg("points"), py::arg("trunc_aabb") = false)
+             py::arg("points"), py::arg("trunc_aabb") = false, py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("contains", &SDF::contains, "Test if points are in mesh",
-             py::arg("points"))
-        .def("nn", &SDF::nn, "Find nearest neighbor indices", py::arg("points"))
+             py::arg("points"), py::arg("n_threads") = DEFAULT_NUM_THREADS)
+        .def("nn", &SDF::nn, "Find nearest neighbor indices", py::arg("points"), py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("update", &SDF::update,
              "Update the SDF to reflect any changes in verts")
         .def("sample_surface", &SDF::sample_surface,
              "Sample num_points uniformly random points on mesh surface. "
              "Internally, picks each triangle wp prop to area and then random "
              "point on triangle.",
              py::arg("num_points"))
@@ -85,45 +87,45 @@
                       int, int, float, float, float, float, bool>(),
              py::arg("verts"), py::arg("faces"), py::arg("width") = 1080,
              py::arg("height") = 1080, py::arg("fx") = 2600.f,
              py::arg("fy") = 2600.f, py::arg("cx") = 540.f,
              py::arg("cy") = 540.f, py::arg("copy") = true)
         .def("__call__", &Renderer::operator(),
              "Compute depth on 2D image-space points (0 if nothing there)",
-             py::arg("points"))
+             py::arg("points"), py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("calc", &Renderer::operator(),
              "Compute depth on 2D image-space points (0 if nothing there), "
              "alias of __call__",
-             py::arg("points"))
+             py::arg("points"), py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("contains", &Renderer::contains,
              "For each point, returns true if the ray cast from (x, y, 0) in"
              "+z direction in image space hits the mesh. This is the "
              "continuous point version of render_mask",
-             py::arg("points"))
+             py::arg("points"), py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("nn", &Renderer::nn,
              "Compute index of closest vertex hit by a ray cast from (x, y, "
              "0) in image space. -1 if no vertex. Continuous point version of "
              "render_nn."
              "For pixels in empty space, returns 2D (xy) nearest-neighbor "
              "if fill_outside is true, or -1 else (default). "
              "dtype int.",
-             py::arg("points"), py::arg("fill_outside") = true)
+             py::arg("points"), py::arg("fill_outside") = true, py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("render_depth", &Renderer::render_depth,
              "Render a depth image, with camera facing +z, right=+x, up=-y. 0 "
-             "means no object. dtype float")
+             "means no object. dtype float", py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("render_mask", &Renderer::render_mask,
              "Render a mask (silhouette), with camera facing +z, right=+x, "
-             "up=-y. 0 means no object, 1 means object present. dtype bool")
+             "up=-y. 0 means no object, 1 means object present. dtype bool", py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("render_nn", &Renderer::render_nn,
              "Render a map of vertex indices, more specifically "
              "closest (in 2D) vertex of first triangle hit by ray. "
              "For pixels in empty space, returns 2D (xy) nearest-neighbor "
              "if fill_outside is true, or -1 else (default). "
              "dtype int.",
-             py::arg("fill_outside") = false)
+             py::arg("fill_outside") = false, py::arg("n_threads") = DEFAULT_NUM_THREADS)
         .def("update", &Renderer::update,
              "Update the Renderer to reflect any changes in verts")
         .def_property_readonly("faces", &Renderer::faces,
                                "Mesh faces passed to Renderer constructor")
         .def_property_readonly("verts", &Renderer::verts,
                                "Mesh vertices passed to Renderer constructor")
         .def_property(
@@ -186,9 +188,9 @@
                 float area = normal.norm();
                 normal /= area;
                 return util::dist_point2tri<float>(p, a, b, c, normal, area);
             },
             "Compute 3d point-triangle squared distance")
         .def("bary2d", &util::bary2d<float>,
              "Test if point is in triangle (2d)");
-    m.attr("num_threads") = std::thread::hardware_concurrency();
+    m.attr("num_threads") = DEFAULT_NUM_THREADS;
 }
```

### Comparing `pysdf-0.1.8/setup.py` & `pysdf-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 import sys
 import setuptools
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path
 
     The purpose of this class is to postpone importing pybind11
     until it is actually installed, so that the ``get_include()``
```

### Comparing `pysdf-0.1.8/src/renderer.cpp` & `pysdf-0.1.9/src/renderer.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "sdf/sdf.hpp"
 
 #include <iostream>
 #include <limits>
+#include <thread>
 #include "sdf/internal/RTree.h"
 #include "sdf/internal/sdf_util.hpp"
 
 namespace {
 using RowVec3 = Eigen::Matrix<float, 1, 3>;
 using RefRowVec3 = Eigen::Ref<const RowVec3>;
 using RowVec3idx = Eigen::Matrix<sdf::Index, 1, 3>;
@@ -86,56 +87,60 @@
     }
 
     template <typename T>
     using FaceHandler = bool (Impl::*)(T&, RefRowVec3, RefRowVec3idx) const;
 
    public:
     Eigen::Matrix<float, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_depth() const {
+    render_depth(int n_threads) const {
         return _render_image<float>(
             (FaceHandler<float>)&Impl::_depth_face_handler,
-            std::numeric_limits<float>::max(), true /* convert FLT_MAX to 0 */);
+            std::numeric_limits<float>::max(), true /* convert FLT_MAX to 0 */, false, n_threads);
     }
 
     Eigen::Matrix<bool, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_mask() const {
+    render_mask(int n_threads) const {
         return _render_image<bool>((FaceHandler<bool>)&Impl::_mask_face_handler,
-                                   false);
+                                   false,
+                                   false, false,
+                                   n_threads);
     }
 
     Eigen::Matrix<int, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-    render_nn(bool fill_outside) const {
+    render_nn(bool fill_outside, int n_threads) const {
         if (fill_outside && !kdtree_ready) {
             kd_tree.rebuild();
             kdtree_ready = true;
         }
         return _render_image<int>((FaceHandler<int>)&Impl::_vertex_face_handler,
-                                  -1, false, fill_outside);
+                                  -1, false, fill_outside, n_threads);
     }
 
-    Vector calc_depth(Eigen::Ref<const Points2D> points) const {
+    Vector calc_depth(Eigen::Ref<const Points2D> points, int n_threads) const {
         return _calc<float>(
             points, (FaceHandler<float>)&Impl::_depth_face_handler,
-            std::numeric_limits<float>::max(), true /* convert FLT_MAX to 0 */);
+            std::numeric_limits<float>::max(), true /* convert FLT_MAX to 0 */,
+            false, n_threads);
     }
 
     Eigen::Matrix<bool, Eigen::Dynamic, 1> calc_mask(
-        Eigen::Ref<const Points2D> points) const {
+        Eigen::Ref<const Points2D> points, int n_threads) const {
         return _calc<bool>(points, (FaceHandler<bool>)&Impl::_mask_face_handler,
-                           uint8_t(0));
+                           uint8_t(0), false, false, n_threads);
     }
 
     Eigen::VectorXi calc_vertex(Eigen::Ref<const Points2D> points,
-                                bool fill_outside) const {
+                                bool fill_outside,
+                                int n_threads) const {
         if (fill_outside && !kdtree_ready) {
             kd_tree.rebuild();
             kdtree_ready = true;
         }
         return _calc<int>(points, (FaceHandler<int>)&Impl::_vertex_face_handler,
-                          -1, false, fill_outside);
+                          -1, false, fill_outside, n_threads);
     }
 
     // Input vertices
     Eigen::Ref<const Points> verts;
     // Input triangular faces
     Eigen::Ref<const Triangles> faces;
 
@@ -168,15 +173,16 @@
         rtree.Search(aabb_min.data(), aabb_max.data(), check_face);
     }
 
     template <class T>
     Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
     _render_image(FaceHandler<T> face_handler, T init_val,
                   bool max_to_zero = false,
-                  bool fill_outside_nn = false) const {
+                  bool fill_outside_nn = false,
+                  int n_threads = std::thread::hardware_concurrency()) const {
         Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
             result(height, width);
         result.setConstant(init_val);
         maybe_parallel_for(
             [&](int i) {
                 int r = i / width, c = i % width;
                 RowVec2 point;
@@ -193,23 +199,26 @@
                     nanoflann::KNNResultSet<float> resultSet(1);
                     resultSet.init(&index, &dist);
                     kd_tree.index->findNeighbors(resultSet, point.data(),
                                                  nanoflann::SearchParams(10));
                     data = static_cast<int>(index);
                 }
             },
-            width * height);
+            width * height,
+            n_threads);
         return result;
     }
 
     template <class T>
     Eigen::Matrix<T, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor> _calc(
         const Eigen::Ref<const Points2D>& points, FaceHandler<T> face_handler,
-        T init_val, bool max_to_zero = false,
-        bool fill_outside_nn = false) const {
+        T init_val,
+        bool max_to_zero = false,
+        bool fill_outside_nn = false,
+        int n_threads = std::thread::hardware_concurrency()) const {
         Eigen::Matrix<T, Eigen::Dynamic, 1> result(points.rows());
         result.setConstant(init_val);
         maybe_parallel_for(
             [&](int i) {
                 T& data = result.data()[i];
                 _raycast<T>(points.row(i), face_handler, data);
 
@@ -223,15 +232,16 @@
                     resultSet.init(&index, &dist);
                     kd_tree.index->findNeighbors(resultSet,
                                                  points.data() + i * 2,
                                                  nanoflann::SearchParams(10));
                     data = static_cast<T>(index);
                 }
             },
-            result.rows());
+            result.rows(),
+            n_threads);
         return result;
     }
 
     // Face R-Tree (aka AABB Tree)
     RTree<int, float, 2> rtree;
 
     // KD tree for NN search (optional)
@@ -255,26 +265,26 @@
     } else {
         p_impl =
             std::make_unique<Impl>(verts, faces, width, height, fx, fy, cx, cy);
     }
 }
 
 Eigen::Matrix<float, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-Renderer::render_depth() const {
-    return p_impl->render_depth();
+Renderer::render_depth(int n_threads) const {
+    return p_impl->render_depth(n_threads);
 }
 
 Eigen::Matrix<bool, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-Renderer::render_mask() const {
-    return p_impl->render_mask();
+Renderer::render_mask(int n_threads) const {
+    return p_impl->render_mask(n_threads);
 }
 
 Eigen::Matrix<int, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>
-Renderer::render_nn(bool fill_outside) const {
-    return p_impl->render_nn(fill_outside);
+Renderer::render_nn(bool fill_outside, int n_threads) const {
+    return p_impl->render_nn(fill_outside, n_threads);
 }
 
 void Renderer::update() { p_impl->update(); }
 
 Eigen::Ref<const Triangles> Renderer::faces() const { return p_impl->faces; }
 Eigen::Ref<Triangles> Renderer::faces_mutable() {
     if (!own_data) {
@@ -289,24 +299,25 @@
     if (!own_data) {
         std::cerr
             << "ERROR: 'verts' is non mutable, construct with copy=True\n";
     }
     return owned_verts;
 }
 
-Vector Renderer::operator()(Eigen::Ref<const Points2D> points) const {
-    return p_impl->calc_depth(points);
+Vector Renderer::operator()(Eigen::Ref<const Points2D> points, int n_threads) const {
+    return p_impl->calc_depth(points, n_threads);
 }
 
 Eigen::Matrix<bool, Eigen::Dynamic, 1> Renderer::contains(
-    Eigen::Ref<const Points2D> points) const {
-    return p_impl->calc_mask(points);
+    Eigen::Ref<const Points2D> points, int n_threads) const {
+    return p_impl->calc_mask(points, n_threads);
 }
 
 Eigen::VectorXi Renderer::nn(Eigen::Ref<const Points2D> points,
-                             bool fill_outside) const {
-    return p_impl->calc_vertex(points, fill_outside);
+                             bool fill_outside,
+                             int n_threads) const {
+    return p_impl->calc_vertex(points, fill_outside, n_threads);
 }
 
 Renderer::~Renderer() = default;
 
 }  // namespace sdf
```

### Comparing `pysdf-0.1.8/src/sdf.cpp` & `pysdf-0.1.9/src/sdf.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -68,32 +68,35 @@
             face_area[i] = face_normal.row(i).norm();
             face_normal.row(i) /= face_area[i];
         }
         total_area = face_area.sum();
         face_area_cum.resize(0);
     }
 
-    Eigen::VectorXi nn(Eigen::Ref<const Points> points) const {
+    Eigen::VectorXi nn(Eigen::Ref<const Points> points,
+                        int n_threads = std::thread::hardware_concurrency()) const {
         Eigen::VectorXi result(points.rows());
         maybe_parallel_for(
             [&](int i) {
                 size_t index;
                 float dist;
                 nanoflann::KNNResultSet<float> resultSet(1);
                 resultSet.init(&index, &dist);
                 kd_tree.index->findNeighbors(resultSet, points.data() + i * 3,
                                              nanoflann::SearchParams(10));
                 result[i] = static_cast<int>(index);
             },
-            (int)points.rows());
+            (int)points.rows(),
+            n_threads);
         return result;
     }
 
     Vector calc(Eigen::Ref<const Points> points,
-                bool trunc_aabb = false) const {
+                bool trunc_aabb = false,
+                int n_threads = std::thread::hardware_concurrency()) const {
         Vector result(points.rows());
         result.setConstant(std::numeric_limits<float>::max());
 
         const float DIST_EPS = robust ? 0.f : 1e-5f;
 
         maybe_parallel_for(
             [&](int i) {
@@ -145,28 +148,31 @@
                     min_dist *= sign;
                 } else if (avg_normal.dot(point - verts.row(neighb_index)) >
                            0) {
                     // Outside, by normal
                     min_dist = -min_dist;
                 }
             },
-            (int)points.rows());
+            (int)points.rows(),
+            n_threads);
         return result;
     }
 
     Eigen::Matrix<bool, Eigen::Dynamic, 1> contains(
-        Eigen::Ref<const Points> points) const {
+        Eigen::Ref<const Points> points,
+        int n_threads = std::thread::hardware_concurrency()) const {
         if (robust) {
             Eigen::Matrix<bool, Eigen::Dynamic, 1> result(points.rows());
             maybe_parallel_for(
                 [&](int i) { result[i] = _raycast(points.row(i)) >= 0.0f; },
-                (int)points.rows());
+                (int)points.rows(),
+                n_threads);
             return result;
         } else {
-            Vector vals = calc(points, true);
+            Vector vals = calc(points, true, n_threads);
             return vals.array() >= 0;
         }
     }
 
     Points sample_surface(int num_points) const {
         if (face_area.rows() == 0) {
             std::cerr << "ERROR: No faces, can't sample surface.\n";
@@ -364,25 +370,26 @@
     if (!own_data) {
         std::cerr
             << "ERROR: 'verts' is non mutable, construct with copy=True\n";
     }
     return owned_verts;
 }
 
-Vector SDF::operator()(Eigen::Ref<const Points> points, bool trunc_aabb) const {
-    return p_impl->calc(points, trunc_aabb);
+Vector SDF::operator()(Eigen::Ref<const Points> points, bool trunc_aabb, int n_threads) const {
+    return p_impl->calc(points, trunc_aabb, n_threads);
 }
 
-Eigen::VectorXi SDF::nn(Eigen::Ref<const Points> points) const {
-    return p_impl->nn(points);
+Eigen::VectorXi SDF::nn(Eigen::Ref<const Points> points, int n_threads) const {
+    return p_impl->nn(points, n_threads);
 }
 
 Eigen::Matrix<bool, Eigen::Dynamic, 1> SDF::contains(
-    Eigen::Ref<const Points> points) const {
-    return p_impl->contains(points);
+    Eigen::Ref<const Points> points,
+    int n_threads) const {
+    return p_impl->contains(points, n_threads);
 }
 
 void SDF::update() { p_impl->update(); }
 
 Points SDF::sample_surface(int num_points) const {
     return p_impl->sample_surface(num_points);
 }
```

### Comparing `pysdf-0.1.8/src/util.cpp` & `pysdf-0.1.9/src/util.cpp`

 * *Files identical despite different names*

