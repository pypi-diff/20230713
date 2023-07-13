# Comparing `tmp/ogc_na-0.2.9.tar.gz` & `tmp/ogc_na-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.9.tar", last modified: Mon May 15 21:16:59 2023, max compression
+gzip compressed data, was "ogc_na-0.3.0.tar", last modified: Thu Jul 13 09:39:29 2023, max compression
```

## Comparing `ogc_na-0.2.9.tar` & `ogc_na-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-15 21:16:47.000000 ogc_na-0.2.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-15 21:16:47.000000 ogc_na-0.2.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 21:16:47.000000 ogc_na-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 21:16:59.727024 ogc_na-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 21:16:47.000000 ogc_na-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-15 21:16:47.000000 ogc_na-0.2.9/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-15 21:16:47.000000 ogc_na-0.2.9/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.723024 ogc_na-0.2.9/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21772 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-15 21:16:47.000000 ogc_na-0.2.9/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 21:16:59.000000 ogc_na-0.2.9/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 21:16:47.000000 ogc_na-0.2.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 21:16:47.000000 ogc_na-0.2.9/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 21:16:47.000000 ogc_na-0.2.9/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 21:16:47.000000 ogc_na-0.2.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:16:59.727024 ogc_na-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 21:16:47.000000 ogc_na-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:59.727024 ogc_na-0.2.9/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-15 21:16:47.000000 ogc_na-0.2.9/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.793216 ogc_na-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 09:39:19.000000 ogc_na-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-13 09:39:19.000000 ogc_na-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 09:39:19.000000 ogc_na-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 09:39:29.793216 ogc_na-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 09:39:19.000000 ogc_na-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-13 09:39:19.000000 ogc_na-0.3.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc/na/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32640 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 09:39:19.000000 ogc_na-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 09:39:19.000000 ogc_na-0.3.0/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-13 09:39:19.000000 ogc_na-0.3.0/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 09:39:19.000000 ogc_na-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:39:29.793216 ogc_na-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 09:39:19.000000 ogc_na-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_profile.py
```

### Comparing `ogc_na-0.2.9/.github/workflows/python-publish.yml` & `ogc_na-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/.gitignore` & `ogc_na-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/PKG-INFO` & `ogc_na-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.2.9
+Version: 0.3.0
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
-Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
+Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
```

### Comparing `ogc_na-0.2.9/README.md` & `ogc_na-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/docs/examples.md` & `ogc_na-0.3.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/docs/gen_ref_pages.py` & `ogc_na-0.3.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/docs/index.md` & `ogc_na-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/docs/tutorials.md` & `ogc_na-0.3.0/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/mkdocs.yml` & `ogc_na-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/ogc/na/domain_config.py` & `ogc_na-0.3.0/ogc/na/domain_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 defining how to find and select files for processing.
 """
 
 from __future__ import annotations
 import logging
 import os
 from pathlib import Path
-from typing import Union, Optional, Sequence, cast, IO, TypeVar
+from typing import Union, Optional, Sequence, cast, IO, TypeVar, Iterable
 
 import wcmatch.glob
 from rdflib import Graph, Namespace, URIRef, DCTERMS, DCAT, Literal
 from wcmatch.glob import globmatch
 
 from ogc.na.profile import ProfileRegistry
 
@@ -102,15 +102,17 @@
     which is the main concept scheme in the file (if more than one is found). Profiles for
     validation, entailment, etc. can be specified using `dcterms:conformsTo`.
 
     `dcfg:hasUpliftDefinition` can also be used to declare (ordered) semantic uplift definitions, either
     from profile artifacts or from files.
     """
 
-    def __init__(self, source: Union[Graph, str, Path, IO], working_directory: str | Path = None):
+    def __init__(self, source: Union[Graph, str, Path, IO], working_directory: str | Path = None,
+                 profile_sources: str | Path | Iterable[str | Path] | None = None,
+                 ignore_artifact_errors=False):
         """
         Creates a new DomainConfiguration, optionally specifying the working directory.
 
         :param source: Graph or Turtle file to load
         :param working_directory: the working directory to use for local paths.
         """
         if working_directory:
@@ -120,14 +122,17 @@
         else:
             self.working_directory = Path().resolve()
         logger.info("Working directory: %s", self.working_directory)
         self.entries = ConfigurationEntryList()
         self.uplift_entries = UpliftConfigurationEntryList()
         self.local_artifacts_mapping = {}
         self.profile_registry: ProfileRegistry | None = None
+        self._profile_sources = profile_sources
+        self._ignore_artifact_errors = ignore_artifact_errors
+
         self._load(source)
 
     def _load(self, source: Union[Graph, str, IO]):
         """
         Load entries from a Graph or Turtle document.
 
         :param source: Graph or Turtle file to load
@@ -140,15 +145,15 @@
             service = source[len('sparql:'):]
             g = Graph()
         else:
             g = Graph().parse(source)
 
         cfg_graph = g.query(DOMAIN_CFG_QUERY.replace('__SERVICE__', service)).graph
 
-        ignore_profile_artifact_errors = False
+        ignore_profile_artifact_errors = self._ignore_artifact_errors
 
         prof_sources: set[str | Path] = set()
         for catalog_ref in cfg_graph.subjects(DCAT.dataset):
             logger.debug("Found catalog %s", catalog_ref)
 
             if bool(cfg_graph.value(catalog_ref, DCFG.ignoreProfileArtifactErrors)):
                 ignore_profile_artifact_errors = True
@@ -163,15 +168,18 @@
             # Profile sources
             for p in cfg_graph.objects(catalog_ref, DCFG.hasProfileSource):
                 if not isinstance(p, Literal):
                     continue
                 if p.value.startswith('sparql:'):
                     prof_sources.add(p.value)
                 else:
-                    prof_sources.add(self.working_directory / p.value)
+                    prof_sources.update(self.working_directory.glob(p.value))
+
+            if self._profile_sources:
+                prof_sources.update(self._profile_sources)
 
         self.profile_registry = ProfileRegistry(prof_sources,
                                                 ignore_artifact_errors=ignore_profile_artifact_errors)
 
         for cfg_ref in cfg_graph.objects(predicate=DCAT.dataset):
 
             globs = [str(g) for g in cfg_graph.objects(cfg_ref, DCFG.glob)]
```

### Comparing `ogc_na-0.2.9/ogc/na/download.py` & `ogc_na-0.3.0/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/ogc/na/ingest_json.py` & `ogc_na-0.3.0/ogc/na/ingest_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,24 +38,26 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from os import scandir
 from pathlib import Path
 from typing import Union, Optional, Sequence, cast, Iterable, Any
 
 import jq
+import pyld.jsonld
 from jsonpath_ng.ext import parse as json_path_parse
 from jsonschema import validate as json_validate
 from pyld import jsonld
 from rdflib import Graph, DC, DCTERMS, SKOS, OWL, RDF, RDFS, XSD, DCAT
 from rdflib.namespace import Namespace, DefinedNamespace
 
 from ogc.na import util, profile
 from ogc.na.domain_config import UpliftConfigurationEntry, DomainConfiguration
 from ogc.na.provenance import ProvenanceMetadata, FileProvenanceMetadata, generate_provenance
 from ogc.na.input_filters import apply_input_filter
+from ogc.na.util import is_iri
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_NAMESPACES: dict[str, Union[str, DefinedNamespace]] = {
     "dc": DC,
     "xsd": XSD,
     "dct": DCTERMS,
@@ -155,15 +157,17 @@
         if url_whitelist is not None and not any(re.match(r, url) for r in url_whitelist if r):
             raise ValueError('Remote document fetching not allowed for URL {}'.format(url))
         return wrapped(url, options=options or {})
 
     return loader
 
 
-def validate_context(context: Union[dict, str] = None, filename: Union[str, Path] = None) -> dict:
+def validate_context(context: Union[dict, str] = None,
+                     filename: Union[str, Path] = None,
+                     transform_args: dict | None = None) -> dict:
     if not context and not filename:
         return {}
     if bool(context) == bool(filename):
         raise ValueError("Only one of context or filename required")
 
     if not isinstance(context, dict):
         context = util.load_yaml(filename=filename, content=context)
@@ -174,15 +178,15 @@
         raise ValidationError(cause=e)
 
     transform = context.get('transform', [])
     if isinstance(transform, str):
         transform = [transform]
     for i, t in enumerate(transform):
         try:
-            jq.compile(t)
+            jq.compile(t, args=transform_args)
         except Exception as e:
             raise ValidationError(cause=e,
                                   msg=f"Error compiling jq expression for transform at index {i}",
                                   property="transform",
                                   value=t,
                                   index=i)
     for json_path in context.get('types', {}).keys():
@@ -209,48 +213,50 @@
         json_doc = [json_doc]
     json_doc.extend(prov)
     return json_doc
 
 
 def uplift_json(data: dict | list, context: dict,
                 fetch_timeout: int = 5,
-                fetch_url_whitelist: Optional[Union[Sequence, bool]] = None) -> dict:
+                fetch_url_whitelist: Optional[Union[Sequence, bool]] = None,
+                transform_args: dict | None = None) -> dict:
     """
     Transform a JSON document loaded in a dict, and embed JSON-LD context into it.
 
     WARNING: This function modifies the input dict. If that is not desired, make a copy
     before invoking.
 
     :param data: the JSON document in dict format
     :param context: YAML context definition
     :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception.
+    :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: the transformed and JSON-LD-enriched data
     """
 
     context_position = context.get('position', 'before')
 
     jsonld.set_document_loader(_document_loader(timeout=fetch_timeout, url_whitelist=fetch_url_whitelist))
 
-    validate_context(context)
+    validate_context(context, transform_args=transform_args)
 
     # Check whether @graph scoping is necessary for transformations and paths
     scoped_graph = context.get('scope', 'graph') == 'graph' and '@graph' in data
     data_graph = data['@graph'] if scoped_graph else data
 
     # Check if pre-transform necessary
     transform = context.get('transform')
     if transform:
         # Allow for transform lists to do sequential transformations
         if isinstance(transform, str):
             transform = (transform,)
         for i, t in enumerate(transform):
-            tranformed_txt = jq.compile(t).input(data_graph).text()
+            tranformed_txt = jq.compile(t, args=transform_args).input(data_graph).text()
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug('After transform %d:\n%s', i + 1, tranformed_txt)
             data_graph = json.loads(tranformed_txt)
 
     # Add types
     types = context.get('types', {})
     for loc, type_list in types.items():
@@ -276,22 +282,30 @@
         if not loc or loc in ['.', '$']:
             global_context = val
         else:
             items = json_path_parse(loc).find(data_graph)
             for item in items:
                 item.value['@context'] = _get_injected_context(item.value, val, context_position)
 
+    data_context = data_graph.pop('@context', None)
+    if data_context:
+        if not global_context:
+            global_context = data_context
+        elif isinstance(global_context, list):
+            global_context.extend(data_context)
+        else:
+            global_context = [data_context, global_context]
+
     if (global_context and not isinstance(data_graph, dict)) or scoped_graph:
         return {
             '@context': _get_injected_context(data, global_context, context_position),
             '@graph': data_graph,
         }
     else:
         if global_context:
-            data_graph.pop('@context', None)
             return {
                 '@context': _get_injected_context(data, global_context, context_position),
                 **data_graph
             }
         return data_graph
 
 
@@ -325,84 +339,102 @@
     return result
 
 
 def generate_graph(input_data: dict | list,
                    context: dict[str, Any] | Sequence[dict] = None,
                    base: str | None = None,
                    fetch_timeout: int = 5,
-                   fetch_url_whitelist: Sequence[str] | bool | None = None) -> UpliftResult:
+                   fetch_url_whitelist: Sequence[str] | bool | None = None,
+                   transform_args: dict | None = None) -> UpliftResult:
     """
     Create a graph from an input JSON document and a YAML context definition file.
 
     :param input_data: input JSON data in dict or list format
     :param context: context definition in dict format, or list thereof
     :param base: base URI for JSON-LD context
     :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception.
+    :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: a tuple with the resulting RDFLib Graph and the JSON-LD enriched file name
     """
 
     if not isinstance(input_data, dict) and not isinstance(input_data, list):
         raise ValueError('input_data must be a list or dictionary')
 
-    if not context:
-        raise ValueError('context must be provided')
-
     g = Graph()
-    base_uri = None
-    for prefix, ns in DEFAULT_NAMESPACES.items():
-        g.bind(prefix, Namespace(ns))
-
     jdoc_ld = input_data
-    context_list = context if isinstance(context, Sequence) else (context,)
-    for context_entry in context_list:
-        base_uri = context_entry.get('base-uri', base_uri)
-        jdoc_ld = uplift_json(input_data, context_entry,
-                              fetch_timeout=fetch_timeout,
-                              fetch_url_whitelist=fetch_url_whitelist)
+    if context:
+        base_uri = None
+        for prefix, ns in DEFAULT_NAMESPACES.items():
+            g.bind(prefix, Namespace(ns))
+
+        context_list = context if isinstance(context, Sequence) else (context,)
+        for context_entry in context_list:
+            base_uri = context_entry.get('base-uri', base_uri)
+            jdoc_ld = uplift_json(input_data, context_entry,
+                                  fetch_timeout=fetch_timeout,
+                                  fetch_url_whitelist=fetch_url_whitelist,
+                                  transform_args=transform_args)
+            if 'context' in context_entry:
+                if '$' in context_entry['context']:
+                    root_ctx = context_entry['context']['$']
+                elif '.' in context_entry['context']:
+                    root_ctx = context_entry['context']['.']
+                else:
+                    continue
 
-    options = {}
-    if not base:
-        if base_uri:
-            options['base'] = context['base-uri']
-        elif '@context' in jdoc_ld:
-            # Try to extract from @context
-            # If it is a list, iterate until @base is found
-            base = None
-            if isinstance(jdoc_ld['@context'], list):
-                for entry in jdoc_ld['@context']:
-                    if not isinstance(entry, dict):
-                        continue
-                    base = entry.get('@base')
-                    if base:
-                        break
-            else:
-                # If not a list, just look @base up
-                base = jdoc_ld['@context'].get('@base')
-    if base:
-        options['base'] = base
-    if logger.isEnabledFor(logging.DEBUG):
-        logger.debug('Uplifted JSON:\n%s', json.dumps(jdoc_ld, indent=2))
-    g.parse(data=json.dumps(jdoc_ld), format='json-ld')
+                for term, term_val in root_ctx.items():
+                    if not term.startswith('@') \
+                            and isinstance(term_val, str) \
+                            and re.match(r'.+[#/:]$', term_val) \
+                            and is_iri(term_val):
+                        g.bind(term, term_val)
+
+        options = {}
+        if not base:
+            if base_uri:
+                options['base'] = context['base-uri']
+            elif '@context' in jdoc_ld:
+                # Try to extract from @context
+                # If it is a list, iterate until @base is found
+                base = None
+                if isinstance(jdoc_ld['@context'], list):
+                    for entry in jdoc_ld['@context']:
+                        if not isinstance(entry, dict):
+                            continue
+                        base = entry.get('@base')
+                        if base:
+                            break
+                else:
+                    # If not a list, just look @base up
+                    base = jdoc_ld['@context'].get('@base')
+        if base:
+            options['base'] = base
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug('Uplifted JSON:\n%s', json.dumps(jdoc_ld, indent=2))
+
+    expanded = pyld.jsonld.expand(jdoc_ld, options)
+    g.parse(data=json.dumps(expanded), format='json-ld')
 
     return UpliftResult(graph=g, uplifted_json=jdoc_ld)
 
 
 def process_file(input_fn: str | Path,
                  jsonld_fn: str | Path | bool | None = False,
                  ttl_fn: str | Path | bool | None = False,
                  context_fn: str | Path | Sequence[str | Path] | None = None,
                  domain_cfg: DomainConfiguration | None = None,
                  base: str | None = None,
                  provenance_base_uri: str | bool | None = None,
                  provenance_process_id: str | None = None,
                  fetch_timeout: int = 5,
-                 fetch_url_whitelist: bool | Sequence[str] | None = None) -> UpliftResult | None:
+                 fetch_url_whitelist: bool | Sequence[str] | None = None,
+                 transform_args: dict | None = None) -> UpliftResult | None:
     """
     Process input file and generate output RDF files.
 
     :param input_fn: input filename
     :param jsonld_fn: output JSON-lD filename (None for automatic).
         If False, no JSON-LD output will be generated
     :param ttl_fn: output Turtle filename (None for automatic).
@@ -415,14 +447,15 @@
     :param base: base URI for JSON-LD
     :param provenance_base_uri: base URI for provenance resources
     :param provenance_process_id: process identifier for provenance tracking
     :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception
+    :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: List of output files created
     """
 
     start_time = datetime.now()
 
     if not isinstance(input_fn, Path):
         input_fn = Path(input_fn)
@@ -445,14 +478,15 @@
                         provenance_contexts.append(a)
 
     elif not isinstance(context_fn, Sequence) or isinstance(context_fn, str):
         provenance_contexts = (context_fn,)
         contexts = (util.load_yaml(context_fn),)
     else:
         provenance_contexts = context_fn
+        contexts = [util.load_yaml(fn) for fn in context_fn]
 
     if not contexts:
         raise MissingContextException('No context file provided and one could not be discovered automatically')
 
     # Apply input filter of first context only (if any)
     input_filters = contexts[0].get('input-filter')
     if input_filters:
@@ -475,19 +509,30 @@
             batch_activity_id=provenance_process_id,
             base_uri=provenance_base_uri,
             root_directory=os.getcwd(),
             start=start_time,
             end_auto=True,
         )
 
+    if transform_args is None:
+        transform_args = {}
+    transform_args['_filename'] = str(input_fn.resolve())
+    transform_args['_basename'] = str(input_fn.name)
+    transform_args['_dirname'] = str(input_fn.resolve().parent)
+    transform_args['_relname'] = os.path.relpath(input_fn)
+
+    if not base:
+        base = str(input_fn)
+
     uplift_result = generate_graph(input_data,
                                    context=contexts,
                                    base=base,
                                    fetch_timeout=fetch_timeout,
-                                   fetch_url_whitelist=fetch_url_whitelist)
+                                   fetch_url_whitelist=fetch_url_whitelist,
+                                   transform_args=transform_args)
 
     uplift_result.input_file = input_fn
 
     # False = do not generate
     # None = auto filename
     # - = stdout
     if ttl_fn is not False:
@@ -616,15 +661,16 @@
             jsonld_fn: bool | str | Path | None = False,
             ttl_fn: bool | str | Path | None = False,
             batch: bool = False,
             base: str = None,
             skip_on_missing_context: bool = False,
             provenance_base_uri: Optional[Union[str, bool]] = None,
             fetch_timeout: int = 5,
-            fetch_url_whitelist: Optional[Union[Sequence, bool]] = None) -> list[UpliftResult]:
+            fetch_url_whitelist: Optional[Union[Sequence, bool]] = None,
+            transform_args: dict | None = None) -> list[UpliftResult]:
     """
     Performs the JSON-LD uplift process.
 
     :param input_files: list of input, plain JSON files
     :param domain_cfg: domain configuration including uplift definition locations
     :param context_fn: used to force the YAML context file name for the uplift. If `None`,
            it will be autodetected
@@ -637,26 +683,32 @@
     :param base: base URI to employ
     :param skip_on_missing_context: whether to silently fail if no context file is found
     :param provenance_base_uri: base URI for provenance resources
     :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
         throw an exception
+    :param transform_args: Additional arguments to pass as variables to the jq transform
     :return: a list of JSON-LD and/or Turtle output files
     """
     result: list[UpliftResult] = []
     process_id = str(uuid.uuid4())
+    workdir = Path()
     if isinstance(input_files, str) or not isinstance(input_files, Sequence):
         input_files = (input_files,)
     if batch:
         logger.info("Input files: %s", input_files)
         remaining_fn: deque = deque()
         for input_file in input_files:
             if isinstance(input_file, str):
-                remaining_fn.extend(input_file.split(','))
+                for x in filter(lambda x: x, input_file.split(',')):
+                    if '?' in x or '#' in x:
+                        remaining_fn.extend(workdir.glob(x))
+                    else:
+                        remaining_fn.append(x)
             else:
                 remaining_fn.append(input_file)
         while remaining_fn:
             fn = str(remaining_fn.popleft())
 
             if not fn or not os.path.isfile(fn):
                 continue
@@ -676,16 +728,17 @@
                     context_fn=None,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
                     fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
                     domain_cfg=domain_cfg,
+                    transform_args=transform_args,
                 ))
-            except Exception as e:
+            except MissingContextException as e:
                 if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
                 else:
                     raise
     else:
         for input_file in input_files:
             try:
@@ -696,14 +749,15 @@
                     context_fn=context_fn,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
                     fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
                     domain_cfg=domain_cfg,
+                    transform_args=transform_args,
                 ))
             except Exception as e:
                 if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
                 else:
                     raise
 
@@ -805,14 +859,20 @@
     )
 
     parser.add_argument(
         '--work-dir',
         help='Set root directory for globs in domain configurations'
     )
 
+    parser.add_argument(
+        '--transform-arg',
+        nargs='*',
+        help='Additional argument to pass to the jq transforms in the form variable=value'
+    )
+
     args = parser.parse_args()
 
     if args.domain_config:
         domain_cfg = DomainConfiguration(args.domain_config, args.work_dir)
     else:
         domain_cfg = None
 
@@ -823,24 +883,29 @@
     elif not input_files:
         print("Error: no input files provided")
         sys.exit(1)
 
     if args.debug:
         logger.setLevel(logging.DEBUG)
 
+    transform_args = None
+    if args.transform_arg:
+        transform_args = dict((e.split('=', 1) for e in args.transform_arg))
+
     result = process(input_files,
                      context_fn=args.context,
                      domain_cfg=domain_cfg,
                      jsonld_fn=args.json_ld_file if args.json_ld else False,
                      ttl_fn=args.ttl_file if args.ttl else False,
                      batch=args.batch,
                      skip_on_missing_context=args.skip_on_missing_context,
                      provenance_base_uri=False if args.no_provenance else args.provenance_base_uri,
                      fetch_url_whitelist=args.url_whitelist,
-                     )
+                     transform_args=transform_args,
+             )
 
     if args.fs:
         print(args.fs.join(str(output_file) for r in result for output_file in r.output_files))
 
 
 if __name__ == '__main__':
```

### Comparing `ogc_na-0.2.9/ogc/na/input_filters/__init__.py` & `ogc_na-0.3.0/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/ogc/na/input_filters/csv.py` & `ogc_na-0.3.0/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/ogc/na/profile.py` & `ogc_na-0.3.0/ogc/na/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         __SERVICE__ {
             { ?profile a prof:Profile } UNION { ?other prof:isProfileOf ?profile }
             ?profile prof:hasToken ?token .
             OPTIONAL {
                 { ?profile owl:sameAs+ ?sameAs } UNION { ?sameAs owl:sameAs+ ?profile }
             }
             OPTIONAL { ?profile rdfs:label ?label }
-            OPTIONAL { ?profile prof:isProfileOf+ ?ancestor }
+            OPTIONAL { ?profile prof:isProfileOf ?ancestor }
             OPTIONAL {
                 ?profile prof:hasResource ?resource .
                 ?resource prof:hasRole ?role ;
                     dct:conformsTo shacl: ;
                     prof:hasArtifact ?artifact
                 OPTIONAL {
                     ?resource prof:hasRole ?role ;
@@ -93,15 +93,15 @@
 
 class Profile:
 
     def __init__(self, uri: URIRef, token: str, profile_of: list[URIRef], label: str | None = None):
         self.uri = uri
         self.token = token
         self.label = label
-        self.profile_of = profile_of
+        self.profile_of = [p for p in profile_of if p != uri]
         self.artifacts: dict[URIRef, list[str]] = {}
 
     def add_artifact(self, role: URIRef, href: URIRef):
         self.artifacts.setdefault(role, []).append(href)
 
     def get_artifacts(self, role: URIRef) -> list[URIRef]:
         return self.artifacts.get(role, [])
@@ -155,31 +155,31 @@
                                 pending.add(prof_of)
                             known[prof_of] = True
             return list(known)
 
         # Otherwise, sort DAG
         # 1. Build dependency tree
         dependencies: dict[URIRef, set[URIRef] | None] = {}
-        pending = deque(profiles) # using a deque to try and preserve as much of the original order as possible
+        pending = deque(profiles)  # using a deque to try and preserve as much of the original order as possible
         while pending:
             prof_uri = pending.popleft()
             if prof_uri in dependencies:
                 # skip if already processed
                 continue
             prof = self.profiles.get(prof_uri)
             if not prof:
                 # skip if unknown
                 continue
-            prof_deps = (d for d in self.profiles.get(prof_uri).profile_of if d in self.profiles)
+            prof_deps = [d for d in self.profiles.get(prof_uri).profile_of if d in self.profiles]
             if not prof_deps:
                 # has no dependencies
                 dependencies[prof_uri] = None
             if not recursive:
                 # non-recursive => only work with provided profile list
-                prof_deps = (d for d in prof_deps if d in profiles)
+                prof_deps = [d for d in prof_deps if d in profiles]
             else:
                 for p in prof_deps:
                     if p not in pending:
                         pending.appendleft(p)
             dependencies[prof_uri] = set(prof_deps)
 
         result: list[URIRef] = []
@@ -188,26 +188,28 @@
             if not dependencies:
                 break
             removed = {}
             for parent_uri, child_uris in dependencies.items():
                 if not child_uris:
                     removed[parent_uri] = True
             if not removed:
-                dependencies_str = '; '.join(f"{p} <- {', '.join(str(c) for c in cs)}" for p, cs in dependencies.items())
+                dependencies_str = '; '.join(
+                    f"{p} <- {', '.join(str(c) for c in cs)}" for p, cs in dependencies.items())
                 raise ValueError(f'Cycle detected in profile DAG, cannot sort: {dependencies_str}')
             for rem in removed:
                 del dependencies[rem]
                 result.append(rem)
             removed = set(removed)
             for child_uris in dependencies.values():
                 child_uris -= removed
 
         return result
 
     def _load_profiles(self):
+        logger.debug("Loading profiles from %s", [str(x) for x in self._srcs])
         g: Graph = Graph()
         for src in self._srcs:
             if isinstance(src, str) and src.startswith('sparql:'):
                 endpoint = src[len('sparql:'):]
                 logger.info("Fetching profiles from SPARQL endpoint %s", endpoint)
                 assert util.is_url(endpoint, http_only=True)
                 s = g.query(PROFILES_QUERY.replace('__SERVICE__', f"SERVICE <{endpoint}>")).graph
@@ -237,14 +239,19 @@
                 for artifact_ref in g.objects(resource_ref, PROF.hasArtifact):
                     profile.add_artifact(role_ref, cast(URIRef, artifact_ref))
 
             self.profiles[profile_ref] = profile
             for same_as_ref in g.objects(profile_ref, OWL.sameAs):
                 self.profiles[cast(URIRef, same_as_ref)] = profile
 
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(f"Profiles loaded: %s", [str(p) for p in self.profiles])
+        else:
+            logger.info(f"Loaded {len(self.profiles)}")
+
     def _apply_mappings(self, uri: str) -> Path | str:
         """
         Returns the longest match in self._local_artifact_mappings (prefixes)
         for a given URI, or the URI itself if not found
         """
 
         if uri in self._local_artifact_mappings:
```

### Comparing `ogc_na-0.2.9/ogc/na/provenance.py` & `ogc_na-0.3.0/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/ogc/na/update_vocabs.py` & `ogc_na-0.3.0/ogc/na/update_vocabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from typing import Union, Generator
 
 import requests
 from rdflib import Graph, RDF, SKOS
 
 from ogc.na import util
 from ogc.na.domain_config import DomainConfiguration, DomainConfigurationEntry
-from ogc.na.profile import ProfileRegistry
 from ogc.na.provenance import generate_provenance, ProvenanceMetadata, FileProvenanceMetadata
 
 logger = logging.getLogger('ogc.na.update_vocabs')
 
 ENTAILED_FORMATS = [
     {'extension': 'ttl', 'format': 'ttl', 'mime': 'text/turtle'},
     {'extension': 'rdf', 'format': 'xml', 'mime': 'application/rdf+xml'},
@@ -328,27 +327,33 @@
 
     parser.add_argument(
         '--auth',
         help="Authentication for uploading data to the triplestore in 'username:password' format. "
              "Alternatively, you can set the DB_USERNAME and DB_PASSWORD env variables."
     )
 
+    parser.add_argument(
+        '--ignore-artifact-errors',
+        action='store_true',
+        help='Ignore errors when retrieving profile artifacts'
+    )
+
     args = parser.parse_args()
 
     setup_logging(args.debug)
 
     graph_store = args.graph_store or os.environ.get('SPARQL_GRAPH_STORE')
 
     if args.update and not graph_store:
         print("ERROR: --update requires a SPARQL Graph Store endpoint", file=sys.stderr)
         sys.exit(-1)
 
     authdetails = None
     if args.auth:
-        authdetails = args.auth.split(':', maxsplit=1)
+        authdetails = tuple(args.auth.split(':', maxsplit=1))
     elif 'DB_USERNAME' in os.environ:
         authdetails = (os.environ["DB_USERNAME"], os.environ.get("DB_PASSWORD", ""))
 
     if graph_store:
         logger.info(f"Using SPARQL graph store %s with{'' if authdetails else 'out'} authentication", graph_store)
 
     mod_list = []
@@ -368,15 +373,17 @@
             add_list = args.added.split(",")
             logger.info("Added: %s", add_list)
 
         if args.removed:
             dellist = args.removed.split(',')
             logger.info("Removed: %s", dellist)
 
-    domain_cfg = DomainConfiguration(args.domain_cfg, working_directory=args.working_directory)
+    domain_cfg = DomainConfiguration(args.domain_cfg, working_directory=args.working_directory,
+                                     profile_sources=args.profile_source,
+                                     ignore_artifact_errors=args.ignore_artifact_errors)
     cfg_entries = domain_cfg.entries
     if not len(cfg_entries):
         if args.domain:
             logger.warning('No configuration found in %s for domain %s, exiting',
                            args.domain_cfg, args.domain)
         else:
             logger.warning('No configuration found in %s exiting', args.domain_cfg)
@@ -482,14 +489,15 @@
                         load_vocab(loadable, versioned_gname,
                                    args.graph_store, authdetails)
                         logging.info("Uploaded %s for %s to SPARQL graph store",
                                      str(path), str(doc))
                     except Exception as e:
                         logging.error("Failed to upload %s for %s: %s",
                                       str(path), str(doc), str(e))
+                        raise e
                     versioned_gname = f'{graphname}{n + 1}'
 
             report.setdefault(cfg.identifier, {}) \
                 .setdefault(report_cat, []).append(os.path.relpath(doc))
 
     for scope, scopereport in report.items():
         logger.info("Scope: %s\n  added: %s\n  modified: %s",
```

### Comparing `ogc_na-0.2.9/ogc/na/util.py` & `ogc_na-0.3.0/ogc/na/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #!/usr/bin/env python3
 """
 General utilities module.
 """
 from __future__ import annotations
 import os.path
 import shlex
-from glob import glob
+from glob import glob, iglob
 from pathlib import Path
 from time import time
 from typing import Optional, Union, Any, Mapping, Hashable
 
 import requests
 import rfc3987
-import git
+
 from rdflib import Graph
 from pyshacl import validate as shacl_validate
 from urllib.parse import urlparse
 
 from ogc.na.validation import ValidationReport
 
 import yaml
 
 try:
     from yaml import CLoader as YamlLoader, CSafeLoader as SafeYamlLoader, CDumper as YamlDumper
 except ImportError:
     from yaml import Loader as YamlLoader, SafeLoader as SafeYamlLoader, Dumper as YamlDumper
 
 
+class ContextMergeError(Exception):
+    pass
+
+
 def copy_triples(src: Graph, dst: Optional[Graph] = None) -> Graph:
     """
     Copies all triples from one graph onto another (or a new, empty [Graph][rdflib.Graph]
     if none is provided).
 
     :param src: the source Graph
     :param dst: the destination Graph (or `None` to create a new one)
@@ -152,28 +156,35 @@
     else:
         if url:
             content = requests.get(url).text
         return yaml.load(content, Loader=SafeYamlLoader if safe else YamlLoader)
 
 
 def dump_yaml(content: Any, filename: str | Path | None = None,
+              ignore_alises=True,
               **kwargs) -> str | None:
     """
     Generates YAML output.
 
     :param content: content to convert to YAML.
     :param filename: optional filename to dump the content into. If None, string content will be returned.
     :param kwargs: other args to pass to `yaml.dump()`
     """
     kwargs.setdefault('sort_keys', False)
+    if ignore_alises:
+        class Dumper(YamlDumper):
+            def ignore_aliases(self, data) -> bool:
+                return True
+    else:
+        Dumper = YamlDumper
     if filename:
         with open(filename, 'w') as f:
-            return yaml.dump(content, f, Dumper=YamlDumper, **kwargs)
+            return yaml.dump(content, f, Dumper=Dumper, **kwargs)
     else:
-        return yaml.dump(content, Dumper=YamlDumper, **kwargs)
+        return yaml.dump(content, Dumper=Dumper, **kwargs)
 
 
 def is_iri(s: str) -> bool:
     try:
         return rfc3987.parse(s, rule='IRI') is not None
     except ValueError:
         return False
@@ -182,16 +193,18 @@
 def merge_dicts(src: dict, dst: dict) -> dict:
     if not src:
         return dst
     for k, v in src.items():
         if isinstance(v, dict):
             node = dst.setdefault(k, {})
             merge_dicts(v, node)
-        else:
+        elif isinstance(dst, dict):
             dst[k] = v
+        else:
+            dst = {k: v}
     return dst
 
 
 def glob_list_split(s: str, exclude_dirs: bool = True, recursive: bool = False) -> list[str]:
     result = []
     for e in shlex.split(s):
         if is_url(s):
@@ -241,14 +254,15 @@
             dest[k] = deep_update(orig_dict.get(k, {}), v, replace)
         else:
             dest[k] = v
     return dest
 
 
 def git_status(repo_path: str | Path = '.'):
+    import git
     repo = git.Repo(repo_path)
     added = repo.untracked_files
     modified = []
     deleted = []
     renamed = []
     for diff in repo.head.commit.diff(None):
         if diff.change_type == 'D':
@@ -259,7 +273,45 @@
             renamed.append((diff.a_path, diff.b_path))
     return {
         'added': added,
         'modified': modified,
         'deleted': deleted,
         'renamed': renamed,
     }
+
+
+def merge_contexts(a: dict, b: dict, from_schema=None, property_chain=None) -> dict[str, Any]:
+    if not b:
+        return a
+    if not a:
+        if isinstance(a, dict):
+            a.update(b)
+            return a
+        return b
+    for term in list(a.keys()):
+        va = a[term]
+        if isinstance(va, str):
+            va = {'@id': va}
+            a[term] = va
+        vb = b.get(term)
+        if isinstance(vb, str):
+            vb = {'@id': vb}
+        if vb:
+            for vb_term, vb_term_val in vb.items():
+                if vb_term != '@context':
+                    va[vb_term] = vb_term_val
+            if '@context' in vb:
+                if '@context' not in va:
+                    va['@context'] = vb['@context']
+                elif isinstance(va['@context'], list):
+                    if isinstance(vb['@context'], list):
+                        va['@context'].extend(vb['@context'])
+                    else:
+                        va['@context'].append(vb['@context'])
+                elif isinstance(vb['@context'], list):
+                    va['@context'] = [va['@context'], *vb['@context']]
+                else:
+                    va['@context'] = merge_contexts(va['@context'], vb['@context'], from_schema, property_chain)
+    for t, tb in b.items():
+        if t not in a:
+            a[t] = tb
+    return a
```

### Comparing `ogc_na-0.2.9/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.3.0/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.2.9
+Version: 0.3.0
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
-Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
+Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
```

### Comparing `ogc_na-0.2.9/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.3.0/ogc_na.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 setup.py
 .github/workflows/python-publish.yml
 docs/examples.md
 docs/gen_ref_pages.py
 docs/index.md
 docs/tutorials.md
 ogc/na/__init__.py
+ogc/na/_version.py
 ogc/na/annotate_schema.py
 ogc/na/domain_config.py
 ogc/na/download.py
+ogc/na/gsp.py
 ogc/na/ingest_json.py
 ogc/na/profile.py
 ogc/na/provenance.py
 ogc/na/update_vocabs.py
 ogc/na/util.py
 ogc/na/validation.py
 ogc/na/input_filters/__init__.py
```

### Comparing `ogc_na-0.2.9/pyproject.toml` & `ogc_na-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,22 +19,23 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/opengeospatial/ogc-na-tools/"
-"Documentation" = "https://opengeospatial.github.com/ogc-na-tools/"
+"Documentation" = "https://opengeospatial.github.io/ogc-na-tools/"
 "Repository" = "https://github.com/opengeospatial/ogc-na-tools.git"
 
 [tool.setuptools]
-include-package-data = true
+include-package-data = false
 
 [tool.setuptools.packages.find]
-include = ["ogc"]
+include = ["ogc*"]
+exclude = ["docs", "test"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools_scm]
 write_to = "ogc/na/_version.py"
```

### Comparing `ogc_na-0.2.9/rdf/domaincfg.vocab.ttl` & `ogc_na-0.3.0/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/test/data/headers.csv` & `ogc_na-0.3.0/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/test/data/uplift_context_valid.yml` & `ogc_na-0.3.0/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/test/test_ingest_json.py` & `ogc_na-0.3.0/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.2.9/test/test_input_filters_csv.py` & `ogc_na-0.3.0/test/test_input_filters_csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,68 +19,68 @@
 
     def test_rows_objects(self):
         cfg = {
             'rows': 'dict',
             'skip-rows': 0,
             'header-row': 0,
         }
-        rows = csv.apply_filter(WITH_HEADERS, cfg)
+        rows = csv.apply_filter(WITH_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 87)
         self.assertEqual(rows[0], {
             'Year': '1968',
             'Score': '86',
             'Title': 'Greetings',
         })
         self.assertEqual(rows[10], {
             'Year': '1977',
             'Score': '67',
             'Title': 'New York,New York',
         })
 
         cfg['skip-rows'] = 3
-        rows = csv.apply_filter(WITH_HEADERS, cfg)
+        rows = csv.apply_filter(WITH_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 84)
         self.assertEqual(rows[0], {
             'Year': '1971',
             'Score': '40',
             'Title': 'Born to Win',
         })
         self.assertEqual(rows[7], {
             'Year': '1977',
             'Score': '67',
             'Title': 'New York,New York',
         })
 
         cfg['skip-rows'] = 0
         cfg['header-row'] = 2
-        rows = csv.apply_filter(WITH_HEADERS, cfg)
+        rows = csv.apply_filter(WITH_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 85)
         self.assertEqual(rows[0], {
             '1970': '1970',
             '17': '73',
             'Bloody Mama': 'Hi,Mom!',
         })
 
     def test_rows_lists(self):
         cfg = {
             'rows': 'list',
             'skip-rows': 0,
         }
-        rows = csv.apply_filter(WITH_HEADERS, cfg)
+        rows = csv.apply_filter(WITH_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 88)
         self.assertEqual(rows[0], ['Year', 'Score', 'Title'])
         self.assertEqual(rows[10], ['1977', '47', '1900'])
         cfg['skip-rows'] = 1
-        rows = csv.apply_filter(WITH_HEADERS, cfg)
+        rows = csv.apply_filter(WITH_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 87)
         self.assertEqual(rows[0], ['1968', '86', "Greetings"])
         self.assertEqual(rows[3], ['1971', '40', "Born to Win"])
         cfg['header-row'] = 2  # should have no effect
-        self.assertEqual(rows, csv.apply_filter(WITH_HEADERS, cfg))
+        self.assertEqual(rows, csv.apply_filter(WITH_HEADERS, cfg)[0])
 
         cfg['skip-rows'] = 0
-        rows = csv.apply_filter(NO_HEADERS, cfg)
+        rows = csv.apply_filter(NO_HEADERS, cfg)[0]
         self.assertEqual(len(rows), 6)
         self.assertEqual(rows[0], ['John', 'Doe', '120 jefferson st.', 'Riverside', ' NJ', ' 08075'])
         cfg['trim-values'] = True
-        rows = csv.apply_filter(NO_HEADERS, cfg)
+        rows = csv.apply_filter(NO_HEADERS, cfg)[0]
         self.assertEqual(rows[0], ['John', 'Doe', '120 jefferson st.', 'Riverside', 'NJ', '08075'])
```

### Comparing `ogc_na-0.2.9/test/test_profile.py` & `ogc_na-0.3.0/test/test_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,14 @@
         registry = ProfileRegistry(empty)
         self.assertFalse(registry.profiles)
 
     def test_build_cyclic_profile_chain(self):
         registry = ProfileRegistry(DATA_DIR / 'profile_tree_cyclic.ttl')
         with self.assertRaises(ValueError):
             registry.build_profile_chain((EX.a, EX.c), recursive=True)
-        with self.assertRaises(ValueError):
-            registry.build_profile_chain((EX.a, EX.c), recursive=False)
         chain = registry.build_profile_chain((EX.a, EX.c), sort=False)
         self.assertEqual(len(chain), 4)
         chain = registry.build_profile_chain((EX.a, EX.c), sort=False, recursive=False)
         self.assertEqual(len(chain), 2)
         chain = registry.build_profile_chain((EX.a, EX.p, EX.q, EX.d), sort=False, recursive=False)
         self.assertEqual(len(chain), 2)
```

