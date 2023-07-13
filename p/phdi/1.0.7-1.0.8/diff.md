# Comparing `tmp/phdi-1.0.7.tar.gz` & `tmp/phdi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.7.tar", max compression
+gzip compressed data, was "phdi-1.0.8.tar", max compression
```

## Comparing `phdi-1.0.7.tar` & `phdi-1.0.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-06-15 17:43:36.256598 phdi-1.0.7/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-06-15 17:43:36.256598 phdi-1.0.7/README.md
--rw-r--r--   0        0        0       22 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9436 2023-06-15 17:43:36.800605 phdi-1.0.7/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2776 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3640 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     8834 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5992 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     2555 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     3167 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/core.py
--rw-r--r--   0        0        0    59276 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/link.py
--rw-r--r--   0        0        0    15429 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2752 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-06-15 17:43:36.804606 phdi-1.0.7/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11838 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-06-15 17:43:36.808606 phdi-1.0.7/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1825 2023-06-15 17:43:36.816606 phdi-1.0.7/pyproject.toml
--rw-r--r--   0        0        0    13445 1970-01-01 00:00:00.000000 phdi-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-07-13 18:18:43.653036 phdi-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-07-13 18:18:43.653036 phdi-1.0.8/README.md
+-rw-r--r--   0        0        0       22 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 18:18:44.137032 phdi-1.0.8/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3640 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     8834 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5992 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     2555 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     3167 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/core.py
+-rw-r--r--   0        0        0    59276 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/link.py
+-rw-r--r--   0        0        0    15429 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2792 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11838 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-07-13 18:18:44.141032 phdi-1.0.8/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1824 2023-07-13 18:18:44.153031 phdi-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0    13543 1970-01-01 00:00:00.000000 phdi-1.0.8/PKG-INFO
```

### Comparing `phdi-1.0.7/LICENSE.md` & `phdi-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/README.md` & `phdi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/cloud/azure.py` & `phdi-1.0.8/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/cloud/core.py` & `phdi-1.0.8/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/cloud/gcp.py` & `phdi-1.0.8/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/containers/base_service.py` & `phdi-1.0.8/phdi/containers/base_service.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/cloud/azure.py` & `phdi-1.0.8/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/conversion/convert.py` & `phdi-1.0.8/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/geospatial/README.md` & `phdi-1.0.8/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/geospatial/census.py` & `phdi-1.0.8/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/geospatial/core.py` & `phdi-1.0.8/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.8/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/harmonization/README.md` & `phdi-1.0.8/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.8/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/linkage/link.py` & `phdi-1.0.8/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/tabulation/tables.py` & `phdi-1.0.8/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/transport/export.py` & `phdi-1.0.8/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/transport/http.py` & `phdi-1.0.8/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/fhir/utils.py` & `phdi-1.0.8/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/geospatial/README.md` & `phdi-1.0.8/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/geospatial/census.py` & `phdi-1.0.8/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/geospatial/core.py` & `phdi-1.0.8/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/geospatial/smarty.py` & `phdi-1.0.8/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/README.md` & `phdi-1.0.8/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/__init__.py` & `phdi-1.0.8/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/double_metaphone.py` & `phdi-1.0.8/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/hl7.py` & `phdi-1.0.8/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.8/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/standardization.py` & `phdi-1.0.8/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/harmonization/utils.py` & `phdi-1.0.8/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/__init__.py` & `phdi-1.0.8/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/algorithms.py` & `phdi-1.0.8/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/core.py` & `phdi-1.0.8/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/link.py` & `phdi-1.0.8/phdi/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/postgres.py` & `phdi-1.0.8/phdi/linkage/postgres.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/linkage/seed.py` & `phdi-1.0.8/phdi/linkage/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,21 @@
                             "code": "SS",
                         }
                     ]
                 },
                 "value": f"{data.get('ssn',None)}",
             },
         ],
-        "name": {
-            "family": f"{data.get('last_name',None)}",
-            "given": data.get("first_name", None).split()
-            + data.get("middle_name", None).split(),
-        },
+        "name": [
+            {
+                "family": f"{data.get('last_name',None)}",
+                "given": data.get("first_name", None).split()
+                + data.get("middle_name", None).split(),
+            }
+        ],
         "telecom": [
             {
                 "system": "phone",
                 "value": f"{data.get('home_phone',None)}",
                 "use": "home",
             },
             {
```

### Comparing `phdi-1.0.7/phdi/tabulation/tables.py` & `phdi-1.0.8/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/tabulation/validation_schema.json` & `phdi-1.0.8/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/transport/http.py` & `phdi-1.0.8/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/validation/__init__.py` & `phdi-1.0.8/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/validation/validation.py` & `phdi-1.0.8/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/phdi/validation/xml_utils.py` & `phdi-1.0.8/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.7/pyproject.toml` & `phdi-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.7"
+version = "v1.0.8"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11.3"
+python = "^3.10"
 smartystreets-python-sdk = "^4.10.6"
 pydantic = "^1.10.9"
 fastapi = "^0.96.0"
 httpx = "^0.23.3"
 hl7 = "^0.4.5"
 azure-identity = "^1.10.0"
 azure-storage-blob = "^12.12.0"
@@ -47,8 +47,8 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = 6.0
-addopts = "--doctest-modules"
+addopts = "--doctest-modules"
```

### Comparing `phdi-1.0.7/PKG-INFO` & `phdi-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
-Requires-Python: >=3.11.3,<4.0.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: azure-storage-blob (>=12.12.0,<13.0.0)
 Requires-Dist: coverage (>=6.4.1,<7.0.0)
 Requires-Dist: detect-delimiter (>=0.1.1,<0.2.0)
 Requires-Dist: faker (>=18.4.0,<19.0.0)
```

