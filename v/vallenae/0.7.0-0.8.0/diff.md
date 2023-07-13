# Comparing `tmp/vallenae-0.7.0.tar.gz` & `tmp/vallenae-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vallenae-0.7.0.tar", last modified: Thu Nov 10 12:31:55 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `vallenae-0.7.0.tar` & `vallenae-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-11-10 12:31:45.000000 vallenae-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2022-11-10 12:31:55.091392 vallenae-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2599 2022-11-10 12:31:45.000000 vallenae-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2091 2022-11-10 12:31:45.000000 vallenae-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-10 12:31:55.091392 vallenae-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2865 2022-11-10 12:31:45.000000 vallenae-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.087392 vallenae-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.087392 vallenae-0.7.0/src/vallenae/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/_numba.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/src/vallenae/_pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)      257 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/_pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/_pyinstaller/hook-vallenae.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/_pyinstaller/test_pyinstaller_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/src/vallenae/features/
--rw-r--r--   0 runner    (1001) docker     (122)      503 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/features/acoustic_emission.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/features/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/src/vallenae/io/
--rw-r--r--   0 runner    (1001) docker     (122)     2370 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9178 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/_database.py
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)    12736 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/_sql.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/compression.py
--rw-r--r--   0 runner    (1001) docker     (122)     8467 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)    20378 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/pridb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/src/vallenae/io/schema_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/schema_templates/pridb.sql
--rw-r--r--   0 runner    (1001) docker     (122)     2100 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/schema_templates/tradb.sql
--rw-r--r--   0 runner    (1001) docker     (122)      709 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/schema_templates/trfdb.sql
--rw-r--r--   0 runner    (1001) docker     (122)    15021 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/tradb.py
--rw-r--r--   0 runner    (1001) docker     (122)     5474 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/trfdb.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/io/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.091392 vallenae-0.7.0/src/vallenae/timepicker/
--rw-r--r--   0 runner    (1001) docker     (122)     8537 2022-11-10 12:31:45.000000 vallenae-0.7.0/src/vallenae/timepicker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-10 12:31:55.087392 vallenae-0.7.0/src/vallenae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      992 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      425 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-10 12:31:55.000000 vallenae-0.7.0/src/vallenae.egg-info/top_level.txt
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vallenae-0.8.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 vallenae-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 vallenae-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/features.rst
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/io.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/timepicker.rst
+-rw-r--r--   0        0        0    84140 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/images/vae_arrival_time_offset.png
+-rw-r--r--   0        0        0    81388 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/images/vae_custom_features.png
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/templates/autosummary/base.rst
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/templates/autosummary/class.rst
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 vallenae-0.8.0/docs/templates/autosummary/module.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/README.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/_feature_extraction.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex1_read_pridb.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex2_read_tradb.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex3_timepicker.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex4_timepicker_batch.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex5_location.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex6_multiprocessing.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex7_custom_feature_extraction.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex8_spectrogram.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/ex9_wavexport.py
+-rw-r--r--   0        0        0   147456 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/bearing/bearing.pridb
+-rw-r--r--   0        0        0  3145728 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/bearing/bearing.tradb
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/bearing/bearing.vaex
+-rw-r--r--   0        0        0  5087232 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/bearing/bearing_plain.tradb
+-rw-r--r--   0        0        0    98304 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/steel_plate/sample.pridb
+-rw-r--r--   0        0        0   237568 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/steel_plate/sample.tradb
+-rw-r--r--   0        0        0    49152 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/steel_plate/sample.trfdb
+-rw-r--r--   0        0        0    12789 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/steel_plate/sample.vaex
+-rw-r--r--   0        0        0   860160 2020-02-02 00:00:00.000000 vallenae-0.8.0/examples/steel_plate/sample_plain.tradb
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/__init__.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/_numba.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/_pyinstaller/hook-vallenae.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/_pyinstaller/test_pyinstaller_hook.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/features/__init__.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/features/acoustic_emission.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/features/conversion.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/__init__.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/_database.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/_dataframe.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/_sql.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/compression.py
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/datatypes.py
+-rw-r--r--   0        0        0    20244 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/pridb.py
+-rw-r--r--   0        0        0    15362 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/tradb.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/trfdb.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/types.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/schema_templates/pridb.sql
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/schema_templates/tradb.sql
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/io/schema_templates/trfdb.sql
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 vallenae-0.8.0/src/vallenae/timepicker/__init__.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_benchmarks.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_features.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_compression.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_database.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_dataframe.py
+-rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_pridb.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_sql.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_tradb.py
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_io_trfdb.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/test_timepicker.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/data/gen_signal.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/data/signal-flac.tradb
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/data/signal-raw.tradb
+-rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 vallenae-0.8.0/tests/data/signal.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 vallenae-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 vallenae-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 vallenae-0.8.0/README.md
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 vallenae-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 vallenae-0.8.0/PKG-INFO
```

### Comparing `vallenae-0.7.0/LICENSE.txt` & `vallenae-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/README.md` & `vallenae-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,64 +3,66 @@
 [![CI](https://github.com/vallen-systems/pyVallenAE/workflows/CI/badge.svg)](https://github.com/vallen-systems/pyVallenAE/actions)
 [![Documentation Status](https://readthedocs.org/projects/pyvallenae/badge/?version=latest)](https://pyvallenae.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/vallen-systems/pyVallenAE/badge.svg?branch=master)](https://coveralls.io/github/vallen-systems/pyVallenAE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/vallenae)](https://pypi.org/project/vallenae)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vallenae)](https://pypi.org/project/vallenae)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
+**[Documentation](https://pyvallenae.readthedocs.io/) · [Examples](https://pyvallenae.readthedocs.io/en/stable/examples)**
 
-Python tools to extract and analyze Acoustic Emission measurement data:
+Python tools to extract and analyze Acoustic Emission measurement data.
+The package includes following modules:
 
 - vallenae.**io**: Reading (and writing) of Vallen Systeme SQLite database files (*.pridb, *.tradb, *.trfdb)
 - vallenae.**features**: Extraction of Acoustic Emission features
 - vallenae.**timepicker**: Timepicking algorithms for arrival time estimations
 
----
-**Note**: A free/lite version of the Vallen AE Suite is available since the release R2020.
-If offers the basic features for real-time data visualization and analysis with VisualAE.
-So you could write you own pridb/tradb files and have real-time visualizations with VisualAE.
-
-The Vallen AE Suite can be downloaded here: https://www.vallen.de/downloads/
-
----
-
-## Documentation
-
-For full documentation and examples, please visit http://pyvallenae.rtfd.io.
+> **Note**:
+> A free/lite version of the Vallen AE Suite is available since the release R2020.
+> If offers the basic features for real-time data visualization and analysis with VisualAE.
+> So you could write you own pridb/tradb files and have real-time visualizations with VisualAE.
+>
+> The Vallen AE Suite can be downloaded [here](https://www.vallen.de/downloads/).
 
 ## Installation
 
-Install the latest version from PyPI:
+Install the latest version from [PyPI](https://pypi.org/project/vallenae):
 
+```shell
+$ pip install vallenae
 ```
-pip install vallenae
+
+If you want to run the latest version of the code, you can install from the master branch directly:
+
+```shell
+$ pip install -U git+https://github.com/vallen-systems/pyVallenAE.git
+# Or if you don't have git installed
+$ pip install -U https://github.com/vallen-systems/pyVallenAE/zipball/master
 ```
 
 Please note, that `vallenae` requires Python 3.6 or newer. On Linux systems, `pip` is usually mapped to Python 2, so use `pip<version>` (e.g. `pip3` or `pip3.7`) instead. Alternatively, you can run `pip` from your specific Python version with `python<version> -m pip`.
 
 ## Contributing
 
 Feature requests, bug reports and fixes are always welcome!
+Just [create an issue](https://github.com/vallen-systems/pyVallenAE/issues/new) or make a pull-request.
 
-After cloning the repository, you can easily install the development environment and tools 
-([pylint](https://www.pylint.org), [mypy](http://mypy-lang.org), [pytest](https://pytest.org), [tox](https://tox.readthedocs.io))
-with:
+### Development setup
 
-```
-git clone https://github.com/vallen-systems/pyVallenAE.git
-cd pyVallenAE
-pip install -e .[dev]
-```
-
-And run the test suite with tox:
+```shell
+# Clone this repository
+$ git clone https://github.com/vallen-systems/pyVallenAE.git
+$ cd pyVallenAE
 
-```
-tox
-```
+# Install package and dependencies
+$ pip install -e .[dev]
 
-The documentation is built with [sphinx](https://www.sphinx-doc.org):
+# Run the test suite with tox
+$ tox
 
-```
-cd docs
-sphinx-build . _build
+# Build the documentation with Sphinx
+$ cd docs
+$ make html  # on Linux
+$ ./make.bat html  # on Windows
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vallenae-0.7.0/src/vallenae/_numba.py` & `vallenae-0.8.0/src/vallenae/_numba.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Optional usage of numba with njit decorator."""
 
 import warnings
 
 USE_NUMBA = True
 
 try:
-    from numba import njit  # pylint: disable=unused-import
+    from numba import njit
 except ImportError:
     USE_NUMBA = False
+
     # https://stackoverflow.com/a/73275170/9967707
-    def njit(f = None, *args, **kwargs):  # pylint: disable=keyword-arg-before-vararg,unused-argument
+    def njit(f=None, *args, **kwargs):
         if callable(f):
             return f
         return lambda func: func
 
 
 class PerformanceWarning(Warning):
     """Warning raised when there is a possible performance impact."""
 
 
 if not USE_NUMBA:
     warnings.warn(
         "Numba not found. Use Numba (pip install numba) for better performance.",
         PerformanceWarning,
+        stacklevel=1,
     )
```

### Comparing `vallenae-0.7.0/src/vallenae/_pyinstaller/test_pyinstaller_hook.py` & `vallenae-0.8.0/src/vallenae/_pyinstaller/test_pyinstaller_hook.py`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/features/acoustic_emission.py` & `vallenae-0.8.0/src/vallenae/features/acoustic_emission.py`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/features/conversion.py` & `vallenae-0.8.0/src/vallenae/features/conversion.py`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/io/__init__.py` & `vallenae-0.8.0/src/vallenae/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/io/_database.py` & `vallenae-0.8.0/src/vallenae/io/_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 from ._sql import ConnectionWrapper, insert_from_dict, read_sql_generator, update_from_dict
 
 
 def require_write_access(func):
     @wraps(func)
     def wrapper(self: "Database", *args, **kwargs):
-        if self._readonly:  # pylint: disable=protected-access
+        if self._readonly:
             raise ValueError(
                 "Can not write to database in read-only mode. Open database with mode='rw'"
             )
         return func(self, *args, **kwargs)
+
     return wrapper
 
 
 class Database:
     """Database base class for pridb, tradb and trfdb."""
 
     __metaclass__ = ABCMeta
@@ -36,19 +37,18 @@
         if required_file_ext is not None:
             file_ext = Path(filename).suffix
             if file_ext.lower() != required_file_ext.lower():
                 raise ValueError(
                     f"File {filename} does not have the required extension {required_file_ext}"
                 )
 
-        if mode == "rwc":
-            if not Path(filename).exists():
-                self.create(filename)  # call abstract method (implemented by child class)
+        if mode == "rwc" and not Path(filename).exists():
+            self.create(filename)  # call abstract method (implemented by child class)
 
-        self._readonly = (mode == "ro")
+        self._readonly = mode == "ro"
         self._connection_wrapper = ConnectionWrapper(filename, mode)
 
         self._table_prefix: str = table_prefix
         self._table_main: str = f"{table_prefix}_data"
         self._table_fieldinfo: str = f"{table_prefix}_fieldinfo"
         self._table_globalinfo: str = f"{table_prefix}_globalinfo"
         self._table_params: str = f"{table_prefix}_params"
@@ -122,16 +122,15 @@
                 if column not in columns_exist:
                     con.execute(f"ALTER TABLE {table} ADD COLUMN {column} {dtype}")
 
     def tables(self) -> Set[str]:
         """Get table names."""
         con = self.connection()
         cur = con.execute("SELECT name FROM sqlite_master WHERE type == 'table'")
-        tables = {result[0] for result in cur.fetchall()}
-        return tables
+        return {result[0] for result in cur.fetchall()}
 
     def fieldinfo(self) -> Dict[str, Dict[str, Any]]:
         """
         Read fieldinfo table.
 
         The fieldinfo table stores informations about columns of the data table (like units).
 
@@ -157,72 +156,81 @@
         if field not in self.columns():
             raise ValueError(f"Field {field} must be a column of data table")
 
         row_dict = info
         row_dict["field"] = field
         with self.connection() as con:  # commit/rollback transaction
             try:
-                if field in self.fieldinfo().keys():
+                if field in self.fieldinfo():
                     update_from_dict(con, self._table_fieldinfo, row_dict, "field")
                 else:
                     insert_from_dict(con, self._table_fieldinfo, row_dict)
             except sqlite3.OperationalError:  # missing column(s)
                 self._add_columns(self._table_fieldinfo, list(row_dict.keys()))
                 self.write_fieldinfo(field, info)  # try again
 
     def globalinfo(self) -> Dict[str, Any]:
         """Read globalinfo table."""
+
         def try_convert_string(value: str) -> Any:
             try:
                 return literal_eval(value)
             except (SyntaxError, ValueError):
                 return str(value)
+
         con = self.connection()
         cur = con.execute(f"SELECT Key, Value FROM {self._table_globalinfo}")
-        return {
-            row[0]: try_convert_string(str(row[1])) for row in cur.fetchall()
-        }
+        return {row[0]: try_convert_string(str(row[1])) for row in cur.fetchall()}
 
     @require_write_access
     def _update_globalinfo(self):
         """Update globalinfo after writes."""
         keys = self.globalinfo().keys()
         with self.connection() as con:  # commit/rollback transaction
             if "ValidSets" in keys:
                 con.execute(
                     """
                     UPDATE {prefix}_globalinfo
                     SET Value = (SELECT MAX(rowid) FROM {prefix}_data)
                     WHERE Key == "ValidSets"
-                    """.format(prefix=self._table_prefix)
+                    """.format(
+                        prefix=self._table_prefix
+                    )
                 )
             if "TRAI" in keys:
                 con.execute(
                     """
                     UPDATE {prefix}_globalinfo
                     SET Value = (SELECT MAX(TRAI) FROM {prefix}_data)
                     WHERE Key == "TRAI";
-                    """.format(prefix=self._table_prefix)
+                    """.format(
+                        prefix=self._table_prefix
+                    )
                 )
 
     def _file_status(self) -> int:
         """Get file status (0: offline, 1: suspended, 2: active)."""
-        result = self.connection().execute(
-            f"SELECT Value FROM {self._table_globalinfo} WHERE Key == 'FileStatus'"
-        ).fetchone()
+        result = (
+            self.connection()
+            .execute(f"SELECT Value FROM {self._table_globalinfo} WHERE Key == 'FileStatus'")
+            .fetchone()
+        )
         return int(result[0]) if result else 0
 
     def _main_index_range(self) -> Tuple[int, int]:
         """Get range of main data table index (SetID for pridb/tradb or TRAI for trfdb)."""
-        return self.connection().execute(
-            f"SELECT MIN(rowid), MAX(rowid) FROM {self._table_main}"
-        ).fetchone()
+        return (
+            self.connection()
+            .execute(f"SELECT MIN(rowid), MAX(rowid) FROM {self._table_main}")
+            .fetchone()
+        )
 
     def _parameter_table(self) -> Dict[int, Dict[str, Any]]:
         """Read *_params table to dict."""
+
         def parameter_by_id():
             for row in read_sql_generator(
                 self.connection(),
                 f"SELECT * FROM {self._table_params}",
             ):
                 param_id = row.pop("ID")
                 yield param_id, row
@@ -232,17 +240,15 @@
         return self._parameter_table_cached
 
     def _parameter(self, param_id: int) -> Dict[str, Any]:
         """Read parameters from *_params by ID."""
         try:
             return self._parameter_table()[param_id]
         except KeyError:
-            raise ValueError(
-                f"Parameter ID {param_id} not found in {self._table_params}"
-            ) from None
+            raise ValueError(f"Parameter ID {param_id} not found in {self._table_params}") from None
 
     def close(self):
         """Close database connection."""
         if not hasattr(self, "_connection_wrapper"):
             return
         if self.connected:
             if not self._readonly:
```

### Comparing `vallenae-0.7.0/src/vallenae/io/_dataframe.py` & `vallenae-0.8.0/src/vallenae/io/_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,9 +43,8 @@
     if show_progress:
         iterator = tqdm(iterator, total=len(iterable), desc=desc)
     df = pd.DataFrame(iterator)
     if not df.empty:
         df = df.dropna(axis="columns", how="all")  # drop empty columns
         if index_column is not None:
             df = df.set_index(index_column)
-    df = _convert_to_nullable_types(df)
-    return df
+    return _convert_to_nullable_types(df)
```

### Comparing `vallenae-0.7.0/src/vallenae/io/_sql.py` & `vallenae-0.8.0/src/vallenae/io/_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,37 +112,39 @@
         self.__dict__.update(state)
         # reopen connection if connected before
         if self._connected:
             self._connect()
 
 
 T = TypeVar("T")
-class QueryIterable(SizedIterable[T]):  # pylint: disable=inherit-non-class
+
+
+class QueryIterable(SizedIterable[T]):
     """
     Sized iterable to query results from SQLite as dictionaries.
 
     SQLite connection is stored in picklable ConnectionWrapper to be used with multiprocessing.
     """
+
     def __init__(
         self,
         connection_wrapper: ConnectionWrapper,
         query: str,
         dict_to_type: Callable[[Dict[str, Any]], T],
     ):
-        super().__init__()  # pylint: disable=no-value-for-parameter
+        super().__init__()
         self._connection_wrapper = connection_wrapper
         self._query = query
         self._dict_to_type = dict_to_type
         self._count_result: Optional[int] = None  # cache result of __len__
 
     def __len__(self) -> int:
         if self._count_result is None:
             self._count_result = count_sql_results(
-                self._connection_wrapper.connection(),
-                self._query
+                self._connection_wrapper.connection(), self._query
             )
         return self._count_result
 
     def __iter__(self) -> Iterator[T]:
         if self.__len__() == 0:
             logger.debug("Empty SQLite query")
 
@@ -162,48 +164,52 @@
     less_equal: Optional[TComparison] = None,
     greater: Optional[TComparison] = None,
     greater_equal: Optional[TComparison] = None,
     custom_filter: Optional[str] = None,
 ) -> str:
     cond = []
 
+    def as_sequence(value):
+        return value if isinstance(value, collections.abc.Sequence) else (value,)
+
     if isin is not None:
         for key, values in isin.items():
             if values is None:
                 continue
-            if not isinstance(values, collections.abc.Sequence):
-                values = (values,)
-            list_values = ", ".join(str(value) for value in values)
+            list_values = ", ".join(str(value) for value in as_sequence(values))
             cond.append(f"{key} IN ({list_values})")
 
     comparison = {
         "==": equal,
         "<": less,
         "<=": less_equal,
         ">": greater,
         ">=": greater_equal,
     }
 
+    def escape_string(value):
+        return f"'{value}'" if isinstance(value, str) else value
+
     for comp_operator, comp_dict in comparison.items():
         if comp_dict is not None:
             for key, value in comp_dict.items():
                 if value is None:
                     continue
-                if isinstance(value, str):
-                    value = f"'{value}'"  # add quotation marks
-                cond.append(f"{key} {comp_operator} {value}")
+                cond.append(f"{key} {comp_operator} {escape_string(value)}")
 
     if custom_filter is not None:
         cond.append(f"({custom_filter})")  # wrap custom condition(s) in brackets
 
     return "WHERE " + " AND ".join(cond) if cond else ""
 
 
 def read_sql_generator(
-    connection: sqlite3.Connection, query: str, *parameter,
+    connection: sqlite3.Connection,
+    query: str,
+    *parameter,
 ) -> Iterator[Dict[str, Any]]:
     """
     Generator to query data from a SQLite connection as a dictionary.
 
     Args:
         connection: SQLite3 connection object
         query: SELECT Query
@@ -310,17 +316,15 @@
 
 
 def create_new_database(filename: str, schema: str):
     if Path(filename).resolve().exists():
         raise ValueError("Can not create new database. File already exists")
 
     # open database in read-write-create mode
-    with contextlib.closing(
-        sqlite3.connect(create_uri(filename, mode="rwc"), uri=True)
-    ) as con:
+    with contextlib.closing(sqlite3.connect(create_uri(filename, mode="rwc"), uri=True)) as con:
         con.executescript(schema)
 
 
 def remove_none_values_from_dict(dictionary: Dict[Any, Any]):
     """Helper function to remove None values from dict."""
     return {k: v for k, v in dictionary.items() if v is not None}
```

### Comparing `vallenae-0.7.0/src/vallenae/io/compression.py` & `vallenae-0.8.0/src/vallenae/io/compression.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,73 +11,81 @@
 
 def _check_flac_codec():
     if not _FLAC_CODEC:
         raise ValueError("FLAC library not found. Please install libsndfile.")
 
 
 def decode_data_blob(
-    data_blob: bytes, data_format: int, factor_millivolts: float
+    data_blob: bytes, data_format: int, factor_millivolts: float, *, raw: bool = False
 ) -> np.ndarray:
     """
     Decodes (compressed) 16-bit ADC values from BLOB to array of voltage values.
 
     Args:
         data_blob: Blob from tradb
         data_format:
             - 0: uncompressed
             - 2: FLAC compression
         factor_millivolts: Factor from int16 representation to millivolts.
             Stored in tradb -> tr_params as 'TR_mV'
+        raw: Return data as ADC values (`np.int16`), `factor_millivolts` will be ignored
 
     Returns:
-        Array of voltage values
+        Array of voltage values or ADC values if `raw` is `True`
     """
-    if data_format == 0:  # uncompressed
-        data = np.frombuffer(data_blob, dtype=np.int16)
-        factor = 1e-3 * factor_millivolts
-        return np.multiply(data, factor, dtype=np.float32)
-    if data_format == 2:  # flac
-        _check_flac_codec()
-        data, _ = sf.read(io.BytesIO(data_blob), dtype=np.float32)
-        factor_libsoundfile = 2 ** 15  # libsoundfile normalizes to +-1
-        factor = 1e-3 * factor_millivolts * factor_libsoundfile
-        return np.multiply(data, factor, dtype=np.float32)
-    raise ValueError("Data format not supported")
+    def get_data_int16():
+        if data_format == 0:  # uncompressed
+            return np.frombuffer(data_blob, dtype=np.int16)
+        if data_format == 2:  # flac
+            _check_flac_codec()
+            return sf.read(io.BytesIO(data_blob), dtype=np.int16)[0]
+        raise ValueError("Data format not supported")
+
+    data_int16 = get_data_int16()
+    if raw:
+        return data_int16
+    return np.multiply(data_int16, 1e-3 * factor_millivolts, dtype=np.float32)
 
 
 def encode_data_blob(
-    data: np.ndarray, data_format: int, factor_millivolts: float
+    data: np.ndarray, data_format: int, factor_millivolts: float, *, raw: bool = False
 ) -> bytes:
     """
     Encodes array of voltage values to BLOB of 16-bit ADC values
     for memory-efficient storage.
 
     Args:
         data: Array with voltage values
         data_format:
             - 0: uncompressed
             - 2: FLAC compression
         factor_millivolts: Factor from int16 representation to millivolts.
             Stored in tradb -> tr_params as 'TR_mV'
+        raw: Provide `data` as ADC values (int16), `factor_millivolts` will be ignored
 
     Returns:
         Data blob
     """
     ii16_min = np.iinfo(np.int16).min
     ii16_max = np.iinfo(np.int16).max
-    temp = np.empty_like(data, dtype=np.float32)
-    np.multiply(data, 1e3 / factor_millivolts, out=temp)
-    # faster than np.clip(temp, a_min=ii16_min, a_max=ii16_max, out=temp)
-    np.minimum(temp, ii16_max, out=temp)
-    np.maximum(temp, ii16_min, out=temp)
-    # faster than np.rint(temp, out=temp)
-    np.floor(temp + 0.5, out=temp)
-    data_int16 = temp.astype(np.int16)
 
+    def get_data_int16():
+        if raw:
+            return data.astype(np.int16, casting="safe", copy=False)  # only safe casts!
+        temp = np.empty_like(data, dtype=np.float32)
+        np.multiply(data, 1e3 / factor_millivolts, out=temp)
+        # faster than np.clip(temp, a_min=ii16_min, a_max=ii16_max, out=temp)
+        np.minimum(temp, ii16_max, out=temp)
+        np.maximum(temp, ii16_min, out=temp)
+        # faster than np.rint(temp, out=temp)
+        np.floor(temp + 0.5, out=temp)
+        return temp.astype(np.int16)
+
+    data_int16 = get_data_int16()
     if data_format == 0:  # uncompressed
         return data_int16.tobytes()
     if data_format == 2:  # flac
         _check_flac_codec()
         buffer = io.BytesIO()
-        sf.write(buffer, data_int16, 1, format="FLAC")  # samplerate = 1
+        sf.write(buffer, data_int16, samplerate=1, format="FLAC")
         return buffer.getvalue()
     raise ValueError("Data format not supported")
```

### Comparing `vallenae-0.7.0/src/vallenae/io/datatypes.py` & `vallenae-0.8.0/src/vallenae/io/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     rise_time: Optional[float] = None  #: Rise time in seconds
     signal_strength: Optional[float] = None  #: Signal strength in nVs (1e-9 Vs)
     counts: Optional[int] = None  #: Number of positive threshold crossings
     trai: Optional[int] = None  #: Transient recorder index (foreign key between pridb and tradb)
     cascade_hits: Optional[int] = None  #: Total number of hits in the same hit-cascade
     cascade_counts: Optional[int] = None  #: Summed counts of hits in the same hit-cascade
     cascade_energy: Optional[int] = None  #: Summed energy of hits in the same hit-cascade
-    cascade_signal_strength: Optional[int] = None  #: Summed signal strength of hits in the same hit-cascade  # noqa  # pylint: disable=line-too-long
+    cascade_signal_strength: Optional[int] = None  #: Summed signal strength of hits in the same hit-cascade  # noqa
 
     @classmethod
     def from_sql(cls, row: Dict[str, Any]) -> "HitRecord":
         """
-        Create HitRecord from SQL row.
+        Create `HitRecord` from SQL row.
 
         Args:
             row: Dict of column names and values
         """
         return cls(
             set_id=row["SetID"],
             time=row["Time"],
@@ -88,15 +88,15 @@
     # optional for creating:
     number: Optional[int] = None  #: Marker number
     set_id: Optional[int] = None  #: Unique identifier for data set in pridb
 
     @classmethod
     def from_sql(cls, row: Dict[str, Any]) -> "MarkerRecord":
         """
-        Create MarkerRecord from SQL row.
+        Create `MarkerRecord` from SQL row.
 
         Args:
             row: Dict of column names and values
         """
         return cls(
             set_id=row["SetID"],
             time=row["Time"],
@@ -120,15 +120,15 @@
     set_id: Optional[int] = None  #: Unique identifier for data set in pridb
     threshold: Optional[float] = None  #: Threshold amplitude in volts
     signal_strength: Optional[float] = None  #: Signal strength in nVs (1e-9 Vs)
 
     @classmethod
     def from_sql(cls, row: Dict[str, Any]) -> "StatusRecord":
         """
-        Create StatusRecord from SQL row.
+        Create `StatusRecord` from SQL row.
 
         Args:
             row: Dict of column names and values
         """
         return cls(
             set_id=row["SetID"],
             time=row["Time"],
@@ -160,15 +160,15 @@
     pa5: Optional[int] = None  #: Amplitude of parametric input 5 in volts
     pa6: Optional[int] = None  #: Amplitude of parametric input 6 in volts
     pa7: Optional[int] = None  #: Amplitude of parametric input 7 in volts
 
     @classmethod
     def from_sql(cls, row: Dict[str, Any]) -> "ParametricRecord":
         """
-        Create ParametricRecord from SQL row.
+        Create `ParametricRecord` from SQL row.
 
         Args:
             row: Dict of column names and values
         """
         return cls(
             set_id=row["SetID"],
             time=row["Time"],
@@ -192,41 +192,57 @@
     time: float  #: Time in seconds
     channel: int  #: Channel number
     param_id: int  #: Parameter ID of table tr_params for ADC value conversion
     pretrigger: int  #: Pretrigger samples
     threshold: float  #: Threshold amplitude in volts
     samplerate: int  #: Samplerate in Hz
     samples: int  #: Number of samples
-    data: np.ndarray  #: Transient signal in volts
-    # optional for creating:
+    data: np.ndarray  #: Transient signal in volts or ADC values if `raw` = `True`
+    # optional for writing
     trai: Optional[int] = None  #: Transient recorder index (foreign key between pridb and tradb)
     rms: Optional[float] = None  #: RMS of the noise before the hit
+    # optional
+    raw: bool = False  #: `data` is stored as ADC values (int16)
 
     @classmethod
-    def from_sql(cls, row: Dict[str, Any]) -> "TraRecord":
+    def from_sql(cls, row: Dict[str, Any], *, raw: bool = False) -> "TraRecord":
+        """
+        Create `TraRecord` from SQL row.
+
+        Args:
+            row: Dict of column names and values
+            raw: Provide `data` as ADC values (int16)
+        """
         return TraRecord(
             time=row["Time"],
             channel=row["Chan"],
             param_id=row["ParamID"],
             pretrigger=row["Pretrigger"],
             threshold=_to_volts(row["Thr"]),
             samplerate=row["SampleRate"],
             samples=row["Samples"],
-            data=decode_data_blob(row["Data"], row["DataFormat"], row["TR_mV"]),
+            data=decode_data_blob(row["Data"], row["DataFormat"], row["TR_mV"], raw=raw),
             trai=row["TRAI"],
+            raw=raw,
         )
 
 
 class FeatureRecord(NamedTuple):
     """
     Transient feature record in trfdb.
     """
 
     trai: int  #: Transient recorder index
     features: Dict[str, float]  #: Feature dictionary (feature name -> value)
 
     @classmethod
     def from_sql(cls, row: Dict[str, Any]) -> "FeatureRecord":
+        """
+        Create `FeatureRecord` from SQL row.
+
+        Args:
+            row: Dict of column names and values
+        """
         return FeatureRecord(
             trai=row.pop("TRAI"),
             features=row,
         )
```

### Comparing `vallenae-0.7.0/src/vallenae/io/pridb.py` & `vallenae-0.8.0/src/vallenae/io/pridb.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,19 +66,17 @@
     def create(filename: str):
         """
         Create empty pridb.
 
         Args:
             filename: Path to new pridb database file
         """
-        file_schema = Path(__file__).resolve().parent / "schema_templates/pridb.sql"
-        with open(file_schema, "r", encoding="utf-8") as file:
-            schema_pridb = file.read()
-        schema_pridb = schema_pridb.format(timebase=int(1e7))  # fill placeholder / constants
-        create_new_database(filename, schema_pridb)
+        schema_path = Path(__file__).parent / "schema_templates/pridb.sql"
+        schema = schema_path.read_text("utf-8").format(timebase=int(1e7))  # fill placeholder
+        create_new_database(filename, schema)
 
     def channel(self) -> Set[int]:
         """Get list of channels."""
         con = self.connection()
         cur = con.execute("SELECT DISTINCT Chan FROM ae_data WHERE Chan IS NOT NULL")
         return {result[0] for result in cur.fetchall()}
 
@@ -180,23 +178,22 @@
             **dict(df_hits.dtypes),
             **dict(df_markers.dtypes),
             **dict(df_parametric.dtypes),
             **dict(df_status.dtypes),
         }
 
         # concat all dataframes, restore types and sort by index
-        df = (
+        return (
             pd.concat(
                 [df_markers, df_hits, df_status, df_parametric], sort=False, copy=False
             )
             .apply(lambda x: x.astype(dtypes[x.name]))
             .sort_index()
             .rename_axis(df_hits.index.name)
         )
-        return df
 
     def iread_hits(
         self,
         *,
         channel: Union[None, int, Sequence[int]] = None,
         time_start: Optional[float] = None,
         time_stop: Optional[float] = None,
```

### Comparing `vallenae-0.7.0/src/vallenae/io/schema_templates/pridb.sql` & `vallenae-0.8.0/src/vallenae/io/schema_templates/pridb.sql`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/io/schema_templates/tradb.sql` & `vallenae-0.8.0/src/vallenae/io/schema_templates/tradb.sql`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/io/schema_templates/trfdb.sql` & `vallenae-0.8.0/src/vallenae/io/schema_templates/trfdb.sql`

 * *Files identical despite different names*

### Comparing `vallenae-0.7.0/src/vallenae/io/tradb.py` & `vallenae-0.8.0/src/vallenae/io/tradb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from functools import lru_cache
+from functools import lru_cache, partial
 from itertools import chain
 from pathlib import Path
 from time import sleep
 from typing import Iterable, Optional, Sequence, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
@@ -57,19 +57,17 @@
     def create(filename: str):
         """
         Create empty tradb.
 
         Args:
             filename: Path to new tradb database file
         """
-        file_schema = Path(__file__).resolve().parent / "schema_templates/tradb.sql"
-        with open(file_schema, "r", encoding="utf-8") as file:
-            schema_tradb = file.read()
-        schema_tradb = schema_tradb.format(timebase=int(1e7))  # fill placeholder / constants
-        create_new_database(filename, schema_tradb)
+        schema_path = Path(__file__).parent / "schema_templates/tradb.sql"
+        schema = schema_path.read_text("utf-8").format(timebase=int(1e7))  # fill placeholder
+        create_new_database(filename, schema)
 
     def channel(self) -> Set[int]:
         """Get list of channels."""
         con = self.connection()
         cur = con.execute("SELECT DISTINCT Chan FROM tr_data WHERE Chan IS NOT NULL")
         return {result[0] for result in cur.fetchall()}
 
@@ -127,41 +125,40 @@
         self,
         *,
         channel: Union[None, int, Sequence[int]] = None,
         time_start: Optional[float] = None,
         time_stop: Optional[float] = None,
         trai: Union[None, int, Sequence[int]] = None,
         query_filter: Optional[str] = None,
+        raw: bool = False,
     ) -> SizedIterable[TraRecord]:
         """
         Stream transient data with returned Iterable.
 
         Args:
             channel: None if all channels should be read.
                 Otherwise specify the channel number or a list of channel numbers
             time_start: Start reading at relative time (in seconds). Start at beginning if `None`
             time_stop: Stop reading at relative time (in seconds). Read until end if `None`
             trai: Read data by TRAI (transient recorder index)
             query_filter: Optional query filter provided as SQL clause,
                 e.g. "Pretrigger == 500 AND Samples >= 1024"
+            raw: Return data as ADC values (int16). Default: `False`
 
         Returns:
             Sized iterable to sequential read transient data
         """
         # check for empty time ranges
         time_min, time_max = self._get_total_time_range()
-        if time_start is not None:
-            if time_start > time_max:
-                return []
-        if time_stop is not None:
-            if time_stop < time_min:
-                return []
-        if time_start is not None and time_stop is not None:
-            if time_start >= time_stop:
-                return []
+        if time_start is not None and time_start > time_max:
+            return []
+        if time_stop is not None and time_stop < time_min:
+            return []
+        if time_start is not None and time_stop is not None and time_start >= time_stop:
+            return []
 
         trai_start, trai_stop = self._get_trai_range_from_time_range(time_start, time_stop)
         # nested query to fix ambiguous column name error with query_filter
         query = """
         SELECT * FROM (
             SELECT vtr.*, tr.ParamID
             FROM view_tr_data vtr
@@ -174,40 +171,45 @@
             # < condition already met in binary search, use <= here for found indice range
             less_equal={"TRAI": trai_stop},
             custom_filter=query_filter,
         )
         return QueryIterable(
             self._connection_wrapper.get_readonly_connection(),
             query,
-            TraRecord.from_sql,
+            partial(TraRecord.from_sql, raw=raw),
         )
 
     def read_wave(
-        self, trai: int, time_axis: bool = True,
+        self,
+        trai: int,
+        time_axis: bool = True,
+        *,
+        raw: bool = False,
     ) -> Union[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, int]]:
         """
         Read transient signal for a given TRAI (transient recorder index).
 
         This method is useful in combination with `PriDatabase.read_hits`,
         that will store the TRAI in a DataFrame.
 
         Args:
             trai: Transient recorder index (unique key between pridb and tradb)
             time_axis: Create the correspondig time axis. Default: `True`
+            raw: Return data as ADC values (int16). Default: `False`
 
         Returns:
             If :attr:`time_axis` is `True`\n
             - Array with transient signal
             - Time axis
 
             If :attr:`time_axis` is `False`\n
             - Array with transient signal
             - Samplerate
         """
-        iterable = self.iread(trai=trai)
+        iterable = self.iread(trai=trai, raw=raw)
         try:
             tra = next(iter(iterable))
         except StopIteration:
             raise ValueError("TRAI does not exists") from None
 
         if time_axis:
             return (
@@ -228,48 +230,51 @@
         self,
         channel: int,
         time_start: Optional[float] = None,
         time_stop: Optional[float] = None,
         *,
         time_axis: bool = True,
         show_progress: bool = True,
+        raw: bool = False,
     ) -> Union[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, int]]:
         """
         Read transient signal of specified channel to a single, continuous array.
 
         The signal is exactly cropped to the given time range. Time gaps are filled with 0's.
 
         Args:
             channel: Channel number to read
             time_start: Start reading at relative time (in seconds). Start at beginning if `None`
             time_stop: Stop reading at relative time (in seconds). Read until end if `None`
             time_axis: Create the correspondig time axis. Default: `True`
             show_progress: Show progress bar. Default: `True`
+            raw: Return data as ADC values (int16). Default: `False`
 
         Returns:
             If `time_axis` is `True`\n
             - Array with transient signal
             - Time axis
 
             If `time_axis` is `False`\n
             - Array with transient signal
             - Samplerate
         """
-        iterable = self.iread(channel=channel, time_start=time_start, time_stop=time_stop)
+        dtype = np.int16 if raw else np.float32
+        iterable = self.iread(channel=channel, time_start=time_start, time_stop=time_stop, raw=raw)
         iterator = iter(iterable)
         if show_progress:
             iterator = tqdm(iterator, total=len(iterable), desc="Tra")  # ignores previous tra
 
         # prepend previous tra to iterator if available
         trai_start, _ = self._get_trai_range_from_time_range(time_start, None)
         if trai_start is not None:
             previous_trai = self._get_previous_trai(channel, trai_start)
             if previous_trai is not None:
                 iterator = chain(
-                    iter(self.iread(channel=channel, trai=previous_trai)),
+                    iter(self.iread(channel=channel, trai=previous_trai, raw=raw)),
                     iterator,
                 )
 
         # find beginning if not provided
         if time_start is None:
             time_start = self._get_total_time_range()[0]
 
@@ -281,61 +286,63 @@
             if time_start is not None:
                 n_start = limit_index(round((time_start - tra.time) * tra.samplerate))
             if time_stop is not None:
                 n_stop = limit_index(round((time_stop - tra.time) * tra.samplerate))
             return n_start, n_stop
 
         samplerate = 0  # will be initialized with samplerate of first record
-        tra_blocks = [np.empty(0, dtype=np.float32)]
+        tra_blocks = [np.empty(0, dtype=dtype)]
         expected_time = time_start
 
         for tra in iterator:
             if samplerate == 0:
                 samplerate = tra.samplerate
             if tra.samplerate != samplerate:
                 raise RuntimeError("Different sampling rates inside requested time interval")
 
             # check for gaps in tra stream
             time_gap = tra.time - expected_time
             if time_gap > 1 / tra.samplerate:
                 samples_gap = round(time_gap * tra.samplerate)
-                tra_blocks.append(np.zeros(samples_gap, dtype=np.float32))
+                tra_blocks.append(np.zeros(samples_gap, dtype=dtype))
 
             sample_start, sample_stop = slice_range(tra)
             tra_blocks.append(tra.data[sample_start:sample_stop])
             expected_time = tra.time + sample_stop / tra.samplerate
             if time_start is not None:
                 # the prepended record might be out of time range -> avoid exceeding zero-padding
                 expected_time = max(expected_time, time_start)
 
         if time_stop is not None and samplerate and abs(expected_time - time_stop) > 1 / samplerate:
             # zero padding at ending
             samples = round((time_stop - expected_time) * samplerate)
-            tra_blocks.append(np.zeros(samples, dtype=np.float32))
+            tra_blocks.append(np.zeros(samples, dtype=dtype))
 
         y = np.concatenate(tra_blocks)
         if time_axis:
             return y, _create_time_vector(len(y), samplerate) + time_start
         return y, samplerate
 
     def listen(
         self,
         existing: bool = False,
         wait: bool = False,
         query_filter: Optional[str] = None,
+        raw: bool = False,
     ) -> Iterable[TraRecord]:
         """
         Listen to database changes and return new records.
 
         Args:
             existing: Return already existing records
             wait: Wait for new records even if no acquisition (writer) is active.
                 Otherwise the function returns after all records are read.
             query_filter: Optional query filter provided as SQL clause,
                 e.g. "TRAI >= 100 AND Samples >= 1024"
+            raw: Return data as ADC values (int16). Default: `False`
 
         Yields:
             New transient data records
         """
         max_buffer_size = 100
         query = f"""
         SELECT * FROM (
@@ -346,15 +353,15 @@
         ) {query_conditions(custom_filter=query_filter)} LIMIT {max_buffer_size}
         """
         last_set_id = 0 if existing else self._main_index_range()[1]
         while True:
             # buffer rows to allow in-between write transactions
             rows = list(read_sql_generator(self.connection(), query, last_set_id))
             for row in rows:
-                yield TraRecord.from_sql(row)
+                yield TraRecord.from_sql(row, raw=raw)
                 last_set_id = row["SetID"]
             if len(rows) == 0:
                 if not wait and self._file_status() == 0:  # no writer active
                     break
                 sleep(0.1)  # wait 100 ms until next read
```

### Comparing `vallenae-0.7.0/src/vallenae/io/trfdb.py` & `vallenae-0.8.0/src/vallenae/io/trfdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,31 +41,30 @@
     def create(filename: str):
         """
         Create empty trfdb.
 
         Args:
             filename: Path to new trfdb database file
         """
-        file_schema = Path(__file__).resolve().parent / "schema_templates/trfdb.sql"
-        with open(file_schema, "r", encoding="utf-8") as file:
-            schema_trfdb = file.read()
-        create_new_database(filename, schema_trfdb)
+        schema_path = Path(__file__).parent / "schema_templates/trfdb.sql"
+        schema = schema_path.read_text("utf-8")
+        create_new_database(filename, schema)
 
     def read(self, **kwargs) -> pd.DataFrame:
         """
         Read features to Pandas DataFrame.
 
         Args:
             **kwargs: Arguments passed to `iread`
 
         Returns:
             Pandas DataFrame with features
         """
         def record_to_dict(record: FeatureRecord):
-            return dict(trai=record.trai, **record.features)
+            return {"trai": record.trai, **record.features}
         return iter_to_dataframe(
             [record_to_dict(r) for r in self.iread(**kwargs)], desc="Trf", index_column="trai",
         )
 
     def iread(
         self,
         *,
```

### Comparing `vallenae-0.7.0/src/vallenae/timepicker/__init__.py` & `vallenae-0.8.0/src/vallenae/timepicker/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     return _hinkley_numpy(arr, alpha)
 
 
 @njit
 def _aic_numba(arr: np.ndarray) -> Tuple[np.ndarray, int]:
     n = len(arr)
     result = np.full(n, np.nan, dtype=np.float32)
-    safety_eps = np.finfo(np.float32).tiny  # pylint: disable=E1101
+    safety_eps = np.finfo(np.float32).tiny
 
     min_value = math.inf
     min_index = 0
 
     l_sum = 0.0
     r_sum = 0.0
     l_squaresum = 0.0
@@ -133,15 +133,15 @@
             min_index = i
 
     return result, min_index
 
 
 def _aic_numpy(arr: np.ndarray) -> Tuple[np.ndarray, int]:
     n = len(arr)
-    safety_eps = np.finfo(np.float32).tiny  # pylint: disable=E1101
+    safety_eps = np.finfo(np.float32).tiny
 
     l_sum = np.cumsum(arr, dtype=np.float64)
     l_squaresum = np.cumsum(arr ** 2, dtype=np.float64)
     r_sum = l_sum[-1] - l_sum
     r_squaresum = l_squaresum[-1] - l_squaresum
 
     index = np.arange(n)
@@ -181,15 +181,15 @@
     References:
         - Molenda, M. (2016). Acoustic Emission monitoring
           of laboratory hydraulic fracturing experiments.
           Ruhr-Universität Bochum.
         - Bai, F., Gagar, D., Foote, P., & Zhao, Y. (2017).
           Comparison of alternatives to amplitude thresholding for onset detection
           of acoustic emission signals.
-          Mechanical Systems and Signal Processing, 84, 717–730.
+          Mechanical Systems and Signal Processing, 84, 717-730.
         - van Rijn, N. (2017).
           Investigating the Behaviour of Acoustic Emission Waves Near Cracks:
           Using the Finite Element Method. Delft University of Technology.
     """
     if USE_NUMBA:
         return _aic_numba(arr)
     return _aic_numpy(arr)
@@ -233,14 +233,32 @@
 
     result = np.zeros_like(arr, dtype=np.float32)
     result[win_len:-win_len] = r_squaresum / l_squaresum
     return result, np.argmax(result)
 
 
 def energy_ratio(arr: np.ndarray, win_len: int = 100) -> Tuple[np.ndarray, int]:
+    """
+    Energy ratio for arrival time estimation.
+
+    Method based on preceding and following energy collection windows.
+
+    Args:
+        arr: Transient signal of hit
+        win_len: Samples of sliding windows. Default: 100
+
+    Returns:
+        - Array with computed detection function
+        - Index of the estimated arrival time (max value)
+
+    References:
+        - Han, L., Wong, J., & Bancroft, J. C. (2009).
+          Time picking and random noise reduction on microseismic data.
+          CREWES Research Report, 21, 1-13.
+    """
     if USE_NUMBA:
         return _energy_ratio_numba(arr, win_len)
     return _energy_ratio_numpy(arr, win_len)
 
 
 def modified_energy_ratio(arr: np.ndarray, win_len: int = 100) -> Tuple[np.ndarray, int]:
     """
@@ -256,15 +274,15 @@
     Returns:
         - Array with computed detection function
         - Index of the estimated arrival time (max value)
 
     References:
         - Han, L., Wong, J., & Bancroft, J. C. (2009).
           Time picking and random noise reduction on microseismic data.
-          CREWES Research Report, 21, 1–13.
+          CREWES Research Report, 21, 1-13.
     """
     result, _ = energy_ratio(arr, win_len)
     np.multiply(result, np.abs(arr), out=result)
     # faster than np.power(result, 3, out=result)
     np.multiply(result, result, out=result)
     np.multiply(result, result, out=result)
     return result, np.argmax(result)
```

