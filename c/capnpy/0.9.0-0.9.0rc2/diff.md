# Comparing `tmp/capnpy-0.9.0.tar.gz` & `tmp/capnpy-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capnpy-0.9.0.tar", last modified: Fri Oct 22 09:32:44 2021, max compression
+gzip compressed data, was "capnpy-0.9.0rc2.tar", last modified: Tue Oct 19 11:55:34 2021, max compression
```

## Comparing `capnpy-0.9.0.tar` & `capnpy-0.9.0rc2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.147179 capnpy-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.119178 capnpy-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.123178 capnpy-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-10-22 09:32:35.000000 capnpy-0.9.0/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2021-10-22 09:32:35.000000 capnpy-0.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-10-22 09:32:35.000000 capnpy-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2021-10-22 09:32:35.000000 capnpy-0.9.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-10-22 09:32:35.000000 capnpy-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-22 09:32:35.000000 capnpy-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-10-22 09:32:35.000000 capnpy-0.9.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-22 09:32:44.147179 capnpy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2021-10-22 09:32:35.000000 capnpy-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.131178 capnpy-0.9.0/capnpy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   198728 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/_hash.c
--rw-r--r--   0 runner    (1001) docker     (121)      962 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_hash.h
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_hash.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_hash.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_hash_cpython.c
--rw-r--r--   0 runner    (1001) docker     (121)   152523 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/_util.c
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_util.h
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/_util.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/annotate.capnp
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/annotate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/annotate_extended.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/anypointer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.135178 capnpy-0.9.0/capnpy/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/benchmarks.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/benchmarks_base.capnp
--rw-r--r--   0 runner    (1001) docker     (121)   163824 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/bigtree.dump
--rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/support.py
--rw-r--r--   0 runner    (1001) docker     (121)     9630 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/test_ctor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/test_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/benchmarks/test_unpack.py
--rw-r--r--   0 runner    (1001) docker     (121)   354843 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/blob.c
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/blob.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/blob.py
--rw-r--r--   0 runner    (1001) docker     (121)   503874 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/buffered.c
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/buffered.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/buffered.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.135178 capnpy-0.9.0/capnpy/compiler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11201 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/distutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     9234 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/fieldtree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9223 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     6720 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    14250 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/struct_.py
--rw-r--r--   0 runner    (1001) docker     (121)     7563 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/structor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/convert_case.py
--rw-r--r--   0 runner    (1001) docker     (121)   263739 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/enum.c
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/enum.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.135178 capnpy-0.9.0/capnpy/ext/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   317884 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/filelike.c
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/filelike.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/filelike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.135178 capnpy-0.9.0/capnpy/floatrepr/
--rw-r--r--   0 runner    (1001) docker     (121)      981 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/floatrepr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/floatrepr/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/floatrepr/kjwrap.cc
--rw-r--r--   0 runner    (1001) docker     (121)  1363434 2021-10-22 09:32:42.000000 capnpy-0.9.0/capnpy/list.c
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/list.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    13330 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/list.py
--rw-r--r--   0 runner    (1001) docker     (121)   415759 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/message.c
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/message.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6404 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/message.py
--rw-r--r--   0 runner    (1001) docker     (121)   372830 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/packing.c
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/packing.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/packing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5886 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/packing.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/printer.py
--rw-r--r--   0 runner    (1001) docker     (121)   272433 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/ptr.c
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/ptr.h
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/ptr.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5558 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/ptr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/ptr.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)    18198 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/schema.capnp
--rw-r--r--   0 runner    (1001) docker     (121)   129103 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    10131 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/schema_extended.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.139178 capnpy-0.9.0/capnpy/segment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/_copy_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/_copy_pointer.h
--rw-r--r--   0 runner    (1001) docker     (121)     8909 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/_copy_pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/_copy_pointer.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   383745 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/segment/base.c
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/base.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/base.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   728156 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/segment/builder.c
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/builder.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8029 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/builder.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   190910 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/segment/endof.c
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/endof.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/endof.py
--rw-r--r--   0 runner    (1001) docker     (121)   320445 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/segment/segment.c
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/segment.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4788 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/segment/segment.py
--rw-r--r--   0 runner    (1001) docker     (121)   750462 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/struct_.c
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/struct_.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    12652 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/struct_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.139178 capnpy-0.9.0/capnpy/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.143179 capnpy-0.9.0/capnpy/testing/compiler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/support.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_anypointer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11092 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_const.py
--rw-r--r--   0 runner    (1001) docker     (121)    14220 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_ctor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8417 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_ctor_union.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_distutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_evolution.py
--rw-r--r--   0 runner    (1001) docker     (121)    18339 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_fieldtree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8416 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_null.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_py_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)    11862 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5123 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_standalone.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/compiler/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.143179 capnpy-0.9.0/capnpy/testing/segment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4672 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    11902 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    15684 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/test_copy_pointer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14688 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/test_endof.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/segment/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test__hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_convert_case.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_filelike.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_floatrepr.py
--rw-r--r--   0 runner    (1001) docker     (121)    15104 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)    10331 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_ptr.py
--rw-r--r--   0 runner    (1001) docker     (121)    10630 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_struct_.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/testing/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)   295789 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy/type.c
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/type.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2021-10-22 09:32:35.000000 capnpy-0.9.0/capnpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.131178 capnpy-0.9.0/capnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5010 2021-10-22 09:32:44.000000 capnpy-0.9.0/capnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-22 09:32:43.000000 capnpy-0.9.0/capnpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.143179 capnpy-0.9.0/ci/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-22 09:32:35.000000 capnpy-0.9.0/ci/install_capnp.sh
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-10-22 09:32:35.000000 capnpy-0.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.143179 capnpy-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7686 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.143179 capnpy-0.9.0/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/ext/benchmark_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)    11015 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/ext/charter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9704 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/ext/test_charter.py
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.147179 capnpy-0.9.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)    11208 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10114 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_compact.capnp
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_enum.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_group.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_key.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_named_union.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_options.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_py_group.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_reflection.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_reflection_db.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_struct.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/example_union.capnp
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    32549 2021-10-22 09:32:35.000000 capnpy-0.9.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 09:32:44.147179 capnpy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6685 2021-10-22 09:32:35.000000 capnpy-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2021-10-22 09:32:35.000000 capnpy-0.9.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.147179 capnpy-0.9.0/travis/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 09:32:44.147179 capnpy-0.9.0/travis/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)    51800 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/bin/tcpserver
--rwxr-xr-x   0 runner    (1001) docker     (121)      735 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/build-wheels.sh
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/clone-benchmarks-repo.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/commit-results.sh
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/install_capnp.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/travis.rsa.enc
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-10-22 09:32:35.000000 capnpy-0.9.0/travis/travis.rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.949266 capnpy-0.9.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.921265 capnpy-0.9.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.925265 capnpy-0.9.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-10-19 11:55:34.949266 capnpy-0.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.933265 capnpy-0.9.0rc2/capnpy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2588 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   198728 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/_hash.c
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_hash.h
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_hash.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_hash.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_hash_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (121)   152523 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/_util.c
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_util.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2569 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/_util.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/annotate.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)     6061 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2890 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/annotate_extended.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/anypointer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.937265 capnpy-0.9.0rc2/capnpy/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/benchmarks.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/benchmarks_base.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)   163824 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/bigtree.dump
+-rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/support.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9630 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4644 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/test_ctor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4366 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/benchmarks/test_unpack.py
+-rw-r--r--   0 runner    (1001) docker     (121)   354843 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/blob.c
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/blob.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/blob.py
+-rw-r--r--   0 runner    (1001) docker     (121)   503874 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/buffered.c
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/buffered.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4316 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/buffered.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.937265 capnpy-0.9.0rc2/capnpy/compiler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11201 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/distutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9234 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/fieldtree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9223 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6720 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7396 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14250 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/struct_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7563 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/structor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/convert_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)   263739 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/enum.c
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/enum.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.937265 capnpy-0.9.0rc2/capnpy/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   317884 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/filelike.c
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/filelike.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/filelike.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.937265 capnpy-0.9.0rc2/capnpy/floatrepr/
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/floatrepr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/floatrepr/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/floatrepr/kjwrap.cc
+-rw-r--r--   0 runner    (1001) docker     (121)  1363434 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/list.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2300 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/list.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    13330 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)   415759 2021-10-19 11:55:33.000000 capnpy-0.9.0rc2/capnpy/message.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/message.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     6404 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)   372830 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/packing.c
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/packing.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1820 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/packing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5886 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/packing.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)   272433 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/ptr.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/ptr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/ptr.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5558 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/ptr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/ptr.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18198 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/schema.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)   129103 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10131 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/schema_extended.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.941265 capnpy-0.9.0rc2/capnpy/segment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/_copy_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8909 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   383745 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/segment/base.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2820 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7343 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   728156 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/segment/builder.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2438 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/builder.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4492 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8029 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/builder.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   190910 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/segment/endof.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/endof.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2970 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/endof.py
+-rw-r--r--   0 runner    (1001) docker     (121)   320445 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/segment/segment.c
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/segment.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4788 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/segment/segment.py
+-rw-r--r--   0 runner    (1001) docker     (121)   750462 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/struct_.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/struct_.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    12652 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/struct_.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.941265 capnpy-0.9.0rc2/capnpy/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/capnpy/testing/compiler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/support.py
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4944 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_anypointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11092 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14220 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_ctor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8417 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_ctor_union.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4347 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_distutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18339 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_fieldtree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5088 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8416 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_null.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2805 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_py_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11862 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5123 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/compiler/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/capnpy/testing/segment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4672 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11902 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15684 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/test_copy_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14688 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/test_endof.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/segment/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test__hash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5471 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_convert_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_filelike.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_floatrepr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15104 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10331 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4221 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10630 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_struct_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/testing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)   295789 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy/type.c
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/type.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3328 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/capnpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.937265 capnpy-0.9.0rc2/capnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5010 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-19 11:55:34.000000 capnpy-0.9.0rc2/capnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/ci/
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/ci/install_capnp.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     7686 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/ext/benchmark_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11015 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/ext/charter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9704 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/ext/test_charter.py
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)    11208 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10114 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_compact.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_enum.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_group.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_key.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_named_union.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_options.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_py_group.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_reflection.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_reflection_db.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_struct.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/example_union.capnp
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    32549 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-19 11:55:34.949266 capnpy-0.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6685 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/travis/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-19 11:55:34.945266 capnpy-0.9.0rc2/travis/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    51800 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/bin/tcpserver
+-rwxr-xr-x   0 runner    (1001) docker     (121)      735 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/build-wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/clone-benchmarks-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/commit-results.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/install_capnp.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/travis.rsa.enc
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-10-19 11:55:26.000000 capnpy-0.9.0rc2/travis/travis.rsa.pub
```

### Comparing `capnpy-0.9.0/.github/workflows/release-pypi.yml` & `capnpy-0.9.0rc2/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/.github/workflows/test.yml` & `capnpy-0.9.0rc2/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ---
 name: tests
 
+# XXX temporary: disable tests for now in this PR
 on:
   push:
     branches:
     - master
-  pull_request:
-    branches:
-    - master
+  # pull_request:
+  #   branches:
+  #   - master
 
 env:
   CAPNPROTO: capnproto-c++-0.7.0
 
 jobs:
   tox_tests:
     name: tox -e ${{ matrix.toxenv }}
```

### Comparing `capnpy-0.9.0/.travis.yml` & `capnpy-0.9.0rc2/.travis.yml`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/LICENSE` & `capnpy-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/Makefile` & `capnpy-0.9.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/__main__.py` & `capnpy-0.9.0rc2/capnpy/__main__.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_hash.c` & `capnpy-0.9.0rc2/capnpy/_hash.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_hash.h` & `capnpy-0.9.0rc2/capnpy/_hash.h`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_hash.pyx` & `capnpy-0.9.0rc2/capnpy/_hash.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_hash_cpython.c` & `capnpy-0.9.0rc2/capnpy/_hash_cpython.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_util.c` & `capnpy-0.9.0rc2/capnpy/_util.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_util.h` & `capnpy-0.9.0rc2/capnpy/_util.h`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/_util.pyx` & `capnpy-0.9.0rc2/capnpy/_util.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/annotate.capnp` & `capnpy-0.9.0rc2/capnpy/annotate.capnp`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/annotate.py` & `capnpy-0.9.0rc2/capnpy/annotate.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/annotate_extended.py` & `capnpy-0.9.0rc2/capnpy/annotate_extended.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/anypointer.py` & `capnpy-0.9.0rc2/capnpy/anypointer.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/benchmarks.capnp` & `capnpy-0.9.0rc2/capnpy/benchmarks/benchmarks.capnp`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/bigtree.dump` & `capnpy-0.9.0rc2/capnpy/benchmarks/bigtree.dump`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/support.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/support.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/test_benchmarks.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/test_buffered.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/test_buffered.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/test_ctor.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/test_ctor.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/test_message.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/test_message.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/benchmarks/test_unpack.py` & `capnpy-0.9.0rc2/capnpy/benchmarks/test_unpack.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/blob.c` & `capnpy-0.9.0rc2/capnpy/blob.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/blob.py` & `capnpy-0.9.0rc2/capnpy/blob.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/buffered.c` & `capnpy-0.9.0rc2/capnpy/buffered.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/buffered.pxd` & `capnpy-0.9.0rc2/capnpy/buffered.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/buffered.py` & `capnpy-0.9.0rc2/capnpy/buffered.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/compiler.py` & `capnpy-0.9.0rc2/capnpy/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/distutils.py` & `capnpy-0.9.0rc2/capnpy/compiler/distutils.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/enum.py` & `capnpy-0.9.0rc2/capnpy/compiler/enum.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/field.py` & `capnpy-0.9.0rc2/capnpy/compiler/field.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/fieldtree.py` & `capnpy-0.9.0rc2/capnpy/compiler/fieldtree.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/misc.py` & `capnpy-0.9.0rc2/capnpy/compiler/misc.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/module.py` & `capnpy-0.9.0rc2/capnpy/compiler/module.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/node.py` & `capnpy-0.9.0rc2/capnpy/compiler/node.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/request.py` & `capnpy-0.9.0rc2/capnpy/compiler/request.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/struct_.py` & `capnpy-0.9.0rc2/capnpy/compiler/struct_.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/structor.py` & `capnpy-0.9.0rc2/capnpy/compiler/structor.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/compiler/util.py` & `capnpy-0.9.0rc2/capnpy/compiler/util.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/enum.c` & `capnpy-0.9.0rc2/capnpy/enum.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/enum.py` & `capnpy-0.9.0rc2/capnpy/enum.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/filelike.c` & `capnpy-0.9.0rc2/capnpy/filelike.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/filelike.py` & `capnpy-0.9.0rc2/capnpy/filelike.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/floatrepr/__init__.py` & `capnpy-0.9.0rc2/capnpy/floatrepr/__init__.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/floatrepr/build.py` & `capnpy-0.9.0rc2/capnpy/floatrepr/build.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/list.c` & `capnpy-0.9.0rc2/capnpy/list.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/list.pxd` & `capnpy-0.9.0rc2/capnpy/list.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/list.py` & `capnpy-0.9.0rc2/capnpy/list.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/message.c` & `capnpy-0.9.0rc2/capnpy/message.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/message.pxd` & `capnpy-0.9.0rc2/capnpy/message.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/message.py` & `capnpy-0.9.0rc2/capnpy/message.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/packing.c` & `capnpy-0.9.0rc2/capnpy/packing.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/packing.pxd` & `capnpy-0.9.0rc2/capnpy/packing.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/packing.py` & `capnpy-0.9.0rc2/capnpy/packing.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/packing.pyx` & `capnpy-0.9.0rc2/capnpy/packing.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/printer.py` & `capnpy-0.9.0rc2/capnpy/printer.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/ptr.c` & `capnpy-0.9.0rc2/capnpy/ptr.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/ptr.h` & `capnpy-0.9.0rc2/capnpy/ptr.h`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/ptr.pxd` & `capnpy-0.9.0rc2/capnpy/ptr.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/ptr.py` & `capnpy-0.9.0rc2/capnpy/ptr.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/ptr.pyx` & `capnpy-0.9.0rc2/capnpy/ptr.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/reflection.py` & `capnpy-0.9.0rc2/capnpy/reflection.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/schema.capnp` & `capnpy-0.9.0rc2/capnpy/schema.capnp`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/schema.py` & `capnpy-0.9.0rc2/capnpy/schema.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/schema_extended.py` & `capnpy-0.9.0rc2/capnpy/schema_extended.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/_copy_list.py` & `capnpy-0.9.0rc2/capnpy/segment/_copy_list.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/_copy_pointer.h` & `capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.h`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/_copy_pointer.py` & `capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/_copy_pointer.pyx` & `capnpy-0.9.0rc2/capnpy/segment/_copy_pointer.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/base.c` & `capnpy-0.9.0rc2/capnpy/segment/base.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/base.pxd` & `capnpy-0.9.0rc2/capnpy/segment/base.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/base.py` & `capnpy-0.9.0rc2/capnpy/segment/base.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/base.pyx` & `capnpy-0.9.0rc2/capnpy/segment/base.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/builder.c` & `capnpy-0.9.0rc2/capnpy/segment/builder.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/builder.pxd` & `capnpy-0.9.0rc2/capnpy/segment/builder.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/builder.py` & `capnpy-0.9.0rc2/capnpy/segment/builder.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/builder.pyx` & `capnpy-0.9.0rc2/capnpy/segment/builder.pyx`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/endof.c` & `capnpy-0.9.0rc2/capnpy/segment/endof.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/endof.pxd` & `capnpy-0.9.0rc2/capnpy/segment/endof.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/endof.py` & `capnpy-0.9.0rc2/capnpy/segment/endof.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/segment.c` & `capnpy-0.9.0rc2/capnpy/segment/segment.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/segment.pxd` & `capnpy-0.9.0rc2/capnpy/segment/segment.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/segment/segment.py` & `capnpy-0.9.0rc2/capnpy/segment/segment.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/struct_.c` & `capnpy-0.9.0rc2/capnpy/struct_.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/struct_.pxd` & `capnpy-0.9.0rc2/capnpy/struct_.pxd`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/struct_.py` & `capnpy-0.9.0rc2/capnpy/struct_.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/support.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/support.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_anypointer.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_anypointer.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_compiler.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_const.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_const.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_ctor.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_ctor.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_ctor_union.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_ctor_union.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_distutils.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_distutils.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_evolution.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_evolution.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_field.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_field.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_fieldtree.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_fieldtree.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_import.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_import.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_key.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_key.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_misc.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_misc.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_null.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_null.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_py_group.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_py_group.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_reflection.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_reflection.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_repr.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_repr.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_standalone.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_standalone.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/compiler/test_util.py` & `capnpy-0.9.0rc2/capnpy/testing/compiler/test_util.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/segment/test_base.py` & `capnpy-0.9.0rc2/capnpy/testing/segment/test_base.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/segment/test_builder.py` & `capnpy-0.9.0rc2/capnpy/testing/segment/test_builder.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/segment/test_copy_pointer.py` & `capnpy-0.9.0rc2/capnpy/testing/segment/test_copy_pointer.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/segment/test_endof.py` & `capnpy-0.9.0rc2/capnpy/testing/segment/test_endof.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/segment/test_segment.py` & `capnpy-0.9.0rc2/capnpy/testing/segment/test_segment.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test__hash.py` & `capnpy-0.9.0rc2/capnpy/testing/test__hash.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_annotate.py` & `capnpy-0.9.0rc2/capnpy/testing/test_annotate.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_blob.py` & `capnpy-0.9.0rc2/capnpy/testing/test_blob.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_buffered.py` & `capnpy-0.9.0rc2/capnpy/testing/test_buffered.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_enum.py` & `capnpy-0.9.0rc2/capnpy/testing/test_enum.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_list.py` & `capnpy-0.9.0rc2/capnpy/testing/test_list.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_main.py` & `capnpy-0.9.0rc2/capnpy/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_message.py` & `capnpy-0.9.0rc2/capnpy/testing/test_message.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_packing.py` & `capnpy-0.9.0rc2/capnpy/testing/test_packing.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_ptr.py` & `capnpy-0.9.0rc2/capnpy/testing/test_ptr.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_struct_.py` & `capnpy-0.9.0rc2/capnpy/testing/test_struct_.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/testing/test_util.py` & `capnpy-0.9.0rc2/capnpy/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/type.c` & `capnpy-0.9.0rc2/capnpy/type.c`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/type.py` & `capnpy-0.9.0rc2/capnpy/type.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy/util.py` & `capnpy-0.9.0rc2/capnpy/util.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/capnpy.egg-info/SOURCES.txt` & `capnpy-0.9.0rc2/capnpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/Makefile` & `capnpy-0.9.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/ext/benchmark_directive.py` & `capnpy-0.9.0rc2/docs/ext/benchmark_directive.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/ext/charter.py` & `capnpy-0.9.0rc2/docs/ext/charter.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/ext/test_charter.py` & `capnpy-0.9.0rc2/docs/ext/test_charter.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/source/benchmarks.rst` & `capnpy-0.9.0rc2/docs/source/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/source/changelog.rst` & `capnpy-0.9.0rc2/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/source/conf.py` & `capnpy-0.9.0rc2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/source/index.rst` & `capnpy-0.9.0rc2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/docs/source/usage.rst` & `capnpy-0.9.0rc2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/setup.py` & `capnpy-0.9.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/tox.ini` & `capnpy-0.9.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/travis/bin/tcpserver` & `capnpy-0.9.0rc2/travis/bin/tcpserver`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/travis/build-wheels.sh` & `capnpy-0.9.0rc2/travis/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/travis/commit-results.sh` & `capnpy-0.9.0rc2/travis/commit-results.sh`

 * *Files identical despite different names*

### Comparing `capnpy-0.9.0/travis/travis.rsa.enc` & `capnpy-0.9.0rc2/travis/travis.rsa.enc`

 * *Files identical despite different names*

