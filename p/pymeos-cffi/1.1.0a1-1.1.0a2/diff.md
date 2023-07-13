# Comparing `tmp/pymeos_cffi-1.1.0a1.tar.gz` & `tmp/pymeos_cffi-1.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeos_cffi-1.1.0a1.tar", last modified: Sun Jul  9 07:49:11 2023, max compression
+gzip compressed data, was "pymeos_cffi-1.1.0a2.tar", last modified: Thu Jul 13 09:00:10 2023, max compression
```

## Comparing `pymeos_cffi-1.1.0a1.tar` & `pymeos_cffi-1.1.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1276 2023-04-07 07:42:43.000000 pymeos_cffi-1.1.0a1/LICENSE
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       34 2022-08-22 13:17:01.000000 pymeos_cffi-1.1.0a1/MANIFEST.in
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3837 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1327 2022-08-23 10:04:27.000000 pymeos_cffi-1.1.0a1/README.md
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/pymeos_cffi/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    24025 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/__init__.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        0 2022-08-22 13:17:01.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1870 2023-04-07 07:42:43.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_header.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    17670 2022-11-11 09:22:02.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_helpers.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      449 2022-08-26 17:50:52.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_pymeos.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    21086 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_pymeos_functions.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3453 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_pymeos_functions_modifiers.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    79167 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/meos.h
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3236 2022-08-26 15:11:01.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/builder/objects.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)   259311 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pymeos_cffi/functions.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3837 2023-07-09 07:49:11.000000 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      577 2023-07-09 07:49:11.000000 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        1 2023-07-09 07:49:11.000000 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       43 2023-07-09 07:49:11.000000 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/requires.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       23 2023-07-09 07:49:11.000000 pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/top_level.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1377 2023-07-08 17:55:34.000000 pymeos_cffi-1.1.0a1/pyproject.toml
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       38 2023-07-09 07:49:11.498215 pymeos_cffi-1.1.0a1/setup.cfg
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      197 2023-04-03 10:47:11.000000 pymeos_cffi-1.1.0a1/setup.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-13 09:00:10.708117 pymeos_cffi-1.1.0a2/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1261 2023-04-12 16:58:39.000000 pymeos_cffi-1.1.0a2/LICENSE
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       34 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/MANIFEST.in
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3837 2023-07-13 09:00:10.708117 pymeos_cffi-1.1.0a2/PKG-INFO
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1295 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/README.md
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-13 09:00:10.698117 pymeos_cffi-1.1.0a2/pymeos_cffi/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    23110 2023-07-13 09:00:00.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/__init__.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-13 09:00:10.708117 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)        0 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1816 2023-04-12 16:58:39.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_header.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    16955 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_helpers.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      434 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_pymeos.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    20583 2023-05-29 10:44:50.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_pymeos_functions.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3363 2023-05-14 18:59:40.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_pymeos_functions_modifiers.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    77313 2023-07-13 08:59:59.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/meos.h
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3188 2023-03-07 16:34:55.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/builder/objects.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)   253185 2023-07-13 09:00:00.000000 pymeos_cffi-1.1.0a2/pymeos_cffi/functions.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-07-13 09:00:10.708117 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3837 2023-07-13 09:00:10.000000 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      577 2023-07-13 09:00:10.000000 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)        1 2023-07-13 09:00:10.000000 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       43 2023-07-13 09:00:10.000000 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/requires.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       23 2023-07-13 09:00:10.000000 pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/top_level.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1331 2023-07-13 08:59:51.000000 pymeos_cffi-1.1.0a2/pyproject.toml
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       38 2023-07-13 09:00:10.708117 pymeos_cffi-1.1.0a2/setup.cfg
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      190 2023-03-07 18:32:10.000000 pymeos_cffi-1.1.0a2/setup.py
```

### Comparing `pymeos_cffi-1.1.0a1/LICENSE` & `pymeos_cffi-1.1.0a2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
--------------------------------------------------------------------------------
-This PyMEOS code is provided under The PostgreSQL License.
-
-Copyright (c) 2020, Université libre de Bruxelles and MobilityDB contributors
-
-Permission to use, copy, modify, and distribute this software and its documentation for any purpose, without fee, and without a written agreement is hereby
-granted, provided that the above copyright notice and this paragraph and the following two paragraphs appear in all copies.
-
-IN NO EVENT SHALL UNIVERSITE LIBRE DE BRUXELLES BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST
-PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF UNIVERSITE LIBRE DE BRUXELLES HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGE.
-
-UNIVERSITE LIBRE DE BRUXELLES SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS, AND UNIVERSITE LIBRE DE BRUXELLES HAS NO OBLIGATIONS TO PROVIDE
-MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
+-------------------------------------------------------------------------------
+This PyMEOS code is provided under The PostgreSQL License.
+
+Copyright (c) 2020, Université libre de Bruxelles and MobilityDB contributors
+
+Permission to use, copy, modify, and distribute this software and its documentation for any purpose, without fee, and without a written agreement is hereby
+granted, provided that the above copyright notice and this paragraph and the following two paragraphs appear in all copies.
+
+IN NO EVENT SHALL UNIVERSITE LIBRE DE BRUXELLES BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST
+PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF UNIVERSITE LIBRE DE BRUXELLES HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGE.
+
+UNIVERSITE LIBRE DE BRUXELLES SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS, AND UNIVERSITE LIBRE DE BRUXELLES HAS NO OBLIGATIONS TO PROVIDE
+MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
 -------------------------------------------------------------------------------
```

### Comparing `pymeos_cffi-1.1.0a1/PKG-INFO` & `pymeos_cffi-1.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos_cffi
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: PyMEOS wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>
 License: -------------------------------------------------------------------------------
         This PyMEOS code is provided under The PostgreSQL License.
         
         Copyright (c) 2020, Université libre de Bruxelles and MobilityDB contributors
```

### Comparing `pymeos_cffi-1.1.0a1/README.md` & `pymeos_cffi-1.1.0a2/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# PyMEOS CFFI
-
-![MEOS Logo](../doc/images/meos-logo.png)
-
-[MEOS (Mobility Engine, Open Source)](https://www.libmeos.org/) is a C library which enables the manipulation of
-temporal and spatio-temporal data based on [MobilityDB](https://mobilitydb.com/)'s data types and functions.
-
-PyMEOS CFFI is a Python library that wraps the MEOS C library using CFFI, providing a set of python functions
-that allows to use all MEOS functionality while automatically taking care of conversions between basic Python and C types
-(such as Python's `str` to C's `char *`).  
-
-This library is not meant to be used directly by the user, since most of the functions receive or return C objects 
-(CFFI's `cdata` type).  
-
-The [PyMEOS](../pymeos) library is built on top of this library and exposes all the functionality
-of MEOS through a set of Python classes.
-
-# Usage
-
-## Installation
-
-````shell
-pip install pymeos-cffi
-````
-
-## Source installation
-If the pre-built distribution is not available for your system, `pip` will try to make source distribution. For that, you will 
-need to make sure you have the following requirements:
-
-- C compiler
-- [MEOS Library](https://www.libmeos.org/)
-
+# PyMEOS CFFI
+
+![MEOS Logo](../doc/images/meos-logo.png)
+
+[MEOS (Mobility Engine, Open Source)](https://www.libmeos.org/) is a C library which enables the manipulation of
+temporal and spatio-temporal data based on [MobilityDB](https://mobilitydb.com/)'s data types and functions.
+
+PyMEOS CFFI is a Python library that wraps the MEOS C library using CFFI, providing a set of python functions
+that allows to use all MEOS functionality while automatically taking care of conversions between basic Python and C types
+(such as Python's `str` to C's `char *`).  
+
+This library is not meant to be used directly by the user, since most of the functions receive or return C objects 
+(CFFI's `cdata` type).  
+
+The [PyMEOS](../pymeos) library is built on top of this library and exposes all the functionality
+of MEOS through a set of Python classes.
+
+# Usage
+
+## Installation
+
+````shell
+pip install pymeos-cffi
+````
+
+## Source installation
+If the pre-built distribution is not available for your system, `pip` will try to make source distribution. For that, you will 
+need to make sure you have the following requirements:
+
+- C compiler
+- [MEOS Library](https://www.libmeos.org/)
+
 If the installation fails, you can submit an issue in the [PyMEOS issue tracker](https://github.com/MobilityDB/PyMEOS/issues)
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/__init__.py` & `pymeos_cffi-1.1.0a2/pymeos_cffi/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,915 +1,915 @@
-from .functions import *
-
-__all__ = [
-    'create_pointer',
-    'get_address',
-    'datetime_to_timestamptz',
-    'timestamptz_to_datetime',
-    'timedelta_to_interval',
-    'interval_to_timedelta',
-    'geometry_to_gserialized',
-    'gserialized_to_shapely_point',
-    'gserialized_to_shapely_geometry',
-    'intrange_to_intspan',
-    'intspan_to_intrange',
-    'floatrange_to_floatspan',
-    'floatspan_to_floatrange',
-    'as_tinstant',
-    'as_tsequence',
-    'as_tsequenceset',
-    'lwpoint_make',
-    'lwgeom_from_gserialized',
-    'gserialized_from_lwgeom',
-    'lwgeom_get_srid',
-    'lwpoint_get_x',
-    'lwpoint_get_y',
-    'lwpoint_get_z',
-    'lwpoint_get_m',
-    'lwgeom_has_z',
-    'lwgeom_has_m',
-    'meos_initialize',
-    'meos_finalize',
-    'bool_in',
-    'bool_out',
-    'cstring2text',
-    'pg_date_in',
-    'pg_date_out',
-    'pg_interval_cmp',
-    'pg_interval_in',
-    'pg_interval_make',
-    'pg_interval_mul',
-    'pg_interval_out',
-    'pg_interval_pl',
-    'pg_time_in',
-    'pg_time_out',
-    'pg_timestamp_in',
-    'pg_timestamp_mi',
-    'pg_timestamp_mi_interval',
-    'pg_timestamp_out',
-    'pg_timestamp_pl_interval',
-    'pg_timestamptz_in',
-    'pg_timestamptz_out',
-    'text2cstring',
-    'gserialized_as_ewkb',
-    'gserialized_as_ewkt',
-    'gserialized_as_geojson',
-    'gserialized_as_hexewkb',
-    'gserialized_as_text',
-    'gserialized_from_ewkb',
-    'gserialized_from_geojson',
-    'gserialized_from_hexewkb',
-    'gserialized_from_text',
-    'gserialized_in',
-    'gserialized_out',
-    'pgis_gserialized_same',
-    'bigintset_in',
-    'bigintset_out',
-    'bigintspan_in',
-    'bigintspan_out',
-    'bigintspanset_in',
-    'bigintspanset_out',
-    'floatset_in',
-    'floatset_out',
-    'floatspan_in',
-    'floatspan_out',
-    'floatspanset_in',
-    'floatspanset_out',
-    'geogset_in',
-    'geogset_out',
-    'geomset_in',
-    'geomset_out',
-    'geoset_as_ewkt',
-    'geoset_as_text',
-    'intset_in',
-    'intset_out',
-    'intspan_in',
-    'intspan_out',
-    'intspanset_in',
-    'intspanset_out',
-    'period_in',
-    'period_out',
-    'periodset_in',
-    'periodset_out',
-    'set_as_hexwkb',
-    'set_as_wkb',
-    'set_from_hexwkb',
-    'set_from_wkb',
-    'set_out',
-    'span_as_wkb',
-    'span_as_hexwkb',
-    'span_from_hexwkb',
-    'span_from_wkb',
-    'span_out',
-    'spanset_as_wkb',
-    'spanset_as_hexwkb',
-    'spanset_from_hexwkb',
-    'spanset_from_wkb',
-    'spanset_out',
-    'textset_in',
-    'textset_out',
-    'timestampset_in',
-    'timestampset_out',
-    'bigintset_make',
-    'bigintspan_make',
-    'floatset_make',
-    'floatspan_make',
-    'geogset_make',
-    'geomset_make',
-    'intset_make',
-    'intspan_make',
-    'period_make',
-    'set_copy',
-    'span_copy',
-    'spanset_copy',
-    'spanset_make',
-    'spanset_make_exp',
-    'spanset_make_free',
-    'textset_make',
-    'timestampset_make',
-    'bigint_to_bigintset',
-    'bigint_to_bigintspan',
-    'bigint_to_bigintspanset',
-    'float_to_floatset',
-    'float_to_floatspan',
-    'float_to_floatspanset',
-    'int_to_intset',
-    'int_to_intspan',
-    'int_to_intspanset',
-    'set_to_spanset',
-    'span_to_spanset',
-    'timestamp_to_period',
-    'timestamp_to_periodset',
-    'timestamp_to_tstzset',
-    'bigintset_end_value',
-    'bigintset_start_value',
-    'bigintset_value_n',
-    'bigintset_values',
-    'bigintspan_lower',
-    'bigintspan_upper',
-    'bigintspanset_lower',
-    'bigintspanset_upper',
-    'floatset_end_value',
-    'floatset_start_value',
-    'floatset_value_n',
-    'floatset_values',
-    'floatspan_lower',
-    'floatspan_upper',
-    'floatspanset_lower',
-    'floatspanset_upper',
-    'geoset_srid',
-    'intset_end_value',
-    'intset_start_value',
-    'intset_value_n',
-    'intset_values',
-    'intspan_lower',
-    'intspan_upper',
-    'intspanset_lower',
-    'intspanset_upper',
-    'period_duration',
-    'period_lower',
-    'period_upper',
-    'periodset_duration',
-    'periodset_end_timestamp',
-    'periodset_lower',
-    'periodset_num_timestamps',
-    'periodset_start_timestamp',
-    'periodset_timestamp_n',
-    'periodset_timestamps',
-    'periodset_upper',
-    'set_hash',
-    'set_hash_extended',
-    'set_mem_size',
-    'set_num_values',
-    'set_span',
-    'span_hash',
-    'span_hash_extended',
-    'span_lower_inc',
-    'span_upper_inc',
-    'span_width',
-    'spanset_end_span',
-    'spanset_hash',
-    'spanset_hash_extended',
-    'spanset_lower_inc',
-    'spanset_mem_size',
-    'spanset_num_spans',
-    'spanset_span',
-    'spanset_span_n',
-    'spanset_spans',
-    'spanset_start_span',
-    'spanset_upper_inc',
-    'spanset_width',
-    'spatialset_stbox',
-    'timestampset_end_timestamp',
-    'timestampset_start_timestamp',
-    'timestampset_timestamp_n',
-    'timestampset_values',
-    'floatspan_set_intspan',
-    'intspan_set_floatspan',
-    'numspan_set_floatspan',
-    'period_tprecision',
-    'periodset_tprecision',
-    'period_shift_tscale',
-    'periodset_shift_tscale',
-    'set_shift',
-    'span_expand',
-    'timestamp_tprecision',
-    'timestampset_shift_tscale',
-    'adjacent_bigintspan_bigint',
-    'adjacent_bigintspanset_bigint',
-    'adjacent_floatspan_float',
-    'adjacent_intspan_int',
-    'adjacent_period_timestamp',
-    'adjacent_periodset_timestamp',
-    'adjacent_span_span',
-    'adjacent_spanset_span',
-    'adjacent_spanset_spanset',
-    'contained_bigint_bigintset',
-    'contained_bigint_bigintspan',
-    'contained_bigint_bigintspanset',
-    'contained_float_floatset',
-    'contained_float_floatspan',
-    'contained_float_floatspanset',
-    'contained_int_intset',
-    'contained_int_intspan',
-    'contained_set_set',
-    'contained_span_span',
-    'contained_span_spanset',
-    'contained_spanset_span',
-    'contained_spanset_spanset',
-    'contained_timestamp_period',
-    'contained_timestamp_timestampset',
-    'contains_floatspan_float',
-    'contains_floatspanset_float',
-    'contains_intspan_int',
-    'contains_set_set',
-    'contains_period_timestamp',
-    'contains_periodset_timestamp',
-    'contains_span_span',
-    'contains_span_spanset',
-    'contains_spanset_span',
-    'contains_spanset_spanset',
-    'contains_timestampset_timestamp',
-    'overlaps_set_set',
-    'overlaps_span_span',
-    'overlaps_spanset_span',
-    'overlaps_spanset_spanset',
-    'after_timestamp_timestampset',
-    'before_periodset_timestamp',
-    'before_timestamp_timestampset',
-    'left_float_floatspan',
-    'left_floatspan_float',
-    'left_int_intspan',
-    'left_intspan_int',
-    'left_set_set',
-    'left_span_span',
-    'left_span_spanset',
-    'left_spanset_span',
-    'left_spanset_spanset',
-    'overafter_period_timestamp',
-    'overafter_periodset_timestamp',
-    'overafter_timestamp_period',
-    'overafter_timestamp_periodset',
-    'overafter_timestamp_timestampset',
-    'overbefore_period_timestamp',
-    'overbefore_periodset_timestamp',
-    'overbefore_timestamp_period',
-    'overbefore_timestamp_periodset',
-    'overbefore_timestamp_timestampset',
-    'overleft_float_floatspan',
-    'overleft_floatspan_float',
-    'overleft_int_intspan',
-    'overleft_intspan_int',
-    'overleft_set_set',
-    'overleft_span_span',
-    'overleft_span_spanset',
-    'overleft_spanset_span',
-    'overleft_spanset_spanset',
-    'overright_float_floatspan',
-    'overright_floatspan_float',
-    'overright_int_intspan',
-    'overright_intspan_int',
-    'overright_set_set',
-    'overright_span_span',
-    'overright_span_spanset',
-    'overright_spanset_span',
-    'overright_spanset_spanset',
-    'right_float_floatspan',
-    'right_floatspan_float',
-    'right_int_intspan',
-    'right_intspan_int',
-    'right_set_set',
-    'right_span_span',
-    'right_span_spanset',
-    'right_spanset_span',
-    'right_spanset_spanset',
-    'bbox_union_span_span',
-    'intersection_set_set',
-    'intersection_period_timestamp',
-    'intersection_periodset_timestamp',
-    'intersection_span_span',
-    'intersection_spanset_span',
-    'intersection_spanset_spanset',
-    'intersection_timestampset_timestamp',
-    'minus_set_set',
-    'minus_period_timestamp',
-    'minus_periodset_timestamp',
-    'minus_span_span',
-    'minus_span_spanset',
-    'minus_spanset_span',
-    'minus_spanset_spanset',
-    'minus_timestamp_period',
-    'minus_timestamp_periodset',
-    'minus_timestampset_timestamp',
-    'union_set_set',
-    'union_period_timestamp',
-    'union_periodset_timestamp',
-    'union_span_span',
-    'union_spanset_span',
-    'union_spanset_spanset',
-    'union_timestampset_timestamp',
-    'distance_floatspan_float',
-    'distance_intspan_int',
-    'distance_set_set',
-    'distance_period_timestamp',
-    'distance_periodset_timestamp',
-    'distance_span_span',
-    'distance_spanset_span',
-    'distance_spanset_spanset',
-    'distance_timestampset_timestamp',
-    'bigint_extent_transfn',
-    'bigint_union_transfn',
-    'float_extent_transfn',
-    'float_union_transfn',
-    'int_extent_transfn',
-    'int_union_transfn',
-    'period_tcount_transfn',
-    'periodset_tcount_transfn',
-    'set_extent_transfn',
-    'set_union_finalfn',
-    'set_union_transfn',
-    'span_extent_transfn',
-    'span_union_transfn',
-    'spanset_extent_transfn',
-    'spanset_union_finalfn',
-    'spanset_union_transfn',
-    'text_union_transfn',
-    'timestamp_extent_transfn',
-    'timestamp_tcount_transfn',
-    'timestamp_union_transfn',
-    'timestampset_tcount_transfn',
-    'set_cmp',
-    'set_eq',
-    'set_ge',
-    'set_gt',
-    'set_le',
-    'set_lt',
-    'set_ne',
-    'span_cmp',
-    'span_eq',
-    'span_ge',
-    'span_gt',
-    'span_le',
-    'span_lt',
-    'span_ne',
-    'spanset_cmp',
-    'spanset_eq',
-    'spanset_ge',
-    'spanset_gt',
-    'spanset_le',
-    'spanset_lt',
-    'spanset_ne',
-    'tbox_in',
-    'tbox_out',
-    'tbox_from_wkb',
-    'tbox_from_hexwkb',
-    'stbox_from_wkb',
-    'stbox_from_hexwkb',
-    'tbox_as_wkb',
-    'tbox_as_hexwkb',
-    'stbox_as_wkb',
-    'stbox_as_hexwkb',
-    'stbox_in',
-    'stbox_out',
-    'tbox_make',
-    'tbox_set',
-    'tbox_copy',
-    'stbox_make',
-    'stbox_set',
-    'stbox_copy',
-    'int_to_tbox',
-    'float_to_tbox',
-    'timestamp_to_tbox',
-    'timestampset_to_tbox',
-    'period_to_tbox',
-    'periodset_to_tbox',
-    'int_timestamp_to_tbox',
-    'float_period_to_tbox',
-    'float_timestamp_to_tbox',
-    'geo_period_to_stbox',
-    'geo_timestamp_to_stbox',
-    'geo_to_stbox',
-    'int_period_to_tbox',
-    'numspan_to_tbox',
-    'span_timestamp_to_tbox',
-    'span_period_to_tbox',
-    'tbox_to_floatspan',
-    'tbox_to_period',
-    'stbox_to_period',
-    'tnumber_to_tbox',
-    'stbox_to_geo',
-    'tpoint_to_stbox',
-    'timestamp_to_stbox',
-    'timestampset_to_stbox',
-    'period_to_stbox',
-    'periodset_to_stbox',
-    'tbox_hasx',
-    'tbox_hast',
-    'tbox_xmin',
-    'tbox_xmax',
-    'tbox_tmin',
-    'tbox_tmax',
-    'stbox_hasx',
-    'stbox_hasz',
-    'stbox_hast',
-    'stbox_isgeodetic',
-    'stbox_xmin',
-    'stbox_xmax',
-    'stbox_ymin',
-    'stbox_ymax',
-    'stbox_zmin',
-    'stbox_zmax',
-    'stbox_tmin',
-    'stbox_tmax',
-    'stbox_srid',
-    'tbox_expand',
-    'tbox_expand_value',
-    'tbox_expand_time',
-    'stbox_expand',
-    'stbox_set_srid',
-    'stbox_get_space',
-    'stbox_expand_space',
-    'stbox_expand_time',
-    'contains_tbox_tbox',
-    'contained_tbox_tbox',
-    'overlaps_tbox_tbox',
-    'same_tbox_tbox',
-    'adjacent_tbox_tbox',
-    'contains_stbox_stbox',
-    'contained_stbox_stbox',
-    'overlaps_stbox_stbox',
-    'same_stbox_stbox',
-    'adjacent_stbox_stbox',
-    'left_tbox_tbox',
-    'overleft_tbox_tbox',
-    'right_tbox_tbox',
-    'overright_tbox_tbox',
-    'before_tbox_tbox',
-    'overbefore_tbox_tbox',
-    'after_tbox_tbox',
-    'overafter_tbox_tbox',
-    'left_stbox_stbox',
-    'overleft_stbox_stbox',
-    'right_stbox_stbox',
-    'overright_stbox_stbox',
-    'below_stbox_stbox',
-    'overbelow_stbox_stbox',
-    'above_stbox_stbox',
-    'overabove_stbox_stbox',
-    'front_stbox_stbox',
-    'overfront_stbox_stbox',
-    'back_stbox_stbox',
-    'overback_stbox_stbox',
-    'before_stbox_stbox',
-    'overbefore_stbox_stbox',
-    'after_stbox_stbox',
-    'overafter_stbox_stbox',
-    'union_tbox_tbox',
-    'inter_tbox_tbox',
-    'intersection_tbox_tbox',
-    'union_stbox_stbox',
-    'inter_stbox_stbox',
-    'intersection_stbox_stbox',
-    'stbox_quad_split',
-    'tbox_eq',
-    'tbox_ne',
-    'tbox_cmp',
-    'tbox_lt',
-    'tbox_le',
-    'tbox_ge',
-    'tbox_gt',
-    'stbox_eq',
-    'stbox_ne',
-    'stbox_cmp',
-    'stbox_lt',
-    'stbox_le',
-    'stbox_ge',
-    'stbox_gt',
-    'tbool_in',
-    'tbool_out',
-    'temporal_as_hexwkb',
-    'temporal_as_mfjson',
-    'temporal_as_wkb',
-    'temporal_from_hexwkb',
-    'temporal_from_mfjson',
-    'temporal_from_wkb',
-    'tfloat_in',
-    'tfloat_out',
-    'tgeogpoint_in',
-    'tgeompoint_in',
-    'tint_in',
-    'tint_out',
-    'tpoint_as_ewkt',
-    'tpoint_as_text',
-    'tpoint_out',
-    'ttext_in',
-    'ttext_out',
-    'tbool_from_base_temp',
-    'tboolinst_make',
-    'tboolseq_from_base_period',
-    'tboolseq_from_base_temp',
-    'tboolseq_from_base_timestampset',
-    'tboolseqset_from_base_periodset',
-    'tboolseqset_from_base_temp',
-    'temporal_copy',
-    'tfloat_from_base_temp',
-    'tfloatinst_make',
-    'tfloatseq_from_base_period',
-    'tfloatseq_from_base_temp',
-    'tfloatseq_from_base_timestampset',
-    'tfloatseqset_from_base_periodset',
-    'tfloatseqset_from_base_temp',
-    'tgeogpoint_from_base_temp',
-    'tgeogpointinst_make',
-    'tgeogpointseq_from_base_period',
-    'tgeogpointseq_from_base_temp',
-    'tgeogpointseq_from_base_timestampset',
-    'tgeogpointseqset_from_base_temp',
-    'tgeogpointseqset_from_base_periodset',
-    'tgeompoint_from_base_temp',
-    'tgeompointinst_make',
-    'tgeompointseq_from_base_period',
-    'tgeompointseq_from_base_temp',
-    'tgeompointseq_from_base_timestampset',
-    'tgeompointseqset_from_base_periodset',
-    'tgeompointseqset_from_base_temp',
-    'tint_from_base_temp',
-    'tintinst_make',
-    'tintseq_from_base_period',
-    'tintseq_from_base_temp',
-    'tintseq_from_base_timestampset',
-    'tintseqset_from_base_periodset',
-    'tintseqset_from_base_temp',
-    'tsequence_make',
-    'tsequence_make_exp',
-    'tsequenceset_make',
-    'tsequenceset_make_exp',
-    'tsequenceset_make_gaps',
-    'ttext_from_base_temp',
-    'ttextinst_make',
-    'ttextseq_from_base_period',
-    'ttextseq_from_base_temp',
-    'ttextseq_from_base_timestampset',
-    'ttextseqset_from_base_periodset',
-    'ttextseqset_from_base_temp',
-    'temporal_to_period',
-    'tfloat_to_tint',
-    'tint_to_tfloat',
-    'tnumber_to_span',
-    'tbool_end_value',
-    'tbool_start_value',
-    'tbool_values',
-    'temporal_duration',
-    'temporal_end_instant',
-    'temporal_end_sequence',
-    'temporal_end_timestamp',
-    'temporal_hash',
-    'temporal_instant_n',
-    'temporal_instants',
-    'temporal_interp',
-    'temporal_max_instant',
-    'temporal_min_instant',
-    'temporal_num_instants',
-    'temporal_num_sequences',
-    'temporal_num_timestamps',
-    'temporal_segments',
-    'temporal_sequence_n',
-    'temporal_sequences',
-    'temporal_start_instant',
-    'temporal_start_sequence',
-    'temporal_start_timestamp',
-    'temporal_stops',
-    'temporal_subtype',
-    'temporal_time',
-    'temporal_timestamp_n',
-    'temporal_timestamps',
-    'temporal_values',
-    'tfloat_end_value',
-    'tfloat_max_value',
-    'tfloat_min_value',
-    'tfloat_start_value',
-    'tfloat_values',
-    'tint_end_value',
-    'tint_max_value',
-    'tint_min_value',
-    'tint_start_value',
-    'tint_values',
-    'tnumber_valuespans',
-    'tpoint_end_value',
-    'tpoint_start_value',
-    'tpoint_values',
-    'ttext_end_value',
-    'ttext_max_value',
-    'ttext_min_value',
-    'ttext_start_value',
-    'ttext_values',
-    'temporal_set_interp',
-    'temporal_shift',
-    'temporal_shift_tscale',
-    'temporal_to_tinstant',
-    'temporal_to_tsequence',
-    'temporal_to_tsequenceset',
-    'temporal_tprecision',
-    'temporal_tsample',
-    'temporal_tscale',
-    'tbool_at_value',
-    'tbool_minus_value',
-    'tbool_value_at_timestamp',
-    'temporal_at_max',
-    'temporal_at_min',
-    'temporal_at_period',
-    'temporal_at_periodset',
-    'temporal_at_timestamp',
-    'temporal_at_timestampset',
-    'temporal_at_values',
-    'temporal_minus_max',
-    'temporal_minus_min',
-    'temporal_minus_period',
-    'temporal_minus_periodset',
-    'temporal_minus_timestamp',
-    'temporal_minus_timestampset',
-    'temporal_minus_values',
-    'tfloat_at_value',
-    'tfloat_minus_value',
-    'tfloat_value_at_timestamp',
-    'tint_at_value',
-    'tint_minus_value',
-    'tint_value_at_timestamp',
-    'tnumber_at_span',
-    'tnumber_at_spanset',
-    'tnumber_at_tbox',
-    'tnumber_minus_span',
-    'tnumber_minus_spanset',
-    'tnumber_minus_tbox',
-    'tpoint_at_geom_time',
-    'tpoint_at_stbox',
-    'tpoint_at_value',
-    'tpoint_minus_geom_time',
-    'tpoint_minus_stbox',
-    'tpoint_minus_value',
-    'tpoint_value_at_timestamp',
-    'ttext_at_value',
-    'ttext_minus_value',
-    'ttext_value_at_timestamp',
-    'temporal_append_tinstant',
-    'temporal_append_tsequence',
-    'temporal_delete_period',
-    'temporal_delete_periodset',
-    'temporal_delete_timestamp',
-    'temporal_delete_timestampset',
-    'temporal_insert',
-    'temporal_merge',
-    'temporal_merge_array',
-    'temporal_update',
-    'tand_bool_tbool',
-    'tand_tbool_bool',
-    'tand_tbool_tbool',
-    'tbool_when_true',
-    'tnot_tbool',
-    'tor_bool_tbool',
-    'tor_tbool_bool',
-    'tor_tbool_tbool',
-    'add_float_tfloat',
-    'add_int_tint',
-    'add_tfloat_float',
-    'add_tint_int',
-    'add_tnumber_tnumber',
-    'div_float_tfloat',
-    'div_int_tint',
-    'div_tfloat_float',
-    'div_tint_int',
-    'div_tnumber_tnumber',
-    'float_degrees',
-    'mult_float_tfloat',
-    'mult_int_tint',
-    'mult_tfloat_float',
-    'mult_tint_int',
-    'mult_tnumber_tnumber',
-    'sub_float_tfloat',
-    'sub_int_tint',
-    'sub_tfloat_float',
-    'sub_tint_int',
-    'sub_tnumber_tnumber',
-    'tfloat_degrees',
-    'tfloat_derivative',
-    'tfloat_radians',
-    'tnumber_abs',
-    'tnumber_angular_difference',
-    'tnumber_delta_value',
-    'textcat_text_ttext',
-    'textcat_ttext_text',
-    'textcat_ttext_ttext',
-    'ttext_upper',
-    'ttext_lower',
-    'distance_tfloat_float',
-    'distance_tint_int',
-    'distance_tnumber_tnumber',
-    'distance_tpoint_geo',
-    'distance_tpoint_tpoint',
-    'nad_stbox_geo',
-    'nad_stbox_stbox',
-    'nad_tbox_tbox',
-    'nad_tfloat_float',
-    'nad_tfloat_tfloat',
-    'nad_tint_int',
-    'nad_tint_tint',
-    'nad_tnumber_tbox',
-    'nad_tpoint_geo',
-    'nad_tpoint_stbox',
-    'nad_tpoint_tpoint',
-    'nai_tpoint_geo',
-    'nai_tpoint_tpoint',
-    'shortestline_tpoint_geo',
-    'shortestline_tpoint_tpoint',
-    'tbool_always_eq',
-    'tbool_ever_eq',
-    'tfloat_always_eq',
-    'tfloat_always_le',
-    'tfloat_always_lt',
-    'tfloat_ever_eq',
-    'tfloat_ever_le',
-    'tfloat_ever_lt',
-    'tgeogpoint_always_eq',
-    'tgeogpoint_ever_eq',
-    'tgeompoint_always_eq',
-    'tgeompoint_ever_eq',
-    'tint_always_eq',
-    'tint_always_le',
-    'tint_always_lt',
-    'tint_ever_eq',
-    'tint_ever_le',
-    'tint_ever_lt',
-    'tpoint_always_eq',
-    'tpoint_ever_eq',
-    'ttext_always_eq',
-    'ttext_always_le',
-    'ttext_always_lt',
-    'ttext_ever_eq',
-    'ttext_ever_le',
-    'ttext_ever_lt',
-    'temporal_cmp',
-    'temporal_eq',
-    'temporal_ge',
-    'temporal_gt',
-    'temporal_le',
-    'temporal_lt',
-    'temporal_ne',
-    'teq_bool_tbool',
-    'teq_float_tfloat',
-    'teq_geo_tpoint',
-    'teq_int_tint',
-    'teq_point_tgeogpoint',
-    'teq_point_tgeompoint',
-    'teq_tbool_bool',
-    'teq_temporal_temporal',
-    'teq_text_ttext',
-    'teq_tfloat_float',
-    'teq_tgeogpoint_point',
-    'teq_tgeompoint_point',
-    'teq_tint_int',
-    'teq_tpoint_geo',
-    'teq_ttext_text',
-    'tge_float_tfloat',
-    'tge_int_tint',
-    'tge_temporal_temporal',
-    'tge_text_ttext',
-    'tge_tfloat_float',
-    'tge_tint_int',
-    'tge_ttext_text',
-    'tgt_float_tfloat',
-    'tgt_int_tint',
-    'tgt_temporal_temporal',
-    'tgt_text_ttext',
-    'tgt_tfloat_float',
-    'tgt_tint_int',
-    'tgt_ttext_text',
-    'tle_float_tfloat',
-    'tle_int_tint',
-    'tle_temporal_temporal',
-    'tle_text_ttext',
-    'tle_tfloat_float',
-    'tle_tint_int',
-    'tle_ttext_text',
-    'tlt_float_tfloat',
-    'tlt_int_tint',
-    'tlt_temporal_temporal',
-    'tlt_text_ttext',
-    'tlt_tfloat_float',
-    'tlt_tint_int',
-    'tlt_ttext_text',
-    'tne_bool_tbool',
-    'tne_float_tfloat',
-    'tne_geo_tpoint',
-    'tne_int_tint',
-    'tne_point_tgeogpoint',
-    'tne_point_tgeompoint',
-    'tne_tbool_bool',
-    'tne_temporal_temporal',
-    'tne_text_ttext',
-    'tne_tfloat_float',
-    'tne_tgeogpoint_point',
-    'tne_tgeompoint_point',
-    'tne_tint_int',
-    'tne_tpoint_geo',
-    'tne_ttext_text',
-    'bearing_point_point',
-    'bearing_tpoint_point',
-    'bearing_tpoint_tpoint',
-    'tpoint_angular_difference',
-    'tpoint_azimuth',
-    'tpoint_convex_hull',
-    'tpoint_cumulative_length',
-    'tpoint_direction',
-    'tpoint_get_coord',
-    'tpoint_is_simple',
-    'tpoint_length',
-    'tpoint_speed',
-    'tpoint_srid',
-    'tpoint_stboxes',
-    'tpoint_trajectory',
-    'geo_expand_space',
-    'tgeompoint_tgeogpoint',
-    'tpoint_expand_space',
-    'tpoint_make_simple',
-    'tpoint_set_srid',
-    'econtains_geo_tpoint',
-    'edisjoint_tpoint_geo',
-    'edisjoint_tpoint_tpoint',
-    'edwithin_tpoint_geo',
-    'edwithin_tpoint_tpoint',
-    'eintersects_tpoint_geo',
-    'eintersects_tpoint_tpoint',
-    'etouches_tpoint_geo',
-    'tcontains_geo_tpoint',
-    'tdisjoint_tpoint_geo',
-    'tdwithin_tpoint_geo',
-    'tdwithin_tpoint_tpoint',
-    'tintersects_tpoint_geo',
-    'ttouches_tpoint_geo',
-    'tbool_tand_transfn',
-    'tbool_tor_transfn',
-    'temporal_extent_transfn',
-    'temporal_tagg_finalfn',
-    'temporal_tcount_transfn',
-    'tfloat_tmax_transfn',
-    'tfloat_tmin_transfn',
-    'tfloat_tsum_transfn',
-    'tint_tmax_transfn',
-    'tint_tmin_transfn',
-    'tint_tsum_transfn',
-    'tnumber_extent_transfn',
-    'tnumber_integral',
-    'tnumber_tavg_finalfn',
-    'tnumber_tavg_transfn',
-    'tnumber_twavg',
-    'tpoint_extent_transfn',
-    'tpoint_tcentroid_finalfn',
-    'tpoint_tcentroid_transfn',
-    'tpoint_twcentroid',
-    'ttext_tmax_transfn',
-    'ttext_tmin_transfn',
-    'float_bucket',
-    'floatspan_bucket_list',
-    'int_bucket',
-    'intspan_bucket_list',
-    'period_bucket_list',
-    'stbox_tile_list',
-    'tbox_tile_list',
-    'temporal_time_split',
-    'tfloat_value_split',
-    'tfloat_value_time_split',
-    'timestamptz_bucket',
-    'tint_value_split',
-    'tint_value_time_split',
-    'temporal_dyntimewarp_distance',
-    'temporal_dyntimewarp_path',
-    'temporal_frechet_distance',
-    'temporal_frechet_path',
-    'temporal_hausdorff_distance',
-    'geo_to_tpoint',
-    'temporal_simplify_min_dist',
-    'temporal_simplify_min_tdelta',
-    'temporal_simplify_dp',
-    'temporal_simplify_max_dist',
-    'tpoint_AsMVTGeom',
-    'tpoint_to_geo_meas',
-]
+from .functions import *
+
+__all__ = [
+    'create_pointer',
+    'get_address',
+    'datetime_to_timestamptz',
+    'timestamptz_to_datetime',
+    'timedelta_to_interval',
+    'interval_to_timedelta',
+    'geometry_to_gserialized',
+    'gserialized_to_shapely_point',
+    'gserialized_to_shapely_geometry',
+    'intrange_to_intspan',
+    'intspan_to_intrange',
+    'floatrange_to_floatspan',
+    'floatspan_to_floatrange',
+    'as_tinstant',
+    'as_tsequence',
+    'as_tsequenceset',
+    'lwpoint_make',
+    'lwgeom_from_gserialized',
+    'gserialized_from_lwgeom',
+    'lwgeom_get_srid',
+    'lwpoint_get_x',
+    'lwpoint_get_y',
+    'lwpoint_get_z',
+    'lwpoint_get_m',
+    'lwgeom_has_z',
+    'lwgeom_has_m',
+    'meos_initialize',
+    'meos_finalize',
+    'bool_in',
+    'bool_out',
+    'cstring2text',
+    'pg_date_in',
+    'pg_date_out',
+    'pg_interval_cmp',
+    'pg_interval_in',
+    'pg_interval_make',
+    'pg_interval_mul',
+    'pg_interval_out',
+    'pg_interval_pl',
+    'pg_time_in',
+    'pg_time_out',
+    'pg_timestamp_in',
+    'pg_timestamp_mi',
+    'pg_timestamp_mi_interval',
+    'pg_timestamp_out',
+    'pg_timestamp_pl_interval',
+    'pg_timestamptz_in',
+    'pg_timestamptz_out',
+    'text2cstring',
+    'gserialized_as_ewkb',
+    'gserialized_as_ewkt',
+    'gserialized_as_geojson',
+    'gserialized_as_hexewkb',
+    'gserialized_as_text',
+    'gserialized_from_ewkb',
+    'gserialized_from_geojson',
+    'gserialized_from_hexewkb',
+    'gserialized_from_text',
+    'gserialized_in',
+    'gserialized_out',
+    'pgis_gserialized_same',
+    'bigintset_in',
+    'bigintset_out',
+    'bigintspan_in',
+    'bigintspan_out',
+    'bigintspanset_in',
+    'bigintspanset_out',
+    'floatset_in',
+    'floatset_out',
+    'floatspan_in',
+    'floatspan_out',
+    'floatspanset_in',
+    'floatspanset_out',
+    'geogset_in',
+    'geogset_out',
+    'geomset_in',
+    'geomset_out',
+    'geoset_as_ewkt',
+    'geoset_as_text',
+    'intset_in',
+    'intset_out',
+    'intspan_in',
+    'intspan_out',
+    'intspanset_in',
+    'intspanset_out',
+    'period_in',
+    'period_out',
+    'periodset_in',
+    'periodset_out',
+    'set_as_hexwkb',
+    'set_as_wkb',
+    'set_from_hexwkb',
+    'set_from_wkb',
+    'set_out',
+    'span_as_wkb',
+    'span_as_hexwkb',
+    'span_from_hexwkb',
+    'span_from_wkb',
+    'span_out',
+    'spanset_as_wkb',
+    'spanset_as_hexwkb',
+    'spanset_from_hexwkb',
+    'spanset_from_wkb',
+    'spanset_out',
+    'textset_in',
+    'textset_out',
+    'timestampset_in',
+    'timestampset_out',
+    'bigintset_make',
+    'bigintspan_make',
+    'floatset_make',
+    'floatspan_make',
+    'geogset_make',
+    'geomset_make',
+    'intset_make',
+    'intspan_make',
+    'period_make',
+    'set_copy',
+    'span_copy',
+    'spanset_copy',
+    'spanset_make',
+    'spanset_make_exp',
+    'spanset_make_free',
+    'textset_make',
+    'timestampset_make',
+    'bigint_to_bigintset',
+    'bigint_to_bigintspan',
+    'bigint_to_bigintspanset',
+    'float_to_floatset',
+    'float_to_floatspan',
+    'float_to_floatspanset',
+    'int_to_intset',
+    'int_to_intspan',
+    'int_to_intspanset',
+    'set_to_spanset',
+    'span_to_spanset',
+    'timestamp_to_period',
+    'timestamp_to_periodset',
+    'timestamp_to_tstzset',
+    'bigintset_end_value',
+    'bigintset_start_value',
+    'bigintset_value_n',
+    'bigintset_values',
+    'bigintspan_lower',
+    'bigintspan_upper',
+    'bigintspanset_lower',
+    'bigintspanset_upper',
+    'floatset_end_value',
+    'floatset_start_value',
+    'floatset_value_n',
+    'floatset_values',
+    'floatspan_lower',
+    'floatspan_upper',
+    'floatspanset_lower',
+    'floatspanset_upper',
+    'geoset_srid',
+    'intset_end_value',
+    'intset_start_value',
+    'intset_value_n',
+    'intset_values',
+    'intspan_lower',
+    'intspan_upper',
+    'intspanset_lower',
+    'intspanset_upper',
+    'period_duration',
+    'period_lower',
+    'period_upper',
+    'periodset_duration',
+    'periodset_end_timestamp',
+    'periodset_lower',
+    'periodset_num_timestamps',
+    'periodset_start_timestamp',
+    'periodset_timestamp_n',
+    'periodset_timestamps',
+    'periodset_upper',
+    'set_hash',
+    'set_hash_extended',
+    'set_mem_size',
+    'set_num_values',
+    'set_span',
+    'span_hash',
+    'span_hash_extended',
+    'span_lower_inc',
+    'span_upper_inc',
+    'span_width',
+    'spanset_end_span',
+    'spanset_hash',
+    'spanset_hash_extended',
+    'spanset_lower_inc',
+    'spanset_mem_size',
+    'spanset_num_spans',
+    'spanset_span',
+    'spanset_span_n',
+    'spanset_spans',
+    'spanset_start_span',
+    'spanset_upper_inc',
+    'spanset_width',
+    'spatialset_stbox',
+    'timestampset_end_timestamp',
+    'timestampset_start_timestamp',
+    'timestampset_timestamp_n',
+    'timestampset_values',
+    'floatspan_set_intspan',
+    'intspan_set_floatspan',
+    'numspan_set_floatspan',
+    'period_tprecision',
+    'periodset_tprecision',
+    'period_shift_tscale',
+    'periodset_shift_tscale',
+    'set_shift',
+    'span_expand',
+    'timestamp_tprecision',
+    'timestampset_shift_tscale',
+    'adjacent_bigintspan_bigint',
+    'adjacent_bigintspanset_bigint',
+    'adjacent_floatspan_float',
+    'adjacent_intspan_int',
+    'adjacent_period_timestamp',
+    'adjacent_periodset_timestamp',
+    'adjacent_span_span',
+    'adjacent_spanset_span',
+    'adjacent_spanset_spanset',
+    'contained_bigint_bigintset',
+    'contained_bigint_bigintspan',
+    'contained_bigint_bigintspanset',
+    'contained_float_floatset',
+    'contained_float_floatspan',
+    'contained_float_floatspanset',
+    'contained_int_intset',
+    'contained_int_intspan',
+    'contained_set_set',
+    'contained_span_span',
+    'contained_span_spanset',
+    'contained_spanset_span',
+    'contained_spanset_spanset',
+    'contained_timestamp_period',
+    'contained_timestamp_timestampset',
+    'contains_floatspan_float',
+    'contains_floatspanset_float',
+    'contains_intspan_int',
+    'contains_set_set',
+    'contains_period_timestamp',
+    'contains_periodset_timestamp',
+    'contains_span_span',
+    'contains_span_spanset',
+    'contains_spanset_span',
+    'contains_spanset_spanset',
+    'contains_timestampset_timestamp',
+    'overlaps_set_set',
+    'overlaps_span_span',
+    'overlaps_spanset_span',
+    'overlaps_spanset_spanset',
+    'after_timestamp_timestampset',
+    'before_periodset_timestamp',
+    'before_timestamp_timestampset',
+    'left_float_floatspan',
+    'left_floatspan_float',
+    'left_int_intspan',
+    'left_intspan_int',
+    'left_set_set',
+    'left_span_span',
+    'left_span_spanset',
+    'left_spanset_span',
+    'left_spanset_spanset',
+    'overafter_period_timestamp',
+    'overafter_periodset_timestamp',
+    'overafter_timestamp_period',
+    'overafter_timestamp_periodset',
+    'overafter_timestamp_timestampset',
+    'overbefore_period_timestamp',
+    'overbefore_periodset_timestamp',
+    'overbefore_timestamp_period',
+    'overbefore_timestamp_periodset',
+    'overbefore_timestamp_timestampset',
+    'overleft_float_floatspan',
+    'overleft_floatspan_float',
+    'overleft_int_intspan',
+    'overleft_intspan_int',
+    'overleft_set_set',
+    'overleft_span_span',
+    'overleft_span_spanset',
+    'overleft_spanset_span',
+    'overleft_spanset_spanset',
+    'overright_float_floatspan',
+    'overright_floatspan_float',
+    'overright_int_intspan',
+    'overright_intspan_int',
+    'overright_set_set',
+    'overright_span_span',
+    'overright_span_spanset',
+    'overright_spanset_span',
+    'overright_spanset_spanset',
+    'right_float_floatspan',
+    'right_floatspan_float',
+    'right_int_intspan',
+    'right_intspan_int',
+    'right_set_set',
+    'right_span_span',
+    'right_span_spanset',
+    'right_spanset_span',
+    'right_spanset_spanset',
+    'bbox_union_span_span',
+    'intersection_set_set',
+    'intersection_period_timestamp',
+    'intersection_periodset_timestamp',
+    'intersection_span_span',
+    'intersection_spanset_span',
+    'intersection_spanset_spanset',
+    'intersection_timestampset_timestamp',
+    'minus_set_set',
+    'minus_period_timestamp',
+    'minus_periodset_timestamp',
+    'minus_span_span',
+    'minus_span_spanset',
+    'minus_spanset_span',
+    'minus_spanset_spanset',
+    'minus_timestamp_period',
+    'minus_timestamp_periodset',
+    'minus_timestampset_timestamp',
+    'union_set_set',
+    'union_period_timestamp',
+    'union_periodset_timestamp',
+    'union_span_span',
+    'union_spanset_span',
+    'union_spanset_spanset',
+    'union_timestampset_timestamp',
+    'distance_floatspan_float',
+    'distance_intspan_int',
+    'distance_set_set',
+    'distance_period_timestamp',
+    'distance_periodset_timestamp',
+    'distance_span_span',
+    'distance_spanset_span',
+    'distance_spanset_spanset',
+    'distance_timestampset_timestamp',
+    'bigint_extent_transfn',
+    'bigint_union_transfn',
+    'float_extent_transfn',
+    'float_union_transfn',
+    'int_extent_transfn',
+    'int_union_transfn',
+    'period_tcount_transfn',
+    'periodset_tcount_transfn',
+    'set_extent_transfn',
+    'set_union_finalfn',
+    'set_union_transfn',
+    'span_extent_transfn',
+    'span_union_transfn',
+    'spanset_extent_transfn',
+    'spanset_union_finalfn',
+    'spanset_union_transfn',
+    'text_union_transfn',
+    'timestamp_extent_transfn',
+    'timestamp_tcount_transfn',
+    'timestamp_union_transfn',
+    'timestampset_tcount_transfn',
+    'set_cmp',
+    'set_eq',
+    'set_ge',
+    'set_gt',
+    'set_le',
+    'set_lt',
+    'set_ne',
+    'span_cmp',
+    'span_eq',
+    'span_ge',
+    'span_gt',
+    'span_le',
+    'span_lt',
+    'span_ne',
+    'spanset_cmp',
+    'spanset_eq',
+    'spanset_ge',
+    'spanset_gt',
+    'spanset_le',
+    'spanset_lt',
+    'spanset_ne',
+    'tbox_in',
+    'tbox_out',
+    'tbox_from_wkb',
+    'tbox_from_hexwkb',
+    'stbox_from_wkb',
+    'stbox_from_hexwkb',
+    'tbox_as_wkb',
+    'tbox_as_hexwkb',
+    'stbox_as_wkb',
+    'stbox_as_hexwkb',
+    'stbox_in',
+    'stbox_out',
+    'tbox_make',
+    'tbox_set',
+    'tbox_copy',
+    'stbox_make',
+    'stbox_set',
+    'stbox_copy',
+    'int_to_tbox',
+    'float_to_tbox',
+    'timestamp_to_tbox',
+    'timestampset_to_tbox',
+    'period_to_tbox',
+    'periodset_to_tbox',
+    'int_timestamp_to_tbox',
+    'float_period_to_tbox',
+    'float_timestamp_to_tbox',
+    'geo_period_to_stbox',
+    'geo_timestamp_to_stbox',
+    'geo_to_stbox',
+    'int_period_to_tbox',
+    'numspan_to_tbox',
+    'span_timestamp_to_tbox',
+    'span_period_to_tbox',
+    'tbox_to_floatspan',
+    'tbox_to_period',
+    'stbox_to_period',
+    'tnumber_to_tbox',
+    'stbox_to_geo',
+    'tpoint_to_stbox',
+    'timestamp_to_stbox',
+    'timestampset_to_stbox',
+    'period_to_stbox',
+    'periodset_to_stbox',
+    'tbox_hasx',
+    'tbox_hast',
+    'tbox_xmin',
+    'tbox_xmax',
+    'tbox_tmin',
+    'tbox_tmax',
+    'stbox_hasx',
+    'stbox_hasz',
+    'stbox_hast',
+    'stbox_isgeodetic',
+    'stbox_xmin',
+    'stbox_xmax',
+    'stbox_ymin',
+    'stbox_ymax',
+    'stbox_zmin',
+    'stbox_zmax',
+    'stbox_tmin',
+    'stbox_tmax',
+    'stbox_srid',
+    'tbox_expand',
+    'tbox_expand_value',
+    'tbox_expand_time',
+    'stbox_expand',
+    'stbox_set_srid',
+    'stbox_get_space',
+    'stbox_expand_space',
+    'stbox_expand_time',
+    'contains_tbox_tbox',
+    'contained_tbox_tbox',
+    'overlaps_tbox_tbox',
+    'same_tbox_tbox',
+    'adjacent_tbox_tbox',
+    'contains_stbox_stbox',
+    'contained_stbox_stbox',
+    'overlaps_stbox_stbox',
+    'same_stbox_stbox',
+    'adjacent_stbox_stbox',
+    'left_tbox_tbox',
+    'overleft_tbox_tbox',
+    'right_tbox_tbox',
+    'overright_tbox_tbox',
+    'before_tbox_tbox',
+    'overbefore_tbox_tbox',
+    'after_tbox_tbox',
+    'overafter_tbox_tbox',
+    'left_stbox_stbox',
+    'overleft_stbox_stbox',
+    'right_stbox_stbox',
+    'overright_stbox_stbox',
+    'below_stbox_stbox',
+    'overbelow_stbox_stbox',
+    'above_stbox_stbox',
+    'overabove_stbox_stbox',
+    'front_stbox_stbox',
+    'overfront_stbox_stbox',
+    'back_stbox_stbox',
+    'overback_stbox_stbox',
+    'before_stbox_stbox',
+    'overbefore_stbox_stbox',
+    'after_stbox_stbox',
+    'overafter_stbox_stbox',
+    'union_tbox_tbox',
+    'inter_tbox_tbox',
+    'intersection_tbox_tbox',
+    'union_stbox_stbox',
+    'inter_stbox_stbox',
+    'intersection_stbox_stbox',
+    'stbox_quad_split',
+    'tbox_eq',
+    'tbox_ne',
+    'tbox_cmp',
+    'tbox_lt',
+    'tbox_le',
+    'tbox_ge',
+    'tbox_gt',
+    'stbox_eq',
+    'stbox_ne',
+    'stbox_cmp',
+    'stbox_lt',
+    'stbox_le',
+    'stbox_ge',
+    'stbox_gt',
+    'tbool_in',
+    'tbool_out',
+    'temporal_as_hexwkb',
+    'temporal_as_mfjson',
+    'temporal_as_wkb',
+    'temporal_from_hexwkb',
+    'temporal_from_mfjson',
+    'temporal_from_wkb',
+    'tfloat_in',
+    'tfloat_out',
+    'tgeogpoint_in',
+    'tgeompoint_in',
+    'tint_in',
+    'tint_out',
+    'tpoint_as_ewkt',
+    'tpoint_as_text',
+    'tpoint_out',
+    'ttext_in',
+    'ttext_out',
+    'tbool_from_base_temp',
+    'tboolinst_make',
+    'tboolseq_from_base_period',
+    'tboolseq_from_base_temp',
+    'tboolseq_from_base_timestampset',
+    'tboolseqset_from_base_periodset',
+    'tboolseqset_from_base_temp',
+    'temporal_copy',
+    'tfloat_from_base_temp',
+    'tfloatinst_make',
+    'tfloatseq_from_base_period',
+    'tfloatseq_from_base_temp',
+    'tfloatseq_from_base_timestampset',
+    'tfloatseqset_from_base_periodset',
+    'tfloatseqset_from_base_temp',
+    'tgeogpoint_from_base_temp',
+    'tgeogpointinst_make',
+    'tgeogpointseq_from_base_period',
+    'tgeogpointseq_from_base_temp',
+    'tgeogpointseq_from_base_timestampset',
+    'tgeogpointseqset_from_base_temp',
+    'tgeogpointseqset_from_base_periodset',
+    'tgeompoint_from_base_temp',
+    'tgeompointinst_make',
+    'tgeompointseq_from_base_period',
+    'tgeompointseq_from_base_temp',
+    'tgeompointseq_from_base_timestampset',
+    'tgeompointseqset_from_base_periodset',
+    'tgeompointseqset_from_base_temp',
+    'tint_from_base_temp',
+    'tintinst_make',
+    'tintseq_from_base_period',
+    'tintseq_from_base_temp',
+    'tintseq_from_base_timestampset',
+    'tintseqset_from_base_periodset',
+    'tintseqset_from_base_temp',
+    'tsequence_make',
+    'tsequence_make_exp',
+    'tsequenceset_make',
+    'tsequenceset_make_exp',
+    'tsequenceset_make_gaps',
+    'ttext_from_base_temp',
+    'ttextinst_make',
+    'ttextseq_from_base_period',
+    'ttextseq_from_base_temp',
+    'ttextseq_from_base_timestampset',
+    'ttextseqset_from_base_periodset',
+    'ttextseqset_from_base_temp',
+    'temporal_to_period',
+    'tfloat_to_tint',
+    'tint_to_tfloat',
+    'tnumber_to_span',
+    'tbool_end_value',
+    'tbool_start_value',
+    'tbool_values',
+    'temporal_duration',
+    'temporal_end_instant',
+    'temporal_end_sequence',
+    'temporal_end_timestamp',
+    'temporal_hash',
+    'temporal_instant_n',
+    'temporal_instants',
+    'temporal_interp',
+    'temporal_max_instant',
+    'temporal_min_instant',
+    'temporal_num_instants',
+    'temporal_num_sequences',
+    'temporal_num_timestamps',
+    'temporal_segments',
+    'temporal_sequence_n',
+    'temporal_sequences',
+    'temporal_start_instant',
+    'temporal_start_sequence',
+    'temporal_start_timestamp',
+    'temporal_stops',
+    'temporal_subtype',
+    'temporal_time',
+    'temporal_timestamp_n',
+    'temporal_timestamps',
+    'temporal_values',
+    'tfloat_end_value',
+    'tfloat_max_value',
+    'tfloat_min_value',
+    'tfloat_start_value',
+    'tfloat_values',
+    'tint_end_value',
+    'tint_max_value',
+    'tint_min_value',
+    'tint_start_value',
+    'tint_values',
+    'tnumber_valuespans',
+    'tpoint_end_value',
+    'tpoint_start_value',
+    'tpoint_values',
+    'ttext_end_value',
+    'ttext_max_value',
+    'ttext_min_value',
+    'ttext_start_value',
+    'ttext_values',
+    'temporal_set_interp',
+    'temporal_shift',
+    'temporal_shift_tscale',
+    'temporal_to_tinstant',
+    'temporal_to_tsequence',
+    'temporal_to_tsequenceset',
+    'temporal_tprecision',
+    'temporal_tsample',
+    'temporal_tscale',
+    'tbool_at_value',
+    'tbool_minus_value',
+    'tbool_value_at_timestamp',
+    'temporal_at_max',
+    'temporal_at_min',
+    'temporal_at_period',
+    'temporal_at_periodset',
+    'temporal_at_timestamp',
+    'temporal_at_timestampset',
+    'temporal_at_values',
+    'temporal_minus_max',
+    'temporal_minus_min',
+    'temporal_minus_period',
+    'temporal_minus_periodset',
+    'temporal_minus_timestamp',
+    'temporal_minus_timestampset',
+    'temporal_minus_values',
+    'tfloat_at_value',
+    'tfloat_minus_value',
+    'tfloat_value_at_timestamp',
+    'tint_at_value',
+    'tint_minus_value',
+    'tint_value_at_timestamp',
+    'tnumber_at_span',
+    'tnumber_at_spanset',
+    'tnumber_at_tbox',
+    'tnumber_minus_span',
+    'tnumber_minus_spanset',
+    'tnumber_minus_tbox',
+    'tpoint_at_geom_time',
+    'tpoint_at_stbox',
+    'tpoint_at_value',
+    'tpoint_minus_geom_time',
+    'tpoint_minus_stbox',
+    'tpoint_minus_value',
+    'tpoint_value_at_timestamp',
+    'ttext_at_value',
+    'ttext_minus_value',
+    'ttext_value_at_timestamp',
+    'temporal_append_tinstant',
+    'temporal_append_tsequence',
+    'temporal_delete_period',
+    'temporal_delete_periodset',
+    'temporal_delete_timestamp',
+    'temporal_delete_timestampset',
+    'temporal_insert',
+    'temporal_merge',
+    'temporal_merge_array',
+    'temporal_update',
+    'tand_bool_tbool',
+    'tand_tbool_bool',
+    'tand_tbool_tbool',
+    'tbool_when_true',
+    'tnot_tbool',
+    'tor_bool_tbool',
+    'tor_tbool_bool',
+    'tor_tbool_tbool',
+    'add_float_tfloat',
+    'add_int_tint',
+    'add_tfloat_float',
+    'add_tint_int',
+    'add_tnumber_tnumber',
+    'div_float_tfloat',
+    'div_int_tint',
+    'div_tfloat_float',
+    'div_tint_int',
+    'div_tnumber_tnumber',
+    'float_degrees',
+    'mult_float_tfloat',
+    'mult_int_tint',
+    'mult_tfloat_float',
+    'mult_tint_int',
+    'mult_tnumber_tnumber',
+    'sub_float_tfloat',
+    'sub_int_tint',
+    'sub_tfloat_float',
+    'sub_tint_int',
+    'sub_tnumber_tnumber',
+    'tfloat_degrees',
+    'tfloat_derivative',
+    'tfloat_radians',
+    'tnumber_abs',
+    'tnumber_angular_difference',
+    'tnumber_delta_value',
+    'textcat_text_ttext',
+    'textcat_ttext_text',
+    'textcat_ttext_ttext',
+    'ttext_upper',
+    'ttext_lower',
+    'distance_tfloat_float',
+    'distance_tint_int',
+    'distance_tnumber_tnumber',
+    'distance_tpoint_geo',
+    'distance_tpoint_tpoint',
+    'nad_stbox_geo',
+    'nad_stbox_stbox',
+    'nad_tbox_tbox',
+    'nad_tfloat_float',
+    'nad_tfloat_tfloat',
+    'nad_tint_int',
+    'nad_tint_tint',
+    'nad_tnumber_tbox',
+    'nad_tpoint_geo',
+    'nad_tpoint_stbox',
+    'nad_tpoint_tpoint',
+    'nai_tpoint_geo',
+    'nai_tpoint_tpoint',
+    'shortestline_tpoint_geo',
+    'shortestline_tpoint_tpoint',
+    'tbool_always_eq',
+    'tbool_ever_eq',
+    'tfloat_always_eq',
+    'tfloat_always_le',
+    'tfloat_always_lt',
+    'tfloat_ever_eq',
+    'tfloat_ever_le',
+    'tfloat_ever_lt',
+    'tgeogpoint_always_eq',
+    'tgeogpoint_ever_eq',
+    'tgeompoint_always_eq',
+    'tgeompoint_ever_eq',
+    'tint_always_eq',
+    'tint_always_le',
+    'tint_always_lt',
+    'tint_ever_eq',
+    'tint_ever_le',
+    'tint_ever_lt',
+    'tpoint_always_eq',
+    'tpoint_ever_eq',
+    'ttext_always_eq',
+    'ttext_always_le',
+    'ttext_always_lt',
+    'ttext_ever_eq',
+    'ttext_ever_le',
+    'ttext_ever_lt',
+    'temporal_cmp',
+    'temporal_eq',
+    'temporal_ge',
+    'temporal_gt',
+    'temporal_le',
+    'temporal_lt',
+    'temporal_ne',
+    'teq_bool_tbool',
+    'teq_float_tfloat',
+    'teq_geo_tpoint',
+    'teq_int_tint',
+    'teq_point_tgeogpoint',
+    'teq_point_tgeompoint',
+    'teq_tbool_bool',
+    'teq_temporal_temporal',
+    'teq_text_ttext',
+    'teq_tfloat_float',
+    'teq_tgeogpoint_point',
+    'teq_tgeompoint_point',
+    'teq_tint_int',
+    'teq_tpoint_geo',
+    'teq_ttext_text',
+    'tge_float_tfloat',
+    'tge_int_tint',
+    'tge_temporal_temporal',
+    'tge_text_ttext',
+    'tge_tfloat_float',
+    'tge_tint_int',
+    'tge_ttext_text',
+    'tgt_float_tfloat',
+    'tgt_int_tint',
+    'tgt_temporal_temporal',
+    'tgt_text_ttext',
+    'tgt_tfloat_float',
+    'tgt_tint_int',
+    'tgt_ttext_text',
+    'tle_float_tfloat',
+    'tle_int_tint',
+    'tle_temporal_temporal',
+    'tle_text_ttext',
+    'tle_tfloat_float',
+    'tle_tint_int',
+    'tle_ttext_text',
+    'tlt_float_tfloat',
+    'tlt_int_tint',
+    'tlt_temporal_temporal',
+    'tlt_text_ttext',
+    'tlt_tfloat_float',
+    'tlt_tint_int',
+    'tlt_ttext_text',
+    'tne_bool_tbool',
+    'tne_float_tfloat',
+    'tne_geo_tpoint',
+    'tne_int_tint',
+    'tne_point_tgeogpoint',
+    'tne_point_tgeompoint',
+    'tne_tbool_bool',
+    'tne_temporal_temporal',
+    'tne_text_ttext',
+    'tne_tfloat_float',
+    'tne_tgeogpoint_point',
+    'tne_tgeompoint_point',
+    'tne_tint_int',
+    'tne_tpoint_geo',
+    'tne_ttext_text',
+    'bearing_point_point',
+    'bearing_tpoint_point',
+    'bearing_tpoint_tpoint',
+    'tpoint_angular_difference',
+    'tpoint_azimuth',
+    'tpoint_convex_hull',
+    'tpoint_cumulative_length',
+    'tpoint_direction',
+    'tpoint_get_coord',
+    'tpoint_is_simple',
+    'tpoint_length',
+    'tpoint_speed',
+    'tpoint_srid',
+    'tpoint_stboxes',
+    'tpoint_trajectory',
+    'geo_expand_space',
+    'tgeompoint_tgeogpoint',
+    'tpoint_expand_space',
+    'tpoint_make_simple',
+    'tpoint_set_srid',
+    'econtains_geo_tpoint',
+    'edisjoint_tpoint_geo',
+    'edisjoint_tpoint_tpoint',
+    'edwithin_tpoint_geo',
+    'edwithin_tpoint_tpoint',
+    'eintersects_tpoint_geo',
+    'eintersects_tpoint_tpoint',
+    'etouches_tpoint_geo',
+    'tcontains_geo_tpoint',
+    'tdisjoint_tpoint_geo',
+    'tdwithin_tpoint_geo',
+    'tdwithin_tpoint_tpoint',
+    'tintersects_tpoint_geo',
+    'ttouches_tpoint_geo',
+    'tbool_tand_transfn',
+    'tbool_tor_transfn',
+    'temporal_extent_transfn',
+    'temporal_tagg_finalfn',
+    'temporal_tcount_transfn',
+    'tfloat_tmax_transfn',
+    'tfloat_tmin_transfn',
+    'tfloat_tsum_transfn',
+    'tint_tmax_transfn',
+    'tint_tmin_transfn',
+    'tint_tsum_transfn',
+    'tnumber_extent_transfn',
+    'tnumber_integral',
+    'tnumber_tavg_finalfn',
+    'tnumber_tavg_transfn',
+    'tnumber_twavg',
+    'tpoint_extent_transfn',
+    'tpoint_tcentroid_finalfn',
+    'tpoint_tcentroid_transfn',
+    'tpoint_twcentroid',
+    'ttext_tmax_transfn',
+    'ttext_tmin_transfn',
+    'float_bucket',
+    'floatspan_bucket_list',
+    'int_bucket',
+    'intspan_bucket_list',
+    'period_bucket_list',
+    'stbox_tile_list',
+    'tbox_tile_list',
+    'temporal_time_split',
+    'tfloat_value_split',
+    'tfloat_value_time_split',
+    'timestamptz_bucket',
+    'tint_value_split',
+    'tint_value_time_split',
+    'temporal_dyntimewarp_distance',
+    'temporal_dyntimewarp_path',
+    'temporal_frechet_distance',
+    'temporal_frechet_path',
+    'temporal_hausdorff_distance',
+    'geo_to_tpoint',
+    'temporal_simplify_min_dist',
+    'temporal_simplify_min_tdelta',
+    'temporal_simplify_dp',
+    'temporal_simplify_max_dist',
+    'tpoint_AsMVTGeom',
+    'tpoint_to_geo_meas',
+]
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_header.py` & `pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_header.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import re
-import subprocess
-import sys
-
-
-def get_defined_functions(library_path):
-    result = subprocess.check_output(['nm', '-gD', library_path])
-    output = result.decode('utf-8')
-    lines = output.splitlines()
-    defined = {line.split(' ')[-1] for line in lines if ' T ' in line}
-    return defined
-
-
-def remove_undefined_functions(content, so_path):
-    defined = get_defined_functions(so_path)
-
-    def remove_if_not_defined(m):
-        function = m.group(0).split('(')[0].strip().split(' ')[-1].strip('*')
-        if function in defined:
-            return m.group(0)
-        else:
-            print('Removing undefined function', function)
-            return ''
-
-    content = re.sub(r'^extern .*?;', remove_if_not_defined, content, flags=re.RegexFlag.MULTILINE)
-    return content
-
-
-def main(header_path, so_path=None):
-    with open(header_path, 'r') as f:
-        content = f.read()
-        # Remove comments
-        content = re.sub(r'//.*', '', content)
-        content = re.sub(r'/\*.*?\*/', '', content, flags=re.RegexFlag.MULTILINE)
-        # Comment macros that are not number constants
-        content = content.replace('#', '//#')
-        content = re.sub(r'^//(#define \w+ \d+)\s*$', r'\g<1>', content, flags=re.RegexFlag.MULTILINE)
-        # Add additional definitions
-        # content = content.replace(*ADDITIONAL_DEFINITIONS)
-
-        # Remove functions that are not actually defined in the library
-        if so_path:
-            content = remove_undefined_functions(content, so_path)
-
-    with open('pymeos_cffi/builder/meos.h', 'w') as f:
-        f.write(content)
-
-
-if __name__ == '__main__':
-    if len(sys.argv) > 1:
-        main(sys.argv[1])
-    else:
-        get_defined_functions('/usr/local/lib/libmeos.so')
-        main('/usr/local/include/meos.h', '/usr/local/lib/libmeos.so')
+import re
+import subprocess
+import sys
+
+
+def get_defined_functions(library_path):
+    result = subprocess.check_output(['nm', '-gD', library_path])
+    output = result.decode('utf-8')
+    lines = output.splitlines()
+    defined = {line.split(' ')[-1] for line in lines if ' T ' in line}
+    return defined
+
+
+def remove_undefined_functions(content, so_path):
+    defined = get_defined_functions(so_path)
+
+    def remove_if_not_defined(m):
+        function = m.group(0).split('(')[0].strip().split(' ')[-1].strip('*')
+        if function in defined:
+            return m.group(0)
+        else:
+            print('Removing undefined function', function)
+            return ''
+
+    content = re.sub(r'^extern .*?;', remove_if_not_defined, content, flags=re.RegexFlag.MULTILINE)
+    return content
+
+
+def main(header_path, so_path=None):
+    with open(header_path, 'r') as f:
+        content = f.read()
+        # Remove comments
+        content = re.sub(r'//.*', '', content)
+        content = re.sub(r'/\*.*?\*/', '', content, flags=re.RegexFlag.MULTILINE)
+        # Comment macros that are not number constants
+        content = content.replace('#', '//#')
+        content = re.sub(r'^//(#define \w+ \d+)\s*$', r'\g<1>', content, flags=re.RegexFlag.MULTILINE)
+        # Add additional definitions
+        # content = content.replace(*ADDITIONAL_DEFINITIONS)
+
+        # Remove functions that are not actually defined in the library
+        if so_path:
+            content = remove_undefined_functions(content, so_path)
+
+    with open('pymeos_cffi/builder/meos.h', 'w') as f:
+        f.write(content)
+
+
+if __name__ == '__main__':
+    if len(sys.argv) > 1:
+        main(sys.argv[1])
+    else:
+        get_defined_functions('/usr/local/lib/libmeos.so')
+        main('/usr/local/include/meos.h', '/usr/local/lib/libmeos.so')
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/builder/build_pymeos_functions.py` & `pymeos_cffi-1.1.0a2/pymeos_cffi/builder/build_pymeos_functions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,503 +1,503 @@
-import re
-from re import RegexFlag
-from typing import List, Optional
-
-from build_pymeos_functions_modifiers import *
-from objects import conversion_map, Conversion
-
-
-class Parameter:
-
-    def __init__(self, name: str, converted_name: str, ctype: str, ptype: str, cp_conversion: Optional[str]) -> None:
-        super().__init__()
-        self.name = name
-        self.converted_name = converted_name
-        self.ctype = ctype
-        self.ptype = ptype
-        self.cp_conversion = cp_conversion
-
-    def is_interoperable(self):
-        return any(self.ctype.startswith(x) for x in ['int', 'bool', 'double', 'TimestampTz'])
-
-    def get_ptype_without_pointers(self):
-        if self.is_interoperable():
-            return self.ptype.replace(" *'", "'").replace("**", '*')
-        else:
-            return self.ptype
-
-    def __str__(self) -> str:
-        return f'{self.name=}, {self.converted_name=}, {self.ctype=}, {self.ptype=}, {self.cp_conversion=}'
-
-
-class ReturnType:
-
-    def __init__(self, ctype: str, ptype: str, conversion: Optional[str]) -> None:
-        super().__init__()
-        self.ctype = ctype
-        self.return_type = ptype
-        self.conversion = conversion
-
-
-BASE = """from datetime import datetime, timedelta
-from typing import Any, Tuple, Optional, List, Union
-
-import _meos_cffi
-import postgis as pg
-import shapely.geometry as spg
-from dateutil.parser import parse
-from shapely import wkt, wkb, get_srid
-from shapely.geometry.base import BaseGeometry
-from spans.types import floatrange, intrange
-
-_ffi = _meos_cffi.ffi
-_lib = _meos_cffi.lib
-
-
-def create_pointer(object: 'Any', type: str) -> 'Any *':
-    return _ffi.new(f'{type} *', object)
-    
-
-def get_address(value: 'Any') -> 'Any *':
-    return _ffi.addressof(value)
-
-
-def datetime_to_timestamptz(dt: datetime) -> int:
-    return _lib.pg_timestamptz_in(dt.strftime('%Y-%m-%d %H:%M:%S%z').encode('utf-8'), -1)
-
-
-def timestamptz_to_datetime(ts: int) -> datetime:
-    return parse(pg_timestamptz_out(ts))
-
-
-def timedelta_to_interval(td: timedelta) -> Any:
-    return _ffi.new('Interval *', {'time': td.microseconds + td.seconds * 1000000, 'day': td.days, 'month': 0})
-
-
-def interval_to_timedelta(interval: Any) -> timedelta:
-    # TODO fix for months/years
-    return timedelta(days=interval.day, microseconds=interval.time)
-
-
-def geometry_to_gserialized(geom: Union[pg.Geometry, BaseGeometry], geodetic: Optional[bool] = None) -> 'GSERIALIZED *':
-    if isinstance(geom, pg.Geometry):
-        text = geom.to_ewkb()
-        if geom.has_srid():
-            text = f'SRID={geom.srid};{text}'
-    elif isinstance(geom, BaseGeometry):
-        text = wkb.dumps(geom, hex=True)
-        if get_srid(geom) > 0:
-            text = f'SRID={get_srid(geom)};{text}'
-    else:
-        raise TypeError('Parameter geom must be either a PostGIS Geometry or a Shapely BaseGeometry')
-    gs = gserialized_in(text, -1)
-    if geodetic is not None:
-        # GFlags is an 8-bit integer, where the 4th bit is the geodetic flag (0x80)
-        # If geodetic is True, then set the 4th bit to 1, otherwise set it to 0
-        gs.gflags = (gs.gflags | 0x08) if geodetic else (gs.gflags & 0xF7)
-    return gs
-
-
-def gserialized_to_shapely_point(geom: 'const GSERIALIZED *', precision: int = 6) -> spg.Point:
-    return wkt.loads(gserialized_as_text(geom, precision))
-
-
-def gserialized_to_shapely_geometry(geom: 'const GSERIALIZED *', precision: int = 6) -> BaseGeometry:
-    return wkt.loads(gserialized_as_text(geom, precision))
-
-
-def intrange_to_intspan(irange: intrange) -> 'Span *':
-    return intspan_make(irange.lower, irange.upper, irange.lower_inc, irange.upper_inc)
-
-
-def intspan_to_intrange(ispan: 'Span *') -> intrange:
-    return intrange(intspan_lower(ispan), intspan_upper(ispan), ispan.lower_inc, ispan.upper_inc)
-
-
-def floatrange_to_floatspan(frange: floatrange) -> 'Span *':
-    return floatspan_make(frange.lower, frange.upper, frange.lower_inc, frange.upper_inc)
-
-
-def floatspan_to_floatrange(fspan: 'Span *') -> floatrange:
-    return floatrange(floatspan_lower(fspan), floatspan_upper(fspan), fspan.lower_inc, fspan.upper_inc)
-
-
-def as_tinstant(temporal: 'Temporal *') -> 'TInstant *':
-    return _ffi.cast('TInstant *', temporal)
-
-
-def as_tsequence(temporal: 'Temporal *') -> 'TSequence *':
-    return _ffi.cast('TSequence *', temporal)
-
-
-def as_tsequenceset(temporal: 'Temporal *') -> 'TSequenceSet *':
-    return _ffi.cast('TSequenceSet *', temporal)
-
-
-# -----------------------------------------------------------------------------
-# ----------------------End of manually-defined functions----------------------
-# -----------------------------------------------------------------------------
-
-
-"""
-
-function_notes = {
-}
-
-function_modifiers = {
-    'cstring2text': cstring2text_modifier,
-    'text2cstring': text2cstring_modifier,
-    'timestampset_make': timestampset_make_modifier,
-    'tint_at_values': tint_at_values_modifier,
-    'tint_minus_values': tint_minus_values_modifier,
-    'tfloat_at_values': tfloat_at_values_modifier,
-    'tfloat_minus_values': tfloat_minus_values_modifier,
-    'tbool_at_values': tbool_at_values_modifier,
-    'tbool_minus_values': tbool_minus_values_modifier,
-    'ttext_at_values': array_length_remover_modifier('values_converted'),
-    'ttext_minus_values': array_length_remover_modifier('values_converted'),
-    'tpoint_at_values': array_length_remover_modifier('values_converted'),
-    'tpoint_minus_values': array_length_remover_modifier('values_converted'),
-    'gserialized_from_lwgeom': gserialized_from_lwgeom_modifier,
-    'tpointseq_make_coords': tpointseq_make_coords_modifier,
-    'spanset_make': spanset_make_modifier,
-}
-
-# List of result function parameters in tuples of (function, parameter)
-result_parameters = {
-    ('tbool_value_at_timestamp', 'value'),
-    ('ttext_value_at_timestamp', 'value'),
-    ('tint_value_at_timestamp', 'value'),
-    ('tfloat_value_at_timestamp', 'value'),
-    ('tpoint_value_at_timestamp', 'value'),
-}
-
-# List of output function parameters in tuples of (function, parameter). All parameters named result are assumed
-# to be output parameters, and it's not necessary to list them here.
-output_parameters = {
-    ('temporal_time_split', 'buckets'),
-    ('temporal_time_split', 'newcount'),
-    ('tint_value_split', 'buckets'),
-    ('tint_value_split', 'newcount'),
-    ('tfloat_value_split', 'buckets'),
-    ('tfloat_value_split', 'newcount'),
-    ('tint_value_time_split', 'newcount'),
-    ('tfloat_value_time_split', 'newcount'),
-    ('tbox_as_hexwkb', 'size'),
-    ('stbox_as_hexwkb', 'size'),
-    ('tbox_tile_list', 'rows'),
-    ('tbox_tile_list', 'columns'),
-    ('stbox_tile_list', 'cellcount'),
-}
-
-# List of nullable function parameters in tuples of (function, parameter)
-nullable_parameters = {
-    ('meos_initialize', 'tz_str'),
-    ('temporal_as_mfjson', 'srs'),
-    ('gserialized_as_geojson', 'srs'),
-    ('period_shift_tscale', 'shift'),
-    ('period_shift_tscale', 'duration'),
-    ('period_shift_tscale', 'delta'),
-    ('period_shift_tscale', 'scale'),
-    ('timestampset_shift_tscale', 'shift'),
-    ('timestampset_shift_tscale', 'duration'),
-    ('periodset_shift_tscale', 'shift'),
-    ('periodset_shift_tscale', 'duration'),
-    ('temporal_shift_tscale', 'shift'),
-    ('temporal_shift_tscale', 'duration'),
-    ('temporal_shift_tscale', 'shift'),
-    ('tbox_make', 'p'),
-    ('tbox_make', 's'),
-    ('stbox_make', 'p'),
-    ('tpointseq_make_coords', 'zcoords'),
-    ('temporal_tcount_transfn', 'state'),
-    ('temporal_extent_transfn', 'p'),
-    ('tnumber_extent_transfn', 'box'),
-    ('tpoint_extent_transfn', 'box'),
-    ('tbool_tand_transfn', 'state'),
-    ('tbool_tor_transfn', 'state'),
-    ('tint_tmin_transfn', 'state'),
-    ('tfloat_tmin_transfn', 'state'),
-    ('tint_tmax_transfn', 'state'),
-    ('tfloat_tmax_transfn', 'state'),
-    ('tint_tsum_transfn', 'state'),
-    ('tfloat_tsum_transfn', 'state'),
-    ('tnumber_tavg_transfn', 'state'),
-    ('ttext_tmin_transfn', 'state'),
-    ('ttext_tmax_transfn', 'state'),
-    ('temporal_tcount_transfn', 'interval'),
-    ('timestamp_tcount_transfn', 'interval'),
-    ('timestampset_tcount_transfn', 'interval'),
-    ('period_tcount_transfn', 'interval'),
-    ('periodset_tcount_transfn', 'interval'),
-    ('timestamp_extent_transfn', 'p'),
-    ('timestampset_extent_transfn', 'p'),
-    ('period_extent_transfn', 'p'),
-    ('periodset_extent_transfn', 'p'),
-    ('timestamp_tunion_transfn', 'state'),
-    ('timestampset_tunion_transfn', 'state'),
-    ('period_tunion_transfn', 'state'),
-    ('periodset_tunion_transfn', 'state'),
-    ('timestamp_tcount_transfn', 'state'),
-    ('timestampset_tcount_transfn', 'state'),
-    ('period_tcount_transfn', 'state'),
-    ('periodset_tcount_transfn', 'state'),
-    ('stbox_tile_list', 'duration'),
-    ('tbox_tile_list', 'xorigin'),
-    ('tbox_tile_list', 'torigin'),
-}
-
-
-# Checks if parameter in function is nullable
-def is_nullable_parameter(function: str, parameter: str) -> bool:
-    return (function, parameter) in nullable_parameters
-
-
-# Checks if parameter in function is actually a result parameter
-def is_result_parameter(function: str, parameter: Parameter) -> bool:
-    if parameter.name == 'result':
-        return True
-    return (function, parameter.name) in result_parameters
-
-
-# Checks if parameter in function is actually an output parameter
-def is_output_parameter(function: str, parameter: Parameter) -> bool:
-    if parameter.name.endswith('_out'):
-        return True
-    if parameter.name == 'count' and parameter.ptype.endswith("*'"):
-        return True
-    return (function, parameter.name) in output_parameters
-
-
-def main():
-    with open('pymeos_cffi/builder/meos.h') as f:
-        content = f.read()
-    # Regex lines:
-    # 1st line: Match beginning of function with optional "extern", "static" and "inline"
-    # 2nd line: Match the return type as any alphanumeric string with optional "const" modifier (before the type) or
-    #             pointer modifier (after the type)
-    # 3rd line: Match the name of the function as any alphanumeric string
-    # 4th line: Match the parameters as any sequence of alphanumeric characters, commas, spaces and asterisks between
-    #             parenthesis and end with a semicolon. (Parameter decomposition will be performed later)
-    f_regex = r'(?:extern )?(?:static )?(?:inline )?' \
-              r'(?P<returnType>(?:const )?\w+(?: \*+)?)' \
-              r'\s*(?P<function>\w+)' \
-              r'\((?P<params>[\w\s,\*]*)\);'
-    matches = re.finditer(f_regex, ''.join(content.splitlines()), flags=RegexFlag.MULTILINE)
-
-    with open('pymeos_cffi/functions.py', 'w+') as file:
-        file.write(BASE)
-        for match in matches:
-            named = match.groupdict()
-            function = named['function']
-            inner_return_type = named['returnType']
-            return_type = get_return_type(inner_return_type)
-            inner_params = named['params']
-            params = get_params(function, inner_params)
-            function_string = build_function_string(function, return_type, params)
-            file.write(function_string)
-            file.write('\n\n\n')
-
-    with open('pymeos_cffi/functions.py', 'r') as funcs, open('pymeos_cffi/__init__.py', 'w+') as init:
-        content = funcs.read()
-        f_names = re.finditer(r'def (\w+)\(', content)
-        init.write('from .functions import *\n\n')
-        init.write('__all__ = [\n')
-        for fn in f_names:
-            init.write(f"    '{fn.group(1)}',\n")
-        init.write(']\n')
-
-
-def get_params(function: str, inner_params: str) -> List[Parameter]:
-    return [p for p in (get_param(function, param.strip()) for param in inner_params.split(',')) if p is not None]
-
-
-# Creates Parameter object from a function parameter
-def get_param(function: str, inner_param: str) -> Optional[Parameter]:
-    # Split param name and type
-    split = inner_param.split(' ')
-
-    # Type is everything except last word
-    param_type = ' '.join(split[:-1])
-
-    # Check if parameter is pointer and fix type and name accordingly
-    if split[-1].startswith('**'):
-        param_type += ' **'
-    elif split[-1].startswith('*'):
-        param_type += ' *'
-    param_name = split[-1].lstrip('*')
-
-    # Check if the parameter name is a reserved word and change it if necessary
-    reserved_words = {
-        'str': 'string',
-        'is': 'iset',
-    }
-    if param_name in reserved_words:
-        param_name = reserved_words[param_name]
-
-    # Return None to remove the parameter if it's void
-    if param_name == 'void':
-        return None
-
-    # Get the type conversion
-    conversion = get_param_conversion(param_type)
-
-    # Check if parameter is nullable
-    nullable = is_nullable_parameter(function, param_name)
-
-    # If no conversion is needed between c and python types, use parameter name also as converted name
-    if conversion.p_to_c is None:
-        # If nullable, add null check
-        if nullable:
-            return Parameter(param_name, f'{param_name}_converted', param_type, f"'Optional[{conversion.p_type}]'",
-                             f'{param_name}_converted = {param_name} if {param_name} is not None else _ffi.NULL')
-        return Parameter(param_name, param_name, param_type, conversion.p_type, None)
-
-    # If a conversion is needed, create new name and add the conversion
-    if nullable:
-        return Parameter(param_name, f'{param_name}_converted', param_type, f'"Optional[{conversion.p_type}]"',
-                         f'{param_name}_converted = {conversion.p_to_c(param_name)} '
-                         f'if {param_name} is not None else _ffi.NULL')
-    return Parameter(param_name, f'{param_name}_converted', param_type, conversion.p_type,
-                     f'{param_name}_converted = {conversion.p_to_c(param_name)}')
-
-
-# Returns a conversion for a type
-def get_param_conversion(param_type: str) -> Conversion:
-    # Check if type is known
-    if param_type in conversion_map:
-        return conversion_map[param_type]
-    # Otherwise, create a new conversion
-
-    # If it's a double pointer, cast as array
-    if param_type.endswith('**'):
-        return Conversion(param_type, f"'{param_type}'",
-                          lambda name: f"[_ffi.cast('{param_type[:-1]}', x) for x in {name}]", lambda name: name)
-
-    # Otherwise, cast normally
-    else:
-        return Conversion(param_type, f"'{param_type}'", lambda name: f"_ffi.cast('{param_type}', {name})",
-                          lambda name: name)
-
-
-# Creates a ReturnType object from the function return type
-def get_return_type(inner_return_type) -> ReturnType:
-    # Check if a conversion is known
-    if inner_return_type in conversion_map:
-        conversion = conversion_map[inner_return_type]
-        return ReturnType(conversion.c_type, conversion.p_type,
-                          conversion.c_to_p('result') if conversion.c_to_p else None)
-    # Otherwise, don't transform anything
-    return ReturnType(inner_return_type, f"'{inner_return_type}'", None)
-
-
-def build_function_string(function_name: str, return_type: ReturnType, parameters: List[Parameter]) -> str:
-    # Check if there is a result param, i.e. output parameters that are the actual product of the function, instead of
-    # whatever the function returns (typically void or bool/int indicating the success or failure of the function)
-    result_param = None
-    if len(parameters) > 1 and is_result_parameter(function_name, parameters[-1]):
-        # Remove it from the list of parameters
-        result_param = parameters.pop(-1)
-
-    # Check if there are output parameters. Unlike result parameters, these are just normal parameters that provide
-    # extra information or actual results that are meant to go along with whatever the function returns
-    out_params = []
-    if len(parameters) > 1:
-        out_params = [p for p in parameters if is_output_parameter(function_name, p)]
-
-    # Create wrapper function parameter list
-    params = ', '.join(f'{p.name}: {p.ptype}' for p in parameters
-                       if p not in out_params)
-
-    # Create necessary conversions for the parameters
-    param_conversions = '\n    '.join(p.cp_conversion for p in parameters
-                                      if p.cp_conversion is not None and p not in out_params)
-
-    # Create CFFI function parameter list
-    inner_params = ', '.join(pc.name if pc in out_params else pc.converted_name for pc in parameters)
-
-    # Add result conversion if necessary
-    result_manipulation = None
-    if return_type.conversion is not None:
-        result_manipulation = f'    result = {return_type.conversion}\n'
-
-    # Initialize the function return type to the python type unless it needs no conversion (where the C type gives
-    # extra information while being interoperable), or the function is void
-    function_return_type = return_type.return_type \
-        if return_type.conversion is not None or return_type.return_type == 'None' \
-        else f"'{return_type.ctype}'"
-    # If there is a result param
-    if result_param is not None:
-        # Create the CFFI object to hold it
-        param_conversions += f"\n    out_result = _ffi.new('{result_param.ctype}')"
-        # Add it to the CFFI call param list
-        inner_params += ', out_result'
-
-        # If result is interoperable, remove pointer, otherwise, keep pointer
-        returning_object = 'out_result'
-        if result_param.is_interoperable():
-            returning_object += '[0]'
-
-        # If original C function returned bool, use it to return it when result is True, or raise exception when False
-        if return_type.return_type == 'bool':
-
-            result_manipulation = (result_manipulation or '') + \
-                                  "    if result:\n" \
-                                  f"        return {returning_object} if {returning_object} != _ffi.NULL else None\n" \
-                                  "    return None"
-        # Otherwise, just return it normally
-        else:
-            result_manipulation = (result_manipulation or '') + f'    return {returning_object} if {returning_object}' \
-                                                                f'!= _ffi.NULL else None\n'
-        # Set the return type as the Python type, removing the pointer modifier if necessary
-        function_return_type = result_param.get_ptype_without_pointers()
-    # Otherwise, return the result normally (if needed)
-    elif return_type.return_type != 'None':
-        result_manipulation = (result_manipulation or '') + '    return result if result != _ffi.NULL else None'
-
-    # For each output param
-    for out_param in out_params:
-        # Create the CFFI object to hold it
-        param_conversions += f"\n    {out_param.name} = _ffi.new('{out_param.ctype}')"
-        # Add its type to the return type of the function, removing the pointer modifier if necessary
-        function_return_type += ', ' + out_param.get_ptype_without_pointers()
-        # Add it to the return statement
-        result_manipulation += f', {out_param.name}[0]'
-
-    # If there are output params, wrap function return type in a Tuple
-    if len(out_params) > 0:
-        function_return_type = f'"Tuple[{function_return_type}]"'
-
-    # Add padding to param conversions
-    if len(param_conversions) > 0:
-        param_conversions = f'    {param_conversions}\n'
-
-    # Add TO DO note if the function is listed in the function_notes dictionary
-    note = ''
-    if function_name in function_notes:
-        note = f'#TODO {function_notes[function_name]}\n'
-
-    # Create common part of function string (note, name, parameters, return type and parameter conversions).
-    base = f'{note}def {function_name}({params}) -> {function_return_type}:\n' \
-           f'{param_conversions}'
-    # If the function didn't return anything, just add the function call to the base
-    if return_type.return_type == 'None':
-        function_string = f'{base}' \
-                          f'    _lib.{function_name}({inner_params})'
-    # Otherwise, store the result in a variable
-    else:
-        function_string = f'{base}' \
-                          f'    result = _lib.{function_name}({inner_params})'
-
-    # Add whatever manipulation the result needs (maybe empty)
-    if result_manipulation is not None:
-        function_string += f'\n{result_manipulation}'
-
-    # Check if there is function modifiers to modify specific elements of the function
-    if function_name in function_modifiers:
-        function_string = function_modifiers[function_name](function_string)
-
-    return function_string
-
-
-if __name__ == '__main__':
-    main()
+import re
+from re import RegexFlag
+from typing import List, Optional
+
+from build_pymeos_functions_modifiers import *
+from objects import conversion_map, Conversion
+
+
+class Parameter:
+
+    def __init__(self, name: str, converted_name: str, ctype: str, ptype: str, cp_conversion: Optional[str]) -> None:
+        super().__init__()
+        self.name = name
+        self.converted_name = converted_name
+        self.ctype = ctype
+        self.ptype = ptype
+        self.cp_conversion = cp_conversion
+
+    def is_interoperable(self):
+        return any(self.ctype.startswith(x) for x in ['int', 'bool', 'double', 'TimestampTz'])
+
+    def get_ptype_without_pointers(self):
+        if self.is_interoperable():
+            return self.ptype.replace(" *'", "'").replace("**", '*')
+        else:
+            return self.ptype
+
+    def __str__(self) -> str:
+        return f'{self.name=}, {self.converted_name=}, {self.ctype=}, {self.ptype=}, {self.cp_conversion=}'
+
+
+class ReturnType:
+
+    def __init__(self, ctype: str, ptype: str, conversion: Optional[str]) -> None:
+        super().__init__()
+        self.ctype = ctype
+        self.return_type = ptype
+        self.conversion = conversion
+
+
+BASE = """from datetime import datetime, timedelta
+from typing import Any, Tuple, Optional, List, Union
+
+import _meos_cffi
+import postgis as pg
+import shapely.geometry as spg
+from dateutil.parser import parse
+from shapely import wkt, wkb, get_srid
+from shapely.geometry.base import BaseGeometry
+from spans.types import floatrange, intrange
+
+_ffi = _meos_cffi.ffi
+_lib = _meos_cffi.lib
+
+
+def create_pointer(object: 'Any', type: str) -> 'Any *':
+    return _ffi.new(f'{type} *', object)
+    
+
+def get_address(value: 'Any') -> 'Any *':
+    return _ffi.addressof(value)
+
+
+def datetime_to_timestamptz(dt: datetime) -> int:
+    return _lib.pg_timestamptz_in(dt.strftime('%Y-%m-%d %H:%M:%S%z').encode('utf-8'), -1)
+
+
+def timestamptz_to_datetime(ts: int) -> datetime:
+    return parse(pg_timestamptz_out(ts))
+
+
+def timedelta_to_interval(td: timedelta) -> Any:
+    return _ffi.new('Interval *', {'time': td.microseconds + td.seconds * 1000000, 'day': td.days, 'month': 0})
+
+
+def interval_to_timedelta(interval: Any) -> timedelta:
+    # TODO fix for months/years
+    return timedelta(days=interval.day, microseconds=interval.time)
+
+
+def geometry_to_gserialized(geom: Union[pg.Geometry, BaseGeometry], geodetic: Optional[bool] = None) -> 'GSERIALIZED *':
+    if isinstance(geom, pg.Geometry):
+        text = geom.to_ewkb()
+        if geom.has_srid():
+            text = f'SRID={geom.srid};{text}'
+    elif isinstance(geom, BaseGeometry):
+        text = wkb.dumps(geom, hex=True)
+        if get_srid(geom) > 0:
+            text = f'SRID={get_srid(geom)};{text}'
+    else:
+        raise TypeError('Parameter geom must be either a PostGIS Geometry or a Shapely BaseGeometry')
+    gs = gserialized_in(text, -1)
+    if geodetic is not None:
+        # GFlags is an 8-bit integer, where the 4th bit is the geodetic flag (0x80)
+        # If geodetic is True, then set the 4th bit to 1, otherwise set it to 0
+        gs.gflags = (gs.gflags | 0x08) if geodetic else (gs.gflags & 0xF7)
+    return gs
+
+
+def gserialized_to_shapely_point(geom: 'const GSERIALIZED *', precision: int = 6) -> spg.Point:
+    return wkt.loads(gserialized_as_text(geom, precision))
+
+
+def gserialized_to_shapely_geometry(geom: 'const GSERIALIZED *', precision: int = 6) -> BaseGeometry:
+    return wkt.loads(gserialized_as_text(geom, precision))
+
+
+def intrange_to_intspan(irange: intrange) -> 'Span *':
+    return intspan_make(irange.lower, irange.upper, irange.lower_inc, irange.upper_inc)
+
+
+def intspan_to_intrange(ispan: 'Span *') -> intrange:
+    return intrange(intspan_lower(ispan), intspan_upper(ispan), ispan.lower_inc, ispan.upper_inc)
+
+
+def floatrange_to_floatspan(frange: floatrange) -> 'Span *':
+    return floatspan_make(frange.lower, frange.upper, frange.lower_inc, frange.upper_inc)
+
+
+def floatspan_to_floatrange(fspan: 'Span *') -> floatrange:
+    return floatrange(floatspan_lower(fspan), floatspan_upper(fspan), fspan.lower_inc, fspan.upper_inc)
+
+
+def as_tinstant(temporal: 'Temporal *') -> 'TInstant *':
+    return _ffi.cast('TInstant *', temporal)
+
+
+def as_tsequence(temporal: 'Temporal *') -> 'TSequence *':
+    return _ffi.cast('TSequence *', temporal)
+
+
+def as_tsequenceset(temporal: 'Temporal *') -> 'TSequenceSet *':
+    return _ffi.cast('TSequenceSet *', temporal)
+
+
+# -----------------------------------------------------------------------------
+# ----------------------End of manually-defined functions----------------------
+# -----------------------------------------------------------------------------
+
+
+"""
+
+function_notes = {
+}
+
+function_modifiers = {
+    'cstring2text': cstring2text_modifier,
+    'text2cstring': text2cstring_modifier,
+    'timestampset_make': timestampset_make_modifier,
+    'tint_at_values': tint_at_values_modifier,
+    'tint_minus_values': tint_minus_values_modifier,
+    'tfloat_at_values': tfloat_at_values_modifier,
+    'tfloat_minus_values': tfloat_minus_values_modifier,
+    'tbool_at_values': tbool_at_values_modifier,
+    'tbool_minus_values': tbool_minus_values_modifier,
+    'ttext_at_values': array_length_remover_modifier('values_converted'),
+    'ttext_minus_values': array_length_remover_modifier('values_converted'),
+    'tpoint_at_values': array_length_remover_modifier('values_converted'),
+    'tpoint_minus_values': array_length_remover_modifier('values_converted'),
+    'gserialized_from_lwgeom': gserialized_from_lwgeom_modifier,
+    'tpointseq_make_coords': tpointseq_make_coords_modifier,
+    'spanset_make': spanset_make_modifier,
+}
+
+# List of result function parameters in tuples of (function, parameter)
+result_parameters = {
+    ('tbool_value_at_timestamp', 'value'),
+    ('ttext_value_at_timestamp', 'value'),
+    ('tint_value_at_timestamp', 'value'),
+    ('tfloat_value_at_timestamp', 'value'),
+    ('tpoint_value_at_timestamp', 'value'),
+}
+
+# List of output function parameters in tuples of (function, parameter). All parameters named result are assumed
+# to be output parameters, and it's not necessary to list them here.
+output_parameters = {
+    ('temporal_time_split', 'buckets'),
+    ('temporal_time_split', 'newcount'),
+    ('tint_value_split', 'buckets'),
+    ('tint_value_split', 'newcount'),
+    ('tfloat_value_split', 'buckets'),
+    ('tfloat_value_split', 'newcount'),
+    ('tint_value_time_split', 'newcount'),
+    ('tfloat_value_time_split', 'newcount'),
+    ('tbox_as_hexwkb', 'size'),
+    ('stbox_as_hexwkb', 'size'),
+    ('tbox_tile_list', 'rows'),
+    ('tbox_tile_list', 'columns'),
+    ('stbox_tile_list', 'cellcount'),
+}
+
+# List of nullable function parameters in tuples of (function, parameter)
+nullable_parameters = {
+    ('meos_initialize', 'tz_str'),
+    ('temporal_as_mfjson', 'srs'),
+    ('gserialized_as_geojson', 'srs'),
+    ('period_shift_tscale', 'shift'),
+    ('period_shift_tscale', 'duration'),
+    ('period_shift_tscale', 'delta'),
+    ('period_shift_tscale', 'scale'),
+    ('timestampset_shift_tscale', 'shift'),
+    ('timestampset_shift_tscale', 'duration'),
+    ('periodset_shift_tscale', 'shift'),
+    ('periodset_shift_tscale', 'duration'),
+    ('temporal_shift_tscale', 'shift'),
+    ('temporal_shift_tscale', 'duration'),
+    ('temporal_shift_tscale', 'shift'),
+    ('tbox_make', 'p'),
+    ('tbox_make', 's'),
+    ('stbox_make', 'p'),
+    ('tpointseq_make_coords', 'zcoords'),
+    ('temporal_tcount_transfn', 'state'),
+    ('temporal_extent_transfn', 'p'),
+    ('tnumber_extent_transfn', 'box'),
+    ('tpoint_extent_transfn', 'box'),
+    ('tbool_tand_transfn', 'state'),
+    ('tbool_tor_transfn', 'state'),
+    ('tint_tmin_transfn', 'state'),
+    ('tfloat_tmin_transfn', 'state'),
+    ('tint_tmax_transfn', 'state'),
+    ('tfloat_tmax_transfn', 'state'),
+    ('tint_tsum_transfn', 'state'),
+    ('tfloat_tsum_transfn', 'state'),
+    ('tnumber_tavg_transfn', 'state'),
+    ('ttext_tmin_transfn', 'state'),
+    ('ttext_tmax_transfn', 'state'),
+    ('temporal_tcount_transfn', 'interval'),
+    ('timestamp_tcount_transfn', 'interval'),
+    ('timestampset_tcount_transfn', 'interval'),
+    ('period_tcount_transfn', 'interval'),
+    ('periodset_tcount_transfn', 'interval'),
+    ('timestamp_extent_transfn', 'p'),
+    ('timestampset_extent_transfn', 'p'),
+    ('period_extent_transfn', 'p'),
+    ('periodset_extent_transfn', 'p'),
+    ('timestamp_tunion_transfn', 'state'),
+    ('timestampset_tunion_transfn', 'state'),
+    ('period_tunion_transfn', 'state'),
+    ('periodset_tunion_transfn', 'state'),
+    ('timestamp_tcount_transfn', 'state'),
+    ('timestampset_tcount_transfn', 'state'),
+    ('period_tcount_transfn', 'state'),
+    ('periodset_tcount_transfn', 'state'),
+    ('stbox_tile_list', 'duration'),
+    ('tbox_tile_list', 'xorigin'),
+    ('tbox_tile_list', 'torigin'),
+}
+
+
+# Checks if parameter in function is nullable
+def is_nullable_parameter(function: str, parameter: str) -> bool:
+    return (function, parameter) in nullable_parameters
+
+
+# Checks if parameter in function is actually a result parameter
+def is_result_parameter(function: str, parameter: Parameter) -> bool:
+    if parameter.name == 'result':
+        return True
+    return (function, parameter.name) in result_parameters
+
+
+# Checks if parameter in function is actually an output parameter
+def is_output_parameter(function: str, parameter: Parameter) -> bool:
+    if parameter.name.endswith('_out'):
+        return True
+    if parameter.name == 'count' and parameter.ptype.endswith("*'"):
+        return True
+    return (function, parameter.name) in output_parameters
+
+
+def main():
+    with open('pymeos_cffi/builder/meos.h') as f:
+        content = f.read()
+    # Regex lines:
+    # 1st line: Match beginning of function with optional "extern", "static" and "inline"
+    # 2nd line: Match the return type as any alphanumeric string with optional "const" modifier (before the type) or
+    #             pointer modifier (after the type)
+    # 3rd line: Match the name of the function as any alphanumeric string
+    # 4th line: Match the parameters as any sequence of alphanumeric characters, commas, spaces and asterisks between
+    #             parenthesis and end with a semicolon. (Parameter decomposition will be performed later)
+    f_regex = r'(?:extern )?(?:static )?(?:inline )?' \
+              r'(?P<returnType>(?:const )?\w+(?: \*+)?)' \
+              r'\s*(?P<function>\w+)' \
+              r'\((?P<params>[\w\s,\*]*)\);'
+    matches = re.finditer(f_regex, ''.join(content.splitlines()), flags=RegexFlag.MULTILINE)
+
+    with open('pymeos_cffi/functions.py', 'w+') as file:
+        file.write(BASE)
+        for match in matches:
+            named = match.groupdict()
+            function = named['function']
+            inner_return_type = named['returnType']
+            return_type = get_return_type(inner_return_type)
+            inner_params = named['params']
+            params = get_params(function, inner_params)
+            function_string = build_function_string(function, return_type, params)
+            file.write(function_string)
+            file.write('\n\n\n')
+
+    with open('pymeos_cffi/functions.py', 'r') as funcs, open('pymeos_cffi/__init__.py', 'w+') as init:
+        content = funcs.read()
+        f_names = re.finditer(r'def (\w+)\(', content)
+        init.write('from .functions import *\n\n')
+        init.write('__all__ = [\n')
+        for fn in f_names:
+            init.write(f"    '{fn.group(1)}',\n")
+        init.write(']\n')
+
+
+def get_params(function: str, inner_params: str) -> List[Parameter]:
+    return [p for p in (get_param(function, param.strip()) for param in inner_params.split(',')) if p is not None]
+
+
+# Creates Parameter object from a function parameter
+def get_param(function: str, inner_param: str) -> Optional[Parameter]:
+    # Split param name and type
+    split = inner_param.split(' ')
+
+    # Type is everything except last word
+    param_type = ' '.join(split[:-1])
+
+    # Check if parameter is pointer and fix type and name accordingly
+    if split[-1].startswith('**'):
+        param_type += ' **'
+    elif split[-1].startswith('*'):
+        param_type += ' *'
+    param_name = split[-1].lstrip('*')
+
+    # Check if the parameter name is a reserved word and change it if necessary
+    reserved_words = {
+        'str': 'string',
+        'is': 'iset',
+    }
+    if param_name in reserved_words:
+        param_name = reserved_words[param_name]
+
+    # Return None to remove the parameter if it's void
+    if param_name == 'void':
+        return None
+
+    # Get the type conversion
+    conversion = get_param_conversion(param_type)
+
+    # Check if parameter is nullable
+    nullable = is_nullable_parameter(function, param_name)
+
+    # If no conversion is needed between c and python types, use parameter name also as converted name
+    if conversion.p_to_c is None:
+        # If nullable, add null check
+        if nullable:
+            return Parameter(param_name, f'{param_name}_converted', param_type, f"'Optional[{conversion.p_type}]'",
+                             f'{param_name}_converted = {param_name} if {param_name} is not None else _ffi.NULL')
+        return Parameter(param_name, param_name, param_type, conversion.p_type, None)
+
+    # If a conversion is needed, create new name and add the conversion
+    if nullable:
+        return Parameter(param_name, f'{param_name}_converted', param_type, f'"Optional[{conversion.p_type}]"',
+                         f'{param_name}_converted = {conversion.p_to_c(param_name)} '
+                         f'if {param_name} is not None else _ffi.NULL')
+    return Parameter(param_name, f'{param_name}_converted', param_type, conversion.p_type,
+                     f'{param_name}_converted = {conversion.p_to_c(param_name)}')
+
+
+# Returns a conversion for a type
+def get_param_conversion(param_type: str) -> Conversion:
+    # Check if type is known
+    if param_type in conversion_map:
+        return conversion_map[param_type]
+    # Otherwise, create a new conversion
+
+    # If it's a double pointer, cast as array
+    if param_type.endswith('**'):
+        return Conversion(param_type, f"'{param_type}'",
+                          lambda name: f"[_ffi.cast('{param_type[:-1]}', x) for x in {name}]", lambda name: name)
+
+    # Otherwise, cast normally
+    else:
+        return Conversion(param_type, f"'{param_type}'", lambda name: f"_ffi.cast('{param_type}', {name})",
+                          lambda name: name)
+
+
+# Creates a ReturnType object from the function return type
+def get_return_type(inner_return_type) -> ReturnType:
+    # Check if a conversion is known
+    if inner_return_type in conversion_map:
+        conversion = conversion_map[inner_return_type]
+        return ReturnType(conversion.c_type, conversion.p_type,
+                          conversion.c_to_p('result') if conversion.c_to_p else None)
+    # Otherwise, don't transform anything
+    return ReturnType(inner_return_type, f"'{inner_return_type}'", None)
+
+
+def build_function_string(function_name: str, return_type: ReturnType, parameters: List[Parameter]) -> str:
+    # Check if there is a result param, i.e. output parameters that are the actual product of the function, instead of
+    # whatever the function returns (typically void or bool/int indicating the success or failure of the function)
+    result_param = None
+    if len(parameters) > 1 and is_result_parameter(function_name, parameters[-1]):
+        # Remove it from the list of parameters
+        result_param = parameters.pop(-1)
+
+    # Check if there are output parameters. Unlike result parameters, these are just normal parameters that provide
+    # extra information or actual results that are meant to go along with whatever the function returns
+    out_params = []
+    if len(parameters) > 1:
+        out_params = [p for p in parameters if is_output_parameter(function_name, p)]
+
+    # Create wrapper function parameter list
+    params = ', '.join(f'{p.name}: {p.ptype}' for p in parameters
+                       if p not in out_params)
+
+    # Create necessary conversions for the parameters
+    param_conversions = '\n    '.join(p.cp_conversion for p in parameters
+                                      if p.cp_conversion is not None and p not in out_params)
+
+    # Create CFFI function parameter list
+    inner_params = ', '.join(pc.name if pc in out_params else pc.converted_name for pc in parameters)
+
+    # Add result conversion if necessary
+    result_manipulation = None
+    if return_type.conversion is not None:
+        result_manipulation = f'    result = {return_type.conversion}\n'
+
+    # Initialize the function return type to the python type unless it needs no conversion (where the C type gives
+    # extra information while being interoperable), or the function is void
+    function_return_type = return_type.return_type \
+        if return_type.conversion is not None or return_type.return_type == 'None' \
+        else f"'{return_type.ctype}'"
+    # If there is a result param
+    if result_param is not None:
+        # Create the CFFI object to hold it
+        param_conversions += f"\n    out_result = _ffi.new('{result_param.ctype}')"
+        # Add it to the CFFI call param list
+        inner_params += ', out_result'
+
+        # If result is interoperable, remove pointer, otherwise, keep pointer
+        returning_object = 'out_result'
+        if result_param.is_interoperable():
+            returning_object += '[0]'
+
+        # If original C function returned bool, use it to return it when result is True, or raise exception when False
+        if return_type.return_type == 'bool':
+
+            result_manipulation = (result_manipulation or '') + \
+                                  "    if result:\n" \
+                                  f"        return {returning_object} if {returning_object} != _ffi.NULL else None\n" \
+                                  "    return None"
+        # Otherwise, just return it normally
+        else:
+            result_manipulation = (result_manipulation or '') + f'    return {returning_object} if {returning_object}' \
+                                                                f'!= _ffi.NULL else None\n'
+        # Set the return type as the Python type, removing the pointer modifier if necessary
+        function_return_type = result_param.get_ptype_without_pointers()
+    # Otherwise, return the result normally (if needed)
+    elif return_type.return_type != 'None':
+        result_manipulation = (result_manipulation or '') + '    return result if result != _ffi.NULL else None'
+
+    # For each output param
+    for out_param in out_params:
+        # Create the CFFI object to hold it
+        param_conversions += f"\n    {out_param.name} = _ffi.new('{out_param.ctype}')"
+        # Add its type to the return type of the function, removing the pointer modifier if necessary
+        function_return_type += ', ' + out_param.get_ptype_without_pointers()
+        # Add it to the return statement
+        result_manipulation += f', {out_param.name}[0]'
+
+    # If there are output params, wrap function return type in a Tuple
+    if len(out_params) > 0:
+        function_return_type = f'"Tuple[{function_return_type}]"'
+
+    # Add padding to param conversions
+    if len(param_conversions) > 0:
+        param_conversions = f'    {param_conversions}\n'
+
+    # Add TO DO note if the function is listed in the function_notes dictionary
+    note = ''
+    if function_name in function_notes:
+        note = f'#TODO {function_notes[function_name]}\n'
+
+    # Create common part of function string (note, name, parameters, return type and parameter conversions).
+    base = f'{note}def {function_name}({params}) -> {function_return_type}:\n' \
+           f'{param_conversions}'
+    # If the function didn't return anything, just add the function call to the base
+    if return_type.return_type == 'None':
+        function_string = f'{base}' \
+                          f'    _lib.{function_name}({inner_params})'
+    # Otherwise, store the result in a variable
+    else:
+        function_string = f'{base}' \
+                          f'    result = _lib.{function_name}({inner_params})'
+
+    # Add whatever manipulation the result needs (maybe empty)
+    if result_manipulation is not None:
+        function_string += f'\n{result_manipulation}'
+
+    # Check if there is function modifiers to modify specific elements of the function
+    if function_name in function_modifiers:
+        function_string = function_modifiers[function_name](function_string)
+
+    return function_string
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/builder/meos.h` & `pymeos_cffi-1.1.0a2/pymeos_cffi/builder/meos.h`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1854 +1,1854 @@
-/*****************************************************************************
- *
- * This MobilityDB code is provided under The PostgreSQL License.
- * Copyright (c) 2016-2023, Université libre de Bruxelles and MobilityDB
- * contributors
- *
- * MobilityDB includes portions of PostGIS version 3 source code released
- * under the GNU General Public License (GPLv2 or later).
- * Copyright (c) 2001-2023, PostGIS contributors
- *
- * Permission to use, copy, modify, and distribute this software and its
- * documentation for any purpose, without fee, and without a written
- * agreement is hereby granted, provided that the above copyright notice and
- * this paragraph and the following two paragraphs appear in all copies.
- *
- * IN NO EVENT SHALL UNIVERSITE LIBRE DE BRUXELLES BE LIABLE TO ANY PARTY FOR
- * DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING
- * LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION,
- * EVEN IF UNIVERSITE LIBRE DE BRUXELLES HAS BEEN ADVISED OF THE POSSIBILITY
- * OF SUCH DAMAGE.
- *
- * UNIVERSITE LIBRE DE BRUXELLES SPECIFICALLY DISCLAIMS ANY WARRANTIES,
- * INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY
- * AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON
- * AN "AS IS" BASIS, AND UNIVERSITE LIBRE DE BRUXELLES HAS NO OBLIGATIONS TO
- * PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
- *
- *****************************************************************************/
-
-/**
- * @brief API of the Mobility Engine Open Source (MEOS) library.
- */
-
-//#ifndef __MEOS_H__
-//#define __MEOS_H__
-
-
-//#include <stdbool.h>
-//#include <stdint.h>
-
-//#ifndef POSTGRES_H
-//#define POSTGRES_H
-
-//#define DatumGetPointer(X) ((Pointer) (X))
-
-typedef char *Pointer;
-typedef uintptr_t Datum;
-
-typedef signed char int8;
-typedef signed short int16;
-typedef signed int int32;
-typedef long int int64;
-
-typedef unsigned char uint8;
-typedef unsigned short uint16;
-typedef unsigned int uint32;
-typedef unsigned long int uint64;
-
-typedef int32 DateADT;
-typedef int64 TimeADT;
-typedef int64 Timestamp;
-typedef int64 TimestampTz;
-typedef int64 TimeOffset;
-typedef int32 fsec_t;      
-
-typedef struct
-{
-  TimeOffset time;  
-  int32 day;        
-  int32 month;      
-} Interval;
-
-typedef struct varlena
-{
-  char vl_len_[4];  
-  char vl_dat[];    
-} varlena;
-
-typedef varlena text;
-typedef struct varlena bytea;
-
-//#endif              
-
-
-//#ifndef _LIBLWGEOM_H
-//#define _LIBLWGEOM_H
-
-
-
-/**
-* Macros for manipulating the 'flags' byte. A uint8_t used as follows:
-* VVSRGBMZ
-* Version bit, followed by
-* Validty, Solid, ReadOnly, Geodetic, HasBBox, HasM and HasZ flags.
-*/
-//#define LWFLAG_Z        0x01
-//#define LWFLAG_M        0x02
-//#define LWFLAG_BBOX     0x04
-//#define LWFLAG_GEODETIC 0x08
-//#define LWFLAG_READONLY 0x10
-//#define LWFLAG_SOLID    0x20
-
-//#define FLAGS_GET_Z(flags)         ((flags) & LWFLAG_Z)
-//#define FLAGS_GET_M(flags)        (((flags) & LWFLAG_M)>>1)
-//#define FLAGS_GET_BBOX(flags)     (((flags) & LWFLAG_BBOX)>>2)
-//#define FLAGS_GET_GEODETIC(flags) (((flags) & LWFLAG_GEODETIC)>>3)
-//#define FLAGS_GET_READONLY(flags) (((flags) & LWFLAG_READONLY)>>4)
-//#define FLAGS_GET_SOLID(flags)    (((flags) & LWFLAG_SOLID)>>5)
-
-//#define FLAGS_SET_Z(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_Z) : ((flags) & ~LWFLAG_Z))
-//#define FLAGS_SET_M(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_M) : ((flags) & ~LWFLAG_M))
-//#define FLAGS_SET_BBOX(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_BBOX) : ((flags) & ~LWFLAG_BBOX))
-//#define FLAGS_SET_GEODETIC(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_GEODETIC) : ((flags) & ~LWFLAG_GEODETIC))
-//#define FLAGS_SET_READONLY(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_READONLY) : ((flags) & ~LWFLAG_READONLY))
-//#define FLAGS_SET_SOLID(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_SOLID) : ((flags) & ~LWFLAG_SOLID))
-
-//#define FLAGS_NDIMS(flags) (2 + FLAGS_GET_Z(flags) + FLAGS_GET_M(flags))
-//#define FLAGS_GET_ZM(flags) (FLAGS_GET_M(flags) + FLAGS_GET_Z(flags) * 2)
-//#define FLAGS_NDIMS_BOX(flags) (FLAGS_GET_GEODETIC(flags) ? 3 : FLAGS_NDIMS(flags))
-
-/*
-** Variants available for WKB and WKT output types
-*/
-
-//#define WKB_ISO 0x01
-//#define WKB_SFSQL 0x02
-//#define WKB_EXTENDED 0x04
-//#define WKB_NDR 0x08
-//#define WKB_XDR 0x10
-//#define WKB_HEX 0x20
-//#define WKB_NO_NPOINTS 0x40 
-//#define WKB_NO_SRID 0x80 
-
-//#define WKT_ISO 0x01
-//#define WKT_SFSQL 0x02
-//#define WKT_EXTENDED 0x04
-
-typedef uint16_t lwflags_t;
-
-
-
-typedef struct {
-    double afac, bfac, cfac, dfac, efac, ffac, gfac, hfac, ifac, xoff, yoff, zoff;
-} AFFINE;
-
-
-
-typedef struct
-{
-    double xmin, ymin, zmin;
-    double xmax, ymax, zmax;
-    int32_t srid;
-}
-BOX3D;
-
-/******************************************************************
-* GBOX structure.
-* We include the flags (information about dimensionality),
-* so we don't have to constantly pass them
-* into functions that use the GBOX.
-*/
-typedef struct
-{
-    lwflags_t flags;
-    double xmin;
-    double xmax;
-    double ymin;
-    double ymax;
-    double zmin;
-    double zmax;
-    double mmin;
-    double mmax;
-} GBOX;
-
-
-/******************************************************************
-* SPHEROID
-*
-*  Standard definition of an ellipsoid (what wkt calls a spheroid)
-*    f = (a-b)/a
-*    e_sq = (a*a - b*b)/(a*a)
-*    b = a - fa
-*/
-typedef struct
-{
-    double  a;  
-    double  b;  
-    double  f;  
-    double  e;  
-    double  e_sq;   
-    double  radius;  
-    char    name[20];  
-}
-SPHEROID;
-
-/******************************************************************
-* POINT2D, POINT3D, POINT3DM, POINT4D
-*/
-typedef struct
-{
-    double x, y;
-}
-POINT2D;
-
-typedef struct
-{
-    double x, y, z;
-}
-POINT3DZ;
-
-typedef struct
-{
-    double x, y, z;
-}
-POINT3D;
-
-typedef struct
-{
-    double x, y, m;
-}
-POINT3DM;
-
-typedef struct
-{
-    double x, y, z, m;
-}
-POINT4D;
-
-/******************************************************************
-*  POINTARRAY
-*  Point array abstracts a lot of the complexity of points and point lists.
-*  It handles 2d/3d translation
-*    (2d points converted to 3d will have z=0 or NaN)
-*  DO NOT MIX 2D and 3D POINTS! EVERYTHING* is either one or the other
-*/
-typedef struct
-{
-    uint32_t npoints;   
-    uint32_t maxpoints; 
-
-    
-    lwflags_t flags;
-
-    
-    uint8_t *serialized_pointlist;
-}
-POINTARRAY;
-
-/******************************************************************
-* GSERIALIZED
-*/
-
-typedef struct
-{
-    uint32_t size; 
-    uint8_t srid[3]; 
-    uint8_t gflags; 
-    uint8_t data[1]; 
-} GSERIALIZED;
-
-/******************************************************************
-* LWGEOM (any geometry type)
-*
-* Abstract type, note that 'type', 'bbox' and 'srid' are available in
-* all geometry variants.
-*/
-typedef struct
-{
-    GBOX *bbox;
-    void *data;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type;
-    char pad[1]; 
-}
-LWGEOM;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    POINTARRAY *point;  
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-}
-LWPOINT; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    POINTARRAY *points; 
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-}
-LWLINE; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    POINTARRAY *points;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type;
-    char pad[1]; 
-}
-LWTRIANGLE;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    POINTARRAY *points; 
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-}
-LWCIRCSTRING; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    POINTARRAY **rings; 
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t nrings;   
-    uint32_t maxrings; 
-}
-LWPOLY; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWPOINT **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWMPOINT;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWLINE **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWMLINE;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWPOLY **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWMPOLY;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWGEOM **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWCOLLECTION;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWGEOM **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWCOMPOUND; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWGEOM **rings;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t nrings;    
-    uint32_t maxrings;  
-}
-LWCURVEPOLY; 
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWGEOM **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWMCURVE;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWGEOM **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWMSURFACE;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWPOLY **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWPSURFACE;
-
-
-typedef struct
-{
-    GBOX *bbox;
-    LWTRIANGLE **geoms;
-    int32_t srid;
-    lwflags_t flags;
-    uint8_t type; 
-    char pad[1]; 
-    uint32_t ngeoms;   
-    uint32_t maxgeoms; 
-}
-LWTIN;
-
-extern LWPOINT *lwpoint_make(int32_t srid, int hasz, int hasm, const POINT4D *p);
-
-extern LWGEOM *lwgeom_from_gserialized(const GSERIALIZED *g);
-extern GSERIALIZED *gserialized_from_lwgeom(LWGEOM *geom, size_t *size);
-
-
-
-extern int32_t lwgeom_get_srid(const LWGEOM *geom);
-
-extern double lwpoint_get_x(const LWPOINT *point);
-extern double lwpoint_get_y(const LWPOINT *point);
-extern double lwpoint_get_z(const LWPOINT *point);
-extern double lwpoint_get_m(const LWPOINT *point);
-
-extern int lwgeom_has_z(const LWGEOM *geom);
-extern int lwgeom_has_m(const LWGEOM *geom);
-
-//#endif              
-
-
-/*****************************************************************************
- * Toolchain dependent definitions
- *****************************************************************************/
-
-//#ifdef _MSC_VER
-/*
- * Under MSVC, functions exported by a loadable module must be marked
- * "dllexport".  Other compilers don't need that.
- * Borrowed from PostgreSQL file win32.h
- */
-//#define PGDLLEXPORT __declspec (dllexport)
-/*
- * Avoids warning C4996: 'strdup': The POSIX name for this item is deprecated.
- */
-//#define strdup _strdup
-//#endif
-
-/*****************************************************************************
- * Type definitions
- *****************************************************************************/
-
-/**
- * @brief Align to double
- */
-//#define DOUBLE_PAD(size) ( (size) + ((size) % 8 ? (8 - (size) % 8) : 0 ) )
-
-/**
- * Structure to represent sets of values
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 settype;        
-  uint8 basetype;       
-  int16 flags;          
-  int32 count;          
-  int32 maxcount;       
-  int16 bboxsize;       
-} Set;
-
-/**
- * Structure to represent spans (a.k.a. ranges)
- */
-typedef struct
-{
-  uint8 spantype;       
-  uint8 basetype;       
-  bool lower_inc;       
-  bool upper_inc;       
-  Datum lower;          
-  Datum upper;          
-} Span;
-
-/**
- * Structure to represent span sets
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 spansettype;    
-  uint8 spantype;       
-  uint8 basetype;       
-  char padding;         
-  int32 count;          
-  int32 maxcount;       
-  Span span;            
-  Span elems[1];        
-} SpanSet;
-
-/**
- * Structure to represent temporal boxes
- */
-typedef struct
-{
-  Span period;          
-  Span span;            
-  int16 flags;          
-} TBox;
-
-/**
- * Structure to represent spatiotemporal boxes
- */
-typedef struct
-{
-  Span period;          
-  double xmin;          
-  double xmax;          
-  double ymin;          
-  double ymax;          
-  double zmin;          
-  double zmax;          
-  int32  srid;          
-  int16  flags;         
-} STBox;
-
-/**
- * @brief Enumeration that defines the interpolation types used in
- * MobilityDB.
- */
-typedef enum
-{
-  INTERP_NONE =    0,
-  DISCRETE =       1,
-  STEP =           2,
-  LINEAR =         3,
-} interpType;
-
-/**
- * @brief Enumeration that defines the spatial relationships for which a call
- * to GEOS is made.
- */
-typedef enum
-{
-  INTERSECTS =     0,
-  CONTAINS =       1,
-  TOUCHES =        2,
-} spatialRel;
-
-/**
- * Structure to represent the common structure of temporal values of
- * any temporal subtype
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 temptype;       
-  uint8 subtype;        
-  int16 flags;          
-  
-} Temporal;
-
-/**
- * Structure to represent temporal values of instant subtype
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 temptype;       
-  uint8 subtype;        
-  int16 flags;          
-  TimestampTz t;        
-  Datum value;          /**< Base value for types passed by value,
-                             first 8 bytes of the base value for values
-                             passed by reference. The extra bytes
-                             needed are added upon creation. */
-  
-} TInstant;
-
-/**
- * Structure to represent temporal values of instant set or sequence subtype
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 temptype;       
-  uint8 subtype;        
-  int16 flags;          
-  int32 count;          
-  int32 maxcount;       
-  int16 bboxsize;       
-  char padding[6];      
-  Span period;          /**< Time span (24 bytes). All bounding boxes start
-                             with a period so actually it is also the begining
-                             of the bounding box. The extra bytes needed for
-                             the bounding box are added upon creation. */
-  
-} TSequence;
-
-//#define TSEQUENCE_BBOX_PTR(seq)      ((void *)(&(seq)->period))
-
-/**
- * Structure to represent temporal values of sequence set subtype
- */
-typedef struct
-{
-  int32 vl_len_;        
-  uint8 temptype;       
-  uint8 subtype;        
-  int16 flags;          
-  int32 count;          
-  int32 totalcount;     /**< Total number of TInstant elements in all
-                             composing TSequence elements */
-  int32 maxcount;       
-  int16 bboxsize;       
-  int16 padding;        
-  Span period;          /**< Time span (24 bytes). All bounding boxes start
-                             with a period so actually it is also the begining
-                             of the bounding box. The extra bytes needed for
-                             the bounding box are added upon creation. */
-  
-} TSequenceSet;
-
-//#define TSEQUENCESET_BBOX_PTR(ss)      ((void *)(&(ss)->period))
-
-/**
- * Struct for storing a similarity match
- */
-typedef struct
-{
-  int i;
-  int j;
-} Match;
-
-
-
-/**
- * Structure to represent skiplist elements
- */
-
-#define SKIPLIST_MAXLEVEL 32
-typedef struct
-{
-  void *value;
-  int height;
-  int next[SKIPLIST_MAXLEVEL];
-} SkipListElem;
-
-/**
- * Structure to represent skiplists that keep the current state of an aggregation
- */
-typedef struct
-{
-  int capacity;
-  int next;
-  int length;
-  int *freed;
-  int freecount;
-  int freecap;
-  int tail;
-  void *extra;
-  size_t extrasize;
-  SkipListElem *elems;
-} SkipList;
-
-/*****************************************************************************
- * Initialization of the MEOS library
- *****************************************************************************/
-
-extern void meos_initialize(const char *tz_str);
-extern void meos_finalize(void);
-
-/*****************************************************************************
- * Functions for input/output PostgreSQL time types
- *****************************************************************************/
-
-extern bool bool_in(const char *in_str);
-extern char *bool_out(bool b);
-extern text *cstring2text(const char *cstring);
-extern DateADT pg_date_in(const char *str);
-extern char *pg_date_out(DateADT date);
-extern int pg_interval_cmp(const Interval *interval1, const Interval *interval2);
-extern Interval *pg_interval_in(const char *str, int32 typmod);
-extern Interval *pg_interval_make(int32 years, int32 months, int32 weeks, int32 days, int32 hours, int32 mins, double secs);
-extern Interval *pg_interval_mul(const Interval *span, double factor);
-extern char *pg_interval_out(const Interval *span);
-extern Interval *pg_interval_pl(const Interval *span1, const Interval *span2);
-extern TimeADT pg_time_in(const char *str, int32 typmod);
-extern char *pg_time_out(TimeADT time);
-extern Timestamp pg_timestamp_in(const char *str, int32 typmod);
-extern Interval *pg_timestamp_mi(TimestampTz dt1, TimestampTz dt2);
-extern TimestampTz pg_timestamp_mi_interval(TimestampTz timestamp, const Interval *span);
-extern char *pg_timestamp_out(Timestamp dt);
-extern TimestampTz pg_timestamp_pl_interval(TimestampTz timestamp, const Interval *span);
-extern TimestampTz pg_timestamptz_in(const char *str, int32 typmod);
-extern char *pg_timestamptz_out(TimestampTz dt);
-extern char *text2cstring(const text *textptr);
-
-/*****************************************************************************
- * Functions for input/output and manipulation of PostGIS types
- *****************************************************************************/
-
-extern bytea *gserialized_as_ewkb(const GSERIALIZED *geom, char *type);
-extern char *gserialized_as_ewkt(const GSERIALIZED *geom, int precision);
-extern char *gserialized_as_geojson(const GSERIALIZED *geom, int option, int precision, char *srs);
-extern char *gserialized_as_hexewkb(const GSERIALIZED *geom, const char *type);
-extern char *gserialized_as_text(const GSERIALIZED *geom, int precision);
-extern GSERIALIZED *gserialized_from_ewkb(const bytea *bytea_wkb, int32 srid);
-extern GSERIALIZED *gserialized_from_geojson(const char *geojson);
-extern GSERIALIZED *gserialized_from_hexewkb(const char *wkt);
-extern GSERIALIZED *gserialized_from_text(char *wkt, int srid);
-extern GSERIALIZED *gserialized_in(char *input, int32 geom_typmod);
-extern char *gserialized_out(const GSERIALIZED *geom);
-extern bool pgis_gserialized_same(const GSERIALIZED *geom1, const GSERIALIZED *geom2);
-
-/*****************************************************************************
- * Functions for set and span types
- *****************************************************************************/
-
-
-
-extern Set *bigintset_in(const char *str);
-extern char *bigintset_out(const Set *set);
-extern Span *bigintspan_in(const char *str);
-extern char *bigintspan_out(const Span *s);
-extern SpanSet *bigintspanset_in(const char *str);
-extern char *bigintspanset_out(const SpanSet *ss);
-extern Set *floatset_in(const char *str);
-extern char *floatset_out(const Set *set, int maxdd);
-extern Span *floatspan_in(const char *str);
-extern char *floatspan_out(const Span *s, int maxdd);
-extern SpanSet *floatspanset_in(const char *str);
-extern char *floatspanset_out(const SpanSet *ss, int maxdd);
-extern Set *geogset_in(const char *str);
-extern char *geogset_out(const Set *set, int maxdd);
-extern Set *geomset_in(const char *str);
-extern char *geomset_out(const Set *set, int maxdd);
-extern char *geoset_as_ewkt(const Set *set, int maxdd);
-extern char *geoset_as_text(const Set *set, int maxdd);
-extern Set *intset_in(const char *str);
-extern char *intset_out(const Set *set);
-extern Span *intspan_in(const char *str);
-extern char *intspan_out(const Span *s);
-extern SpanSet *intspanset_in(const char *str);
-extern char *intspanset_out(const SpanSet *ss);
-extern Span *period_in(const char *str);
-extern char *period_out(const Span *s);
-extern SpanSet *periodset_in(const char *str);
-extern char *periodset_out(const SpanSet *ss);
-extern char *set_as_hexwkb(const Set *s, uint8_t variant, size_t *size_out);
-extern uint8_t *set_as_wkb(const Set *s, uint8_t variant, size_t *size_out);
-extern Set *set_from_hexwkb(const char *hexwkb);
-extern Set *set_from_wkb(const uint8_t *wkb, size_t size);
-extern char *set_out(const Set *s, int maxdd);
-extern uint8_t *span_as_wkb(const Span *s, uint8_t variant, size_t *size_out);
-extern char *span_as_hexwkb(const Span *s, uint8_t variant, size_t *size_out);
-extern Span *span_from_hexwkb(const char *hexwkb);
-extern Span *span_from_wkb(const uint8_t *wkb, size_t size);
-extern char *span_out(const Span *s, int maxdd);
-extern uint8_t *spanset_as_wkb(const SpanSet *ss, uint8_t variant, size_t *size_out);
-extern char *spanset_as_hexwkb(const SpanSet *ss, uint8_t variant, size_t *size_out);
-extern SpanSet *spanset_from_hexwkb(const char *hexwkb);
-extern SpanSet *spanset_from_wkb(const uint8_t *wkb, size_t size);
-extern char *spanset_out(const SpanSet *ss, int maxdd);
-extern Set *textset_in(const char *str);
-extern char *textset_out(const Set *set);
-extern Set *timestampset_in(const char *str);
-extern char *timestampset_out(const Set *set);
-
-
-
-
-
-extern Set *bigintset_make(const int64 *values, int count);
-extern Span *bigintspan_make(int64 lower, int64 upper, bool lower_inc, bool upper_inc);
-extern Set *floatset_make(const double *values, int count);
-extern Span *floatspan_make(double lower, double upper, bool lower_inc, bool upper_inc);
-extern Set *geogset_make(const GSERIALIZED **values, int count);
-extern Set *geomset_make(const GSERIALIZED **values, int count);
-extern Set *intset_make(const int *values, int count);
-extern Span *intspan_make(int lower, int upper, bool lower_inc, bool upper_inc);
-extern Span *period_make(TimestampTz lower, TimestampTz upper, bool lower_inc, bool upper_inc);
-extern Set *set_copy(const Set *s);
-extern Span *span_copy(const Span *s);
-extern SpanSet *spanset_copy(const SpanSet *ps);
-extern SpanSet *spanset_make(Span *spans, int count, bool normalize);
-extern SpanSet *spanset_make_exp(Span *spans, int count, int maxcount, bool normalize, bool ordered);
-extern SpanSet *spanset_make_free(Span *spans, int count, bool normalize);
-extern Set *textset_make(const text **values, int count);
-extern Set *timestampset_make(const TimestampTz *values, int count);
-
-
-
-
-
-extern Set *bigint_to_bigintset(int64 i);
-extern Span *bigint_to_bigintspan(int i);
-extern SpanSet *bigint_to_bigintspanset(int i);
-extern Set *float_to_floatset(double d);
-extern Span *float_to_floatspan(double d);
-extern SpanSet *float_to_floatspanset(double d);
-extern Set *int_to_intset(int i);
-extern Span *int_to_intspan(int i);
-extern SpanSet *int_to_intspanset(int i);
-extern SpanSet *set_to_spanset(const Set *s);
-extern SpanSet *span_to_spanset(const Span *s);
-extern Span *timestamp_to_period(TimestampTz t);
-extern SpanSet *timestamp_to_periodset(TimestampTz t);
-extern Set *timestamp_to_tstzset(TimestampTz t);
-
-
-
-
-
-extern int64 bigintset_end_value(const Set *s);
-extern int64 bigintset_start_value(const Set *s);
-extern bool bigintset_value_n(const Set *s, int n, int64 *result);
-extern int64 *bigintset_values(const Set *s);
-extern int bigintspan_lower(const Span *s);
-extern int bigintspan_upper(const Span *s);
-extern int bigintspanset_lower(const SpanSet *ss);
-extern int bigintspanset_upper(const SpanSet *ss);
-extern double floatset_end_value(const Set *s);
-extern double floatset_start_value(const Set *s);
-extern bool floatset_value_n(const Set *s, int n, double *result);
-extern double *floatset_values(const Set *s);
-extern double floatspan_lower(const Span *s);
-extern double floatspan_upper(const Span *s);
-extern double floatspanset_lower(const SpanSet *ss);
-extern double floatspanset_upper(const SpanSet *ss);
-extern int geoset_srid(const Set *set);
-extern int intset_end_value(const Set *s);
-extern int intset_start_value(const Set *s);
-extern bool intset_value_n(const Set *s, int n, int *result);
-extern int *intset_values(const Set *s);
-extern int intspan_lower(const Span *s);
-extern int intspan_upper(const Span *s);
-extern int intspanset_lower(const SpanSet *ss);
-extern int intspanset_upper(const SpanSet *ss);
-extern Interval *period_duration(const Span *s);
-extern TimestampTz period_lower(const Span *p);
-extern TimestampTz period_upper(const Span *p);
-extern Interval *periodset_duration(const SpanSet *ps, bool boundspan);
-extern TimestampTz periodset_end_timestamp(const SpanSet *ps);
-extern TimestampTz periodset_lower(const SpanSet *ps);
-extern int periodset_num_timestamps(const SpanSet *ps);
-extern TimestampTz periodset_start_timestamp(const SpanSet *ps);
-extern bool periodset_timestamp_n(const SpanSet *ps, int n, TimestampTz *result);
-extern TimestampTz *periodset_timestamps(const SpanSet *ps, int *count);
-extern TimestampTz periodset_upper(const SpanSet *ps);
-extern uint32 set_hash(const Set *s);
-extern uint64 set_hash_extended(const Set *s, uint64 seed);
-extern int set_mem_size(const Set *s);
-extern int set_num_values(const Set *s);
-extern Span *set_span(const Set *s);
-extern uint32 span_hash(const Span *s);
-extern uint64 span_hash_extended(const Span *s, uint64 seed);
-extern bool span_lower_inc(const Span *s);
-extern bool span_upper_inc(const Span *s);
-extern double span_width(const Span *s);
-extern Span *spanset_end_span(const SpanSet *ss);
-extern uint32 spanset_hash(const SpanSet *ps);
-extern uint64 spanset_hash_extended(const SpanSet *ps, uint64 seed);
-extern bool spanset_lower_inc(const SpanSet *ss);
-extern int spanset_mem_size(const SpanSet *ss);
-extern int spanset_num_spans(const SpanSet *ss);
-extern Span *spanset_span(const SpanSet *ss);
-extern Span *spanset_span_n(const SpanSet *ss, int i);
-extern const Span **spanset_spans(const SpanSet *ss);
-extern Span *spanset_start_span(const SpanSet *ss);
-extern bool spanset_upper_inc(const SpanSet *ss);
-extern double spanset_width(const SpanSet *ss);
-extern STBox *spatialset_stbox(const Set *s);
-extern TimestampTz timestampset_end_timestamp(const Set *ts);
-extern TimestampTz timestampset_start_timestamp(const Set *ts);
-extern bool timestampset_timestamp_n(const Set *ts, int n, TimestampTz *result);
-extern TimestampTz *timestampset_values(const Set *ts);
-
-
-
-
-
-extern void floatspan_set_intspan(const Span *s1, Span *s2);
-extern void intspan_set_floatspan(const Span *s1, Span *s2);
-extern void numspan_set_floatspan(const Span *s1, Span *s2);
-extern Span *period_tprecision(const Span *s, const Interval *duration, TimestampTz torigin);
-extern SpanSet *periodset_tprecision(const SpanSet *ss, const Interval *duration, TimestampTz torigin);
-extern Span *period_shift_tscale(const Span *p, const Interval *shift, const Interval *duration);
-extern SpanSet *periodset_shift_tscale(const SpanSet *ps, const Interval *shift, const Interval *duration);
-extern Set *set_shift(const Set *s, Datum shift);
-extern void span_expand(const Span *s1, Span *s2);
-extern TimestampTz timestamp_tprecision(TimestampTz t, const Interval *duration, TimestampTz torigin);
-extern Set *timestampset_shift_tscale(const Set *ts, const Interval *shift, const Interval *duration);
-
-/*****************************************************************************
- * Bounding box functions for set and span types
- *****************************************************************************/
-
-
-
-extern bool adjacent_bigintspan_bigint(const Span *s, int64 i);
-extern bool adjacent_bigintspanset_bigint(const SpanSet *ss, int64 i);
-extern bool adjacent_floatspan_float(const Span *s, double d);
-extern bool adjacent_intspan_int(const Span *s, int i);
-extern bool adjacent_period_timestamp(const Span *p, TimestampTz t);
-extern bool adjacent_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern bool adjacent_span_span(const Span *s1, const Span *s2);
-extern bool adjacent_spanset_span(const SpanSet *ss, const Span *s);
-extern bool adjacent_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool contained_bigint_bigintset(int64 i, const Set *s);
-extern bool contained_bigint_bigintspan(int64 i, const Span *s);
-extern bool contained_bigint_bigintspanset(int64 i, const SpanSet *ss);
-extern bool contained_float_floatset(double d, const Set *s);
-extern bool contained_float_floatspan(double d, const Span *s);
-extern bool contained_float_floatspanset(double d, const SpanSet *ss);
-extern bool contained_int_intset(int i, const Set *s);
-extern bool contained_int_intspanset (int i, const SpanSet *ss);
-extern bool contained_int_intspan(int i, const Span *s);
-extern bool contained_set_set(const Set *s1, const Set *s2);
-extern bool contained_span_span(const Span *s1, const Span *s2);
-extern bool contained_span_spanset(const Span *s, const SpanSet *ss);
-extern bool contained_spanset_span(const SpanSet *ss, const Span *s);
-extern bool contained_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool contained_timestamp_period(TimestampTz t, const Span *p);
-extern bool contained_timestamp_timestampset(TimestampTz t, const Set *ts);
-extern bool contains_floatspan_float(const Span *s, double d);
-extern bool contains_floatspanset_float(const SpanSet *ss, double d);
-extern bool contains_intspan_int(const Span *s, int i);
-extern bool contains_set_set(const Set *s1, const Set *s2);
-extern bool contains_period_timestamp(const Span *p, TimestampTz t);
-extern bool contains_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern bool contains_span_span(const Span *s1, const Span *s2);
-extern bool contains_span_spanset(const Span *s, const SpanSet *ss);
-extern bool contains_spanset_span(const SpanSet *ss, const Span *s);
-extern bool contains_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool contains_timestampset_timestamp(const Set *ts, TimestampTz t);
-extern bool overlaps_set_set(const Set *s1, const Set *s2);
-extern bool overlaps_span_span(const Span *s1, const Span *s2);
-extern bool overlaps_spanset_span(const SpanSet *ss, const Span *s);
-extern bool overlaps_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-
-
-
-
-
-extern bool after_timestamp_timestampset(TimestampTz t, const Set *ts);
-extern bool before_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern bool before_timestamp_timestampset(TimestampTz t, const Set *ts);
-extern bool left_float_floatspan(double d, const Span *s);
-extern bool left_floatspan_float(const Span *s, double d);
-extern bool left_int_intspan(int i, const Span *s);
-extern bool left_intspan_int(const Span *s, int i);
-extern bool left_set_set(const Set *s1, const Set *s2);
-extern bool left_span_span(const Span *s1, const Span *s2);
-extern bool left_span_spanset(const Span *s, const SpanSet *ss);
-extern bool left_spanset_span(const SpanSet *ss, const Span *s);
-extern bool left_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool overafter_period_timestamp(const Span *p, TimestampTz t);
-extern bool overafter_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern bool overafter_timestamp_period(TimestampTz t, const Span *p);
-extern bool overafter_timestamp_periodset(TimestampTz t, const SpanSet *ps);
-extern bool overafter_timestamp_timestampset(TimestampTz t, const Set *ts);
-extern bool overbefore_period_timestamp(const Span *p, TimestampTz t);
-extern bool overbefore_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern bool overbefore_timestamp_period(TimestampTz t, const Span *p);
-extern bool overbefore_timestamp_periodset(TimestampTz t, const SpanSet *ps);
-extern bool overbefore_timestamp_timestampset(TimestampTz t, const Set *ts);
-extern bool overleft_float_floatspan(double d, const Span *s);
-extern bool overleft_floatspan_float(const Span *s, double d);
-extern bool overleft_int_intspan(int i, const Span *s);
-extern bool overleft_intspan_int(const Span *s, int i);
-extern bool overleft_set_set(const Set *s1, const Set *s2);
-extern bool overleft_span_span(const Span *s1, const Span *s2);
-extern bool overleft_span_spanset(const Span *s, const SpanSet *ss);
-extern bool overleft_spanset_span(const SpanSet *ss, const Span *s);
-extern bool overleft_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool overright_float_floatspan(double d, const Span *s);
-extern bool overright_floatspan_float(const Span *s, double d);
-extern bool overright_int_intspan(int i, const Span *s);
-extern bool overright_intspan_int(const Span *s, int i);
-extern bool overright_set_set(const Set *s1, const Set *s2);
-extern bool overright_span_span(const Span *s1, const Span *s2);
-extern bool overright_span_spanset(const Span *s, const SpanSet *ss);
-extern bool overright_spanset_span(const SpanSet *ss, const Span *s);
-extern bool overright_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool right_float_floatspan(double d, const Span *s);
-extern bool right_floatspan_float(const Span *s, double d);
-extern bool right_int_intspan(int i, const Span *s);
-extern bool right_intspan_int(const Span *s, int i);
-extern bool right_set_set(const Set *s1, const Set *s2);
-extern bool right_span_span(const Span *s1, const Span *s2);
-extern bool right_span_spanset(const Span *s, const SpanSet *ss);
-extern bool right_spanset_span(const SpanSet *ss, const Span *s);
-extern bool right_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-
-
-
-
-
-extern void bbox_union_span_span(const Span *s1, const Span *s2, Span *result);
-extern Set *intersection_set_set(const Set *s1, const Set *s2);
-extern bool intersection_period_timestamp(const Span *p, TimestampTz t, TimestampTz *result);
-extern bool intersection_periodset_timestamp(const SpanSet *ps, TimestampTz t, TimestampTz *result);
-extern Span *intersection_span_span(const Span *s1, const Span *s2);
-extern SpanSet *intersection_spanset_span(const SpanSet *ss, const Span *s);
-extern SpanSet *intersection_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool intersection_timestampset_timestamp(const Set *ts, const TimestampTz t, TimestampTz *result);
-extern Set *minus_set_set(const Set *s1, const Set *s2);
-extern SpanSet *minus_period_timestamp(const Span *p, TimestampTz t);
-extern SpanSet *minus_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern SpanSet *minus_span_span(const Span *s1, const Span *s2);
-extern SpanSet *minus_span_spanset(const Span *s, const SpanSet *ss);
-extern SpanSet *minus_spanset_span(const SpanSet *ss, const Span *s);
-extern SpanSet *minus_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern bool minus_timestamp_period(TimestampTz t, const Span *p, TimestampTz *result);
-extern bool minus_timestamp_periodset(TimestampTz t, const SpanSet *ps, TimestampTz *result);
-extern Set *minus_timestampset_timestamp(const Set *ts, TimestampTz t);
-extern Set *union_set_set(const Set *s1, const Set *s2);
-extern SpanSet *union_period_timestamp(const Span *p, TimestampTz t);
-extern SpanSet *union_periodset_timestamp(SpanSet *ps, TimestampTz t);
-extern SpanSet *union_span_span(const Span *s1, const Span *s2);
-extern SpanSet *union_spanset_span(const SpanSet *ss, const Span *s);
-extern SpanSet *union_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern Set *union_timestampset_timestamp(const Set *ts, const TimestampTz t);
-
-
-
-
-
-extern double distance_floatspan_float(const Span *s, double d);
-extern double distance_intspan_int(const Span *s, int i);
-extern double distance_set_set(const Set *s1, const Set *s2);
-extern double distance_period_timestamp(const Span *p, TimestampTz t);
-extern double distance_periodset_timestamp(const SpanSet *ps, TimestampTz t);
-extern double distance_span_span(const Span *s1, const Span *s2);
-extern double distance_spanset_span(const SpanSet *ss, const Span *s);
-extern double distance_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
-extern double distance_timestampset_timestamp(const Set *ts, TimestampTz t);
-
-
-
-
-
-extern Span *bigint_extent_transfn(Span *s, int64 i);
-extern Set *bigint_union_transfn(Set *state, int64 i);
-extern Span *float_extent_transfn(Span *s, double d);
-extern Set *float_union_transfn(Set *state, double d);
-extern Span *int_extent_transfn(Span *s, int i);
-extern Set *int_union_transfn(Set *state, int i);
-extern SkipList *period_tcount_transfn(SkipList *state, const Span *p);
-extern SkipList *periodset_tcount_transfn(SkipList *state, const SpanSet *ps);
-extern Span *set_extent_transfn(Span *span, const Set *set);
-extern Set *set_union_finalfn(Set *state);
-extern Set *set_union_transfn(Set *state, Set *set);
-extern Span *span_extent_transfn(Span *s1, const Span *s2);
-extern SpanSet *span_union_transfn(SpanSet *state, const Span *span);
-extern Span *spanset_extent_transfn(Span *s, const SpanSet *ss);
-extern SpanSet *spanset_union_finalfn(SpanSet *state);
-extern SpanSet *spanset_union_transfn(SpanSet *state, const SpanSet *ss);
-extern Set *text_union_transfn(Set *state, const text *txt);
-extern Span *timestamp_extent_transfn(Span *p, TimestampTz t);
-extern SkipList *timestamp_tcount_transfn(SkipList *state, TimestampTz t);
-extern Set *timestamp_union_transfn(Set *state, TimestampTz t);
-extern SkipList *timestampset_tcount_transfn(SkipList *state, const Set *ts);
-
-
-
-
-
-extern int set_cmp(const Set *s1, const Set *s2);
-extern bool set_eq(const Set *s1, const Set *s2);
-extern bool set_ge(const Set *s1, const Set *s2);
-extern bool set_gt(const Set *s1, const Set *s2);
-extern bool set_le(const Set *s1, const Set *s2);
-extern bool set_lt(const Set *s1, const Set *s2);
-extern bool set_ne(const Set *s1, const Set *s2);
-extern int span_cmp(const Span *s1, const Span *s2);
-extern bool span_eq(const Span *s1, const Span *s2);
-extern bool span_ge(const Span *s1, const Span *s2);
-extern bool span_gt(const Span *s1, const Span *s2);
-extern bool span_le(const Span *s1, const Span *s2);
-extern bool span_lt(const Span *s1, const Span *s2);
-extern bool span_ne(const Span *s1, const Span *s2);
-extern int spanset_cmp(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_eq(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_ge(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_gt(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_le(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_lt(const SpanSet *ss1, const SpanSet *ss2);
-extern bool spanset_ne(const SpanSet *ss1, const SpanSet *ss2);
-
-/******************************************************************************
- * Functions for box types
- *****************************************************************************/
-
-
-
-extern TBox *tbox_in(const char *str);
-extern char *tbox_out(const TBox *box, int maxdd);
-extern TBox *tbox_from_wkb(const uint8_t *wkb, size_t size);
-extern TBox *tbox_from_hexwkb(const char *hexwkb);
-extern STBox *stbox_from_wkb(const uint8_t *wkb, size_t size);
-extern STBox *stbox_from_hexwkb(const char *hexwkb);
-extern uint8_t *tbox_as_wkb(const TBox *box, uint8_t variant, size_t *size_out);
-extern char *tbox_as_hexwkb(const TBox *box, uint8_t variant, size_t *size);
-extern uint8_t *stbox_as_wkb(const STBox *box, uint8_t variant, size_t *size_out);
-extern char *stbox_as_hexwkb(const STBox *box, uint8_t variant, size_t *size);
-extern STBox *stbox_in(const char *str);
-extern char *stbox_out(const STBox *box, int maxdd);
-
-
-
-
-
-extern TBox *tbox_make(const Span *s, const Span *p);
-extern void tbox_set(const Span *s, const Span *p, TBox *box);
-extern TBox *tbox_copy(const TBox *box);
-extern STBox * stbox_make(bool hasx, bool hasz, bool geodetic, int32 srid,
-  double xmin, double xmax, double ymin, double ymax, double zmin, double zmax, const Span *p);
-extern void stbox_set(bool hasx, bool hasz, bool geodetic, int32 srid, double xmin, double xmax,
-  double ymin, double ymax, double zmin, double zmax, const Span *p, STBox *box);
-extern STBox *stbox_copy(const STBox *box);
-
-
-
-
-
-extern TBox *int_to_tbox(int i);
-extern TBox *float_to_tbox(double d);
-extern TBox *timestamp_to_tbox(TimestampTz t);
-extern TBox *timestampset_to_tbox(const Set *ss);
-extern TBox *period_to_tbox(const Span *p);
-extern TBox *periodset_to_tbox(const SpanSet *ps);
-extern TBox *int_timestamp_to_tbox(int i, TimestampTz t);
-extern TBox *float_period_to_tbox(double d, const Span *p);
-extern TBox *float_timestamp_to_tbox(double d, TimestampTz t);
-extern STBox *geo_period_to_stbox(const GSERIALIZED *gs, const Span *p);
-extern STBox *geo_timestamp_to_stbox(const GSERIALIZED *gs, TimestampTz t);
-extern STBox *geo_to_stbox(const GSERIALIZED *gs);
-extern TBox *int_period_to_tbox(int i, const Span *p);
-extern TBox *numspan_to_tbox(const Span *s);
-extern TBox *span_timestamp_to_tbox(const Span *span, TimestampTz t);
-extern TBox *span_period_to_tbox(const Span *span, const Span *p);
-extern Span *tbox_to_floatspan(const TBox *box);
-extern Span *tbox_to_period(const TBox *box);
-extern Span *stbox_to_period(const STBox *box);
-extern TBox *tnumber_to_tbox(const Temporal *temp);
-extern GSERIALIZED *stbox_to_geo(const STBox *box);
-extern STBox *tpoint_to_stbox(const Temporal *temp);
-extern STBox *timestamp_to_stbox(TimestampTz t);
-extern STBox *timestampset_to_stbox(const Set *ts);
-extern STBox *period_to_stbox(const Span *p);
-extern STBox *periodset_to_stbox(const SpanSet *ps);
-
-
-
-
-
-extern bool tbox_hasx(const TBox *box);
-extern bool tbox_hast(const TBox *box);
-extern bool tbox_xmin(const TBox *box, double *result);
-extern bool tbox_xmax(const TBox *box, double *result);
-extern bool tbox_tmin(const TBox *box, TimestampTz *result);
-extern bool tbox_tmax(const TBox *box, TimestampTz *result);
-extern bool stbox_hasx(const STBox *box);
-extern bool stbox_hasz(const STBox *box);
-extern bool stbox_hast(const STBox *box);
-extern bool stbox_isgeodetic(const STBox *box);
-extern bool stbox_xmin(const STBox *box, double *result);
-extern bool stbox_xmax(const STBox *box, double *result);
-extern bool stbox_ymin(const STBox *box, double *result);
-extern bool stbox_ymax(const STBox *box, double *result);
-extern bool stbox_zmin(const STBox *box, double *result);
-extern bool stbox_zmax(const STBox *box, double *result);
-extern bool stbox_tmin(const STBox *box, TimestampTz *result);
-extern bool stbox_tmax(const STBox *box, TimestampTz *result);
-extern int32 stbox_srid(const STBox *box);
-
-
-
-
-
-extern void tbox_expand(const TBox *box1, TBox *box2);
-extern TBox *tbox_expand_value(const TBox *box, const double d);
-extern TBox *tbox_expand_time(const TBox *box, const Interval *interval);
-extern void stbox_expand(const STBox *box1, STBox *box2);
-extern STBox *stbox_set_srid(const STBox *box, int32 srid);
-extern STBox *stbox_get_space(const STBox *box);
-extern STBox *stbox_expand_space(const STBox *box, double d);
-extern STBox *stbox_expand_time(const STBox *box, const Interval *interval);
-
-
-
-
-
-extern bool contains_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool contained_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool overlaps_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool same_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool adjacent_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool contains_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool contained_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overlaps_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool same_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool adjacent_stbox_stbox(const STBox *box1, const STBox *box2);
-
-
-
-
-
-extern bool left_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool overleft_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool right_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool overright_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool before_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool overbefore_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool after_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool overafter_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool left_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overleft_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool right_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overright_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool below_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overbelow_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool above_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overabove_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool front_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overfront_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool back_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overback_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool before_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overbefore_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool after_stbox_stbox(const STBox *box1, const STBox *box2);
-extern bool overafter_stbox_stbox(const STBox *box1, const STBox *box2);
-
-
-
-
-
-extern TBox *union_tbox_tbox(const TBox *box1, const TBox *box2);
-extern bool inter_tbox_tbox(const TBox *box1, const TBox *box2, TBox *result);
-extern TBox *intersection_tbox_tbox(const TBox *box1, const TBox *box2);
-extern STBox *union_stbox_stbox(const STBox *box1, const STBox *box2, bool strict);
-extern bool inter_stbox_stbox(const STBox *box1, const STBox *box2, STBox *result);
-extern STBox *intersection_stbox_stbox(const STBox *box1, const STBox *box2);
-
-
-
-
-
-extern STBox *stbox_quad_split(const STBox *box, int *count);
-
-
-
-
-
-extern bool tbox_eq(const TBox *box1, const TBox *box2);
-extern bool tbox_ne(const TBox *box1, const TBox *box2);
-extern int tbox_cmp(const TBox *box1, const TBox *box2);
-extern bool tbox_lt(const TBox *box1, const TBox *box2);
-extern bool tbox_le(const TBox *box1, const TBox *box2);
-extern bool tbox_ge(const TBox *box1, const TBox *box2);
-extern bool tbox_gt(const TBox *box1, const TBox *box2);
-extern bool stbox_eq(const STBox *box1, const STBox *box2);
-extern bool stbox_ne(const STBox *box1, const STBox *box2);
-extern int stbox_cmp(const STBox *box1, const STBox *box2);
-extern bool stbox_lt(const STBox *box1, const STBox *box2);
-extern bool stbox_le(const STBox *box1, const STBox *box2);
-extern bool stbox_ge(const STBox *box1, const STBox *box2);
-extern bool stbox_gt(const STBox *box1, const STBox *box2);
-
-/*****************************************************************************
- * Functions for temporal types
- *****************************************************************************/
-
-
-
-extern Temporal *tbool_in(const char *str);
-extern char *tbool_out(const Temporal *temp);
-extern char *temporal_as_hexwkb(const Temporal *temp, uint8_t variant, size_t *size_out);
-extern char *temporal_as_mfjson(const Temporal *temp, bool with_bbox, int flags, int precision, char *srs);
-extern uint8_t *temporal_as_wkb(const Temporal *temp, uint8_t variant, size_t *size_out);
-extern Temporal *temporal_from_hexwkb(const char *hexwkb);
-extern Temporal *temporal_from_mfjson(const char *mfjson);
-extern Temporal *temporal_from_wkb(const uint8_t *wkb, size_t size);
-extern Temporal *tfloat_in(const char *str);
-extern char *tfloat_out(const Temporal *temp, int maxdd);
-extern Temporal *tgeogpoint_in(const char *str);
-extern Temporal *tgeompoint_in(const char *str);
-extern Temporal *tint_in(const char *str);
-extern char *tint_out(const Temporal *temp);
-extern char *tpoint_as_ewkt(const Temporal *temp, int maxdd);
-extern char *tpoint_as_text(const Temporal *temp, int maxdd);
-extern char *tpoint_out(const Temporal *temp, int maxdd);
-extern Temporal *ttext_in(const char *str);
-extern char *ttext_out(const Temporal *temp);
-
-
-
-
-
-extern Temporal *tbool_from_base_temp(bool b, const Temporal *temp);
-extern TInstant *tboolinst_make(bool b, TimestampTz t);
-extern TSequence *tboolseq_from_base_period(bool b, const Span *p);
-extern TSequence *tboolseq_from_base_temp(bool b, const TSequence *seq);
-extern TSequence *tboolseq_from_base_timestampset(bool b, const Set *ts);
-extern TSequenceSet *tboolseqset_from_base_periodset(bool b, const SpanSet *ps);
-extern TSequenceSet *tboolseqset_from_base_temp(bool b, const TSequenceSet *ss);
-extern Temporal *temporal_copy(const Temporal *temp);
-extern Temporal *tfloat_from_base_temp(double d, const Temporal *temp);
-extern TInstant *tfloatinst_make(double d, TimestampTz t);
-extern TSequence *tfloatseq_from_base_period(double d, const Span *p, interpType interp);
-extern TSequence *tfloatseq_from_base_temp(double d, const TSequence *seq);
-extern TSequence *tfloatseq_from_base_timestampset(double d, const Set *ts);
-extern TSequenceSet *tfloatseqset_from_base_periodset(double d, const SpanSet *ps, interpType interp);
-extern TSequenceSet *tfloatseqset_from_base_temp(double d, const TSequenceSet *ss);
-extern Temporal *tgeogpoint_from_base_temp(const GSERIALIZED *gs, const Temporal *temp);
-extern TInstant *tgeogpointinst_make(const GSERIALIZED *gs, TimestampTz t);
-extern TSequence *tgeogpointseq_from_base_period(const GSERIALIZED *gs, const Span *p, interpType interp);
-extern TSequence *tgeogpointseq_from_base_temp(const GSERIALIZED *gs, const TSequence *seq);
-extern TSequence *tgeogpointseq_from_base_timestampset(const GSERIALIZED *gs, const Set *ts);
-extern TSequenceSet *tgeogpointseqset_from_base_temp(const GSERIALIZED *gs, const TSequenceSet *ss);
-extern TSequenceSet *tgeogpointseqset_from_base_periodset(const GSERIALIZED *gs, const SpanSet *ps, interpType interp);
-extern Temporal *tgeompoint_from_base_temp(const GSERIALIZED *gs, const Temporal *temp);
-extern TInstant *tgeompointinst_make(const GSERIALIZED *gs, TimestampTz t);
-extern TSequence *tgeompointseq_from_base_period(const GSERIALIZED *gs, const Span *p, interpType interp);
-extern TSequence *tgeompointseq_from_base_temp(const GSERIALIZED *gs, const TSequence *seq);
-extern TSequence *tgeompointseq_from_base_timestampset(const GSERIALIZED *gs, const Set *ts);
-extern TSequenceSet *tgeompointseqset_from_base_periodset(const GSERIALIZED *gs, const SpanSet *ps, interpType interp);
-extern TSequenceSet *tgeompointseqset_from_base_temp(const GSERIALIZED *gs, const TSequenceSet *ss);
-extern Temporal *tint_from_base_temp(int i, const Temporal *temp);
-extern TInstant *tintinst_make(int i, TimestampTz t);
-extern TSequence *tintseq_from_base_period(int i, const Span *p);
-extern TSequence *tintseq_from_base_temp(int i, const TSequence *seq);
-extern TSequence *tintseq_from_base_timestampset(int i, const Set *ts);
-extern TSequenceSet *tintseqset_from_base_periodset(int i, const SpanSet *ps);
-extern TSequenceSet *tintseqset_from_base_temp(int i, const TSequenceSet *ss);
-extern TSequence *tsequence_make(const TInstant **instants, int count, bool lower_inc, bool upper_inc, interpType interp, bool normalize);
-extern TSequence *tsequence_make_exp(const TInstant **instants, int count, int maxcount, bool lower_inc, bool upper_inc, interpType interp, bool normalize);
-extern TSequenceSet *tsequenceset_make(const TSequence **sequences, int count, bool normalize);
-extern TSequenceSet *tsequenceset_make_exp(const TSequence **sequences, int count, int maxcount, bool normalize);
-extern TSequenceSet *tsequenceset_make_gaps(const TInstant **instants, int count, interpType interp, Interval *maxt, double maxdist);
-extern Temporal *ttext_from_base_temp(const text *txt, const Temporal *temp);
-extern TInstant *ttextinst_make(const text *txt, TimestampTz t);
-extern TSequence *ttextseq_from_base_period(const text *txt, const Span *p);
-extern TSequence *ttextseq_from_base_temp(const text *txt, const TSequence *seq);
-extern TSequence *ttextseq_from_base_timestampset(const text *txt, const Set *ts);
-extern TSequenceSet *ttextseqset_from_base_periodset(const text *txt, const SpanSet *ps);
-extern TSequenceSet *ttextseqset_from_base_temp(const text *txt, const TSequenceSet *ss);
-
-
-
-
-
-extern Span *temporal_to_period(const Temporal *temp);
-extern Temporal *tfloat_to_tint(const Temporal *temp);
-extern Temporal *tint_to_tfloat(const Temporal *temp);
-extern Span *tnumber_to_span(const Temporal *temp);
-
-
-
-
-
-extern bool tbool_end_value(const Temporal *temp);
-extern bool tbool_start_value(const Temporal *temp);
-extern bool *tbool_values(const Temporal *temp, int *count);
-extern Interval *temporal_duration(const Temporal *temp, bool boundspan);
-extern const TInstant *temporal_end_instant(const Temporal *temp);
-extern TSequence *temporal_end_sequence(const Temporal *temp);
-extern TimestampTz temporal_end_timestamp(const Temporal *temp);
-extern uint32 temporal_hash(const Temporal *temp);
-extern const TInstant *temporal_instant_n(const Temporal *temp, int n);
-extern const TInstant **temporal_instants(const Temporal *temp, int *count);
-extern char *temporal_interp(const Temporal *temp);
-extern const TInstant *temporal_max_instant(const Temporal *temp);
-extern const TInstant *temporal_min_instant(const Temporal *temp);
-extern int temporal_num_instants(const Temporal *temp);
-extern int temporal_num_sequences(const Temporal *temp);
-extern int temporal_num_timestamps(const Temporal *temp);
-extern TSequence **temporal_segments(const Temporal *temp, int *count);
-extern TSequence *temporal_sequence_n(const Temporal *temp, int i);
-extern TSequence **temporal_sequences(const Temporal *temp, int *count);
-extern const TInstant *temporal_start_instant(const Temporal *temp);
-extern TSequence *temporal_start_sequence(const Temporal *temp);
-extern TimestampTz temporal_start_timestamp(const Temporal *temp);
-extern TSequenceSet *temporal_stops(const Temporal *temp, double maxdist, const Interval *minduration);
-extern char *temporal_subtype(const Temporal *temp);
-extern SpanSet *temporal_time(const Temporal *temp);
-extern bool temporal_timestamp_n(const Temporal *temp, int n, TimestampTz *result);
-extern TimestampTz *temporal_timestamps(const Temporal *temp, int *count);
-extern Datum *temporal_values(const Temporal *temp, int *count);
-extern double tfloat_end_value(const Temporal *temp);
-extern double tfloat_max_value(const Temporal *temp);
-extern double tfloat_min_value(const Temporal *temp);
-extern double tfloat_start_value(const Temporal *temp);
-extern double *tfloat_values(const Temporal *temp, int *count);
-extern int tint_end_value(const Temporal *temp);
-extern int tint_max_value(const Temporal *temp);
-extern int tint_min_value(const Temporal *temp);
-extern int tint_start_value(const Temporal *temp);
-extern int *tint_values(const Temporal *temp, int *count);
-extern SpanSet *tnumber_valuespans(const Temporal *temp);
-extern GSERIALIZED *tpoint_end_value(const Temporal *temp);
-extern GSERIALIZED *tpoint_start_value(const Temporal *temp);
-extern GSERIALIZED **tpoint_values(const Temporal *temp, int *count);
-extern text *ttext_end_value(const Temporal *temp);
-extern text *ttext_max_value(const Temporal *temp);
-extern text *ttext_min_value(const Temporal *temp);
-extern text *ttext_start_value(const Temporal *temp);
-extern text **ttext_values(const Temporal *temp, int *count);
-
-
-
-
-
-extern Temporal *temporal_set_interp(const Temporal *temp, interpType interp);
-extern Temporal *temporal_shift(const Temporal *temp, const Interval *shift);
-extern Temporal *temporal_shift_tscale(const Temporal *temp, const Interval *shift, const Interval *duration);
-extern Temporal *temporal_to_tinstant(const Temporal *temp);
-extern Temporal *temporal_to_tsequence(const Temporal *temp);
-extern Temporal *temporal_to_tsequenceset(const Temporal *temp);
-extern Temporal *temporal_tprecision(const Temporal *temp, const Interval *duration, TimestampTz origin);
-extern Temporal *temporal_tsample(const Temporal *temp, const Interval *duration, TimestampTz origin);
-extern Temporal *temporal_tscale(const Temporal *temp, const Interval *duration);
-
-
-
-
-
-extern Temporal *tbool_at_value(const Temporal *temp, bool b);
-extern Temporal *tbool_minus_value(const Temporal *temp, bool b);
-extern bool tbool_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, bool *value);
-extern Temporal *temporal_at_max(const Temporal *temp);
-extern Temporal *temporal_at_min(const Temporal *temp);
-extern Temporal *temporal_at_period(const Temporal *temp, const Span *p);
-extern Temporal *temporal_at_periodset(const Temporal *temp, const SpanSet *ps);
-extern Temporal *temporal_at_timestamp(const Temporal *temp, TimestampTz t);
-extern Temporal *temporal_at_timestampset(const Temporal *temp, const Set *ts);
-extern Temporal *temporal_at_values(const Temporal *temp, const Set *set);
-extern Temporal *temporal_minus_max(const Temporal *temp);
-extern Temporal *temporal_minus_min(const Temporal *temp);
-extern Temporal *temporal_minus_period(const Temporal *temp, const Span *p);
-extern Temporal *temporal_minus_periodset(const Temporal *temp, const SpanSet *ps);
-extern Temporal *temporal_minus_timestamp(const Temporal *temp, TimestampTz t);
-extern Temporal *temporal_minus_timestampset(const Temporal *temp, const Set *ts);
-extern Temporal *temporal_minus_values(const Temporal *temp, const Set *set);
-extern Temporal *tfloat_at_value(const Temporal *temp, double d);
-extern Temporal *tfloat_minus_value(const Temporal *temp, double d);
-extern bool tfloat_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, double *value);
-extern Temporal *tint_at_value(const Temporal *temp, int i);
-extern Temporal *tint_minus_value(const Temporal *temp, int i);
-extern bool tint_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, int *value);
-extern Temporal *tnumber_at_span(const Temporal *temp, const Span *span);
-extern Temporal *tnumber_at_spanset(const Temporal *temp, const SpanSet *ss);
-extern Temporal *tnumber_at_tbox(const Temporal *temp, const TBox *box);
-extern Temporal *tnumber_minus_span(const Temporal *temp, const Span *span);
-extern Temporal *tnumber_minus_spanset(const Temporal *temp, const SpanSet *ss);
-extern Temporal *tnumber_minus_tbox(const Temporal *temp, const TBox *box);
-extern Temporal *tpoint_at_geom_time(const Temporal *temp, const GSERIALIZED *gs, const Span *zspan, const Span *period);
-extern Temporal *tpoint_at_stbox(const Temporal *temp, const STBox *box, bool border_inc);
-extern Temporal *tpoint_at_value(const Temporal *temp, GSERIALIZED *gs);
-extern Temporal *tpoint_minus_geom_time(const Temporal *temp, const GSERIALIZED *gs, const Span *zspan, const Span *period);
-extern Temporal *tpoint_minus_stbox(const Temporal *temp, const STBox *box, bool border_inc);
-extern Temporal *tpoint_minus_value(const Temporal *temp, GSERIALIZED *gs);
-extern bool tpoint_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, GSERIALIZED **value);
-extern Temporal *ttext_at_value(const Temporal *temp, text *txt);
-extern Temporal *ttext_minus_value(const Temporal *temp, text *txt);
-extern bool ttext_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, text **value);
-
-
-
-
-
-extern Temporal *temporal_append_tinstant(Temporal *temp, const TInstant *inst, double maxdist, Interval *maxt, bool expand);
-extern Temporal *temporal_append_tsequence(Temporal *temp, const TSequence *seq, bool expand);
-extern Temporal *temporal_delete_period(const Temporal *temp, const Span *p, bool connect);
-extern Temporal *temporal_delete_periodset(const Temporal *temp, const SpanSet *ps, bool connect);
-extern Temporal *temporal_delete_timestamp(const Temporal *temp, TimestampTz t, bool connect);
-extern Temporal *temporal_delete_timestampset(const Temporal *temp, const Set *ts, bool connect);
-extern Temporal *temporal_insert(const Temporal *temp1, const Temporal *temp2, bool connect);
-extern Temporal *temporal_merge(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *temporal_merge_array(Temporal **temparr, int count);
-extern Temporal *temporal_update(const Temporal *temp1, const Temporal *temp2, bool connect);
-
-
-
-
-
-extern Temporal *tand_bool_tbool(bool b, const Temporal *temp);
-extern Temporal *tand_tbool_bool(const Temporal *temp, bool b);
-extern Temporal *tand_tbool_tbool(const Temporal *temp1, const Temporal *temp2);
-extern SpanSet *tbool_when_true(const Temporal *temp);
-extern Temporal *tnot_tbool(const Temporal *temp);
-extern Temporal *tor_bool_tbool(bool b, const Temporal *temp);
-extern Temporal *tor_tbool_bool(const Temporal *temp, bool b);
-extern Temporal *tor_tbool_tbool(const Temporal *temp1, const Temporal *temp2);
-
-
-
-
-
-extern Temporal *add_float_tfloat(double d, const Temporal *tnumber);
-extern Temporal *add_int_tint(int i, const Temporal *tnumber);
-extern Temporal *add_tfloat_float(const Temporal *tnumber, double d);
-extern Temporal *add_tint_int(const Temporal *tnumber, int i);
-extern Temporal *add_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
-extern Temporal *div_float_tfloat(double d, const Temporal *tnumber);
-extern Temporal *div_int_tint(int i, const Temporal *tnumber);
-extern Temporal *div_tfloat_float(const Temporal *tnumber, double d);
-extern Temporal *div_tint_int(const Temporal *tnumber, int i);
-extern Temporal *div_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
-extern double float_degrees(double value, bool normalize);
-extern Temporal *mult_float_tfloat(double d, const Temporal *tnumber);
-extern Temporal *mult_int_tint(int i, const Temporal *tnumber);
-extern Temporal *mult_tfloat_float(const Temporal *tnumber, double d);
-extern Temporal *mult_tint_int(const Temporal *tnumber, int i);
-extern Temporal *mult_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
-extern Temporal *sub_float_tfloat(double d, const Temporal *tnumber);
-extern Temporal *sub_int_tint(int i, const Temporal *tnumber);
-extern Temporal *sub_tfloat_float(const Temporal *tnumber, double d);
-extern Temporal *sub_tint_int(const Temporal *tnumber, int i);
-extern Temporal *sub_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
-extern Temporal *tfloat_degrees(const Temporal *temp, bool normalize);
-extern Temporal *tfloat_derivative(const Temporal *temp);
-extern Temporal *tfloat_radians(const Temporal *temp);
-extern Temporal *tnumber_abs(const Temporal *temp);
-extern Temporal *tnumber_angular_difference(const Temporal *temp);
-extern Temporal *tnumber_delta_value(const Temporal *temp);
-
-
-
-
-
-extern Temporal *textcat_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *textcat_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *textcat_ttext_ttext(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *ttext_upper(const Temporal *temp);
-extern Temporal *ttext_lower(const Temporal *temp);
-
-
-
-
-
-extern Temporal *distance_tfloat_float(const Temporal *temp, double d);
-extern Temporal *distance_tint_int(const Temporal *temp, int i);
-extern Temporal *distance_tnumber_tnumber(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *distance_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo);
-extern Temporal *distance_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern double nad_stbox_geo(const STBox *box, const GSERIALIZED *gs);
-extern double nad_stbox_stbox(const STBox *box1, const STBox *box2);
-extern double nad_tbox_tbox(const TBox *box1, const TBox *box2);
-extern double nad_tfloat_float(const Temporal *temp, double d);
-extern double nad_tfloat_tfloat(const Temporal *temp1, const Temporal *temp2);
-extern int nad_tint_int(const Temporal *temp, int i);
-extern int nad_tint_tint(const Temporal *temp1, const Temporal *temp2);
-extern double nad_tnumber_tbox(const Temporal *temp, const TBox *box);
-extern double nad_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
-extern double nad_tpoint_stbox(const Temporal *temp, const STBox *box);
-extern double nad_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern TInstant *nai_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
-extern TInstant *nai_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern bool shortestline_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, GSERIALIZED **result);
-extern bool shortestline_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, GSERIALIZED **result);
-
-
-
-
-
-extern bool tbool_always_eq(const Temporal *temp, bool b);
-extern bool tbool_ever_eq(const Temporal *temp, bool b);
-extern bool tfloat_always_eq(const Temporal *temp, double d);
-extern bool tfloat_always_le(const Temporal *temp, double d);
-extern bool tfloat_always_lt(const Temporal *temp, double d);
-extern bool tfloat_ever_eq(const Temporal *temp, double d);
-extern bool tfloat_ever_le(const Temporal *temp, double d);
-extern bool tfloat_ever_lt(const Temporal *temp, double d);
-extern bool tgeogpoint_always_eq(const Temporal *temp, GSERIALIZED *gs);;
-extern bool tgeogpoint_ever_eq(const Temporal *temp, GSERIALIZED *gs);;
-extern bool tgeompoint_always_eq(const Temporal *temp, GSERIALIZED *gs);
-extern bool tgeompoint_ever_eq(const Temporal *temp, GSERIALIZED *gs);;
-extern bool tint_always_eq(const Temporal *temp, int i);
-extern bool tint_always_le(const Temporal *temp, int i);
-extern bool tint_always_lt(const Temporal *temp, int i);
-extern bool tint_ever_eq(const Temporal *temp, int i);
-extern bool tint_ever_le(const Temporal *temp, int i);
-extern bool tint_ever_lt(const Temporal *temp, int i);
-extern bool tpoint_always_eq(const Temporal *temp, Datum value);
-extern bool tpoint_ever_eq(const Temporal *temp, Datum value);
-extern bool ttext_always_eq(const Temporal *temp, text *txt);
-extern bool ttext_always_le(const Temporal *temp, text *txt);
-extern bool ttext_always_lt(const Temporal *temp, text *txt);
-extern bool ttext_ever_eq(const Temporal *temp, text *txt);
-extern bool ttext_ever_le(const Temporal *temp, text *txt);
-extern bool ttext_ever_lt(const Temporal *temp, text *txt);
-
-
-
-
-
-extern int temporal_cmp(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_eq(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_ge(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_gt(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_le(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_lt(const Temporal *temp1, const Temporal *temp2);
-extern bool temporal_ne(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *teq_bool_tbool(bool b, const Temporal *temp);
-extern Temporal *teq_float_tfloat(double d, const Temporal *temp);
-extern Temporal *teq_geo_tpoint(const GSERIALIZED *geo, const Temporal *tpoint);
-extern Temporal *teq_int_tint(int i, const Temporal *temp);
-extern Temporal *teq_point_tgeogpoint(const GSERIALIZED *gs, const Temporal *temp);
-extern Temporal *teq_point_tgeompoint(const GSERIALIZED *gs, const Temporal *temp);
-extern Temporal *teq_tbool_bool(const Temporal *temp, bool b);
-extern Temporal *teq_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *teq_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *teq_tfloat_float(const Temporal *temp, double d);
-extern Temporal *teq_tgeogpoint_point(const Temporal *temp, const GSERIALIZED *gs);
-extern Temporal *teq_tgeompoint_point(const Temporal *temp, const GSERIALIZED *gs);
-extern Temporal *teq_tint_int(const Temporal *temp, int i);
-extern Temporal *teq_tpoint_geo(const Temporal *tpoint, const GSERIALIZED *geo);
-extern Temporal *teq_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *tge_float_tfloat(double d, const Temporal *temp);
-extern Temporal *tge_int_tint(int i, const Temporal *temp);
-extern Temporal *tge_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tge_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *tge_tfloat_float(const Temporal *temp, double d);
-extern Temporal *tge_tint_int(const Temporal *temp, int i);
-extern Temporal *tge_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *tgt_float_tfloat(double d, const Temporal *temp);
-extern Temporal *tgt_int_tint(int i, const Temporal *temp);
-extern Temporal *tgt_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tgt_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *tgt_tfloat_float(const Temporal *temp, double d);
-extern Temporal *tgt_tint_int(const Temporal *temp, int i);
-extern Temporal *tgt_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *tle_float_tfloat(double d, const Temporal *temp);
-extern Temporal *tle_int_tint(int i, const Temporal *temp);
-extern Temporal *tle_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tle_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *tle_tfloat_float(const Temporal *temp, double d);
-extern Temporal *tle_tint_int(const Temporal *temp, int i);
-extern Temporal *tle_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *tlt_float_tfloat(double d, const Temporal *temp);
-extern Temporal *tlt_int_tint(int i, const Temporal *temp);
-extern Temporal *tlt_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tlt_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *tlt_tfloat_float(const Temporal *temp, double d);
-extern Temporal *tlt_tint_int(const Temporal *temp, int i);
-extern Temporal *tlt_ttext_text(const Temporal *temp, const text *txt);
-extern Temporal *tne_bool_tbool(bool b, const Temporal *temp);
-extern Temporal *tne_float_tfloat(double d, const Temporal *temp);
-extern Temporal *tne_geo_tpoint(const GSERIALIZED *geo, const Temporal *tpoint);
-extern Temporal *tne_int_tint(int i, const Temporal *temp);
-extern Temporal *tne_point_tgeogpoint(const GSERIALIZED *gs, const Temporal *temp);
-extern Temporal *tne_point_tgeompoint(const GSERIALIZED *gs, const Temporal *temp);
-extern Temporal *tne_tbool_bool(const Temporal *temp, bool b);
-extern Temporal *tne_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tne_text_ttext(const text *txt, const Temporal *temp);
-extern Temporal *tne_tfloat_float(const Temporal *temp, double d);
-extern Temporal *tne_tgeogpoint_point(const Temporal *temp, const GSERIALIZED *gs);
-extern Temporal *tne_tgeompoint_point(const Temporal *temp, const GSERIALIZED *gs);
-extern Temporal *tne_tint_int(const Temporal *temp, int i);
-extern Temporal *tne_tpoint_geo(const Temporal *tpoint, const GSERIALIZED *geo);
-extern Temporal *tne_ttext_text(const Temporal *temp, const text *txt);
-
-/*****************************************************************************
-  Spatial functions for temporal point types
- *****************************************************************************/
-
-
-
-extern bool bearing_point_point(const GSERIALIZED *geo1, const GSERIALIZED *geo2, double *result);
-extern Temporal *bearing_tpoint_point(const Temporal *temp, const GSERIALIZED *gs, bool invert);
-extern Temporal *bearing_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern Temporal *tpoint_angular_difference(const Temporal *temp);
-extern Temporal *tpoint_azimuth(const Temporal *temp);
-extern GSERIALIZED *tpoint_convex_hull(const Temporal *temp);
-extern Temporal *tpoint_cumulative_length(const Temporal *temp);
-extern bool tpoint_direction(const Temporal *temp, double *result);
-extern Temporal *tpoint_get_coord(const Temporal *temp, int coord);
-extern bool tpoint_is_simple(const Temporal *temp);
-extern double tpoint_length(const Temporal *temp);
-extern Temporal *tpoint_speed(const Temporal *temp);
-extern int tpoint_srid(const Temporal *temp);
-extern STBox *tpoint_stboxes(const Temporal *temp, int *count);
-extern GSERIALIZED *tpoint_trajectory(const Temporal *temp);
-
-
-
-
-
-extern STBox *geo_expand_space(const GSERIALIZED *gs, double d);
-extern Temporal *tgeompoint_tgeogpoint(const Temporal *temp, bool oper);
-extern STBox *tpoint_expand_space(const Temporal *temp, double d);
-extern Temporal **tpoint_make_simple(const Temporal *temp, int *count);
-extern Temporal *tpoint_set_srid(const Temporal *temp, int32 srid);
-
-
-
-
-
-extern int econtains_geo_tpoint(const GSERIALIZED *geo, const Temporal *temp);
-extern int edisjoint_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
-extern int edisjoint_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern int edwithin_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, double dist);
-extern int edwithin_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, double dist);
-extern int eintersects_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
-extern int eintersects_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
-extern int etouches_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
-extern Temporal *tcontains_geo_tpoint(const GSERIALIZED *gs, const Temporal *temp, bool restr, bool atvalue);
-extern Temporal *tdisjoint_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo, bool restr, bool atvalue);
-extern Temporal *tdwithin_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, double dist, bool restr, bool atvalue);
-extern Temporal *tdwithin_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, double dist, bool restr, bool atvalue);
-extern Temporal *tintersects_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo, bool restr, bool atvalue);
-extern Temporal *ttouches_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, bool restr, bool atvalue);
-
-
-
-
-
-extern SkipList *tbool_tand_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tbool_tor_transfn(SkipList *state, const Temporal *temp);
-extern Span *temporal_extent_transfn(Span *p, const Temporal *temp);
-extern Temporal *temporal_tagg_finalfn(SkipList *state);
-extern SkipList *temporal_tcount_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tfloat_tmax_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tfloat_tmin_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tfloat_tsum_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tint_tmax_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tint_tmin_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *tint_tsum_transfn(SkipList *state, const Temporal *temp);
-extern TBox *tnumber_extent_transfn(TBox *box, const Temporal *temp);
-extern double tnumber_integral(const Temporal *temp);
-extern Temporal *tnumber_tavg_finalfn(SkipList *state);
-extern SkipList *tnumber_tavg_transfn(SkipList *state, const Temporal *temp);
-extern double tnumber_twavg(const Temporal *temp);
-extern STBox *tpoint_extent_transfn(STBox *box, const Temporal *temp);
-extern Temporal *tpoint_tcentroid_finalfn(SkipList *state);
-extern SkipList *tpoint_tcentroid_transfn(SkipList *state, Temporal *temp);
-extern GSERIALIZED *tpoint_twcentroid(const Temporal *temp);
-extern SkipList *ttext_tmax_transfn(SkipList *state, const Temporal *temp);
-extern SkipList *ttext_tmin_transfn(SkipList *state, const Temporal *temp);
-
-
-
-
-
-extern double float_bucket(double value, double size, double origin);
-extern Span *floatspan_bucket_list(const Span *bounds, double size, double origin, int *newcount);
-extern int int_bucket(int value, int size, int origin);
-extern Span *intspan_bucket_list(const Span *bounds, int size, int origin, int *newcount);
-extern Span *period_bucket_list(const Span *bounds, const Interval *duration, TimestampTz origin, int *newcount);
-extern STBox *stbox_tile_list(const STBox *bounds, double xsize, double ysize, double zsize, const Interval *duration, GSERIALIZED *sorigin, TimestampTz torigin, int **cellcount);
-extern TBox *tbox_tile_list(const TBox *bounds, double xsize, const Interval *duration, double xorigin, TimestampTz torigin, int *rows, int *columns);
-extern Temporal **temporal_time_split(Temporal *temp, Interval *duration, TimestampTz torigin, int *newcount);
-extern Temporal **tfloat_value_split(Temporal *temp, double size, double origin, int *newcount);
-extern Temporal **tfloat_value_time_split(Temporal *temp, double size, double vorigin, Interval *duration, TimestampTz torigin, int *newcount);
-extern TimestampTz timestamptz_bucket(TimestampTz timestamp, const Interval *duration, TimestampTz origin);
-extern Temporal **tint_value_split(Temporal *temp, int size, int origin, int *newcount);
-extern Temporal **tint_value_time_split(Temporal *temp, int size, int vorigin, Interval *duration, TimestampTz torigin, int *newcount);
-
-
-
-
-
-extern double temporal_dyntimewarp_distance(const Temporal *temp1, const Temporal *temp2);
-extern Match *temporal_dyntimewarp_path(const Temporal *temp1, const Temporal *temp2, int *count);
-extern double temporal_frechet_distance(const Temporal *temp1, const Temporal *temp2);
-extern Match *temporal_frechet_path(const Temporal *temp1, const Temporal *temp2, int *count);
-extern double temporal_hausdorff_distance(const Temporal *temp1, const Temporal *temp2);
-
-
-
-
-
-Temporal *geo_to_tpoint(const GSERIALIZED *geo);
-Temporal *temporal_simplify_min_dist(const Temporal *temp, double dist);
-Temporal *temporal_simplify_min_tdelta(const Temporal *temp, const Interval *mint);
-Temporal *temporal_simplify_dp(const Temporal *temp, double eps_dist, bool synchronized);
-Temporal *temporal_simplify_max_dist(const Temporal *temp, double eps_dist, bool synchronized);
-bool tpoint_AsMVTGeom(const Temporal *temp, const STBox *bounds, int32_t extent, int32_t buffer, bool clip_geom, GSERIALIZED **geom, int64 **timesarr, int *count);
-bool tpoint_to_geo_meas(const Temporal *tpoint, const Temporal *measure, bool segmentize, GSERIALIZED **result);
-
-
-
-//#endif
+/*****************************************************************************
+ *
+ * This MobilityDB code is provided under The PostgreSQL License.
+ * Copyright (c) 2016-2023, Université libre de Bruxelles and MobilityDB
+ * contributors
+ *
+ * MobilityDB includes portions of PostGIS version 3 source code released
+ * under the GNU General Public License (GPLv2 or later).
+ * Copyright (c) 2001-2023, PostGIS contributors
+ *
+ * Permission to use, copy, modify, and distribute this software and its
+ * documentation for any purpose, without fee, and without a written
+ * agreement is hereby granted, provided that the above copyright notice and
+ * this paragraph and the following two paragraphs appear in all copies.
+ *
+ * IN NO EVENT SHALL UNIVERSITE LIBRE DE BRUXELLES BE LIABLE TO ANY PARTY FOR
+ * DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING
+ * LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION,
+ * EVEN IF UNIVERSITE LIBRE DE BRUXELLES HAS BEEN ADVISED OF THE POSSIBILITY
+ * OF SUCH DAMAGE.
+ *
+ * UNIVERSITE LIBRE DE BRUXELLES SPECIFICALLY DISCLAIMS ANY WARRANTIES,
+ * INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY
+ * AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON
+ * AN "AS IS" BASIS, AND UNIVERSITE LIBRE DE BRUXELLES HAS NO OBLIGATIONS TO
+ * PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
+ *
+ *****************************************************************************/
+
+/**
+ * @brief API of the Mobility Engine Open Source (MEOS) library.
+ */
+
+//#ifndef __MEOS_H__
+//#define __MEOS_H__
+
+
+//#include <stdbool.h>
+//#include <stdint.h>
+
+//#ifndef POSTGRES_H
+//#define POSTGRES_H
+
+//#define DatumGetPointer(X) ((Pointer) (X))
+
+typedef char *Pointer;
+typedef uintptr_t Datum;
+
+typedef signed char int8;
+typedef signed short int16;
+typedef signed int int32;
+typedef long int int64;
+
+typedef unsigned char uint8;
+typedef unsigned short uint16;
+typedef unsigned int uint32;
+typedef unsigned long int uint64;
+
+typedef int32 DateADT;
+typedef int64 TimeADT;
+typedef int64 Timestamp;
+typedef int64 TimestampTz;
+typedef int64 TimeOffset;
+typedef int32 fsec_t;      
+
+typedef struct
+{
+  TimeOffset time;  
+  int32 day;        
+  int32 month;      
+} Interval;
+
+typedef struct varlena
+{
+  char vl_len_[4];  
+  char vl_dat[];    
+} varlena;
+
+typedef varlena text;
+typedef struct varlena bytea;
+
+//#endif              
+
+
+//#ifndef _LIBLWGEOM_H
+//#define _LIBLWGEOM_H
+
+
+
+/**
+* Macros for manipulating the 'flags' byte. A uint8_t used as follows:
+* VVSRGBMZ
+* Version bit, followed by
+* Validty, Solid, ReadOnly, Geodetic, HasBBox, HasM and HasZ flags.
+*/
+//#define LWFLAG_Z        0x01
+//#define LWFLAG_M        0x02
+//#define LWFLAG_BBOX     0x04
+//#define LWFLAG_GEODETIC 0x08
+//#define LWFLAG_READONLY 0x10
+//#define LWFLAG_SOLID    0x20
+
+//#define FLAGS_GET_Z(flags)         ((flags) & LWFLAG_Z)
+//#define FLAGS_GET_M(flags)        (((flags) & LWFLAG_M)>>1)
+//#define FLAGS_GET_BBOX(flags)     (((flags) & LWFLAG_BBOX)>>2)
+//#define FLAGS_GET_GEODETIC(flags) (((flags) & LWFLAG_GEODETIC)>>3)
+//#define FLAGS_GET_READONLY(flags) (((flags) & LWFLAG_READONLY)>>4)
+//#define FLAGS_GET_SOLID(flags)    (((flags) & LWFLAG_SOLID)>>5)
+
+//#define FLAGS_SET_Z(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_Z) : ((flags) & ~LWFLAG_Z))
+//#define FLAGS_SET_M(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_M) : ((flags) & ~LWFLAG_M))
+//#define FLAGS_SET_BBOX(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_BBOX) : ((flags) & ~LWFLAG_BBOX))
+//#define FLAGS_SET_GEODETIC(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_GEODETIC) : ((flags) & ~LWFLAG_GEODETIC))
+//#define FLAGS_SET_READONLY(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_READONLY) : ((flags) & ~LWFLAG_READONLY))
+//#define FLAGS_SET_SOLID(flags, value) ((flags) = (value) ? ((flags) | LWFLAG_SOLID) : ((flags) & ~LWFLAG_SOLID))
+
+//#define FLAGS_NDIMS(flags) (2 + FLAGS_GET_Z(flags) + FLAGS_GET_M(flags))
+//#define FLAGS_GET_ZM(flags) (FLAGS_GET_M(flags) + FLAGS_GET_Z(flags) * 2)
+//#define FLAGS_NDIMS_BOX(flags) (FLAGS_GET_GEODETIC(flags) ? 3 : FLAGS_NDIMS(flags))
+
+/*
+** Variants available for WKB and WKT output types
+*/
+
+//#define WKB_ISO 0x01
+//#define WKB_SFSQL 0x02
+//#define WKB_EXTENDED 0x04
+//#define WKB_NDR 0x08
+//#define WKB_XDR 0x10
+//#define WKB_HEX 0x20
+//#define WKB_NO_NPOINTS 0x40 
+//#define WKB_NO_SRID 0x80 
+
+//#define WKT_ISO 0x01
+//#define WKT_SFSQL 0x02
+//#define WKT_EXTENDED 0x04
+
+typedef uint16_t lwflags_t;
+
+
+
+typedef struct {
+    double afac, bfac, cfac, dfac, efac, ffac, gfac, hfac, ifac, xoff, yoff, zoff;
+} AFFINE;
+
+
+
+typedef struct
+{
+    double xmin, ymin, zmin;
+    double xmax, ymax, zmax;
+    int32_t srid;
+}
+BOX3D;
+
+/******************************************************************
+* GBOX structure.
+* We include the flags (information about dimensionality),
+* so we don't have to constantly pass them
+* into functions that use the GBOX.
+*/
+typedef struct
+{
+    lwflags_t flags;
+    double xmin;
+    double xmax;
+    double ymin;
+    double ymax;
+    double zmin;
+    double zmax;
+    double mmin;
+    double mmax;
+} GBOX;
+
+
+/******************************************************************
+* SPHEROID
+*
+*  Standard definition of an ellipsoid (what wkt calls a spheroid)
+*    f = (a-b)/a
+*    e_sq = (a*a - b*b)/(a*a)
+*    b = a - fa
+*/
+typedef struct
+{
+    double  a;  
+    double  b;  
+    double  f;  
+    double  e;  
+    double  e_sq;   
+    double  radius;  
+    char    name[20];  
+}
+SPHEROID;
+
+/******************************************************************
+* POINT2D, POINT3D, POINT3DM, POINT4D
+*/
+typedef struct
+{
+    double x, y;
+}
+POINT2D;
+
+typedef struct
+{
+    double x, y, z;
+}
+POINT3DZ;
+
+typedef struct
+{
+    double x, y, z;
+}
+POINT3D;
+
+typedef struct
+{
+    double x, y, m;
+}
+POINT3DM;
+
+typedef struct
+{
+    double x, y, z, m;
+}
+POINT4D;
+
+/******************************************************************
+*  POINTARRAY
+*  Point array abstracts a lot of the complexity of points and point lists.
+*  It handles 2d/3d translation
+*    (2d points converted to 3d will have z=0 or NaN)
+*  DO NOT MIX 2D and 3D POINTS! EVERYTHING* is either one or the other
+*/
+typedef struct
+{
+    uint32_t npoints;   
+    uint32_t maxpoints; 
+
+    
+    lwflags_t flags;
+
+    
+    uint8_t *serialized_pointlist;
+}
+POINTARRAY;
+
+/******************************************************************
+* GSERIALIZED
+*/
+
+typedef struct
+{
+    uint32_t size; 
+    uint8_t srid[3]; 
+    uint8_t gflags; 
+    uint8_t data[1]; 
+} GSERIALIZED;
+
+/******************************************************************
+* LWGEOM (any geometry type)
+*
+* Abstract type, note that 'type', 'bbox' and 'srid' are available in
+* all geometry variants.
+*/
+typedef struct
+{
+    GBOX *bbox;
+    void *data;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type;
+    char pad[1]; 
+}
+LWGEOM;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    POINTARRAY *point;  
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+}
+LWPOINT; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    POINTARRAY *points; 
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+}
+LWLINE; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    POINTARRAY *points;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type;
+    char pad[1]; 
+}
+LWTRIANGLE;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    POINTARRAY *points; 
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+}
+LWCIRCSTRING; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    POINTARRAY **rings; 
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t nrings;   
+    uint32_t maxrings; 
+}
+LWPOLY; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWPOINT **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWMPOINT;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWLINE **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWMLINE;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWPOLY **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWMPOLY;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWGEOM **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWCOLLECTION;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWGEOM **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWCOMPOUND; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWGEOM **rings;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t nrings;    
+    uint32_t maxrings;  
+}
+LWCURVEPOLY; 
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWGEOM **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWMCURVE;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWGEOM **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWMSURFACE;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWPOLY **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWPSURFACE;
+
+
+typedef struct
+{
+    GBOX *bbox;
+    LWTRIANGLE **geoms;
+    int32_t srid;
+    lwflags_t flags;
+    uint8_t type; 
+    char pad[1]; 
+    uint32_t ngeoms;   
+    uint32_t maxgeoms; 
+}
+LWTIN;
+
+extern LWPOINT *lwpoint_make(int32_t srid, int hasz, int hasm, const POINT4D *p);
+
+extern LWGEOM *lwgeom_from_gserialized(const GSERIALIZED *g);
+extern GSERIALIZED *gserialized_from_lwgeom(LWGEOM *geom, size_t *size);
+
+
+
+extern int32_t lwgeom_get_srid(const LWGEOM *geom);
+
+extern double lwpoint_get_x(const LWPOINT *point);
+extern double lwpoint_get_y(const LWPOINT *point);
+extern double lwpoint_get_z(const LWPOINT *point);
+extern double lwpoint_get_m(const LWPOINT *point);
+
+extern int lwgeom_has_z(const LWGEOM *geom);
+extern int lwgeom_has_m(const LWGEOM *geom);
+
+//#endif              
+
+
+/*****************************************************************************
+ * Toolchain dependent definitions
+ *****************************************************************************/
+
+//#ifdef _MSC_VER
+/*
+ * Under MSVC, functions exported by a loadable module must be marked
+ * "dllexport".  Other compilers don't need that.
+ * Borrowed from PostgreSQL file win32.h
+ */
+//#define PGDLLEXPORT __declspec (dllexport)
+/*
+ * Avoids warning C4996: 'strdup': The POSIX name for this item is deprecated.
+ */
+//#define strdup _strdup
+//#endif
+
+/*****************************************************************************
+ * Type definitions
+ *****************************************************************************/
+
+/**
+ * @brief Align to double
+ */
+//#define DOUBLE_PAD(size) ( (size) + ((size) % 8 ? (8 - (size) % 8) : 0 ) )
+
+/**
+ * Structure to represent sets of values
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 settype;        
+  uint8 basetype;       
+  int16 flags;          
+  int32 count;          
+  int32 maxcount;       
+  int16 bboxsize;       
+} Set;
+
+/**
+ * Structure to represent spans (a.k.a. ranges)
+ */
+typedef struct
+{
+  uint8 spantype;       
+  uint8 basetype;       
+  bool lower_inc;       
+  bool upper_inc;       
+  Datum lower;          
+  Datum upper;          
+} Span;
+
+/**
+ * Structure to represent span sets
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 spansettype;    
+  uint8 spantype;       
+  uint8 basetype;       
+  char padding;         
+  int32 count;          
+  int32 maxcount;       
+  Span span;            
+  Span elems[1];        
+} SpanSet;
+
+/**
+ * Structure to represent temporal boxes
+ */
+typedef struct
+{
+  Span period;          
+  Span span;            
+  int16 flags;          
+} TBox;
+
+/**
+ * Structure to represent spatiotemporal boxes
+ */
+typedef struct
+{
+  Span period;          
+  double xmin;          
+  double xmax;          
+  double ymin;          
+  double ymax;          
+  double zmin;          
+  double zmax;          
+  int32  srid;          
+  int16  flags;         
+} STBox;
+
+/**
+ * @brief Enumeration that defines the interpolation types used in
+ * MobilityDB.
+ */
+typedef enum
+{
+  INTERP_NONE =    0,
+  DISCRETE =       1,
+  STEP =           2,
+  LINEAR =         3,
+} interpType;
+
+/**
+ * @brief Enumeration that defines the spatial relationships for which a call
+ * to GEOS is made.
+ */
+typedef enum
+{
+  INTERSECTS =     0,
+  CONTAINS =       1,
+  TOUCHES =        2,
+} spatialRel;
+
+/**
+ * Structure to represent the common structure of temporal values of
+ * any temporal subtype
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 temptype;       
+  uint8 subtype;        
+  int16 flags;          
+  
+} Temporal;
+
+/**
+ * Structure to represent temporal values of instant subtype
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 temptype;       
+  uint8 subtype;        
+  int16 flags;          
+  TimestampTz t;        
+  Datum value;          /**< Base value for types passed by value,
+                             first 8 bytes of the base value for values
+                             passed by reference. The extra bytes
+                             needed are added upon creation. */
+  
+} TInstant;
+
+/**
+ * Structure to represent temporal values of instant set or sequence subtype
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 temptype;       
+  uint8 subtype;        
+  int16 flags;          
+  int32 count;          
+  int32 maxcount;       
+  int16 bboxsize;       
+  char padding[6];      
+  Span period;          /**< Time span (24 bytes). All bounding boxes start
+                             with a period so actually it is also the begining
+                             of the bounding box. The extra bytes needed for
+                             the bounding box are added upon creation. */
+  
+} TSequence;
+
+//#define TSEQUENCE_BBOX_PTR(seq)      ((void *)(&(seq)->period))
+
+/**
+ * Structure to represent temporal values of sequence set subtype
+ */
+typedef struct
+{
+  int32 vl_len_;        
+  uint8 temptype;       
+  uint8 subtype;        
+  int16 flags;          
+  int32 count;          
+  int32 totalcount;     /**< Total number of TInstant elements in all
+                             composing TSequence elements */
+  int32 maxcount;       
+  int16 bboxsize;       
+  int16 padding;        
+  Span period;          /**< Time span (24 bytes). All bounding boxes start
+                             with a period so actually it is also the begining
+                             of the bounding box. The extra bytes needed for
+                             the bounding box are added upon creation. */
+  
+} TSequenceSet;
+
+//#define TSEQUENCESET_BBOX_PTR(ss)      ((void *)(&(ss)->period))
+
+/**
+ * Struct for storing a similarity match
+ */
+typedef struct
+{
+  int i;
+  int j;
+} Match;
+
+
+
+/**
+ * Structure to represent skiplist elements
+ */
+
+#define SKIPLIST_MAXLEVEL 32
+typedef struct
+{
+  void *value;
+  int height;
+  int next[SKIPLIST_MAXLEVEL];
+} SkipListElem;
+
+/**
+ * Structure to represent skiplists that keep the current state of an aggregation
+ */
+typedef struct
+{
+  int capacity;
+  int next;
+  int length;
+  int *freed;
+  int freecount;
+  int freecap;
+  int tail;
+  void *extra;
+  size_t extrasize;
+  SkipListElem *elems;
+} SkipList;
+
+/*****************************************************************************
+ * Initialization of the MEOS library
+ *****************************************************************************/
+
+extern void meos_initialize(const char *tz_str);
+extern void meos_finalize(void);
+
+/*****************************************************************************
+ * Functions for input/output PostgreSQL time types
+ *****************************************************************************/
+
+extern bool bool_in(const char *in_str);
+extern char *bool_out(bool b);
+extern text *cstring2text(const char *cstring);
+extern DateADT pg_date_in(const char *str);
+extern char *pg_date_out(DateADT date);
+extern int pg_interval_cmp(const Interval *interval1, const Interval *interval2);
+extern Interval *pg_interval_in(const char *str, int32 typmod);
+extern Interval *pg_interval_make(int32 years, int32 months, int32 weeks, int32 days, int32 hours, int32 mins, double secs);
+extern Interval *pg_interval_mul(const Interval *span, double factor);
+extern char *pg_interval_out(const Interval *span);
+extern Interval *pg_interval_pl(const Interval *span1, const Interval *span2);
+extern TimeADT pg_time_in(const char *str, int32 typmod);
+extern char *pg_time_out(TimeADT time);
+extern Timestamp pg_timestamp_in(const char *str, int32 typmod);
+extern Interval *pg_timestamp_mi(TimestampTz dt1, TimestampTz dt2);
+extern TimestampTz pg_timestamp_mi_interval(TimestampTz timestamp, const Interval *span);
+extern char *pg_timestamp_out(Timestamp dt);
+extern TimestampTz pg_timestamp_pl_interval(TimestampTz timestamp, const Interval *span);
+extern TimestampTz pg_timestamptz_in(const char *str, int32 typmod);
+extern char *pg_timestamptz_out(TimestampTz dt);
+extern char *text2cstring(const text *textptr);
+
+/*****************************************************************************
+ * Functions for input/output and manipulation of PostGIS types
+ *****************************************************************************/
+
+extern bytea *gserialized_as_ewkb(const GSERIALIZED *geom, char *type);
+extern char *gserialized_as_ewkt(const GSERIALIZED *geom, int precision);
+extern char *gserialized_as_geojson(const GSERIALIZED *geom, int option, int precision, char *srs);
+extern char *gserialized_as_hexewkb(const GSERIALIZED *geom, const char *type);
+extern char *gserialized_as_text(const GSERIALIZED *geom, int precision);
+extern GSERIALIZED *gserialized_from_ewkb(const bytea *bytea_wkb, int32 srid);
+extern GSERIALIZED *gserialized_from_geojson(const char *geojson);
+extern GSERIALIZED *gserialized_from_hexewkb(const char *wkt);
+extern GSERIALIZED *gserialized_from_text(char *wkt, int srid);
+extern GSERIALIZED *gserialized_in(char *input, int32 geom_typmod);
+extern char *gserialized_out(const GSERIALIZED *geom);
+extern bool pgis_gserialized_same(const GSERIALIZED *geom1, const GSERIALIZED *geom2);
+
+/*****************************************************************************
+ * Functions for set and span types
+ *****************************************************************************/
+
+
+
+extern Set *bigintset_in(const char *str);
+extern char *bigintset_out(const Set *set);
+extern Span *bigintspan_in(const char *str);
+extern char *bigintspan_out(const Span *s);
+extern SpanSet *bigintspanset_in(const char *str);
+extern char *bigintspanset_out(const SpanSet *ss);
+extern Set *floatset_in(const char *str);
+extern char *floatset_out(const Set *set, int maxdd);
+extern Span *floatspan_in(const char *str);
+extern char *floatspan_out(const Span *s, int maxdd);
+extern SpanSet *floatspanset_in(const char *str);
+extern char *floatspanset_out(const SpanSet *ss, int maxdd);
+extern Set *geogset_in(const char *str);
+extern char *geogset_out(const Set *set, int maxdd);
+extern Set *geomset_in(const char *str);
+extern char *geomset_out(const Set *set, int maxdd);
+extern char *geoset_as_ewkt(const Set *set, int maxdd);
+extern char *geoset_as_text(const Set *set, int maxdd);
+extern Set *intset_in(const char *str);
+extern char *intset_out(const Set *set);
+extern Span *intspan_in(const char *str);
+extern char *intspan_out(const Span *s);
+extern SpanSet *intspanset_in(const char *str);
+extern char *intspanset_out(const SpanSet *ss);
+extern Span *period_in(const char *str);
+extern char *period_out(const Span *s);
+extern SpanSet *periodset_in(const char *str);
+extern char *periodset_out(const SpanSet *ss);
+extern char *set_as_hexwkb(const Set *s, uint8_t variant, size_t *size_out);
+extern uint8_t *set_as_wkb(const Set *s, uint8_t variant, size_t *size_out);
+extern Set *set_from_hexwkb(const char *hexwkb);
+extern Set *set_from_wkb(const uint8_t *wkb, size_t size);
+extern char *set_out(const Set *s, int maxdd);
+extern uint8_t *span_as_wkb(const Span *s, uint8_t variant, size_t *size_out);
+extern char *span_as_hexwkb(const Span *s, uint8_t variant, size_t *size_out);
+extern Span *span_from_hexwkb(const char *hexwkb);
+extern Span *span_from_wkb(const uint8_t *wkb, size_t size);
+extern char *span_out(const Span *s, int maxdd);
+extern uint8_t *spanset_as_wkb(const SpanSet *ss, uint8_t variant, size_t *size_out);
+extern char *spanset_as_hexwkb(const SpanSet *ss, uint8_t variant, size_t *size_out);
+extern SpanSet *spanset_from_hexwkb(const char *hexwkb);
+extern SpanSet *spanset_from_wkb(const uint8_t *wkb, size_t size);
+extern char *spanset_out(const SpanSet *ss, int maxdd);
+extern Set *textset_in(const char *str);
+extern char *textset_out(const Set *set);
+extern Set *timestampset_in(const char *str);
+extern char *timestampset_out(const Set *set);
+
+
+
+
+
+extern Set *bigintset_make(const int64 *values, int count);
+extern Span *bigintspan_make(int64 lower, int64 upper, bool lower_inc, bool upper_inc);
+extern Set *floatset_make(const double *values, int count);
+extern Span *floatspan_make(double lower, double upper, bool lower_inc, bool upper_inc);
+extern Set *geogset_make(const GSERIALIZED **values, int count);
+extern Set *geomset_make(const GSERIALIZED **values, int count);
+extern Set *intset_make(const int *values, int count);
+extern Span *intspan_make(int lower, int upper, bool lower_inc, bool upper_inc);
+extern Span *period_make(TimestampTz lower, TimestampTz upper, bool lower_inc, bool upper_inc);
+extern Set *set_copy(const Set *s);
+extern Span *span_copy(const Span *s);
+extern SpanSet *spanset_copy(const SpanSet *ps);
+extern SpanSet *spanset_make(Span *spans, int count, bool normalize);
+extern SpanSet *spanset_make_exp(Span *spans, int count, int maxcount, bool normalize, bool ordered);
+extern SpanSet *spanset_make_free(Span *spans, int count, bool normalize);
+extern Set *textset_make(const text **values, int count);
+extern Set *timestampset_make(const TimestampTz *values, int count);
+
+
+
+
+
+extern Set *bigint_to_bigintset(int64 i);
+extern Span *bigint_to_bigintspan(int i);
+extern SpanSet *bigint_to_bigintspanset(int i);
+extern Set *float_to_floatset(double d);
+extern Span *float_to_floatspan(double d);
+extern SpanSet *float_to_floatspanset(double d);
+extern Set *int_to_intset(int i);
+extern Span *int_to_intspan(int i);
+extern SpanSet *int_to_intspanset(int i);
+extern SpanSet *set_to_spanset(const Set *s);
+extern SpanSet *span_to_spanset(const Span *s);
+extern Span *timestamp_to_period(TimestampTz t);
+extern SpanSet *timestamp_to_periodset(TimestampTz t);
+extern Set *timestamp_to_tstzset(TimestampTz t);
+
+
+
+
+
+extern int64 bigintset_end_value(const Set *s);
+extern int64 bigintset_start_value(const Set *s);
+extern bool bigintset_value_n(const Set *s, int n, int64 *result);
+extern int64 *bigintset_values(const Set *s);
+extern int bigintspan_lower(const Span *s);
+extern int bigintspan_upper(const Span *s);
+extern int bigintspanset_lower(const SpanSet *ss);
+extern int bigintspanset_upper(const SpanSet *ss);
+extern double floatset_end_value(const Set *s);
+extern double floatset_start_value(const Set *s);
+extern bool floatset_value_n(const Set *s, int n, double *result);
+extern double *floatset_values(const Set *s);
+extern double floatspan_lower(const Span *s);
+extern double floatspan_upper(const Span *s);
+extern double floatspanset_lower(const SpanSet *ss);
+extern double floatspanset_upper(const SpanSet *ss);
+extern int geoset_srid(const Set *set);
+extern int intset_end_value(const Set *s);
+extern int intset_start_value(const Set *s);
+extern bool intset_value_n(const Set *s, int n, int *result);
+extern int *intset_values(const Set *s);
+extern int intspan_lower(const Span *s);
+extern int intspan_upper(const Span *s);
+extern int intspanset_lower(const SpanSet *ss);
+extern int intspanset_upper(const SpanSet *ss);
+extern Interval *period_duration(const Span *s);
+extern TimestampTz period_lower(const Span *p);
+extern TimestampTz period_upper(const Span *p);
+extern Interval *periodset_duration(const SpanSet *ps, bool boundspan);
+extern TimestampTz periodset_end_timestamp(const SpanSet *ps);
+extern TimestampTz periodset_lower(const SpanSet *ps);
+extern int periodset_num_timestamps(const SpanSet *ps);
+extern TimestampTz periodset_start_timestamp(const SpanSet *ps);
+extern bool periodset_timestamp_n(const SpanSet *ps, int n, TimestampTz *result);
+extern TimestampTz *periodset_timestamps(const SpanSet *ps, int *count);
+extern TimestampTz periodset_upper(const SpanSet *ps);
+extern uint32 set_hash(const Set *s);
+extern uint64 set_hash_extended(const Set *s, uint64 seed);
+extern int set_mem_size(const Set *s);
+extern int set_num_values(const Set *s);
+extern Span *set_span(const Set *s);
+extern uint32 span_hash(const Span *s);
+extern uint64 span_hash_extended(const Span *s, uint64 seed);
+extern bool span_lower_inc(const Span *s);
+extern bool span_upper_inc(const Span *s);
+extern double span_width(const Span *s);
+extern Span *spanset_end_span(const SpanSet *ss);
+extern uint32 spanset_hash(const SpanSet *ps);
+extern uint64 spanset_hash_extended(const SpanSet *ps, uint64 seed);
+extern bool spanset_lower_inc(const SpanSet *ss);
+extern int spanset_mem_size(const SpanSet *ss);
+extern int spanset_num_spans(const SpanSet *ss);
+extern Span *spanset_span(const SpanSet *ss);
+extern Span *spanset_span_n(const SpanSet *ss, int i);
+extern const Span **spanset_spans(const SpanSet *ss);
+extern Span *spanset_start_span(const SpanSet *ss);
+extern bool spanset_upper_inc(const SpanSet *ss);
+extern double spanset_width(const SpanSet *ss);
+extern STBox *spatialset_stbox(const Set *s);
+extern TimestampTz timestampset_end_timestamp(const Set *ts);
+extern TimestampTz timestampset_start_timestamp(const Set *ts);
+extern bool timestampset_timestamp_n(const Set *ts, int n, TimestampTz *result);
+extern TimestampTz *timestampset_values(const Set *ts);
+
+
+
+
+
+extern void floatspan_set_intspan(const Span *s1, Span *s2);
+extern void intspan_set_floatspan(const Span *s1, Span *s2);
+extern void numspan_set_floatspan(const Span *s1, Span *s2);
+extern Span *period_tprecision(const Span *s, const Interval *duration, TimestampTz torigin);
+extern SpanSet *periodset_tprecision(const SpanSet *ss, const Interval *duration, TimestampTz torigin);
+extern Span *period_shift_tscale(const Span *p, const Interval *shift, const Interval *duration);
+extern SpanSet *periodset_shift_tscale(const SpanSet *ps, const Interval *shift, const Interval *duration);
+extern Set *set_shift(const Set *s, Datum shift);
+extern void span_expand(const Span *s1, Span *s2);
+extern TimestampTz timestamp_tprecision(TimestampTz t, const Interval *duration, TimestampTz torigin);
+extern Set *timestampset_shift_tscale(const Set *ts, const Interval *shift, const Interval *duration);
+
+/*****************************************************************************
+ * Bounding box functions for set and span types
+ *****************************************************************************/
+
+
+
+extern bool adjacent_bigintspan_bigint(const Span *s, int64 i);
+extern bool adjacent_bigintspanset_bigint(const SpanSet *ss, int64 i);
+extern bool adjacent_floatspan_float(const Span *s, double d);
+extern bool adjacent_intspan_int(const Span *s, int i);
+extern bool adjacent_period_timestamp(const Span *p, TimestampTz t);
+extern bool adjacent_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern bool adjacent_span_span(const Span *s1, const Span *s2);
+extern bool adjacent_spanset_span(const SpanSet *ss, const Span *s);
+extern bool adjacent_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool contained_bigint_bigintset(int64 i, const Set *s);
+extern bool contained_bigint_bigintspan(int64 i, const Span *s);
+extern bool contained_bigint_bigintspanset(int64 i, const SpanSet *ss);
+extern bool contained_float_floatset(double d, const Set *s);
+extern bool contained_float_floatspan(double d, const Span *s);
+extern bool contained_float_floatspanset(double d, const SpanSet *ss);
+extern bool contained_int_intset(int i, const Set *s);
+extern bool contained_int_intspanset (int i, const SpanSet *ss);
+extern bool contained_int_intspan(int i, const Span *s);
+extern bool contained_set_set(const Set *s1, const Set *s2);
+extern bool contained_span_span(const Span *s1, const Span *s2);
+extern bool contained_span_spanset(const Span *s, const SpanSet *ss);
+extern bool contained_spanset_span(const SpanSet *ss, const Span *s);
+extern bool contained_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool contained_timestamp_period(TimestampTz t, const Span *p);
+extern bool contained_timestamp_timestampset(TimestampTz t, const Set *ts);
+extern bool contains_floatspan_float(const Span *s, double d);
+extern bool contains_floatspanset_float(const SpanSet *ss, double d);
+extern bool contains_intspan_int(const Span *s, int i);
+extern bool contains_set_set(const Set *s1, const Set *s2);
+extern bool contains_period_timestamp(const Span *p, TimestampTz t);
+extern bool contains_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern bool contains_span_span(const Span *s1, const Span *s2);
+extern bool contains_span_spanset(const Span *s, const SpanSet *ss);
+extern bool contains_spanset_span(const SpanSet *ss, const Span *s);
+extern bool contains_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool contains_timestampset_timestamp(const Set *ts, TimestampTz t);
+extern bool overlaps_set_set(const Set *s1, const Set *s2);
+extern bool overlaps_span_span(const Span *s1, const Span *s2);
+extern bool overlaps_spanset_span(const SpanSet *ss, const Span *s);
+extern bool overlaps_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+
+
+
+
+
+extern bool after_timestamp_timestampset(TimestampTz t, const Set *ts);
+extern bool before_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern bool before_timestamp_timestampset(TimestampTz t, const Set *ts);
+extern bool left_float_floatspan(double d, const Span *s);
+extern bool left_floatspan_float(const Span *s, double d);
+extern bool left_int_intspan(int i, const Span *s);
+extern bool left_intspan_int(const Span *s, int i);
+extern bool left_set_set(const Set *s1, const Set *s2);
+extern bool left_span_span(const Span *s1, const Span *s2);
+extern bool left_span_spanset(const Span *s, const SpanSet *ss);
+extern bool left_spanset_span(const SpanSet *ss, const Span *s);
+extern bool left_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool overafter_period_timestamp(const Span *p, TimestampTz t);
+extern bool overafter_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern bool overafter_timestamp_period(TimestampTz t, const Span *p);
+extern bool overafter_timestamp_periodset(TimestampTz t, const SpanSet *ps);
+extern bool overafter_timestamp_timestampset(TimestampTz t, const Set *ts);
+extern bool overbefore_period_timestamp(const Span *p, TimestampTz t);
+extern bool overbefore_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern bool overbefore_timestamp_period(TimestampTz t, const Span *p);
+extern bool overbefore_timestamp_periodset(TimestampTz t, const SpanSet *ps);
+extern bool overbefore_timestamp_timestampset(TimestampTz t, const Set *ts);
+extern bool overleft_float_floatspan(double d, const Span *s);
+extern bool overleft_floatspan_float(const Span *s, double d);
+extern bool overleft_int_intspan(int i, const Span *s);
+extern bool overleft_intspan_int(const Span *s, int i);
+extern bool overleft_set_set(const Set *s1, const Set *s2);
+extern bool overleft_span_span(const Span *s1, const Span *s2);
+extern bool overleft_span_spanset(const Span *s, const SpanSet *ss);
+extern bool overleft_spanset_span(const SpanSet *ss, const Span *s);
+extern bool overleft_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool overright_float_floatspan(double d, const Span *s);
+extern bool overright_floatspan_float(const Span *s, double d);
+extern bool overright_int_intspan(int i, const Span *s);
+extern bool overright_intspan_int(const Span *s, int i);
+extern bool overright_set_set(const Set *s1, const Set *s2);
+extern bool overright_span_span(const Span *s1, const Span *s2);
+extern bool overright_span_spanset(const Span *s, const SpanSet *ss);
+extern bool overright_spanset_span(const SpanSet *ss, const Span *s);
+extern bool overright_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool right_float_floatspan(double d, const Span *s);
+extern bool right_floatspan_float(const Span *s, double d);
+extern bool right_int_intspan(int i, const Span *s);
+extern bool right_intspan_int(const Span *s, int i);
+extern bool right_set_set(const Set *s1, const Set *s2);
+extern bool right_span_span(const Span *s1, const Span *s2);
+extern bool right_span_spanset(const Span *s, const SpanSet *ss);
+extern bool right_spanset_span(const SpanSet *ss, const Span *s);
+extern bool right_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+
+
+
+
+
+extern void bbox_union_span_span(const Span *s1, const Span *s2, Span *result);
+extern Set *intersection_set_set(const Set *s1, const Set *s2);
+extern bool intersection_period_timestamp(const Span *p, TimestampTz t, TimestampTz *result);
+extern bool intersection_periodset_timestamp(const SpanSet *ps, TimestampTz t, TimestampTz *result);
+extern Span *intersection_span_span(const Span *s1, const Span *s2);
+extern SpanSet *intersection_spanset_span(const SpanSet *ss, const Span *s);
+extern SpanSet *intersection_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool intersection_timestampset_timestamp(const Set *ts, const TimestampTz t, TimestampTz *result);
+extern Set *minus_set_set(const Set *s1, const Set *s2);
+extern SpanSet *minus_period_timestamp(const Span *p, TimestampTz t);
+extern SpanSet *minus_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern SpanSet *minus_span_span(const Span *s1, const Span *s2);
+extern SpanSet *minus_span_spanset(const Span *s, const SpanSet *ss);
+extern SpanSet *minus_spanset_span(const SpanSet *ss, const Span *s);
+extern SpanSet *minus_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern bool minus_timestamp_period(TimestampTz t, const Span *p, TimestampTz *result);
+extern bool minus_timestamp_periodset(TimestampTz t, const SpanSet *ps, TimestampTz *result);
+extern Set *minus_timestampset_timestamp(const Set *ts, TimestampTz t);
+extern Set *union_set_set(const Set *s1, const Set *s2);
+extern SpanSet *union_period_timestamp(const Span *p, TimestampTz t);
+extern SpanSet *union_periodset_timestamp(SpanSet *ps, TimestampTz t);
+extern SpanSet *union_span_span(const Span *s1, const Span *s2);
+extern SpanSet *union_spanset_span(const SpanSet *ss, const Span *s);
+extern SpanSet *union_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern Set *union_timestampset_timestamp(const Set *ts, const TimestampTz t);
+
+
+
+
+
+extern double distance_floatspan_float(const Span *s, double d);
+extern double distance_intspan_int(const Span *s, int i);
+extern double distance_set_set(const Set *s1, const Set *s2);
+extern double distance_period_timestamp(const Span *p, TimestampTz t);
+extern double distance_periodset_timestamp(const SpanSet *ps, TimestampTz t);
+extern double distance_span_span(const Span *s1, const Span *s2);
+extern double distance_spanset_span(const SpanSet *ss, const Span *s);
+extern double distance_spanset_spanset(const SpanSet *ss1, const SpanSet *ss2);
+extern double distance_timestampset_timestamp(const Set *ts, TimestampTz t);
+
+
+
+
+
+extern Span *bigint_extent_transfn(Span *s, int64 i);
+extern Set *bigint_union_transfn(Set *state, int64 i);
+extern Span *float_extent_transfn(Span *s, double d);
+extern Set *float_union_transfn(Set *state, double d);
+extern Span *int_extent_transfn(Span *s, int i);
+extern Set *int_union_transfn(Set *state, int i);
+extern SkipList *period_tcount_transfn(SkipList *state, const Span *p);
+extern SkipList *periodset_tcount_transfn(SkipList *state, const SpanSet *ps);
+extern Span *set_extent_transfn(Span *span, const Set *set);
+extern Set *set_union_finalfn(Set *state);
+extern Set *set_union_transfn(Set *state, Set *set);
+extern Span *span_extent_transfn(Span *s1, const Span *s2);
+extern SpanSet *span_union_transfn(SpanSet *state, const Span *span);
+extern Span *spanset_extent_transfn(Span *s, const SpanSet *ss);
+extern SpanSet *spanset_union_finalfn(SpanSet *state);
+extern SpanSet *spanset_union_transfn(SpanSet *state, const SpanSet *ss);
+extern Set *text_union_transfn(Set *state, const text *txt);
+extern Span *timestamp_extent_transfn(Span *p, TimestampTz t);
+extern SkipList *timestamp_tcount_transfn(SkipList *state, TimestampTz t);
+extern Set *timestamp_union_transfn(Set *state, TimestampTz t);
+extern SkipList *timestampset_tcount_transfn(SkipList *state, const Set *ts);
+
+
+
+
+
+extern int set_cmp(const Set *s1, const Set *s2);
+extern bool set_eq(const Set *s1, const Set *s2);
+extern bool set_ge(const Set *s1, const Set *s2);
+extern bool set_gt(const Set *s1, const Set *s2);
+extern bool set_le(const Set *s1, const Set *s2);
+extern bool set_lt(const Set *s1, const Set *s2);
+extern bool set_ne(const Set *s1, const Set *s2);
+extern int span_cmp(const Span *s1, const Span *s2);
+extern bool span_eq(const Span *s1, const Span *s2);
+extern bool span_ge(const Span *s1, const Span *s2);
+extern bool span_gt(const Span *s1, const Span *s2);
+extern bool span_le(const Span *s1, const Span *s2);
+extern bool span_lt(const Span *s1, const Span *s2);
+extern bool span_ne(const Span *s1, const Span *s2);
+extern int spanset_cmp(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_eq(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_ge(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_gt(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_le(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_lt(const SpanSet *ss1, const SpanSet *ss2);
+extern bool spanset_ne(const SpanSet *ss1, const SpanSet *ss2);
+
+/******************************************************************************
+ * Functions for box types
+ *****************************************************************************/
+
+
+
+extern TBox *tbox_in(const char *str);
+extern char *tbox_out(const TBox *box, int maxdd);
+extern TBox *tbox_from_wkb(const uint8_t *wkb, size_t size);
+extern TBox *tbox_from_hexwkb(const char *hexwkb);
+extern STBox *stbox_from_wkb(const uint8_t *wkb, size_t size);
+extern STBox *stbox_from_hexwkb(const char *hexwkb);
+extern uint8_t *tbox_as_wkb(const TBox *box, uint8_t variant, size_t *size_out);
+extern char *tbox_as_hexwkb(const TBox *box, uint8_t variant, size_t *size);
+extern uint8_t *stbox_as_wkb(const STBox *box, uint8_t variant, size_t *size_out);
+extern char *stbox_as_hexwkb(const STBox *box, uint8_t variant, size_t *size);
+extern STBox *stbox_in(const char *str);
+extern char *stbox_out(const STBox *box, int maxdd);
+
+
+
+
+
+extern TBox *tbox_make(const Span *s, const Span *p);
+extern void tbox_set(const Span *s, const Span *p, TBox *box);
+extern TBox *tbox_copy(const TBox *box);
+extern STBox * stbox_make(bool hasx, bool hasz, bool geodetic, int32 srid,
+  double xmin, double xmax, double ymin, double ymax, double zmin, double zmax, const Span *p);
+extern void stbox_set(bool hasx, bool hasz, bool geodetic, int32 srid, double xmin, double xmax,
+  double ymin, double ymax, double zmin, double zmax, const Span *p, STBox *box);
+extern STBox *stbox_copy(const STBox *box);
+
+
+
+
+
+extern TBox *int_to_tbox(int i);
+extern TBox *float_to_tbox(double d);
+extern TBox *timestamp_to_tbox(TimestampTz t);
+extern TBox *timestampset_to_tbox(const Set *ss);
+extern TBox *period_to_tbox(const Span *p);
+extern TBox *periodset_to_tbox(const SpanSet *ps);
+extern TBox *int_timestamp_to_tbox(int i, TimestampTz t);
+extern TBox *float_period_to_tbox(double d, const Span *p);
+extern TBox *float_timestamp_to_tbox(double d, TimestampTz t);
+extern STBox *geo_period_to_stbox(const GSERIALIZED *gs, const Span *p);
+extern STBox *geo_timestamp_to_stbox(const GSERIALIZED *gs, TimestampTz t);
+extern STBox *geo_to_stbox(const GSERIALIZED *gs);
+extern TBox *int_period_to_tbox(int i, const Span *p);
+extern TBox *numspan_to_tbox(const Span *s);
+extern TBox *span_timestamp_to_tbox(const Span *span, TimestampTz t);
+extern TBox *span_period_to_tbox(const Span *span, const Span *p);
+extern Span *tbox_to_floatspan(const TBox *box);
+extern Span *tbox_to_period(const TBox *box);
+extern Span *stbox_to_period(const STBox *box);
+extern TBox *tnumber_to_tbox(const Temporal *temp);
+extern GSERIALIZED *stbox_to_geo(const STBox *box);
+extern STBox *tpoint_to_stbox(const Temporal *temp);
+extern STBox *timestamp_to_stbox(TimestampTz t);
+extern STBox *timestampset_to_stbox(const Set *ts);
+extern STBox *period_to_stbox(const Span *p);
+extern STBox *periodset_to_stbox(const SpanSet *ps);
+
+
+
+
+
+extern bool tbox_hasx(const TBox *box);
+extern bool tbox_hast(const TBox *box);
+extern bool tbox_xmin(const TBox *box, double *result);
+extern bool tbox_xmax(const TBox *box, double *result);
+extern bool tbox_tmin(const TBox *box, TimestampTz *result);
+extern bool tbox_tmax(const TBox *box, TimestampTz *result);
+extern bool stbox_hasx(const STBox *box);
+extern bool stbox_hasz(const STBox *box);
+extern bool stbox_hast(const STBox *box);
+extern bool stbox_isgeodetic(const STBox *box);
+extern bool stbox_xmin(const STBox *box, double *result);
+extern bool stbox_xmax(const STBox *box, double *result);
+extern bool stbox_ymin(const STBox *box, double *result);
+extern bool stbox_ymax(const STBox *box, double *result);
+extern bool stbox_zmin(const STBox *box, double *result);
+extern bool stbox_zmax(const STBox *box, double *result);
+extern bool stbox_tmin(const STBox *box, TimestampTz *result);
+extern bool stbox_tmax(const STBox *box, TimestampTz *result);
+extern int32 stbox_srid(const STBox *box);
+
+
+
+
+
+extern void tbox_expand(const TBox *box1, TBox *box2);
+extern TBox *tbox_expand_value(const TBox *box, const double d);
+extern TBox *tbox_expand_time(const TBox *box, const Interval *interval);
+extern void stbox_expand(const STBox *box1, STBox *box2);
+extern STBox *stbox_set_srid(const STBox *box, int32 srid);
+extern STBox *stbox_get_space(const STBox *box);
+extern STBox *stbox_expand_space(const STBox *box, double d);
+extern STBox *stbox_expand_time(const STBox *box, const Interval *interval);
+
+
+
+
+
+extern bool contains_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool contained_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool overlaps_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool same_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool adjacent_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool contains_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool contained_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overlaps_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool same_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool adjacent_stbox_stbox(const STBox *box1, const STBox *box2);
+
+
+
+
+
+extern bool left_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool overleft_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool right_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool overright_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool before_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool overbefore_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool after_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool overafter_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool left_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overleft_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool right_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overright_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool below_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overbelow_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool above_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overabove_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool front_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overfront_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool back_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overback_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool before_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overbefore_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool after_stbox_stbox(const STBox *box1, const STBox *box2);
+extern bool overafter_stbox_stbox(const STBox *box1, const STBox *box2);
+
+
+
+
+
+extern TBox *union_tbox_tbox(const TBox *box1, const TBox *box2);
+extern bool inter_tbox_tbox(const TBox *box1, const TBox *box2, TBox *result);
+extern TBox *intersection_tbox_tbox(const TBox *box1, const TBox *box2);
+extern STBox *union_stbox_stbox(const STBox *box1, const STBox *box2, bool strict);
+extern bool inter_stbox_stbox(const STBox *box1, const STBox *box2, STBox *result);
+extern STBox *intersection_stbox_stbox(const STBox *box1, const STBox *box2);
+
+
+
+
+
+extern STBox *stbox_quad_split(const STBox *box, int *count);
+
+
+
+
+
+extern bool tbox_eq(const TBox *box1, const TBox *box2);
+extern bool tbox_ne(const TBox *box1, const TBox *box2);
+extern int tbox_cmp(const TBox *box1, const TBox *box2);
+extern bool tbox_lt(const TBox *box1, const TBox *box2);
+extern bool tbox_le(const TBox *box1, const TBox *box2);
+extern bool tbox_ge(const TBox *box1, const TBox *box2);
+extern bool tbox_gt(const TBox *box1, const TBox *box2);
+extern bool stbox_eq(const STBox *box1, const STBox *box2);
+extern bool stbox_ne(const STBox *box1, const STBox *box2);
+extern int stbox_cmp(const STBox *box1, const STBox *box2);
+extern bool stbox_lt(const STBox *box1, const STBox *box2);
+extern bool stbox_le(const STBox *box1, const STBox *box2);
+extern bool stbox_ge(const STBox *box1, const STBox *box2);
+extern bool stbox_gt(const STBox *box1, const STBox *box2);
+
+/*****************************************************************************
+ * Functions for temporal types
+ *****************************************************************************/
+
+
+
+extern Temporal *tbool_in(const char *str);
+extern char *tbool_out(const Temporal *temp);
+extern char *temporal_as_hexwkb(const Temporal *temp, uint8_t variant, size_t *size_out);
+extern char *temporal_as_mfjson(const Temporal *temp, bool with_bbox, int flags, int precision, char *srs);
+extern uint8_t *temporal_as_wkb(const Temporal *temp, uint8_t variant, size_t *size_out);
+extern Temporal *temporal_from_hexwkb(const char *hexwkb);
+extern Temporal *temporal_from_mfjson(const char *mfjson);
+extern Temporal *temporal_from_wkb(const uint8_t *wkb, size_t size);
+extern Temporal *tfloat_in(const char *str);
+extern char *tfloat_out(const Temporal *temp, int maxdd);
+extern Temporal *tgeogpoint_in(const char *str);
+extern Temporal *tgeompoint_in(const char *str);
+extern Temporal *tint_in(const char *str);
+extern char *tint_out(const Temporal *temp);
+extern char *tpoint_as_ewkt(const Temporal *temp, int maxdd);
+extern char *tpoint_as_text(const Temporal *temp, int maxdd);
+extern char *tpoint_out(const Temporal *temp, int maxdd);
+extern Temporal *ttext_in(const char *str);
+extern char *ttext_out(const Temporal *temp);
+
+
+
+
+
+extern Temporal *tbool_from_base_temp(bool b, const Temporal *temp);
+extern TInstant *tboolinst_make(bool b, TimestampTz t);
+extern TSequence *tboolseq_from_base_period(bool b, const Span *p);
+extern TSequence *tboolseq_from_base_temp(bool b, const TSequence *seq);
+extern TSequence *tboolseq_from_base_timestampset(bool b, const Set *ts);
+extern TSequenceSet *tboolseqset_from_base_periodset(bool b, const SpanSet *ps);
+extern TSequenceSet *tboolseqset_from_base_temp(bool b, const TSequenceSet *ss);
+extern Temporal *temporal_copy(const Temporal *temp);
+extern Temporal *tfloat_from_base_temp(double d, const Temporal *temp);
+extern TInstant *tfloatinst_make(double d, TimestampTz t);
+extern TSequence *tfloatseq_from_base_period(double d, const Span *p, interpType interp);
+extern TSequence *tfloatseq_from_base_temp(double d, const TSequence *seq);
+extern TSequence *tfloatseq_from_base_timestampset(double d, const Set *ts);
+extern TSequenceSet *tfloatseqset_from_base_periodset(double d, const SpanSet *ps, interpType interp);
+extern TSequenceSet *tfloatseqset_from_base_temp(double d, const TSequenceSet *ss);
+extern Temporal *tgeogpoint_from_base_temp(const GSERIALIZED *gs, const Temporal *temp);
+extern TInstant *tgeogpointinst_make(const GSERIALIZED *gs, TimestampTz t);
+extern TSequence *tgeogpointseq_from_base_period(const GSERIALIZED *gs, const Span *p, interpType interp);
+extern TSequence *tgeogpointseq_from_base_temp(const GSERIALIZED *gs, const TSequence *seq);
+extern TSequence *tgeogpointseq_from_base_timestampset(const GSERIALIZED *gs, const Set *ts);
+extern TSequenceSet *tgeogpointseqset_from_base_temp(const GSERIALIZED *gs, const TSequenceSet *ss);
+extern TSequenceSet *tgeogpointseqset_from_base_periodset(const GSERIALIZED *gs, const SpanSet *ps, interpType interp);
+extern Temporal *tgeompoint_from_base_temp(const GSERIALIZED *gs, const Temporal *temp);
+extern TInstant *tgeompointinst_make(const GSERIALIZED *gs, TimestampTz t);
+extern TSequence *tgeompointseq_from_base_period(const GSERIALIZED *gs, const Span *p, interpType interp);
+extern TSequence *tgeompointseq_from_base_temp(const GSERIALIZED *gs, const TSequence *seq);
+extern TSequence *tgeompointseq_from_base_timestampset(const GSERIALIZED *gs, const Set *ts);
+extern TSequenceSet *tgeompointseqset_from_base_periodset(const GSERIALIZED *gs, const SpanSet *ps, interpType interp);
+extern TSequenceSet *tgeompointseqset_from_base_temp(const GSERIALIZED *gs, const TSequenceSet *ss);
+extern Temporal *tint_from_base_temp(int i, const Temporal *temp);
+extern TInstant *tintinst_make(int i, TimestampTz t);
+extern TSequence *tintseq_from_base_period(int i, const Span *p);
+extern TSequence *tintseq_from_base_temp(int i, const TSequence *seq);
+extern TSequence *tintseq_from_base_timestampset(int i, const Set *ts);
+extern TSequenceSet *tintseqset_from_base_periodset(int i, const SpanSet *ps);
+extern TSequenceSet *tintseqset_from_base_temp(int i, const TSequenceSet *ss);
+extern TSequence *tsequence_make(const TInstant **instants, int count, bool lower_inc, bool upper_inc, interpType interp, bool normalize);
+extern TSequence *tsequence_make_exp(const TInstant **instants, int count, int maxcount, bool lower_inc, bool upper_inc, interpType interp, bool normalize);
+extern TSequenceSet *tsequenceset_make(const TSequence **sequences, int count, bool normalize);
+extern TSequenceSet *tsequenceset_make_exp(const TSequence **sequences, int count, int maxcount, bool normalize);
+extern TSequenceSet *tsequenceset_make_gaps(const TInstant **instants, int count, interpType interp, Interval *maxt, double maxdist);
+extern Temporal *ttext_from_base_temp(const text *txt, const Temporal *temp);
+extern TInstant *ttextinst_make(const text *txt, TimestampTz t);
+extern TSequence *ttextseq_from_base_period(const text *txt, const Span *p);
+extern TSequence *ttextseq_from_base_temp(const text *txt, const TSequence *seq);
+extern TSequence *ttextseq_from_base_timestampset(const text *txt, const Set *ts);
+extern TSequenceSet *ttextseqset_from_base_periodset(const text *txt, const SpanSet *ps);
+extern TSequenceSet *ttextseqset_from_base_temp(const text *txt, const TSequenceSet *ss);
+
+
+
+
+
+extern Span *temporal_to_period(const Temporal *temp);
+extern Temporal *tfloat_to_tint(const Temporal *temp);
+extern Temporal *tint_to_tfloat(const Temporal *temp);
+extern Span *tnumber_to_span(const Temporal *temp);
+
+
+
+
+
+extern bool tbool_end_value(const Temporal *temp);
+extern bool tbool_start_value(const Temporal *temp);
+extern bool *tbool_values(const Temporal *temp, int *count);
+extern Interval *temporal_duration(const Temporal *temp, bool boundspan);
+extern const TInstant *temporal_end_instant(const Temporal *temp);
+extern TSequence *temporal_end_sequence(const Temporal *temp);
+extern TimestampTz temporal_end_timestamp(const Temporal *temp);
+extern uint32 temporal_hash(const Temporal *temp);
+extern const TInstant *temporal_instant_n(const Temporal *temp, int n);
+extern const TInstant **temporal_instants(const Temporal *temp, int *count);
+extern char *temporal_interp(const Temporal *temp);
+extern const TInstant *temporal_max_instant(const Temporal *temp);
+extern const TInstant *temporal_min_instant(const Temporal *temp);
+extern int temporal_num_instants(const Temporal *temp);
+extern int temporal_num_sequences(const Temporal *temp);
+extern int temporal_num_timestamps(const Temporal *temp);
+extern TSequence **temporal_segments(const Temporal *temp, int *count);
+extern TSequence *temporal_sequence_n(const Temporal *temp, int i);
+extern TSequence **temporal_sequences(const Temporal *temp, int *count);
+extern const TInstant *temporal_start_instant(const Temporal *temp);
+extern TSequence *temporal_start_sequence(const Temporal *temp);
+extern TimestampTz temporal_start_timestamp(const Temporal *temp);
+extern TSequenceSet *temporal_stops(const Temporal *temp, double maxdist, const Interval *minduration);
+extern char *temporal_subtype(const Temporal *temp);
+extern SpanSet *temporal_time(const Temporal *temp);
+extern bool temporal_timestamp_n(const Temporal *temp, int n, TimestampTz *result);
+extern TimestampTz *temporal_timestamps(const Temporal *temp, int *count);
+extern Datum *temporal_values(const Temporal *temp, int *count);
+extern double tfloat_end_value(const Temporal *temp);
+extern double tfloat_max_value(const Temporal *temp);
+extern double tfloat_min_value(const Temporal *temp);
+extern double tfloat_start_value(const Temporal *temp);
+extern double *tfloat_values(const Temporal *temp, int *count);
+extern int tint_end_value(const Temporal *temp);
+extern int tint_max_value(const Temporal *temp);
+extern int tint_min_value(const Temporal *temp);
+extern int tint_start_value(const Temporal *temp);
+extern int *tint_values(const Temporal *temp, int *count);
+extern SpanSet *tnumber_valuespans(const Temporal *temp);
+extern GSERIALIZED *tpoint_end_value(const Temporal *temp);
+extern GSERIALIZED *tpoint_start_value(const Temporal *temp);
+extern GSERIALIZED **tpoint_values(const Temporal *temp, int *count);
+extern text *ttext_end_value(const Temporal *temp);
+extern text *ttext_max_value(const Temporal *temp);
+extern text *ttext_min_value(const Temporal *temp);
+extern text *ttext_start_value(const Temporal *temp);
+extern text **ttext_values(const Temporal *temp, int *count);
+
+
+
+
+
+extern Temporal *temporal_set_interp(const Temporal *temp, interpType interp);
+extern Temporal *temporal_shift(const Temporal *temp, const Interval *shift);
+extern Temporal *temporal_shift_tscale(const Temporal *temp, const Interval *shift, const Interval *duration);
+extern Temporal *temporal_to_tinstant(const Temporal *temp);
+extern Temporal *temporal_to_tsequence(const Temporal *temp);
+extern Temporal *temporal_to_tsequenceset(const Temporal *temp);
+extern Temporal *temporal_tprecision(const Temporal *temp, const Interval *duration, TimestampTz origin);
+extern Temporal *temporal_tsample(const Temporal *temp, const Interval *duration, TimestampTz origin);
+extern Temporal *temporal_tscale(const Temporal *temp, const Interval *duration);
+
+
+
+
+
+extern Temporal *tbool_at_value(const Temporal *temp, bool b);
+extern Temporal *tbool_minus_value(const Temporal *temp, bool b);
+extern bool tbool_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, bool *value);
+extern Temporal *temporal_at_max(const Temporal *temp);
+extern Temporal *temporal_at_min(const Temporal *temp);
+extern Temporal *temporal_at_period(const Temporal *temp, const Span *p);
+extern Temporal *temporal_at_periodset(const Temporal *temp, const SpanSet *ps);
+extern Temporal *temporal_at_timestamp(const Temporal *temp, TimestampTz t);
+extern Temporal *temporal_at_timestampset(const Temporal *temp, const Set *ts);
+extern Temporal *temporal_at_values(const Temporal *temp, const Set *set);
+extern Temporal *temporal_minus_max(const Temporal *temp);
+extern Temporal *temporal_minus_min(const Temporal *temp);
+extern Temporal *temporal_minus_period(const Temporal *temp, const Span *p);
+extern Temporal *temporal_minus_periodset(const Temporal *temp, const SpanSet *ps);
+extern Temporal *temporal_minus_timestamp(const Temporal *temp, TimestampTz t);
+extern Temporal *temporal_minus_timestampset(const Temporal *temp, const Set *ts);
+extern Temporal *temporal_minus_values(const Temporal *temp, const Set *set);
+extern Temporal *tfloat_at_value(const Temporal *temp, double d);
+extern Temporal *tfloat_minus_value(const Temporal *temp, double d);
+extern bool tfloat_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, double *value);
+extern Temporal *tint_at_value(const Temporal *temp, int i);
+extern Temporal *tint_minus_value(const Temporal *temp, int i);
+extern bool tint_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, int *value);
+extern Temporal *tnumber_at_span(const Temporal *temp, const Span *span);
+extern Temporal *tnumber_at_spanset(const Temporal *temp, const SpanSet *ss);
+extern Temporal *tnumber_at_tbox(const Temporal *temp, const TBox *box);
+extern Temporal *tnumber_minus_span(const Temporal *temp, const Span *span);
+extern Temporal *tnumber_minus_spanset(const Temporal *temp, const SpanSet *ss);
+extern Temporal *tnumber_minus_tbox(const Temporal *temp, const TBox *box);
+extern Temporal *tpoint_at_geom_time(const Temporal *temp, const GSERIALIZED *gs, const Span *zspan, const Span *period);
+extern Temporal *tpoint_at_stbox(const Temporal *temp, const STBox *box, bool border_inc);
+extern Temporal *tpoint_at_value(const Temporal *temp, GSERIALIZED *gs);
+extern Temporal *tpoint_minus_geom_time(const Temporal *temp, const GSERIALIZED *gs, const Span *zspan, const Span *period);
+extern Temporal *tpoint_minus_stbox(const Temporal *temp, const STBox *box, bool border_inc);
+extern Temporal *tpoint_minus_value(const Temporal *temp, GSERIALIZED *gs);
+extern bool tpoint_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, GSERIALIZED **value);
+extern Temporal *ttext_at_value(const Temporal *temp, text *txt);
+extern Temporal *ttext_minus_value(const Temporal *temp, text *txt);
+extern bool ttext_value_at_timestamp(const Temporal *temp, TimestampTz t, bool strict, text **value);
+
+
+
+
+
+extern Temporal *temporal_append_tinstant(Temporal *temp, const TInstant *inst, double maxdist, Interval *maxt, bool expand);
+extern Temporal *temporal_append_tsequence(Temporal *temp, const TSequence *seq, bool expand);
+extern Temporal *temporal_delete_period(const Temporal *temp, const Span *p, bool connect);
+extern Temporal *temporal_delete_periodset(const Temporal *temp, const SpanSet *ps, bool connect);
+extern Temporal *temporal_delete_timestamp(const Temporal *temp, TimestampTz t, bool connect);
+extern Temporal *temporal_delete_timestampset(const Temporal *temp, const Set *ts, bool connect);
+extern Temporal *temporal_insert(const Temporal *temp1, const Temporal *temp2, bool connect);
+extern Temporal *temporal_merge(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *temporal_merge_array(Temporal **temparr, int count);
+extern Temporal *temporal_update(const Temporal *temp1, const Temporal *temp2, bool connect);
+
+
+
+
+
+extern Temporal *tand_bool_tbool(bool b, const Temporal *temp);
+extern Temporal *tand_tbool_bool(const Temporal *temp, bool b);
+extern Temporal *tand_tbool_tbool(const Temporal *temp1, const Temporal *temp2);
+extern SpanSet *tbool_when_true(const Temporal *temp);
+extern Temporal *tnot_tbool(const Temporal *temp);
+extern Temporal *tor_bool_tbool(bool b, const Temporal *temp);
+extern Temporal *tor_tbool_bool(const Temporal *temp, bool b);
+extern Temporal *tor_tbool_tbool(const Temporal *temp1, const Temporal *temp2);
+
+
+
+
+
+extern Temporal *add_float_tfloat(double d, const Temporal *tnumber);
+extern Temporal *add_int_tint(int i, const Temporal *tnumber);
+extern Temporal *add_tfloat_float(const Temporal *tnumber, double d);
+extern Temporal *add_tint_int(const Temporal *tnumber, int i);
+extern Temporal *add_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
+extern Temporal *div_float_tfloat(double d, const Temporal *tnumber);
+extern Temporal *div_int_tint(int i, const Temporal *tnumber);
+extern Temporal *div_tfloat_float(const Temporal *tnumber, double d);
+extern Temporal *div_tint_int(const Temporal *tnumber, int i);
+extern Temporal *div_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
+extern double float_degrees(double value, bool normalize);
+extern Temporal *mult_float_tfloat(double d, const Temporal *tnumber);
+extern Temporal *mult_int_tint(int i, const Temporal *tnumber);
+extern Temporal *mult_tfloat_float(const Temporal *tnumber, double d);
+extern Temporal *mult_tint_int(const Temporal *tnumber, int i);
+extern Temporal *mult_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
+extern Temporal *sub_float_tfloat(double d, const Temporal *tnumber);
+extern Temporal *sub_int_tint(int i, const Temporal *tnumber);
+extern Temporal *sub_tfloat_float(const Temporal *tnumber, double d);
+extern Temporal *sub_tint_int(const Temporal *tnumber, int i);
+extern Temporal *sub_tnumber_tnumber(const Temporal *tnumber1, const Temporal *tnumber2);
+extern Temporal *tfloat_degrees(const Temporal *temp, bool normalize);
+extern Temporal *tfloat_derivative(const Temporal *temp);
+extern Temporal *tfloat_radians(const Temporal *temp);
+extern Temporal *tnumber_abs(const Temporal *temp);
+extern Temporal *tnumber_angular_difference(const Temporal *temp);
+extern Temporal *tnumber_delta_value(const Temporal *temp);
+
+
+
+
+
+extern Temporal *textcat_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *textcat_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *textcat_ttext_ttext(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *ttext_upper(const Temporal *temp);
+extern Temporal *ttext_lower(const Temporal *temp);
+
+
+
+
+
+extern Temporal *distance_tfloat_float(const Temporal *temp, double d);
+extern Temporal *distance_tint_int(const Temporal *temp, int i);
+extern Temporal *distance_tnumber_tnumber(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *distance_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo);
+extern Temporal *distance_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern double nad_stbox_geo(const STBox *box, const GSERIALIZED *gs);
+extern double nad_stbox_stbox(const STBox *box1, const STBox *box2);
+extern double nad_tbox_tbox(const TBox *box1, const TBox *box2);
+extern double nad_tfloat_float(const Temporal *temp, double d);
+extern double nad_tfloat_tfloat(const Temporal *temp1, const Temporal *temp2);
+extern int nad_tint_int(const Temporal *temp, int i);
+extern int nad_tint_tint(const Temporal *temp1, const Temporal *temp2);
+extern double nad_tnumber_tbox(const Temporal *temp, const TBox *box);
+extern double nad_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
+extern double nad_tpoint_stbox(const Temporal *temp, const STBox *box);
+extern double nad_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern TInstant *nai_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
+extern TInstant *nai_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern bool shortestline_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, GSERIALIZED **result);
+extern bool shortestline_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, GSERIALIZED **result);
+
+
+
+
+
+extern bool tbool_always_eq(const Temporal *temp, bool b);
+extern bool tbool_ever_eq(const Temporal *temp, bool b);
+extern bool tfloat_always_eq(const Temporal *temp, double d);
+extern bool tfloat_always_le(const Temporal *temp, double d);
+extern bool tfloat_always_lt(const Temporal *temp, double d);
+extern bool tfloat_ever_eq(const Temporal *temp, double d);
+extern bool tfloat_ever_le(const Temporal *temp, double d);
+extern bool tfloat_ever_lt(const Temporal *temp, double d);
+extern bool tgeogpoint_always_eq(const Temporal *temp, GSERIALIZED *gs);;
+extern bool tgeogpoint_ever_eq(const Temporal *temp, GSERIALIZED *gs);;
+extern bool tgeompoint_always_eq(const Temporal *temp, GSERIALIZED *gs);
+extern bool tgeompoint_ever_eq(const Temporal *temp, GSERIALIZED *gs);;
+extern bool tint_always_eq(const Temporal *temp, int i);
+extern bool tint_always_le(const Temporal *temp, int i);
+extern bool tint_always_lt(const Temporal *temp, int i);
+extern bool tint_ever_eq(const Temporal *temp, int i);
+extern bool tint_ever_le(const Temporal *temp, int i);
+extern bool tint_ever_lt(const Temporal *temp, int i);
+extern bool tpoint_always_eq(const Temporal *temp, Datum value);
+extern bool tpoint_ever_eq(const Temporal *temp, Datum value);
+extern bool ttext_always_eq(const Temporal *temp, text *txt);
+extern bool ttext_always_le(const Temporal *temp, text *txt);
+extern bool ttext_always_lt(const Temporal *temp, text *txt);
+extern bool ttext_ever_eq(const Temporal *temp, text *txt);
+extern bool ttext_ever_le(const Temporal *temp, text *txt);
+extern bool ttext_ever_lt(const Temporal *temp, text *txt);
+
+
+
+
+
+extern int temporal_cmp(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_eq(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_ge(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_gt(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_le(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_lt(const Temporal *temp1, const Temporal *temp2);
+extern bool temporal_ne(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *teq_bool_tbool(bool b, const Temporal *temp);
+extern Temporal *teq_float_tfloat(double d, const Temporal *temp);
+extern Temporal *teq_geo_tpoint(const GSERIALIZED *geo, const Temporal *tpoint);
+extern Temporal *teq_int_tint(int i, const Temporal *temp);
+extern Temporal *teq_point_tgeogpoint(const GSERIALIZED *gs, const Temporal *temp);
+extern Temporal *teq_point_tgeompoint(const GSERIALIZED *gs, const Temporal *temp);
+extern Temporal *teq_tbool_bool(const Temporal *temp, bool b);
+extern Temporal *teq_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *teq_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *teq_tfloat_float(const Temporal *temp, double d);
+extern Temporal *teq_tgeogpoint_point(const Temporal *temp, const GSERIALIZED *gs);
+extern Temporal *teq_tgeompoint_point(const Temporal *temp, const GSERIALIZED *gs);
+extern Temporal *teq_tint_int(const Temporal *temp, int i);
+extern Temporal *teq_tpoint_geo(const Temporal *tpoint, const GSERIALIZED *geo);
+extern Temporal *teq_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *tge_float_tfloat(double d, const Temporal *temp);
+extern Temporal *tge_int_tint(int i, const Temporal *temp);
+extern Temporal *tge_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tge_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *tge_tfloat_float(const Temporal *temp, double d);
+extern Temporal *tge_tint_int(const Temporal *temp, int i);
+extern Temporal *tge_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *tgt_float_tfloat(double d, const Temporal *temp);
+extern Temporal *tgt_int_tint(int i, const Temporal *temp);
+extern Temporal *tgt_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tgt_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *tgt_tfloat_float(const Temporal *temp, double d);
+extern Temporal *tgt_tint_int(const Temporal *temp, int i);
+extern Temporal *tgt_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *tle_float_tfloat(double d, const Temporal *temp);
+extern Temporal *tle_int_tint(int i, const Temporal *temp);
+extern Temporal *tle_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tle_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *tle_tfloat_float(const Temporal *temp, double d);
+extern Temporal *tle_tint_int(const Temporal *temp, int i);
+extern Temporal *tle_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *tlt_float_tfloat(double d, const Temporal *temp);
+extern Temporal *tlt_int_tint(int i, const Temporal *temp);
+extern Temporal *tlt_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tlt_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *tlt_tfloat_float(const Temporal *temp, double d);
+extern Temporal *tlt_tint_int(const Temporal *temp, int i);
+extern Temporal *tlt_ttext_text(const Temporal *temp, const text *txt);
+extern Temporal *tne_bool_tbool(bool b, const Temporal *temp);
+extern Temporal *tne_float_tfloat(double d, const Temporal *temp);
+extern Temporal *tne_geo_tpoint(const GSERIALIZED *geo, const Temporal *tpoint);
+extern Temporal *tne_int_tint(int i, const Temporal *temp);
+extern Temporal *tne_point_tgeogpoint(const GSERIALIZED *gs, const Temporal *temp);
+extern Temporal *tne_point_tgeompoint(const GSERIALIZED *gs, const Temporal *temp);
+extern Temporal *tne_tbool_bool(const Temporal *temp, bool b);
+extern Temporal *tne_temporal_temporal(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tne_text_ttext(const text *txt, const Temporal *temp);
+extern Temporal *tne_tfloat_float(const Temporal *temp, double d);
+extern Temporal *tne_tgeogpoint_point(const Temporal *temp, const GSERIALIZED *gs);
+extern Temporal *tne_tgeompoint_point(const Temporal *temp, const GSERIALIZED *gs);
+extern Temporal *tne_tint_int(const Temporal *temp, int i);
+extern Temporal *tne_tpoint_geo(const Temporal *tpoint, const GSERIALIZED *geo);
+extern Temporal *tne_ttext_text(const Temporal *temp, const text *txt);
+
+/*****************************************************************************
+  Spatial functions for temporal point types
+ *****************************************************************************/
+
+
+
+extern bool bearing_point_point(const GSERIALIZED *geo1, const GSERIALIZED *geo2, double *result);
+extern Temporal *bearing_tpoint_point(const Temporal *temp, const GSERIALIZED *gs, bool invert);
+extern Temporal *bearing_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern Temporal *tpoint_angular_difference(const Temporal *temp);
+extern Temporal *tpoint_azimuth(const Temporal *temp);
+extern GSERIALIZED *tpoint_convex_hull(const Temporal *temp);
+extern Temporal *tpoint_cumulative_length(const Temporal *temp);
+extern bool tpoint_direction(const Temporal *temp, double *result);
+extern Temporal *tpoint_get_coord(const Temporal *temp, int coord);
+extern bool tpoint_is_simple(const Temporal *temp);
+extern double tpoint_length(const Temporal *temp);
+extern Temporal *tpoint_speed(const Temporal *temp);
+extern int tpoint_srid(const Temporal *temp);
+extern STBox *tpoint_stboxes(const Temporal *temp, int *count);
+extern GSERIALIZED *tpoint_trajectory(const Temporal *temp);
+
+
+
+
+
+extern STBox *geo_expand_space(const GSERIALIZED *gs, double d);
+extern Temporal *tgeompoint_tgeogpoint(const Temporal *temp, bool oper);
+extern STBox *tpoint_expand_space(const Temporal *temp, double d);
+extern Temporal **tpoint_make_simple(const Temporal *temp, int *count);
+extern Temporal *tpoint_set_srid(const Temporal *temp, int32 srid);
+
+
+
+
+
+extern int econtains_geo_tpoint(const GSERIALIZED *geo, const Temporal *temp);
+extern int edisjoint_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
+extern int edisjoint_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern int edwithin_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, double dist);
+extern int edwithin_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, double dist);
+extern int eintersects_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
+extern int eintersects_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2);
+extern int etouches_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs);
+extern Temporal *tcontains_geo_tpoint(const GSERIALIZED *gs, const Temporal *temp, bool restr, bool atvalue);
+extern Temporal *tdisjoint_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo, bool restr, bool atvalue);
+extern Temporal *tdwithin_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, double dist, bool restr, bool atvalue);
+extern Temporal *tdwithin_tpoint_tpoint(const Temporal *temp1, const Temporal *temp2, double dist, bool restr, bool atvalue);
+extern Temporal *tintersects_tpoint_geo(const Temporal *temp, const GSERIALIZED *geo, bool restr, bool atvalue);
+extern Temporal *ttouches_tpoint_geo(const Temporal *temp, const GSERIALIZED *gs, bool restr, bool atvalue);
+
+
+
+
+
+extern SkipList *tbool_tand_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tbool_tor_transfn(SkipList *state, const Temporal *temp);
+extern Span *temporal_extent_transfn(Span *p, const Temporal *temp);
+extern Temporal *temporal_tagg_finalfn(SkipList *state);
+extern SkipList *temporal_tcount_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tfloat_tmax_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tfloat_tmin_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tfloat_tsum_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tint_tmax_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tint_tmin_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *tint_tsum_transfn(SkipList *state, const Temporal *temp);
+extern TBox *tnumber_extent_transfn(TBox *box, const Temporal *temp);
+extern double tnumber_integral(const Temporal *temp);
+extern Temporal *tnumber_tavg_finalfn(SkipList *state);
+extern SkipList *tnumber_tavg_transfn(SkipList *state, const Temporal *temp);
+extern double tnumber_twavg(const Temporal *temp);
+extern STBox *tpoint_extent_transfn(STBox *box, const Temporal *temp);
+extern Temporal *tpoint_tcentroid_finalfn(SkipList *state);
+extern SkipList *tpoint_tcentroid_transfn(SkipList *state, Temporal *temp);
+extern GSERIALIZED *tpoint_twcentroid(const Temporal *temp);
+extern SkipList *ttext_tmax_transfn(SkipList *state, const Temporal *temp);
+extern SkipList *ttext_tmin_transfn(SkipList *state, const Temporal *temp);
+
+
+
+
+
+extern double float_bucket(double value, double size, double origin);
+extern Span *floatspan_bucket_list(const Span *bounds, double size, double origin, int *newcount);
+extern int int_bucket(int value, int size, int origin);
+extern Span *intspan_bucket_list(const Span *bounds, int size, int origin, int *newcount);
+extern Span *period_bucket_list(const Span *bounds, const Interval *duration, TimestampTz origin, int *newcount);
+extern STBox *stbox_tile_list(const STBox *bounds, double xsize, double ysize, double zsize, const Interval *duration, GSERIALIZED *sorigin, TimestampTz torigin, int **cellcount);
+extern TBox *tbox_tile_list(const TBox *bounds, double xsize, const Interval *duration, double xorigin, TimestampTz torigin, int *rows, int *columns);
+extern Temporal **temporal_time_split(Temporal *temp, Interval *duration, TimestampTz torigin, int *newcount);
+extern Temporal **tfloat_value_split(Temporal *temp, double size, double origin, int *newcount);
+extern Temporal **tfloat_value_time_split(Temporal *temp, double size, double vorigin, Interval *duration, TimestampTz torigin, int *newcount);
+extern TimestampTz timestamptz_bucket(TimestampTz timestamp, const Interval *duration, TimestampTz origin);
+extern Temporal **tint_value_split(Temporal *temp, int size, int origin, int *newcount);
+extern Temporal **tint_value_time_split(Temporal *temp, int size, int vorigin, Interval *duration, TimestampTz torigin, int *newcount);
+
+
+
+
+
+extern double temporal_dyntimewarp_distance(const Temporal *temp1, const Temporal *temp2);
+extern Match *temporal_dyntimewarp_path(const Temporal *temp1, const Temporal *temp2, int *count);
+extern double temporal_frechet_distance(const Temporal *temp1, const Temporal *temp2);
+extern Match *temporal_frechet_path(const Temporal *temp1, const Temporal *temp2, int *count);
+extern double temporal_hausdorff_distance(const Temporal *temp1, const Temporal *temp2);
+
+
+
+
+
+Temporal *geo_to_tpoint(const GSERIALIZED *geo);
+Temporal *temporal_simplify_min_dist(const Temporal *temp, double dist);
+Temporal *temporal_simplify_min_tdelta(const Temporal *temp, const Interval *mint);
+Temporal *temporal_simplify_dp(const Temporal *temp, double eps_dist, bool synchronized);
+Temporal *temporal_simplify_max_dist(const Temporal *temp, double eps_dist, bool synchronized);
+bool tpoint_AsMVTGeom(const Temporal *temp, const STBox *bounds, int32_t extent, int32_t buffer, bool clip_geom, GSERIALIZED **geom, int64 **timesarr, int *count);
+bool tpoint_to_geo_meas(const Temporal *tpoint, const Temporal *measure, bool segmentize, GSERIALIZED **result);
+
+
+
+//#endif
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/builder/objects.py` & `pymeos_cffi-1.1.0a2/pymeos_cffi/builder/objects.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Callable, Dict, Optional
-
-
-class Conversion:
-
-    def __init__(self, c_type: str, p_type: str, p_to_c: Optional[Callable[[str], str]],
-                 c_to_p: Optional[Callable[[str], str]]) -> None:
-        super().__init__()
-        self.c_type = c_type
-        self.p_type = p_type
-        self.p_to_c = p_to_c
-        self.c_to_p = c_to_p
-
-
-conversion_map: Dict[str, Conversion] = {
-    'void': Conversion('void', 'None', None, None),
-    'bool': Conversion('bool', 'bool', None, None),
-    'double': Conversion('double', 'float', None, None),
-    'char *': Conversion('char *', 'str', lambda p_obj: f"{p_obj}.encode('utf-8')",
-                         lambda c_obj: f"_ffi.string({c_obj}).decode('utf-8')"),
-    'const char *': Conversion('const char *', 'str', lambda p_obj: f"{p_obj}.encode('utf-8')",
-                               lambda c_obj: f"_ffi.string({c_obj}).decode('utf-8')"),
-    'text': Conversion('text', 'str', lambda p_obj: f"cstring2text({p_obj})", lambda c_obj: f"text2cstring({c_obj})"),
-    'text *': Conversion('text *', 'str', lambda p_obj: f"cstring2text({p_obj})",
-                         lambda c_obj: f"text2cstring({c_obj})"),
-    'const text': Conversion('const text', 'str', lambda p_obj: f"cstring2text({p_obj})",
-                             lambda c_obj: f"text2cstring({c_obj})"),
-    'const text *': Conversion('const text *', 'str', lambda p_obj: f"cstring2text({p_obj})",
-                               lambda c_obj: f"text2cstring({c_obj})"),
-    'int': Conversion('int', 'int', None, None),
-    'int8': Conversion('int8', 'int', lambda p_obj: f"_ffi.cast('int8', {p_obj})", None),
-    'int16': Conversion('int16', 'int', lambda p_obj: f"_ffi.cast('int16', {p_obj})", None),
-    'int32': Conversion('int32', 'int', lambda p_obj: f"_ffi.cast('int32', {p_obj})", None),
-    'int64': Conversion('int64', 'int', lambda p_obj: f"_ffi.cast('int64', {p_obj})", None),
-    'uint8': Conversion('uint8', 'int', lambda p_obj: f"_ffi.cast('uint8', {p_obj})", None),
-    'uint16': Conversion('uint16', 'int', lambda p_obj: f"_ffi.cast('uint16', {p_obj})", None),
-    'uint32': Conversion('uint32', 'int', lambda p_obj: f"_ffi.cast('uint32', {p_obj})", None),
-    'uint64': Conversion('uint64', 'int', lambda p_obj: f"_ffi.cast('uint64', {p_obj})", None),
-    'uint8_t': Conversion('uint8_t', 'int', lambda p_obj: f"_ffi.cast('uint8_t', {p_obj})", None),
-    'Timestamp': Conversion('Timestamp', 'int', lambda p_obj: f"_ffi.cast('Timestamp', {p_obj})", None),
-    'TimestampTz': Conversion('TimestampTz', 'int', lambda p_obj: f"_ffi.cast('TimestampTz', {p_obj})", None),
-    'TimestampTz *': Conversion('TimestampTz *', 'int', lambda p_obj: f"_ffi.cast('TimestampTz *', {p_obj})", None),
-    'const TimestampTz': Conversion('const TimestampTz', 'int',
-                                    lambda p_obj: f"_ffi.cast('const TimestampTz', {p_obj})", None),
-    'const TimestampTz *': Conversion('const TimestampTz *', 'int',
-                                      lambda p_obj: f"_ffi.cast('const TimestampTz *', {p_obj})", None),
-    'TimeOffset': Conversion('TimeOffset', 'int', lambda p_obj: f"_ffi.cast('TimeOffset', {p_obj})", None),
-}
+from typing import Callable, Dict, Optional
+
+
+class Conversion:
+
+    def __init__(self, c_type: str, p_type: str, p_to_c: Optional[Callable[[str], str]],
+                 c_to_p: Optional[Callable[[str], str]]) -> None:
+        super().__init__()
+        self.c_type = c_type
+        self.p_type = p_type
+        self.p_to_c = p_to_c
+        self.c_to_p = c_to_p
+
+
+conversion_map: Dict[str, Conversion] = {
+    'void': Conversion('void', 'None', None, None),
+    'bool': Conversion('bool', 'bool', None, None),
+    'double': Conversion('double', 'float', None, None),
+    'char *': Conversion('char *', 'str', lambda p_obj: f"{p_obj}.encode('utf-8')",
+                         lambda c_obj: f"_ffi.string({c_obj}).decode('utf-8')"),
+    'const char *': Conversion('const char *', 'str', lambda p_obj: f"{p_obj}.encode('utf-8')",
+                               lambda c_obj: f"_ffi.string({c_obj}).decode('utf-8')"),
+    'text': Conversion('text', 'str', lambda p_obj: f"cstring2text({p_obj})", lambda c_obj: f"text2cstring({c_obj})"),
+    'text *': Conversion('text *', 'str', lambda p_obj: f"cstring2text({p_obj})",
+                         lambda c_obj: f"text2cstring({c_obj})"),
+    'const text': Conversion('const text', 'str', lambda p_obj: f"cstring2text({p_obj})",
+                             lambda c_obj: f"text2cstring({c_obj})"),
+    'const text *': Conversion('const text *', 'str', lambda p_obj: f"cstring2text({p_obj})",
+                               lambda c_obj: f"text2cstring({c_obj})"),
+    'int': Conversion('int', 'int', None, None),
+    'int8': Conversion('int8', 'int', lambda p_obj: f"_ffi.cast('int8', {p_obj})", None),
+    'int16': Conversion('int16', 'int', lambda p_obj: f"_ffi.cast('int16', {p_obj})", None),
+    'int32': Conversion('int32', 'int', lambda p_obj: f"_ffi.cast('int32', {p_obj})", None),
+    'int64': Conversion('int64', 'int', lambda p_obj: f"_ffi.cast('int64', {p_obj})", None),
+    'uint8': Conversion('uint8', 'int', lambda p_obj: f"_ffi.cast('uint8', {p_obj})", None),
+    'uint16': Conversion('uint16', 'int', lambda p_obj: f"_ffi.cast('uint16', {p_obj})", None),
+    'uint32': Conversion('uint32', 'int', lambda p_obj: f"_ffi.cast('uint32', {p_obj})", None),
+    'uint64': Conversion('uint64', 'int', lambda p_obj: f"_ffi.cast('uint64', {p_obj})", None),
+    'uint8_t': Conversion('uint8_t', 'int', lambda p_obj: f"_ffi.cast('uint8_t', {p_obj})", None),
+    'Timestamp': Conversion('Timestamp', 'int', lambda p_obj: f"_ffi.cast('Timestamp', {p_obj})", None),
+    'TimestampTz': Conversion('TimestampTz', 'int', lambda p_obj: f"_ffi.cast('TimestampTz', {p_obj})", None),
+    'TimestampTz *': Conversion('TimestampTz *', 'int', lambda p_obj: f"_ffi.cast('TimestampTz *', {p_obj})", None),
+    'const TimestampTz': Conversion('const TimestampTz', 'int',
+                                    lambda p_obj: f"_ffi.cast('const TimestampTz', {p_obj})", None),
+    'const TimestampTz *': Conversion('const TimestampTz *', 'int',
+                                      lambda p_obj: f"_ffi.cast('const TimestampTz *', {p_obj})", None),
+    'TimeOffset': Conversion('TimeOffset', 'int', lambda p_obj: f"_ffi.cast('TimeOffset', {p_obj})", None),
+}
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi/functions.py` & `pymeos_cffi-1.1.0a2/pymeos_cffi/functions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,6126 +1,6126 @@
-from datetime import datetime, timedelta
-from typing import Any, Tuple, Optional, List, Union
-
-import _meos_cffi
-import postgis as pg
-import shapely.geometry as spg
-from dateutil.parser import parse
-from shapely import wkt, wkb, get_srid
-from shapely.geometry.base import BaseGeometry
-from spans.types import floatrange, intrange
-
-_ffi = _meos_cffi.ffi
-_lib = _meos_cffi.lib
-
-
-def create_pointer(object: 'Any', type: str) -> 'Any *':
-    return _ffi.new(f'{type} *', object)
-    
-
-def get_address(value: 'Any') -> 'Any *':
-    return _ffi.addressof(value)
-
-
-def datetime_to_timestamptz(dt: datetime) -> int:
-    return _lib.pg_timestamptz_in(dt.strftime('%Y-%m-%d %H:%M:%S%z').encode('utf-8'), -1)
-
-
-def timestamptz_to_datetime(ts: int) -> datetime:
-    return parse(pg_timestamptz_out(ts))
-
-
-def timedelta_to_interval(td: timedelta) -> Any:
-    return _ffi.new('Interval *', {'time': td.microseconds + td.seconds * 1000000, 'day': td.days, 'month': 0})
-
-
-def interval_to_timedelta(interval: Any) -> timedelta:
-    # TODO fix for months/years
-    return timedelta(days=interval.day, microseconds=interval.time)
-
-
-def geometry_to_gserialized(geom: Union[pg.Geometry, BaseGeometry], geodetic: Optional[bool] = None) -> 'GSERIALIZED *':
-    if isinstance(geom, pg.Geometry):
-        text = geom.to_ewkb()
-        if geom.has_srid():
-            text = f'SRID={geom.srid};{text}'
-    elif isinstance(geom, BaseGeometry):
-        text = wkb.dumps(geom, hex=True)
-        if get_srid(geom) > 0:
-            text = f'SRID={get_srid(geom)};{text}'
-    else:
-        raise TypeError('Parameter geom must be either a PostGIS Geometry or a Shapely BaseGeometry')
-    gs = gserialized_in(text, -1)
-    if geodetic is not None:
-        # GFlags is an 8-bit integer, where the 4th bit is the geodetic flag (0x80)
-        # If geodetic is True, then set the 4th bit to 1, otherwise set it to 0
-        gs.gflags = (gs.gflags | 0x08) if geodetic else (gs.gflags & 0xF7)
-    return gs
-
-
-def gserialized_to_shapely_point(geom: 'const GSERIALIZED *', precision: int = 6) -> spg.Point:
-    return wkt.loads(gserialized_as_text(geom, precision))
-
-
-def gserialized_to_shapely_geometry(geom: 'const GSERIALIZED *', precision: int = 6) -> BaseGeometry:
-    return wkt.loads(gserialized_as_text(geom, precision))
-
-
-def intrange_to_intspan(irange: intrange) -> 'Span *':
-    return intspan_make(irange.lower, irange.upper, irange.lower_inc, irange.upper_inc)
-
-
-def intspan_to_intrange(ispan: 'Span *') -> intrange:
-    return intrange(intspan_lower(ispan), intspan_upper(ispan), ispan.lower_inc, ispan.upper_inc)
-
-
-def floatrange_to_floatspan(frange: floatrange) -> 'Span *':
-    return floatspan_make(frange.lower, frange.upper, frange.lower_inc, frange.upper_inc)
-
-
-def floatspan_to_floatrange(fspan: 'Span *') -> floatrange:
-    return floatrange(floatspan_lower(fspan), floatspan_upper(fspan), fspan.lower_inc, fspan.upper_inc)
-
-
-def as_tinstant(temporal: 'Temporal *') -> 'TInstant *':
-    return _ffi.cast('TInstant *', temporal)
-
-
-def as_tsequence(temporal: 'Temporal *') -> 'TSequence *':
-    return _ffi.cast('TSequence *', temporal)
-
-
-def as_tsequenceset(temporal: 'Temporal *') -> 'TSequenceSet *':
-    return _ffi.cast('TSequenceSet *', temporal)
-
-
-# -----------------------------------------------------------------------------
-# ----------------------End of manually-defined functions----------------------
-# -----------------------------------------------------------------------------
-
-
-def lwpoint_make(srid: 'int32_t', hasz: int, hasm: int, p: 'const POINT4D *') -> 'LWPOINT *':
-    srid_converted = _ffi.cast('int32_t', srid)
-    p_converted = _ffi.cast('const POINT4D *', p)
-    result = _lib.lwpoint_make(srid_converted, hasz, hasm, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwgeom_from_gserialized(g: 'const GSERIALIZED *') -> 'LWGEOM *':
-    g_converted = _ffi.cast('const GSERIALIZED *', g)
-    result = _lib.lwgeom_from_gserialized(g_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_from_lwgeom(geom: 'LWGEOM *') -> 'GSERIALIZED *':
-    geom_converted = _ffi.cast('LWGEOM *', geom)
-    size_converted = _ffi.NULL
-    result = _lib.gserialized_from_lwgeom(geom_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwgeom_get_srid(geom: 'const LWGEOM *') -> 'int32_t':
-    geom_converted = _ffi.cast('const LWGEOM *', geom)
-    result = _lib.lwgeom_get_srid(geom_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwpoint_get_x(point: 'const LWPOINT *') -> 'double':
-    point_converted = _ffi.cast('const LWPOINT *', point)
-    result = _lib.lwpoint_get_x(point_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwpoint_get_y(point: 'const LWPOINT *') -> 'double':
-    point_converted = _ffi.cast('const LWPOINT *', point)
-    result = _lib.lwpoint_get_y(point_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwpoint_get_z(point: 'const LWPOINT *') -> 'double':
-    point_converted = _ffi.cast('const LWPOINT *', point)
-    result = _lib.lwpoint_get_z(point_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwpoint_get_m(point: 'const LWPOINT *') -> 'double':
-    point_converted = _ffi.cast('const LWPOINT *', point)
-    result = _lib.lwpoint_get_m(point_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwgeom_has_z(geom: 'const LWGEOM *') -> 'int':
-    geom_converted = _ffi.cast('const LWGEOM *', geom)
-    result = _lib.lwgeom_has_z(geom_converted)
-    return result if result != _ffi.NULL else None
-
-
-def lwgeom_has_m(geom: 'const LWGEOM *') -> 'int':
-    geom_converted = _ffi.cast('const LWGEOM *', geom)
-    result = _lib.lwgeom_has_m(geom_converted)
-    return result if result != _ffi.NULL else None
-
-
-def meos_initialize(tz_str: "Optional[str]") -> None:
-    tz_str_converted = tz_str.encode('utf-8') if tz_str is not None else _ffi.NULL
-    _lib.meos_initialize(tz_str_converted)
-
-
-def meos_finalize() -> None:
-    _lib.meos_finalize()
-
-
-def bool_in(in_str: str) -> 'bool':
-    in_str_converted = in_str.encode('utf-8')
-    result = _lib.bool_in(in_str_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bool_out(b: bool) -> str:
-    result = _lib.bool_out(b)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def cstring2text(cstring: str) -> 'text *':
-    cstring_converted = cstring.encode('utf-8')
-    result = _lib.cstring2text(cstring_converted)
-    return result
-
-
-def pg_date_in(string: str) -> 'DateADT':
-    string_converted = string.encode('utf-8')
-    result = _lib.pg_date_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_date_out(date: 'DateADT') -> str:
-    date_converted = _ffi.cast('DateADT', date)
-    result = _lib.pg_date_out(date_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_cmp(interval1: 'const Interval *', interval2: 'const Interval *') -> 'int':
-    interval1_converted = _ffi.cast('const Interval *', interval1)
-    interval2_converted = _ffi.cast('const Interval *', interval2)
-    result = _lib.pg_interval_cmp(interval1_converted, interval2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_in(string: str, typmod: int) -> 'Interval *':
-    string_converted = string.encode('utf-8')
-    typmod_converted = _ffi.cast('int32', typmod)
-    result = _lib.pg_interval_in(string_converted, typmod_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_make(years: int, months: int, weeks: int, days: int, hours: int, mins: int, secs: float) -> 'Interval *':
-    years_converted = _ffi.cast('int32', years)
-    months_converted = _ffi.cast('int32', months)
-    weeks_converted = _ffi.cast('int32', weeks)
-    days_converted = _ffi.cast('int32', days)
-    hours_converted = _ffi.cast('int32', hours)
-    mins_converted = _ffi.cast('int32', mins)
-    result = _lib.pg_interval_make(years_converted, months_converted, weeks_converted, days_converted, hours_converted, mins_converted, secs)
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_mul(span: 'const Interval *', factor: float) -> 'Interval *':
-    span_converted = _ffi.cast('const Interval *', span)
-    result = _lib.pg_interval_mul(span_converted, factor)
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_out(span: 'const Interval *') -> str:
-    span_converted = _ffi.cast('const Interval *', span)
-    result = _lib.pg_interval_out(span_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def pg_interval_pl(span1: 'const Interval *', span2: 'const Interval *') -> 'Interval *':
-    span1_converted = _ffi.cast('const Interval *', span1)
-    span2_converted = _ffi.cast('const Interval *', span2)
-    result = _lib.pg_interval_pl(span1_converted, span2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_time_in(string: str, typmod: int) -> 'TimeADT':
-    string_converted = string.encode('utf-8')
-    typmod_converted = _ffi.cast('int32', typmod)
-    result = _lib.pg_time_in(string_converted, typmod_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_time_out(time: 'TimeADT') -> str:
-    time_converted = _ffi.cast('TimeADT', time)
-    result = _lib.pg_time_out(time_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamp_in(string: str, typmod: int) -> 'Timestamp':
-    string_converted = string.encode('utf-8')
-    typmod_converted = _ffi.cast('int32', typmod)
-    result = _lib.pg_timestamp_in(string_converted, typmod_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamp_mi(dt1: int, dt2: int) -> 'Interval *':
-    dt1_converted = _ffi.cast('TimestampTz', dt1)
-    dt2_converted = _ffi.cast('TimestampTz', dt2)
-    result = _lib.pg_timestamp_mi(dt1_converted, dt2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamp_mi_interval(timestamp: int, span: 'const Interval *') -> 'TimestampTz':
-    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
-    span_converted = _ffi.cast('const Interval *', span)
-    result = _lib.pg_timestamp_mi_interval(timestamp_converted, span_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamp_out(dt: int) -> str:
-    dt_converted = _ffi.cast('Timestamp', dt)
-    result = _lib.pg_timestamp_out(dt_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamp_pl_interval(timestamp: int, span: 'const Interval *') -> 'TimestampTz':
-    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
-    span_converted = _ffi.cast('const Interval *', span)
-    result = _lib.pg_timestamp_pl_interval(timestamp_converted, span_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamptz_in(string: str, typmod: int) -> 'TimestampTz':
-    string_converted = string.encode('utf-8')
-    typmod_converted = _ffi.cast('int32', typmod)
-    result = _lib.pg_timestamptz_in(string_converted, typmod_converted)
-    return result if result != _ffi.NULL else None
-
-
-def pg_timestamptz_out(dt: int) -> str:
-    dt_converted = _ffi.cast('TimestampTz', dt)
-    result = _lib.pg_timestamptz_out(dt_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def text2cstring(textptr: 'text *') -> str:
-    result = _lib.text2cstring(textptr)
-    result = _ffi.string(result).decode('utf-8')
-    return result
-
-
-def gserialized_as_ewkb(geom: 'const GSERIALIZED *', type: str) -> 'bytea *':
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    type_converted = type.encode('utf-8')
-    result = _lib.gserialized_as_ewkb(geom_converted, type_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_as_ewkt(geom: 'const GSERIALIZED *', precision: int) -> str:
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    result = _lib.gserialized_as_ewkt(geom_converted, precision)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_as_geojson(geom: 'const GSERIALIZED *', option: int, precision: int, srs: "Optional[str]") -> str:
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    srs_converted = srs.encode('utf-8') if srs is not None else _ffi.NULL
-    result = _lib.gserialized_as_geojson(geom_converted, option, precision, srs_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_as_hexewkb(geom: 'const GSERIALIZED *', type: str) -> str:
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    type_converted = type.encode('utf-8')
-    result = _lib.gserialized_as_hexewkb(geom_converted, type_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_as_text(geom: 'const GSERIALIZED *', precision: int) -> str:
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    result = _lib.gserialized_as_text(geom_converted, precision)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_from_ewkb(bytea_wkb: 'const bytea *', srid: int) -> 'GSERIALIZED *':
-    bytea_wkb_converted = _ffi.cast('const bytea *', bytea_wkb)
-    srid_converted = _ffi.cast('int32', srid)
-    result = _lib.gserialized_from_ewkb(bytea_wkb_converted, srid_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_from_geojson(geojson: str) -> 'GSERIALIZED *':
-    geojson_converted = geojson.encode('utf-8')
-    result = _lib.gserialized_from_geojson(geojson_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_from_hexewkb(wkt: str) -> 'GSERIALIZED *':
-    wkt_converted = wkt.encode('utf-8')
-    result = _lib.gserialized_from_hexewkb(wkt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_from_text(wkt: str, srid: int) -> 'GSERIALIZED *':
-    wkt_converted = wkt.encode('utf-8')
-    result = _lib.gserialized_from_text(wkt_converted, srid)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_in(input: str, geom_typmod: int) -> 'GSERIALIZED *':
-    input_converted = input.encode('utf-8')
-    geom_typmod_converted = _ffi.cast('int32', geom_typmod)
-    result = _lib.gserialized_in(input_converted, geom_typmod_converted)
-    return result if result != _ffi.NULL else None
-
-
-def gserialized_out(geom: 'const GSERIALIZED *') -> str:
-    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
-    result = _lib.gserialized_out(geom_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def pgis_gserialized_same(geom1: 'const GSERIALIZED *', geom2: 'const GSERIALIZED *') -> 'bool':
-    geom1_converted = _ffi.cast('const GSERIALIZED *', geom1)
-    geom2_converted = _ffi.cast('const GSERIALIZED *', geom2)
-    result = _lib.pgis_gserialized_same(geom1_converted, geom2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.bigintset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_out(set: 'const Set *') -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.bigintset_out(set_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def bigintspan_in(string: str) -> 'Span *':
-    string_converted = string.encode('utf-8')
-    result = _lib.bigintspan_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspan_out(s: 'const Span *') -> str:
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.bigintspan_out(s_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def bigintspanset_in(string: str) -> 'SpanSet *':
-    string_converted = string.encode('utf-8')
-    result = _lib.bigintspanset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspanset_out(ss: 'const SpanSet *') -> str:
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.bigintspanset_out(ss_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def floatset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.floatset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatset_out(set: 'const Set *', maxdd: int) -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.floatset_out(set_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_in(string: str) -> 'Span *':
-    string_converted = string.encode('utf-8')
-    result = _lib.floatspan_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_out(s: 'const Span *', maxdd: int) -> str:
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.floatspan_out(s_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def floatspanset_in(string: str) -> 'SpanSet *':
-    string_converted = string.encode('utf-8')
-    result = _lib.floatspanset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspanset_out(ss: 'const SpanSet *', maxdd: int) -> str:
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.floatspanset_out(ss_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def geogset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.geogset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geogset_out(set: 'const Set *', maxdd: int) -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.geogset_out(set_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def geomset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.geomset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geomset_out(set: 'const Set *', maxdd: int) -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.geomset_out(set_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def geoset_as_ewkt(set: 'const Set *', maxdd: int) -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.geoset_as_ewkt(set_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def geoset_as_text(set: 'const Set *', maxdd: int) -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.geoset_as_text(set_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def intset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.intset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intset_out(set: 'const Set *') -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.intset_out(set_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def intspan_in(string: str) -> 'Span *':
-    string_converted = string.encode('utf-8')
-    result = _lib.intspan_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspan_out(s: 'const Span *') -> str:
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.intspan_out(s_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def intspanset_in(string: str) -> 'SpanSet *':
-    string_converted = string.encode('utf-8')
-    result = _lib.intspanset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspanset_out(ss: 'const SpanSet *') -> str:
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.intspanset_out(ss_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def period_in(string: str) -> 'Span *':
-    string_converted = string.encode('utf-8')
-    result = _lib.period_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_out(s: 'const Span *') -> str:
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.period_out(s_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def periodset_in(string: str) -> 'SpanSet *':
-    string_converted = string.encode('utf-8')
-    result = _lib.periodset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_out(ss: 'const SpanSet *') -> str:
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.periodset_out(ss_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def set_as_hexwkb(s: 'const Set *', variant: int) -> "Tuple[str, 'size_t *']":
-    s_converted = _ffi.cast('const Set *', s)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.set_as_hexwkb(s_converted, variant_converted, size_out)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def set_as_wkb(s: 'const Set *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    s_converted = _ffi.cast('const Set *', s)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.set_as_wkb(s_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def set_from_hexwkb(hexwkb: str) -> 'Set *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.set_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Set *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.set_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_out(s: 'const Set *', maxdd: int) -> str:
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_out(s_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def span_as_wkb(s: 'const Span *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    s_converted = _ffi.cast('const Span *', s)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.span_as_wkb(s_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def span_as_hexwkb(s: 'const Span *', variant: int) -> "Tuple[str, 'size_t *']":
-    s_converted = _ffi.cast('const Span *', s)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.span_as_hexwkb(s_converted, variant_converted, size_out)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def span_from_hexwkb(hexwkb: str) -> 'Span *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.span_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Span *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.span_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_out(s: 'const Span *', maxdd: int) -> str:
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_out(s_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def spanset_as_wkb(ss: 'const SpanSet *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.spanset_as_wkb(ss_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def spanset_as_hexwkb(ss: 'const SpanSet *', variant: int) -> "Tuple[str, 'size_t *']":
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.spanset_as_hexwkb(ss_converted, variant_converted, size_out)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def spanset_from_hexwkb(hexwkb: str) -> 'SpanSet *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.spanset_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'SpanSet *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.spanset_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_out(ss: 'const SpanSet *', maxdd: int) -> str:
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_out(ss_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def textset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.textset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def textset_out(set: 'const Set *') -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.textset_out(set_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_in(string: str) -> 'Set *':
-    string_converted = string.encode('utf-8')
-    result = _lib.timestampset_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_out(set: 'const Set *') -> str:
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.timestampset_out(set_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_make(values: 'const int64 *', count: int) -> 'Set *':
-    values_converted = _ffi.cast('const int64 *', values)
-    result = _lib.bigintset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspan_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
-    lower_converted = _ffi.cast('int64', lower)
-    upper_converted = _ffi.cast('int64', upper)
-    result = _lib.bigintspan_make(lower_converted, upper_converted, lower_inc, upper_inc)
-    return result if result != _ffi.NULL else None
-
-
-def floatset_make(values: 'const double *', count: int) -> 'Set *':
-    values_converted = _ffi.cast('const double *', values)
-    result = _lib.floatset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_make(lower: float, upper: float, lower_inc: bool, upper_inc: bool) -> 'Span *':
-    result = _lib.floatspan_make(lower, upper, lower_inc, upper_inc)
-    return result if result != _ffi.NULL else None
-
-
-def geogset_make(values: 'const GSERIALIZED **', count: int) -> 'Set *':
-    values_converted = [_ffi.cast('const GSERIALIZED *', x) for x in values]
-    result = _lib.geogset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def geomset_make(values: 'const GSERIALIZED **', count: int) -> 'Set *':
-    values_converted = [_ffi.cast('const GSERIALIZED *', x) for x in values]
-    result = _lib.geomset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def intset_make(values: 'const int *', count: int) -> 'Set *':
-    values_converted = _ffi.cast('const int *', values)
-    result = _lib.intset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def intspan_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
-    result = _lib.intspan_make(lower, upper, lower_inc, upper_inc)
-    return result if result != _ffi.NULL else None
-
-
-def period_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
-    lower_converted = _ffi.cast('TimestampTz', lower)
-    upper_converted = _ffi.cast('TimestampTz', upper)
-    result = _lib.period_make(lower_converted, upper_converted, lower_inc, upper_inc)
-    return result if result != _ffi.NULL else None
-
-
-def set_copy(s: 'const Set *') -> 'Set *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_copy(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_copy(s: 'const Span *') -> 'Span *':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_copy(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_copy(ps: 'const SpanSet *') -> 'SpanSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.spanset_copy(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_make(spans: 'List[Span *]', normalize: bool) -> 'SpanSet *':
-    spans_converted = _ffi.new('Span []', spans)
-    result = _lib.spanset_make(spans_converted, len(spans), normalize)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_make_exp(spans: 'Span *', count: int, maxcount: int, normalize: bool, ordered: bool) -> 'SpanSet *':
-    spans_converted = _ffi.cast('Span *', spans)
-    result = _lib.spanset_make_exp(spans_converted, count, maxcount, normalize, ordered)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_make_free(spans: 'Span *', count: int, normalize: bool) -> 'SpanSet *':
-    spans_converted = _ffi.cast('Span *', spans)
-    result = _lib.spanset_make_free(spans_converted, count, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def textset_make(values: 'const text **', count: int) -> 'Set *':
-    values_converted = [_ffi.cast('const text *', x) for x in values]
-    result = _lib.textset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_make(values: List[int], count: int) -> 'Set *':
-    values_converted = [_ffi.cast('const TimestampTz', x) for x in values]
-    result = _lib.timestampset_make(values_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def bigint_to_bigintset(i: int) -> 'Set *':
-    i_converted = _ffi.cast('int64', i)
-    result = _lib.bigint_to_bigintset(i_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigint_to_bigintspan(i: int) -> 'Span *':
-    result = _lib.bigint_to_bigintspan(i)
-    return result if result != _ffi.NULL else None
-
-
-def bigint_to_bigintspanset(i: int) -> 'SpanSet *':
-    result = _lib.bigint_to_bigintspanset(i)
-    return result if result != _ffi.NULL else None
-
-
-def float_to_floatset(d: float) -> 'Set *':
-    result = _lib.float_to_floatset(d)
-    return result if result != _ffi.NULL else None
-
-
-def float_to_floatspan(d: float) -> 'Span *':
-    result = _lib.float_to_floatspan(d)
-    return result if result != _ffi.NULL else None
-
-
-def float_to_floatspanset(d: float) -> 'SpanSet *':
-    result = _lib.float_to_floatspanset(d)
-    return result if result != _ffi.NULL else None
-
-
-def int_to_intset(i: int) -> 'Set *':
-    result = _lib.int_to_intset(i)
-    return result if result != _ffi.NULL else None
-
-
-def int_to_intspan(i: int) -> 'Span *':
-    result = _lib.int_to_intspan(i)
-    return result if result != _ffi.NULL else None
-
-
-def int_to_intspanset(i: int) -> 'SpanSet *':
-    result = _lib.int_to_intspanset(i)
-    return result if result != _ffi.NULL else None
-
-
-def set_to_spanset(s: 'const Set *') -> 'SpanSet *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_to_spanset(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_to_spanset(s: 'const Span *') -> 'SpanSet *':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_to_spanset(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_to_period(t: int) -> 'Span *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_to_period(t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_to_periodset(t: int) -> 'SpanSet *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_to_periodset(t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_to_tstzset(t: int) -> 'Set *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_to_tstzset(t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_end_value(s: 'const Set *') -> 'int64':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.bigintset_end_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_start_value(s: 'const Set *') -> 'int64':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.bigintset_start_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintset_value_n(s: 'const Set *', n: int) -> 'int64':
-    s_converted = _ffi.cast('const Set *', s)
-    out_result = _ffi.new('int64 *')
-    result = _lib.bigintset_value_n(s_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def bigintset_values(s: 'const Set *') -> 'int64 *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.bigintset_values(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspan_lower(s: 'const Span *') -> 'int':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.bigintspan_lower(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspan_upper(s: 'const Span *') -> 'int':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.bigintspan_upper(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspanset_lower(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.bigintspanset_lower(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigintspanset_upper(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.bigintspanset_upper(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatset_end_value(s: 'const Set *') -> 'double':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.floatset_end_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatset_start_value(s: 'const Set *') -> 'double':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.floatset_start_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatset_value_n(s: 'const Set *', n: int) -> 'double':
-    s_converted = _ffi.cast('const Set *', s)
-    out_result = _ffi.new('double *')
-    result = _lib.floatset_value_n(s_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def floatset_values(s: 'const Set *') -> 'double *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.floatset_values(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_lower(s: 'const Span *') -> 'double':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.floatspan_lower(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_upper(s: 'const Span *') -> 'double':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.floatspan_upper(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspanset_lower(ss: 'const SpanSet *') -> 'double':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.floatspanset_lower(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspanset_upper(ss: 'const SpanSet *') -> 'double':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.floatspanset_upper(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geoset_srid(set: 'const Set *') -> 'int':
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.geoset_srid(set_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intset_end_value(s: 'const Set *') -> 'int':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.intset_end_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intset_start_value(s: 'const Set *') -> 'int':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.intset_start_value(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intset_value_n(s: 'const Set *', n: int) -> 'int':
-    s_converted = _ffi.cast('const Set *', s)
-    out_result = _ffi.new('int *')
-    result = _lib.intset_value_n(s_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def intset_values(s: 'const Set *') -> 'int *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.intset_values(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspan_lower(s: 'const Span *') -> 'int':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.intspan_lower(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspan_upper(s: 'const Span *') -> 'int':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.intspan_upper(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspanset_lower(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.intspanset_lower(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intspanset_upper(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.intspanset_upper(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_duration(s: 'const Span *') -> 'Interval *':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.period_duration(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_lower(p: 'const Span *') -> 'TimestampTz':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.period_lower(p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_upper(p: 'const Span *') -> 'TimestampTz':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.period_upper(p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_duration(ps: 'const SpanSet *', boundspan: bool) -> 'Interval *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_duration(ps_converted, boundspan)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_end_timestamp(ps: 'const SpanSet *') -> 'TimestampTz':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_end_timestamp(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_lower(ps: 'const SpanSet *') -> 'TimestampTz':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_lower(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_num_timestamps(ps: 'const SpanSet *') -> 'int':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_num_timestamps(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_start_timestamp(ps: 'const SpanSet *') -> 'TimestampTz':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_start_timestamp(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_timestamp_n(ps: 'const SpanSet *', n: int) -> int:
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.periodset_timestamp_n(ps_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def periodset_timestamps(ps: 'const SpanSet *') -> "Tuple['TimestampTz *', 'int']":
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    count = _ffi.new('int *')
-    result = _lib.periodset_timestamps(ps_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def periodset_upper(ps: 'const SpanSet *') -> 'TimestampTz':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_upper(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_hash(s: 'const Set *') -> 'uint32':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_hash(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_hash_extended(s: 'const Set *', seed: int) -> 'uint64':
-    s_converted = _ffi.cast('const Set *', s)
-    seed_converted = _ffi.cast('uint64', seed)
-    result = _lib.set_hash_extended(s_converted, seed_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_mem_size(s: 'const Set *') -> 'int':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_mem_size(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_num_values(s: 'const Set *') -> 'int':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_num_values(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_span(s: 'const Set *') -> 'Span *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.set_span(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_hash(s: 'const Span *') -> 'uint32':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_hash(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_hash_extended(s: 'const Span *', seed: int) -> 'uint64':
-    s_converted = _ffi.cast('const Span *', s)
-    seed_converted = _ffi.cast('uint64', seed)
-    result = _lib.span_hash_extended(s_converted, seed_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_lower_inc(s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_lower_inc(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_upper_inc(s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_upper_inc(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_width(s: 'const Span *') -> 'double':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.span_width(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_end_span(ss: 'const SpanSet *') -> 'Span *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_end_span(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_hash(ps: 'const SpanSet *') -> 'uint32':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.spanset_hash(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_hash_extended(ps: 'const SpanSet *', seed: int) -> 'uint64':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    seed_converted = _ffi.cast('uint64', seed)
-    result = _lib.spanset_hash_extended(ps_converted, seed_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_lower_inc(ss: 'const SpanSet *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_lower_inc(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_mem_size(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_mem_size(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_num_spans(ss: 'const SpanSet *') -> 'int':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_num_spans(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_span(ss: 'const SpanSet *') -> 'Span *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_span(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_span_n(ss: 'const SpanSet *', i: int) -> 'Span *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_span_n(ss_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_spans(ss: 'const SpanSet *') -> 'const Span **':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_spans(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_start_span(ss: 'const SpanSet *') -> 'Span *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_start_span(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_upper_inc(ss: 'const SpanSet *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_upper_inc(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_width(ss: 'const SpanSet *') -> 'double':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_width(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spatialset_stbox(s: 'const Set *') -> 'STBox *':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.spatialset_stbox(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_end_timestamp(ts: 'const Set *') -> 'TimestampTz':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.timestampset_end_timestamp(ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_start_timestamp(ts: 'const Set *') -> 'TimestampTz':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.timestampset_start_timestamp(ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_timestamp_n(ts: 'const Set *', n: int) -> int:
-    ts_converted = _ffi.cast('const Set *', ts)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.timestampset_timestamp_n(ts_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def timestampset_values(ts: 'const Set *') -> 'TimestampTz *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.timestampset_values(ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_set_intspan(s1: 'const Span *', s2: 'Span *') -> None:
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('Span *', s2)
-    _lib.floatspan_set_intspan(s1_converted, s2_converted)
-
-
-def intspan_set_floatspan(s1: 'const Span *', s2: 'Span *') -> None:
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('Span *', s2)
-    _lib.intspan_set_floatspan(s1_converted, s2_converted)
-
-
-def numspan_set_floatspan(s1: 'const Span *', s2: 'Span *') -> None:
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('Span *', s2)
-    _lib.numspan_set_floatspan(s1_converted, s2_converted)
-
-
-def period_tprecision(s: 'const Span *', duration: 'const Interval *', torigin: int) -> 'Span *':
-    s_converted = _ffi.cast('const Span *', s)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    result = _lib.period_tprecision(s_converted, duration_converted, torigin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_tprecision(ss: 'const SpanSet *', duration: 'const Interval *', torigin: int) -> 'SpanSet *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    result = _lib.periodset_tprecision(ss_converted, duration_converted, torigin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_shift_tscale(p: 'const Span *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Span *':
-    p_converted = _ffi.cast('const Span *', p)
-    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
-    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
-    result = _lib.period_shift_tscale(p_converted, shift_converted, duration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_shift_tscale(ps: 'const SpanSet *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'SpanSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
-    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
-    result = _lib.periodset_shift_tscale(ps_converted, shift_converted, duration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_shift(s: 'const Set *', shift: 'Datum') -> 'Set *':
-    s_converted = _ffi.cast('const Set *', s)
-    shift_converted = _ffi.cast('Datum', shift)
-    result = _lib.set_shift(s_converted, shift_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_expand(s1: 'const Span *', s2: 'Span *') -> None:
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('Span *', s2)
-    _lib.span_expand(s1_converted, s2_converted)
-
-
-def timestamp_tprecision(t: int, duration: 'const Interval *', torigin: int) -> 'TimestampTz':
-    t_converted = _ffi.cast('TimestampTz', t)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    result = _lib.timestamp_tprecision(t_converted, duration_converted, torigin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_shift_tscale(ts: 'const Set *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Set *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
-    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
-    result = _lib.timestampset_shift_tscale(ts_converted, shift_converted, duration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_bigintspan_bigint(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    i_converted = _ffi.cast('int64', i)
-    result = _lib.adjacent_bigintspan_bigint(s_converted, i_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_bigintspanset_bigint(ss: 'const SpanSet *', i: int) -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    i_converted = _ffi.cast('int64', i)
-    result = _lib.adjacent_bigintspanset_bigint(ss_converted, i_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.adjacent_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.adjacent_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_period_timestamp(p: 'const Span *', t: int) -> 'bool':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.adjacent_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.adjacent_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.adjacent_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.adjacent_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.adjacent_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_bigint_bigintset(i: int, s: 'const Set *') -> 'bool':
-    i_converted = _ffi.cast('int64', i)
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.contained_bigint_bigintset(i_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_bigint_bigintspan(i: int, s: 'const Span *') -> 'bool':
-    i_converted = _ffi.cast('int64', i)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contained_bigint_bigintspan(i_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_bigint_bigintspanset(i: int, ss: 'const SpanSet *') -> 'bool':
-    i_converted = _ffi.cast('int64', i)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.contained_bigint_bigintspanset(i_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_float_floatset(d: float, s: 'const Set *') -> 'bool':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.contained_float_floatset(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_float_floatspan(d: float, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contained_float_floatspan(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_float_floatspanset(d: float, ss: 'const SpanSet *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.contained_float_floatspanset(d, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_int_intset(i: int, s: 'const Set *') -> 'bool':
-    s_converted = _ffi.cast('const Set *', s)
-    result = _lib.contained_int_intset(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_int_intspan(i: int, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contained_int_intspan(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.contained_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.contained_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.contained_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contained_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.contained_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_timestamp_period(t: int, p: 'const Span *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.contained_timestamp_period(t_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.contained_timestamp_timestampset(t_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contains_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def contains_floatspanset_float(ss: 'const SpanSet *', d: float) -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.contains_floatspanset_float(ss_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def contains_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contains_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def contains_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.contains_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_period_timestamp(p: 'const Span *', t: int) -> 'bool':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.contains_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.contains_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.contains_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.contains_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.contains_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.contains_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_timestampset_timestamp(ts: 'const Set *', t: int) -> 'bool':
-    ts_converted = _ffi.cast('const Set *', ts)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.contains_timestampset_timestamp(ts_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.overlaps_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.overlaps_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overlaps_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.overlaps_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def after_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.after_timestamp_timestampset(t_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def before_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.before_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def before_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.before_timestamp_timestampset(t_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_float_floatspan(d: float, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.left_float_floatspan(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.left_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def left_int_intspan(i: int, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.left_int_intspan(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.left_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def left_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.left_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.left_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.left_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.left_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.left_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_period_timestamp(p: 'const Span *', t: int) -> 'bool':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.overafter_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.overafter_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_timestamp_period(t: int, p: 'const Span *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.overafter_timestamp_period(t_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_timestamp_periodset(t: int, ps: 'const SpanSet *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.overafter_timestamp_periodset(t_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.overafter_timestamp_timestampset(t_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_period_timestamp(p: 'const Span *', t: int) -> 'bool':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.overbefore_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.overbefore_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_timestamp_period(t: int, p: 'const Span *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.overbefore_timestamp_period(t_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_timestamp_periodset(t: int, ps: 'const SpanSet *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.overbefore_timestamp_periodset(t_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
-    t_converted = _ffi.cast('TimestampTz', t)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.overbefore_timestamp_timestampset(t_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_float_floatspan(d: float, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overleft_float_floatspan(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overleft_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_int_intspan(i: int, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overleft_int_intspan(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overleft_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.overleft_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.overleft_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.overleft_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overleft_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.overleft_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_float_floatspan(d: float, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overright_float_floatspan(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overright_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def overright_int_intspan(i: int, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overright_int_intspan(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overright_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def overright_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.overright_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.overright_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.overright_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.overright_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.overright_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_float_floatspan(d: float, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.right_float_floatspan(d, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_floatspan_float(s: 'const Span *', d: float) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.right_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def right_int_intspan(i: int, s: 'const Span *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.right_int_intspan(i, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_intspan_int(s: 'const Span *', i: int) -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.right_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def right_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.right_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.right_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.right_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.right_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.right_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bbox_union_span_span(s1: 'const Span *', s2: 'const Span *') -> 'Span *':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    out_result = _ffi.new('Span *')
-    _lib.bbox_union_span_span(s1_converted, s2_converted, out_result)
-    return out_result if out_result!= _ffi.NULL else None
-
-
-
-def intersection_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.intersection_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intersection_period_timestamp(p: 'const Span *', t: int) -> int:
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.intersection_period_timestamp(p_converted, t_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def intersection_periodset_timestamp(ps: 'const SpanSet *', t: int) -> int:
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.intersection_periodset_timestamp(ps_converted, t_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def intersection_span_span(s1: 'const Span *', s2: 'const Span *') -> 'Span *':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.intersection_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intersection_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.intersection_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intersection_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.intersection_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def intersection_timestampset_timestamp(ts: 'const Set *', t: int) -> int:
-    ts_converted = _ffi.cast('const Set *', ts)
-    t_converted = _ffi.cast('const TimestampTz', t)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.intersection_timestampset_timestamp(ts_converted, t_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def minus_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.minus_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_period_timestamp(p: 'const Span *', t: int) -> 'SpanSet *':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.minus_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'SpanSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.minus_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_span_span(s1: 'const Span *', s2: 'const Span *') -> 'SpanSet *':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.minus_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'SpanSet *':
-    s_converted = _ffi.cast('const Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.minus_span_spanset(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.minus_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.minus_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def minus_timestamp_period(t: int, p: 'const Span *') -> int:
-    t_converted = _ffi.cast('TimestampTz', t)
-    p_converted = _ffi.cast('const Span *', p)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.minus_timestamp_period(t_converted, p_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def minus_timestamp_periodset(t: int, ps: 'const SpanSet *') -> int:
-    t_converted = _ffi.cast('TimestampTz', t)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.minus_timestamp_periodset(t_converted, ps_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def minus_timestampset_timestamp(ts: 'const Set *', t: int) -> 'Set *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.minus_timestampset_timestamp(ts_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.union_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_period_timestamp(p: 'const Span *', t: int) -> 'SpanSet *':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.union_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_periodset_timestamp(ps: 'SpanSet *', t: int) -> 'SpanSet *':
-    ps_converted = _ffi.cast('SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.union_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_span_span(s1: 'const Span *', s2: 'const Span *') -> 'SpanSet *':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.union_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.union_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.union_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_timestampset_timestamp(ts: 'const Set *', t: int) -> 'Set *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    t_converted = _ffi.cast('const TimestampTz', t)
-    result = _lib.union_timestampset_timestamp(ts_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_floatspan_float(s: 'const Span *', d: float) -> 'double':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.distance_floatspan_float(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def distance_intspan_int(s: 'const Span *', i: int) -> 'double':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.distance_intspan_int(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def distance_set_set(s1: 'const Set *', s2: 'const Set *') -> 'double':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.distance_set_set(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_period_timestamp(p: 'const Span *', t: int) -> 'double':
-    p_converted = _ffi.cast('const Span *', p)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.distance_period_timestamp(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'double':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.distance_periodset_timestamp(ps_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_span_span(s1: 'const Span *', s2: 'const Span *') -> 'double':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.distance_span_span(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'double':
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.distance_spanset_span(ss_converted, s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'double':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.distance_spanset_spanset(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_timestampset_timestamp(ts: 'const Set *', t: int) -> 'double':
-    ts_converted = _ffi.cast('const Set *', ts)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.distance_timestampset_timestamp(ts_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigint_extent_transfn(s: 'Span *', i: int) -> 'Span *':
-    s_converted = _ffi.cast('Span *', s)
-    i_converted = _ffi.cast('int64', i)
-    result = _lib.bigint_extent_transfn(s_converted, i_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bigint_union_transfn(state: 'Set *', i: int) -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    i_converted = _ffi.cast('int64', i)
-    result = _lib.bigint_union_transfn(state_converted, i_converted)
-    return result if result != _ffi.NULL else None
-
-
-def float_extent_transfn(s: 'Span *', d: float) -> 'Span *':
-    s_converted = _ffi.cast('Span *', s)
-    result = _lib.float_extent_transfn(s_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def float_union_transfn(state: 'Set *', d: float) -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    result = _lib.float_union_transfn(state_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def int_extent_transfn(s: 'Span *', i: int) -> 'Span *':
-    s_converted = _ffi.cast('Span *', s)
-    result = _lib.int_extent_transfn(s_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def int_union_transfn(state: 'Set *', i: int) -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    result = _lib.int_union_transfn(state_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def period_tcount_transfn(state: "Optional['SkipList *']", p: 'const Span *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.period_tcount_transfn(state_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_tcount_transfn(state: "Optional['SkipList *']", ps: 'const SpanSet *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_tcount_transfn(state_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_extent_transfn(span: 'Span *', set: 'const Set *') -> 'Span *':
-    span_converted = _ffi.cast('Span *', span)
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.set_extent_transfn(span_converted, set_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_union_finalfn(state: 'Set *') -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    result = _lib.set_union_finalfn(state_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_union_transfn(state: 'Set *', set: 'Set *') -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    set_converted = _ffi.cast('Set *', set)
-    result = _lib.set_union_transfn(state_converted, set_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_extent_transfn(s1: 'Span *', s2: 'const Span *') -> 'Span *':
-    s1_converted = _ffi.cast('Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_extent_transfn(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_union_transfn(state: 'SpanSet *', span: 'const Span *') -> 'SpanSet *':
-    state_converted = _ffi.cast('SpanSet *', state)
-    span_converted = _ffi.cast('const Span *', span)
-    result = _lib.span_union_transfn(state_converted, span_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_extent_transfn(s: 'Span *', ss: 'const SpanSet *') -> 'Span *':
-    s_converted = _ffi.cast('Span *', s)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_extent_transfn(s_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_union_finalfn(state: 'SpanSet *') -> 'SpanSet *':
-    state_converted = _ffi.cast('SpanSet *', state)
-    result = _lib.spanset_union_finalfn(state_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_union_transfn(state: 'SpanSet *', ss: 'const SpanSet *') -> 'SpanSet *':
-    state_converted = _ffi.cast('SpanSet *', state)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.spanset_union_transfn(state_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def text_union_transfn(state: 'Set *', txt: str) -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    txt_converted = cstring2text(txt)
-    result = _lib.text_union_transfn(state_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_extent_transfn(p: "Optional['Span *']", t: int) -> 'Span *':
-    p_converted = _ffi.cast('Span *', p) if p is not None else _ffi.NULL
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_extent_transfn(p_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_tcount_transfn(state: "Optional['SkipList *']", t: int) -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_tcount_transfn(state_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_union_transfn(state: 'Set *', t: int) -> 'Set *':
-    state_converted = _ffi.cast('Set *', state)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_union_transfn(state_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_tcount_transfn(state: "Optional['SkipList *']", ts: 'const Set *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.timestampset_tcount_transfn(state_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_cmp(s1: 'const Set *', s2: 'const Set *') -> 'int':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_cmp(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_eq(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_eq(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_ge(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_ge(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_gt(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_gt(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_le(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_le(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_lt(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_lt(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def set_ne(s1: 'const Set *', s2: 'const Set *') -> 'bool':
-    s1_converted = _ffi.cast('const Set *', s1)
-    s2_converted = _ffi.cast('const Set *', s2)
-    result = _lib.set_ne(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_cmp(s1: 'const Span *', s2: 'const Span *') -> 'int':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_cmp(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_eq(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_eq(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_ge(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_ge(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_gt(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_gt(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_le(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_le(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_lt(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_lt(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_ne(s1: 'const Span *', s2: 'const Span *') -> 'bool':
-    s1_converted = _ffi.cast('const Span *', s1)
-    s2_converted = _ffi.cast('const Span *', s2)
-    result = _lib.span_ne(s1_converted, s2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_cmp(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'int':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_cmp(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_eq(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_eq(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_ge(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_ge(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_gt(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_gt(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_le(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_le(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_lt(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_lt(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def spanset_ne(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
-    ss1_converted = _ffi.cast('const SpanSet *', ss1)
-    ss2_converted = _ffi.cast('const SpanSet *', ss2)
-    result = _lib.spanset_ne(ss1_converted, ss2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_in(string: str) -> 'TBox *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tbox_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_out(box: 'const TBox *', maxdd: int) -> str:
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_out(box_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tbox_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'TBox *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.tbox_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_from_hexwkb(hexwkb: str) -> 'TBox *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.tbox_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'STBox *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.stbox_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_from_hexwkb(hexwkb: str) -> 'STBox *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.stbox_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_as_wkb(box: 'const TBox *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    box_converted = _ffi.cast('const TBox *', box)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.tbox_as_wkb(box_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def tbox_as_hexwkb(box: 'const TBox *', variant: int) -> "Tuple[str, 'size_t *']":
-    box_converted = _ffi.cast('const TBox *', box)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size = _ffi.new('size_t *')
-    result = _lib.tbox_as_hexwkb(box_converted, variant_converted, size)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size[0]
-
-
-def stbox_as_wkb(box: 'const STBox *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    box_converted = _ffi.cast('const STBox *', box)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.stbox_as_wkb(box_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def stbox_as_hexwkb(box: 'const STBox *', variant: int) -> "Tuple[str, 'size_t *']":
-    box_converted = _ffi.cast('const STBox *', box)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size = _ffi.new('size_t *')
-    result = _lib.stbox_as_hexwkb(box_converted, variant_converted, size)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size[0]
-
-
-def stbox_in(string: str) -> 'STBox *':
-    string_converted = string.encode('utf-8')
-    result = _lib.stbox_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_out(box: 'const STBox *', maxdd: int) -> str:
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_out(box_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tbox_make(s: "Optional['const Span *']", p: "Optional['const Span *']") -> 'TBox *':
-    s_converted = _ffi.cast('const Span *', s) if s is not None else _ffi.NULL
-    p_converted = _ffi.cast('const Span *', p) if p is not None else _ffi.NULL
-    result = _lib.tbox_make(s_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_set(s: 'const Span *', p: 'const Span *', box: 'TBox *') -> None:
-    s_converted = _ffi.cast('const Span *', s)
-    p_converted = _ffi.cast('const Span *', p)
-    box_converted = _ffi.cast('TBox *', box)
-    _lib.tbox_set(s_converted, p_converted, box_converted)
-
-
-def tbox_copy(box: 'const TBox *') -> 'TBox *':
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_copy(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_make(hasx: bool, hasz: bool, geodetic: bool, srid: int, xmin: float, xmax: float, ymin: float, ymax: float, zmin: float, zmax: float, p: "Optional['const Span *']") -> 'STBox *':
-    srid_converted = _ffi.cast('int32', srid)
-    p_converted = _ffi.cast('const Span *', p) if p is not None else _ffi.NULL
-    result = _lib.stbox_make(hasx, hasz, geodetic, srid_converted, xmin, xmax, ymin, ymax, zmin, zmax, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_set(hasx: bool, hasz: bool, geodetic: bool, srid: int, xmin: float, xmax: float, ymin: float, ymax: float, zmin: float, zmax: float, p: 'const Span *', box: 'STBox *') -> None:
-    srid_converted = _ffi.cast('int32', srid)
-    p_converted = _ffi.cast('const Span *', p)
-    box_converted = _ffi.cast('STBox *', box)
-    _lib.stbox_set(hasx, hasz, geodetic, srid_converted, xmin, xmax, ymin, ymax, zmin, zmax, p_converted, box_converted)
-
-
-def stbox_copy(box: 'const STBox *') -> 'STBox *':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_copy(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def int_to_tbox(i: int) -> 'TBox *':
-    result = _lib.int_to_tbox(i)
-    return result if result != _ffi.NULL else None
-
-
-def float_to_tbox(d: float) -> 'TBox *':
-    result = _lib.float_to_tbox(d)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_to_tbox(t: int) -> 'TBox *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_to_tbox(t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_to_tbox(ss: 'const Set *') -> 'TBox *':
-    ss_converted = _ffi.cast('const Set *', ss)
-    result = _lib.timestampset_to_tbox(ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_to_tbox(p: 'const Span *') -> 'TBox *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.period_to_tbox(p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_to_tbox(ps: 'const SpanSet *') -> 'TBox *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_to_tbox(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def int_timestamp_to_tbox(i: int, t: int) -> 'TBox *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.int_timestamp_to_tbox(i, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def float_period_to_tbox(d: float, p: 'const Span *') -> 'TBox *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.float_period_to_tbox(d, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def float_timestamp_to_tbox(d: float, t: int) -> 'TBox *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.float_timestamp_to_tbox(d, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geo_period_to_stbox(gs: 'const GSERIALIZED *', p: 'const Span *') -> 'STBox *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.geo_period_to_stbox(gs_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geo_timestamp_to_stbox(gs: 'const GSERIALIZED *', t: int) -> 'STBox *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.geo_timestamp_to_stbox(gs_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geo_to_stbox(gs: 'const GSERIALIZED *') -> 'STBox *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.geo_to_stbox(gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def int_period_to_tbox(i: int, p: 'const Span *') -> 'TBox *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.int_period_to_tbox(i, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def numspan_to_tbox(s: 'const Span *') -> 'TBox *':
-    s_converted = _ffi.cast('const Span *', s)
-    result = _lib.numspan_to_tbox(s_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_timestamp_to_tbox(span: 'const Span *', t: int) -> 'TBox *':
-    span_converted = _ffi.cast('const Span *', span)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.span_timestamp_to_tbox(span_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def span_period_to_tbox(span: 'const Span *', p: 'const Span *') -> 'TBox *':
-    span_converted = _ffi.cast('const Span *', span)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.span_period_to_tbox(span_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_to_floatspan(box: 'const TBox *') -> 'Span *':
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_to_floatspan(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_to_period(box: 'const TBox *') -> 'Span *':
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_to_period(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_to_period(box: 'const STBox *') -> 'Span *':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_to_period(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_to_tbox(temp: 'const Temporal *') -> 'TBox *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_to_tbox(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_to_geo(box: 'const STBox *') -> 'GSERIALIZED *':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_to_geo(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_to_stbox(temp: 'const Temporal *') -> 'STBox *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_to_stbox(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestamp_to_stbox(t: int) -> 'STBox *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.timestamp_to_stbox(t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def timestampset_to_stbox(ts: 'const Set *') -> 'STBox *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.timestampset_to_stbox(ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_to_stbox(p: 'const Span *') -> 'STBox *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.period_to_stbox(p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def periodset_to_stbox(ps: 'const SpanSet *') -> 'STBox *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.periodset_to_stbox(ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_hasx(box: 'const TBox *') -> 'bool':
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_hasx(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_hast(box: 'const TBox *') -> 'bool':
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tbox_hast(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_xmin(box: 'const TBox *') -> 'double':
-    box_converted = _ffi.cast('const TBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.tbox_xmin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tbox_xmax(box: 'const TBox *') -> 'double':
-    box_converted = _ffi.cast('const TBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.tbox_xmax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tbox_tmin(box: 'const TBox *') -> int:
-    box_converted = _ffi.cast('const TBox *', box)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.tbox_tmin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tbox_tmax(box: 'const TBox *') -> int:
-    box_converted = _ffi.cast('const TBox *', box)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.tbox_tmax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_hasx(box: 'const STBox *') -> 'bool':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_hasx(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_hasz(box: 'const STBox *') -> 'bool':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_hasz(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_hast(box: 'const STBox *') -> 'bool':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_hast(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_isgeodetic(box: 'const STBox *') -> 'bool':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_isgeodetic(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_xmin(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_xmin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_xmax(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_xmax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_ymin(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_ymin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_ymax(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_ymax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_zmin(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_zmin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_zmax(box: 'const STBox *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('double *')
-    result = _lib.stbox_zmax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_tmin(box: 'const STBox *') -> int:
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.stbox_tmin(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_tmax(box: 'const STBox *') -> int:
-    box_converted = _ffi.cast('const STBox *', box)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.stbox_tmax(box_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def stbox_srid(box: 'const STBox *') -> 'int32':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_srid(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_expand(box1: 'const TBox *', box2: 'TBox *') -> None:
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('TBox *', box2)
-    _lib.tbox_expand(box1_converted, box2_converted)
-
-
-def tbox_expand_value(box: 'const TBox *', d: 'const double') -> 'TBox *':
-    box_converted = _ffi.cast('const TBox *', box)
-    d_converted = _ffi.cast('const double', d)
-    result = _lib.tbox_expand_value(box_converted, d_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_expand_time(box: 'const TBox *', interval: 'const Interval *') -> 'TBox *':
-    box_converted = _ffi.cast('const TBox *', box)
-    interval_converted = _ffi.cast('const Interval *', interval)
-    result = _lib.tbox_expand_time(box_converted, interval_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_expand(box1: 'const STBox *', box2: 'STBox *') -> None:
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('STBox *', box2)
-    _lib.stbox_expand(box1_converted, box2_converted)
-
-
-def stbox_set_srid(box: 'const STBox *', srid: int) -> 'STBox *':
-    box_converted = _ffi.cast('const STBox *', box)
-    srid_converted = _ffi.cast('int32', srid)
-    result = _lib.stbox_set_srid(box_converted, srid_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_get_space(box: 'const STBox *') -> 'STBox *':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_get_space(box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_expand_space(box: 'const STBox *', d: float) -> 'STBox *':
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.stbox_expand_space(box_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_expand_time(box: 'const STBox *', interval: 'const Interval *') -> 'STBox *':
-    box_converted = _ffi.cast('const STBox *', box)
-    interval_converted = _ffi.cast('const Interval *', interval)
-    result = _lib.stbox_expand_time(box_converted, interval_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.contains_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.contained_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.overlaps_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def same_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.same_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.adjacent_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contains_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.contains_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def contained_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.contained_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overlaps_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overlaps_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def same_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.same_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def adjacent_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.adjacent_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.left_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.overleft_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.right_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.overright_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def before_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.before_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.overbefore_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def after_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.after_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.overafter_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def left_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.left_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overleft_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overleft_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def right_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.right_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overright_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overright_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def below_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.below_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbelow_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overbelow_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def above_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.above_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overabove_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overabove_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def front_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.front_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overfront_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overfront_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def back_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.back_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overback_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overback_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def before_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.before_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overbefore_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overbefore_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def after_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.after_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def overafter_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.overafter_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.union_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def inter_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    out_result = _ffi.new('TBox *')
-    result = _lib.inter_tbox_tbox(box1_converted, box2_converted, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def intersection_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.intersection_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def union_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *', strict: bool) -> 'STBox *':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.union_stbox_stbox(box1_converted, box2_converted, strict)
-    return result if result != _ffi.NULL else None
-
-
-def inter_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'STBox *':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    out_result = _ffi.new('STBox *')
-    result = _lib.inter_stbox_stbox(box1_converted, box2_converted, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def intersection_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'STBox *':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.intersection_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_quad_split(box: 'const STBox *') -> "Tuple['STBox *', 'int']":
-    box_converted = _ffi.cast('const STBox *', box)
-    count = _ffi.new('int *')
-    result = _lib.stbox_quad_split(box_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tbox_eq(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_eq(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_ne(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_ne(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_cmp(box1: 'const TBox *', box2: 'const TBox *') -> 'int':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_cmp(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_lt(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_lt(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_le(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_le(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_ge(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_ge(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbox_gt(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.tbox_gt(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_eq(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_eq(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_ne(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_ne(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_cmp(box1: 'const STBox *', box2: 'const STBox *') -> 'int':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_cmp(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_lt(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_lt(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_le(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_le(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_ge(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_ge(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_gt(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.stbox_gt(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tbool_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_out(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_out(temp_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def temporal_as_hexwkb(temp: 'const Temporal *', variant: int) -> "Tuple[str, 'size_t *']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.temporal_as_hexwkb(temp_converted, variant_converted, size_out)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def temporal_as_mfjson(temp: 'const Temporal *', with_bbox: bool, flags: int, precision: int, srs: "Optional[str]") -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    srs_converted = srs.encode('utf-8') if srs is not None else _ffi.NULL
-    result = _lib.temporal_as_mfjson(temp_converted, with_bbox, flags, precision, srs_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def temporal_as_wkb(temp: 'const Temporal *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    variant_converted = _ffi.cast('uint8_t', variant)
-    size_out = _ffi.new('size_t *')
-    result = _lib.temporal_as_wkb(temp_converted, variant_converted, size_out)
-    return result if result != _ffi.NULL else None, size_out[0]
-
-
-def temporal_from_hexwkb(hexwkb: str) -> 'Temporal *':
-    hexwkb_converted = hexwkb.encode('utf-8')
-    result = _lib.temporal_from_hexwkb(hexwkb_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_from_mfjson(mfjson: str) -> 'Temporal *':
-    mfjson_converted = mfjson.encode('utf-8')
-    result = _lib.temporal_from_mfjson(mfjson_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Temporal *':
-    wkb_converted = _ffi.cast('const uint8_t *', wkb)
-    size_converted = _ffi.cast('size_t', size)
-    result = _lib.temporal_from_wkb(wkb_converted, size_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tfloat_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_out(temp: 'const Temporal *', maxdd: int) -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_out(temp_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpoint_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tgeogpoint_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompoint_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tgeompoint_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.tint_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_out(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_out(temp_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_as_ewkt(temp: 'const Temporal *', maxdd: int) -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_as_ewkt(temp_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_as_text(temp: 'const Temporal *', maxdd: int) -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_as_text(temp_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_out(temp: 'const Temporal *', maxdd: int) -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_out(temp_converted, maxdd)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def ttext_in(string: str) -> 'Temporal *':
-    string_converted = string.encode('utf-8')
-    result = _lib.ttext_in(string_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_out(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_out(temp_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def tbool_from_base_temp(b: bool, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_from_base_temp(b, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolinst_make(b: bool, t: int) -> 'TInstant *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.tboolinst_make(b, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolseq_from_base_period(b: bool, p: 'const Span *') -> 'TSequence *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.tboolseq_from_base_period(b, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolseq_from_base_temp(b: bool, seq: 'const TSequence *') -> 'TSequence *':
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.tboolseq_from_base_temp(b, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolseq_from_base_timestampset(b: bool, ts: 'const Set *') -> 'TSequence *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.tboolseq_from_base_timestampset(b, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolseqset_from_base_periodset(b: bool, ps: 'const SpanSet *') -> 'TSequenceSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.tboolseqset_from_base_periodset(b, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tboolseqset_from_base_temp(b: bool, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.tboolseqset_from_base_temp(b, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_copy(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_copy(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_from_base_temp(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_from_base_temp(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatinst_make(d: float, t: int) -> 'TInstant *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.tfloatinst_make(d, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatseq_from_base_period(d: float, p: 'const Span *', interp: 'interpType') -> 'TSequence *':
-    p_converted = _ffi.cast('const Span *', p)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tfloatseq_from_base_period(d, p_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatseq_from_base_temp(d: float, seq: 'const TSequence *') -> 'TSequence *':
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.tfloatseq_from_base_temp(d, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatseq_from_base_timestampset(d: float, ts: 'const Set *') -> 'TSequence *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.tfloatseq_from_base_timestampset(d, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatseqset_from_base_periodset(d: float, ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tfloatseqset_from_base_periodset(d, ps_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloatseqset_from_base_temp(d: float, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.tfloatseqset_from_base_temp(d, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpoint_from_base_temp(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgeogpoint_from_base_temp(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointinst_make(gs: 'const GSERIALIZED *', t: int) -> 'TInstant *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.tgeogpointinst_make(gs_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointseq_from_base_period(gs: 'const GSERIALIZED *', p: 'const Span *', interp: 'interpType') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    p_converted = _ffi.cast('const Span *', p)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tgeogpointseq_from_base_period(gs_converted, p_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointseq_from_base_temp(gs: 'const GSERIALIZED *', seq: 'const TSequence *') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.tgeogpointseq_from_base_temp(gs_converted, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointseq_from_base_timestampset(gs: 'const GSERIALIZED *', ts: 'const Set *') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.tgeogpointseq_from_base_timestampset(gs_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointseqset_from_base_temp(gs: 'const GSERIALIZED *', ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.tgeogpointseqset_from_base_temp(gs_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpointseqset_from_base_periodset(gs: 'const GSERIALIZED *', ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tgeogpointseqset_from_base_periodset(gs_converted, ps_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompoint_from_base_temp(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgeompoint_from_base_temp(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointinst_make(gs: 'const GSERIALIZED *', t: int) -> 'TInstant *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.tgeompointinst_make(gs_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointseq_from_base_period(gs: 'const GSERIALIZED *', p: 'const Span *', interp: 'interpType') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    p_converted = _ffi.cast('const Span *', p)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tgeompointseq_from_base_period(gs_converted, p_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointseq_from_base_temp(gs: 'const GSERIALIZED *', seq: 'const TSequence *') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.tgeompointseq_from_base_temp(gs_converted, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointseq_from_base_timestampset(gs: 'const GSERIALIZED *', ts: 'const Set *') -> 'TSequence *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.tgeompointseq_from_base_timestampset(gs_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointseqset_from_base_periodset(gs: 'const GSERIALIZED *', ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tgeompointseqset_from_base_periodset(gs_converted, ps_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompointseqset_from_base_temp(gs: 'const GSERIALIZED *', ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.tgeompointseqset_from_base_temp(gs_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_from_base_temp(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_from_base_temp(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintinst_make(i: int, t: int) -> 'TInstant *':
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.tintinst_make(i, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintseq_from_base_period(i: int, p: 'const Span *') -> 'TSequence *':
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.tintseq_from_base_period(i, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintseq_from_base_temp(i: int, seq: 'const TSequence *') -> 'TSequence *':
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.tintseq_from_base_temp(i, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintseq_from_base_timestampset(i: int, ts: 'const Set *') -> 'TSequence *':
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.tintseq_from_base_timestampset(i, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintseqset_from_base_periodset(i: int, ps: 'const SpanSet *') -> 'TSequenceSet *':
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.tintseqset_from_base_periodset(i, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tintseqset_from_base_temp(i: int, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.tintseqset_from_base_temp(i, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tsequence_make(instants: 'const TInstant **', count: int, lower_inc: bool, upper_inc: bool, interp: 'interpType', normalize: bool) -> 'TSequence *':
-    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tsequence_make(instants_converted, count, lower_inc, upper_inc, interp_converted, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def tsequence_make_exp(instants: 'const TInstant **', count: int, maxcount: int, lower_inc: bool, upper_inc: bool, interp: 'interpType', normalize: bool) -> 'TSequence *':
-    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.tsequence_make_exp(instants_converted, count, maxcount, lower_inc, upper_inc, interp_converted, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def tsequenceset_make(sequences: 'const TSequence **', count: int, normalize: bool) -> 'TSequenceSet *':
-    sequences_converted = [_ffi.cast('const TSequence *', x) for x in sequences]
-    result = _lib.tsequenceset_make(sequences_converted, count, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def tsequenceset_make_exp(sequences: 'const TSequence **', count: int, maxcount: int, normalize: bool) -> 'TSequenceSet *':
-    sequences_converted = [_ffi.cast('const TSequence *', x) for x in sequences]
-    result = _lib.tsequenceset_make_exp(sequences_converted, count, maxcount, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def tsequenceset_make_gaps(instants: 'const TInstant **', count: int, interp: 'interpType', maxt: 'Interval *', maxdist: float) -> 'TSequenceSet *':
-    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
-    interp_converted = _ffi.cast('interpType', interp)
-    maxt_converted = _ffi.cast('Interval *', maxt)
-    result = _lib.tsequenceset_make_gaps(instants_converted, count, interp_converted, maxt_converted, maxdist)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_from_base_temp(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_from_base_temp(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextinst_make(txt: str, t: int) -> 'TInstant *':
-    txt_converted = cstring2text(txt)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.ttextinst_make(txt_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextseq_from_base_period(txt: str, p: 'const Span *') -> 'TSequence *':
-    txt_converted = cstring2text(txt)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.ttextseq_from_base_period(txt_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextseq_from_base_temp(txt: str, seq: 'const TSequence *') -> 'TSequence *':
-    txt_converted = cstring2text(txt)
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.ttextseq_from_base_temp(txt_converted, seq_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextseq_from_base_timestampset(txt: str, ts: 'const Set *') -> 'TSequence *':
-    txt_converted = cstring2text(txt)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.ttextseq_from_base_timestampset(txt_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextseqset_from_base_periodset(txt: str, ps: 'const SpanSet *') -> 'TSequenceSet *':
-    txt_converted = cstring2text(txt)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.ttextseqset_from_base_periodset(txt_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttextseqset_from_base_temp(txt: str, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
-    txt_converted = cstring2text(txt)
-    ss_converted = _ffi.cast('const TSequenceSet *', ss)
-    result = _lib.ttextseqset_from_base_temp(txt_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_to_period(temp: 'const Temporal *') -> 'Span *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_to_period(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_to_tint(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_to_tint(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_to_tfloat(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_to_tfloat(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_to_span(temp: 'const Temporal *') -> 'Span *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_to_span(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_end_value(temp: 'const Temporal *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_end_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_start_value(temp: 'const Temporal *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_start_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_values(temp: 'const Temporal *') -> "Tuple['bool *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tbool_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_duration(temp: 'const Temporal *', boundspan: bool) -> 'Interval *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_duration(temp_converted, boundspan)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_end_instant(temp: 'const Temporal *') -> 'const TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_end_instant(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_end_sequence(temp: 'const Temporal *') -> 'TSequence *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_end_sequence(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_end_timestamp(temp: 'const Temporal *') -> 'TimestampTz':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_end_timestamp(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_hash(temp: 'const Temporal *') -> 'uint32':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_hash(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_instant_n(temp: 'const Temporal *', n: int) -> 'const TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_instant_n(temp_converted, n)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_instants(temp: 'const Temporal *') -> "Tuple['const TInstant **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.temporal_instants(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_interp(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_interp(temp_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def temporal_max_instant(temp: 'const Temporal *') -> 'const TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_max_instant(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_min_instant(temp: 'const Temporal *') -> 'const TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_min_instant(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_num_instants(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_num_instants(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_num_sequences(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_num_sequences(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_num_timestamps(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_num_timestamps(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_segments(temp: 'const Temporal *') -> "Tuple['TSequence **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.temporal_segments(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_sequence_n(temp: 'const Temporal *', i: int) -> 'TSequence *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_sequence_n(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_sequences(temp: 'const Temporal *') -> "Tuple['TSequence **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.temporal_sequences(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_start_instant(temp: 'const Temporal *') -> 'const TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_start_instant(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_start_sequence(temp: 'const Temporal *') -> 'TSequence *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_start_sequence(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_start_timestamp(temp: 'const Temporal *') -> 'TimestampTz':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_start_timestamp(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_stops(temp: 'const Temporal *', maxdist: float, minduration: 'const Interval *') -> 'TSequenceSet *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    minduration_converted = _ffi.cast('const Interval *', minduration)
-    result = _lib.temporal_stops(temp_converted, maxdist, minduration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_subtype(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_subtype(temp_converted)
-    result = _ffi.string(result).decode('utf-8')
-    return result if result != _ffi.NULL else None
-
-
-def temporal_time(temp: 'const Temporal *') -> 'SpanSet *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_time(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_timestamp_n(temp: 'const Temporal *', n: int) -> int:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    out_result = _ffi.new('TimestampTz *')
-    result = _lib.temporal_timestamp_n(temp_converted, n, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def temporal_timestamps(temp: 'const Temporal *') -> "Tuple['TimestampTz *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.temporal_timestamps(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_values(temp: 'const Temporal *') -> "Tuple['Datum *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.temporal_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tfloat_end_value(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_end_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_max_value(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_max_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_min_value(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_min_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_start_value(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_start_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_values(temp: 'const Temporal *') -> "Tuple['double *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tfloat_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tint_end_value(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_end_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_max_value(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_max_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_min_value(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_min_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_start_value(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_start_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_values(temp: 'const Temporal *') -> "Tuple['int *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tint_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tnumber_valuespans(temp: 'const Temporal *') -> 'SpanSet *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_valuespans(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_end_value(temp: 'const Temporal *') -> 'GSERIALIZED *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_end_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_start_value(temp: 'const Temporal *') -> 'GSERIALIZED *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_start_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_values(temp: 'const Temporal *') -> "Tuple['GSERIALIZED **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tpoint_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def ttext_end_value(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_end_value(temp_converted)
-    result = text2cstring(result)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_max_value(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_max_value(temp_converted)
-    result = text2cstring(result)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_min_value(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_min_value(temp_converted)
-    result = text2cstring(result)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_start_value(temp: 'const Temporal *') -> str:
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_start_value(temp_converted)
-    result = text2cstring(result)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_values(temp: 'const Temporal *') -> "Tuple['text **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.ttext_values(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_set_interp(temp: 'const Temporal *', interp: 'interpType') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    interp_converted = _ffi.cast('interpType', interp)
-    result = _lib.temporal_set_interp(temp_converted, interp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_shift(temp: 'const Temporal *', shift: 'const Interval *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    shift_converted = _ffi.cast('const Interval *', shift)
-    result = _lib.temporal_shift(temp_converted, shift_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_shift_tscale(temp: 'const Temporal *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
-    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
-    result = _lib.temporal_shift_tscale(temp_converted, shift_converted, duration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_to_tinstant(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_to_tinstant(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_to_tsequence(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_to_tsequence(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_to_tsequenceset(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_to_tsequenceset(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_tprecision(temp: 'const Temporal *', duration: 'const Interval *', origin: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    origin_converted = _ffi.cast('TimestampTz', origin)
-    result = _lib.temporal_tprecision(temp_converted, duration_converted, origin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_tsample(temp: 'const Temporal *', duration: 'const Interval *', origin: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    origin_converted = _ffi.cast('TimestampTz', origin)
-    result = _lib.temporal_tsample(temp_converted, duration_converted, origin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_tscale(temp: 'const Temporal *', duration: 'const Interval *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    result = _lib.temporal_tscale(temp_converted, duration_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_at_value(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_at_value(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_minus_value(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_minus_value(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('bool *')
-    result = _lib.tbool_value_at_timestamp(temp_converted, t_converted, strict, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def temporal_at_max(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_at_max(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_min(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_at_min(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_period(temp: 'const Temporal *', p: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.temporal_at_period(temp_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_periodset(temp: 'const Temporal *', ps: 'const SpanSet *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.temporal_at_periodset(temp_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_timestamp(temp: 'const Temporal *', t: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.temporal_at_timestamp(temp_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_timestampset(temp: 'const Temporal *', ts: 'const Set *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.temporal_at_timestampset(temp_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_at_values(temp: 'const Temporal *', set: 'const Set *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.temporal_at_values(temp_converted, set_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_max(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_minus_max(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_min(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_minus_min(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_period(temp: 'const Temporal *', p: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.temporal_minus_period(temp_converted, p_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_periodset(temp: 'const Temporal *', ps: 'const SpanSet *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.temporal_minus_periodset(temp_converted, ps_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_timestamp(temp: 'const Temporal *', t: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.temporal_minus_timestamp(temp_converted, t_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_timestampset(temp: 'const Temporal *', ts: 'const Set *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.temporal_minus_timestampset(temp_converted, ts_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_minus_values(temp: 'const Temporal *', set: 'const Set *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    set_converted = _ffi.cast('const Set *', set)
-    result = _lib.temporal_minus_values(temp_converted, set_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_at_value(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_at_value(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_minus_value(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_minus_value(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('double *')
-    result = _lib.tfloat_value_at_timestamp(temp_converted, t_converted, strict, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tint_at_value(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_at_value(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_minus_value(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_minus_value(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('int *')
-    result = _lib.tint_value_at_timestamp(temp_converted, t_converted, strict, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tnumber_at_span(temp: 'const Temporal *', span: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    span_converted = _ffi.cast('const Span *', span)
-    result = _lib.tnumber_at_span(temp_converted, span_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_at_spanset(temp: 'const Temporal *', ss: 'const SpanSet *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.tnumber_at_spanset(temp_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_at_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tnumber_at_tbox(temp_converted, box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_minus_span(temp: 'const Temporal *', span: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    span_converted = _ffi.cast('const Span *', span)
-    result = _lib.tnumber_minus_span(temp_converted, span_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_minus_spanset(temp: 'const Temporal *', ss: 'const SpanSet *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ss_converted = _ffi.cast('const SpanSet *', ss)
-    result = _lib.tnumber_minus_spanset(temp_converted, ss_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_minus_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.tnumber_minus_tbox(temp_converted, box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_at_geom_time(temp: 'const Temporal *', gs: 'const GSERIALIZED *', zspan: 'const Span *', period: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    zspan_converted = _ffi.cast('const Span *', zspan)
-    period_converted = _ffi.cast('const Span *', period)
-    result = _lib.tpoint_at_geom_time(temp_converted, gs_converted, zspan_converted, period_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_at_stbox(temp: 'const Temporal *', box: 'const STBox *', border_inc: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.tpoint_at_stbox(temp_converted, box_converted, border_inc)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_at_value(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tpoint_at_value(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_minus_geom_time(temp: 'const Temporal *', gs: 'const GSERIALIZED *', zspan: 'const Span *', period: 'const Span *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    zspan_converted = _ffi.cast('const Span *', zspan)
-    period_converted = _ffi.cast('const Span *', period)
-    result = _lib.tpoint_minus_geom_time(temp_converted, gs_converted, zspan_converted, period_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_minus_stbox(temp: 'const Temporal *', box: 'const STBox *', border_inc: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.tpoint_minus_stbox(temp_converted, box_converted, border_inc)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_minus_value(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tpoint_minus_value(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'GSERIALIZED **':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('GSERIALIZED **')
-    result = _lib.tpoint_value_at_timestamp(temp_converted, t_converted, strict, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def ttext_at_value(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_at_value(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_minus_value(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_minus_value(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'text **':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    out_result = _ffi.new('text **')
-    result = _lib.ttext_value_at_timestamp(temp_converted, t_converted, strict, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def temporal_append_tinstant(temp: 'Temporal *', inst: 'const TInstant *', maxdist: float, maxt: 'Interval *', expand: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('Temporal *', temp)
-    inst_converted = _ffi.cast('const TInstant *', inst)
-    maxt_converted = _ffi.cast('Interval *', maxt)
-    result = _lib.temporal_append_tinstant(temp_converted, inst_converted, maxdist, maxt_converted, expand)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_append_tsequence(temp: 'Temporal *', seq: 'const TSequence *', expand: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('Temporal *', temp)
-    seq_converted = _ffi.cast('const TSequence *', seq)
-    result = _lib.temporal_append_tsequence(temp_converted, seq_converted, expand)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_delete_period(temp: 'const Temporal *', p: 'const Span *', connect: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    p_converted = _ffi.cast('const Span *', p)
-    result = _lib.temporal_delete_period(temp_converted, p_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_delete_periodset(temp: 'const Temporal *', ps: 'const SpanSet *', connect: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ps_converted = _ffi.cast('const SpanSet *', ps)
-    result = _lib.temporal_delete_periodset(temp_converted, ps_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_delete_timestamp(temp: 'const Temporal *', t: int, connect: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    t_converted = _ffi.cast('TimestampTz', t)
-    result = _lib.temporal_delete_timestamp(temp_converted, t_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_delete_timestampset(temp: 'const Temporal *', ts: 'const Set *', connect: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    ts_converted = _ffi.cast('const Set *', ts)
-    result = _lib.temporal_delete_timestampset(temp_converted, ts_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_insert(temp1: 'const Temporal *', temp2: 'const Temporal *', connect: bool) -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_insert(temp1_converted, temp2_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_merge(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_merge(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_merge_array(temparr: 'Temporal **', count: int) -> 'Temporal *':
-    temparr_converted = [_ffi.cast('Temporal *', x) for x in temparr]
-    result = _lib.temporal_merge_array(temparr_converted, count)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_update(temp1: 'const Temporal *', temp2: 'const Temporal *', connect: bool) -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_update(temp1_converted, temp2_converted, connect)
-    return result if result != _ffi.NULL else None
-
-
-def tand_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tand_bool_tbool(b, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tand_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tand_tbool_bool(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tand_tbool_tbool(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tand_tbool_tbool(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_when_true(temp: 'const Temporal *') -> 'SpanSet *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_when_true(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnot_tbool(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnot_tbool(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tor_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tor_bool_tbool(b, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tor_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tor_tbool_bool(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tor_tbool_tbool(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tor_tbool_tbool(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def add_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.add_float_tfloat(d, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def add_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.add_int_tint(i, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def add_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.add_tfloat_float(tnumber_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def add_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.add_tint_int(tnumber_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def add_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
-    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
-    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
-    result = _lib.add_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def div_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.div_float_tfloat(d, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def div_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.div_int_tint(i, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def div_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.div_tfloat_float(tnumber_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def div_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.div_tint_int(tnumber_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def div_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
-    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
-    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
-    result = _lib.div_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def float_degrees(value: float, normalize: bool) -> 'double':
-    result = _lib.float_degrees(value, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def mult_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.mult_float_tfloat(d, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def mult_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.mult_int_tint(i, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def mult_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.mult_tfloat_float(tnumber_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def mult_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.mult_tint_int(tnumber_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def mult_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
-    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
-    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
-    result = _lib.mult_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def sub_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.sub_float_tfloat(d, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def sub_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.sub_int_tint(i, tnumber_converted)
-    return result if result != _ffi.NULL else None
-
-
-def sub_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.sub_tfloat_float(tnumber_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def sub_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
-    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
-    result = _lib.sub_tint_int(tnumber_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def sub_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
-    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
-    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
-    result = _lib.sub_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_degrees(temp: 'const Temporal *', normalize: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_degrees(temp_converted, normalize)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_derivative(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_derivative(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_radians(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_radians(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_abs(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_abs(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_angular_difference(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_angular_difference(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_delta_value(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_delta_value(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def textcat_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.textcat_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def textcat_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.textcat_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def textcat_ttext_ttext(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.textcat_ttext_ttext(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_upper(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_upper(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_lower(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_lower(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.distance_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def distance_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.distance_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def distance_tnumber_tnumber(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.distance_tnumber_tnumber(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.distance_tpoint_geo(temp_converted, geo_converted)
-    return result if result != _ffi.NULL else None
-
-
-def distance_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.distance_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_stbox_geo(box: 'const STBox *', gs: 'const GSERIALIZED *') -> 'double':
-    box_converted = _ffi.cast('const STBox *', box)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.nad_stbox_geo(box_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'double':
-    box1_converted = _ffi.cast('const STBox *', box1)
-    box2_converted = _ffi.cast('const STBox *', box2)
-    result = _lib.nad_stbox_stbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'double':
-    box1_converted = _ffi.cast('const TBox *', box1)
-    box2_converted = _ffi.cast('const TBox *', box2)
-    result = _lib.nad_tbox_tbox(box1_converted, box2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tfloat_float(temp: 'const Temporal *', d: float) -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.nad_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tfloat_tfloat(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.nad_tfloat_tfloat(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tint_int(temp: 'const Temporal *', i: int) -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.nad_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tint_tint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.nad_tint_tint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tnumber_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const TBox *', box)
-    result = _lib.nad_tnumber_tbox(temp_converted, box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.nad_tpoint_geo(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tpoint_stbox(temp: 'const Temporal *', box: 'const STBox *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    box_converted = _ffi.cast('const STBox *', box)
-    result = _lib.nad_tpoint_stbox(temp_converted, box_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nad_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.nad_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nai_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'TInstant *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.nai_tpoint_geo(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def nai_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'TInstant *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.nai_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def shortestline_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'GSERIALIZED **':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    out_result = _ffi.new('GSERIALIZED **')
-    result = _lib.shortestline_tpoint_geo(temp_converted, gs_converted, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def shortestline_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'GSERIALIZED **':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    out_result = _ffi.new('GSERIALIZED **')
-    result = _lib.shortestline_tpoint_tpoint(temp1_converted, temp2_converted, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
-def tbool_always_eq(temp: 'const Temporal *', b: bool) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_always_eq(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_ever_eq(temp: 'const Temporal *', b: bool) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_ever_eq(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_always_eq(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_always_eq(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_always_le(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_always_le(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_always_lt(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_always_lt(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_ever_eq(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_ever_eq(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_ever_le(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_ever_le(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_ever_lt(temp: 'const Temporal *', d: float) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_ever_lt(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpoint_always_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tgeogpoint_always_eq(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeogpoint_ever_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tgeogpoint_ever_eq(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompoint_always_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tgeompoint_always_eq(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompoint_ever_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('GSERIALIZED *', gs)
-    result = _lib.tgeompoint_ever_eq(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_always_eq(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_always_eq(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_always_le(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_always_le(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_always_lt(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_always_lt(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_ever_eq(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_ever_eq(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_ever_le(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_ever_le(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tint_ever_lt(temp: 'const Temporal *', i: int) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_ever_lt(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_always_eq(temp: 'const Temporal *', value: 'Datum') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    value_converted = _ffi.cast('Datum', value)
-    result = _lib.tpoint_always_eq(temp_converted, value_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_ever_eq(temp: 'const Temporal *', value: 'Datum') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    value_converted = _ffi.cast('Datum', value)
-    result = _lib.tpoint_ever_eq(temp_converted, value_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_always_eq(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_always_eq(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_always_le(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_always_le(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_always_lt(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_always_lt(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_ever_eq(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_ever_eq(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_ever_le(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_ever_le(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_ever_lt(temp: 'const Temporal *', txt: str) -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.ttext_ever_lt(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_cmp(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_cmp(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_eq(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_eq(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_ge(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_ge(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_gt(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_gt(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_le(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_le(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_lt(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_lt(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_ne(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_ne(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_bool_tbool(b, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_geo_tpoint(geo: 'const GSERIALIZED *', tpoint: 'const Temporal *') -> 'Temporal *':
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
-    result = _lib.teq_geo_tpoint(geo_converted, tpoint_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_point_tgeogpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_point_tgeogpoint(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_point_tgeompoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_point_tgeompoint(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_tbool_bool(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def teq_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.teq_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tgeogpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.teq_tgeogpoint_point(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tgeompoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.teq_tgeompoint_point(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.teq_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def teq_tpoint_geo(tpoint: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
-    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.teq_tpoint_geo(tpoint_converted, geo_converted)
-    return result if result != _ffi.NULL else None
-
-
-def teq_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.teq_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tge_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tge_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tge_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tge_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tge_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tge_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tge_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tge_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tge_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tge_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tge_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tge_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tge_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.tge_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgt_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgt_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tgt_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgt_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgt_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgt_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tgt_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.tgt_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tle_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tle_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tle_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tle_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tle_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tle_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tle_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tle_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tle_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tle_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tle_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tle_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tle_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.tle_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tlt_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tlt_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tlt_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tlt_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tlt_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tlt_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tlt_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.tlt_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_bool_tbool(b, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_float_tfloat(d, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_geo_tpoint(geo: 'const GSERIALIZED *', tpoint: 'const Temporal *') -> 'Temporal *':
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
-    result = _lib.tne_geo_tpoint(geo_converted, tpoint_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_int_tint(i, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_point_tgeogpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_point_tgeogpoint(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_point_tgeompoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_point_tgeompoint(gs_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_tbool_bool(temp_converted, b)
-    return result if result != _ffi.NULL else None
-
-
-def tne_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tne_temporal_temporal(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
-    txt_converted = cstring2text(txt)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_text_ttext(txt_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_tfloat_float(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tgeogpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.tne_tgeogpoint_point(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tgeompoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.tne_tgeompoint_point(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tne_tint_int(temp_converted, i)
-    return result if result != _ffi.NULL else None
-
-
-def tne_tpoint_geo(tpoint: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
-    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.tne_tpoint_geo(tpoint_converted, geo_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tne_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    txt_converted = cstring2text(txt)
-    result = _lib.tne_ttext_text(temp_converted, txt_converted)
-    return result if result != _ffi.NULL else None
-
-
-def bearing_point_point(geo1: 'const GSERIALIZED *', geo2: 'const GSERIALIZED *') -> 'double':
-    geo1_converted = _ffi.cast('const GSERIALIZED *', geo1)
-    geo2_converted = _ffi.cast('const GSERIALIZED *', geo2)
-    out_result = _ffi.new('double *')
-    result = _lib.bearing_point_point(geo1_converted, geo2_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def bearing_tpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *', invert: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.bearing_tpoint_point(temp_converted, gs_converted, invert)
-    return result if result != _ffi.NULL else None
-
-
-def bearing_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.bearing_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_angular_difference(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_angular_difference(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_azimuth(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_azimuth(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_convex_hull(temp: 'const Temporal *') -> 'GSERIALIZED *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_convex_hull(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_cumulative_length(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_cumulative_length(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_direction(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    out_result = _ffi.new('double *')
-    result = _lib.tpoint_direction(temp_converted, out_result)
-    if result:
-        return out_result[0] if out_result[0] != _ffi.NULL else None
-    return None
-
-
-def tpoint_get_coord(temp: 'const Temporal *', coord: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_get_coord(temp_converted, coord)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_is_simple(temp: 'const Temporal *') -> 'bool':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_is_simple(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_length(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_length(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_speed(temp: 'const Temporal *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_speed(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_srid(temp: 'const Temporal *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_srid(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_stboxes(temp: 'const Temporal *') -> "Tuple['STBox *', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tpoint_stboxes(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tpoint_trajectory(temp: 'const Temporal *') -> 'GSERIALIZED *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_trajectory(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geo_expand_space(gs: 'const GSERIALIZED *', d: float) -> 'STBox *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.geo_expand_space(gs_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tgeompoint_tgeogpoint(temp: 'const Temporal *', oper: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tgeompoint_tgeogpoint(temp_converted, oper)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_expand_space(temp: 'const Temporal *', d: float) -> 'STBox *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_expand_space(temp_converted, d)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_make_simple(temp: 'const Temporal *') -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    count = _ffi.new('int *')
-    result = _lib.tpoint_make_simple(temp_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tpoint_set_srid(temp: 'const Temporal *', srid: int) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    srid_converted = _ffi.cast('int32', srid)
-    result = _lib.tpoint_set_srid(temp_converted, srid_converted)
-    return result if result != _ffi.NULL else None
-
-
-def econtains_geo_tpoint(geo: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'int':
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.econtains_geo_tpoint(geo_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def edisjoint_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.edisjoint_tpoint_geo(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def edisjoint_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.edisjoint_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def edwithin_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', dist: float) -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.edwithin_tpoint_geo(temp_converted, gs_converted, dist)
-    return result if result != _ffi.NULL else None
-
-
-def edwithin_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *', dist: float) -> 'int':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.edwithin_tpoint_tpoint(temp1_converted, temp2_converted, dist)
-    return result if result != _ffi.NULL else None
-
-
-def eintersects_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.eintersects_tpoint_geo(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def eintersects_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.eintersects_tpoint_tpoint(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def etouches_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.etouches_tpoint_geo(temp_converted, gs_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tcontains_geo_tpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *', restr: bool, atvalue: bool) -> 'Temporal *':
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tcontains_geo_tpoint(gs_converted, temp_converted, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def tdisjoint_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.tdisjoint_tpoint_geo(temp_converted, geo_converted, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def tdwithin_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', dist: float, restr: bool, atvalue: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.tdwithin_tpoint_geo(temp_converted, gs_converted, dist, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def tdwithin_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *', dist: float, restr: bool, atvalue: bool) -> 'Temporal *':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.tdwithin_tpoint_tpoint(temp1_converted, temp2_converted, dist, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def tintersects_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.tintersects_tpoint_geo(temp_converted, geo_converted, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def ttouches_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
-    result = _lib.ttouches_tpoint_geo(temp_converted, gs_converted, restr, atvalue)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_tand_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_tand_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tbool_tor_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tbool_tor_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_extent_transfn(p: "Optional['Span *']", temp: 'const Temporal *') -> 'Span *':
-    p_converted = _ffi.cast('Span *', p) if p is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_extent_transfn(p_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_tagg_finalfn(state: 'SkipList *') -> 'Temporal *':
-    state_converted = _ffi.cast('SkipList *', state)
-    result = _lib.temporal_tagg_finalfn(state_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_tcount_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_tcount_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_tmax_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_tmin_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tfloat_tsum_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tfloat_tsum_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_tmax_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_tmin_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_tsum_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tint_tsum_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_extent_transfn(box: "Optional['TBox *']", temp: 'const Temporal *') -> 'TBox *':
-    box_converted = _ffi.cast('TBox *', box) if box is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_extent_transfn(box_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_integral(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_integral(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_tavg_finalfn(state: 'SkipList *') -> 'Temporal *':
-    state_converted = _ffi.cast('SkipList *', state)
-    result = _lib.tnumber_tavg_finalfn(state_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_tavg_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_tavg_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tnumber_twavg(temp: 'const Temporal *') -> 'double':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tnumber_twavg(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_extent_transfn(box: "Optional['STBox *']", temp: 'const Temporal *') -> 'STBox *':
-    box_converted = _ffi.cast('STBox *', box) if box is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_extent_transfn(box_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_tcentroid_finalfn(state: 'SkipList *') -> 'Temporal *':
-    state_converted = _ffi.cast('SkipList *', state)
-    result = _lib.tpoint_tcentroid_finalfn(state_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_tcentroid_transfn(state: 'SkipList *', temp: 'Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state)
-    temp_converted = _ffi.cast('Temporal *', temp)
-    result = _lib.tpoint_tcentroid_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_twcentroid(temp: 'const Temporal *') -> 'GSERIALIZED *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.tpoint_twcentroid(temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_tmax_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def ttext_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
-    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.ttext_tmin_transfn(state_converted, temp_converted)
-    return result if result != _ffi.NULL else None
-
-
-def float_bucket(value: float, size: float, origin: float) -> 'double':
-    result = _lib.float_bucket(value, size, origin)
-    return result if result != _ffi.NULL else None
-
-
-def floatspan_bucket_list(bounds: 'const Span *', size: float, origin: float, newcount: 'int *') -> 'Span *':
-    bounds_converted = _ffi.cast('const Span *', bounds)
-    newcount_converted = _ffi.cast('int *', newcount)
-    result = _lib.floatspan_bucket_list(bounds_converted, size, origin, newcount_converted)
-    return result if result != _ffi.NULL else None
-
-
-def int_bucket(value: int, size: int, origin: int) -> 'int':
-    result = _lib.int_bucket(value, size, origin)
-    return result if result != _ffi.NULL else None
-
-
-def intspan_bucket_list(bounds: 'const Span *', size: int, origin: int, newcount: 'int *') -> 'Span *':
-    bounds_converted = _ffi.cast('const Span *', bounds)
-    newcount_converted = _ffi.cast('int *', newcount)
-    result = _lib.intspan_bucket_list(bounds_converted, size, origin, newcount_converted)
-    return result if result != _ffi.NULL else None
-
-
-def period_bucket_list(bounds: 'const Span *', duration: 'const Interval *', origin: int, newcount: 'int *') -> 'Span *':
-    bounds_converted = _ffi.cast('const Span *', bounds)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    origin_converted = _ffi.cast('TimestampTz', origin)
-    newcount_converted = _ffi.cast('int *', newcount)
-    result = _lib.period_bucket_list(bounds_converted, duration_converted, origin_converted, newcount_converted)
-    return result if result != _ffi.NULL else None
-
-
-def stbox_tile_list(bounds: 'const STBox *', xsize: float, ysize: float, zsize: float, duration: "Optional['const Interval *']", sorigin: 'GSERIALIZED *', torigin: int) -> "Tuple['STBox *', 'int *']":
-    bounds_converted = _ffi.cast('const STBox *', bounds)
-    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
-    sorigin_converted = _ffi.cast('GSERIALIZED *', sorigin)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    cellcount = _ffi.new('int **')
-    result = _lib.stbox_tile_list(bounds_converted, xsize, ysize, zsize, duration_converted, sorigin_converted, torigin_converted, cellcount)
-    return result if result != _ffi.NULL else None, cellcount[0]
-
-
-def tbox_tile_list(bounds: 'const TBox *', xsize: float, duration: 'const Interval *', xorigin: 'Optional[float]', torigin: "Optional[int]") -> "Tuple['TBox *', 'int', 'int']":
-    bounds_converted = _ffi.cast('const TBox *', bounds)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    xorigin_converted = xorigin if xorigin is not None else _ffi.NULL
-    torigin_converted = _ffi.cast('TimestampTz', torigin) if torigin is not None else _ffi.NULL
-    rows = _ffi.new('int *')
-    columns = _ffi.new('int *')
-    result = _lib.tbox_tile_list(bounds_converted, xsize, duration_converted, xorigin_converted, torigin_converted, rows, columns)
-    return result if result != _ffi.NULL else None, rows[0], columns[0]
-
-
-def temporal_time_split(temp: 'Temporal *', duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('Temporal *', temp)
-    duration_converted = _ffi.cast('Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    newcount = _ffi.new('int *')
-    result = _lib.temporal_time_split(temp_converted, duration_converted, torigin_converted, newcount)
-    return result if result != _ffi.NULL else None, newcount[0]
-
-
-def tfloat_value_split(temp: 'Temporal *', size: float, origin: float) -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('Temporal *', temp)
-    newcount = _ffi.new('int *')
-    result = _lib.tfloat_value_split(temp_converted, size, origin, newcount)
-    return result if result != _ffi.NULL else None, newcount[0]
-
-
-def tfloat_value_time_split(temp: 'Temporal *', size: float, vorigin: float, duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('Temporal *', temp)
-    duration_converted = _ffi.cast('Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    newcount = _ffi.new('int *')
-    result = _lib.tfloat_value_time_split(temp_converted, size, vorigin, duration_converted, torigin_converted, newcount)
-    return result if result != _ffi.NULL else None, newcount[0]
-
-
-def timestamptz_bucket(timestamp: int, duration: 'const Interval *', origin: int) -> 'TimestampTz':
-    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
-    duration_converted = _ffi.cast('const Interval *', duration)
-    origin_converted = _ffi.cast('TimestampTz', origin)
-    result = _lib.timestamptz_bucket(timestamp_converted, duration_converted, origin_converted)
-    return result if result != _ffi.NULL else None
-
-
-def tint_value_split(temp: 'Temporal *', size: int, origin: int) -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('Temporal *', temp)
-    newcount = _ffi.new('int *')
-    result = _lib.tint_value_split(temp_converted, size, origin, newcount)
-    return result if result != _ffi.NULL else None, newcount[0]
-
-
-def tint_value_time_split(temp: 'Temporal *', size: int, vorigin: int, duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
-    temp_converted = _ffi.cast('Temporal *', temp)
-    duration_converted = _ffi.cast('Interval *', duration)
-    torigin_converted = _ffi.cast('TimestampTz', torigin)
-    newcount = _ffi.new('int *')
-    result = _lib.tint_value_time_split(temp_converted, size, vorigin, duration_converted, torigin_converted, newcount)
-    return result if result != _ffi.NULL else None, newcount[0]
-
-
-def temporal_dyntimewarp_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_dyntimewarp_distance(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_dyntimewarp_path(temp1: 'const Temporal *', temp2: 'const Temporal *') -> "Tuple['Match *', 'int']":
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    count = _ffi.new('int *')
-    result = _lib.temporal_dyntimewarp_path(temp1_converted, temp2_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_frechet_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_frechet_distance(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_frechet_path(temp1: 'const Temporal *', temp2: 'const Temporal *') -> "Tuple['Match *', 'int']":
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    count = _ffi.new('int *')
-    result = _lib.temporal_frechet_path(temp1_converted, temp2_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def temporal_hausdorff_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
-    temp1_converted = _ffi.cast('const Temporal *', temp1)
-    temp2_converted = _ffi.cast('const Temporal *', temp2)
-    result = _lib.temporal_hausdorff_distance(temp1_converted, temp2_converted)
-    return result if result != _ffi.NULL else None
-
-
-def geo_to_tpoint(geo: 'const GSERIALIZED *') -> 'Temporal *':
-    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
-    result = _lib.geo_to_tpoint(geo_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_simplify_min_dist(temp: 'const Temporal *', dist: float) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_simplify_min_dist(temp_converted, dist)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_simplify_min_tdelta(temp: 'const Temporal *', mint: 'const Interval *') -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    mint_converted = _ffi.cast('const Interval *', mint)
-    result = _lib.temporal_simplify_min_tdelta(temp_converted, mint_converted)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_simplify_dp(temp: 'const Temporal *', eps_dist: float, synchronized: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_simplify_dp(temp_converted, eps_dist, synchronized)
-    return result if result != _ffi.NULL else None
-
-
-def temporal_simplify_max_dist(temp: 'const Temporal *', eps_dist: float, synchronized: bool) -> 'Temporal *':
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    result = _lib.temporal_simplify_max_dist(temp_converted, eps_dist, synchronized)
-    return result if result != _ffi.NULL else None
-
-
-def tpoint_AsMVTGeom(temp: 'const Temporal *', bounds: 'const STBox *', extent: 'int32_t', buffer: 'int32_t', clip_geom: bool, geom: 'GSERIALIZED **', timesarr: 'int64 **') -> "Tuple['bool', 'int']":
-    temp_converted = _ffi.cast('const Temporal *', temp)
-    bounds_converted = _ffi.cast('const STBox *', bounds)
-    extent_converted = _ffi.cast('int32_t', extent)
-    buffer_converted = _ffi.cast('int32_t', buffer)
-    geom_converted = [_ffi.cast('GSERIALIZED *', x) for x in geom]
-    timesarr_converted = [_ffi.cast('int64 *', x) for x in timesarr]
-    count = _ffi.new('int *')
-    result = _lib.tpoint_AsMVTGeom(temp_converted, bounds_converted, extent_converted, buffer_converted, clip_geom, geom_converted, timesarr_converted, count)
-    return result if result != _ffi.NULL else None, count[0]
-
-
-def tpoint_to_geo_meas(tpoint: 'const Temporal *', measure: 'const Temporal *', segmentize: bool) -> 'GSERIALIZED **':
-    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
-    measure_converted = _ffi.cast('const Temporal *', measure)
-    out_result = _ffi.new('GSERIALIZED **')
-    result = _lib.tpoint_to_geo_meas(tpoint_converted, measure_converted, segmentize, out_result)
-    if result:
-        return out_result if out_result != _ffi.NULL else None
-    return None
-
-
+from datetime import datetime, timedelta
+from typing import Any, Tuple, Optional, List, Union
+
+import _meos_cffi
+import postgis as pg
+import shapely.geometry as spg
+from dateutil.parser import parse
+from shapely import wkt, wkb, get_srid
+from shapely.geometry.base import BaseGeometry
+from spans.types import floatrange, intrange
+
+_ffi = _meos_cffi.ffi
+_lib = _meos_cffi.lib
+
+
+def create_pointer(object: 'Any', type: str) -> 'Any *':
+    return _ffi.new(f'{type} *', object)
+    
+
+def get_address(value: 'Any') -> 'Any *':
+    return _ffi.addressof(value)
+
+
+def datetime_to_timestamptz(dt: datetime) -> int:
+    return _lib.pg_timestamptz_in(dt.strftime('%Y-%m-%d %H:%M:%S%z').encode('utf-8'), -1)
+
+
+def timestamptz_to_datetime(ts: int) -> datetime:
+    return parse(pg_timestamptz_out(ts))
+
+
+def timedelta_to_interval(td: timedelta) -> Any:
+    return _ffi.new('Interval *', {'time': td.microseconds + td.seconds * 1000000, 'day': td.days, 'month': 0})
+
+
+def interval_to_timedelta(interval: Any) -> timedelta:
+    # TODO fix for months/years
+    return timedelta(days=interval.day, microseconds=interval.time)
+
+
+def geometry_to_gserialized(geom: Union[pg.Geometry, BaseGeometry], geodetic: Optional[bool] = None) -> 'GSERIALIZED *':
+    if isinstance(geom, pg.Geometry):
+        text = geom.to_ewkb()
+        if geom.has_srid():
+            text = f'SRID={geom.srid};{text}'
+    elif isinstance(geom, BaseGeometry):
+        text = wkb.dumps(geom, hex=True)
+        if get_srid(geom) > 0:
+            text = f'SRID={get_srid(geom)};{text}'
+    else:
+        raise TypeError('Parameter geom must be either a PostGIS Geometry or a Shapely BaseGeometry')
+    gs = gserialized_in(text, -1)
+    if geodetic is not None:
+        # GFlags is an 8-bit integer, where the 4th bit is the geodetic flag (0x80)
+        # If geodetic is True, then set the 4th bit to 1, otherwise set it to 0
+        gs.gflags = (gs.gflags | 0x08) if geodetic else (gs.gflags & 0xF7)
+    return gs
+
+
+def gserialized_to_shapely_point(geom: 'const GSERIALIZED *', precision: int = 6) -> spg.Point:
+    return wkt.loads(gserialized_as_text(geom, precision))
+
+
+def gserialized_to_shapely_geometry(geom: 'const GSERIALIZED *', precision: int = 6) -> BaseGeometry:
+    return wkt.loads(gserialized_as_text(geom, precision))
+
+
+def intrange_to_intspan(irange: intrange) -> 'Span *':
+    return intspan_make(irange.lower, irange.upper, irange.lower_inc, irange.upper_inc)
+
+
+def intspan_to_intrange(ispan: 'Span *') -> intrange:
+    return intrange(intspan_lower(ispan), intspan_upper(ispan), ispan.lower_inc, ispan.upper_inc)
+
+
+def floatrange_to_floatspan(frange: floatrange) -> 'Span *':
+    return floatspan_make(frange.lower, frange.upper, frange.lower_inc, frange.upper_inc)
+
+
+def floatspan_to_floatrange(fspan: 'Span *') -> floatrange:
+    return floatrange(floatspan_lower(fspan), floatspan_upper(fspan), fspan.lower_inc, fspan.upper_inc)
+
+
+def as_tinstant(temporal: 'Temporal *') -> 'TInstant *':
+    return _ffi.cast('TInstant *', temporal)
+
+
+def as_tsequence(temporal: 'Temporal *') -> 'TSequence *':
+    return _ffi.cast('TSequence *', temporal)
+
+
+def as_tsequenceset(temporal: 'Temporal *') -> 'TSequenceSet *':
+    return _ffi.cast('TSequenceSet *', temporal)
+
+
+# -----------------------------------------------------------------------------
+# ----------------------End of manually-defined functions----------------------
+# -----------------------------------------------------------------------------
+
+
+def lwpoint_make(srid: 'int32_t', hasz: int, hasm: int, p: 'const POINT4D *') -> 'LWPOINT *':
+    srid_converted = _ffi.cast('int32_t', srid)
+    p_converted = _ffi.cast('const POINT4D *', p)
+    result = _lib.lwpoint_make(srid_converted, hasz, hasm, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwgeom_from_gserialized(g: 'const GSERIALIZED *') -> 'LWGEOM *':
+    g_converted = _ffi.cast('const GSERIALIZED *', g)
+    result = _lib.lwgeom_from_gserialized(g_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_from_lwgeom(geom: 'LWGEOM *') -> 'GSERIALIZED *':
+    geom_converted = _ffi.cast('LWGEOM *', geom)
+    size_converted = _ffi.NULL
+    result = _lib.gserialized_from_lwgeom(geom_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwgeom_get_srid(geom: 'const LWGEOM *') -> 'int32_t':
+    geom_converted = _ffi.cast('const LWGEOM *', geom)
+    result = _lib.lwgeom_get_srid(geom_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwpoint_get_x(point: 'const LWPOINT *') -> 'double':
+    point_converted = _ffi.cast('const LWPOINT *', point)
+    result = _lib.lwpoint_get_x(point_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwpoint_get_y(point: 'const LWPOINT *') -> 'double':
+    point_converted = _ffi.cast('const LWPOINT *', point)
+    result = _lib.lwpoint_get_y(point_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwpoint_get_z(point: 'const LWPOINT *') -> 'double':
+    point_converted = _ffi.cast('const LWPOINT *', point)
+    result = _lib.lwpoint_get_z(point_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwpoint_get_m(point: 'const LWPOINT *') -> 'double':
+    point_converted = _ffi.cast('const LWPOINT *', point)
+    result = _lib.lwpoint_get_m(point_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwgeom_has_z(geom: 'const LWGEOM *') -> 'int':
+    geom_converted = _ffi.cast('const LWGEOM *', geom)
+    result = _lib.lwgeom_has_z(geom_converted)
+    return result if result != _ffi.NULL else None
+
+
+def lwgeom_has_m(geom: 'const LWGEOM *') -> 'int':
+    geom_converted = _ffi.cast('const LWGEOM *', geom)
+    result = _lib.lwgeom_has_m(geom_converted)
+    return result if result != _ffi.NULL else None
+
+
+def meos_initialize(tz_str: "Optional[str]") -> None:
+    tz_str_converted = tz_str.encode('utf-8') if tz_str is not None else _ffi.NULL
+    _lib.meos_initialize(tz_str_converted)
+
+
+def meos_finalize() -> None:
+    _lib.meos_finalize()
+
+
+def bool_in(in_str: str) -> 'bool':
+    in_str_converted = in_str.encode('utf-8')
+    result = _lib.bool_in(in_str_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bool_out(b: bool) -> str:
+    result = _lib.bool_out(b)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def cstring2text(cstring: str) -> 'text *':
+    cstring_converted = cstring.encode('utf-8')
+    result = _lib.cstring2text(cstring_converted)
+    return result
+
+
+def pg_date_in(string: str) -> 'DateADT':
+    string_converted = string.encode('utf-8')
+    result = _lib.pg_date_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_date_out(date: 'DateADT') -> str:
+    date_converted = _ffi.cast('DateADT', date)
+    result = _lib.pg_date_out(date_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_cmp(interval1: 'const Interval *', interval2: 'const Interval *') -> 'int':
+    interval1_converted = _ffi.cast('const Interval *', interval1)
+    interval2_converted = _ffi.cast('const Interval *', interval2)
+    result = _lib.pg_interval_cmp(interval1_converted, interval2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_in(string: str, typmod: int) -> 'Interval *':
+    string_converted = string.encode('utf-8')
+    typmod_converted = _ffi.cast('int32', typmod)
+    result = _lib.pg_interval_in(string_converted, typmod_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_make(years: int, months: int, weeks: int, days: int, hours: int, mins: int, secs: float) -> 'Interval *':
+    years_converted = _ffi.cast('int32', years)
+    months_converted = _ffi.cast('int32', months)
+    weeks_converted = _ffi.cast('int32', weeks)
+    days_converted = _ffi.cast('int32', days)
+    hours_converted = _ffi.cast('int32', hours)
+    mins_converted = _ffi.cast('int32', mins)
+    result = _lib.pg_interval_make(years_converted, months_converted, weeks_converted, days_converted, hours_converted, mins_converted, secs)
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_mul(span: 'const Interval *', factor: float) -> 'Interval *':
+    span_converted = _ffi.cast('const Interval *', span)
+    result = _lib.pg_interval_mul(span_converted, factor)
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_out(span: 'const Interval *') -> str:
+    span_converted = _ffi.cast('const Interval *', span)
+    result = _lib.pg_interval_out(span_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def pg_interval_pl(span1: 'const Interval *', span2: 'const Interval *') -> 'Interval *':
+    span1_converted = _ffi.cast('const Interval *', span1)
+    span2_converted = _ffi.cast('const Interval *', span2)
+    result = _lib.pg_interval_pl(span1_converted, span2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_time_in(string: str, typmod: int) -> 'TimeADT':
+    string_converted = string.encode('utf-8')
+    typmod_converted = _ffi.cast('int32', typmod)
+    result = _lib.pg_time_in(string_converted, typmod_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_time_out(time: 'TimeADT') -> str:
+    time_converted = _ffi.cast('TimeADT', time)
+    result = _lib.pg_time_out(time_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamp_in(string: str, typmod: int) -> 'Timestamp':
+    string_converted = string.encode('utf-8')
+    typmod_converted = _ffi.cast('int32', typmod)
+    result = _lib.pg_timestamp_in(string_converted, typmod_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamp_mi(dt1: int, dt2: int) -> 'Interval *':
+    dt1_converted = _ffi.cast('TimestampTz', dt1)
+    dt2_converted = _ffi.cast('TimestampTz', dt2)
+    result = _lib.pg_timestamp_mi(dt1_converted, dt2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamp_mi_interval(timestamp: int, span: 'const Interval *') -> 'TimestampTz':
+    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
+    span_converted = _ffi.cast('const Interval *', span)
+    result = _lib.pg_timestamp_mi_interval(timestamp_converted, span_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamp_out(dt: int) -> str:
+    dt_converted = _ffi.cast('Timestamp', dt)
+    result = _lib.pg_timestamp_out(dt_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamp_pl_interval(timestamp: int, span: 'const Interval *') -> 'TimestampTz':
+    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
+    span_converted = _ffi.cast('const Interval *', span)
+    result = _lib.pg_timestamp_pl_interval(timestamp_converted, span_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamptz_in(string: str, typmod: int) -> 'TimestampTz':
+    string_converted = string.encode('utf-8')
+    typmod_converted = _ffi.cast('int32', typmod)
+    result = _lib.pg_timestamptz_in(string_converted, typmod_converted)
+    return result if result != _ffi.NULL else None
+
+
+def pg_timestamptz_out(dt: int) -> str:
+    dt_converted = _ffi.cast('TimestampTz', dt)
+    result = _lib.pg_timestamptz_out(dt_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def text2cstring(textptr: 'text *') -> str:
+    result = _lib.text2cstring(textptr)
+    result = _ffi.string(result).decode('utf-8')
+    return result
+
+
+def gserialized_as_ewkb(geom: 'const GSERIALIZED *', type: str) -> 'bytea *':
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    type_converted = type.encode('utf-8')
+    result = _lib.gserialized_as_ewkb(geom_converted, type_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_as_ewkt(geom: 'const GSERIALIZED *', precision: int) -> str:
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    result = _lib.gserialized_as_ewkt(geom_converted, precision)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_as_geojson(geom: 'const GSERIALIZED *', option: int, precision: int, srs: "Optional[str]") -> str:
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    srs_converted = srs.encode('utf-8') if srs is not None else _ffi.NULL
+    result = _lib.gserialized_as_geojson(geom_converted, option, precision, srs_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_as_hexewkb(geom: 'const GSERIALIZED *', type: str) -> str:
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    type_converted = type.encode('utf-8')
+    result = _lib.gserialized_as_hexewkb(geom_converted, type_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_as_text(geom: 'const GSERIALIZED *', precision: int) -> str:
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    result = _lib.gserialized_as_text(geom_converted, precision)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_from_ewkb(bytea_wkb: 'const bytea *', srid: int) -> 'GSERIALIZED *':
+    bytea_wkb_converted = _ffi.cast('const bytea *', bytea_wkb)
+    srid_converted = _ffi.cast('int32', srid)
+    result = _lib.gserialized_from_ewkb(bytea_wkb_converted, srid_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_from_geojson(geojson: str) -> 'GSERIALIZED *':
+    geojson_converted = geojson.encode('utf-8')
+    result = _lib.gserialized_from_geojson(geojson_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_from_hexewkb(wkt: str) -> 'GSERIALIZED *':
+    wkt_converted = wkt.encode('utf-8')
+    result = _lib.gserialized_from_hexewkb(wkt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_from_text(wkt: str, srid: int) -> 'GSERIALIZED *':
+    wkt_converted = wkt.encode('utf-8')
+    result = _lib.gserialized_from_text(wkt_converted, srid)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_in(input: str, geom_typmod: int) -> 'GSERIALIZED *':
+    input_converted = input.encode('utf-8')
+    geom_typmod_converted = _ffi.cast('int32', geom_typmod)
+    result = _lib.gserialized_in(input_converted, geom_typmod_converted)
+    return result if result != _ffi.NULL else None
+
+
+def gserialized_out(geom: 'const GSERIALIZED *') -> str:
+    geom_converted = _ffi.cast('const GSERIALIZED *', geom)
+    result = _lib.gserialized_out(geom_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def pgis_gserialized_same(geom1: 'const GSERIALIZED *', geom2: 'const GSERIALIZED *') -> 'bool':
+    geom1_converted = _ffi.cast('const GSERIALIZED *', geom1)
+    geom2_converted = _ffi.cast('const GSERIALIZED *', geom2)
+    result = _lib.pgis_gserialized_same(geom1_converted, geom2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.bigintset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_out(set: 'const Set *') -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.bigintset_out(set_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def bigintspan_in(string: str) -> 'Span *':
+    string_converted = string.encode('utf-8')
+    result = _lib.bigintspan_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspan_out(s: 'const Span *') -> str:
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.bigintspan_out(s_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def bigintspanset_in(string: str) -> 'SpanSet *':
+    string_converted = string.encode('utf-8')
+    result = _lib.bigintspanset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspanset_out(ss: 'const SpanSet *') -> str:
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.bigintspanset_out(ss_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def floatset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.floatset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatset_out(set: 'const Set *', maxdd: int) -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.floatset_out(set_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_in(string: str) -> 'Span *':
+    string_converted = string.encode('utf-8')
+    result = _lib.floatspan_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_out(s: 'const Span *', maxdd: int) -> str:
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.floatspan_out(s_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def floatspanset_in(string: str) -> 'SpanSet *':
+    string_converted = string.encode('utf-8')
+    result = _lib.floatspanset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspanset_out(ss: 'const SpanSet *', maxdd: int) -> str:
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.floatspanset_out(ss_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def geogset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.geogset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geogset_out(set: 'const Set *', maxdd: int) -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.geogset_out(set_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def geomset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.geomset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geomset_out(set: 'const Set *', maxdd: int) -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.geomset_out(set_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def geoset_as_ewkt(set: 'const Set *', maxdd: int) -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.geoset_as_ewkt(set_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def geoset_as_text(set: 'const Set *', maxdd: int) -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.geoset_as_text(set_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def intset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.intset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intset_out(set: 'const Set *') -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.intset_out(set_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def intspan_in(string: str) -> 'Span *':
+    string_converted = string.encode('utf-8')
+    result = _lib.intspan_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspan_out(s: 'const Span *') -> str:
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.intspan_out(s_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def intspanset_in(string: str) -> 'SpanSet *':
+    string_converted = string.encode('utf-8')
+    result = _lib.intspanset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspanset_out(ss: 'const SpanSet *') -> str:
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.intspanset_out(ss_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def period_in(string: str) -> 'Span *':
+    string_converted = string.encode('utf-8')
+    result = _lib.period_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_out(s: 'const Span *') -> str:
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.period_out(s_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def periodset_in(string: str) -> 'SpanSet *':
+    string_converted = string.encode('utf-8')
+    result = _lib.periodset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_out(ss: 'const SpanSet *') -> str:
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.periodset_out(ss_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def set_as_hexwkb(s: 'const Set *', variant: int) -> "Tuple[str, 'size_t *']":
+    s_converted = _ffi.cast('const Set *', s)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.set_as_hexwkb(s_converted, variant_converted, size_out)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def set_as_wkb(s: 'const Set *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    s_converted = _ffi.cast('const Set *', s)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.set_as_wkb(s_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def set_from_hexwkb(hexwkb: str) -> 'Set *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.set_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Set *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.set_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_out(s: 'const Set *', maxdd: int) -> str:
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_out(s_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def span_as_wkb(s: 'const Span *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    s_converted = _ffi.cast('const Span *', s)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.span_as_wkb(s_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def span_as_hexwkb(s: 'const Span *', variant: int) -> "Tuple[str, 'size_t *']":
+    s_converted = _ffi.cast('const Span *', s)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.span_as_hexwkb(s_converted, variant_converted, size_out)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def span_from_hexwkb(hexwkb: str) -> 'Span *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.span_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Span *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.span_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_out(s: 'const Span *', maxdd: int) -> str:
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_out(s_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def spanset_as_wkb(ss: 'const SpanSet *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.spanset_as_wkb(ss_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def spanset_as_hexwkb(ss: 'const SpanSet *', variant: int) -> "Tuple[str, 'size_t *']":
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.spanset_as_hexwkb(ss_converted, variant_converted, size_out)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def spanset_from_hexwkb(hexwkb: str) -> 'SpanSet *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.spanset_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'SpanSet *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.spanset_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_out(ss: 'const SpanSet *', maxdd: int) -> str:
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_out(ss_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def textset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.textset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def textset_out(set: 'const Set *') -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.textset_out(set_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_in(string: str) -> 'Set *':
+    string_converted = string.encode('utf-8')
+    result = _lib.timestampset_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_out(set: 'const Set *') -> str:
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.timestampset_out(set_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_make(values: 'const int64 *', count: int) -> 'Set *':
+    values_converted = _ffi.cast('const int64 *', values)
+    result = _lib.bigintset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspan_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
+    lower_converted = _ffi.cast('int64', lower)
+    upper_converted = _ffi.cast('int64', upper)
+    result = _lib.bigintspan_make(lower_converted, upper_converted, lower_inc, upper_inc)
+    return result if result != _ffi.NULL else None
+
+
+def floatset_make(values: 'const double *', count: int) -> 'Set *':
+    values_converted = _ffi.cast('const double *', values)
+    result = _lib.floatset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_make(lower: float, upper: float, lower_inc: bool, upper_inc: bool) -> 'Span *':
+    result = _lib.floatspan_make(lower, upper, lower_inc, upper_inc)
+    return result if result != _ffi.NULL else None
+
+
+def geogset_make(values: 'const GSERIALIZED **', count: int) -> 'Set *':
+    values_converted = [_ffi.cast('const GSERIALIZED *', x) for x in values]
+    result = _lib.geogset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def geomset_make(values: 'const GSERIALIZED **', count: int) -> 'Set *':
+    values_converted = [_ffi.cast('const GSERIALIZED *', x) for x in values]
+    result = _lib.geomset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def intset_make(values: 'const int *', count: int) -> 'Set *':
+    values_converted = _ffi.cast('const int *', values)
+    result = _lib.intset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def intspan_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
+    result = _lib.intspan_make(lower, upper, lower_inc, upper_inc)
+    return result if result != _ffi.NULL else None
+
+
+def period_make(lower: int, upper: int, lower_inc: bool, upper_inc: bool) -> 'Span *':
+    lower_converted = _ffi.cast('TimestampTz', lower)
+    upper_converted = _ffi.cast('TimestampTz', upper)
+    result = _lib.period_make(lower_converted, upper_converted, lower_inc, upper_inc)
+    return result if result != _ffi.NULL else None
+
+
+def set_copy(s: 'const Set *') -> 'Set *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_copy(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_copy(s: 'const Span *') -> 'Span *':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_copy(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_copy(ps: 'const SpanSet *') -> 'SpanSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.spanset_copy(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_make(spans: 'List[Span *]', normalize: bool) -> 'SpanSet *':
+    spans_converted = _ffi.new('Span []', spans)
+    result = _lib.spanset_make(spans_converted, len(spans), normalize)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_make_exp(spans: 'Span *', count: int, maxcount: int, normalize: bool, ordered: bool) -> 'SpanSet *':
+    spans_converted = _ffi.cast('Span *', spans)
+    result = _lib.spanset_make_exp(spans_converted, count, maxcount, normalize, ordered)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_make_free(spans: 'Span *', count: int, normalize: bool) -> 'SpanSet *':
+    spans_converted = _ffi.cast('Span *', spans)
+    result = _lib.spanset_make_free(spans_converted, count, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def textset_make(values: 'const text **', count: int) -> 'Set *':
+    values_converted = [_ffi.cast('const text *', x) for x in values]
+    result = _lib.textset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_make(values: List[int], count: int) -> 'Set *':
+    values_converted = [_ffi.cast('const TimestampTz', x) for x in values]
+    result = _lib.timestampset_make(values_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def bigint_to_bigintset(i: int) -> 'Set *':
+    i_converted = _ffi.cast('int64', i)
+    result = _lib.bigint_to_bigintset(i_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigint_to_bigintspan(i: int) -> 'Span *':
+    result = _lib.bigint_to_bigintspan(i)
+    return result if result != _ffi.NULL else None
+
+
+def bigint_to_bigintspanset(i: int) -> 'SpanSet *':
+    result = _lib.bigint_to_bigintspanset(i)
+    return result if result != _ffi.NULL else None
+
+
+def float_to_floatset(d: float) -> 'Set *':
+    result = _lib.float_to_floatset(d)
+    return result if result != _ffi.NULL else None
+
+
+def float_to_floatspan(d: float) -> 'Span *':
+    result = _lib.float_to_floatspan(d)
+    return result if result != _ffi.NULL else None
+
+
+def float_to_floatspanset(d: float) -> 'SpanSet *':
+    result = _lib.float_to_floatspanset(d)
+    return result if result != _ffi.NULL else None
+
+
+def int_to_intset(i: int) -> 'Set *':
+    result = _lib.int_to_intset(i)
+    return result if result != _ffi.NULL else None
+
+
+def int_to_intspan(i: int) -> 'Span *':
+    result = _lib.int_to_intspan(i)
+    return result if result != _ffi.NULL else None
+
+
+def int_to_intspanset(i: int) -> 'SpanSet *':
+    result = _lib.int_to_intspanset(i)
+    return result if result != _ffi.NULL else None
+
+
+def set_to_spanset(s: 'const Set *') -> 'SpanSet *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_to_spanset(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_to_spanset(s: 'const Span *') -> 'SpanSet *':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_to_spanset(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_to_period(t: int) -> 'Span *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_to_period(t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_to_periodset(t: int) -> 'SpanSet *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_to_periodset(t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_to_tstzset(t: int) -> 'Set *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_to_tstzset(t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_end_value(s: 'const Set *') -> 'int64':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.bigintset_end_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_start_value(s: 'const Set *') -> 'int64':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.bigintset_start_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintset_value_n(s: 'const Set *', n: int) -> 'int64':
+    s_converted = _ffi.cast('const Set *', s)
+    out_result = _ffi.new('int64 *')
+    result = _lib.bigintset_value_n(s_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def bigintset_values(s: 'const Set *') -> 'int64 *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.bigintset_values(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspan_lower(s: 'const Span *') -> 'int':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.bigintspan_lower(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspan_upper(s: 'const Span *') -> 'int':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.bigintspan_upper(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspanset_lower(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.bigintspanset_lower(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigintspanset_upper(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.bigintspanset_upper(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatset_end_value(s: 'const Set *') -> 'double':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.floatset_end_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatset_start_value(s: 'const Set *') -> 'double':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.floatset_start_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatset_value_n(s: 'const Set *', n: int) -> 'double':
+    s_converted = _ffi.cast('const Set *', s)
+    out_result = _ffi.new('double *')
+    result = _lib.floatset_value_n(s_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def floatset_values(s: 'const Set *') -> 'double *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.floatset_values(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_lower(s: 'const Span *') -> 'double':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.floatspan_lower(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_upper(s: 'const Span *') -> 'double':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.floatspan_upper(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspanset_lower(ss: 'const SpanSet *') -> 'double':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.floatspanset_lower(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspanset_upper(ss: 'const SpanSet *') -> 'double':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.floatspanset_upper(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geoset_srid(set: 'const Set *') -> 'int':
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.geoset_srid(set_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intset_end_value(s: 'const Set *') -> 'int':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.intset_end_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intset_start_value(s: 'const Set *') -> 'int':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.intset_start_value(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intset_value_n(s: 'const Set *', n: int) -> 'int':
+    s_converted = _ffi.cast('const Set *', s)
+    out_result = _ffi.new('int *')
+    result = _lib.intset_value_n(s_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def intset_values(s: 'const Set *') -> 'int *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.intset_values(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspan_lower(s: 'const Span *') -> 'int':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.intspan_lower(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspan_upper(s: 'const Span *') -> 'int':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.intspan_upper(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspanset_lower(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.intspanset_lower(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intspanset_upper(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.intspanset_upper(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_duration(s: 'const Span *') -> 'Interval *':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.period_duration(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_lower(p: 'const Span *') -> 'TimestampTz':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.period_lower(p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_upper(p: 'const Span *') -> 'TimestampTz':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.period_upper(p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_duration(ps: 'const SpanSet *', boundspan: bool) -> 'Interval *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_duration(ps_converted, boundspan)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_end_timestamp(ps: 'const SpanSet *') -> 'TimestampTz':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_end_timestamp(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_lower(ps: 'const SpanSet *') -> 'TimestampTz':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_lower(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_num_timestamps(ps: 'const SpanSet *') -> 'int':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_num_timestamps(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_start_timestamp(ps: 'const SpanSet *') -> 'TimestampTz':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_start_timestamp(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_timestamp_n(ps: 'const SpanSet *', n: int) -> int:
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.periodset_timestamp_n(ps_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def periodset_timestamps(ps: 'const SpanSet *') -> "Tuple['TimestampTz *', 'int']":
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    count = _ffi.new('int *')
+    result = _lib.periodset_timestamps(ps_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def periodset_upper(ps: 'const SpanSet *') -> 'TimestampTz':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_upper(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_hash(s: 'const Set *') -> 'uint32':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_hash(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_hash_extended(s: 'const Set *', seed: int) -> 'uint64':
+    s_converted = _ffi.cast('const Set *', s)
+    seed_converted = _ffi.cast('uint64', seed)
+    result = _lib.set_hash_extended(s_converted, seed_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_mem_size(s: 'const Set *') -> 'int':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_mem_size(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_num_values(s: 'const Set *') -> 'int':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_num_values(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_span(s: 'const Set *') -> 'Span *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.set_span(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_hash(s: 'const Span *') -> 'uint32':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_hash(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_hash_extended(s: 'const Span *', seed: int) -> 'uint64':
+    s_converted = _ffi.cast('const Span *', s)
+    seed_converted = _ffi.cast('uint64', seed)
+    result = _lib.span_hash_extended(s_converted, seed_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_lower_inc(s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_lower_inc(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_upper_inc(s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_upper_inc(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_width(s: 'const Span *') -> 'double':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.span_width(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_end_span(ss: 'const SpanSet *') -> 'Span *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_end_span(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_hash(ps: 'const SpanSet *') -> 'uint32':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.spanset_hash(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_hash_extended(ps: 'const SpanSet *', seed: int) -> 'uint64':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    seed_converted = _ffi.cast('uint64', seed)
+    result = _lib.spanset_hash_extended(ps_converted, seed_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_lower_inc(ss: 'const SpanSet *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_lower_inc(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_mem_size(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_mem_size(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_num_spans(ss: 'const SpanSet *') -> 'int':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_num_spans(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_span(ss: 'const SpanSet *') -> 'Span *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_span(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_span_n(ss: 'const SpanSet *', i: int) -> 'Span *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_span_n(ss_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_spans(ss: 'const SpanSet *') -> 'const Span **':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_spans(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_start_span(ss: 'const SpanSet *') -> 'Span *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_start_span(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_upper_inc(ss: 'const SpanSet *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_upper_inc(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_width(ss: 'const SpanSet *') -> 'double':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_width(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spatialset_stbox(s: 'const Set *') -> 'STBox *':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.spatialset_stbox(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_end_timestamp(ts: 'const Set *') -> 'TimestampTz':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.timestampset_end_timestamp(ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_start_timestamp(ts: 'const Set *') -> 'TimestampTz':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.timestampset_start_timestamp(ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_timestamp_n(ts: 'const Set *', n: int) -> int:
+    ts_converted = _ffi.cast('const Set *', ts)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.timestampset_timestamp_n(ts_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def timestampset_values(ts: 'const Set *') -> 'TimestampTz *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.timestampset_values(ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_set_intspan(s1: 'const Span *', s2: 'Span *') -> None:
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('Span *', s2)
+    _lib.floatspan_set_intspan(s1_converted, s2_converted)
+
+
+def intspan_set_floatspan(s1: 'const Span *', s2: 'Span *') -> None:
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('Span *', s2)
+    _lib.intspan_set_floatspan(s1_converted, s2_converted)
+
+
+def numspan_set_floatspan(s1: 'const Span *', s2: 'Span *') -> None:
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('Span *', s2)
+    _lib.numspan_set_floatspan(s1_converted, s2_converted)
+
+
+def period_tprecision(s: 'const Span *', duration: 'const Interval *', torigin: int) -> 'Span *':
+    s_converted = _ffi.cast('const Span *', s)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    result = _lib.period_tprecision(s_converted, duration_converted, torigin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_tprecision(ss: 'const SpanSet *', duration: 'const Interval *', torigin: int) -> 'SpanSet *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    result = _lib.periodset_tprecision(ss_converted, duration_converted, torigin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_shift_tscale(p: 'const Span *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Span *':
+    p_converted = _ffi.cast('const Span *', p)
+    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
+    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
+    result = _lib.period_shift_tscale(p_converted, shift_converted, duration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_shift_tscale(ps: 'const SpanSet *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'SpanSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
+    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
+    result = _lib.periodset_shift_tscale(ps_converted, shift_converted, duration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_shift(s: 'const Set *', shift: 'Datum') -> 'Set *':
+    s_converted = _ffi.cast('const Set *', s)
+    shift_converted = _ffi.cast('Datum', shift)
+    result = _lib.set_shift(s_converted, shift_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_expand(s1: 'const Span *', s2: 'Span *') -> None:
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('Span *', s2)
+    _lib.span_expand(s1_converted, s2_converted)
+
+
+def timestamp_tprecision(t: int, duration: 'const Interval *', torigin: int) -> 'TimestampTz':
+    t_converted = _ffi.cast('TimestampTz', t)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    result = _lib.timestamp_tprecision(t_converted, duration_converted, torigin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_shift_tscale(ts: 'const Set *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Set *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
+    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
+    result = _lib.timestampset_shift_tscale(ts_converted, shift_converted, duration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_bigintspan_bigint(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    i_converted = _ffi.cast('int64', i)
+    result = _lib.adjacent_bigintspan_bigint(s_converted, i_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_bigintspanset_bigint(ss: 'const SpanSet *', i: int) -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    i_converted = _ffi.cast('int64', i)
+    result = _lib.adjacent_bigintspanset_bigint(ss_converted, i_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.adjacent_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.adjacent_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_period_timestamp(p: 'const Span *', t: int) -> 'bool':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.adjacent_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.adjacent_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.adjacent_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.adjacent_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.adjacent_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_bigint_bigintset(i: int, s: 'const Set *') -> 'bool':
+    i_converted = _ffi.cast('int64', i)
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.contained_bigint_bigintset(i_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_bigint_bigintspan(i: int, s: 'const Span *') -> 'bool':
+    i_converted = _ffi.cast('int64', i)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contained_bigint_bigintspan(i_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_bigint_bigintspanset(i: int, ss: 'const SpanSet *') -> 'bool':
+    i_converted = _ffi.cast('int64', i)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.contained_bigint_bigintspanset(i_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_float_floatset(d: float, s: 'const Set *') -> 'bool':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.contained_float_floatset(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_float_floatspan(d: float, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contained_float_floatspan(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_float_floatspanset(d: float, ss: 'const SpanSet *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.contained_float_floatspanset(d, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_int_intset(i: int, s: 'const Set *') -> 'bool':
+    s_converted = _ffi.cast('const Set *', s)
+    result = _lib.contained_int_intset(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_int_intspan(i: int, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contained_int_intspan(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.contained_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.contained_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.contained_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contained_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.contained_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_timestamp_period(t: int, p: 'const Span *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.contained_timestamp_period(t_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.contained_timestamp_timestampset(t_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contains_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def contains_floatspanset_float(ss: 'const SpanSet *', d: float) -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.contains_floatspanset_float(ss_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def contains_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contains_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def contains_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.contains_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_period_timestamp(p: 'const Span *', t: int) -> 'bool':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.contains_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.contains_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.contains_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.contains_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.contains_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.contains_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_timestampset_timestamp(ts: 'const Set *', t: int) -> 'bool':
+    ts_converted = _ffi.cast('const Set *', ts)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.contains_timestampset_timestamp(ts_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.overlaps_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.overlaps_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overlaps_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.overlaps_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def after_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.after_timestamp_timestampset(t_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def before_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.before_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def before_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.before_timestamp_timestampset(t_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_float_floatspan(d: float, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.left_float_floatspan(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.left_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def left_int_intspan(i: int, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.left_int_intspan(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.left_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def left_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.left_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.left_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.left_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.left_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.left_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_period_timestamp(p: 'const Span *', t: int) -> 'bool':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.overafter_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.overafter_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_timestamp_period(t: int, p: 'const Span *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.overafter_timestamp_period(t_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_timestamp_periodset(t: int, ps: 'const SpanSet *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.overafter_timestamp_periodset(t_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.overafter_timestamp_timestampset(t_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_period_timestamp(p: 'const Span *', t: int) -> 'bool':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.overbefore_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'bool':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.overbefore_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_timestamp_period(t: int, p: 'const Span *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.overbefore_timestamp_period(t_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_timestamp_periodset(t: int, ps: 'const SpanSet *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.overbefore_timestamp_periodset(t_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_timestamp_timestampset(t: int, ts: 'const Set *') -> 'bool':
+    t_converted = _ffi.cast('TimestampTz', t)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.overbefore_timestamp_timestampset(t_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_float_floatspan(d: float, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overleft_float_floatspan(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overleft_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_int_intspan(i: int, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overleft_int_intspan(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overleft_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.overleft_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.overleft_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.overleft_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overleft_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.overleft_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_float_floatspan(d: float, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overright_float_floatspan(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overright_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def overright_int_intspan(i: int, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overright_int_intspan(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overright_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def overright_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.overright_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.overright_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.overright_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.overright_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.overright_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_float_floatspan(d: float, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.right_float_floatspan(d, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_floatspan_float(s: 'const Span *', d: float) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.right_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def right_int_intspan(i: int, s: 'const Span *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.right_int_intspan(i, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_intspan_int(s: 'const Span *', i: int) -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.right_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def right_set_set(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.right_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_span_span(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.right_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'bool':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.right_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'bool':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.right_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.right_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bbox_union_span_span(s1: 'const Span *', s2: 'const Span *') -> 'Span *':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    out_result = _ffi.new('Span *')
+    _lib.bbox_union_span_span(s1_converted, s2_converted, out_result)
+    return out_result if out_result!= _ffi.NULL else None
+
+
+
+def intersection_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.intersection_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intersection_period_timestamp(p: 'const Span *', t: int) -> int:
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.intersection_period_timestamp(p_converted, t_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def intersection_periodset_timestamp(ps: 'const SpanSet *', t: int) -> int:
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.intersection_periodset_timestamp(ps_converted, t_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def intersection_span_span(s1: 'const Span *', s2: 'const Span *') -> 'Span *':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.intersection_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intersection_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.intersection_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intersection_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.intersection_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def intersection_timestampset_timestamp(ts: 'const Set *', t: int) -> int:
+    ts_converted = _ffi.cast('const Set *', ts)
+    t_converted = _ffi.cast('const TimestampTz', t)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.intersection_timestampset_timestamp(ts_converted, t_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def minus_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.minus_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_period_timestamp(p: 'const Span *', t: int) -> 'SpanSet *':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.minus_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'SpanSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.minus_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_span_span(s1: 'const Span *', s2: 'const Span *') -> 'SpanSet *':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.minus_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_span_spanset(s: 'const Span *', ss: 'const SpanSet *') -> 'SpanSet *':
+    s_converted = _ffi.cast('const Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.minus_span_spanset(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.minus_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.minus_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def minus_timestamp_period(t: int, p: 'const Span *') -> int:
+    t_converted = _ffi.cast('TimestampTz', t)
+    p_converted = _ffi.cast('const Span *', p)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.minus_timestamp_period(t_converted, p_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def minus_timestamp_periodset(t: int, ps: 'const SpanSet *') -> int:
+    t_converted = _ffi.cast('TimestampTz', t)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.minus_timestamp_periodset(t_converted, ps_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def minus_timestampset_timestamp(ts: 'const Set *', t: int) -> 'Set *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.minus_timestampset_timestamp(ts_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_set_set(s1: 'const Set *', s2: 'const Set *') -> 'Set *':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.union_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_period_timestamp(p: 'const Span *', t: int) -> 'SpanSet *':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.union_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_periodset_timestamp(ps: 'SpanSet *', t: int) -> 'SpanSet *':
+    ps_converted = _ffi.cast('SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.union_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_span_span(s1: 'const Span *', s2: 'const Span *') -> 'SpanSet *':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.union_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'SpanSet *':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.union_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'SpanSet *':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.union_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_timestampset_timestamp(ts: 'const Set *', t: int) -> 'Set *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    t_converted = _ffi.cast('const TimestampTz', t)
+    result = _lib.union_timestampset_timestamp(ts_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_floatspan_float(s: 'const Span *', d: float) -> 'double':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.distance_floatspan_float(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def distance_intspan_int(s: 'const Span *', i: int) -> 'double':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.distance_intspan_int(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def distance_set_set(s1: 'const Set *', s2: 'const Set *') -> 'double':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.distance_set_set(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_period_timestamp(p: 'const Span *', t: int) -> 'double':
+    p_converted = _ffi.cast('const Span *', p)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.distance_period_timestamp(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_periodset_timestamp(ps: 'const SpanSet *', t: int) -> 'double':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.distance_periodset_timestamp(ps_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_span_span(s1: 'const Span *', s2: 'const Span *') -> 'double':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.distance_span_span(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_spanset_span(ss: 'const SpanSet *', s: 'const Span *') -> 'double':
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.distance_spanset_span(ss_converted, s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_spanset_spanset(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'double':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.distance_spanset_spanset(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_timestampset_timestamp(ts: 'const Set *', t: int) -> 'double':
+    ts_converted = _ffi.cast('const Set *', ts)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.distance_timestampset_timestamp(ts_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigint_extent_transfn(s: 'Span *', i: int) -> 'Span *':
+    s_converted = _ffi.cast('Span *', s)
+    i_converted = _ffi.cast('int64', i)
+    result = _lib.bigint_extent_transfn(s_converted, i_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bigint_union_transfn(state: 'Set *', i: int) -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    i_converted = _ffi.cast('int64', i)
+    result = _lib.bigint_union_transfn(state_converted, i_converted)
+    return result if result != _ffi.NULL else None
+
+
+def float_extent_transfn(s: 'Span *', d: float) -> 'Span *':
+    s_converted = _ffi.cast('Span *', s)
+    result = _lib.float_extent_transfn(s_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def float_union_transfn(state: 'Set *', d: float) -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    result = _lib.float_union_transfn(state_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def int_extent_transfn(s: 'Span *', i: int) -> 'Span *':
+    s_converted = _ffi.cast('Span *', s)
+    result = _lib.int_extent_transfn(s_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def int_union_transfn(state: 'Set *', i: int) -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    result = _lib.int_union_transfn(state_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def period_tcount_transfn(state: "Optional['SkipList *']", p: 'const Span *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.period_tcount_transfn(state_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_tcount_transfn(state: "Optional['SkipList *']", ps: 'const SpanSet *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_tcount_transfn(state_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_extent_transfn(span: 'Span *', set: 'const Set *') -> 'Span *':
+    span_converted = _ffi.cast('Span *', span)
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.set_extent_transfn(span_converted, set_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_union_finalfn(state: 'Set *') -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    result = _lib.set_union_finalfn(state_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_union_transfn(state: 'Set *', set: 'Set *') -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    set_converted = _ffi.cast('Set *', set)
+    result = _lib.set_union_transfn(state_converted, set_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_extent_transfn(s1: 'Span *', s2: 'const Span *') -> 'Span *':
+    s1_converted = _ffi.cast('Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_extent_transfn(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_union_transfn(state: 'SpanSet *', span: 'const Span *') -> 'SpanSet *':
+    state_converted = _ffi.cast('SpanSet *', state)
+    span_converted = _ffi.cast('const Span *', span)
+    result = _lib.span_union_transfn(state_converted, span_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_extent_transfn(s: 'Span *', ss: 'const SpanSet *') -> 'Span *':
+    s_converted = _ffi.cast('Span *', s)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_extent_transfn(s_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_union_finalfn(state: 'SpanSet *') -> 'SpanSet *':
+    state_converted = _ffi.cast('SpanSet *', state)
+    result = _lib.spanset_union_finalfn(state_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_union_transfn(state: 'SpanSet *', ss: 'const SpanSet *') -> 'SpanSet *':
+    state_converted = _ffi.cast('SpanSet *', state)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.spanset_union_transfn(state_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def text_union_transfn(state: 'Set *', txt: str) -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    txt_converted = cstring2text(txt)
+    result = _lib.text_union_transfn(state_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_extent_transfn(p: "Optional['Span *']", t: int) -> 'Span *':
+    p_converted = _ffi.cast('Span *', p) if p is not None else _ffi.NULL
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_extent_transfn(p_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_tcount_transfn(state: "Optional['SkipList *']", t: int) -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_tcount_transfn(state_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_union_transfn(state: 'Set *', t: int) -> 'Set *':
+    state_converted = _ffi.cast('Set *', state)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_union_transfn(state_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_tcount_transfn(state: "Optional['SkipList *']", ts: 'const Set *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.timestampset_tcount_transfn(state_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_cmp(s1: 'const Set *', s2: 'const Set *') -> 'int':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_cmp(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_eq(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_eq(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_ge(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_ge(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_gt(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_gt(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_le(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_le(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_lt(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_lt(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def set_ne(s1: 'const Set *', s2: 'const Set *') -> 'bool':
+    s1_converted = _ffi.cast('const Set *', s1)
+    s2_converted = _ffi.cast('const Set *', s2)
+    result = _lib.set_ne(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_cmp(s1: 'const Span *', s2: 'const Span *') -> 'int':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_cmp(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_eq(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_eq(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_ge(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_ge(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_gt(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_gt(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_le(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_le(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_lt(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_lt(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_ne(s1: 'const Span *', s2: 'const Span *') -> 'bool':
+    s1_converted = _ffi.cast('const Span *', s1)
+    s2_converted = _ffi.cast('const Span *', s2)
+    result = _lib.span_ne(s1_converted, s2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_cmp(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'int':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_cmp(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_eq(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_eq(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_ge(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_ge(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_gt(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_gt(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_le(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_le(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_lt(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_lt(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def spanset_ne(ss1: 'const SpanSet *', ss2: 'const SpanSet *') -> 'bool':
+    ss1_converted = _ffi.cast('const SpanSet *', ss1)
+    ss2_converted = _ffi.cast('const SpanSet *', ss2)
+    result = _lib.spanset_ne(ss1_converted, ss2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_in(string: str) -> 'TBox *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tbox_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_out(box: 'const TBox *', maxdd: int) -> str:
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_out(box_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tbox_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'TBox *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.tbox_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_from_hexwkb(hexwkb: str) -> 'TBox *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.tbox_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'STBox *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.stbox_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_from_hexwkb(hexwkb: str) -> 'STBox *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.stbox_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_as_wkb(box: 'const TBox *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    box_converted = _ffi.cast('const TBox *', box)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.tbox_as_wkb(box_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def tbox_as_hexwkb(box: 'const TBox *', variant: int) -> "Tuple[str, 'size_t *']":
+    box_converted = _ffi.cast('const TBox *', box)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size = _ffi.new('size_t *')
+    result = _lib.tbox_as_hexwkb(box_converted, variant_converted, size)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size[0]
+
+
+def stbox_as_wkb(box: 'const STBox *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    box_converted = _ffi.cast('const STBox *', box)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.stbox_as_wkb(box_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def stbox_as_hexwkb(box: 'const STBox *', variant: int) -> "Tuple[str, 'size_t *']":
+    box_converted = _ffi.cast('const STBox *', box)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size = _ffi.new('size_t *')
+    result = _lib.stbox_as_hexwkb(box_converted, variant_converted, size)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size[0]
+
+
+def stbox_in(string: str) -> 'STBox *':
+    string_converted = string.encode('utf-8')
+    result = _lib.stbox_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_out(box: 'const STBox *', maxdd: int) -> str:
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_out(box_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tbox_make(s: "Optional['const Span *']", p: "Optional['const Span *']") -> 'TBox *':
+    s_converted = _ffi.cast('const Span *', s) if s is not None else _ffi.NULL
+    p_converted = _ffi.cast('const Span *', p) if p is not None else _ffi.NULL
+    result = _lib.tbox_make(s_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_set(s: 'const Span *', p: 'const Span *', box: 'TBox *') -> None:
+    s_converted = _ffi.cast('const Span *', s)
+    p_converted = _ffi.cast('const Span *', p)
+    box_converted = _ffi.cast('TBox *', box)
+    _lib.tbox_set(s_converted, p_converted, box_converted)
+
+
+def tbox_copy(box: 'const TBox *') -> 'TBox *':
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_copy(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_make(hasx: bool, hasz: bool, geodetic: bool, srid: int, xmin: float, xmax: float, ymin: float, ymax: float, zmin: float, zmax: float, p: "Optional['const Span *']") -> 'STBox *':
+    srid_converted = _ffi.cast('int32', srid)
+    p_converted = _ffi.cast('const Span *', p) if p is not None else _ffi.NULL
+    result = _lib.stbox_make(hasx, hasz, geodetic, srid_converted, xmin, xmax, ymin, ymax, zmin, zmax, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_set(hasx: bool, hasz: bool, geodetic: bool, srid: int, xmin: float, xmax: float, ymin: float, ymax: float, zmin: float, zmax: float, p: 'const Span *', box: 'STBox *') -> None:
+    srid_converted = _ffi.cast('int32', srid)
+    p_converted = _ffi.cast('const Span *', p)
+    box_converted = _ffi.cast('STBox *', box)
+    _lib.stbox_set(hasx, hasz, geodetic, srid_converted, xmin, xmax, ymin, ymax, zmin, zmax, p_converted, box_converted)
+
+
+def stbox_copy(box: 'const STBox *') -> 'STBox *':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_copy(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def int_to_tbox(i: int) -> 'TBox *':
+    result = _lib.int_to_tbox(i)
+    return result if result != _ffi.NULL else None
+
+
+def float_to_tbox(d: float) -> 'TBox *':
+    result = _lib.float_to_tbox(d)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_to_tbox(t: int) -> 'TBox *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_to_tbox(t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_to_tbox(ss: 'const Set *') -> 'TBox *':
+    ss_converted = _ffi.cast('const Set *', ss)
+    result = _lib.timestampset_to_tbox(ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_to_tbox(p: 'const Span *') -> 'TBox *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.period_to_tbox(p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_to_tbox(ps: 'const SpanSet *') -> 'TBox *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_to_tbox(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def int_timestamp_to_tbox(i: int, t: int) -> 'TBox *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.int_timestamp_to_tbox(i, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def float_period_to_tbox(d: float, p: 'const Span *') -> 'TBox *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.float_period_to_tbox(d, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def float_timestamp_to_tbox(d: float, t: int) -> 'TBox *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.float_timestamp_to_tbox(d, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geo_period_to_stbox(gs: 'const GSERIALIZED *', p: 'const Span *') -> 'STBox *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.geo_period_to_stbox(gs_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geo_timestamp_to_stbox(gs: 'const GSERIALIZED *', t: int) -> 'STBox *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.geo_timestamp_to_stbox(gs_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geo_to_stbox(gs: 'const GSERIALIZED *') -> 'STBox *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.geo_to_stbox(gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def int_period_to_tbox(i: int, p: 'const Span *') -> 'TBox *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.int_period_to_tbox(i, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def numspan_to_tbox(s: 'const Span *') -> 'TBox *':
+    s_converted = _ffi.cast('const Span *', s)
+    result = _lib.numspan_to_tbox(s_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_timestamp_to_tbox(span: 'const Span *', t: int) -> 'TBox *':
+    span_converted = _ffi.cast('const Span *', span)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.span_timestamp_to_tbox(span_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def span_period_to_tbox(span: 'const Span *', p: 'const Span *') -> 'TBox *':
+    span_converted = _ffi.cast('const Span *', span)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.span_period_to_tbox(span_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_to_floatspan(box: 'const TBox *') -> 'Span *':
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_to_floatspan(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_to_period(box: 'const TBox *') -> 'Span *':
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_to_period(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_to_period(box: 'const STBox *') -> 'Span *':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_to_period(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_to_tbox(temp: 'const Temporal *') -> 'TBox *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_to_tbox(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_to_geo(box: 'const STBox *') -> 'GSERIALIZED *':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_to_geo(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_to_stbox(temp: 'const Temporal *') -> 'STBox *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_to_stbox(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestamp_to_stbox(t: int) -> 'STBox *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.timestamp_to_stbox(t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def timestampset_to_stbox(ts: 'const Set *') -> 'STBox *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.timestampset_to_stbox(ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_to_stbox(p: 'const Span *') -> 'STBox *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.period_to_stbox(p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def periodset_to_stbox(ps: 'const SpanSet *') -> 'STBox *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.periodset_to_stbox(ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_hasx(box: 'const TBox *') -> 'bool':
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_hasx(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_hast(box: 'const TBox *') -> 'bool':
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tbox_hast(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_xmin(box: 'const TBox *') -> 'double':
+    box_converted = _ffi.cast('const TBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.tbox_xmin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tbox_xmax(box: 'const TBox *') -> 'double':
+    box_converted = _ffi.cast('const TBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.tbox_xmax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tbox_tmin(box: 'const TBox *') -> int:
+    box_converted = _ffi.cast('const TBox *', box)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.tbox_tmin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tbox_tmax(box: 'const TBox *') -> int:
+    box_converted = _ffi.cast('const TBox *', box)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.tbox_tmax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_hasx(box: 'const STBox *') -> 'bool':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_hasx(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_hasz(box: 'const STBox *') -> 'bool':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_hasz(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_hast(box: 'const STBox *') -> 'bool':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_hast(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_isgeodetic(box: 'const STBox *') -> 'bool':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_isgeodetic(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_xmin(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_xmin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_xmax(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_xmax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_ymin(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_ymin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_ymax(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_ymax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_zmin(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_zmin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_zmax(box: 'const STBox *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('double *')
+    result = _lib.stbox_zmax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_tmin(box: 'const STBox *') -> int:
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.stbox_tmin(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_tmax(box: 'const STBox *') -> int:
+    box_converted = _ffi.cast('const STBox *', box)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.stbox_tmax(box_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def stbox_srid(box: 'const STBox *') -> 'int32':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_srid(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_expand(box1: 'const TBox *', box2: 'TBox *') -> None:
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('TBox *', box2)
+    _lib.tbox_expand(box1_converted, box2_converted)
+
+
+def tbox_expand_value(box: 'const TBox *', d: 'const double') -> 'TBox *':
+    box_converted = _ffi.cast('const TBox *', box)
+    d_converted = _ffi.cast('const double', d)
+    result = _lib.tbox_expand_value(box_converted, d_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_expand_time(box: 'const TBox *', interval: 'const Interval *') -> 'TBox *':
+    box_converted = _ffi.cast('const TBox *', box)
+    interval_converted = _ffi.cast('const Interval *', interval)
+    result = _lib.tbox_expand_time(box_converted, interval_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_expand(box1: 'const STBox *', box2: 'STBox *') -> None:
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('STBox *', box2)
+    _lib.stbox_expand(box1_converted, box2_converted)
+
+
+def stbox_set_srid(box: 'const STBox *', srid: int) -> 'STBox *':
+    box_converted = _ffi.cast('const STBox *', box)
+    srid_converted = _ffi.cast('int32', srid)
+    result = _lib.stbox_set_srid(box_converted, srid_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_get_space(box: 'const STBox *') -> 'STBox *':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_get_space(box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_expand_space(box: 'const STBox *', d: float) -> 'STBox *':
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.stbox_expand_space(box_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_expand_time(box: 'const STBox *', interval: 'const Interval *') -> 'STBox *':
+    box_converted = _ffi.cast('const STBox *', box)
+    interval_converted = _ffi.cast('const Interval *', interval)
+    result = _lib.stbox_expand_time(box_converted, interval_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.contains_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.contained_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.overlaps_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def same_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.same_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.adjacent_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contains_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.contains_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def contained_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.contained_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overlaps_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overlaps_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def same_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.same_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def adjacent_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.adjacent_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.left_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.overleft_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.right_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.overright_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def before_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.before_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.overbefore_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def after_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.after_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.overafter_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def left_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.left_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overleft_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overleft_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def right_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.right_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overright_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overright_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def below_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.below_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbelow_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overbelow_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def above_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.above_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overabove_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overabove_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def front_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.front_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overfront_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overfront_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def back_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.back_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overback_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overback_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def before_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.before_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overbefore_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overbefore_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def after_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.after_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def overafter_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.overafter_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.union_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def inter_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    out_result = _ffi.new('TBox *')
+    result = _lib.inter_tbox_tbox(box1_converted, box2_converted, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def intersection_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'TBox *':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.intersection_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def union_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *', strict: bool) -> 'STBox *':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.union_stbox_stbox(box1_converted, box2_converted, strict)
+    return result if result != _ffi.NULL else None
+
+
+def inter_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'STBox *':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    out_result = _ffi.new('STBox *')
+    result = _lib.inter_stbox_stbox(box1_converted, box2_converted, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def intersection_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'STBox *':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.intersection_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_quad_split(box: 'const STBox *') -> "Tuple['STBox *', 'int']":
+    box_converted = _ffi.cast('const STBox *', box)
+    count = _ffi.new('int *')
+    result = _lib.stbox_quad_split(box_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tbox_eq(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_eq(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_ne(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_ne(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_cmp(box1: 'const TBox *', box2: 'const TBox *') -> 'int':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_cmp(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_lt(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_lt(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_le(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_le(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_ge(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_ge(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbox_gt(box1: 'const TBox *', box2: 'const TBox *') -> 'bool':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.tbox_gt(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_eq(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_eq(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_ne(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_ne(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_cmp(box1: 'const STBox *', box2: 'const STBox *') -> 'int':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_cmp(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_lt(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_lt(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_le(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_le(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_ge(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_ge(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_gt(box1: 'const STBox *', box2: 'const STBox *') -> 'bool':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.stbox_gt(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tbool_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_out(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_out(temp_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def temporal_as_hexwkb(temp: 'const Temporal *', variant: int) -> "Tuple[str, 'size_t *']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.temporal_as_hexwkb(temp_converted, variant_converted, size_out)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def temporal_as_mfjson(temp: 'const Temporal *', with_bbox: bool, flags: int, precision: int, srs: "Optional[str]") -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    srs_converted = srs.encode('utf-8') if srs is not None else _ffi.NULL
+    result = _lib.temporal_as_mfjson(temp_converted, with_bbox, flags, precision, srs_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def temporal_as_wkb(temp: 'const Temporal *', variant: int) -> "Tuple['uint8_t *', 'size_t *']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    variant_converted = _ffi.cast('uint8_t', variant)
+    size_out = _ffi.new('size_t *')
+    result = _lib.temporal_as_wkb(temp_converted, variant_converted, size_out)
+    return result if result != _ffi.NULL else None, size_out[0]
+
+
+def temporal_from_hexwkb(hexwkb: str) -> 'Temporal *':
+    hexwkb_converted = hexwkb.encode('utf-8')
+    result = _lib.temporal_from_hexwkb(hexwkb_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_from_mfjson(mfjson: str) -> 'Temporal *':
+    mfjson_converted = mfjson.encode('utf-8')
+    result = _lib.temporal_from_mfjson(mfjson_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_from_wkb(wkb: 'const uint8_t *', size: 'size_t') -> 'Temporal *':
+    wkb_converted = _ffi.cast('const uint8_t *', wkb)
+    size_converted = _ffi.cast('size_t', size)
+    result = _lib.temporal_from_wkb(wkb_converted, size_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tfloat_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_out(temp: 'const Temporal *', maxdd: int) -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_out(temp_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpoint_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tgeogpoint_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompoint_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tgeompoint_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.tint_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_out(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_out(temp_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_as_ewkt(temp: 'const Temporal *', maxdd: int) -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_as_ewkt(temp_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_as_text(temp: 'const Temporal *', maxdd: int) -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_as_text(temp_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_out(temp: 'const Temporal *', maxdd: int) -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_out(temp_converted, maxdd)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def ttext_in(string: str) -> 'Temporal *':
+    string_converted = string.encode('utf-8')
+    result = _lib.ttext_in(string_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_out(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_out(temp_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def tbool_from_base_temp(b: bool, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_from_base_temp(b, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolinst_make(b: bool, t: int) -> 'TInstant *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.tboolinst_make(b, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolseq_from_base_period(b: bool, p: 'const Span *') -> 'TSequence *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.tboolseq_from_base_period(b, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolseq_from_base_temp(b: bool, seq: 'const TSequence *') -> 'TSequence *':
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.tboolseq_from_base_temp(b, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolseq_from_base_timestampset(b: bool, ts: 'const Set *') -> 'TSequence *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.tboolseq_from_base_timestampset(b, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolseqset_from_base_periodset(b: bool, ps: 'const SpanSet *') -> 'TSequenceSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.tboolseqset_from_base_periodset(b, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tboolseqset_from_base_temp(b: bool, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.tboolseqset_from_base_temp(b, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_copy(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_copy(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_from_base_temp(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_from_base_temp(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatinst_make(d: float, t: int) -> 'TInstant *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.tfloatinst_make(d, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatseq_from_base_period(d: float, p: 'const Span *', interp: 'interpType') -> 'TSequence *':
+    p_converted = _ffi.cast('const Span *', p)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tfloatseq_from_base_period(d, p_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatseq_from_base_temp(d: float, seq: 'const TSequence *') -> 'TSequence *':
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.tfloatseq_from_base_temp(d, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatseq_from_base_timestampset(d: float, ts: 'const Set *') -> 'TSequence *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.tfloatseq_from_base_timestampset(d, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatseqset_from_base_periodset(d: float, ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tfloatseqset_from_base_periodset(d, ps_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloatseqset_from_base_temp(d: float, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.tfloatseqset_from_base_temp(d, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpoint_from_base_temp(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgeogpoint_from_base_temp(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointinst_make(gs: 'const GSERIALIZED *', t: int) -> 'TInstant *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.tgeogpointinst_make(gs_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointseq_from_base_period(gs: 'const GSERIALIZED *', p: 'const Span *', interp: 'interpType') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    p_converted = _ffi.cast('const Span *', p)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tgeogpointseq_from_base_period(gs_converted, p_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointseq_from_base_temp(gs: 'const GSERIALIZED *', seq: 'const TSequence *') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.tgeogpointseq_from_base_temp(gs_converted, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointseq_from_base_timestampset(gs: 'const GSERIALIZED *', ts: 'const Set *') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.tgeogpointseq_from_base_timestampset(gs_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointseqset_from_base_temp(gs: 'const GSERIALIZED *', ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.tgeogpointseqset_from_base_temp(gs_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpointseqset_from_base_periodset(gs: 'const GSERIALIZED *', ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tgeogpointseqset_from_base_periodset(gs_converted, ps_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompoint_from_base_temp(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgeompoint_from_base_temp(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointinst_make(gs: 'const GSERIALIZED *', t: int) -> 'TInstant *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.tgeompointinst_make(gs_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointseq_from_base_period(gs: 'const GSERIALIZED *', p: 'const Span *', interp: 'interpType') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    p_converted = _ffi.cast('const Span *', p)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tgeompointseq_from_base_period(gs_converted, p_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointseq_from_base_temp(gs: 'const GSERIALIZED *', seq: 'const TSequence *') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.tgeompointseq_from_base_temp(gs_converted, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointseq_from_base_timestampset(gs: 'const GSERIALIZED *', ts: 'const Set *') -> 'TSequence *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.tgeompointseq_from_base_timestampset(gs_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointseqset_from_base_periodset(gs: 'const GSERIALIZED *', ps: 'const SpanSet *', interp: 'interpType') -> 'TSequenceSet *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tgeompointseqset_from_base_periodset(gs_converted, ps_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompointseqset_from_base_temp(gs: 'const GSERIALIZED *', ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.tgeompointseqset_from_base_temp(gs_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_from_base_temp(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_from_base_temp(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintinst_make(i: int, t: int) -> 'TInstant *':
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.tintinst_make(i, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintseq_from_base_period(i: int, p: 'const Span *') -> 'TSequence *':
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.tintseq_from_base_period(i, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintseq_from_base_temp(i: int, seq: 'const TSequence *') -> 'TSequence *':
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.tintseq_from_base_temp(i, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintseq_from_base_timestampset(i: int, ts: 'const Set *') -> 'TSequence *':
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.tintseq_from_base_timestampset(i, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintseqset_from_base_periodset(i: int, ps: 'const SpanSet *') -> 'TSequenceSet *':
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.tintseqset_from_base_periodset(i, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tintseqset_from_base_temp(i: int, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.tintseqset_from_base_temp(i, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tsequence_make(instants: 'const TInstant **', count: int, lower_inc: bool, upper_inc: bool, interp: 'interpType', normalize: bool) -> 'TSequence *':
+    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tsequence_make(instants_converted, count, lower_inc, upper_inc, interp_converted, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def tsequence_make_exp(instants: 'const TInstant **', count: int, maxcount: int, lower_inc: bool, upper_inc: bool, interp: 'interpType', normalize: bool) -> 'TSequence *':
+    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.tsequence_make_exp(instants_converted, count, maxcount, lower_inc, upper_inc, interp_converted, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def tsequenceset_make(sequences: 'const TSequence **', count: int, normalize: bool) -> 'TSequenceSet *':
+    sequences_converted = [_ffi.cast('const TSequence *', x) for x in sequences]
+    result = _lib.tsequenceset_make(sequences_converted, count, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def tsequenceset_make_exp(sequences: 'const TSequence **', count: int, maxcount: int, normalize: bool) -> 'TSequenceSet *':
+    sequences_converted = [_ffi.cast('const TSequence *', x) for x in sequences]
+    result = _lib.tsequenceset_make_exp(sequences_converted, count, maxcount, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def tsequenceset_make_gaps(instants: 'const TInstant **', count: int, interp: 'interpType', maxt: 'Interval *', maxdist: float) -> 'TSequenceSet *':
+    instants_converted = [_ffi.cast('const TInstant *', x) for x in instants]
+    interp_converted = _ffi.cast('interpType', interp)
+    maxt_converted = _ffi.cast('Interval *', maxt)
+    result = _lib.tsequenceset_make_gaps(instants_converted, count, interp_converted, maxt_converted, maxdist)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_from_base_temp(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_from_base_temp(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextinst_make(txt: str, t: int) -> 'TInstant *':
+    txt_converted = cstring2text(txt)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.ttextinst_make(txt_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextseq_from_base_period(txt: str, p: 'const Span *') -> 'TSequence *':
+    txt_converted = cstring2text(txt)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.ttextseq_from_base_period(txt_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextseq_from_base_temp(txt: str, seq: 'const TSequence *') -> 'TSequence *':
+    txt_converted = cstring2text(txt)
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.ttextseq_from_base_temp(txt_converted, seq_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextseq_from_base_timestampset(txt: str, ts: 'const Set *') -> 'TSequence *':
+    txt_converted = cstring2text(txt)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.ttextseq_from_base_timestampset(txt_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextseqset_from_base_periodset(txt: str, ps: 'const SpanSet *') -> 'TSequenceSet *':
+    txt_converted = cstring2text(txt)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.ttextseqset_from_base_periodset(txt_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttextseqset_from_base_temp(txt: str, ss: 'const TSequenceSet *') -> 'TSequenceSet *':
+    txt_converted = cstring2text(txt)
+    ss_converted = _ffi.cast('const TSequenceSet *', ss)
+    result = _lib.ttextseqset_from_base_temp(txt_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_to_period(temp: 'const Temporal *') -> 'Span *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_to_period(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_to_tint(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_to_tint(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_to_tfloat(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_to_tfloat(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_to_span(temp: 'const Temporal *') -> 'Span *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_to_span(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_end_value(temp: 'const Temporal *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_end_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_start_value(temp: 'const Temporal *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_start_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_values(temp: 'const Temporal *') -> "Tuple['bool *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tbool_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_duration(temp: 'const Temporal *', boundspan: bool) -> 'Interval *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_duration(temp_converted, boundspan)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_end_instant(temp: 'const Temporal *') -> 'const TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_end_instant(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_end_sequence(temp: 'const Temporal *') -> 'TSequence *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_end_sequence(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_end_timestamp(temp: 'const Temporal *') -> 'TimestampTz':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_end_timestamp(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_hash(temp: 'const Temporal *') -> 'uint32':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_hash(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_instant_n(temp: 'const Temporal *', n: int) -> 'const TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_instant_n(temp_converted, n)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_instants(temp: 'const Temporal *') -> "Tuple['const TInstant **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.temporal_instants(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_interp(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_interp(temp_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def temporal_max_instant(temp: 'const Temporal *') -> 'const TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_max_instant(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_min_instant(temp: 'const Temporal *') -> 'const TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_min_instant(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_num_instants(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_num_instants(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_num_sequences(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_num_sequences(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_num_timestamps(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_num_timestamps(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_segments(temp: 'const Temporal *') -> "Tuple['TSequence **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.temporal_segments(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_sequence_n(temp: 'const Temporal *', i: int) -> 'TSequence *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_sequence_n(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_sequences(temp: 'const Temporal *') -> "Tuple['TSequence **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.temporal_sequences(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_start_instant(temp: 'const Temporal *') -> 'const TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_start_instant(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_start_sequence(temp: 'const Temporal *') -> 'TSequence *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_start_sequence(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_start_timestamp(temp: 'const Temporal *') -> 'TimestampTz':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_start_timestamp(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_stops(temp: 'const Temporal *', maxdist: float, minduration: 'const Interval *') -> 'TSequenceSet *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    minduration_converted = _ffi.cast('const Interval *', minduration)
+    result = _lib.temporal_stops(temp_converted, maxdist, minduration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_subtype(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_subtype(temp_converted)
+    result = _ffi.string(result).decode('utf-8')
+    return result if result != _ffi.NULL else None
+
+
+def temporal_time(temp: 'const Temporal *') -> 'SpanSet *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_time(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_timestamp_n(temp: 'const Temporal *', n: int) -> int:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    out_result = _ffi.new('TimestampTz *')
+    result = _lib.temporal_timestamp_n(temp_converted, n, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def temporal_timestamps(temp: 'const Temporal *') -> "Tuple['TimestampTz *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.temporal_timestamps(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_values(temp: 'const Temporal *') -> "Tuple['Datum *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.temporal_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tfloat_end_value(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_end_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_max_value(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_max_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_min_value(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_min_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_start_value(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_start_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_values(temp: 'const Temporal *') -> "Tuple['double *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tfloat_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tint_end_value(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_end_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_max_value(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_max_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_min_value(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_min_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_start_value(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_start_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_values(temp: 'const Temporal *') -> "Tuple['int *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tint_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tnumber_valuespans(temp: 'const Temporal *') -> 'SpanSet *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_valuespans(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_end_value(temp: 'const Temporal *') -> 'GSERIALIZED *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_end_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_start_value(temp: 'const Temporal *') -> 'GSERIALIZED *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_start_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_values(temp: 'const Temporal *') -> "Tuple['GSERIALIZED **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tpoint_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def ttext_end_value(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_end_value(temp_converted)
+    result = text2cstring(result)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_max_value(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_max_value(temp_converted)
+    result = text2cstring(result)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_min_value(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_min_value(temp_converted)
+    result = text2cstring(result)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_start_value(temp: 'const Temporal *') -> str:
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_start_value(temp_converted)
+    result = text2cstring(result)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_values(temp: 'const Temporal *') -> "Tuple['text **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.ttext_values(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_set_interp(temp: 'const Temporal *', interp: 'interpType') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    interp_converted = _ffi.cast('interpType', interp)
+    result = _lib.temporal_set_interp(temp_converted, interp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_shift(temp: 'const Temporal *', shift: 'const Interval *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    shift_converted = _ffi.cast('const Interval *', shift)
+    result = _lib.temporal_shift(temp_converted, shift_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_shift_tscale(temp: 'const Temporal *', shift: "Optional['const Interval *']", duration: "Optional['const Interval *']") -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    shift_converted = _ffi.cast('const Interval *', shift) if shift is not None else _ffi.NULL
+    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
+    result = _lib.temporal_shift_tscale(temp_converted, shift_converted, duration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_to_tinstant(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_to_tinstant(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_to_tsequence(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_to_tsequence(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_to_tsequenceset(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_to_tsequenceset(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_tprecision(temp: 'const Temporal *', duration: 'const Interval *', origin: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    origin_converted = _ffi.cast('TimestampTz', origin)
+    result = _lib.temporal_tprecision(temp_converted, duration_converted, origin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_tsample(temp: 'const Temporal *', duration: 'const Interval *', origin: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    origin_converted = _ffi.cast('TimestampTz', origin)
+    result = _lib.temporal_tsample(temp_converted, duration_converted, origin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_tscale(temp: 'const Temporal *', duration: 'const Interval *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    result = _lib.temporal_tscale(temp_converted, duration_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_at_value(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_at_value(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_minus_value(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_minus_value(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('bool *')
+    result = _lib.tbool_value_at_timestamp(temp_converted, t_converted, strict, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def temporal_at_max(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_at_max(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_min(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_at_min(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_period(temp: 'const Temporal *', p: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.temporal_at_period(temp_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_periodset(temp: 'const Temporal *', ps: 'const SpanSet *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.temporal_at_periodset(temp_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_timestamp(temp: 'const Temporal *', t: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.temporal_at_timestamp(temp_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_timestampset(temp: 'const Temporal *', ts: 'const Set *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.temporal_at_timestampset(temp_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_at_values(temp: 'const Temporal *', set: 'const Set *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.temporal_at_values(temp_converted, set_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_max(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_minus_max(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_min(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_minus_min(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_period(temp: 'const Temporal *', p: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.temporal_minus_period(temp_converted, p_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_periodset(temp: 'const Temporal *', ps: 'const SpanSet *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.temporal_minus_periodset(temp_converted, ps_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_timestamp(temp: 'const Temporal *', t: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.temporal_minus_timestamp(temp_converted, t_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_timestampset(temp: 'const Temporal *', ts: 'const Set *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.temporal_minus_timestampset(temp_converted, ts_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_minus_values(temp: 'const Temporal *', set: 'const Set *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    set_converted = _ffi.cast('const Set *', set)
+    result = _lib.temporal_minus_values(temp_converted, set_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_at_value(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_at_value(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_minus_value(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_minus_value(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('double *')
+    result = _lib.tfloat_value_at_timestamp(temp_converted, t_converted, strict, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tint_at_value(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_at_value(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_minus_value(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_minus_value(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('int *')
+    result = _lib.tint_value_at_timestamp(temp_converted, t_converted, strict, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tnumber_at_span(temp: 'const Temporal *', span: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    span_converted = _ffi.cast('const Span *', span)
+    result = _lib.tnumber_at_span(temp_converted, span_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_at_spanset(temp: 'const Temporal *', ss: 'const SpanSet *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.tnumber_at_spanset(temp_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_at_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tnumber_at_tbox(temp_converted, box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_minus_span(temp: 'const Temporal *', span: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    span_converted = _ffi.cast('const Span *', span)
+    result = _lib.tnumber_minus_span(temp_converted, span_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_minus_spanset(temp: 'const Temporal *', ss: 'const SpanSet *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ss_converted = _ffi.cast('const SpanSet *', ss)
+    result = _lib.tnumber_minus_spanset(temp_converted, ss_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_minus_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.tnumber_minus_tbox(temp_converted, box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_at_geom_time(temp: 'const Temporal *', gs: 'const GSERIALIZED *', zspan: 'const Span *', period: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    zspan_converted = _ffi.cast('const Span *', zspan)
+    period_converted = _ffi.cast('const Span *', period)
+    result = _lib.tpoint_at_geom_time(temp_converted, gs_converted, zspan_converted, period_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_at_stbox(temp: 'const Temporal *', box: 'const STBox *', border_inc: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.tpoint_at_stbox(temp_converted, box_converted, border_inc)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_at_value(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tpoint_at_value(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_minus_geom_time(temp: 'const Temporal *', gs: 'const GSERIALIZED *', zspan: 'const Span *', period: 'const Span *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    zspan_converted = _ffi.cast('const Span *', zspan)
+    period_converted = _ffi.cast('const Span *', period)
+    result = _lib.tpoint_minus_geom_time(temp_converted, gs_converted, zspan_converted, period_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_minus_stbox(temp: 'const Temporal *', box: 'const STBox *', border_inc: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.tpoint_minus_stbox(temp_converted, box_converted, border_inc)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_minus_value(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tpoint_minus_value(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'GSERIALIZED **':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('GSERIALIZED **')
+    result = _lib.tpoint_value_at_timestamp(temp_converted, t_converted, strict, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def ttext_at_value(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_at_value(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_minus_value(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_minus_value(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_value_at_timestamp(temp: 'const Temporal *', t: int, strict: bool) -> 'text **':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    out_result = _ffi.new('text **')
+    result = _lib.ttext_value_at_timestamp(temp_converted, t_converted, strict, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def temporal_append_tinstant(temp: 'Temporal *', inst: 'const TInstant *', maxdist: float, maxt: 'Interval *', expand: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('Temporal *', temp)
+    inst_converted = _ffi.cast('const TInstant *', inst)
+    maxt_converted = _ffi.cast('Interval *', maxt)
+    result = _lib.temporal_append_tinstant(temp_converted, inst_converted, maxdist, maxt_converted, expand)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_append_tsequence(temp: 'Temporal *', seq: 'const TSequence *', expand: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('Temporal *', temp)
+    seq_converted = _ffi.cast('const TSequence *', seq)
+    result = _lib.temporal_append_tsequence(temp_converted, seq_converted, expand)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_delete_period(temp: 'const Temporal *', p: 'const Span *', connect: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    p_converted = _ffi.cast('const Span *', p)
+    result = _lib.temporal_delete_period(temp_converted, p_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_delete_periodset(temp: 'const Temporal *', ps: 'const SpanSet *', connect: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ps_converted = _ffi.cast('const SpanSet *', ps)
+    result = _lib.temporal_delete_periodset(temp_converted, ps_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_delete_timestamp(temp: 'const Temporal *', t: int, connect: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    t_converted = _ffi.cast('TimestampTz', t)
+    result = _lib.temporal_delete_timestamp(temp_converted, t_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_delete_timestampset(temp: 'const Temporal *', ts: 'const Set *', connect: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    ts_converted = _ffi.cast('const Set *', ts)
+    result = _lib.temporal_delete_timestampset(temp_converted, ts_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_insert(temp1: 'const Temporal *', temp2: 'const Temporal *', connect: bool) -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_insert(temp1_converted, temp2_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_merge(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_merge(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_merge_array(temparr: 'Temporal **', count: int) -> 'Temporal *':
+    temparr_converted = [_ffi.cast('Temporal *', x) for x in temparr]
+    result = _lib.temporal_merge_array(temparr_converted, count)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_update(temp1: 'const Temporal *', temp2: 'const Temporal *', connect: bool) -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_update(temp1_converted, temp2_converted, connect)
+    return result if result != _ffi.NULL else None
+
+
+def tand_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tand_bool_tbool(b, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tand_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tand_tbool_bool(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tand_tbool_tbool(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tand_tbool_tbool(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_when_true(temp: 'const Temporal *') -> 'SpanSet *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_when_true(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnot_tbool(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnot_tbool(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tor_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tor_bool_tbool(b, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tor_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tor_tbool_bool(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tor_tbool_tbool(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tor_tbool_tbool(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def add_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.add_float_tfloat(d, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def add_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.add_int_tint(i, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def add_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.add_tfloat_float(tnumber_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def add_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.add_tint_int(tnumber_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def add_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
+    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
+    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
+    result = _lib.add_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def div_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.div_float_tfloat(d, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def div_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.div_int_tint(i, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def div_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.div_tfloat_float(tnumber_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def div_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.div_tint_int(tnumber_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def div_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
+    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
+    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
+    result = _lib.div_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def float_degrees(value: float, normalize: bool) -> 'double':
+    result = _lib.float_degrees(value, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def mult_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.mult_float_tfloat(d, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def mult_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.mult_int_tint(i, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def mult_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.mult_tfloat_float(tnumber_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def mult_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.mult_tint_int(tnumber_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def mult_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
+    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
+    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
+    result = _lib.mult_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def sub_float_tfloat(d: float, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.sub_float_tfloat(d, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def sub_int_tint(i: int, tnumber: 'const Temporal *') -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.sub_int_tint(i, tnumber_converted)
+    return result if result != _ffi.NULL else None
+
+
+def sub_tfloat_float(tnumber: 'const Temporal *', d: float) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.sub_tfloat_float(tnumber_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def sub_tint_int(tnumber: 'const Temporal *', i: int) -> 'Temporal *':
+    tnumber_converted = _ffi.cast('const Temporal *', tnumber)
+    result = _lib.sub_tint_int(tnumber_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def sub_tnumber_tnumber(tnumber1: 'const Temporal *', tnumber2: 'const Temporal *') -> 'Temporal *':
+    tnumber1_converted = _ffi.cast('const Temporal *', tnumber1)
+    tnumber2_converted = _ffi.cast('const Temporal *', tnumber2)
+    result = _lib.sub_tnumber_tnumber(tnumber1_converted, tnumber2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_degrees(temp: 'const Temporal *', normalize: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_degrees(temp_converted, normalize)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_derivative(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_derivative(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_radians(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_radians(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_abs(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_abs(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_angular_difference(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_angular_difference(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_delta_value(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_delta_value(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def textcat_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.textcat_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def textcat_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.textcat_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def textcat_ttext_ttext(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.textcat_ttext_ttext(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_upper(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_upper(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_lower(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_lower(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.distance_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def distance_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.distance_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def distance_tnumber_tnumber(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.distance_tnumber_tnumber(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.distance_tpoint_geo(temp_converted, geo_converted)
+    return result if result != _ffi.NULL else None
+
+
+def distance_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.distance_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_stbox_geo(box: 'const STBox *', gs: 'const GSERIALIZED *') -> 'double':
+    box_converted = _ffi.cast('const STBox *', box)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.nad_stbox_geo(box_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_stbox_stbox(box1: 'const STBox *', box2: 'const STBox *') -> 'double':
+    box1_converted = _ffi.cast('const STBox *', box1)
+    box2_converted = _ffi.cast('const STBox *', box2)
+    result = _lib.nad_stbox_stbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tbox_tbox(box1: 'const TBox *', box2: 'const TBox *') -> 'double':
+    box1_converted = _ffi.cast('const TBox *', box1)
+    box2_converted = _ffi.cast('const TBox *', box2)
+    result = _lib.nad_tbox_tbox(box1_converted, box2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tfloat_float(temp: 'const Temporal *', d: float) -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.nad_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tfloat_tfloat(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.nad_tfloat_tfloat(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tint_int(temp: 'const Temporal *', i: int) -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.nad_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tint_tint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.nad_tint_tint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tnumber_tbox(temp: 'const Temporal *', box: 'const TBox *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const TBox *', box)
+    result = _lib.nad_tnumber_tbox(temp_converted, box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.nad_tpoint_geo(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tpoint_stbox(temp: 'const Temporal *', box: 'const STBox *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    box_converted = _ffi.cast('const STBox *', box)
+    result = _lib.nad_tpoint_stbox(temp_converted, box_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nad_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.nad_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nai_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'TInstant *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.nai_tpoint_geo(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def nai_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'TInstant *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.nai_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def shortestline_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'GSERIALIZED **':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    out_result = _ffi.new('GSERIALIZED **')
+    result = _lib.shortestline_tpoint_geo(temp_converted, gs_converted, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def shortestline_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'GSERIALIZED **':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    out_result = _ffi.new('GSERIALIZED **')
+    result = _lib.shortestline_tpoint_tpoint(temp1_converted, temp2_converted, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
+def tbool_always_eq(temp: 'const Temporal *', b: bool) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_always_eq(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_ever_eq(temp: 'const Temporal *', b: bool) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_ever_eq(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_always_eq(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_always_eq(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_always_le(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_always_le(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_always_lt(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_always_lt(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_ever_eq(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_ever_eq(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_ever_le(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_ever_le(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_ever_lt(temp: 'const Temporal *', d: float) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_ever_lt(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpoint_always_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tgeogpoint_always_eq(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeogpoint_ever_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tgeogpoint_ever_eq(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompoint_always_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tgeompoint_always_eq(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompoint_ever_eq(temp: 'const Temporal *', gs: 'GSERIALIZED *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('GSERIALIZED *', gs)
+    result = _lib.tgeompoint_ever_eq(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_always_eq(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_always_eq(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_always_le(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_always_le(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_always_lt(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_always_lt(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_ever_eq(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_ever_eq(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_ever_le(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_ever_le(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tint_ever_lt(temp: 'const Temporal *', i: int) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_ever_lt(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_always_eq(temp: 'const Temporal *', value: 'Datum') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    value_converted = _ffi.cast('Datum', value)
+    result = _lib.tpoint_always_eq(temp_converted, value_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_ever_eq(temp: 'const Temporal *', value: 'Datum') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    value_converted = _ffi.cast('Datum', value)
+    result = _lib.tpoint_ever_eq(temp_converted, value_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_always_eq(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_always_eq(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_always_le(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_always_le(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_always_lt(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_always_lt(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_ever_eq(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_ever_eq(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_ever_le(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_ever_le(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_ever_lt(temp: 'const Temporal *', txt: str) -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.ttext_ever_lt(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_cmp(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_cmp(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_eq(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_eq(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_ge(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_ge(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_gt(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_gt(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_le(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_le(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_lt(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_lt(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_ne(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'bool':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_ne(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_bool_tbool(b, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_geo_tpoint(geo: 'const GSERIALIZED *', tpoint: 'const Temporal *') -> 'Temporal *':
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
+    result = _lib.teq_geo_tpoint(geo_converted, tpoint_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_point_tgeogpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_point_tgeogpoint(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_point_tgeompoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_point_tgeompoint(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_tbool_bool(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def teq_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.teq_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tgeogpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.teq_tgeogpoint_point(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tgeompoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.teq_tgeompoint_point(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.teq_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def teq_tpoint_geo(tpoint: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
+    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.teq_tpoint_geo(tpoint_converted, geo_converted)
+    return result if result != _ffi.NULL else None
+
+
+def teq_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.teq_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tge_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tge_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tge_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tge_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tge_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tge_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tge_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tge_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tge_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tge_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tge_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tge_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tge_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.tge_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgt_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgt_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tgt_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgt_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgt_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgt_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tgt_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.tgt_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tle_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tle_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tle_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tle_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tle_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tle_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tle_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tle_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tle_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tle_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tle_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tle_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tle_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.tle_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tlt_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tlt_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tlt_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tlt_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tlt_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tlt_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tlt_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.tlt_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_bool_tbool(b: bool, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_bool_tbool(b, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_float_tfloat(d: float, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_float_tfloat(d, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_geo_tpoint(geo: 'const GSERIALIZED *', tpoint: 'const Temporal *') -> 'Temporal *':
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
+    result = _lib.tne_geo_tpoint(geo_converted, tpoint_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_int_tint(i: int, temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_int_tint(i, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_point_tgeogpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_point_tgeogpoint(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_point_tgeompoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_point_tgeompoint(gs_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tbool_bool(temp: 'const Temporal *', b: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_tbool_bool(temp_converted, b)
+    return result if result != _ffi.NULL else None
+
+
+def tne_temporal_temporal(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tne_temporal_temporal(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_text_ttext(txt: str, temp: 'const Temporal *') -> 'Temporal *':
+    txt_converted = cstring2text(txt)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_text_ttext(txt_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tfloat_float(temp: 'const Temporal *', d: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_tfloat_float(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tgeogpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.tne_tgeogpoint_point(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tgeompoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.tne_tgeompoint_point(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tint_int(temp: 'const Temporal *', i: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tne_tint_int(temp_converted, i)
+    return result if result != _ffi.NULL else None
+
+
+def tne_tpoint_geo(tpoint: 'const Temporal *', geo: 'const GSERIALIZED *') -> 'Temporal *':
+    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.tne_tpoint_geo(tpoint_converted, geo_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tne_ttext_text(temp: 'const Temporal *', txt: str) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    txt_converted = cstring2text(txt)
+    result = _lib.tne_ttext_text(temp_converted, txt_converted)
+    return result if result != _ffi.NULL else None
+
+
+def bearing_point_point(geo1: 'const GSERIALIZED *', geo2: 'const GSERIALIZED *') -> 'double':
+    geo1_converted = _ffi.cast('const GSERIALIZED *', geo1)
+    geo2_converted = _ffi.cast('const GSERIALIZED *', geo2)
+    out_result = _ffi.new('double *')
+    result = _lib.bearing_point_point(geo1_converted, geo2_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def bearing_tpoint_point(temp: 'const Temporal *', gs: 'const GSERIALIZED *', invert: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.bearing_tpoint_point(temp_converted, gs_converted, invert)
+    return result if result != _ffi.NULL else None
+
+
+def bearing_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.bearing_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_angular_difference(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_angular_difference(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_azimuth(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_azimuth(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_convex_hull(temp: 'const Temporal *') -> 'GSERIALIZED *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_convex_hull(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_cumulative_length(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_cumulative_length(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_direction(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    out_result = _ffi.new('double *')
+    result = _lib.tpoint_direction(temp_converted, out_result)
+    if result:
+        return out_result[0] if out_result[0] != _ffi.NULL else None
+    return None
+
+
+def tpoint_get_coord(temp: 'const Temporal *', coord: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_get_coord(temp_converted, coord)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_is_simple(temp: 'const Temporal *') -> 'bool':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_is_simple(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_length(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_length(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_speed(temp: 'const Temporal *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_speed(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_srid(temp: 'const Temporal *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_srid(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_stboxes(temp: 'const Temporal *') -> "Tuple['STBox *', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tpoint_stboxes(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tpoint_trajectory(temp: 'const Temporal *') -> 'GSERIALIZED *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_trajectory(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geo_expand_space(gs: 'const GSERIALIZED *', d: float) -> 'STBox *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.geo_expand_space(gs_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tgeompoint_tgeogpoint(temp: 'const Temporal *', oper: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tgeompoint_tgeogpoint(temp_converted, oper)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_expand_space(temp: 'const Temporal *', d: float) -> 'STBox *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_expand_space(temp_converted, d)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_make_simple(temp: 'const Temporal *') -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    count = _ffi.new('int *')
+    result = _lib.tpoint_make_simple(temp_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tpoint_set_srid(temp: 'const Temporal *', srid: int) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    srid_converted = _ffi.cast('int32', srid)
+    result = _lib.tpoint_set_srid(temp_converted, srid_converted)
+    return result if result != _ffi.NULL else None
+
+
+def econtains_geo_tpoint(geo: 'const GSERIALIZED *', temp: 'const Temporal *') -> 'int':
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.econtains_geo_tpoint(geo_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def edisjoint_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.edisjoint_tpoint_geo(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def edisjoint_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.edisjoint_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def edwithin_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', dist: float) -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.edwithin_tpoint_geo(temp_converted, gs_converted, dist)
+    return result if result != _ffi.NULL else None
+
+
+def edwithin_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *', dist: float) -> 'int':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.edwithin_tpoint_tpoint(temp1_converted, temp2_converted, dist)
+    return result if result != _ffi.NULL else None
+
+
+def eintersects_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.eintersects_tpoint_geo(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def eintersects_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'int':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.eintersects_tpoint_tpoint(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def etouches_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *') -> 'int':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.etouches_tpoint_geo(temp_converted, gs_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tcontains_geo_tpoint(gs: 'const GSERIALIZED *', temp: 'const Temporal *', restr: bool, atvalue: bool) -> 'Temporal *':
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tcontains_geo_tpoint(gs_converted, temp_converted, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def tdisjoint_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.tdisjoint_tpoint_geo(temp_converted, geo_converted, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def tdwithin_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', dist: float, restr: bool, atvalue: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.tdwithin_tpoint_geo(temp_converted, gs_converted, dist, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def tdwithin_tpoint_tpoint(temp1: 'const Temporal *', temp2: 'const Temporal *', dist: float, restr: bool, atvalue: bool) -> 'Temporal *':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.tdwithin_tpoint_tpoint(temp1_converted, temp2_converted, dist, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def tintersects_tpoint_geo(temp: 'const Temporal *', geo: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.tintersects_tpoint_geo(temp_converted, geo_converted, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def ttouches_tpoint_geo(temp: 'const Temporal *', gs: 'const GSERIALIZED *', restr: bool, atvalue: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    gs_converted = _ffi.cast('const GSERIALIZED *', gs)
+    result = _lib.ttouches_tpoint_geo(temp_converted, gs_converted, restr, atvalue)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_tand_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_tand_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tbool_tor_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tbool_tor_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_extent_transfn(p: "Optional['Span *']", temp: 'const Temporal *') -> 'Span *':
+    p_converted = _ffi.cast('Span *', p) if p is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_extent_transfn(p_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_tagg_finalfn(state: 'SkipList *') -> 'Temporal *':
+    state_converted = _ffi.cast('SkipList *', state)
+    result = _lib.temporal_tagg_finalfn(state_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_tcount_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_tcount_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_tmax_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_tmin_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tfloat_tsum_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tfloat_tsum_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_tmax_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_tmin_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_tsum_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tint_tsum_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_extent_transfn(box: "Optional['TBox *']", temp: 'const Temporal *') -> 'TBox *':
+    box_converted = _ffi.cast('TBox *', box) if box is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_extent_transfn(box_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_integral(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_integral(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_tavg_finalfn(state: 'SkipList *') -> 'Temporal *':
+    state_converted = _ffi.cast('SkipList *', state)
+    result = _lib.tnumber_tavg_finalfn(state_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_tavg_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_tavg_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tnumber_twavg(temp: 'const Temporal *') -> 'double':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tnumber_twavg(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_extent_transfn(box: "Optional['STBox *']", temp: 'const Temporal *') -> 'STBox *':
+    box_converted = _ffi.cast('STBox *', box) if box is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_extent_transfn(box_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_tcentroid_finalfn(state: 'SkipList *') -> 'Temporal *':
+    state_converted = _ffi.cast('SkipList *', state)
+    result = _lib.tpoint_tcentroid_finalfn(state_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_tcentroid_transfn(state: 'SkipList *', temp: 'Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state)
+    temp_converted = _ffi.cast('Temporal *', temp)
+    result = _lib.tpoint_tcentroid_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_twcentroid(temp: 'const Temporal *') -> 'GSERIALIZED *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.tpoint_twcentroid(temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_tmax_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_tmax_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def ttext_tmin_transfn(state: "Optional['SkipList *']", temp: 'const Temporal *') -> 'SkipList *':
+    state_converted = _ffi.cast('SkipList *', state) if state is not None else _ffi.NULL
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.ttext_tmin_transfn(state_converted, temp_converted)
+    return result if result != _ffi.NULL else None
+
+
+def float_bucket(value: float, size: float, origin: float) -> 'double':
+    result = _lib.float_bucket(value, size, origin)
+    return result if result != _ffi.NULL else None
+
+
+def floatspan_bucket_list(bounds: 'const Span *', size: float, origin: float, newcount: 'int *') -> 'Span *':
+    bounds_converted = _ffi.cast('const Span *', bounds)
+    newcount_converted = _ffi.cast('int *', newcount)
+    result = _lib.floatspan_bucket_list(bounds_converted, size, origin, newcount_converted)
+    return result if result != _ffi.NULL else None
+
+
+def int_bucket(value: int, size: int, origin: int) -> 'int':
+    result = _lib.int_bucket(value, size, origin)
+    return result if result != _ffi.NULL else None
+
+
+def intspan_bucket_list(bounds: 'const Span *', size: int, origin: int, newcount: 'int *') -> 'Span *':
+    bounds_converted = _ffi.cast('const Span *', bounds)
+    newcount_converted = _ffi.cast('int *', newcount)
+    result = _lib.intspan_bucket_list(bounds_converted, size, origin, newcount_converted)
+    return result if result != _ffi.NULL else None
+
+
+def period_bucket_list(bounds: 'const Span *', duration: 'const Interval *', origin: int, newcount: 'int *') -> 'Span *':
+    bounds_converted = _ffi.cast('const Span *', bounds)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    origin_converted = _ffi.cast('TimestampTz', origin)
+    newcount_converted = _ffi.cast('int *', newcount)
+    result = _lib.period_bucket_list(bounds_converted, duration_converted, origin_converted, newcount_converted)
+    return result if result != _ffi.NULL else None
+
+
+def stbox_tile_list(bounds: 'const STBox *', xsize: float, ysize: float, zsize: float, duration: "Optional['const Interval *']", sorigin: 'GSERIALIZED *', torigin: int) -> "Tuple['STBox *', 'int *']":
+    bounds_converted = _ffi.cast('const STBox *', bounds)
+    duration_converted = _ffi.cast('const Interval *', duration) if duration is not None else _ffi.NULL
+    sorigin_converted = _ffi.cast('GSERIALIZED *', sorigin)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    cellcount = _ffi.new('int **')
+    result = _lib.stbox_tile_list(bounds_converted, xsize, ysize, zsize, duration_converted, sorigin_converted, torigin_converted, cellcount)
+    return result if result != _ffi.NULL else None, cellcount[0]
+
+
+def tbox_tile_list(bounds: 'const TBox *', xsize: float, duration: 'const Interval *', xorigin: 'Optional[float]', torigin: "Optional[int]") -> "Tuple['TBox *', 'int', 'int']":
+    bounds_converted = _ffi.cast('const TBox *', bounds)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    xorigin_converted = xorigin if xorigin is not None else _ffi.NULL
+    torigin_converted = _ffi.cast('TimestampTz', torigin) if torigin is not None else _ffi.NULL
+    rows = _ffi.new('int *')
+    columns = _ffi.new('int *')
+    result = _lib.tbox_tile_list(bounds_converted, xsize, duration_converted, xorigin_converted, torigin_converted, rows, columns)
+    return result if result != _ffi.NULL else None, rows[0], columns[0]
+
+
+def temporal_time_split(temp: 'Temporal *', duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('Temporal *', temp)
+    duration_converted = _ffi.cast('Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    newcount = _ffi.new('int *')
+    result = _lib.temporal_time_split(temp_converted, duration_converted, torigin_converted, newcount)
+    return result if result != _ffi.NULL else None, newcount[0]
+
+
+def tfloat_value_split(temp: 'Temporal *', size: float, origin: float) -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('Temporal *', temp)
+    newcount = _ffi.new('int *')
+    result = _lib.tfloat_value_split(temp_converted, size, origin, newcount)
+    return result if result != _ffi.NULL else None, newcount[0]
+
+
+def tfloat_value_time_split(temp: 'Temporal *', size: float, vorigin: float, duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('Temporal *', temp)
+    duration_converted = _ffi.cast('Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    newcount = _ffi.new('int *')
+    result = _lib.tfloat_value_time_split(temp_converted, size, vorigin, duration_converted, torigin_converted, newcount)
+    return result if result != _ffi.NULL else None, newcount[0]
+
+
+def timestamptz_bucket(timestamp: int, duration: 'const Interval *', origin: int) -> 'TimestampTz':
+    timestamp_converted = _ffi.cast('TimestampTz', timestamp)
+    duration_converted = _ffi.cast('const Interval *', duration)
+    origin_converted = _ffi.cast('TimestampTz', origin)
+    result = _lib.timestamptz_bucket(timestamp_converted, duration_converted, origin_converted)
+    return result if result != _ffi.NULL else None
+
+
+def tint_value_split(temp: 'Temporal *', size: int, origin: int) -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('Temporal *', temp)
+    newcount = _ffi.new('int *')
+    result = _lib.tint_value_split(temp_converted, size, origin, newcount)
+    return result if result != _ffi.NULL else None, newcount[0]
+
+
+def tint_value_time_split(temp: 'Temporal *', size: int, vorigin: int, duration: 'Interval *', torigin: int) -> "Tuple['Temporal **', 'int']":
+    temp_converted = _ffi.cast('Temporal *', temp)
+    duration_converted = _ffi.cast('Interval *', duration)
+    torigin_converted = _ffi.cast('TimestampTz', torigin)
+    newcount = _ffi.new('int *')
+    result = _lib.tint_value_time_split(temp_converted, size, vorigin, duration_converted, torigin_converted, newcount)
+    return result if result != _ffi.NULL else None, newcount[0]
+
+
+def temporal_dyntimewarp_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_dyntimewarp_distance(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_dyntimewarp_path(temp1: 'const Temporal *', temp2: 'const Temporal *') -> "Tuple['Match *', 'int']":
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    count = _ffi.new('int *')
+    result = _lib.temporal_dyntimewarp_path(temp1_converted, temp2_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_frechet_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_frechet_distance(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_frechet_path(temp1: 'const Temporal *', temp2: 'const Temporal *') -> "Tuple['Match *', 'int']":
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    count = _ffi.new('int *')
+    result = _lib.temporal_frechet_path(temp1_converted, temp2_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def temporal_hausdorff_distance(temp1: 'const Temporal *', temp2: 'const Temporal *') -> 'double':
+    temp1_converted = _ffi.cast('const Temporal *', temp1)
+    temp2_converted = _ffi.cast('const Temporal *', temp2)
+    result = _lib.temporal_hausdorff_distance(temp1_converted, temp2_converted)
+    return result if result != _ffi.NULL else None
+
+
+def geo_to_tpoint(geo: 'const GSERIALIZED *') -> 'Temporal *':
+    geo_converted = _ffi.cast('const GSERIALIZED *', geo)
+    result = _lib.geo_to_tpoint(geo_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_simplify_min_dist(temp: 'const Temporal *', dist: float) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_simplify_min_dist(temp_converted, dist)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_simplify_min_tdelta(temp: 'const Temporal *', mint: 'const Interval *') -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    mint_converted = _ffi.cast('const Interval *', mint)
+    result = _lib.temporal_simplify_min_tdelta(temp_converted, mint_converted)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_simplify_dp(temp: 'const Temporal *', eps_dist: float, synchronized: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_simplify_dp(temp_converted, eps_dist, synchronized)
+    return result if result != _ffi.NULL else None
+
+
+def temporal_simplify_max_dist(temp: 'const Temporal *', eps_dist: float, synchronized: bool) -> 'Temporal *':
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    result = _lib.temporal_simplify_max_dist(temp_converted, eps_dist, synchronized)
+    return result if result != _ffi.NULL else None
+
+
+def tpoint_AsMVTGeom(temp: 'const Temporal *', bounds: 'const STBox *', extent: 'int32_t', buffer: 'int32_t', clip_geom: bool, geom: 'GSERIALIZED **', timesarr: 'int64 **') -> "Tuple['bool', 'int']":
+    temp_converted = _ffi.cast('const Temporal *', temp)
+    bounds_converted = _ffi.cast('const STBox *', bounds)
+    extent_converted = _ffi.cast('int32_t', extent)
+    buffer_converted = _ffi.cast('int32_t', buffer)
+    geom_converted = [_ffi.cast('GSERIALIZED *', x) for x in geom]
+    timesarr_converted = [_ffi.cast('int64 *', x) for x in timesarr]
+    count = _ffi.new('int *')
+    result = _lib.tpoint_AsMVTGeom(temp_converted, bounds_converted, extent_converted, buffer_converted, clip_geom, geom_converted, timesarr_converted, count)
+    return result if result != _ffi.NULL else None, count[0]
+
+
+def tpoint_to_geo_meas(tpoint: 'const Temporal *', measure: 'const Temporal *', segmentize: bool) -> 'GSERIALIZED **':
+    tpoint_converted = _ffi.cast('const Temporal *', tpoint)
+    measure_converted = _ffi.cast('const Temporal *', measure)
+    out_result = _ffi.new('GSERIALIZED **')
+    result = _lib.tpoint_to_geo_meas(tpoint_converted, measure_converted, segmentize, out_result)
+    if result:
+        return out_result if out_result != _ffi.NULL else None
+    return None
+
+
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/PKG-INFO` & `pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos-cffi
-Version: 1.1.0a1
+Version: 1.1.0a2
 Summary: PyMEOS wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>
 License: -------------------------------------------------------------------------------
         This PyMEOS code is provided under The PostgreSQL License.
         
         Copyright (c) 2020, Université libre de Bruxelles and MobilityDB contributors
```

### Comparing `pymeos_cffi-1.1.0a1/pymeos_cffi.egg-info/SOURCES.txt` & `pymeos_cffi-1.1.0a2/pymeos_cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0a1/pyproject.toml` & `pymeos_cffi-1.1.0a2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-[build-system]
-requires = ['setuptools>=61.0']
-build-backend = 'setuptools.build_meta'
-
-[tool.setuptools]
-py-modules = []
-
-[project]
-name = 'pymeos_cffi'
-version = '1.1.0-alpha.1'
-authors = [
-    { name = 'Victor Divi', email = 'vdiviloper@gmail.com' }
-]
-description = 'PyMEOS wrapper for the MEOS C Library.'
-classifiers = [
-    'License :: OSI Approved :: PostgreSQL License',
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'Intended Audience :: Science/Research',
-    'Programming Language :: C',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: Implementation :: CPython',
-    'Operating System :: POSIX',
-    'Operating System :: Unix'
-]
-readme = 'README.md'
-license = { file = 'LICENSE' }
-
-requires-python = '>=3.7'
-dependencies = [
-    'cffi',
-    'python-dateutil',
-    'spans',
-    'postgis',
-    'shapely'
-]
-
-[project.urls]
-'Homepage' = 'https://github.com/MobilityDB/PyMEOS'
+[build-system]
+requires = ['setuptools>=61.0']
+build-backend = 'setuptools.build_meta'
+
+[tool.setuptools]
+py-modules = []
+
+[project]
+name = 'pymeos_cffi'
+version = '1.1.0-alpha.2'
+authors = [
+    { name = 'Victor Divi', email = 'vdiviloper@gmail.com' }
+]
+description = 'PyMEOS wrapper for the MEOS C Library.'
+classifiers = [
+    'License :: OSI Approved :: PostgreSQL License',
+    'Development Status :: 3 - Alpha',
+    'Intended Audience :: Developers',
+    'Intended Audience :: Science/Research',
+    'Programming Language :: C',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: Implementation :: CPython',
+    'Operating System :: POSIX',
+    'Operating System :: Unix'
+]
+readme = 'README.md'
+license = { file = 'LICENSE' }
+
+requires-python = '>=3.7'
+dependencies = [
+    'cffi',
+    'python-dateutil',
+    'spans',
+    'postgis',
+    'shapely'
+]
+
+[project.urls]
+'Homepage' = 'https://github.com/MobilityDB/PyMEOS'
 'Bug Tracker' = 'https://github.com/MobilityDB/PyMEOS/issues'
```

