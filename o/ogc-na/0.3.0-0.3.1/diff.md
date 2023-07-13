# Comparing `tmp/ogc_na-0.3.0.tar.gz` & `tmp/ogc_na-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.3.0.tar", last modified: Thu Jul 13 09:39:29 2023, max compression
+gzip compressed data, was "ogc_na-0.3.1.tar", last modified: Thu Jul 13 12:19:21 2023, max compression
```

## Comparing `ogc_na-0.3.0.tar` & `ogc_na-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.793216 ogc_na-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 09:39:19.000000 ogc_na-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-13 09:39:19.000000 ogc_na-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 09:39:19.000000 ogc_na-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 09:39:29.793216 ogc_na-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 09:39:19.000000 ogc_na-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-13 09:39:19.000000 ogc_na-0.3.0/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-13 09:39:19.000000 ogc_na-0.3.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.785216 ogc_na-0.3.0/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc/na/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    32640 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-13 09:39:19.000000 ogc_na-0.3.0/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 09:39:29.000000 ogc_na-0.3.0/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 09:39:19.000000 ogc_na-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 09:39:19.000000 ogc_na-0.3.0/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-13 09:39:19.000000 ogc_na-0.3.0/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 09:39:19.000000 ogc_na-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:39:29.793216 ogc_na-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 09:39:19.000000 ogc_na-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:29.789216 ogc_na-0.3.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 09:39:19.000000 ogc_na-0.3.0/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.975117 ogc_na-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.967117 ogc_na-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 12:19:09.000000 ogc_na-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-13 12:19:09.000000 ogc_na-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 12:19:09.000000 ogc_na-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 12:19:21.975117 ogc_na-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 12:19:09.000000 ogc_na-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-13 12:19:09.000000 ogc_na-0.3.1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-13 12:19:09.000000 ogc_na-0.3.1/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 12:19:09.000000 ogc_na-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-13 12:19:09.000000 ogc_na-0.3.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-13 12:19:09.000000 ogc_na-0.3.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.967117 ogc_na-0.3.1/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc/na/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-13 12:19:09.000000 ogc_na-0.3.1/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 12:19:21.000000 ogc_na-0.3.1/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 12:19:09.000000 ogc_na-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 12:19:09.000000 ogc_na-0.3.1/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-13 12:19:09.000000 ogc_na-0.3.1/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 12:19:09.000000 ogc_na-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:19:21.975117 ogc_na-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 12:19:09.000000 ogc_na-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.971117 ogc_na-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:21.975117 ogc_na-0.3.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 12:19:09.000000 ogc_na-0.3.1/test/test_profile.py
```

### Comparing `ogc_na-0.3.0/.github/workflows/python-publish.yml` & `ogc_na-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/.gitignore` & `ogc_na-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/PKG-INFO` & `ogc_na-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.3.0
+Version: 0.3.1
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.0/README.md` & `ogc_na-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/docs/examples.md` & `ogc_na-0.3.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/docs/gen_ref_pages.py` & `ogc_na-0.3.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/docs/index.md` & `ogc_na-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/docs/tutorials.md` & `ogc_na-0.3.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/mkdocs.yml` & `ogc_na-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/annotate_schema.py` & `ogc_na-0.3.1/ogc/na/annotate_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                 location = from_schema.location.resolve().parent.joinpath(location).resolve()
 
         if location is None:
             raise ValueError(f'Unexpected ref type {type(ref).__name__}')
 
         return location, fragment
 
-    def resolve_schema(self, ref: str | Path, from_schema: ReferencedSchema | None = None) -> ReferencedSchema:
+    def resolve_schema(self, ref: str | Path, from_schema: ReferencedSchema | None = None) -> ReferencedSchema | None:
         chain = from_schema.chain + [from_schema] if from_schema else []
         try:
             schema_source, fragment = self.resolve_ref(ref, from_schema)
             if from_schema:
                 for ancestor in from_schema.chain:
                     if (not schema_source or ancestor.location == schema_source) and ancestor.fragment == fragment:
                         return None
@@ -399,15 +399,15 @@
             term_val = resolved.context[term]
             resolved.context[term] = resolve_prop(term_val, ctx_stack)
 
         return resolved
 
     resolved_inner = resolve_inner(ctx)
     if not resolved_inner:
-        return None
+        return ResolvedContext()
     for p, puri in resolved_inner.prefixes.items():
         if p not in prefixes:
             prefixes[p] = puri
 
     return ResolvedContext(context=resolved_inner.context, prefixes=prefixes)
 
 
@@ -422,30 +422,28 @@
 
     The results will be stored in the `schemas` property (a dictionary of
     schema-path-or-url -> AnnotatedSchema mappings).
     """
 
     def __init__(self, ref_mapper: Callable[[str, Any], str] | None = None):
         """
-        :param fn: file path to load (root schema)
-        :param url: URL to load (root schema)
-        :follow_refs: whether to follow `$ref`s (otherwise just annotate the provided root schema)
+        :ref_mapper: an optional function to map JSON `$ref`'s before resolving them
         """
         self._schema_resolver = SchemaResolver()
         self._ref_mapper = ref_mapper
 
     def process_schema(self, location: Path | str | None,
                        default_context: str | Path | dict | None = None) -> AnnotatedSchema | None:
         resolved_schema = self._schema_resolver.resolve_schema(location)
         schema = resolved_schema.subschema
 
         try:
             if '$schema' in schema and all(x not in schema for x in ('schema', 'openapi')):
                 validate_schema(schema)
-        except jsonschema.exceptions.SchemaError as e:
+        except jsonschema.exceptions.SchemaError:
             return None
 
         context_fn = schema.get(ANNOTATION_CONTEXT)
         schema.pop(ANNOTATION_CONTEXT, None)
 
         context = {}
         prefixes = {}
@@ -473,18 +471,21 @@
                     if isinstance(prop_ctx, str):
                         return {'@id': prop_ctx}
                     elif '@id' not in prop_ctx and not vocab:
                         raise ValueError(f'Missing @id for property {prop} in context {json.dumps(ctx, indent=2)}')
                     else:
                         result = {k: v for k, v in prop_ctx.items() if k.startswith('@')}
                         result['@id'] = f"{vocab}{prop}"
+                        return result
                 elif '@vocab' in ctx:
                     return {'@id': f"{ctx['@vocab']}{prop}"}
 
-        def process_properties(obj: dict, context_stack: list[dict[str, Any]], level) -> Iterable[str]:
+        def process_properties(obj: dict, context_stack: list[dict[str, Any]],
+                               from_schema: ReferencedSchema, level) -> Iterable[str]:
+
             properties: dict[str, dict] = obj.get('properties') if obj else None
             if not properties:
                 return ()
             if not isinstance(properties, dict):
                 raise ValueError('"properties" must be a dictionary')
 
             used_terms = set()
@@ -503,69 +504,71 @@
                         for k, v in prop_schema_ctx.items():
                             prop_value.setdefault(k, v)
 
                 if prop_ctx and '@context' in prop_ctx:
                     prop_context_stack = context_stack + [prop_ctx['@context']]
                 else:
                     prop_context_stack = context_stack
-                used_terms.update(process_subschema(prop_value, prop_context_stack, level))
+                used_terms.update(process_subschema(prop_value, prop_context_stack, from_schema, level))
 
             return used_terms
 
-        def process_subschema(subschema, context_stack, level=1) -> Iterable[str]:
+        def process_subschema(subschema, context_stack, from_schema: ReferencedSchema, level=1) -> Iterable[str]:
             if not subschema or not isinstance(subschema, dict):
                 return ()
 
-            if self._ref_mapper and '$ref' in subschema:
-                subschema['$ref'] = self._ref_mapper(subschema['$ref'], subschema)
-
             used_terms = set()
 
+            if '$ref' in subschema:
+                if self._ref_mapper:
+                    subschema['$ref'] = self._ref_mapper(subschema['$ref'], subschema)
+                if subschema['$ref'].startswith('#/') or subschema['$ref'].startswith(f"{from_schema.location}#/"):
+                    target_schema = self._schema_resolver.resolve_schema(subschema['$ref'], from_schema)
+                    if target_schema:
+                        used_terms.update(process_subschema(target_schema.subschema, context_stack, target_schema, level + 1))
+
             # Annotate oneOf, allOf, anyOf
             for p in ('oneOf', 'allOf', 'anyOf'):
                 collection = subschema.get(p)
                 if collection and isinstance(collection, list):
                     for entry in collection:
-                        used_terms.update(process_subschema(entry, context_stack, level + 1))
+                        used_terms.update(process_subschema(entry, context_stack, from_schema, level + 1))
 
             # Annotate main schema
             schema_type = subschema.get('type')
             if not schema_type and 'properties' in subschema:
                 schema_type = 'object'
 
             if schema_type == 'object':
-                used_terms.update(process_properties(subschema, context_stack, level + 1))
+                used_terms.update(process_properties(subschema, context_stack, from_schema, level + 1))
             elif schema_type == 'array':
                 for k in ('prefixItems', 'items', 'contains'):
-                    used_terms.update(process_subschema(subschema.get(k), context_stack, level + 1))
-
-            # Annotate $defs
-            for defs_prop in ('$defs', 'definitions'):
-                defs_value = subschema.get(defs_prop)
-                if isinstance(defs_value, dict):
-                    for defs_entry in defs_value.values():
-                        used_terms.update(process_subschema(defs_entry, context_stack))
+                    used_terms.update(process_subschema(subschema.get(k), context_stack, from_schema, level + 1))
 
             # Get prefixes
             for p, bu in subschema.get(ANNOTATION_PREFIXES, {}).items():
                 if p not in prefixes:
                     prefixes[p] = bu
 
             if len(context_stack) == level and context_stack[-1]:
-                extra_terms = {k: (v if isinstance(v, str)
-                                   else {f"{ANNOTATION_PREFIX}{vk[1:]}": vv for vk, vv in v.items() if vk[0] == '@'})
-                               for k, v in context_stack[-1].items() if k[0] != '@'
-                               and k not in prefixes
-                               and k not in used_terms }
+                extra_terms = {}
+                for k, v in context_stack[-1].items():
+                    if k[0] != '@' and k not in prefixes and k not in used_terms:
+                        if isinstance(v, dict):
+                            if len(v) == 1 and '@id' in v:
+                                v = v['@id']
+                            else:
+                                v = {f"{ANNOTATION_PREFIX}{vk[1:]}": vv for vk, vv in v.items() if vk[0] == '@'}
+                        extra_terms[k] = v
                 if extra_terms:
                     subschema.setdefault(ANNOTATION_EXTRA_TERMS, {}).update(extra_terms)
 
             return used_terms
 
-        process_subschema(schema, [context])
+        process_subschema(schema, [context], resolved_schema)
 
         if prefixes:
             schema[ANNOTATION_PREFIXES] = prefixes
 
         return AnnotatedSchema(
             source=location,
             is_json=resolved_schema.is_json,
@@ -577,16 +580,17 @@
     """
     Builds a JSON-LD context from a set of annotated JSON schemas.
     """
 
     def __init__(self, location: Path | str = None,
                  compact: bool = True, ref_mapper: Callable[[str], str] | None = None):
         """
-        :param fn: file to load the annotated schema from
-        :param url: URL to load the annotated schema from
+        :param location: file or URL load the annotated schema from
+        :param compact: whether to compact the resulting context (remove redundancies, compact CURIEs)
+        :ref_mapper: an optional function to map JSON `$ref`'s before resolving them
         """
         self.context = {'@context': {}}
         self._parsed_schemas: dict[str | Path, dict] = {}
         self._ref_mapper = ref_mapper
 
         self._resolver = SchemaResolver()
 
@@ -631,15 +635,15 @@
                 if isinstance(prop_context.get('@id'), str):
                     subschema_context[prop] = prop_context
                 elif inner_context:
                     subschema_context = merge_contexts(subschema_context, inner_context, from_schema, property_chain)
 
             return subschema_context
 
-        def process_subschema(subschema, from_schema, property_chain=None, ref_chain=None) -> dict | None:
+        def process_subschema(subschema, from_schema, property_chain=None) -> dict | None:
 
             if property_chain is None:
                 property_chain = []
 
             if not isinstance(subschema, dict):
                 return None
 
@@ -674,15 +678,15 @@
                     sub_context = merge_contexts(sub_context, items_ctx, from_schema, property_chain)
 
             if ANNOTATION_EXTRA_TERMS in subschema:
                 for extra_term, extra_term_context in subschema[ANNOTATION_EXTRA_TERMS].items():
                     if extra_term not in sub_context:
                         if isinstance(extra_term_context, str):
                             extra_term_context = {'@id': extra_term_context}
-                        else:
+                        elif isinstance(extra_term_context, dict):
                             extra_term_context = {f"@{k[len(ANNOTATION_PREFIX):]}": v for k, v in extra_term_context.items()}
                         sub_context[extra_term] = extra_term_context
 
             if sub_context:
                 fixed_sub_context = {}
                 for prop, prop_ctx in sub_context.items():
                     if prop.startswith('@'):
@@ -698,63 +702,70 @@
                 prefixes.update(sub_prefixes)
 
             return sub_context
 
         own_context = merge_contexts(own_context, process_subschema(root_schema.subschema, root_schema),
                                      root_schema)
 
-        if compact:
+        for prefix in list(prefixes.keys()):
+            if prefix not in own_context:
+                own_context[prefix] = {'@id': prefixes[prefix]}
+            else:
+                del prefixes[prefix]
 
-            rev_prefixes = {v: k for k, v in prefixes.items()}
+        if compact:
 
             def compact_uri(uri: str) -> str:
                 if uri.startswith('@'):
                     # JSON-LD keyword
                     return uri
-                parts = urlparse(uri)
-                if parts.fragment:
-                    pref, suf = uri.rsplit('#', 1)
-                    pref += '#'
-                elif len(parts.path) > 1:
-                    pref, suf = uri.rsplit('/', 1)
-                    pref += '/'
-                else:
-                    return uri
 
-                if pref in rev_prefixes:
-                    return f"{rev_prefixes[pref]}:{suf}"
-                else:
-                    return uri
+                for pref, pref_uri in prefixes.items():
+                    if uri.startswith(pref_uri) and len(pref_uri) < len(uri):
+                        local_part = uri[len(pref_uri):]
+                        if local_part.startswith('//'):
+                            return uri
+                        return f"{pref}:{local_part}"
+
+                return uri
 
-            def compact_branch(branch, context_stack=None):
+            def compact_branch(branch, context_stack=None) -> bool:
                 child_context_stack = context_stack + [branch] if context_stack else [branch]
                 terms = list(k for k in branch.keys() if k[0] != '@')
 
+                changed = False
                 for term in terms:
                     term_value = branch[term]
                     deleted = False
                     if context_stack:
                         for ctx in context_stack:
                             if term in ctx and ctx[term] == term_value:
                                 del branch[term]
                                 deleted = True
+                                changed = True
                                 break
                     if not deleted and isinstance(term_value, dict) and '@context' in term_value:
-                        compact_branch(term_value['@context'], child_context_stack)
+                        while True:
+                            if not compact_branch(term_value['@context'], child_context_stack):
+                                break
+
+                return changed
 
             def compact_uris(branch, context_stack=None):
                 child_context_stack = context_stack + [branch] if context_stack else [branch]
                 terms = list(k for k in branch.keys() if k[0] != '@')
                 for term in terms:
                     term_value = branch.get(term)
                     if isinstance(term_value, str):
                         branch[term] = compact_uri(term_value)
                     elif isinstance(term_value, dict):
+                        if '@id' in term_value:
+                            term_value['@id'] = compact_uri(term_value['@id'])
                         if len(term_value) == 1 and '@id' in term_value:
-                            branch[term] = compact_uri(term_value['@id'])
+                            branch[term] = term_value['@id']
                         elif '@context' in term_value:
                             compact_uris(term_value['@context'], child_context_stack)
 
             compact_branch(own_context)
             compact_uris(own_context)
 
         self._parsed_schemas[schema_location] = own_context
@@ -764,15 +775,15 @@
 def dump_annotated_schema(schema: AnnotatedSchema, subdir: Path | str = 'annotated',
                            root_dir: Path | str | None = None,
                            output_fn_transform: Callable[[Path], Path] | None = None) -> None:
     """
     Creates a "mirror" directory (named `annotated` by default) with the resulting
     schemas annotated by a `SchemaAnnotator`.
 
-    :param annotator: a `SchemaAnnotator` with the annotated schemas to read
+    :param schema: the `AnnotatedSchema` to dump
     :param subdir: a name for the mirror directory
     :param root_dir: root directory for computing relative paths to schemas
     :param output_fn_transform: optional callable to transform the output path
     """
     wd = (Path(root_dir) if root_dir else Path()).resolve()
     subdir = subdir if isinstance(subdir, Path) else Path(subdir)
     path = schema.source
```

### Comparing `ogc_na-0.3.0/ogc/na/domain_config.py` & `ogc_na-0.3.1/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/download.py` & `ogc_na-0.3.1/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/gsp.py` & `ogc_na-0.3.1/ogc/na/gsp.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/ingest_json.py` & `ogc_na-0.3.1/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/input_filters/__init__.py` & `ogc_na-0.3.1/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/input_filters/csv.py` & `ogc_na-0.3.1/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/profile.py` & `ogc_na-0.3.1/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/provenance.py` & `ogc_na-0.3.1/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/update_vocabs.py` & `ogc_na-0.3.1/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/util.py` & `ogc_na-0.3.1/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc/na/validation.py` & `ogc_na-0.3.1/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.3.1/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.3.0
+Version: 0.3.1
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.0/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.3.1/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/pyproject.toml` & `ogc_na-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/rdf/domaincfg.vocab.ttl` & `ogc_na-0.3.1/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/data/headers.csv` & `ogc_na-0.3.1/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/data/uplift_context_valid.yml` & `ogc_na-0.3.1/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/test_annotate_schema.py` & `ogc_na-0.3.1/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/test_ingest_json.py` & `ogc_na-0.3.1/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/test_input_filters_csv.py` & `ogc_na-0.3.1/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.0/test/test_profile.py` & `ogc_na-0.3.1/test/test_profile.py`

 * *Files identical despite different names*

