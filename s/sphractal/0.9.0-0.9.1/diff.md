# Comparing `tmp/sphractal-0.9.0.tar.gz` & `tmp/sphractal-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-0.9.0.tar", max compression
+gzip compressed data, was "sphractal-0.9.1.tar", max compression
```

## Comparing `sphractal-0.9.0.tar` & `sphractal-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2023-07-10 06:35:37.325830 sphractal-0.9.0/LICENSE
--rw-r--r--   0        0        0     4017 2023-07-10 06:35:37.325830 sphractal-0.9.0/README.md
--rw-r--r--   0        0        0     2056 2023-07-10 06:36:20.890169 sphractal-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      736 2023-07-10 06:36:20.890169 sphractal-0.9.0/setup.py
--rw-r--r--   0        0        0     1429 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/__init__.py
--rw-r--r--   0        0        0    23389 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4382 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/constants.py
--rw-r--r--   0        0        0        0 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    20105 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/data/example.xyz
--rw-r--r--   0        0        0      264 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/datasets.py
--rw-r--r--   0        0        0     8929 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/surfExact.py
--rw-r--r--   0        0        0     8121 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/surfPointClouds.py
--rw-r--r--   0        0        0    11511 2023-07-10 06:35:37.385831 sphractal-0.9.0/src/sphractal/utils.py
--rw-r--r--   0        0        0    94032 2023-07-10 06:35:37.385831 sphractal-0.9.0/tests/fixtures.py
--rw-r--r--   0        0        0    17618 2023-07-10 06:35:37.385831 sphractal-0.9.0/tests/test_sphractal.py
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 sphractal-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-11 07:30:55.684251 sphractal-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4643 2023-07-11 07:30:55.684251 sphractal-0.9.1/README.md
+-rw-r--r--   0        0        0     2056 2023-07-11 07:31:56.620432 sphractal-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2023-07-11 07:31:56.620432 sphractal-0.9.1/setup.py
+-rw-r--r--   0        0        0     1429 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    23389 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4382 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/constants.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    20105 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/data/example.xyz
+-rw-r--r--   0        0        0      264 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/datasets.py
+-rw-r--r--   0        0        0     8929 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0     8121 2023-07-11 07:30:55.756251 sphractal-0.9.1/src/sphractal/surfPointClouds.py
+-rw-r--r--   0        0        0    11511 2023-07-11 07:30:55.760251 sphractal-0.9.1/src/sphractal/utils.py
+-rw-r--r--   0        0        0    94032 2023-07-11 07:30:55.760251 sphractal-0.9.1/tests/fixtures.py
+-rw-r--r--   0        0        0    17618 2023-07-11 07:30:55.760251 sphractal-0.9.1/tests/test_sphractal.py
+-rw-r--r--   0        0        0     5912 1970-01-01 00:00:00.000000 sphractal-0.9.1/PKG-INFO
```

### Comparing `sphractal-0.9.0/LICENSE` & `sphractal-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/README.md` & `sphractal-0.9.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,49 +3,54 @@
 [![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
 
 ## Description
 
 `Sphractal` is a package that provides functionalities to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
+## Background
+* Atomic objects in molecular and nanosciences such are often represented as collection of spheres with radii associated 
+with the atomic radius of the individual component.
+* Some examples of these objects (inclusive of both fine- and coarse-grained representation of the individual components) 
+are small molecules, proteins, nanoparticles, polymers, and porous materials such as zeolite, metal-organic framework (MOFs).
+* The overall properties of these objects are often significantly influenced by their surface properties, in particular 
+the surface area available for interaction with other entities, which is related to the surface roughness.
+* Fractal dimension allows the surface complexity/roughness of objects to be measured quantitatively, more details about 
+fractal dimension is included in the [notebook tutorial](https://github.com/Jon-Ting/sphractal/blob/main/docs/example.ipynb)).
+
 ## Features
 
 ### Aims
-* Representation of the surface as either point clouds or exact surfaces.
+* Representation of the surface as either voxelised point clouds or mathematically exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
-### Under Development
-* Optional input argument of surface atoms (to guarantee accurate box counts).
-* Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
-* Integration of C++ code for point cloud surface representation into the package.
-
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
 
 ```bash
 $ pip install sphractal
 ```
 ```bash
 $ conda install -c conda-forge sphractal
 ```
 
 ### Special Requirement for Point Cloud Surface Representation
 `Sphractal` requires an executable compiled from another freely available repository for the functionalities related 
-to point clouds surface representation to operate properly. 
+to voxelised point clouds surface representation to operate properly. 
 
 This could be done by:
 
 * Downloading the source code from the [repository](https://github.com/Jon-Ting/fastBC.git) to a directory of your choice:
 ```bash
 git clone https://github.com/Jon-Ting/fastBC.git
 ```
 
-* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables to any other sensible names:
+* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables:
 ```bash
 $ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
 $ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
 ```
```

### Comparing `sphractal-0.9.0/pyproject.toml` & `sphractal-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "0.9.0"
+version = "0.9.1"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-0.9.0/setup.py` & `sphractal-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-0.9.0/src/sphractal/__init__.py` & `sphractal-0.9.1/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/boxCnt.py` & `sphractal-0.9.1/src/sphractal/boxCnt.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/constants.py` & `sphractal-0.9.1/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/data/example.xyz` & `sphractal-0.9.1/src/sphractal/data/example.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/surfExact.py` & `sphractal-0.9.1/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/surfPointClouds.py` & `sphractal-0.9.1/src/sphractal/surfPointClouds.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/src/sphractal/utils.py` & `sphractal-0.9.1/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/tests/fixtures.py` & `sphractal-0.9.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/tests/test_sphractal.py` & `sphractal-0.9.1/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-0.9.0/PKG-INFO` & `sphractal-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
@@ -32,49 +32,54 @@
 [![ci-cd](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Jon-Ting/sphractal/actions/workflows/ci-cd.yml)
 
 ## Description
 
 `Sphractal` is a package that provides functionalities to estimate the fractal dimension of complex 3D surfaces formed 
 from overlapping spheres via box-counting algorithm. 
 
+## Background
+* Atomic objects in molecular and nanosciences such are often represented as collection of spheres with radii associated 
+with the atomic radius of the individual component.
+* Some examples of these objects (inclusive of both fine- and coarse-grained representation of the individual components) 
+are small molecules, proteins, nanoparticles, polymers, and porous materials such as zeolite, metal-organic framework (MOFs).
+* The overall properties of these objects are often significantly influenced by their surface properties, in particular 
+the surface area available for interaction with other entities, which is related to the surface roughness.
+* Fractal dimension allows the surface complexity/roughness of objects to be measured quantitatively, more details about 
+fractal dimension is included in the [notebook tutorial](https://github.com/Jon-Ting/sphractal/blob/main/docs/example.ipynb)).
+
 ## Features
 
 ### Aims
-* Representation of the surface as either point clouds or exact surfaces.
+* Representation of the surface as either voxelised point clouds or mathematically exact surfaces.
 * Efficient algorithm for 3D box-counting calculations.
 * Customisable parameters to control the level of detail and accuracy of the calculation.
 
-### Under Development
-* Optional input argument of surface atoms (to guarantee accurate box counts).
-* Transformation of xyz coordinates when atoms are read in to avoid using minXYZ repetitively in `scanAtom()`.
-* Integration of C++ code for point cloud surface representation into the package.
-
 ## Installation
 
 Use `pip` or `conda` to install `Sphractal`:
 
 ```bash
 $ pip install sphractal
 ```
 ```bash
 $ conda install -c conda-forge sphractal
 ```
 
 ### Special Requirement for Point Cloud Surface Representation
 `Sphractal` requires an executable compiled from another freely available repository for the functionalities related 
-to point clouds surface representation to operate properly. 
+to voxelised point clouds surface representation to operate properly. 
 
 This could be done by:
 
 * Downloading the source code from the [repository](https://github.com/Jon-Ting/fastBC.git) to a directory of your choice:
 ```bash
 git clone https://github.com/Jon-Ting/fastBC.git
 ```
 
-* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables to any other sensible names:
+* Building an executable by doing either one of the following compilations according to the instructions on the [README.md](https://github.com/Jon-Ting/fastBC/blob/main/README.md) page. This will decide whether you will be running the box counting algorithm with GPU acceleration. Feel free to rename the executables:
 ```bash
 $ g++ 3DbinImBCcpu.cpp bcCPU.cpp -o 3DbinImBCcpu.exe
 ```
 ```bash
 $ nvcc -O3 3DbinImBCgpu.cpp bcCUDA3D.cu -o 3DbinImBCgpu.exe
 ```
```

