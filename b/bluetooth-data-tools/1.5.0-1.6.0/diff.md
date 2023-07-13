# Comparing `tmp/bluetooth_data_tools-1.5.0.tar.gz` & `tmp/bluetooth_data_tools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_data_tools-1.5.0.tar", max compression
+gzip compressed data, was "bluetooth_data_tools-1.6.0.tar", max compression
```

## Comparing `bluetooth_data_tools-1.5.0.tar` & `bluetooth_data_tools-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11345 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/LICENSE
--rw-r--r--   0        0        0     3598 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/README.md
--rw-r--r--   0        0        0     1168 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/build_ext.py
--rw-r--r--   0        0        0     2471 2023-07-13 06:26:36.356814 bluetooth_data_tools-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1900 2023-07-13 06:26:36.316814 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/__init__.py
--rw-r--r--   0        0        0      536 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/_utils_impl.pyx
--rw-r--r--   0        0        0     1300 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/gap.pxd
--rw-r--r--   0        0        0     7939 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/gap.py
--rw-r--r--   0        0        0        0 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/py.typed
--rw-r--r--   0        0        0      576 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/utils.py
--rw-r--r--   0        0        0      431 2023-07-13 06:26:35.568806 bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/utils_wrapper.h
--rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 bluetooth_data_tools-1.5.0/setup.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 bluetooth_data_tools-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3598 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/README.md
+-rw-r--r--   0        0        0     1168 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/build_ext.py
+-rw-r--r--   0        0        0     2471 2023-07-13 06:36:20.080267 bluetooth_data_tools-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1900 2023-07-13 06:36:20.032265 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/_utils_impl.pyx
+-rw-r--r--   0        0        0     1398 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/gap.pxd
+-rw-r--r--   0        0        0     8165 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/gap.py
+-rw-r--r--   0        0        0        0 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/py.typed
+-rw-r--r--   0        0        0      576 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/utils.py
+-rw-r--r--   0        0        0      431 2023-07-13 06:36:19.108219 bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/utils_wrapper.h
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 bluetooth_data_tools-1.6.0/setup.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 bluetooth_data_tools-1.6.0/PKG-INFO
```

### Comparing `bluetooth_data_tools-1.5.0/LICENSE` & `bluetooth_data_tools-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-1.5.0/README.md` & `bluetooth_data_tools-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-1.5.0/build_ext.py` & `bluetooth_data_tools-1.6.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-1.5.0/pyproject.toml` & `bluetooth_data_tools-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-data-tools"
-version = "1.5.0"
+version = "1.6.0"
 description = "Tools for converting bluetooth data and packets"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/bluetooth-data-tools"
 documentation = "https://bluetooth-data-tools.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/__init__.py` & `bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from struct import Struct
 
 from .gap import BLEGAPAdvertisement, BLEGAPType, parse_advertisement_data
 from .utils import int_to_bluetooth_address
 
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 L_PACK = Struct(">L")
 
 __all__ = [
     "address_to_bytes",
     "manufacturer_data_to_raw",
     "newest_manufacturer_data",
```

### Comparing `bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/_utils_impl.pyx` & `bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/_utils_impl.pyx`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/gap.pxd` & `bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/gap.pxd`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 cdef object from_bytes_little
 cdef object from_bytes_signed
 
 cdef object _cached_uint64_bytes_as_uuid
 cdef object _cached_uint16_bytes_as_uuid
 cdef object _cached_uint32_bytes_as_uuid
 cdef object _cached_uint128_bytes_as_uuid
+cdef object _cached_parse_advertisement_data
 
 cdef object _LOGGER
 
 cdef class BLEGAPAdvertisement:
 
     cdef public object local_name
     cdef public object service_uuids
@@ -30,19 +31,20 @@
 cdef cython.uint TYPE_128BIT_SERVICE_UUID_COMPLETE
 cdef cython.uint TYPE_128BIT_SERVICE_UUID_MORE_AVAILABLE
 cdef cython.uint TYPE_SERVICE_DATA
 cdef cython.uint TYPE_SERVICE_DATA_32BIT_UUID
 cdef cython.uint TYPE_SERVICE_DATA_128BIT_UUID
 cdef cython.uint TYPE_TX_POWER_LEVEL
 
+cpdef parse_advertisement_data(object data)
 
 @cython.locals(
     gap_data=cython.bytes,
     gap_value=cython.bytes,
     gap_type_num=cython.uint,
     total_length=cython.uint,
     length=cython.uint,
     offset=cython.uint,
     start=cython.uint,
     end=cython.uint,
 )
-cpdef parse_advertisement_data(object data)
+cpdef _uncached_parse_advertisement_data(tuple data)
```

### Comparing `bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/gap.py` & `bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/gap.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,28 +134,37 @@
     """Convert manufacturer ID bytes to an int."""
     return from_bytes_little(manufacturer_id_bytes)
 
 
 _cached_manufacturer_id_bytes_to_int = _manufacturer_id_bytes_to_int
 
 
+@lru_cache(maxsize=256)
+def _parse_advertisement_data(
+    data: Tuple[bytes, ...],
+) -> BLEGAPAdvertisement:
+    """Parse advertisement data."""
+    return _uncached_parse_advertisement_data(data)
+
+
+_cached_parse_advertisement_data = _parse_advertisement_data
+
+
 def parse_advertisement_data(
     data: Iterable[bytes],
 ) -> BLEGAPAdvertisement:
     """Parse advertisement data."""
     if type(data) is tuple:
-        return _parse_advertisement_data(data)
-    return _parse_advertisement_data(tuple(data))
+        return _cached_parse_advertisement_data(data)
+    return _cached_parse_advertisement_data(tuple(data))
 
 
-@lru_cache(maxsize=256)
-def _parse_advertisement_data(
+def _uncached_parse_advertisement_data(
     data: Tuple[bytes, ...],
 ) -> BLEGAPAdvertisement:
-    """Parse advertisement data."""
     manufacturer_data: Dict[int, bytes] = {}
     service_data: Dict[str, bytes] = {}
     service_uuids: List[str] = []
     local_name: str | None = None
     tx_power: int | None = None
 
     for gap_data in data:
```

### Comparing `bluetooth_data_tools-1.5.0/src/bluetooth_data_tools/utils.py` & `bluetooth_data_tools-1.6.0/src/bluetooth_data_tools/utils.py`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-1.5.0/setup.py` & `bluetooth_data_tools-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'bluetooth-data-tools',
-    'version': '1.5.0',
+    'version': '1.6.0',
     'description': 'Tools for converting bluetooth data and packets',
     'long_description': '# Bluetooth Data Tools\n\n<p align="center">\n  <a href="https://github.com/bdraco/bluetooth-data-tools/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bdraco/bluetooth-data-tools/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://bluetooth-data-tools.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/bluetooth-data-tools.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bdraco/bluetooth-data-tools">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/bluetooth-data-tools.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/bluetooth-data-tools/">\n    <img src="https://img.shields.io/pypi/v/bluetooth-data-tools.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/bluetooth-data-tools.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/bluetooth-data-tools.svg?style=flat-square" alt="License">\n</p>\n\nTools for converting bluetooth data and packets\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install bluetooth-data-tools`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/bluetooth-data-tools',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['bluetooth_data_tools'] package_data = \ {'': ['*']}
 extras_require = \ {'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0',
 'myst-parser>=0.18,<0.19']} setup_kwargs = { 'name': 'bluetooth-data-tools',
-'version': '1.5.0', 'description': 'Tools for converting bluetooth data and
+'version': '1.6.0', 'description': 'Tools for converting bluetooth data and
 packets', 'long_description': '# Bluetooth Data Tools\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `bluetooth_data_tools-1.5.0/PKG-INFO` & `bluetooth_data_tools-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-data-tools
-Version: 1.5.0
+Version: 1.6.0
 Summary: Tools for converting bluetooth data and packets
 Home-page: https://github.com/bdraco/bluetooth-data-tools
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bluetooth-data-tools Version: 1.5.0 Summary: Tools
+Metadata-Version: 2.1 Name: bluetooth-data-tools Version: 1.6.0 Summary: Tools
 for converting bluetooth data and packets Home-page: https://github.com/bdraco/
 bluetooth-data-tools License: Apache Software License 2.0 Author: J. Nick
 Koston Author-email: nick@koston.org Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

