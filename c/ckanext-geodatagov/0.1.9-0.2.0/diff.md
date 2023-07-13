# Comparing `tmp/ckanext-geodatagov-0.1.9.tar.gz` & `tmp/ckanext-geodatagov-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-geodatagov-0.1.9.tar", last modified: Wed Oct  5 20:29:24 2022, max compression
+gzip compressed data, was "ckanext-geodatagov-0.2.0.tar", last modified: Thu Jul 13 19:10:28 2023, max compression
```

## Comparing `ckanext-geodatagov-0.1.9.tar` & `ckanext-geodatagov-0.2.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5922 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.571268 ckanext-geodatagov-0.1.9/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.571268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    42703 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15250 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (121)    10218 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/waf_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/z3950.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19670 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/logic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    24420 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/read.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/organization_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/read.html
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/search.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/snippets/related_collection.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/
--rw-r--r--   0 runner    (1001) docker     (121)     5494 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/geodatagov_source_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection1/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.575268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection2/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-fgdc/
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-gmi/
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.579268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.567268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.583268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    50490 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    27105 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    35634 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10500 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    12185 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.583268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    69938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    17854 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    26698 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    31196 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    31779 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10267 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6691 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
--rw-r--r--   0 runner    (1001) docker     (121)     9878 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7751 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    24168 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9012 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10276 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    10195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
--rw-r--r--   0 runner    (1001) docker     (121)   101010 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    20687 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    22569 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    27195 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    35720 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     7967 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7210 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-05 20:29:24.000000 ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-05 20:29:24.587268 ckanext-geodatagov-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-10-05 20:29:23.000000 ckanext-geodatagov-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24050 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36767 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262469 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/waf_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/z3950.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/organization_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/read.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/snippets/related_collection.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/geodatagov_source_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection1/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection2/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-collection2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-fgdc/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-fgdc/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-gmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-gmi/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-trim-tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf-trim-tags/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.347781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.351781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    50490 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    35634 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.355781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    69938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    31779 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   101010 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    20687 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    22569 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    27195 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    35720 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 19:10:28.000000 ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 19:10:28.359781 ckanext-geodatagov-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 19:10:27.000000 ckanext-geodatagov-0.2.0/setup.py
```

### Comparing `ckanext-geodatagov-0.1.9/LICENSE.md` & `ckanext-geodatagov-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/PKG-INFO` & `ckanext-geodatagov-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,150 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.1.9
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
-Description: [![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
-        [![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
-        
-        # Data.gov  
-        
-        [Data.gov](http://data.gov) is an open data website created by the [U.S. General Services Administration](https://github.com/GSA/) that is based on two robust open source projects: [CKAN](http://ckan.org) and [WordPress](http://wordpress.org). The data catalog at [catalog.data.gov](catalog.data.gov) is powered by CKAN, while the content seen at [Data.gov](Data.gov) is powered by WordPress.  
-                
-        **For all code, bugs, and feature requests related to Data.gov, see the project wide Data.gov [issue tracker](https://github.com/GSA/data.gov/issues).** 
-        
-        Currently this repository is only used for source version control on the code for the CKAN extension for geospatial data, but you can see all of the Data.gov relevant repos listed in the [GSA Data.gov README file](https://github.com/GSA/data.gov/blob/master/README.md). 
-        
-        ## CKAN Extension for Geospatial Data
-        
-        Most Data.gov specific CKAN customizations are contained within this extension, but the extension also provides additional geospatial capabilities.
-        
-        ### Customization
-        
-        Due to CKAN 2.3 and 2.8 migrations, some features should be removed or moved to the official community versions:
-          - [Stop rolling up the extras](https://github.com/GSA/ckanext-geodatagov/issues/178)
-          - [Move to the official search by geolocation](https://github.com/GSA/datagov-deploy/issues/2440) (probably sharing our version that has improvements)
-          - Do a general analysis of this extension to detect other personalized functionalities that should be discontinued.
-        
-        ### Requirements
-        
-        Package                                                                | Notes
-        ---------------------------------------------------------------------- | -------------
-        [ckanext-harvest](https://github.com/ckan/ckanext-harvest/)            | --
-        [ckanext-spatial](https://github.com/ckan/ckanext-spatial)             | --
-        [PyZ3950](https://github.com/asl2/PyZ3950)                             | --
-        [werkzeug](https://github.com/nickumia-reisys/werkzeug)                | This only effects the tests.  For all intents and purposes, this should be tracking [upstream](https://github.com/pallets/werkzeug)
-        
-        This extension is compatible with these versions of CKAN.
-        
-        CKAN version | Compatibility
-        ------------ | -------------
-        <=2.8        | no
-        2.9          | [complete](https://github.com/GSA/datagov-ckan-multi/issues/570)
-        
-        ## Tests
-        
-        All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.9 when you open a pull request.
-        
-        ## Using the Docker Dev Environment
-        
-        ### Build Environment
-        
-        To start environment, run:
-        ```docker-compose build```
-        ```docker-compose up```
-        
-        CKAN will start at localhost:5000
-        
-        To shut down environment, run:
-        
-        ```docker-compose down```
-        
-        To docker exec into the CKAN image, run:
-        
-        ```docker-compose exec app /bin/bash```
-        
-        ### Testing
-        
-        They follow the guidelines for [testing CKAN
-        extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
-        
-        To run the extension tests, start the containers with `make up`, then:
-        
-            $ make test
-        
-        Lint the code.
-        
-            $ make lint
-        
-        ### Debugging
-        
-        We have not determined a good way for most IDE native debugging, however you can use the built in
-        Python pdb debugger. Simply run `make debug`, which will run docker with an interactive shell.
-        Add `import pdb; pdb.set_trace()` anywhere you want to start debugging, and if the code is triggered
-        you should see a command prompt waiting in the shell. Use a pdb cheat sheet when starting to learn
-        like [this](https://kapeli.com/cheat_sheets/Python_Debugger.docset/Contents/Resources/Documents/index).
-        
-        When you edit/add/remove code, the server is smart enough to restart. If you are editing logic that is
-        not part of the webserver (ckan command, etc) then you should be able to run the command after edits
-        and get the same debugger prompt.
-            
-        ### Matrix builds
-        
-        The existing development environment assumes a full catalog.data.gov test setup. This makes
-        it difficult to develop and test against new versions of CKAN (or really any
-        dependency) because everything is tightly coupled and would require us to
-        upgrade everything at once which doesn't really work. A new make target
-        `test-new` is introduced with a new docker-compose file.
-        
-        The "new" development environment drops as many dependencies as possible. It is
-        not meant to have feature parity with
-        [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
-        mock external dependencies where possible.
-        
-        In order to support multiple versions of CKAN, or even upgrade to new versions
-        of CKAN, we support development and testing through the `CKAN_VERSION`
-        environment variable.
-        
-            $ make CKAN_VERSION=2.9 test
-        
-        ## Credit / Copying
-        
-        Original work written by the HealthData.gov team. It has been modified in support of Data.gov.
-        
-        As a work of the United States Government, this package is in the public
-        domain within the United States. Additionally, we waive copyright and
-        related rights in the work worldwide through the CC0 1.0 Universal
-        public domain dedication (which can be found at http://creativecommons.org/publicdomain/zero/1.0/).
-        
-        ## Ways to Contribute
-        We're so glad you're thinking about contributing to ckanext-datajson!
-        
-        Before contributing to ckanext-datajson we encourage you to read our
-        [CONTRIBUTING](CONTRIBUTING.md) guide, our [LICENSE](LICENSE.md), and our README
-        (you are here), all of which should be in this repository. If you have any
-        questions, you can email the Data.gov team at
-        [datagov@gsa.gov](mailto:datagov@gsa.gov).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
+[![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
+
+# Data.gov  
+
+[Data.gov](http://data.gov) is an open data website created by the [U.S. General Services Administration](https://github.com/GSA/) that is based on two robust open source projects: [CKAN](http://ckan.org) and [WordPress](http://wordpress.org). The data catalog at [catalog.data.gov](catalog.data.gov) is powered by CKAN, while the content seen at [Data.gov](Data.gov) is powered by WordPress.  
+        
+**For all code, bugs, and feature requests related to Data.gov, see the project wide Data.gov [issue tracker](https://github.com/GSA/data.gov/issues).** 
+
+Currently this repository is only used for source version control on the code for the CKAN extension for geospatial data, but you can see all of the Data.gov relevant repos listed in the [GSA Data.gov README file](https://github.com/GSA/data.gov/blob/master/README.md). 
+
+## CKAN Extension for Geospatial Data
+
+Most Data.gov specific CKAN customizations are contained within this extension, but the extension also provides additional geospatial capabilities.
+
+### Customization
+
+Due to CKAN 2.3 and 2.8 migrations, some features should be removed or moved to the official community versions:
+  - [Stop rolling up the extras](https://github.com/GSA/ckanext-geodatagov/issues/178)
+  - [Move to the official search by geolocation](https://github.com/GSA/datagov-deploy/issues/2440) (probably sharing our version that has improvements)
+  - Do a general analysis of this extension to detect other personalized functionalities that should be discontinued.
+
+### Requirements
+
+Package                                                                | Notes
+---------------------------------------------------------------------- | -------------
+[ckanext-harvest](https://github.com/ckan/ckanext-harvest/)            | --
+[ckanext-spatial](https://github.com/ckan/ckanext-spatial)             | --
+[PyZ3950](https://github.com/asl2/PyZ3950)                             | --
+[werkzeug](https://github.com/nickumia-reisys/werkzeug)                | This only effects the tests.  For all intents and purposes, this should be tracking [upstream](https://github.com/pallets/werkzeug)
+
+This extension is compatible with these versions of CKAN.
+
+CKAN version | Compatibility
+------------ | -------------
+<=2.8        | no
+2.9          | 0.1.37 (last supported)
+2.10         | >=0.2.0
+
+## Tests
+
+All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.10 when you open a pull request.
+
+## Using the Docker Dev Environment
+
+### Build Environment
+
+To start environment, run:
+```docker-compose build```
+```docker-compose up```
+
+CKAN will start at localhost:5000
+
+To shut down environment, run:
+
+```docker-compose down```
+
+To docker exec into the CKAN image, run:
+
+```docker-compose exec app /bin/bash```
+
+### Testing
+
+They follow the guidelines for [testing CKAN
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
+
+To run the extension tests, start the containers with `make up`, then:
+
+    $ make test
+
+Lint the code.
+
+    $ make lint
+
+### Debugging
+
+We have not determined a good way for most IDE native debugging, however you can use the built in
+Python pdb debugger. Simply run `make debug`, which will run docker with an interactive shell.
+Add `import pdb; pdb.set_trace()` anywhere you want to start debugging, and if the code is triggered
+you should see a command prompt waiting in the shell. Use a pdb cheat sheet when starting to learn
+like [this](https://kapeli.com/cheat_sheets/Python_Debugger.docset/Contents/Resources/Documents/index).
+
+When you edit/add/remove code, the server is smart enough to restart. If you are editing logic that is
+not part of the webserver (ckan command, etc) then you should be able to run the command after edits
+and get the same debugger prompt.
+    
+### Matrix builds
+
+The existing development environment assumes a full catalog.data.gov test setup. This makes
+it difficult to develop and test against new versions of CKAN (or really any
+dependency) because everything is tightly coupled and would require us to
+upgrade everything at once which doesn't really work. A new make target
+`test-new` is introduced with a new docker-compose file.
+
+The "new" development environment drops as many dependencies as possible. It is
+not meant to have feature parity with
+[GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
+mock external dependencies where possible.
+
+In order to support multiple versions of CKAN, or even upgrade to new versions
+of CKAN, we support development and testing through the `CKAN_VERSION`
+environment variable.
+
+    $ make CKAN_VERSION=2.10 test
+
+### Command line interface
+
+The following operations can be run from the command line as described underneath::
+
+      geodatagov sitemap-to-s3 [{upload_to_s3}] [{page_size}] [{max_per_page}]
+        - Generates sitemap and uploads to s3
+
+      geodatagov db-solr-sync [{dryrun}] [{cleanup_solr}] [{update_solr}]
+        - DB Solr sync. 
+
+      geodatagov tracking-update [{start_date}]
+        - ckan tracking update with customized options and output
+
+## Credit / Copying
+
+Original work written by the HealthData.gov team. It has been modified in support of Data.gov.
+
+As a work of the United States Government, this package is in the public
+domain within the United States. Additionally, we waive copyright and
+related rights in the work worldwide through the CC0 1.0 Universal
+public domain dedication (which can be found at http://creativecommons.org/publicdomain/zero/1.0/).
+
+## Ways to Contribute
+We're so glad you're thinking about contributing to ckanext-datajson!
+
+Before contributing to ckanext-datajson we encourage you to read our
+[CONTRIBUTING](CONTRIBUTING.md) guide, our [LICENSE](LICENSE.md), and our README
+(you are here), all of which should be in this repository. If you have any
+questions, you can email the Data.gov team at
+[datagov@gsa.gov](mailto:datagov@gsa.gov).
+
+
```

### Comparing `ckanext-geodatagov-0.1.9/README.md` & `ckanext-geodatagov-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 [werkzeug](https://github.com/nickumia-reisys/werkzeug)                | This only effects the tests.  For all intents and purposes, this should be tracking [upstream](https://github.com/pallets/werkzeug)
 
 This extension is compatible with these versions of CKAN.
 
 CKAN version | Compatibility
 ------------ | -------------
 <=2.8        | no
-2.9          | [complete](https://github.com/GSA/datagov-ckan-multi/issues/570)
+2.9          | 0.1.37 (last supported)
+2.10         | >=0.2.0
 
 ## Tests
 
-All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.9 when you open a pull request.
+All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.10 when you open a pull request.
 
 ## Using the Docker Dev Environment
 
 ### Build Environment
 
 To start environment, run:
 ```docker-compose build```
@@ -57,15 +58,15 @@
 To docker exec into the CKAN image, run:
 
 ```docker-compose exec app /bin/bash```
 
 ### Testing
 
 They follow the guidelines for [testing CKAN
-extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
 
 To run the extension tests, start the containers with `make up`, then:
 
     $ make test
 
 Lint the code.
 
@@ -96,15 +97,28 @@
 [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
 mock external dependencies where possible.
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
-    $ make CKAN_VERSION=2.9 test
+    $ make CKAN_VERSION=2.10 test
+
+### Command line interface
+
+The following operations can be run from the command line as described underneath::
+
+      geodatagov sitemap-to-s3 [{upload_to_s3}] [{page_size}] [{max_per_page}]
+        - Generates sitemap and uploads to s3
+
+      geodatagov db-solr-sync [{dryrun}] [{cleanup_solr}] [{update_solr}]
+        - DB Solr sync. 
+
+      geodatagov tracking-update [{start_date}]
+        - ckan tracking update with customized options and output
 
 ## Credit / Copying
 
 Original work written by the HealthData.gov team. It has been modified in support of Data.gov.
 
 As a work of the United States Government, this package is in the public
 domain within the United States. Additionally, we waive copyright and
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/commands.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 from urllib.request import Request, urlopen
 from urllib.error import URLError, HTTPError
 
 import ckan
 import ckan.model as model
 import ckan.logic as logic
 import ckan.lib.munge as munge
-import ckan.lib.search as search
 from ckan import plugins as p
 from ckan.plugins.toolkit import config
 
 from ckanext.harvest.model import HarvestSource, HarvestJob
-from ckanext.geodatagov.model import MiscsFeed, MiscsTopicCSV
+from ckanext.geodatagov.model import MiscsFeed
 
 
 # https://github.com/GSA/ckanext-geodatagov/issues/117
 log = logging.getLogger('ckanext.geodatagov')
 
 ckan_tmp_path = '/var/tmp/ckan'
 
@@ -96,19 +95,14 @@
             print("Success")
         if cmd == 'clean-deleted':
             self.clean_deleted()
         if cmd == 'combine-feeds':
             self.combine_feeds()
         if cmd == 'harvest-job-cleanup':
             self.harvest_job_cleanup()
-        if cmd == 'harvest-object-relink':
-            harvest_source_id = None
-            if len(self.args) == 2:
-                harvest_source_id = self.args[1]
-            self.harvest_object_relink(harvest_source_id)
         if cmd == 'export-csv':
             self.export_csv()
         # this code is defunct and will need to be refactored into cli.py
         """
         if cmd == "jsonl-export":
             self.jsonl_export()
         if cmd == 'metrics-csv':
@@ -532,87 +526,14 @@
         print('%s combined feeds updated' % datetime.datetime.now())
 
     def harvest_job_cleanup(self):
         if p.toolkit.check_ckan_version(min_version='2.8'):
             print('Task removed since new ckanext-harvest include ckan.harvest.timeout to mark as finished stuck jobs')
             return
 
-    def harvest_object_relink(self, harvest_source_id=None):
-        print('%s: Fix packages which lost harvest objects for harvest source %s.' %
-              (datetime.datetime.now(), harvest_source_id if harvest_source_id else 'all'))
-
-        pkgs_problematic = set()
-        # find packages that has no current harvest object
-        sql = '''
-            WITH package_with_current AS (
-                SELECT package_id FROM harvest_object WHERE current
-            )
-            SELECT distinct(p.id) FROM package p
-            JOIN harvest_object h ON p.id = h.package_id
-            LEFT JOIN package_with_current c ON p.id = c.package_id
-            WHERE p.state='active' AND p.type='dataset' AND c.package_id IS NULL
-        '''
-        if harvest_source_id:
-            sql += '''
-            AND
-                h.harvest_source_id = :harvest_source_id
-            '''
-            results = model.Session.execute(sql,
-                                            {'harvest_source_id': harvest_source_id})
-        else:
-            results = model.Session.execute(sql)
-
-        for row in results:
-            pkgs_problematic.add(row['id'])
-        total = len(pkgs_problematic)
-        print('%s packages to be fixed.' % total)
-
-        # set last complete harvest object to be current
-        sql = '''
-            UPDATE harvest_object
-            SET current = 't'
-            WHERE
-                package_id = :id
-            AND
-                state = 'COMPLETE'
-            AND
-                import_finished = (
-                    SELECT MAX(import_finished)
-                    FROM harvest_object
-                    WHERE
-                        state = 'COMPLETE'
-                    AND
-                        report_status <> 'deleted'
-                    AND
-                        package_id = :id
-                )
-            RETURNING 1
-        '''
-        count = 0
-        for id in pkgs_problematic:
-            result = model.Session.execute(sql, {'id': id}).fetchall()
-            model.Session.commit()
-            count = count + 1
-            if result:
-                print('%s: %s/%s id %s fixed. Now pushing to solr... ' % (datetime.datetime.now(), count, total, id))
-                try:
-                    search.rebuild(id)
-                except KeyboardInterrupt:
-                    print("Stopped.")
-                    return
-                except BaseException:
-                    raise
-                print('Done.')
-            else:
-                print('%s: %s/%s id %s has no valid harvest object. Need to inspect mannully. ' % (
-                    datetime.datetime.now(), count, total, id))
-
-        if not pkgs_problematic:
-            print('%s: All harvest objects look good. Nothing to do. ' % datetime.datetime.now())
-
     @staticmethod
     def export_group_and_tags(packages, domain='https://catalog.data.gov'):
 
         result = []
         for pkg in packages:
             package = dict()
 
@@ -641,112 +562,14 @@
                 if package_categories:
                     package_categories = package_categories.strip('"[],').split('","')
                     package['topicCategories'] = ';'.join(package_categories)
 
                 result.append(package)
         return result
 
-    def export_csv(self, domain='https://catalog.data.gov'):
-        print('export started...')
-
-        # cron job
-        # paster --plugin=ckanext-geodatagov geodatagov export-csv --config=/etc/ckan/production.ini
-
-        # Exported CSV header list:
-        # - Dataset Title
-        # - Dataset URL
-        # - Organization Name
-        # - Organization Link
-        # - Harvest Source Name
-        # - Harvest Source Link
-        # - Topic Name
-        # - Topic Categories
-
-        import io
-        import csv
-
-        limit = 100
-        page = 1
-
-        import pprint
-
-        result = []
-
-        while True:
-            data_dict = {
-                'q': 'groups: *',
-                # 'fq': fq,
-                # 'facet.field': facets.keys(),
-                'rows': limit,
-                # 'sort': sort_by,
-                'start': (page - 1) * limit
-                # 'extras': search_extras
-            }
-
-            query = logic.get_action('package_search')({'model': model, 'ignore_auth': True}, data_dict)
-
-            page += 1
-            # import pprint
-            # pprint.pprint(packages)
-
-            if not query['results']:
-                break
-
-            packages = query['results']
-            result = result + GeoGovCommand.export_group_and_tags(packages=packages, domain=domain)
-
-        if not result:
-            print('nothing to do')
-            return
-
-        import datetime
-
-        print('writing into db...')
-
-        date_suffix = datetime.datetime.strftime(datetime.datetime.now(), '%Y%m%d')
-        csv_output = io.StringIO()
-
-        fieldnames = ['Dataset Title', 'Dataset URL', 'Organization Name', 'Organization Link',
-                      'Harvest Source Name', 'Harvest Source Link', 'Topic Name', 'Topic Categories']
-
-        writer = csv.writer(csv_output)
-        writer.writerow(fieldnames)
-
-        for pkg in result:
-            try:
-                writer.writerow(
-                    [
-                        pkg['title'],
-                        pkg['url'],
-                        pkg['organization'],
-                        pkg['organizationUrl'],
-                        pkg['harvestSourceTitle'],
-                        pkg['harvestSourceUrl'],
-                        pkg['topic'],
-                        pkg['topicCategories']
-                    ]
-                )
-            except UnicodeEncodeError:
-                pprint.pprint(pkg)
-
-        content = csv_output.getvalue()
-
-        entry = model.Session.query(MiscsTopicCSV) \
-            .filter_by(date=date_suffix) \
-            .first()
-        if not entry:
-            # create the empty entry for the first time
-            entry = MiscsTopicCSV()
-            entry.date = date_suffix
-        entry.csv = content
-        entry.save()
-
-        print('csv file topics-%s.csv is ready.' % date_suffix)
-        return result, entry
-
     # this code is defunct and will need to be refactored into cli.py
     """
     def jsonl_export(self):
 
         '''
         cron job
         paster --plugin=ckanext-geodatagov geodatagov jsonl-export --config=/etc/ckan/production.ini
@@ -913,15 +736,15 @@
             On `package_create` or `package_update` this transformation will happend but
             datasets already harvested will not be updated automatically.
             """
 
         # iterate over all datasets
 
         search_backend = config.get('ckanext.spatial.search_backend', 'postgis')
-        if search_backend != 'solr':
+        if search_backend != 'solr-bbox':
             raise ValueError('Solr is not your default search backend (ckanext.spatial.search_backend)')
 
         datasets = model.Session.query(model.Package).all()
         total = len(datasets)
         print('Transforming {} datasets.'.format(total))
         c = 0
         transformed = 0
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/__init__.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/arcgis.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/arcgis.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from ckan.lib.navl.validators import not_empty, ignore_empty
 from ckan.logic.validators import boolean_validator
 from html.parser import HTMLParser
 
 from ckan.plugins.toolkit import add_template_directory, add_resource, requires_ckan_version
 from ckan.plugins import IConfigurer
 
+from ckanext.geodatagov.helpers import string as custom_string
+
 requires_ckan_version("2.9")
 
 
 TYPES = ['Web Map', 'KML', 'Mobile Application',
          'Web Mapping Application', 'WMS', 'Map Service']
 
 
@@ -40,23 +42,24 @@
     Normalizes string, converts to lowercase, removes non-alpha characters,
     and converts spaces to hyphens.
 
     From Django's "django/template/defaultfilters.py".
     """
     if not isinstance(value, str):
         value = str(value)
-    value = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore')
+    value = unicodedata.normalize('NFKD', value)
     value = str(_slugify_strip_re.sub('', value).strip().lower())
     return _slugify_hyphenate_re.sub('-', value)
 
 
 # from http://stackoverflow.com/questions/753052/strip-html-from-strings-in-python
 class MLStripper(HTMLParser):
     def __init__(self):
         self.reset()
+        self.convert_charrefs = True
         self.fed = []
 
     def handle_data(self, d):
         self.fed.append(d)
 
     def get_data(self):
         return ''.join(self.fed)
@@ -113,30 +116,30 @@
             'title': 'ArcGIS REST API',
             'description': 'An ArcGIS REST API endpoint'
         }
 
     def extra_schema(self):
         return {
             'private_datasets': [ignore_empty, boolean_validator],
-            'extra_search_criteria': [ignore_empty, str],
+            'extra_search_criteria': [ignore_empty, custom_string],
         }
 
     def gather_stage(self, harvest_job):
 
         self.harvest_job = harvest_job
-        source_url = harvest_job.source.url
+        source_url = harvest_job.source.url + '/'
         source_config = json.loads(harvest_job.source.config or '{}')
         extra_search_criteria = source_config.get('extra_search_criteria')
 
         num = 100
 
         modified_from = 0
         modified_to = 999999999999999999
 
-        query_template = 'modified:[{modified_from}+TO+{modified_to}]'
+        query_template = 'modified:%5B{modified_from}%20TO%20{modified_to}%5D'
 
         if extra_search_criteria:
             query_template = query_template + ' AND (%s)' % extra_search_criteria
 
         # accountid:0123456789ABCDEF
 
         query = query_template.format(
@@ -150,15 +153,19 @@
 
         while start != -1:
             search_path = 'sharing/search?f=pjson&q={query}&num={num}&start={start}'.format(
                 query=query,
                 num=num,
                 start=start,
             )
-            url = urllib.parse.urljoin(source_url, search_path)
+            try:
+                url = urllib.parse.urljoin(str(source_url), str(search_path))
+            except TypeError as e:
+                self._save_gather_error('Unable to build url (%s, %s): %s' %
+                                        (str(source_url), str(search_path), e), harvest_job)
 
             try:
                 r = requests.get(url)
                 r.raise_for_status()
             except requests.exceptions.RequestException as e:
                 self._save_gather_error('Unable to get content for URL: %s: %r' %
                                         (url, e), harvest_job)
@@ -278,26 +285,26 @@
 
         if status == 'new':
             package_schema = logic.schema.default_create_package_schema()
         else:
             package_schema = logic.schema.default_update_package_schema()
 
         tag_schema = logic.schema.default_tags_schema()
-        tag_schema['name'] = [not_empty, str]
+        tag_schema['name'] = [not_empty, custom_string]
         package_schema['tags'] = tag_schema
         context['schema'] = package_schema  # TODO: user
 
         harvest_object.current = True
         harvest_object.add()
 
         if status == 'new':
             # We need to explicitly provide a package ID, otherwise ckanext-spatial
             # won't be be able to link the extent to the package.
             package_dict['id'] = str(uuid.uuid4())
-            package_schema['id'] = [str]
+            package_schema['id'] = [custom_string]
 
             # Save reference to the package on the object
             harvest_object.package_id = package_dict['id']
             harvest_object.add()
             # Defer constraints and flush so the dataset can be indexed with
             # the harvest object id (on the after_show hook from the harvester
             # plugin)
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/base.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/waf_collection.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/waf_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 
 import ckanext.harvest.queue as queue
 from ckanext.geodatagov.harvesters.base import (
     GeoDataGovWAFHarvester,
 )  # , validate_profiles; , validate_profiles
 from ckanext.harvest.model import HarvestObject
 from ckanext.harvest.model import HarvestObjectExtra as HOExtra
+from ckanext.geodatagov.helpers import string
 
 
 class WAFCollectionHarvester(GeoDataGovWAFHarvester):
     def info(self):
         return {
             "name": "waf-collection",
             "title": "Web Accessible Folder (WAF) Homogeneous Collection",
             "description": "A Web Accessible Folder (WAF) displaying a list"
             "of spatial metadata documents with a collection record",
         }
 
     def extra_schema(self):
         extra_schema = super(WAFCollectionHarvester, self).extra_schema()
-        extra_schema["collection_metadata_url"] = [not_empty, str]
+        extra_schema["collection_metadata_url"] = [not_empty, string]
         log.debug(
             "Getting extra schema for WAFCollectionHarvester: {}".format(extra_schema)
         )
         return extra_schema
 
     def get_package_dict(self, iso_values, harvest_object):
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/harvesters/z3950.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/harvesters/z3950.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from ckanext.geodatagov.harvesters import GeoDataGovHarvester
 
 from ckan.lib.navl.validators import not_empty, convert_int, ignore_empty
 from ckan.logic.validators import boolean_validator
 
 from ckan.plugins.toolkit import add_template_directory, add_resource, requires_ckan_version
+from ckanext.geodatagov.helpers import string
 
 requires_ckan_version("2.9")
 
 
 class Z3950Harvester(GeoDataGovHarvester, SingletonPlugin):
     '''
     A Harvester for z3950.
@@ -39,15 +40,15 @@
             'name': 'z3950',
             'title': 'Z39.50',
             'description': 'A remote database supporting the Z39.50 protocol'
         }
 
     def extra_schema(self):
         return {'private_datasets': [ignore_empty, boolean_validator],
-                'database': [not_empty, str],
+                'database': [not_empty, string],
                 'port': [not_empty, convert_int]}
 
     def gather_stage(self, harvest_job):
 
         log = logging.getLogger(__name__ + '.WAF.gather')
         log.debug('z3950Harvester gather_stage for job: %r', harvest_job)
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/helpers.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,7 +57,11 @@
                 source_config[key] = value[0]
     return source_config
 
 
 def get_collection_package(collection_package_id):
     package = p.toolkit.get_action('package_show')({}, {'id': collection_package_id})
     return package
+
+
+def string(value):
+    return str(value)
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/logic.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/logic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import datetime
 import hashlib
 import logging
 import json
+import re
 import time
 import uuid
 
+from ckan.lib.navl.validators import not_empty
 from ckan.logic import side_effect_free
 import ckan.logic.schema as schema
 from ckan.logic.action import get as core_get
 import ckan.model as model
 import ckan.plugins as p
 from ckanext.geodatagov.plugin import change_resource_details, split_tags
 from ckanext.geodatagov.harvesters.arcgis import _slugify
+from ckanext.geodatagov.helpers import string
 from ckanext.harvest.model import HarvestObject  # , HarvestJob
 
 from ckan.common import config
 
 log = logging.getLogger(__name__)
 
 
@@ -233,15 +236,15 @@
     if not owner_org:
         p.toolkit.get_action('organization_create')(
             context,
             {'name': new_package['owner_org'], 'title': group_name,
              'extras': [{'key': 'organization_type', 'value': "Federal Government"}]})
 
     context['schema'] = schema.default_create_package_schema()
-    context['schema']['id'] = [p.toolkit.get_validator('not_empty')]
+    context['schema']['id'] = [not_empty]
     context['return_id_only'] = True
     return p.toolkit.get_action('package_create')(context, new_package)
 
 
 def datajson_update(context, data_dict):
     new_package = create_data_dict(data_dict)
     model = context['model']
@@ -298,15 +301,15 @@
         guid=uuid.uuid4().hex,
         job=context['harvest_job'],
         content=context['harvestobj'])
     obj.save()
     new_package["extras"].append({"key": "harvest_object_id", "value": obj.id})
 
     context['schema'] = schema.default_create_package_schema()
-    context['schema']['id'] = [p.toolkit.get_validator('not_empty')]
+    context['schema']['id'] = [not_empty]
     context['return_id_only'] = True
     p.toolkit.get_action('package_create')(context, new_package)
     print(str(datetime.datetime.now()) + ' Imported doi id ' + new_package['id'])
 
 
 def doi_update(context, data_dict):
     model = context['model']
@@ -408,15 +411,15 @@
     # update new values
     new_extras_rollup.update(extras_rollup)
 
     # If we use SOLR, try to index (with ckanext-spatial) a valid spatial data
     if p.toolkit.check_ckan_version(min_version='2.8'):
         search_backend = config.get('ckanext.spatial.search_backend', 'postgis')
         log.debug('Search backend {}'.format(search_backend))
-        if search_backend == 'solr':
+        if search_backend == 'solr-bbox':
             old_spatial = new_extras_rollup.get('spatial', None)
             if old_spatial is not None:
                 log.info('Old Spatial found {}'.format(old_spatial))
 
                 # TODO look for more not-found location names
                 if old_spatial in ['National', 'US']:
                     old_spatial = 'United States'
@@ -424,14 +427,18 @@
                 new_spatial = translate_spatial(old_spatial)
                 if new_spatial is not None:
                     log.info('New Spatial transformed {}'.format(new_spatial))
                     # add the real spatial
                     new_extras.append({'key': 'spatial', 'value': new_spatial})
                     # remove rolled spatial to skip run this process again
                     new_extras_rollup['old-spatial'] = new_extras_rollup.pop('spatial')
+                else:
+                    log.info('New spatial could not be created')
+                    new_extras.append({'key': 'spatial', 'value': ''})
+                    new_extras_rollup['old-spatial'] = new_extras_rollup.pop('spatial')
 
     if new_extras_rollup:
         new_extras.append({'key': 'extras_rollup', 'value': json.dumps(new_extras_rollup)})
 
     data_dict['extras'] = new_extras
 
 
@@ -455,39 +462,61 @@
             ]
         } """
 
     geojson_tpl = ('{{"type": "Polygon", '
                    '"coordinates": [[[{minx}, {miny}], [{minx}, {maxy}], '
                    '[{maxx}, {maxy}], [{maxx}, {miny}], [{minx}, {miny}]]]}}')
 
+    # Replace all things that create bad JSON, https://github.com/GSA/data.gov/issues/3549
+    # all instances of '+', '[+23, -1]' is not valid, but '[23, -1]' is valid
+    old_spatial_transformed = old_spatial.replace('+', '')
+    # all trailing decimals, '[34., 2]' is not valid, but '[34.0, 2]' and '[34, 2]' are valid
+    old_spatial_transformed = old_spatial_transformed.replace('.,', ',').replace('.]', ']')
+    # '-98, 29, -83, 35.' is not valid
+    if old_spatial_transformed[-1] == '.':
+        old_spatial_transformed = old_spatial_transformed[0:-1]
+    # all leading 0s, '[-089.63,  30.36]' is not valid, '[-89.63,  30.36]' is valid
+    old_spatial_transformed = re.sub(r'(^|\s)(-?)0+((0|[1-9][0-9]*)(\.[0-9]*)?)', r'\1\2\3', old_spatial_transformed)
+    # if spatial is a space-separated number list, set the new spatial to 'null'
+    try:
+        numbers_with_spaces = [int(i) for i in old_spatial_transformed.split(' ')]
+        if all(isinstance(x, int) for x in numbers_with_spaces):
+            old_spatial_transformed = ''
+    except ValueError:
+        pass
+
+    # If we have 4 numbers separated by commas, transform them as GeoJSON
+    parts = old_spatial_transformed.strip().split(',')
+    if len(parts) == 4 and all(is_number(x) for x in parts):
+        minx, miny, maxx, maxy = parts
+        params = {"minx": minx, "miny": miny, "maxx": maxx, "maxy": maxy}
+        new_spatial = geojson_tpl.format(**params)
+        return new_spatial
+
     # Analyze with type of data is JSON valid
     try:
-        geometry = json.loads(old_spatial)  # NOQA F841
+        geometry = json.loads(old_spatial_transformed)  # NOQA F841
         # If we have 2 lists of 2 numbers, transform them as GeoJSON
         if (isinstance(geometry, list) and len(geometry) == 2):
             min, max = geometry
             params = {"minx": min[0], "miny": min[1], "maxx": max[0], "maxy": max[1]}
             new_spatial = geojson_tpl.format(**params)
             return new_spatial
         else:
             # If we already have a good geometry, use it
-            return old_spatial
+            return old_spatial_transformed
     except BaseException:
-        pass
+        log.info('JSON that could not be parsed\n\t{}'.format(old_spatial_transformed))
 
-    # If we have 4 numbers separated by commas, transform them as GeoJSON
-    parts = old_spatial.strip().split(',')
-    if len(parts) == 4 and all(is_number(x) for x in parts):
-        minx, miny, maxx, maxy = parts
-        params = {"minx": minx, "miny": miny, "maxx": maxx, "maxy": maxy}
-        new_spatial = geojson_tpl.format(**params)
-        return new_spatial
+    try:
+        return get_geo_from_string(old_spatial)
+    except AttributeError:
+        pass
 
-    g = get_geo_from_string(old_spatial)
-    return g
+    return ''
 
 
 def is_number(s):
     try:
         float(s)
         return True
     except ValueError:
@@ -517,14 +546,18 @@
     return up_func(context, data_dict)
 
 
 def package_create(up_func, context, data_dict):
     """ before_package_create for CKAN 2.8 """
     rollup_save_action(context, data_dict)
     data_dict = fix_dataset(data_dict)
+    # TODO: This fix is bad, find a better one :(
+    if 'schema' in context.keys():
+        context['schema']['id'] = [string]
+        context['schema']['tags']['name'] = [not_empty, string]
     return up_func(context, data_dict)
 
 
 def fix_dataset(data_dict):
     """ final changes before create or update a dataset """
     # stop using tags as extras
     # CKAN don't allow extras with the same name as fields
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/plugin.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -401,72 +401,25 @@
     # IConfigurer
     def update_config(self, config):
         p.toolkit.add_template_directory(config, 'templates')
         p.toolkit.add_resource('fanstatic_library', 'geodatagov')
 
     edit_url = None
 
-    UPDATE_CATEGORY_ACTIONS = ['package_update', 'dataset_update']
-    ROLLUP_SAVE_ACTIONS = ['package_create', 'dataset_create', 'package_update', 'dataset_update']
-
-    # source ignored as queried diretly
-    EXTRAS_ROLLUP_KEY_IGNORE = ["metadata-source", "tags", "extras_rollup"]
-
-    def before_action(self, action_name, context, data_dict):
-        """ before_action is a hook in CKAN 2.3 for ALL actions
-            This not exists at CKAN 2.8 and chained action do not exists at CKAN 2.3 """
-        log.info('before_action CKAN {} {} {} {}'.format(ckan_version, action_name, context, data_dict))
-        if action_name in self.UPDATE_CATEGORY_ACTIONS:
-            pkg_dict = p.toolkit.get_action('package_show')(context, {'id': data_dict['id']})
-            if 'groups' not in data_dict:
-                data_dict['groups'] = pkg_dict.get('groups', [])
-            cats = {}
-            for extra in pkg_dict.get('extras', []):
-                if extra['key'].startswith('__category_tag_'):
-                    cats[extra['key']] = extra['value']
-            extras = data_dict.get('extras', [])
-            for item in extras:
-                if item['key'] in cats:
-                    del cats[item['key']]
-            for cat in cats:
-                extras.append({'key': cat, 'value': cats[cat]})
-
-        # make sure rollup happens after any other actions
-        if action_name in self.ROLLUP_SAVE_ACTIONS:
-            extras_rollup = {}
-            new_extras = []
-            for extra in data_dict.get('extras', []):
-                if extra['key'] in self.EXTRAS_ROLLUP_KEY_IGNORE:
-                    new_extras.append(extra)
-                else:
-                    extras_rollup[extra['key']] = extra['value']
-            if extras_rollup:
-                found_extras_rollup = False
-                for new_extra in new_extras:
-                    if new_extra['key'] == "extras_rollup":
-                        # Update extras_rollup
-                        new_extra['value'] = json.dumps(extras_rollup)
-                        found_extras_rollup = True
-                if not found_extras_rollup:
-                    # Insert extras_rollup if not found
-                    new_extras.append({'key': 'extras_rollup',
-                                       'value': json.dumps(extras_rollup)})
-            data_dict['extras'] = new_extras
-
     def configure(self, config):
         log.info('plugin initialized: %s', self.__class__.__name__)
         self.__class__.edit_url = config.get('saml2.user_edit')
 
     @classmethod
     def saml2_user_edit_url(cls):
         return cls.edit_url
 
     # IPackageController
 
-    def before_view(self, pkg_dict):
+    def before_dataset_view(self, pkg_dict):
 
         for num, extra in enumerate(pkg_dict.get('extras', [])):
             if extra['key'] == 'tags':
                 tags = pkg_dict.get('tags', [])
                 tags.extend([dict(name=tag, display_name=tag) for tag
                              in split_tags(extra['value'])])
                 pkg_dict['tags'] = tags
@@ -483,15 +436,15 @@
                 key='terms_of_use', state='active',
                 group_id=organization['id']).first()
             if result:
                 organization['terms_of_use'] = result[0]
 
         return pkg_dict
 
-    def before_index(self, pkg_dict):
+    def before_dataset_index(self, pkg_dict):
 
         tags = pkg_dict.get('tags', [])
         tags.extend(tag for tag in split_tags(pkg_dict.get('extras_tags', '')))
         pkg_dict['tags'] = tags
 
         org_name = pkg_dict['organization']
         group = model.Group.get(org_name)
@@ -518,15 +471,15 @@
                         cats['vocab_category_all'] = new_list
                     except ValueError:
                         pass
         pkg_dict.update(cats)
 
         return pkg_dict
 
-    def before_search(self, search_params):
+    def before_dataset_search(self, search_params):
 
         fq = search_params.get('fq', '')
 
         if search_params.get('sort') in (None, 'rank'):
             search_params['sort'] = 'views_recent desc'
 
         if search_params.get('sort') in ('none'):
@@ -545,15 +498,15 @@
             fq += ' -collection_package_id:["" TO *]'
         else:
             log.info('NOT Added FQ to collection_package_id')
 
         search_params['fq'] = fq
         return search_params
 
-    def after_show(self, context, data_dict):
+    def after_dataset_show(self, context, data_dict):
 
         current_extras = data_dict.get('extras', [])
         new_extras = []
         for extra in current_extras:
             if extra['key'] == 'extras_rollup':
                 rolledup_extras = json.loads(extra['value'])
                 for key, value in list(rolledup_extras.items()):
@@ -631,22 +584,29 @@
 
 
 class Miscs(p.SingletonPlugin):
     ''' Places for something that has nowhere to go otherwise.
     '''
     p.implements(p.IConfigurer)
     p.implements(p.IConfigurable)
-    p.implements(p.IRoutes, inherit=True)
     p.implements(p.IBlueprint)
 
     # IConfigurer
     def update_config(self, config):
         p.toolkit.add_template_directory(config, 'templates')
         p.toolkit.add_resource('fanstatic_library', 'geodatagov')
 
     # IConfigurable
     def configure(self, config):
         log.info('plugin initialized: %s', self.__class__.__name__)
         geodatagovmodel.setup()
 
     def get_blueprint(self):
         return blueprint.datapusher
+
+
+class S3Test(p.SingletonPlugin):
+
+    p.implements(p.IClick)
+
+    def get_commands(self) -> list:
+        return cli.get_commands2()
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mycert.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/saml2/pkitestcrt/mykey.pem`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/search.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/organization/snippets/organization_form.html` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/organization/snippets/organization_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/package/read.html` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/package/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/templates/source/geodatagov_source_form.html` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/templates/source/geodatagov_source_form.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends 'source/new_source_form.html' %}
 {% import 'macros/form.html' as form %}
-{% resource 'harvest-extra-field/main' %}
+{% asset 'harvest-extra-field/main' %}
 
 {% block extra_config %}
 
 {% set source_config = h.get_harvest_source_config(data.id) %}
 <fieldset data-module="harvest-extra-form-change" data-module-form-items="{{ h.dump_json(h.harvest_source_extra_fields()) }}">
         {% set database = source_config.get('database') or data.database %}
         {% set port = source_config.get('port') or data.port %}
@@ -15,15 +15,15 @@
         {{ form.input('port', id='field-port', label=_('Port'), placeholder=_('eg. 3452'), value=port, error=errors.port, classes=['control-full', 'control-group']) }}
 
         {{ form.input('collection_metadata_url', id='field-collection_metadata_url', label=_('Collection Metadata Url'), placeholder=_('eg. http://example.com/collection.xml'), value=collection_metadata_url, error=errors.port, classes=['control-full', 'control-group']) }}
         {{ form.input('extra_search_criteria', id='field-extra_search_criteria', label=_('Extra Search Criteria'), placeholder=_('eg. accountid:0123456789ABCDEF'), value=extra_search_criteria, error=errors.extra_search_criteria, classes=['control-full', 'control-group']) }}
 
 {% set validator_profiles = source_config.get('validator_profiles') or data.validator_profiles %}
 {% set validator_schema = source_config.get('validator_schema') or data.validator_schema %}
-  <div data-module="reclinepreview" data-module-site_url="{{ h.dump_json(h.url('/', locale='default', qualified=true)) }}">
+  <div data-module="reclinepreview" data-module-site_url="{{ g.site_url }}">
          <div class="harvest-types form-group control-group">
            <label class="control-label">Validation</label>
            <div class="controls">
              {% for key, value in h.get_validation_profiles() %}
                {% set checked = key == (validator_profiles or '') %}
                <label class="radio">
                  <input type="radio" name="validator_profiles" value="{{ key }}" {{ "checked " if checked }}>
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/tests/data-samples/waf1/index.html` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/tests/data-samples/waf1/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/__init__.py` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.1-1999/fgdc-std-001.1-1999.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-001.2-2001/fgdc-std-001.2-2001.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect06.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect07.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect08.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect09.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-001-1998-sect10.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-instinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-locainfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-plmiinfo.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect01.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect02.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect03.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect04.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002-sect05.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd` & `ckanext-geodatagov-0.2.0/ckanext/geodatagov/validation/xml/fgdc-std-012-2002/fgdc-std-012-2002.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/PKG-INFO` & `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,150 @@
 Metadata-Version: 2.1
 Name: ckanext-geodatagov
-Version: 0.1.9
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: https://github.com/GSA/ckanext-geodatagov
 Author: Data.gov
 Author-email: datagovhelp@gsa.gov
 License: UNKNOWN
-Description: [![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
-        [![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
-        
-        # Data.gov  
-        
-        [Data.gov](http://data.gov) is an open data website created by the [U.S. General Services Administration](https://github.com/GSA/) that is based on two robust open source projects: [CKAN](http://ckan.org) and [WordPress](http://wordpress.org). The data catalog at [catalog.data.gov](catalog.data.gov) is powered by CKAN, while the content seen at [Data.gov](Data.gov) is powered by WordPress.  
-                
-        **For all code, bugs, and feature requests related to Data.gov, see the project wide Data.gov [issue tracker](https://github.com/GSA/data.gov/issues).** 
-        
-        Currently this repository is only used for source version control on the code for the CKAN extension for geospatial data, but you can see all of the Data.gov relevant repos listed in the [GSA Data.gov README file](https://github.com/GSA/data.gov/blob/master/README.md). 
-        
-        ## CKAN Extension for Geospatial Data
-        
-        Most Data.gov specific CKAN customizations are contained within this extension, but the extension also provides additional geospatial capabilities.
-        
-        ### Customization
-        
-        Due to CKAN 2.3 and 2.8 migrations, some features should be removed or moved to the official community versions:
-          - [Stop rolling up the extras](https://github.com/GSA/ckanext-geodatagov/issues/178)
-          - [Move to the official search by geolocation](https://github.com/GSA/datagov-deploy/issues/2440) (probably sharing our version that has improvements)
-          - Do a general analysis of this extension to detect other personalized functionalities that should be discontinued.
-        
-        ### Requirements
-        
-        Package                                                                | Notes
-        ---------------------------------------------------------------------- | -------------
-        [ckanext-harvest](https://github.com/ckan/ckanext-harvest/)            | --
-        [ckanext-spatial](https://github.com/ckan/ckanext-spatial)             | --
-        [PyZ3950](https://github.com/asl2/PyZ3950)                             | --
-        [werkzeug](https://github.com/nickumia-reisys/werkzeug)                | This only effects the tests.  For all intents and purposes, this should be tracking [upstream](https://github.com/pallets/werkzeug)
-        
-        This extension is compatible with these versions of CKAN.
-        
-        CKAN version | Compatibility
-        ------------ | -------------
-        <=2.8        | no
-        2.9          | [complete](https://github.com/GSA/datagov-ckan-multi/issues/570)
-        
-        ## Tests
-        
-        All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.9 when you open a pull request.
-        
-        ## Using the Docker Dev Environment
-        
-        ### Build Environment
-        
-        To start environment, run:
-        ```docker-compose build```
-        ```docker-compose up```
-        
-        CKAN will start at localhost:5000
-        
-        To shut down environment, run:
-        
-        ```docker-compose down```
-        
-        To docker exec into the CKAN image, run:
-        
-        ```docker-compose exec app /bin/bash```
-        
-        ### Testing
-        
-        They follow the guidelines for [testing CKAN
-        extensions](https://docs.ckan.org/en/2.9/extensions/testing-extensions.html#testing-extensions).
-        
-        To run the extension tests, start the containers with `make up`, then:
-        
-            $ make test
-        
-        Lint the code.
-        
-            $ make lint
-        
-        ### Debugging
-        
-        We have not determined a good way for most IDE native debugging, however you can use the built in
-        Python pdb debugger. Simply run `make debug`, which will run docker with an interactive shell.
-        Add `import pdb; pdb.set_trace()` anywhere you want to start debugging, and if the code is triggered
-        you should see a command prompt waiting in the shell. Use a pdb cheat sheet when starting to learn
-        like [this](https://kapeli.com/cheat_sheets/Python_Debugger.docset/Contents/Resources/Documents/index).
-        
-        When you edit/add/remove code, the server is smart enough to restart. If you are editing logic that is
-        not part of the webserver (ckan command, etc) then you should be able to run the command after edits
-        and get the same debugger prompt.
-            
-        ### Matrix builds
-        
-        The existing development environment assumes a full catalog.data.gov test setup. This makes
-        it difficult to develop and test against new versions of CKAN (or really any
-        dependency) because everything is tightly coupled and would require us to
-        upgrade everything at once which doesn't really work. A new make target
-        `test-new` is introduced with a new docker-compose file.
-        
-        The "new" development environment drops as many dependencies as possible. It is
-        not meant to have feature parity with
-        [GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
-        mock external dependencies where possible.
-        
-        In order to support multiple versions of CKAN, or even upgrade to new versions
-        of CKAN, we support development and testing through the `CKAN_VERSION`
-        environment variable.
-        
-            $ make CKAN_VERSION=2.9 test
-        
-        ## Credit / Copying
-        
-        Original work written by the HealthData.gov team. It has been modified in support of Data.gov.
-        
-        As a work of the United States Government, this package is in the public
-        domain within the United States. Additionally, we waive copyright and
-        related rights in the work worldwide through the CC0 1.0 Universal
-        public domain dedication (which can be found at http://creativecommons.org/publicdomain/zero/1.0/).
-        
-        ## Ways to Contribute
-        We're so glad you're thinking about contributing to ckanext-datajson!
-        
-        Before contributing to ckanext-datajson we encourage you to read our
-        [CONTRIBUTING](CONTRIBUTING.md) guide, our [LICENSE](LICENSE.md), and our README
-        (you are here), all of which should be in this repository. If you have any
-        questions, you can email the Data.gov team at
-        [datagov@gsa.gov](mailto:datagov@gsa.gov).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![Github Actions](https://github.com/GSA/ckanext-geodatagov/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-geodatagov/actions)
+[![PyPI version](https://badge.fury.io/py/ckanext-geodatagov.svg)](https://badge.fury.io/py/ckanext-geodatagov)
+
+# Data.gov  
+
+[Data.gov](http://data.gov) is an open data website created by the [U.S. General Services Administration](https://github.com/GSA/) that is based on two robust open source projects: [CKAN](http://ckan.org) and [WordPress](http://wordpress.org). The data catalog at [catalog.data.gov](catalog.data.gov) is powered by CKAN, while the content seen at [Data.gov](Data.gov) is powered by WordPress.  
+        
+**For all code, bugs, and feature requests related to Data.gov, see the project wide Data.gov [issue tracker](https://github.com/GSA/data.gov/issues).** 
+
+Currently this repository is only used for source version control on the code for the CKAN extension for geospatial data, but you can see all of the Data.gov relevant repos listed in the [GSA Data.gov README file](https://github.com/GSA/data.gov/blob/master/README.md). 
+
+## CKAN Extension for Geospatial Data
+
+Most Data.gov specific CKAN customizations are contained within this extension, but the extension also provides additional geospatial capabilities.
+
+### Customization
+
+Due to CKAN 2.3 and 2.8 migrations, some features should be removed or moved to the official community versions:
+  - [Stop rolling up the extras](https://github.com/GSA/ckanext-geodatagov/issues/178)
+  - [Move to the official search by geolocation](https://github.com/GSA/datagov-deploy/issues/2440) (probably sharing our version that has improvements)
+  - Do a general analysis of this extension to detect other personalized functionalities that should be discontinued.
+
+### Requirements
+
+Package                                                                | Notes
+---------------------------------------------------------------------- | -------------
+[ckanext-harvest](https://github.com/ckan/ckanext-harvest/)            | --
+[ckanext-spatial](https://github.com/ckan/ckanext-spatial)             | --
+[PyZ3950](https://github.com/asl2/PyZ3950)                             | --
+[werkzeug](https://github.com/nickumia-reisys/werkzeug)                | This only effects the tests.  For all intents and purposes, this should be tracking [upstream](https://github.com/pallets/werkzeug)
+
+This extension is compatible with these versions of CKAN.
+
+CKAN version | Compatibility
+------------ | -------------
+<=2.8        | no
+2.9          | 0.1.37 (last supported)
+2.10         | >=0.2.0
+
+## Tests
+
+All the tests live in the [/ckanext/geodatagov/tests](/ckanext/geodatagov/tests) folder. [Github actions](https://github.com/GSA/ckanext-geodatagov/blob/main/.github/workflows/test.yml) is configured to run the tests against CKAN 2.10 when you open a pull request.
+
+## Using the Docker Dev Environment
+
+### Build Environment
+
+To start environment, run:
+```docker-compose build```
+```docker-compose up```
+
+CKAN will start at localhost:5000
+
+To shut down environment, run:
+
+```docker-compose down```
+
+To docker exec into the CKAN image, run:
+
+```docker-compose exec app /bin/bash```
+
+### Testing
+
+They follow the guidelines for [testing CKAN
+extensions](https://docs.ckan.org/en/2.10/extensions/testing-extensions.html#testing-extensions).
+
+To run the extension tests, start the containers with `make up`, then:
+
+    $ make test
+
+Lint the code.
+
+    $ make lint
+
+### Debugging
+
+We have not determined a good way for most IDE native debugging, however you can use the built in
+Python pdb debugger. Simply run `make debug`, which will run docker with an interactive shell.
+Add `import pdb; pdb.set_trace()` anywhere you want to start debugging, and if the code is triggered
+you should see a command prompt waiting in the shell. Use a pdb cheat sheet when starting to learn
+like [this](https://kapeli.com/cheat_sheets/Python_Debugger.docset/Contents/Resources/Documents/index).
+
+When you edit/add/remove code, the server is smart enough to restart. If you are editing logic that is
+not part of the webserver (ckan command, etc) then you should be able to run the command after edits
+and get the same debugger prompt.
+    
+### Matrix builds
+
+The existing development environment assumes a full catalog.data.gov test setup. This makes
+it difficult to develop and test against new versions of CKAN (or really any
+dependency) because everything is tightly coupled and would require us to
+upgrade everything at once which doesn't really work. A new make target
+`test-new` is introduced with a new docker-compose file.
+
+The "new" development environment drops as many dependencies as possible. It is
+not meant to have feature parity with
+[GSA/catalog.data.gov](https://github.com/GSA/catalog.data.gov/). Tests should
+mock external dependencies where possible.
+
+In order to support multiple versions of CKAN, or even upgrade to new versions
+of CKAN, we support development and testing through the `CKAN_VERSION`
+environment variable.
+
+    $ make CKAN_VERSION=2.10 test
+
+### Command line interface
+
+The following operations can be run from the command line as described underneath::
+
+      geodatagov sitemap-to-s3 [{upload_to_s3}] [{page_size}] [{max_per_page}]
+        - Generates sitemap and uploads to s3
+
+      geodatagov db-solr-sync [{dryrun}] [{cleanup_solr}] [{update_solr}]
+        - DB Solr sync. 
+
+      geodatagov tracking-update [{start_date}]
+        - ckan tracking update with customized options and output
+
+## Credit / Copying
+
+Original work written by the HealthData.gov team. It has been modified in support of Data.gov.
+
+As a work of the United States Government, this package is in the public
+domain within the United States. Additionally, we waive copyright and
+related rights in the work worldwide through the CC0 1.0 Universal
+public domain dedication (which can be found at http://creativecommons.org/publicdomain/zero/1.0/).
+
+## Ways to Contribute
+We're so glad you're thinking about contributing to ckanext-datajson!
+
+Before contributing to ckanext-datajson we encourage you to read our
+[CONTRIBUTING](CONTRIBUTING.md) guide, our [LICENSE](LICENSE.md), and our README
+(you are here), all of which should be in this repository. If you have any
+questions, you can email the Data.gov team at
+[datagov@gsa.gov](mailto:datagov@gsa.gov).
+
+
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/SOURCES.txt` & `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ckanext/geodatagov/logic.py
 ckanext/geodatagov/model.py
 ckanext/geodatagov/plugin.py
 ckanext/geodatagov/search.py
 ckanext/geodatagov/harvesters/__init__.py
 ckanext/geodatagov/harvesters/arcgis.py
 ckanext/geodatagov/harvesters/base.py
+ckanext/geodatagov/harvesters/fgdcrse2iso19115-2.xslt
 ckanext/geodatagov/harvesters/waf_collection.py
 ckanext/geodatagov/harvesters/z3950.py
 ckanext/geodatagov/saml2/__init__.py
 ckanext/geodatagov/saml2/pkitestcrt/mycert.pem
 ckanext/geodatagov/saml2/pkitestcrt/mykey.pem
 ckanext/geodatagov/templates/organization/read.html
 ckanext/geodatagov/templates/organization/snippets/organization_form.html
```

### Comparing `ckanext-geodatagov-0.1.9/ckanext_geodatagov.egg-info/entry_points.txt` & `ckanext-geodatagov-0.2.0/ckanext_geodatagov.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
         [ckan.plugins]
     # Add plugins here, eg
     geodatagov=ckanext.geodatagov.plugin:Demo
+    s3test=ckanext.geodatagov.plugin:S3Test
     datagov_harvest=ckanext.geodatagov.plugin:DataGovHarvest
 
     geodatagov_csw_harvester=ckanext.geodatagov.harvesters:GeoDataGovCSWHarvester
     geodatagov_waf_harvester=ckanext.geodatagov.harvesters:GeoDataGovWAFHarvester
     geodatagov_doc_harvester=ckanext.geodatagov.harvesters:GeoDataGovDocHarvester
     geodatagov_geoportal_harvester=ckanext.geodatagov.harvesters:GeoDataGovGeoportalHarvester
     waf_harvester_collection=ckanext.geodatagov.harvesters:WAFCollectionHarvester
```

### Comparing `ckanext-geodatagov-0.1.9/requirements.txt` & `ckanext-geodatagov-0.2.0/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 -e git+https://github.com/ckan/ckanext-harvest.git#egg=ckanext_harvest
--e git+https://github.com/GSA/ckanext-spatial.git#egg=ckanext-spatial
+-e git+https://github.com/ckan/ckanext-spatial.git#egg=ckanext-spatial
 -e git+https://github.com/asl2/PyZ3950.git#egg=PyZ3950
--e git+https://github.com/nickumia-reisys/werkzeug@e1f6527604ab30e4b46b5430a5fb97e7a7055cd7#egg=werkzeug
+git+https://github.com/gsa/ckan.git@ckan-210-temp#egg=ckan
 
 # ckanext-harvest dependencies
 ckantoolkit>=0.0.7
 pika>=1.1.0
-pyOpenSSL==22.0.0
+pyOpenSSL>22.10 #pinning to fix error with crypto (https://levelup.gitconnected.com/fix-attributeerror-module-lib-has-no-attribute-openssl-521a35d83769)
 # redis==2.10.6 # included in ckan core
 # requests>=2.11.1 # included in ckan core
 
 # ckanext-spatial
-# GeoAlchemy>=0.6 # Unnecessary
 # ckantoolkit # included as dep of ckanext-harvest
-# GeoAlchemy>=0.6 #unnessary
-GeoAlchemy2==0.5.0 
+GeoAlchemy2==0.5.0
 Shapely>=1.2.13
-pyproj==2.6.1
-OWSLib==0.18.0
+pyproj==3.4.1
+OWSLib==0.28.1
 lxml>=2.3
 argparse
-pyparsing>=2.1.10 
+pyparsing>=2.1.10
 # requests>=1.1.0 # included in ckan-core
+six
+geojson==3.0.1
 
 # PyZ3950
 pyasn1
 # ply #required in setup.py
 
 # other requirments
 boto3
```

### Comparing `ckanext-geodatagov-0.1.9/setup.py` & `ckanext-geodatagov-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ckanext-geodatagov",
-    version="0.1.9",
+    version="0.2.0",
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3'
     ],  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     keywords='',
@@ -24,23 +24,24 @@
     license='',
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
     namespace_packages=['ckanext', 'ckanext.geodatagov'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         # -*- Extra requirements: -*-
-        'ckanext-datajson',
+        'ckanext-datajson>=0.1.19',
         'boto3',
         'ply>=3.4',
     ],
     setup_requires=['wheel'],
     entry_points="""
         [ckan.plugins]
     # Add plugins here, eg
     geodatagov=ckanext.geodatagov.plugin:Demo
+    s3test=ckanext.geodatagov.plugin:S3Test
     datagov_harvest=ckanext.geodatagov.plugin:DataGovHarvest
 
     geodatagov_csw_harvester=ckanext.geodatagov.harvesters:GeoDataGovCSWHarvester
     geodatagov_waf_harvester=ckanext.geodatagov.harvesters:GeoDataGovWAFHarvester
     geodatagov_doc_harvester=ckanext.geodatagov.harvesters:GeoDataGovDocHarvester
     geodatagov_geoportal_harvester=ckanext.geodatagov.harvesters:GeoDataGovGeoportalHarvester
     waf_harvester_collection=ckanext.geodatagov.harvesters:WAFCollectionHarvester
```

