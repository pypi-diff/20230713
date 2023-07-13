# Comparing `tmp/opensr-test-0.0.1.tar.gz` & `tmp/opensr-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensr-test-0.0.1.tar", last modified: Wed Jul 12 18:54:18 2023, max compression
+gzip compressed data, was "opensr-test-0.0.2.tar", last modified: Thu Jul 13 09:46:17 2023, max compression
```

## Comparing `opensr-test-0.0.1.tar` & `opensr-test-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-12 18:54:18.210965 opensr-test-0.0.1/
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1077 2023-07-12 18:42:54.000000 opensr-test-0.0.1/LICENSE
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    15209 2023-07-12 18:54:18.210965 opensr-test-0.0.1/PKG-INFO
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14485 2023-07-12 18:42:18.000000 opensr-test-0.0.1/README.md
-drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-12 18:54:18.206965 opensr-test-0.0.1/opensr_test.egg-info/
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    15209 2023-07-12 18:54:18.000000 opensr-test-0.0.1/opensr_test.egg-info/PKG-INFO
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)      200 2023-07-12 18:54:18.000000 opensr-test-0.0.1/opensr_test.egg-info/SOURCES.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-12 18:54:18.000000 opensr-test-0.0.1/opensr_test.egg-info/dependency_links.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       61 2023-07-12 18:54:18.000000 opensr-test-0.0.1/opensr_test.egg-info/requires.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-12 18:54:18.000000 opensr-test-0.0.1/opensr_test.egg-info/top_level.txt
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       38 2023-07-12 18:54:18.210965 opensr-test-0.0.1/setup.cfg
--rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1395 2023-07-12 18:54:07.000000 opensr-test-0.0.1/setup.py
+drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-13 09:46:17.397294 opensr-test-0.0.2/
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1077 2023-07-12 18:42:54.000000 opensr-test-0.0.2/LICENSE
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14757 2023-07-13 09:46:17.397294 opensr-test-0.0.2/PKG-INFO
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14135 2023-07-12 19:05:04.000000 opensr-test-0.0.2/README.md
+drwxrwxr-x   0 csaybar   (1000) csaybar   (1000)        0 2023-07-13 09:46:17.397294 opensr-test-0.0.2/opensr_test.egg-info/
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)    14757 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/PKG-INFO
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)      200 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       61 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/requires.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)        1 2023-07-13 09:46:17.000000 opensr-test-0.0.2/opensr_test.egg-info/top_level.txt
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)       38 2023-07-13 09:46:17.397294 opensr-test-0.0.2/setup.cfg
+-rw-rw-r--   0 csaybar   (1000) csaybar   (1000)     1295 2023-07-13 09:46:07.000000 opensr-test-0.0.2/setup.py
```

### Comparing `opensr-test-0.0.1/LICENSE` & `opensr-test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opensr-test-0.0.1/PKG-INFO` & `opensr-test-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-Home-page: https://github.com/ESAOpenSR/opensr-check
+Home-page: https://github.com/ESAOpenSR/opensr-test
 Author: Cesar Aybar Camacho
 Author-email: csaybar@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://github.com/ESAOpenSR/opensr-check"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
+  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
 </p>[Title](https://github.com/ESAOpenSR/opensr-check)
 
 <p align="center">
     <em>A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution</em>
 </p>
 
 <p align="center">
-<a href='https://pypi.python.org/pypi/srcheck'>
-    <img src='https://img.shields.io/pypi/v/srcheck.svg' alt='PyPI' />
-</a>
-<a href='https://anaconda.org/conda-forge/srcheck'>
-    <img src='https://img.shields.io/conda/vn/conda-forge/srcheck.svg' alt='conda-forge' />
+<a href='https://pypi.python.org/pypi/opensr-test'>
+    <img src='https://img.shields.io/pypi/v/opensr-test.svg' alt='PyPI' />
 </a>
+
 <a href="https://opensource.org/licenses/MIT" target="_blank">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
 </a>
-<a href='https://srcheck.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/eemont/badge/?version=latest' alt='Documentation Status' />
+<a href='https://opensr-test.readthedocs.io/en/latest/?badge=latest'>
+    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href="https://github.com/psf/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
 </a>
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
 </a>
 </p>
 
 ---
 
-**GitHub**: [https://github.com/csaybar/srcheck](https://github.com/csaybar/srcheck)
-
-**Documentation**: [https://srcheck.readthedocs.io/](https://srcheck.readthedocs.io/)
-
-**PyPI**: [https://pypi.org/project/srcheck/](https://pypi.org/project/srcheck/)
+**GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Conda-forge**: [https://anaconda.org/conda-forge/srcheck](https://anaconda.org/conda-forge/srcheck)
+**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
 
-**Tutorials**: [https://github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/davemlz/srcheck/tree/master/docs/tutorials)
+**PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.0.1 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.0.2 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
-/github.com/ESAOpenSR/opensr-check Author: Cesar Aybar Camacho Author-email:
+/github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
 csaybar@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown License-File: LICENSE
+Language :: Python :: 3.8 Description-Content-Type: text/markdown License-File:
+LICENSE
                                    [header]
 [Title](https://github.com/ESAOpenSR/opensr-check)
  A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-     [PyPI] [conda-forge] [License] [Documentation_Status] [Black] [isort]
---- **GitHub**: [https://github.com/csaybar/srcheck](https://github.com/
-csaybar/srcheck) **Documentation**: [https://srcheck.readthedocs.io/](https://
-srcheck.readthedocs.io/) **PyPI**: [https://pypi.org/project/srcheck/](https://
-pypi.org/project/srcheck/) **Conda-forge**: [https://anaconda.org/conda-forge/
-srcheck](https://anaconda.org/conda-forge/srcheck) **Tutorials**: [https://
-github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/
-davemlz/srcheck/tree/master/docs/tutorials) **Paper**: Coming soon! --- ##
-Overview In remote sensing, image super-resolution (ISR) is a technique used to
-create high-resolution (HR) images from low-resolution (R) satellite images,
-giving a more detailed view of the Earth's surface. However, with the constant
-development and introduction of new ISR algorithms, it can be challenging to
-stay updated on the latest advancements and to evaluate their performance
-objectively. To address this issue, we introduce SRcheck, a Python package that
-provides an easy-to-use interface for comparing and benchmarking various ISR
-methods. SRcheck includes a range of datasets that consist of high-resolution
-and low-resolution image pairs, as well as a set of quantitative metrics for
-evaluating the performance of SISR algorithms. ## Installation Install the
-latest version from PyPI: ``` pip install srcheck ``` Upgrade `srcheck` by
-running: ``` pip install -U srcheck ``` Install the latest version from conda-
-forge: ``` conda install -c conda-forge srcheck ``` Install the latest dev
-version from GitHub by running: ``` pip install git+https://github.com/csaybar/
-srcheck ``` ## How does it work?
+            [PyPI] [License] [Documentation_Status] [Black] [isort]
+--- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
+ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
+(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
+opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
+- ## Overview In remote sensing, image super-resolution (ISR) is a technique
+used to create high-resolution (HR) images from low-resolution (R) satellite
+images, giving a more detailed view of the Earth's surface. However, with the
+constant development and introduction of new ISR algorithms, it can be
+challenging to stay updated on the latest advancements and to evaluate their
+performance objectively. To address this issue, we introduce SRcheck, a Python
+package that provides an easy-to-use interface for comparing and benchmarking
+various ISR methods. SRcheck includes a range of datasets that consist of high-
+resolution and low-resolution image pairs, as well as a set of quantitative
+metrics for evaluating the performance of SISR algorithms. ## Installation
+Install the latest version from PyPI: ``` pip install srcheck ``` Upgrade
+`srcheck` by running: ``` pip install -U srcheck ``` Install the latest version
+from conda-forge: ``` conda install -c conda-forge srcheck ``` Install the
+latest dev version from GitHub by running: ``` pip install git+https://
+github.com/csaybar/srcheck ``` ## How does it work?
                                    [header]
 **srcheck** needs either a `torch.nn.Module` class or a compiled model via
 `torch.jit.trace` or `torch.jit.script`. The following example shows how to run
 the benchmarks: ```python import torch import srcheck model = torch.jit.load('/
 content/quantSRmodel.pt', map_location='cpu') srcheck.benchmark(model,
 dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI") ``` srcheck
 supports two group types of metrics: (a) Surface Reflectance Integrity (SRI)
```

### Comparing `opensr-test-0.0.1/README.md` & `opensr-test-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 <p align="center">
-  <a href="https://github.com/ESAOpenSR/opensr-check"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
+  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
 </p>[Title](https://github.com/ESAOpenSR/opensr-check)
 
 <p align="center">
     <em>A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution</em>
 </p>
 
 <p align="center">
-<a href='https://pypi.python.org/pypi/srcheck'>
-    <img src='https://img.shields.io/pypi/v/srcheck.svg' alt='PyPI' />
-</a>
-<a href='https://anaconda.org/conda-forge/srcheck'>
-    <img src='https://img.shields.io/conda/vn/conda-forge/srcheck.svg' alt='conda-forge' />
+<a href='https://pypi.python.org/pypi/opensr-test'>
+    <img src='https://img.shields.io/pypi/v/opensr-test.svg' alt='PyPI' />
 </a>
+
 <a href="https://opensource.org/licenses/MIT" target="_blank">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
 </a>
-<a href='https://srcheck.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/eemont/badge/?version=latest' alt='Documentation Status' />
+<a href='https://opensr-test.readthedocs.io/en/latest/?badge=latest'>
+    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href="https://github.com/psf/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
 </a>
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
 </a>
 </p>
 
 ---
 
-**GitHub**: [https://github.com/csaybar/srcheck](https://github.com/csaybar/srcheck)
-
-**Documentation**: [https://srcheck.readthedocs.io/](https://srcheck.readthedocs.io/)
-
-**PyPI**: [https://pypi.org/project/srcheck/](https://pypi.org/project/srcheck/)
+**GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Conda-forge**: [https://anaconda.org/conda-forge/srcheck](https://anaconda.org/conda-forge/srcheck)
+**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
 
-**Tutorials**: [https://github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/davemlz/srcheck/tree/master/docs/tutorials)
+**PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,33 +1,30 @@
                                    [header]
 [Title](https://github.com/ESAOpenSR/opensr-check)
  A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-     [PyPI] [conda-forge] [License] [Documentation_Status] [Black] [isort]
---- **GitHub**: [https://github.com/csaybar/srcheck](https://github.com/
-csaybar/srcheck) **Documentation**: [https://srcheck.readthedocs.io/](https://
-srcheck.readthedocs.io/) **PyPI**: [https://pypi.org/project/srcheck/](https://
-pypi.org/project/srcheck/) **Conda-forge**: [https://anaconda.org/conda-forge/
-srcheck](https://anaconda.org/conda-forge/srcheck) **Tutorials**: [https://
-github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/
-davemlz/srcheck/tree/master/docs/tutorials) **Paper**: Coming soon! --- ##
-Overview In remote sensing, image super-resolution (ISR) is a technique used to
-create high-resolution (HR) images from low-resolution (R) satellite images,
-giving a more detailed view of the Earth's surface. However, with the constant
-development and introduction of new ISR algorithms, it can be challenging to
-stay updated on the latest advancements and to evaluate their performance
-objectively. To address this issue, we introduce SRcheck, a Python package that
-provides an easy-to-use interface for comparing and benchmarking various ISR
-methods. SRcheck includes a range of datasets that consist of high-resolution
-and low-resolution image pairs, as well as a set of quantitative metrics for
-evaluating the performance of SISR algorithms. ## Installation Install the
-latest version from PyPI: ``` pip install srcheck ``` Upgrade `srcheck` by
-running: ``` pip install -U srcheck ``` Install the latest version from conda-
-forge: ``` conda install -c conda-forge srcheck ``` Install the latest dev
-version from GitHub by running: ``` pip install git+https://github.com/csaybar/
-srcheck ``` ## How does it work?
+            [PyPI] [License] [Documentation_Status] [Black] [isort]
+--- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
+ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
+(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
+opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
+- ## Overview In remote sensing, image super-resolution (ISR) is a technique
+used to create high-resolution (HR) images from low-resolution (R) satellite
+images, giving a more detailed view of the Earth's surface. However, with the
+constant development and introduction of new ISR algorithms, it can be
+challenging to stay updated on the latest advancements and to evaluate their
+performance objectively. To address this issue, we introduce SRcheck, a Python
+package that provides an easy-to-use interface for comparing and benchmarking
+various ISR methods. SRcheck includes a range of datasets that consist of high-
+resolution and low-resolution image pairs, as well as a set of quantitative
+metrics for evaluating the performance of SISR algorithms. ## Installation
+Install the latest version from PyPI: ``` pip install srcheck ``` Upgrade
+`srcheck` by running: ``` pip install -U srcheck ``` Install the latest version
+from conda-forge: ``` conda install -c conda-forge srcheck ``` Install the
+latest dev version from GitHub by running: ``` pip install git+https://
+github.com/csaybar/srcheck ``` ## How does it work?
                                    [header]
 **srcheck** needs either a `torch.nn.Module` class or a compiled model via
 `torch.jit.trace` or `torch.jit.script`. The following example shows how to run
 the benchmarks: ```python import torch import srcheck model = torch.jit.load('/
 content/quantSRmodel.pt', map_location='cpu') srcheck.benchmark(model,
 dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI") ``` srcheck
 supports two group types of metrics: (a) Surface Reflectance Integrity (SRI)
```

### Comparing `opensr-test-0.0.1/opensr_test.egg-info/PKG-INFO` & `opensr-test-0.0.2/opensr_test.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 Metadata-Version: 2.1
 Name: opensr-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-Home-page: https://github.com/ESAOpenSR/opensr-check
+Home-page: https://github.com/ESAOpenSR/opensr-test
 Author: Cesar Aybar Camacho
 Author-email: csaybar@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <a href="https://github.com/ESAOpenSR/opensr-check"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
+  <a href="https://github.com/ESAOpenSR/opensr-test"><img src="https://user-images.githubusercontent.com/16768318/213960001-66bb7d18-13d8-41d4-9de3-1e8a77f73787.png" alt="header" width="55%"></a>
 </p>[Title](https://github.com/ESAOpenSR/opensr-check)
 
 <p align="center">
     <em>A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution</em>
 </p>
 
 <p align="center">
-<a href='https://pypi.python.org/pypi/srcheck'>
-    <img src='https://img.shields.io/pypi/v/srcheck.svg' alt='PyPI' />
-</a>
-<a href='https://anaconda.org/conda-forge/srcheck'>
-    <img src='https://img.shields.io/conda/vn/conda-forge/srcheck.svg' alt='conda-forge' />
+<a href='https://pypi.python.org/pypi/opensr-test'>
+    <img src='https://img.shields.io/pypi/v/opensr-test.svg' alt='PyPI' />
 </a>
+
 <a href="https://opensource.org/licenses/MIT" target="_blank">
     <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
 </a>
-<a href='https://srcheck.readthedocs.io/en/latest/?badge=latest'>
-    <img src='https://readthedocs.org/projects/eemont/badge/?version=latest' alt='Documentation Status' />
+<a href='https://opensr-test.readthedocs.io/en/latest/?badge=latest'>
+    <img src='https://readthedocs.org/projects/opensr-test/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href="https://github.com/psf/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
 </a>
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
 </a>
 </p>
 
 ---
 
-**GitHub**: [https://github.com/csaybar/srcheck](https://github.com/csaybar/srcheck)
-
-**Documentation**: [https://srcheck.readthedocs.io/](https://srcheck.readthedocs.io/)
-
-**PyPI**: [https://pypi.org/project/srcheck/](https://pypi.org/project/srcheck/)
+**GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/ESAOpenSR/opensr-test)
 
-**Conda-forge**: [https://anaconda.org/conda-forge/srcheck](https://anaconda.org/conda-forge/srcheck)
+**Documentation**: [https://opensr-test.readthedocs.io/](https://opensr-test.readthedocs.io/)
 
-**Tutorials**: [https://github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/davemlz/srcheck/tree/master/docs/tutorials)
+**PyPI**: [https://pypi.org/project/opensr-test/](https://pypi.org/project/opensr-test/)
 
 **Paper**: Coming soon!
 
 ---
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,43 +1,39 @@
-Metadata-Version: 2.1 Name: opensr-test Version: 0.0.1 Summary: A comprehensive
+Metadata-Version: 2.1 Name: opensr-test Version: 0.0.2 Summary: A comprehensive
 benchmark for real-world Sentinel-2 imagery super-resolution Home-page: https:/
-/github.com/ESAOpenSR/opensr-check Author: Cesar Aybar Camacho Author-email:
+/github.com/ESAOpenSR/opensr-test Author: Cesar Aybar Camacho Author-email:
 csaybar@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown License-File: LICENSE
+Language :: Python :: 3.8 Description-Content-Type: text/markdown License-File:
+LICENSE
                                    [header]
 [Title](https://github.com/ESAOpenSR/opensr-check)
  A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution
-     [PyPI] [conda-forge] [License] [Documentation_Status] [Black] [isort]
---- **GitHub**: [https://github.com/csaybar/srcheck](https://github.com/
-csaybar/srcheck) **Documentation**: [https://srcheck.readthedocs.io/](https://
-srcheck.readthedocs.io/) **PyPI**: [https://pypi.org/project/srcheck/](https://
-pypi.org/project/srcheck/) **Conda-forge**: [https://anaconda.org/conda-forge/
-srcheck](https://anaconda.org/conda-forge/srcheck) **Tutorials**: [https://
-github.com/davemlz/srcheck/tree/master/docs/tutorials](https://github.com/
-davemlz/srcheck/tree/master/docs/tutorials) **Paper**: Coming soon! --- ##
-Overview In remote sensing, image super-resolution (ISR) is a technique used to
-create high-resolution (HR) images from low-resolution (R) satellite images,
-giving a more detailed view of the Earth's surface. However, with the constant
-development and introduction of new ISR algorithms, it can be challenging to
-stay updated on the latest advancements and to evaluate their performance
-objectively. To address this issue, we introduce SRcheck, a Python package that
-provides an easy-to-use interface for comparing and benchmarking various ISR
-methods. SRcheck includes a range of datasets that consist of high-resolution
-and low-resolution image pairs, as well as a set of quantitative metrics for
-evaluating the performance of SISR algorithms. ## Installation Install the
-latest version from PyPI: ``` pip install srcheck ``` Upgrade `srcheck` by
-running: ``` pip install -U srcheck ``` Install the latest version from conda-
-forge: ``` conda install -c conda-forge srcheck ``` Install the latest dev
-version from GitHub by running: ``` pip install git+https://github.com/csaybar/
-srcheck ``` ## How does it work?
+            [PyPI] [License] [Documentation_Status] [Black] [isort]
+--- **GitHub**: [https://github.com/ESAOpenSR/opensr-test](https://github.com/
+ESAOpenSR/opensr-test) **Documentation**: [https://opensr-test.readthedocs.io/]
+(https://opensr-test.readthedocs.io/) **PyPI**: [https://pypi.org/project/
+opensr-test/](https://pypi.org/project/opensr-test/) **Paper**: Coming soon! --
+- ## Overview In remote sensing, image super-resolution (ISR) is a technique
+used to create high-resolution (HR) images from low-resolution (R) satellite
+images, giving a more detailed view of the Earth's surface. However, with the
+constant development and introduction of new ISR algorithms, it can be
+challenging to stay updated on the latest advancements and to evaluate their
+performance objectively. To address this issue, we introduce SRcheck, a Python
+package that provides an easy-to-use interface for comparing and benchmarking
+various ISR methods. SRcheck includes a range of datasets that consist of high-
+resolution and low-resolution image pairs, as well as a set of quantitative
+metrics for evaluating the performance of SISR algorithms. ## Installation
+Install the latest version from PyPI: ``` pip install srcheck ``` Upgrade
+`srcheck` by running: ``` pip install -U srcheck ``` Install the latest version
+from conda-forge: ``` conda install -c conda-forge srcheck ``` Install the
+latest dev version from GitHub by running: ``` pip install git+https://
+github.com/csaybar/srcheck ``` ## How does it work?
                                    [header]
 **srcheck** needs either a `torch.nn.Module` class or a compiled model via
 `torch.jit.trace` or `torch.jit.script`. The following example shows how to run
 the benchmarks: ```python import torch import srcheck model = torch.jit.load('/
 content/quantSRmodel.pt', map_location='cpu') srcheck.benchmark(model,
 dataset='SPOT-50', metrics=['PSNR', 'SSIM'], type= "NoSRI") ``` srcheck
 supports two group types of metrics: (a) Surface Reflectance Integrity (SRI)
```

### Comparing `opensr-test-0.0.1/setup.py` & `opensr-test-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     text_type = type("")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="opensr-test",
-    version="0.0.1",
-    url="https://github.com/ESAOpenSR/opensr-check",
+    version="0.0.2",
+    url="https://github.com/ESAOpenSR/opensr-test",
     license="MIT",
     author="Cesar Aybar Camacho",
     author_email="csaybar@gmail.com",
     description="A comprehensive benchmark for real-world Sentinel-2 imagery super-resolution",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",), include=["opensr-test", "opensr-test.*"]),    
@@ -34,12 +34,10 @@
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.8"
     ],
 )
```

