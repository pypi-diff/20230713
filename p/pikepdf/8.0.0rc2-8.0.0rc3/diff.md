# Comparing `tmp/pikepdf-8.0.0rc2.tar.gz` & `tmp/pikepdf-8.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-8.0.0rc2.tar", last modified: Fri Jul  7 09:57:15 2023, max compression
+gzip compressed data, was "pikepdf-8.0.0rc3.tar", last modified: Tue Jul 11 21:13:12 2023, max compression
```

## Comparing `pikepdf-8.0.0rc2.tar` & `pikepdf-8.0.0rc3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.832679 pikepdf-8.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-07 09:57:15.828679 pikepdf-8.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6030 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 09:57:15.832679 pikepdf-8.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.808679 pikepdf-8.0.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.816679 pikepdf-8.0.0rc2/src/core/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/gsl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42088 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14258 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.820679 pikepdf-8.0.0rc2/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.824679 pikepdf-8.0.0rc2/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    32038 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.820679 pikepdf-8.0.0rc2/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-07 09:57:15.000000 pikepdf-8.0.0rc2/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:57:15.828679 pikepdf-8.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    36923 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-07 09:53:24.000000 pikepdf-8.0.0rc2/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.594720 pikepdf-8.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-11 21:13:12.594720 pikepdf-8.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6030 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5892 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 21:13:12.594720 pikepdf-8.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3856 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.578719 pikepdf-8.0.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.586719 pikepdf-8.0.0rc3/src/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1187 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5492 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42071 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10569 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14256 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.586719 pikepdf-8.0.0rc3/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.590720 pikepdf-8.0.0rc3/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36349 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32038 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15420 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.586719 pikepdf-8.0.0rc3/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-07-11 21:13:12.000000 pikepdf-8.0.0rc3/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-11 21:13:12.000000 pikepdf-8.0.0rc3/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 21:13:12.000000 pikepdf-8.0.0rc3/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-07-11 21:13:12.000000 pikepdf-8.0.0rc3/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-11 21:13:12.000000 pikepdf-8.0.0rc3/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 21:13:12.594720 pikepdf-8.0.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36923 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-07-11 21:10:00.000000 pikepdf-8.0.0rc3/tests/test_sanity.py
```

### Comparing `pikepdf-8.0.0rc2/LICENSE.txt` & `pikepdf-8.0.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/PKG-INFO` & `pikepdf-8.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.0.0rc2/README.md` & `pikepdf-8.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/pyproject.toml` & `pikepdf-8.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "wheel >= 0.37",
   "pybind11 >= 2.10.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pikepdf"
-version = "8.0.0rc2"
+version = "8.0.0rc3"
 description = "Read and write PDFs with Python, powered by qpdf"
 readme = "README.md"
 requires-python = ">= 3.8"
 keywords = ["PDF"]
 authors = [
   { name = "James R. Barlow", email= "james@purplerock.ca"}
 ]
@@ -115,18 +115,19 @@
 '''
 
 [tool.cibuildwheel]
 test-command = "pytest -nauto {project}/tests"
 test-extras = "test"
 # cp36: ancient
 # pp37: discontinued by Pillow - https://pypi.org/project/Pillow/#files
+# pp310: no Pillow wheels yet
 # Reminder:
 #   build.yml sets CIBW_BUILD to select what can be built
 #   this file sets skip to deselect what cannot be built
-skip = ["cp36-*", "cp37-*", "pp37-*", "*-win32", "*musllinux*", "pp*-manylinux*_aarch64"]
+skip = ["cp36-*", "cp37-*", "pp37-*", "pp310-*", "*-win32", "*musllinux*", "pp*-manylinux*_aarch64"]
 test-skip = "*_universal2:arm64"
 
 [tool.cibuildwheel.environment]
 QPDF_MIN_VERSION = "11.4.0"
 QPDF_VERSION = "11.4.0"
 QPDF_PATTERN = "https://github.com/qpdf/qpdf/releases/download/vVERSION/qpdf-VERSION.tar.gz"
```

### Comparing `pikepdf-8.0.0rc2/setup.py` & `pikepdf-8.0.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/annotation.cpp` & `pikepdf-8.0.0rc3/src/core/annotation.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/embeddedfiles.cpp` & `pikepdf-8.0.0rc3/src/core/embeddedfiles.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/gsl.h` & `pikepdf-8.0.0rc3/src/core/gsl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/jbig2-inl.h` & `pikepdf-8.0.0rc3/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/job.cpp` & `pikepdf-8.0.0rc3/src/core/job.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -116,16 +116,17 @@
             &QPDFJob::hasWarnings,
             "After run(), returns True if there were warnings.")
         .def_property_readonly("exit_code",
             &QPDFJob::getExitCode,
             R"~~~(
             After run(), returns an integer exit code.
 
-            Some exit codes have integer value. Their applicably is determined by
-            context of the job being run.
+            The meaning of exit code depends on the details of the Job that was run.
+            Details are subject to change in libqpdf. Use properties ``has_warnings``
+            and ``encryption_status`` instead.
             )~~~")
         .def_property_readonly(
             "encryption_status",
             [](QPDFJob &job) {
                 uint bits = job.getEncryptionStatus();
                 py::dict result;
                 result["encrypted"]          = bool(bits & qpdf_es_encrypted);
```

### Comparing `pikepdf-8.0.0rc2/src/core/logger.cpp` & `pikepdf-8.0.0rc3/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/mmap_inputsource-inl.h` & `pikepdf-8.0.0rc3/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/nametree.cpp` & `pikepdf-8.0.0rc3/src/core/nametree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/numbertree.cpp` & `pikepdf-8.0.0rc3/src/core/numbertree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/object.cpp` & `pikepdf-8.0.0rc3/src/core/object.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     Real <- float
     Null <-> None
 
 PDF semantics dictate that setting a dictionary key to Null deletes the key.
 
     d['/Key'] = None  # would delete /Key
 
-For Python users appears to have an unexpected side effect, so this action is
-prohibited. You cannot set keys to None.
+For Python users this would be unexpected, so this action is prohibited.
+You cannot set keys to None.
 
 pikepdf.String is a "type" that can be converted with str() or bytes() as
 needed.
 
 */
 
 py::size_t list_range_check(QPDFObjectHandle h, int index)
```

### Comparing `pikepdf-8.0.0rc2/src/core/object_convert.cpp` & `pikepdf-8.0.0rc3/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/object_repr.cpp` & `pikepdf-8.0.0rc3/src/core/object_repr.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/page.cpp` & `pikepdf-8.0.0rc3/src/core/page.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "externalize_inline_images",
             [](QPDFPageObjectHelper &poh, size_t min_size = 0, bool shallow = false) {
                 return poh.externalizeInlineImages(min_size, shallow);
             },
             py::arg("min_size") = 0,
             py::arg("shallow")  = false,
             R"~~~(
-                Convert inlines image to normal (external) images.
+                Convert inline image to normal (external) images.
 
                 Args:
                     min_size (int): minimum size in bytes
                     shallow (bool): If False, recurse into nested Form XObjects.
                         If True, do not recurse.
             )~~~")
         .def("rotate",
@@ -129,15 +129,15 @@
 
                 A page's resources dictionary maps names to objects elsewhere
                 in the file. This method walks through a page's contents and
                 keeps tracks of which resources are referenced somewhere in the
                 contents. Then it removes from the resources dictionary any
                 object that is not referenced in the contents. This
                 method is used by page splitting code to avoid copying unused
-                objects in files that used shared resource dictionaries across
+                objects in files that use shared resource dictionaries across
                 multiple pages.
             )~~~")
         .def("as_form_xobject",
             &QPDFPageObjectHelper::getFormXObjectForPage, // LCOV_EXCL_LINE
             py::arg("handle_transformations") = true,
             R"~~~(
                 Return a form XObject that draws this page.
```

### Comparing `pikepdf-8.0.0rc2/src/core/parsers.cpp` & `pikepdf-8.0.0rc3/src/core/parsers.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/parsers.h` & `pikepdf-8.0.0rc3/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/pikepdf.cpp` & `pikepdf-8.0.0rc3/src/core/pikepdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/pikepdf.h` & `pikepdf-8.0.0rc3/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/pipeline.cpp` & `pikepdf-8.0.0rc3/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/pipeline.h` & `pikepdf-8.0.0rc3/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/qpdf.cpp` & `pikepdf-8.0.0rc3/src/core/qpdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/qpdf_inputsource-inl.h` & `pikepdf-8.0.0rc3/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/qpdf_pagelist.cpp` & `pikepdf-8.0.0rc3/src/core/qpdf_pagelist.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/qpdf_pagelist.h` & `pikepdf-8.0.0rc3/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/rectangle.cpp` & `pikepdf-8.0.0rc3/src/core/rectangle.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/tokenfilter.cpp` & `pikepdf-8.0.0rc3/src/core/tokenfilter.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/utils.cpp` & `pikepdf-8.0.0rc3/src/core/utils.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/core/utils.h` & `pikepdf-8.0.0rc3/src/core/utils.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/__init__.py` & `pikepdf-8.0.0rc3/src/pikepdf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """A library for manipulating PDFs."""
 
 # isort:skip_file
 
 from __future__ import annotations
 
-__version__ = "8.0.0rc2"
+__version__ = "8.0.0rc3"
 
 try:
     from . import _core
 except ImportError as _e:  # pragma: no cover
     _msg = "pikepdf's extension library failed to import"
     raise ImportError(_msg) from _e
```

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/_augments.py` & `pikepdf-8.0.0rc3/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/_cpphelpers.py` & `pikepdf-8.0.0rc3/src/pikepdf/_cpphelpers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/_methods.py` & `pikepdf-8.0.0rc3/src/pikepdf/_methods.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/_qpdf.py` & `pikepdf-8.0.0rc3/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/_xml.py` & `pikepdf-8.0.0rc3/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/codec.py` & `pikepdf-8.0.0rc3/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/jbig2.py` & `pikepdf-8.0.0rc3/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/__init__.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/_content_stream.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/_content_stream.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/_transcoding.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/encryption.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/encryption.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/image.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/image.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/matrix.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/metadata.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/models/outlines.py` & `pikepdf-8.0.0rc3/src/pikepdf/models/outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf/objects.py` & `pikepdf-8.0.0rc3/src/pikepdf/objects.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-8.0.0rc3/src/pikepdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-8.0.0rc2/src/pikepdf.egg-info/SOURCES.txt` & `pikepdf-8.0.0rc3/src/pikepdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/src/pikepdf.egg-info/requires.txt` & `pikepdf-8.0.0rc3/src/pikepdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_annotation.py` & `pikepdf-8.0.0rc3/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_attachments.py` & `pikepdf-8.0.0rc3/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_augments.py` & `pikepdf-8.0.0rc3/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_codec.py` & `pikepdf-8.0.0rc3/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_decimal.py` & `pikepdf-8.0.0rc3/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_dictionary.py` & `pikepdf-8.0.0rc3/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_encrypt.py` & `pikepdf-8.0.0rc3/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_errors.py` & `pikepdf-8.0.0rc3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_filters.py` & `pikepdf-8.0.0rc3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_foreign.py` & `pikepdf-8.0.0rc3/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_formxobject.py` & `pikepdf-8.0.0rc3/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_image_access.py` & `pikepdf-8.0.0rc3/tests/test_image_access.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_io.py` & `pikepdf-8.0.0rc3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_ipython.py` & `pikepdf-8.0.0rc3/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_job.py` & `pikepdf-8.0.0rc3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_matrix.py` & `pikepdf-8.0.0rc3/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_metadata.py` & `pikepdf-8.0.0rc3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_nametree.py` & `pikepdf-8.0.0rc3/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_numbertree.py` & `pikepdf-8.0.0rc3/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_object.py` & `pikepdf-8.0.0rc3/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_objectlist.py` & `pikepdf-8.0.0rc3/tests/test_objectlist.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_outlines.py` & `pikepdf-8.0.0rc3/tests/test_outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_page.py` & `pikepdf-8.0.0rc3/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_pages.py` & `pikepdf-8.0.0rc3/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_parsers.py` & `pikepdf-8.0.0rc3/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_pdf.py` & `pikepdf-8.0.0rc3/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_pdfa.py` & `pikepdf-8.0.0rc3/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_private_pdfs.py` & `pikepdf-8.0.0rc3/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_rectangle.py` & `pikepdf-8.0.0rc3/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_refcount.py` & `pikepdf-8.0.0rc3/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_repr.py` & `pikepdf-8.0.0rc3/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.0.0rc2/tests/test_sanity.py` & `pikepdf-8.0.0rc3/tests/test_sanity.py`

 * *Files identical despite different names*

