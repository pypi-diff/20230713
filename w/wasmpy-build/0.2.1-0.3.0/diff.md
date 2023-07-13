# Comparing `tmp/wasmpy-build-0.2.1.tar.gz` & `tmp/wasmpy-build-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.2.1.tar", last modified: Mon May 22 11:37:15 2023, max compression
+gzip compressed data, was "wasmpy-build-0.3.0.tar", last modified: Thu Jul 13 01:15:53 2023, max compression
```

## Comparing `wasmpy-build-0.2.1.tar` & `wasmpy-build-0.3.0.tar`

### file list

```diff
@@ -1,677 +1,677 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:15.544855 wasmpy-build-0.2.1/
--rw-rw-rw-   0        0        0     1068 2022-10-10 14:10:03.000000 wasmpy-build-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1863 2023-05-22 11:37:15.477333 wasmpy-build-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2022-10-10 14:10:03.000000 wasmpy-build-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 11:37:15.545844 wasmpy-build-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1431 2023-05-22 08:36:05.000000 wasmpy-build-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:10.969835 wasmpy-build-0.2.1/wasmpy_build/
--rw-rw-rw-   0        0        0     1165 2023-05-22 11:35:05.000000 wasmpy-build-0.2.1/wasmpy_build/__init__.py
--rw-rw-rw-   0        0        0       64 2023-05-22 11:09:10.000000 wasmpy-build-0.2.1/wasmpy_build/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:10.957105 wasmpy-build-0.2.1/wasmpy_build/include/
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:11.198654 wasmpy-build-0.2.1/wasmpy_build/include/cp310/
--rw-rw-rw-   0        0        0    13936 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/LICENSE
--rw-rw-rw-   0        0        0     3226 2023-05-22 11:20:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/Python.h
--rw-rw-rw-   0        0        0      344 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/README.rst
--rw-rw-rw-   0        0        0    31405 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/abstract.h
--rw-rw-rw-   0        0        0      264 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/bltinmodule.h
--rw-rw-rw-   0        0        0     1224 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/bytearrayobject.h
--rw-rw-rw-   0        0        0     2593 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/bytesobject.h
--rw-rw-rw-   0        0        0      720 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cellobject.h
--rw-rw-rw-   0        0        0     5703 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/classobject.h
--rw-rw-rw-   0        0        0      318 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/code.h
--rw-rw-rw-   0        0        0     7071 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/codecs.h
--rw-rw-rw-   0        0        0      520 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/compile.h
--rw-rw-rw-   0        0        0     1806 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/context.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:11.279583 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/
--rw-rw-rw-   0        0        0    14054 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4119 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1468 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/ceval.h
--rw-rw-rw-   0        0        0     7570 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/compile.h
--rw-rw-rw-   0        0        0     3734 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/dictobject.h
--rw-rw-rw-   0        0        0      723 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4267 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3152 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1630 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/import.h
--rw-rw-rw-   0        0        0     7597 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/initconfig.h
--rw-rw-rw-   0        0        0      387 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1243 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19613 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/object.h
--rw-rw-rw-   0        0        0     3356 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     1387 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pydebug.h
--rw-rw-rw-   0        0        0     5476 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pyfpe.h
--rw-rw-rw-   0        0        0     2095 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pymem.h
--rw-rw-rw-   0        0        0    11914 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     9196 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pytime.h
--rw-rw-rw-   0        0        0      506 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      404 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/traceback.h
--rw-rw-rw-   0        0        0      975 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    44284 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9635 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/datetime.h
--rw-rw-rw-   0        0        0     3002 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/descrobject.h
--rw-rw-rw-   0        0        0     3853 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/errcode.h
--rw-rw-rw-   0        0        0      831 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/eval.h
--rw-rw-rw-   0        0        0     1098 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/exports.h
--rw-rw-rw-   0        0        0     1571 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/fileobject.h
--rw-rw-rw-   0        0        0      508 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/frameobject.h
--rw-rw-rw-   0        0        0     4257 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/genericaliasobject.h
--rw-rw-rw-   0        0        0     3347 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/genobject.h
--rw-rw-rw-   0        0        0     3026 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/import.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:11.408564 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/
--rw-rw-rw-   0        0        0      479 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     2971 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    28828 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6457 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16981 2023-05-22 11:20:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     5271 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0      870 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3484 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      696 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2809 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      822 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1704 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      480 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_format.h
--rw-rw-rw-   0        0        0     6859 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      346 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5625 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     9289 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      350 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_list.h
--rw-rw-rw-   0        0        0     2589 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1047 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0     5989 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_object.h
--rw-rw-rw-   0        0        0      626 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_parser.h
--rw-rw-rw-   0        0        0     1981 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2314 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     4940 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3211 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3938 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4902 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      386 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5578 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      548 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     2970 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      425 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0      898 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0      629 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      633 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/interpreteridobject.h
--rw-rw-rw-   0        0        0      772 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/longintrepr.h
--rw-rw-rw-   0        0        0     8606 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/memoryobject.h
--rw-rw-rw-   0        0        0     4147 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/methodobject.h
--rw-rw-rw-   0        0        0    10333 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/modsupport.h
--rw-rw-rw-   0        0        0     2458 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/namespaceobject.h
--rw-rw-rw-   0        0        0    28344 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/object.h
--rw-rw-rw-   0        0        0     8445 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/objimpl.h
--rw-rw-rw-   0        0        0     5509 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/opcode.h
--rw-rw-rw-   0        0        0      737 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/osdefs.h
--rw-rw-rw-   0        0        0      291 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/osmodule.h
--rw-rw-rw-   0        0        0     1302 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/patchlevel.h
--rw-rw-rw-   0        0        0     2474 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/py_curses.h
--rw-rw-rw-   0        0        0     1725 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pycapsule.h
--rw-rw-rw-   0        0        0     1008 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pydtrace.h
--rw-rw-rw-   0        0        0    12426 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyexpat.h
--rw-rw-rw-   0        0        0      466 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyframe.h
--rw-rw-rw-   0        0        0     4223 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyhash.h
--rw-rw-rw-   0        0        0     2080 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymacro.h
--rw-rw-rw-   0        0        0     8315 2023-05-22 11:20:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymath.h
--rw-rw-rw-   0        0        0     3891 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymem.h
--rw-rw-rw-   0        0        0    31688 2023-05-22 11:20:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystate.h
--rw-rw-rw-   0        0        0      436 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystrtod.h
--rw-rw-rw-   0        0        0     1110 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/pythread.h
--rw-rw-rw-   0        0        0      628 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/rangeobject.h
--rw-rw-rw-   0        0        0     3381 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/sliceobject.h
--rw-rw-rw-   0        0        0     2074 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/structseq.h
--rw-rw-rw-   0        0        0     1242 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/token.h
--rw-rw-rw-   0        0        0      584 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/traceback.h
--rw-rw-rw-   0        0        0     1114 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/tupleobject.h
--rw-rw-rw-   0        0        0     2460 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/typeslots.h
--rw-rw-rw-   0        0        0    36148 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-22 11:13:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp310/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:11.691806 wasmpy-build-0.2.1/wasmpy_build/include/cp311/
--rw-rw-rw-   0        0        0    13936 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/LICENSE
--rw-rw-rw-   0        0        0     2856 2023-05-22 11:20:37.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/Python.h
--rw-rw-rw-   0        0        0      344 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/README.rst
--rw-rw-rw-   0        0        0    31404 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/abstract.h
--rw-rw-rw-   0        0        0      264 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/bltinmodule.h
--rw-rw-rw-   0        0        0     1212 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/boolobject.h
--rw-rw-rw-   0        0        0     1462 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/bytearrayobject.h
--rw-rw-rw-   0        0        0     2617 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/bytesobject.h
--rw-rw-rw-   0        0        0     6255 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/ceval.h
--rw-rw-rw-   0        0        0     7071 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/codecs.h
--rw-rw-rw-   0        0        0      520 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/compile.h
--rw-rw-rw-   0        0        0      724 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/complexobject.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:11.929359 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/
--rw-rw-rw-   0        0        0     8229 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/abstract.h
--rw-rw-rw-   0        0        0     1305 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4568 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/bytesobject.h
--rw-rw-rw-   0        0        0      723 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/cellobject.h
--rw-rw-rw-   0        0        0     1239 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/ceval.h
--rw-rw-rw-   0        0        0     1656 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/classobject.h
--rw-rw-rw-   0        0        0    11484 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/code.h
--rw-rw-rw-   0        0        0     2218 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/compile.h
--rw-rw-rw-   0        0        0     1248 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/complexobject.h
--rw-rw-rw-   0        0        0     1959 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/context.h
--rw-rw-rw-   0        0        0     1642 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/descrobject.h
--rw-rw-rw-   0        0        0     3324 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/dictobject.h
--rw-rw-rw-   0        0        0      818 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/fileobject.h
--rw-rw-rw-   0        0        0      232 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/fileutils.h
--rw-rw-rw-   0        0        0      702 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/floatobject.h
--rw-rw-rw-   0        0        0     1108 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/frameobject.h
--rw-rw-rw-   0        0        0     4424 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/funcobject.h
--rw-rw-rw-   0        0        0     3279 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/genobject.h
--rw-rw-rw-   0        0        0     1526 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/import.h
--rw-rw-rw-   0        0        0     7817 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/initconfig.h
--rw-rw-rw-   0        0        0     1769 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/listobject.h
--rw-rw-rw-   0        0        0     3817 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/longintrepr.h
--rw-rw-rw-   0        0        0     4532 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/longobject.h
--rw-rw-rw-   0        0        0     2556 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/methodobject.h
--rw-rw-rw-   0        0        0     4234 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/modsupport.h
--rw-rw-rw-   0        0        0    18305 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/object.h
--rw-rw-rw-   0        0        0     2998 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/odictobject.h
--rw-rw-rw-   0        0        0      846 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/picklebufobject.h
--rw-rw-rw-   0        0        0     3505 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h
--rw-rw-rw-   0        0        0     1387 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyctype.h
--rw-rw-rw-   0        0        0     1073 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pydebug.h
--rw-rw-rw-   0        0        0     4522 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyerrors.h
--rw-rw-rw-   0        0        0      444 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyfpe.h
--rw-rw-rw-   0        0        0      582 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyframe.h
--rw-rw-rw-   0        0        0     2099 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3379 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pymem.h
--rw-rw-rw-   0        0        0    14351 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pystate.h
--rw-rw-rw-   0        0        0     4811 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pythonrun.h
--rw-rw-rw-   0        0        0     1426 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pythread.h
--rw-rw-rw-   0        0        0    12158 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pytime.h
--rw-rw-rw-   0        0        0     1997 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/setobject.h
--rw-rw-rw-   0        0        0      489 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      444 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/traceback.h
--rw-rw-rw-   0        0        0     1513 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    41910 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0      560 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/warnings.h
--rw-rw-rw-   0        0        0     2103 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/weakrefobject.h
--rw-rw-rw-   0        0        0     9635 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/datetime.h
--rw-rw-rw-   0        0        0     1256 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/descrobject.h
--rw-rw-rw-   0        0        0     3852 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/dictobject.h
--rw-rw-rw-   0        0        0    22471 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/enumobject.h
--rw-rw-rw-   0        0        0     1700 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/errcode.h
--rw-rw-rw-   0        0        0     1098 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/exports.h
--rw-rw-rw-   0        0        0     1570 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/fileobject.h
--rw-rw-rw-   0        0        0      507 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/fileutils.h
--rw-rw-rw-   0        0        0     1530 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/floatobject.h
--rw-rw-rw-   0        0        0      336 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/frameobject.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/genericaliasobject.h
--rw-rw-rw-   0        0        0     3025 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/import.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:12.836620 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/
--rw-rw-rw-   0        0        0      611 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_accu.h
--rw-rw-rw-   0        0        0     3031 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_asdl.h
--rw-rw-rw-   0        0        0    29315 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ast.h
--rw-rw-rw-   0        0        0     6535 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h
--rw-rw-rw-   0        0        0    16981 2023-05-22 11:20:37.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     2438 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
--rw-rw-rw-   0        0        0     6062 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h
--rw-rw-rw-   0        0        0     8688 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
--rw-rw-rw-   0        0        0     3384 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     1424 2023-05-22 11:20:24.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
--rw-rw-rw-   0        0        0     3475 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_call.h
--rw-rw-rw-   0        0        0     4409 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0    15930 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_code.h
--rw-rw-rw-   0        0        0     1045 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_compile.h
--rw-rw-rw-   0        0        0     2839 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0     1239 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_context.h
--rw-rw-rw-   0        0        0     5684 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_dict.h
--rw-rw-rw-   0        0        0      704 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0      562 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
--rw-rw-rw-   0        0        0      842 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h
--rw-rw-rw-   0        0        0     7313 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     1307 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h
--rw-rw-rw-   0        0        0      480 2023-05-22 11:20:09.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_format.h
--rw-rw-rw-   0        0        0     7567 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_frame.h
--rw-rw-rw-   0        0        0      413 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_function.h
--rw-rw-rw-   0        0        0     6895 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_gc.h
--rw-rw-rw-   0        0        0     1164 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_genobject.h
--rw-rw-rw-   0        0        0      490 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     1436 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h
--rw-rw-rw-   0        0        0    12980 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h
--rw-rw-rw-   0        0        0     3696 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      743 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5800 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     6671 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_interp.h
--rw-rw-rw-   0        0        0      562 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
--rw-rw-rw-   0        0        0     1352 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_list.h
--rw-rw-rw-   0        0        0     3516 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_long.h
--rw-rw-rw-   0        0        0     1040 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
--rw-rw-rw-   0        0        0      392 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_namespace.h
--rw-rw-rw-   0        0        0    10037 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_object.h
--rw-rw-rw-   0        0        0    18986 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_opcode.h
--rw-rw-rw-   0        0        0      626 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_parser.h
--rw-rw-rw-   0        0        0      606 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2733 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h
--rw-rw-rw-   0        0        0     2494 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3507 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     9435 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pymath.h
--rw-rw-rw-   0        0        0     3708 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     4107 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     5988 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0    49092 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
--rw-rw-rw-   0        0        0      937 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_signal.h
--rw-rw-rw-   0        0        0      336 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
--rw-rw-rw-   0        0        0      937 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_strhex.h
--rw-rw-rw-   0        0        0      580 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_structseq.h
--rw-rw-rw-   0        0        0     5638 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_symtable.h
--rw-rw-rw-   0        0        0      605 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3501 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0     2089 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_tuple.h
--rw-rw-rw-   0        0        0     1158 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h
--rw-rw-rw-   0        0        0      898 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
--rw-rw-rw-   0        0        0     1716 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
--rw-rw-rw-   0        0        0      678 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h
--rw-rw-rw-   0        0        0      740 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      772 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/intrcheck.h
--rw-rw-rw-   0        0        0      593 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/iterobject.h
--rw-rw-rw-   0        0        0     1780 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/listobject.h
--rw-rw-rw-   0        0        0     3272 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/longobject.h
--rw-rw-rw-   0        0        0      827 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/marshal.h
--rw-rw-rw-   0        0        0     2810 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/memoryobject.h
--rw-rw-rw-   0        0        0     5072 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/methodobject.h
--rw-rw-rw-   0        0        0     6448 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/modsupport.h
--rw-rw-rw-   0        0        0     2374 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/moduleobject.h
--rw-rw-rw-   0        0        0    29800 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/object.h
--rw-rw-rw-   0        0        0     8428 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/objimpl.h
--rw-rw-rw-   0        0        0    11187 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/opcode.h
--rw-rw-rw-   0        0        0      737 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/osdefs.h
--rw-rw-rw-   0        0        0      291 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/osmodule.h
--rw-rw-rw-   0        0        0     1300 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/patchlevel.h
--rw-rw-rw-   0        0        0     2471 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/py_curses.h
--rw-rw-rw-   0        0        0     5115 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pybuffer.h
--rw-rw-rw-   0        0        0     1725 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pycapsule.h
--rw-rw-rw-   0        0        0     1008 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pydtrace.h
--rw-rw-rw-   0        0        0    12782 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyexpat.h
--rw-rw-rw-   0        0        0      551 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyframe.h
--rw-rw-rw-   0        0        0     4154 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyhash.h
--rw-rw-rw-   0        0        0     2249 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymacconfig.h
--rw-rw-rw-   0        0        0     6064 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymacro.h
--rw-rw-rw-   0        0        0     1979 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymath.h
--rw-rw-rw-   0        0        0     3890 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymem.h
--rw-rw-rw-   0        0        0    24532 2023-05-22 11:20:37.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyport.h
--rw-rw-rw-   0        0        0     4635 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pystate.h
--rw-rw-rw-   0        0        0      436 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pystrcmp.h
--rw-rw-rw-   0        0        0     1557 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pystrtod.h
--rw-rw-rw-   0        0        0     1189 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pythonrun.h
--rw-rw-rw-   0        0        0     4833 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pythread.h
--rw-rw-rw-   0        0        0      851 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/pytypedefs.h
--rw-rw-rw-   0        0        0      628 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/rangeobject.h
--rw-rw-rw-   0        0        0     1543 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-22 11:13:20.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/sliceobject.h
--rw-rw-rw-   0        0        0     2040 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/structmember.h
--rw-rw-rw-   0        0        0     1388 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/structseq.h
--rw-rw-rw-   0        0        0     1381 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/sysmodule.h
--rw-rw-rw-   0        0        0     2669 2023-05-22 11:20:10.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/token.h
--rw-rw-rw-   0        0        0      583 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/traceback.h
--rw-rw-rw-   0        0        0     1114 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/tracemalloc.h
--rw-rw-rw-   0        0        0     1613 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/tupleobject.h
--rw-rw-rw-   0        0        0     2342 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/typeslots.h
--rw-rw-rw-   0        0        0    36032 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/unicodeobject.h
--rw-rw-rw-   0        0        0     1129 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/warnings.h
--rw-rw-rw-   0        0        0     1226 2023-05-22 11:20:25.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp311/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:13.367033 wasmpy-build-0.2.1/wasmpy_build/include/cp38/
--rw-rw-rw-   0        0        0    13937 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/LICENSE
--rw-rw-rw-   0        0        0    26491 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/Python-ast.h
--rw-rw-rw-   0        0        0     3617 2023-05-22 11:21:00.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/Python.h
--rw-rw-rw-   0        0        0    30286 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/abstract.h
--rw-rw-rw-   0        0        0     1229 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/asdl.h
--rw-rw-rw-   0        0        0      948 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/ast.h
--rw-rw-rw-   0        0        0      468 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/bitset.h
--rw-rw-rw-   0        0        0      264 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/bltinmodule.h
--rw-rw-rw-   0        0        0      886 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/boolobject.h
--rw-rw-rw-   0        0        0     2114 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytearrayobject.h
--rw-rw-rw-   0        0        0     3301 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytes_methods.h
--rw-rw-rw-   0        0        0     8493 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytesobject.h
--rw-rw-rw-   0        0        0      713 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cellobject.h
--rw-rw-rw-   0        0        0     8366 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/ceval.h
--rw-rw-rw-   0        0        0     1710 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/classobject.h
--rw-rw-rw-   0        0        0     7178 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/code.h
--rw-rw-rw-   0        0        0     6793 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/codecs.h
--rw-rw-rw-   0        0        0     3582 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/compile.h
--rw-rw-rw-   0        0        0     1807 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/complexobject.h
--rw-rw-rw-   0        0        0     2014 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/context.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:13.475284 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/
--rw-rw-rw-   0        0        0    12294 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/abstract.h
--rw-rw-rw-   0        0        0     3845 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/fileobject.h
--rw-rw-rw-   0        0        0    16028 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0    15691 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/object.h
--rw-rw-rw-   0        0        0     3600 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/objimpl.h
--rw-rw-rw-   0        0        0     4717 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2263 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pymem.h
--rw-rw-rw-   0        0        0     9810 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pystate.h
--rw-rw-rw-   0        0        0      547 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46308 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9260 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/descrobject.h
--rw-rw-rw-   0        0        0     3716 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/dictobject.h
--rw-rw-rw-   0        0        0      458 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/dtoa.h
--rw-rw-rw-   0        0        0    22469 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/enumobject.h
--rw-rw-rw-   0        0        0     1695 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/eval.h
--rw-rw-rw-   0        0        0     1571 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/fileobject.h
--rw-rw-rw-   0        0        0     4352 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/fileutils.h
--rw-rw-rw-   0        0        0     4794 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/floatobject.h
--rw-rw-rw-   0        0        0     3317 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/frameobject.h
--rw-rw-rw-   0        0        0     4200 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/funcobject.h
--rw-rw-rw-   0        0        0     3720 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/grammar.h
--rw-rw-rw-   0        0        0     4926 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/import.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:14.189133 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/
--rw-rw-rw-   0        0        0     1126 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16946 2023-05-22 11:21:00.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0      966 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      542 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      779 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_context.h
--rw-rw-rw-   0        0        0     1254 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0      490 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1520 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3698 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     5218 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     1548 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_long.h
--rw-rw-rw-   0        0        0     2896 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_object.h
--rw-rw-rw-   0        0        0     2037 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     1329 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3815 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     8217 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     9588 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     3076 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      418 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      591 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/intrcheck.h
--rw-rw-rw-   0        0        0      567 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/iterobject.h
--rw-rw-rw-   0        0        0     2927 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/longintrepr.h
--rw-rw-rw-   0        0        0     9520 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/marshal.h
--rw-rw-rw-   0        0        0     2765 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/memoryobject.h
--rw-rw-rw-   0        0        0     4406 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/methodobject.h
--rw-rw-rw-   0        0        0     9591 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/modsupport.h
--rw-rw-rw-   0        0        0     2362 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/namespaceobject.h
--rw-rw-rw-   0        0        0     1328 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/node.h
--rw-rw-rw-   0        0        0    29599 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/object.h
--rw-rw-rw-   0        0        0    10537 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/objimpl.h
--rw-rw-rw-   0        0        0     1300 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/odictobject.h
--rw-rw-rw-   0        0        0     5164 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/opcode.h
--rw-rw-rw-   0        0        0      737 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/osdefs.h
--rw-rw-rw-   0        0        0      291 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/patchlevel.h
--rw-rw-rw-   0        0        0      847 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/picklebufobject.h
--rw-rw-rw-   0        0        0     2477 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyarena.h
--rw-rw-rw-   0        0        0     1726 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pycapsule.h
--rw-rw-rw-   0        0        0     1387 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyctype.h
--rw-rw-rw-   0        0        0     1214 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydebug.h
--rw-rw-rw-   0        0        0     1008 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydtrace.h
--rw-rw-rw-   0        0        0    12786 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyexpat.h
--rw-rw-rw-   0        0        0      341 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyfpe.h
--rw-rw-rw-   0        0        0     4140 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyhash.h
--rw-rw-rw-   0        0        0     2081 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymacconfig.h
--rw-rw-rw-   0        0        0     3778 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymacro.h
--rw-rw-rw-   0        0        0     8314 2023-05-22 11:21:00.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymath.h
--rw-rw-rw-   0        0        0     5406 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymem.h
--rw-rw-rw-   0        0        0    30225 2023-05-22 11:21:00.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyport.h
--rw-rw-rw-   0        0        0     4686 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystate.h
--rw-rw-rw-   0        0        0      436 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystrtod.h
--rw-rw-rw-   0        0        0     7645 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pythonrun.h
--rw-rw-rw-   0        0        0     5660 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pythread.h
--rw-rw-rw-   0        0        0     8928 2023-05-22 11:21:00.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/pytime.h
--rw-rw-rw-   0        0        0      629 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/rangeobject.h
--rw-rw-rw-   0        0        0     3362 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/setobject.h
--rw-rw-rw-   0        0        0     2517 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/structmember.h
--rw-rw-rw-   0        0        0     1377 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/structseq.h
--rw-rw-rw-   0        0        0     5308 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/sysmodule.h
--rw-rw-rw-   0        0        0     2429 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/token.h
--rw-rw-rw-   0        0        0      601 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/traceback.h
--rw-rw-rw-   0        0        0     1114 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/tracemalloc.h
--rw-rw-rw-   0        0        0     1661 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/tupleobject.h
--rw-rw-rw-   0        0        0     2253 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/ucnhash.h
--rw-rw-rw-   0        0        0    35732 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/warnings.h
--rw-rw-rw-   0        0        0     2866 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp38/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:14.806183 wasmpy-build-0.2.1/wasmpy_build/include/cp39/
--rw-rw-rw-   0        0        0    13937 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/LICENSE
--rw-rw-rw-   0        0        0    26193 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/Python-ast.h
--rw-rw-rw-   0        0        0     3534 2023-05-22 11:21:15.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/Python.h
--rw-rw-rw-   0        0        0    30476 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/abstract.h
--rw-rw-rw-   0        0        0     1224 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/asdl.h
--rw-rw-rw-   0        0        0      947 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/ast.h
--rw-rw-rw-   0        0        0      468 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/bitset.h
--rw-rw-rw-   0        0        0      264 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/bltinmodule.h
--rw-rw-rw-   0        0        0      885 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/boolobject.h
--rw-rw-rw-   0        0        0     1484 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/bytearrayobject.h
--rw-rw-rw-   0        0        0     3048 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/bytesobject.h
--rw-rw-rw-   0        0        0      712 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cellobject.h
--rw-rw-rw-   0        0        0     5954 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/ceval.h
--rw-rw-rw-   0        0        0     1657 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/classobject.h
--rw-rw-rw-   0        0        0      318 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/code.h
--rw-rw-rw-   0        0        0     6793 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/codecs.h
--rw-rw-rw-   0        0        0     3778 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/compile.h
--rw-rw-rw-   0        0        0     1806 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/complexobject.h
--rw-rw-rw-   0        0        0     1962 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/context.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:14.956601 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/
--rw-rw-rw-   0        0        0    14200 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/abstract.h
--rw-rw-rw-   0        0        0      769 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h
--rw-rw-rw-   0        0        0     4114 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/bytesobject.h
--rw-rw-rw-   0        0        0     1537 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/ceval.h
--rw-rw-rw-   0        0        0     6989 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/code.h
--rw-rw-rw-   0        0        0     3797 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/dictobject.h
--rw-rw-rw-   0        0        0      721 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/fileobject.h
--rw-rw-rw-   0        0        0     4004 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/fileutils.h
--rw-rw-rw-   0        0        0     3059 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/frameobject.h
--rw-rw-rw-   0        0        0     1473 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/import.h
--rw-rw-rw-   0        0        0    16979 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/initconfig.h
--rw-rw-rw-   0        0        0      456 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/interpreteridobject.h
--rw-rw-rw-   0        0        0     1364 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/listobject.h
--rw-rw-rw-   0        0        0     1399 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/methodobject.h
--rw-rw-rw-   0        0        0    19358 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/object.h
--rw-rw-rw-   0        0        0     4456 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/objimpl.h
--rw-rw-rw-   0        0        0     5101 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pyerrors.h
--rw-rw-rw-   0        0        0     2096 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pylifecycle.h
--rw-rw-rw-   0        0        0     3511 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pymem.h
--rw-rw-rw-   0        0        0    10134 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pystate.h
--rw-rw-rw-   0        0        0      575 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/sysmodule.h
--rw-rw-rw-   0        0        0      473 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/traceback.h
--rw-rw-rw-   0        0        0     1036 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/tupleobject.h
--rw-rw-rw-   0        0        0    46154 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/unicodeobject.h
--rw-rw-rw-   0        0        0     9255 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/datetime.h
--rw-rw-rw-   0        0        0     3019 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/descrobject.h
--rw-rw-rw-   0        0        0     3715 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/dictobject.h
--rw-rw-rw-   0        0        0    22469 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/dynamic_annotations.h
--rw-rw-rw-   0        0        0      253 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/enumobject.h
--rw-rw-rw-   0        0        0     1624 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/errcode.h
--rw-rw-rw-   0        0        0     1209 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/eval.h
--rw-rw-rw-   0        0        0     1098 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/exports.h
--rw-rw-rw-   0        0        0     1571 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/fileobject.h
--rw-rw-rw-   0        0        0      597 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/fileutils.h
--rw-rw-rw-   0        0        0     4360 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/floatobject.h
--rw-rw-rw-   0        0        0      337 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/frameobject.h
--rw-rw-rw-   0        0        0     4057 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/funcobject.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/genericaliasobject.h
--rw-rw-rw-   0        0        0     3525 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/genobject.h
--rw-rw-rw-   0        0        0     2118 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/graminit.h
--rw-rw-rw-   0        0        0     1821 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/grammar.h
--rw-rw-rw-   0        0        0     3026 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/import.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:15.454926 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/
--rw-rw-rw-   0        0        0      953 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pegen_interface.h
--rw-rw-rw-   0        0        0      479 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_abstract.h
--rw-rw-rw-   0        0        0     1126 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_accu.h
--rw-rw-rw-   0        0        0    16979 2023-05-22 11:21:15.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_atomic.h
--rw-rw-rw-   0        0        0     3384 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
--rw-rw-rw-   0        0        0     2620 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h
--rw-rw-rw-   0        0        0      870 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_call.h
--rw-rw-rw-   0        0        0     3403 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_ceval.h
--rw-rw-rw-   0        0        0      541 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_code.h
--rw-rw-rw-   0        0        0     2809 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_condvar.h
--rw-rw-rw-   0        0        0      800 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_context.h
--rw-rw-rw-   0        0        0      646 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h
--rw-rw-rw-   0        0        0     1541 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h
--rw-rw-rw-   0        0        0     6647 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_gc.h
--rw-rw-rw-   0        0        0      490 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_getopt.h
--rw-rw-rw-   0        0        0     1565 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_gil.h
--rw-rw-rw-   0        0        0     3697 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_hamt.h
--rw-rw-rw-   0        0        0     4197 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h
--rw-rw-rw-   0        0        0      473 2023-05-22 11:21:03.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_import.h
--rw-rw-rw-   0        0        0     5233 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h
--rw-rw-rw-   0        0        0     5299 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_interp.h
--rw-rw-rw-   0        0        0     1548 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_long.h
--rw-rw-rw-   0        0        0     4157 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_object.h
--rw-rw-rw-   0        0        0     1936 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
--rw-rw-rw-   0        0        0     2032 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
--rw-rw-rw-   0        0        0      206 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pyhash.h
--rw-rw-rw-   0        0        0     3741 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
--rw-rw-rw-   0        0        0     3363 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pymem.h
--rw-rw-rw-   0        0        0     3583 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pystate.h
--rw-rw-rw-   0        0        0     4452 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_runtime.h
--rw-rw-rw-   0        0        0      548 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
--rw-rw-rw-   0        0        0     3056 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_traceback.h
--rw-rw-rw-   0        0        0      442 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
--rw-rw-rw-   0        0        0      633 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_warnings.h
--rw-rw-rw-   0        0        0      334 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/interpreteridobject.h
--rw-rw-rw-   0        0        0      861 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/intrcheck.h
--rw-rw-rw-   0        0        0      521 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/iterobject.h
--rw-rw-rw-   0        0        0     1781 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/listobject.h
--rw-rw-rw-   0        0        0     3799 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/longintrepr.h
--rw-rw-rw-   0        0        0     9513 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/longobject.h
--rw-rw-rw-   0        0        0      803 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/marshal.h
--rw-rw-rw-   0        0        0     2764 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/memoryobject.h
--rw-rw-rw-   0        0        0     3775 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/methodobject.h
--rw-rw-rw-   0        0        0     9959 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/modsupport.h
--rw-rw-rw-   0        0        0     2361 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/moduleobject.h
--rw-rw-rw-   0        0        0      349 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/namespaceobject.h
--rw-rw-rw-   0        0        0     1281 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/node.h
--rw-rw-rw-   0        0        0    24628 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/object.h
--rw-rw-rw-   0        0        0     8423 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/objimpl.h
--rw-rw-rw-   0        0        0     1299 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/odictobject.h
--rw-rw-rw-   0        0        0     4900 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/opcode.h
--rw-rw-rw-   0        0        0      737 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/osdefs.h
--rw-rw-rw-   0        0        0      291 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/osmodule.h
--rw-rw-rw-   0        0        0     2958 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/parsetok.h
--rw-rw-rw-   0        0        0     1300 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/patchlevel.h
--rw-rw-rw-   0        0        0      846 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/picklebufobject.h
--rw-rw-rw-   0        0        0     2474 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/py_curses.h
--rw-rw-rw-   0        0        0     2744 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyarena.h
--rw-rw-rw-   0        0        0     1725 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pycapsule.h
--rw-rw-rw-   0        0        0     1387 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyctype.h
--rw-rw-rw-   0        0        0     1093 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydebug.h
--rw-rw-rw-   0        0        0     1008 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydtrace.d
--rw-rw-rw-   0        0        0     2413 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydtrace.h
--rw-rw-rw-   0        0        0    12427 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyerrors.h
--rw-rw-rw-   0        0        0     2450 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyexpat.h
--rw-rw-rw-   0        0        0      444 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyfpe.h
--rw-rw-rw-   0        0        0      466 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyframe.h
--rw-rw-rw-   0        0        0     4263 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyhash.h
--rw-rw-rw-   0        0        0     2136 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pylifecycle.h
--rw-rw-rw-   0        0        0     2989 2022-10-10 14:14:21.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymacconfig.h
--rw-rw-rw-   0        0        0     4920 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymacro.h
--rw-rw-rw-   0        0        0     8582 2023-05-22 11:21:15.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymath.h
--rw-rw-rw-   0        0        0     4406 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymem.h
--rw-rw-rw-   0        0        0    31277 2023-05-22 11:21:15.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyport.h
--rw-rw-rw-   0        0        0     5250 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystate.h
--rw-rw-rw-   0        0        0      436 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystrcmp.h
--rw-rw-rw-   0        0        0      849 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystrhex.h
--rw-rw-rw-   0        0        0     1483 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystrtod.h
--rw-rw-rw-   0        0        0     7673 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pythonrun.h
--rw-rw-rw-   0        0        0     5938 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pythread.h
--rw-rw-rw-   0        0        0     8930 2023-05-22 11:21:15.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/pytime.h
--rw-rw-rw-   0        0        0      628 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/rangeobject.h
--rw-rw-rw-   0        0        0     3324 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/setobject.h
--rw-rw-rw-   0        0        0     2516 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/sliceobject.h
--rw-rw-rw-   0        0        0     2030 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/structmember.h
--rw-rw-rw-   0        0        0     1390 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/structseq.h
--rw-rw-rw-   0        0        0     5307 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/symtable.h
--rw-rw-rw-   0        0        0     1242 2023-05-22 11:20:45.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/sysmodule.h
--rw-rw-rw-   0        0        0     2642 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/token.h
--rw-rw-rw-   0        0        0      584 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/traceback.h
--rw-rw-rw-   0        0        0     1114 2022-10-10 14:12:36.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/tracemalloc.h
--rw-rw-rw-   0        0        0     1614 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/tupleobject.h
--rw-rw-rw-   0        0        0     2350 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/typeslots.h
--rw-rw-rw-   0        0        0     1056 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/ucnhash.h
--rw-rw-rw-   0        0        0    35426 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/unicodeobject.h
--rw-rw-rw-   0        0        0     1776 2023-05-22 11:20:46.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/warnings.h
--rw-rw-rw-   0        0        0     2863 2023-05-22 11:21:04.000000 wasmpy-build-0.2.1/wasmpy_build/include/cp39/weakrefobject.h
-drwxrwxrwx   0        0        0        0 2023-05-22 11:37:10.996984 wasmpy-build-0.2.1/wasmpy_build.egg-info/
--rw-rw-rw-   0        0        0     1863 2023-05-22 11:37:10.000000 wasmpy-build-0.2.1/wasmpy_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    28738 2023-05-22 11:37:10.000000 wasmpy-build-0.2.1/wasmpy_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 11:37:10.000000 wasmpy-build-0.2.1/wasmpy_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-22 11:37:10.000000 wasmpy-build-0.2.1/wasmpy_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 11:37:10.000000 wasmpy-build-0.2.1/wasmpy_build.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.555275 wasmpy-build-0.3.0/
+-rw-rw-rw-   0        0        0     1068 2023-07-13 01:09:54.000000 wasmpy-build-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1560 2023-07-13 01:15:53.554274 wasmpy-build-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2023-07-13 01:11:51.000000 wasmpy-build-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 01:15:53.555275 wasmpy-build-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2023-07-13 01:15:38.000000 wasmpy-build-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.254963 wasmpy-build-0.3.0/wasmpy_build/
+-rw-rw-rw-   0        0        0     2231 2023-07-13 01:13:45.000000 wasmpy-build-0.3.0/wasmpy_build/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 01:13:42.000000 wasmpy-build-0.3.0/wasmpy_build/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.229405 wasmpy-build-0.3.0/wasmpy_build/include/
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.416182 wasmpy-build-0.3.0/wasmpy_build/include/cp310/
+-rw-rw-rw-   0        0        0    13936 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/LICENSE
+-rw-rw-rw-   0        0        0     3226 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/Python.h
+-rw-rw-rw-   0        0        0      344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/README.rst
+-rw-rw-rw-   0        0        0    31405 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/bltinmodule.h
+-rw-rw-rw-   0        0        0     1224 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/bytesobject.h
+-rw-rw-rw-   0        0        0      720 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cellobject.h
+-rw-rw-rw-   0        0        0     5703 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/code.h
+-rw-rw-rw-   0        0        0     7071 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/context.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.464854 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/
+-rw-rw-rw-   0        0        0    14054 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4119 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1468 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/ceval.h
+-rw-rw-rw-   0        0        0     7570 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/compile.h
+-rw-rw-rw-   0        0        0     3734 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      723 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4267 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3152 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1630 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/import.h
+-rw-rw-rw-   0        0        0     7597 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1243 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19613 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/object.h
+-rw-rw-rw-   0        0        0     3356 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     5476 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0     2095 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pymem.h
+-rw-rw-rw-   0        0        0    11914 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     9196 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pytime.h
+-rw-rw-rw-   0        0        0      506 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      404 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/traceback.h
+-rw-rw-rw-   0        0        0      975 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    44284 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9635 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/datetime.h
+-rw-rw-rw-   0        0        0     3002 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/descrobject.h
+-rw-rw-rw-   0        0        0     3853 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/errcode.h
+-rw-rw-rw-   0        0        0      831 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/fileobject.h
+-rw-rw-rw-   0        0        0      508 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/frameobject.h
+-rw-rw-rw-   0        0        0     4257 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3347 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/genobject.h
+-rw-rw-rw-   0        0        0     3026 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/import.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.535778 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/
+-rw-rw-rw-   0        0        0      479 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     2971 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    28828 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6457 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16981 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     5271 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0      870 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3484 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      696 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2809 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      822 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1704 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      480 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     6859 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      346 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5625 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     9289 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      350 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     2589 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1047 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0     5989 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_object.h
+-rw-rw-rw-   0        0        0      626 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0     1981 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2314 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     4940 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3211 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3938 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4902 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      386 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5578 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      548 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     2970 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      425 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0      898 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0      629 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      633 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/interpreteridobject.h
+-rw-rw-rw-   0        0        0      772 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/longintrepr.h
+-rw-rw-rw-   0        0        0     8606 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/memoryobject.h
+-rw-rw-rw-   0        0        0     4147 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/methodobject.h
+-rw-rw-rw-   0        0        0    10333 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/modsupport.h
+-rw-rw-rw-   0        0        0     2458 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/namespaceobject.h
+-rw-rw-rw-   0        0        0    28344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/object.h
+-rw-rw-rw-   0        0        0     8445 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/objimpl.h
+-rw-rw-rw-   0        0        0     5509 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/osmodule.h
+-rw-rw-rw-   0        0        0     1302 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/patchlevel.h
+-rw-rw-rw-   0        0        0     2474 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/py_curses.h
+-rw-rw-rw-   0        0        0     1725 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pycapsule.h
+-rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pydtrace.h
+-rw-rw-rw-   0        0        0    12426 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyexpat.h
+-rw-rw-rw-   0        0        0      466 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyframe.h
+-rw-rw-rw-   0        0        0     4223 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyhash.h
+-rw-rw-rw-   0        0        0     2080 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymacro.h
+-rw-rw-rw-   0        0        0     8315 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymath.h
+-rw-rw-rw-   0        0        0     3891 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymem.h
+-rw-rw-rw-   0        0        0    31688 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystrtod.h
+-rw-rw-rw-   0        0        0     1110 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/pythread.h
+-rw-rw-rw-   0        0        0      628 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/rangeobject.h
+-rw-rw-rw-   0        0        0     3381 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/sliceobject.h
+-rw-rw-rw-   0        0        0     2074 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/structseq.h
+-rw-rw-rw-   0        0        0     1242 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/token.h
+-rw-rw-rw-   0        0        0      584 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/tupleobject.h
+-rw-rw-rw-   0        0        0     2460 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/typeslots.h
+-rw-rw-rw-   0        0        0    36148 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-05-29 09:08:23.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp310/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.639303 wasmpy-build-0.3.0/wasmpy_build/include/cp311/
+-rw-rw-rw-   0        0        0    13936 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/LICENSE
+-rw-rw-rw-   0        0        0     2856 2023-05-29 09:11:37.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/Python.h
+-rw-rw-rw-   0        0        0      344 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/README.rst
+-rw-rw-rw-   0        0        0    31404 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/abstract.h
+-rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/bltinmodule.h
+-rw-rw-rw-   0        0        0     1212 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/boolobject.h
+-rw-rw-rw-   0        0        0     1462 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/bytearrayobject.h
+-rw-rw-rw-   0        0        0     2617 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/bytesobject.h
+-rw-rw-rw-   0        0        0     6255 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/ceval.h
+-rw-rw-rw-   0        0        0     7071 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/codecs.h
+-rw-rw-rw-   0        0        0      520 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/compile.h
+-rw-rw-rw-   0        0        0      724 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/complexobject.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.707055 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/
+-rw-rw-rw-   0        0        0     8229 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/abstract.h
+-rw-rw-rw-   0        0        0     1305 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4568 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0      723 2023-05-29 09:11:33.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/cellobject.h
+-rw-rw-rw-   0        0        0     1239 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/ceval.h
+-rw-rw-rw-   0        0        0     1656 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/classobject.h
+-rw-rw-rw-   0        0        0    11484 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/code.h
+-rw-rw-rw-   0        0        0     2218 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/compile.h
+-rw-rw-rw-   0        0        0     1248 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/complexobject.h
+-rw-rw-rw-   0        0        0     1959 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/context.h
+-rw-rw-rw-   0        0        0     1642 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/descrobject.h
+-rw-rw-rw-   0        0        0     3324 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      818 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/fileobject.h
+-rw-rw-rw-   0        0        0      232 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/fileutils.h
+-rw-rw-rw-   0        0        0      702 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/floatobject.h
+-rw-rw-rw-   0        0        0     1108 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     4424 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/funcobject.h
+-rw-rw-rw-   0        0        0     3279 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/genobject.h
+-rw-rw-rw-   0        0        0     1526 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/import.h
+-rw-rw-rw-   0        0        0     7817 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/initconfig.h
+-rw-rw-rw-   0        0        0     1769 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/listobject.h
+-rw-rw-rw-   0        0        0     3817 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/longintrepr.h
+-rw-rw-rw-   0        0        0     4532 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/longobject.h
+-rw-rw-rw-   0        0        0     2556 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/methodobject.h
+-rw-rw-rw-   0        0        0     4234 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/modsupport.h
+-rw-rw-rw-   0        0        0    18305 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/object.h
+-rw-rw-rw-   0        0        0     2998 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/odictobject.h
+-rw-rw-rw-   0        0        0      846 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/picklebufobject.h
+-rw-rw-rw-   0        0        0     3505 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pthread_stubs.h
+-rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyctype.h
+-rw-rw-rw-   0        0        0     1073 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pydebug.h
+-rw-rw-rw-   0        0        0     4522 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0      444 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyfpe.h
+-rw-rw-rw-   0        0        0      582 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyframe.h
+-rw-rw-rw-   0        0        0     2099 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3379 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pymem.h
+-rw-rw-rw-   0        0        0    14351 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pystate.h
+-rw-rw-rw-   0        0        0     4811 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pythonrun.h
+-rw-rw-rw-   0        0        0     1426 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pythread.h
+-rw-rw-rw-   0        0        0    12158 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pytime.h
+-rw-rw-rw-   0        0        0     1997 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/setobject.h
+-rw-rw-rw-   0        0        0      489 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      444 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1513 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    41910 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0      560 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/warnings.h
+-rw-rw-rw-   0        0        0     2103 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/weakrefobject.h
+-rw-rw-rw-   0        0        0     9635 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/datetime.h
+-rw-rw-rw-   0        0        0     1256 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/descrobject.h
+-rw-rw-rw-   0        0        0     3852 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/dictobject.h
+-rw-rw-rw-   0        0        0    22471 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/enumobject.h
+-rw-rw-rw-   0        0        0     1700 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/errcode.h
+-rw-rw-rw-   0        0        0     1098 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/exports.h
+-rw-rw-rw-   0        0        0     1570 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/fileobject.h
+-rw-rw-rw-   0        0        0      507 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/fileutils.h
+-rw-rw-rw-   0        0        0     1530 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/floatobject.h
+-rw-rw-rw-   0        0        0      336 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/frameobject.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3025 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/import.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.816367 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/
+-rw-rw-rw-   0        0        0      611 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0     3031 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_asdl.h
+-rw-rw-rw-   0        0        0    29315 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ast.h
+-rw-rw-rw-   0        0        0     6535 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ast_state.h
+-rw-rw-rw-   0        0        0    16981 2023-05-29 09:11:37.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     2438 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h
+-rw-rw-rw-   0        0        0     6062 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bitutils.h
+-rw-rw-rw-   0        0        0     8688 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h
+-rw-rw-rw-   0        0        0     3384 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     1424 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bytesobject.h
+-rw-rw-rw-   0        0        0     3475 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     4409 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0    15930 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     1045 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_compile.h
+-rw-rw-rw-   0        0        0     2839 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0     1239 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     5684 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_dict.h
+-rw-rw-rw-   0        0        0      704 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0      562 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h
+-rw-rw-rw-   0        0        0      842 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_exceptions.h
+-rw-rw-rw-   0        0        0     7313 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     1307 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_floatobject.h
+-rw-rw-rw-   0        0        0      480 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_format.h
+-rw-rw-rw-   0        0        0     7567 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_frame.h
+-rw-rw-rw-   0        0        0      413 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_function.h
+-rw-rw-rw-   0        0        0     6895 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0     1164 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_genobject.h
+-rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     1436 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_global_objects.h
+-rw-rw-rw-   0        0        0    12980 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_global_strings.h
+-rw-rw-rw-   0        0        0     3696 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      743 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5800 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     6671 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0      562 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h
+-rw-rw-rw-   0        0        0     1352 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_list.h
+-rw-rw-rw-   0        0        0     3516 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     1040 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_moduleobject.h
+-rw-rw-rw-   0        0        0      392 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_namespace.h
+-rw-rw-rw-   0        0        0    10037 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_object.h
+-rw-rw-rw-   0        0        0    18986 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_opcode.h
+-rw-rw-rw-   0        0        0      626 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_parser.h
+-rw-rw-rw-   0        0        0      606 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2733 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pyarena.h
+-rw-rw-rw-   0        0        0     2494 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3507 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     9435 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pymath.h
+-rw-rw-rw-   0        0        0     3708 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     4107 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     5988 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0    49092 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_runtime_init.h
+-rw-rw-rw-   0        0        0      937 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_signal.h
+-rw-rw-rw-   0        0        0      336 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_sliceobject.h
+-rw-rw-rw-   0        0        0      937 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_strhex.h
+-rw-rw-rw-   0        0        0      580 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_structseq.h
+-rw-rw-rw-   0        0        0     5638 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_symtable.h
+-rw-rw-rw-   0        0        0      605 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3501 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0     2089 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_tuple.h
+-rw-rw-rw-   0        0        0     1158 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_typeobject.h
+-rw-rw-rw-   0        0        0      898 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ucnhash.h
+-rw-rw-rw-   0        0        0     1716 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h
+-rw-rw-rw-   0        0        0      678 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_unionobject.h
+-rw-rw-rw-   0        0        0      740 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      772 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/intrcheck.h
+-rw-rw-rw-   0        0        0      593 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/iterobject.h
+-rw-rw-rw-   0        0        0     1780 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/listobject.h
+-rw-rw-rw-   0        0        0     3272 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/longobject.h
+-rw-rw-rw-   0        0        0      827 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/marshal.h
+-rw-rw-rw-   0        0        0     2810 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/memoryobject.h
+-rw-rw-rw-   0        0        0     5072 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/methodobject.h
+-rw-rw-rw-   0        0        0     6448 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/modsupport.h
+-rw-rw-rw-   0        0        0     2374 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/moduleobject.h
+-rw-rw-rw-   0        0        0    29800 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/object.h
+-rw-rw-rw-   0        0        0     8428 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/objimpl.h
+-rw-rw-rw-   0        0        0    11187 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/osmodule.h
+-rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/patchlevel.h
+-rw-rw-rw-   0        0        0     2471 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/py_curses.h
+-rw-rw-rw-   0        0        0     5115 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pybuffer.h
+-rw-rw-rw-   0        0        0     1725 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pycapsule.h
+-rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pydtrace.h
+-rw-rw-rw-   0        0        0    12782 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyexpat.h
+-rw-rw-rw-   0        0        0      551 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyframe.h
+-rw-rw-rw-   0        0        0     4154 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyhash.h
+-rw-rw-rw-   0        0        0     2249 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymacconfig.h
+-rw-rw-rw-   0        0        0     6064 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymacro.h
+-rw-rw-rw-   0        0        0     1979 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymath.h
+-rw-rw-rw-   0        0        0     3890 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymem.h
+-rw-rw-rw-   0        0        0    24532 2023-05-29 09:11:37.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyport.h
+-rw-rw-rw-   0        0        0     4635 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pystrcmp.h
+-rw-rw-rw-   0        0        0     1557 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pystrtod.h
+-rw-rw-rw-   0        0        0     1189 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pythonrun.h
+-rw-rw-rw-   0        0        0     4833 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pythread.h
+-rw-rw-rw-   0        0        0      851 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/pytypedefs.h
+-rw-rw-rw-   0        0        0      628 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/rangeobject.h
+-rw-rw-rw-   0        0        0     1543 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-05-29 09:08:27.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/sliceobject.h
+-rw-rw-rw-   0        0        0     2040 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/structmember.h
+-rw-rw-rw-   0        0        0     1388 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/structseq.h
+-rw-rw-rw-   0        0        0     1381 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/sysmodule.h
+-rw-rw-rw-   0        0        0     2669 2023-05-29 09:11:30.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/token.h
+-rw-rw-rw-   0        0        0      583 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/tracemalloc.h
+-rw-rw-rw-   0        0        0     1613 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/tupleobject.h
+-rw-rw-rw-   0        0        0     2342 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/typeslots.h
+-rw-rw-rw-   0        0        0    36032 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/unicodeobject.h
+-rw-rw-rw-   0        0        0     1129 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/warnings.h
+-rw-rw-rw-   0        0        0     1226 2023-05-29 09:11:34.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp311/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.046104 wasmpy-build-0.3.0/wasmpy_build/include/cp38/
+-rw-rw-rw-   0        0        0    13937 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/LICENSE
+-rw-rw-rw-   0        0        0    26491 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/Python-ast.h
+-rw-rw-rw-   0        0        0     3617 2023-05-29 09:11:43.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/Python.h
+-rw-rw-rw-   0        0        0    30286 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/abstract.h
+-rw-rw-rw-   0        0        0     1229 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/asdl.h
+-rw-rw-rw-   0        0        0      948 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/ast.h
+-rw-rw-rw-   0        0        0      468 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/bltinmodule.h
+-rw-rw-rw-   0        0        0      886 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/boolobject.h
+-rw-rw-rw-   0        0        0     2114 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3301 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytes_methods.h
+-rw-rw-rw-   0        0        0     8493 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytesobject.h
+-rw-rw-rw-   0        0        0      713 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cellobject.h
+-rw-rw-rw-   0        0        0     8366 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/ceval.h
+-rw-rw-rw-   0        0        0     1710 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/classobject.h
+-rw-rw-rw-   0        0        0     7178 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/code.h
+-rw-rw-rw-   0        0        0     6793 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/codecs.h
+-rw-rw-rw-   0        0        0     3582 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/compile.h
+-rw-rw-rw-   0        0        0     1807 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/complexobject.h
+-rw-rw-rw-   0        0        0     2014 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/context.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.089619 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/
+-rw-rw-rw-   0        0        0    12294 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/abstract.h
+-rw-rw-rw-   0        0        0     3845 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/fileobject.h
+-rw-rw-rw-   0        0        0    16028 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0    15691 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/object.h
+-rw-rw-rw-   0        0        0     3600 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     4717 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2263 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pymem.h
+-rw-rw-rw-   0        0        0     9810 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pystate.h
+-rw-rw-rw-   0        0        0      547 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46308 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9260 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/descrobject.h
+-rw-rw-rw-   0        0        0     3716 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/dictobject.h
+-rw-rw-rw-   0        0        0      458 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/dtoa.h
+-rw-rw-rw-   0        0        0    22469 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/enumobject.h
+-rw-rw-rw-   0        0        0     1695 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/eval.h
+-rw-rw-rw-   0        0        0     1571 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/fileobject.h
+-rw-rw-rw-   0        0        0     4352 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/fileutils.h
+-rw-rw-rw-   0        0        0     4794 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/floatobject.h
+-rw-rw-rw-   0        0        0     3317 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/frameobject.h
+-rw-rw-rw-   0        0        0     4200 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/funcobject.h
+-rw-rw-rw-   0        0        0     3720 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/grammar.h
+-rw-rw-rw-   0        0        0     4926 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/import.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.153622 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/
+-rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16946 2023-05-29 09:11:43.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0      966 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      542 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      779 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_context.h
+-rw-rw-rw-   0        0        0     1254 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1520 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3698 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     5218 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     1548 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     2896 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     2037 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     1329 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3815 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     8217 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     9588 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     3076 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      418 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      591 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/intrcheck.h
+-rw-rw-rw-   0        0        0      567 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/iterobject.h
+-rw-rw-rw-   0        0        0     2927 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/longintrepr.h
+-rw-rw-rw-   0        0        0     9520 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/marshal.h
+-rw-rw-rw-   0        0        0     2765 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/memoryobject.h
+-rw-rw-rw-   0        0        0     4406 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/methodobject.h
+-rw-rw-rw-   0        0        0     9591 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/modsupport.h
+-rw-rw-rw-   0        0        0     2362 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/namespaceobject.h
+-rw-rw-rw-   0        0        0     1328 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/node.h
+-rw-rw-rw-   0        0        0    29599 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/object.h
+-rw-rw-rw-   0        0        0    10537 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/objimpl.h
+-rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/odictobject.h
+-rw-rw-rw-   0        0        0     5164 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/patchlevel.h
+-rw-rw-rw-   0        0        0      847 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/picklebufobject.h
+-rw-rw-rw-   0        0        0     2477 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyarena.h
+-rw-rw-rw-   0        0        0     1726 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pycapsule.h
+-rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyctype.h
+-rw-rw-rw-   0        0        0     1214 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydtrace.h
+-rw-rw-rw-   0        0        0    12786 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyexpat.h
+-rw-rw-rw-   0        0        0      341 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyfpe.h
+-rw-rw-rw-   0        0        0     4140 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyhash.h
+-rw-rw-rw-   0        0        0     2081 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymacconfig.h
+-rw-rw-rw-   0        0        0     3778 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymacro.h
+-rw-rw-rw-   0        0        0     8314 2023-05-29 09:11:43.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymath.h
+-rw-rw-rw-   0        0        0     5406 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymem.h
+-rw-rw-rw-   0        0        0    30225 2023-05-29 09:11:43.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyport.h
+-rw-rw-rw-   0        0        0     4686 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystrtod.h
+-rw-rw-rw-   0        0        0     7645 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pythonrun.h
+-rw-rw-rw-   0        0        0     5660 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pythread.h
+-rw-rw-rw-   0        0        0     8928 2023-05-29 09:11:43.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/pytime.h
+-rw-rw-rw-   0        0        0      629 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/rangeobject.h
+-rw-rw-rw-   0        0        0     3362 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/setobject.h
+-rw-rw-rw-   0        0        0     2517 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/structmember.h
+-rw-rw-rw-   0        0        0     1377 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/structseq.h
+-rw-rw-rw-   0        0        0     5308 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/sysmodule.h
+-rw-rw-rw-   0        0        0     2429 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/token.h
+-rw-rw-rw-   0        0        0      601 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/tracemalloc.h
+-rw-rw-rw-   0        0        0     1661 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/tupleobject.h
+-rw-rw-rw-   0        0        0     2253 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/ucnhash.h
+-rw-rw-rw-   0        0        0    35732 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/warnings.h
+-rw-rw-rw-   0        0        0     2866 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp38/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.402747 wasmpy-build-0.3.0/wasmpy_build/include/cp39/
+-rw-rw-rw-   0        0        0    13937 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/LICENSE
+-rw-rw-rw-   0        0        0    26193 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/Python-ast.h
+-rw-rw-rw-   0        0        0     3534 2023-05-29 09:11:47.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/Python.h
+-rw-rw-rw-   0        0        0    30476 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/abstract.h
+-rw-rw-rw-   0        0        0     1224 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/asdl.h
+-rw-rw-rw-   0        0        0      947 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/ast.h
+-rw-rw-rw-   0        0        0      468 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/bitset.h
+-rw-rw-rw-   0        0        0      264 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/bltinmodule.h
+-rw-rw-rw-   0        0        0      885 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/boolobject.h
+-rw-rw-rw-   0        0        0     1484 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/bytearrayobject.h
+-rw-rw-rw-   0        0        0     3048 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/bytesobject.h
+-rw-rw-rw-   0        0        0      712 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cellobject.h
+-rw-rw-rw-   0        0        0     5954 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/ceval.h
+-rw-rw-rw-   0        0        0     1657 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/classobject.h
+-rw-rw-rw-   0        0        0      318 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/code.h
+-rw-rw-rw-   0        0        0     6793 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/codecs.h
+-rw-rw-rw-   0        0        0     3778 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/compile.h
+-rw-rw-rw-   0        0        0     1806 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/complexobject.h
+-rw-rw-rw-   0        0        0     1962 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/context.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.455752 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/
+-rw-rw-rw-   0        0        0    14200 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/abstract.h
+-rw-rw-rw-   0        0        0      769 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/bytearrayobject.h
+-rw-rw-rw-   0        0        0     4114 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/bytesobject.h
+-rw-rw-rw-   0        0        0     1537 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/ceval.h
+-rw-rw-rw-   0        0        0     6989 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/code.h
+-rw-rw-rw-   0        0        0     3797 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/dictobject.h
+-rw-rw-rw-   0        0        0      721 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/fileobject.h
+-rw-rw-rw-   0        0        0     4004 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/fileutils.h
+-rw-rw-rw-   0        0        0     3059 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/frameobject.h
+-rw-rw-rw-   0        0        0     1473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/import.h
+-rw-rw-rw-   0        0        0    16979 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/initconfig.h
+-rw-rw-rw-   0        0        0      456 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/interpreteridobject.h
+-rw-rw-rw-   0        0        0     1364 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/listobject.h
+-rw-rw-rw-   0        0        0     1399 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/methodobject.h
+-rw-rw-rw-   0        0        0    19358 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/object.h
+-rw-rw-rw-   0        0        0     4456 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/objimpl.h
+-rw-rw-rw-   0        0        0     5101 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pyerrors.h
+-rw-rw-rw-   0        0        0     2096 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pylifecycle.h
+-rw-rw-rw-   0        0        0     3511 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pymem.h
+-rw-rw-rw-   0        0        0    10134 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pystate.h
+-rw-rw-rw-   0        0        0      575 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/sysmodule.h
+-rw-rw-rw-   0        0        0      473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/traceback.h
+-rw-rw-rw-   0        0        0     1036 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/tupleobject.h
+-rw-rw-rw-   0        0        0    46154 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/unicodeobject.h
+-rw-rw-rw-   0        0        0     9255 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/datetime.h
+-rw-rw-rw-   0        0        0     3019 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/descrobject.h
+-rw-rw-rw-   0        0        0     3715 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/dictobject.h
+-rw-rw-rw-   0        0        0    22469 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/dynamic_annotations.h
+-rw-rw-rw-   0        0        0      253 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/enumobject.h
+-rw-rw-rw-   0        0        0     1624 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/errcode.h
+-rw-rw-rw-   0        0        0     1209 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/eval.h
+-rw-rw-rw-   0        0        0     1098 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/exports.h
+-rw-rw-rw-   0        0        0     1571 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/fileobject.h
+-rw-rw-rw-   0        0        0      597 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/fileutils.h
+-rw-rw-rw-   0        0        0     4360 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/floatobject.h
+-rw-rw-rw-   0        0        0      337 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/frameobject.h
+-rw-rw-rw-   0        0        0     4057 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/funcobject.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/genericaliasobject.h
+-rw-rw-rw-   0        0        0     3525 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/genobject.h
+-rw-rw-rw-   0        0        0     2118 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/graminit.h
+-rw-rw-rw-   0        0        0     1821 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/grammar.h
+-rw-rw-rw-   0        0        0     3026 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/import.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:53.551268 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/
+-rw-rw-rw-   0        0        0      953 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pegen_interface.h
+-rw-rw-rw-   0        0        0      479 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_abstract.h
+-rw-rw-rw-   0        0        0     1126 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_accu.h
+-rw-rw-rw-   0        0        0    16979 2023-05-29 09:11:47.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_atomic.h
+-rw-rw-rw-   0        0        0     3384 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h
+-rw-rw-rw-   0        0        0     2620 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_byteswap.h
+-rw-rw-rw-   0        0        0      870 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_call.h
+-rw-rw-rw-   0        0        0     3403 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_ceval.h
+-rw-rw-rw-   0        0        0      541 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_code.h
+-rw-rw-rw-   0        0        0     2809 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_condvar.h
+-rw-rw-rw-   0        0        0      800 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_context.h
+-rw-rw-rw-   0        0        0      646 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_dtoa.h
+-rw-rw-rw-   0        0        0     1541 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_fileutils.h
+-rw-rw-rw-   0        0        0     6647 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_gc.h
+-rw-rw-rw-   0        0        0      490 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_getopt.h
+-rw-rw-rw-   0        0        0     1565 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_gil.h
+-rw-rw-rw-   0        0        0     3697 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_hamt.h
+-rw-rw-rw-   0        0        0     4197 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_hashtable.h
+-rw-rw-rw-   0        0        0      473 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_import.h
+-rw-rw-rw-   0        0        0     5233 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_initconfig.h
+-rw-rw-rw-   0        0        0     5299 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_interp.h
+-rw-rw-rw-   0        0        0     1548 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_long.h
+-rw-rw-rw-   0        0        0     4157 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_object.h
+-rw-rw-rw-   0        0        0     1936 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pathconfig.h
+-rw-rw-rw-   0        0        0     2032 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pyerrors.h
+-rw-rw-rw-   0        0        0      206 2023-05-22 18:44:20.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pyhash.h
+-rw-rw-rw-   0        0        0     3741 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h
+-rw-rw-rw-   0        0        0     3363 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pymem.h
+-rw-rw-rw-   0        0        0     3583 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pystate.h
+-rw-rw-rw-   0        0        0     4452 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_runtime.h
+-rw-rw-rw-   0        0        0      548 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_sysmodule.h
+-rw-rw-rw-   0        0        0     3056 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_traceback.h
+-rw-rw-rw-   0        0        0      442 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_tupleobject.h
+-rw-rw-rw-   0        0        0      633 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_warnings.h
+-rw-rw-rw-   0        0        0      334 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/interpreteridobject.h
+-rw-rw-rw-   0        0        0      861 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/intrcheck.h
+-rw-rw-rw-   0        0        0      521 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/iterobject.h
+-rw-rw-rw-   0        0        0     1781 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/listobject.h
+-rw-rw-rw-   0        0        0     3799 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/longintrepr.h
+-rw-rw-rw-   0        0        0     9513 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/longobject.h
+-rw-rw-rw-   0        0        0      803 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/marshal.h
+-rw-rw-rw-   0        0        0     2764 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/memoryobject.h
+-rw-rw-rw-   0        0        0     3775 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/methodobject.h
+-rw-rw-rw-   0        0        0     9959 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/modsupport.h
+-rw-rw-rw-   0        0        0     2361 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/moduleobject.h
+-rw-rw-rw-   0        0        0      349 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/namespaceobject.h
+-rw-rw-rw-   0        0        0     1281 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/node.h
+-rw-rw-rw-   0        0        0    24628 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/object.h
+-rw-rw-rw-   0        0        0     8423 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/objimpl.h
+-rw-rw-rw-   0        0        0     1299 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/odictobject.h
+-rw-rw-rw-   0        0        0     4900 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/opcode.h
+-rw-rw-rw-   0        0        0      737 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/osdefs.h
+-rw-rw-rw-   0        0        0      291 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/osmodule.h
+-rw-rw-rw-   0        0        0     2958 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/parsetok.h
+-rw-rw-rw-   0        0        0     1300 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/patchlevel.h
+-rw-rw-rw-   0        0        0      846 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/picklebufobject.h
+-rw-rw-rw-   0        0        0     2474 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/py_curses.h
+-rw-rw-rw-   0        0        0     2744 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyarena.h
+-rw-rw-rw-   0        0        0     1725 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pycapsule.h
+-rw-rw-rw-   0        0        0     1387 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyctype.h
+-rw-rw-rw-   0        0        0     1093 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydebug.h
+-rw-rw-rw-   0        0        0     1008 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydtrace.d
+-rw-rw-rw-   0        0        0     2413 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydtrace.h
+-rw-rw-rw-   0        0        0    12427 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyerrors.h
+-rw-rw-rw-   0        0        0     2450 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyexpat.h
+-rw-rw-rw-   0        0        0      444 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyfpe.h
+-rw-rw-rw-   0        0        0      466 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyframe.h
+-rw-rw-rw-   0        0        0     4263 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyhash.h
+-rw-rw-rw-   0        0        0     2136 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pylifecycle.h
+-rw-rw-rw-   0        0        0     2989 2023-05-22 18:44:48.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymacconfig.h
+-rw-rw-rw-   0        0        0     4920 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymacro.h
+-rw-rw-rw-   0        0        0     8582 2023-05-29 09:11:47.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymath.h
+-rw-rw-rw-   0        0        0     4406 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymem.h
+-rw-rw-rw-   0        0        0    31277 2023-05-29 09:11:47.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyport.h
+-rw-rw-rw-   0        0        0     5250 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystate.h
+-rw-rw-rw-   0        0        0      436 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystrcmp.h
+-rw-rw-rw-   0        0        0      849 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystrhex.h
+-rw-rw-rw-   0        0        0     1483 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystrtod.h
+-rw-rw-rw-   0        0        0     7673 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pythonrun.h
+-rw-rw-rw-   0        0        0     5938 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pythread.h
+-rw-rw-rw-   0        0        0     8930 2023-05-29 09:11:47.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/pytime.h
+-rw-rw-rw-   0        0        0      628 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/rangeobject.h
+-rw-rw-rw-   0        0        0     3324 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/setobject.h
+-rw-rw-rw-   0        0        0     2516 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/sliceobject.h
+-rw-rw-rw-   0        0        0     2030 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/structmember.h
+-rw-rw-rw-   0        0        0     1390 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/structseq.h
+-rw-rw-rw-   0        0        0     5307 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/symtable.h
+-rw-rw-rw-   0        0        0     1242 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/sysmodule.h
+-rw-rw-rw-   0        0        0     2642 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/token.h
+-rw-rw-rw-   0        0        0      584 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/traceback.h
+-rw-rw-rw-   0        0        0     1114 2023-05-22 18:44:21.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/tracemalloc.h
+-rw-rw-rw-   0        0        0     1614 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/tupleobject.h
+-rw-rw-rw-   0        0        0     2350 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/typeslots.h
+-rw-rw-rw-   0        0        0     1056 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/ucnhash.h
+-rw-rw-rw-   0        0        0    35426 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/unicodeobject.h
+-rw-rw-rw-   0        0        0     1776 2023-05-29 09:11:38.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/warnings.h
+-rw-rw-rw-   0        0        0     2863 2023-05-29 09:11:44.000000 wasmpy-build-0.3.0/wasmpy_build/include/cp39/weakrefobject.h
+drwxrwxrwx   0        0        0        0 2023-07-13 01:15:52.283467 wasmpy-build-0.3.0/wasmpy_build.egg-info/
+-rw-rw-rw-   0        0        0     1560 2023-07-13 01:15:52.000000 wasmpy-build-0.3.0/wasmpy_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28738 2023-07-13 01:15:52.000000 wasmpy-build-0.3.0/wasmpy_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 01:15:52.000000 wasmpy-build-0.3.0/wasmpy_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-13 01:15:52.000000 wasmpy-build-0.3.0/wasmpy_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 01:15:52.000000 wasmpy-build-0.3.0/wasmpy_build.egg-info/top_level.txt
```

### Comparing `wasmpy-build-0.2.1/LICENSE` & `wasmpy-build-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/PKG-INFO` & `wasmpy-build-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.2.1
-Summary: Emscripten compatible build script for CPython C extensions
+Version: 0.3.0
+Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WasmPy-Build
+# wasmpy-build
 
 This tool can compile CPython C extension files, such as the ones created by Cython, to WebAssembly so that the extensions are platform independent.
 
-The created `.wasm` files can be imported by [WasmPy](https://github.com/olivi-r/wasmpy) in a simmilar manner to native C extensions.
-
 This project contains modified CPython header files as well as a build script to ease the creation of `.wasm` extension files.
 
-Currently this project only supports CPython 3.8, 3.9 and 3.10 but I'm hoping to add support for older versions.
-
-# Installation
+Currently this project only supports CPython 3.8, 3.9, 3.10 and 3.11 but I'm hoping to add support for older and future versions.
 
-To install WasmPy-Build you will first need to install the [Emscripten SDK](https://emscripten.org/docs/getting_started/downloads.html#installation-instructions).
+The project will automatically download [wasi-sdk](https://github.com/WebAssembly/wasi-sdk) on first use.
 
-### Install WasmPy-Build from pip
+# Installation
+### Install from pip
 
 ```bash
-$ pip install wasmpy-build
+pip install wasmpy-build
 ```
 
-### ... or build from source
+### or build from source
 
 ```bash
-$ git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
-$ cd wasmpy-build
-$ python -m pip install -r requirements.txt
-$ python patch_headers.py
-$ python setup.py install
+git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
+cd wasmpy-build
+python -m pip install -r requirements.txt
+python patch_headers.py
+python setup.py install
 ```
```

### Comparing `wasmpy-build-0.2.1/setup.py` & `wasmpy-build-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-import os, setuptools
-
-with open("README.md") as fp:
-    long_description = fp.read()
-
-def recurse_files(directory):
-    paths = []
-    for path, dirs, files in os.walk(directory):
-        for file in files:
-            paths.append(os.path.join("..", path, file))
-
-    return paths
-
-setuptools.setup(
-    name="wasmpy-build",
-    version="0.2.1",
-    author="Olivia Ryan",
-    author_email="olivia.r.dev@gmail.com",
-    description="Emscripten compatible build script for CPython C extensions",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/olivi-r/wasmpy-build",
-    packages=["wasmpy_build"],
-    package_data={
-        "wasmpy_build": recurse_files("wasmpy_build/include")
-    },
-    entry_points={
-        "console_scripts": [
-            "wasmpy-build=wasmpy_build:build"
-        ]
-    },
-    classifiers=[
-        "Programming Language :: C",
-        "Programming Language :: Cython",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "License :: OSI Approved :: MIT License",
-    ],
-    license="MIT",
-    python_requires=">=3.8"
-)
+import os, setuptools
+
+
+with open("README.md") as fp:
+    long_description = fp.read()
+
+
+def recurse_files(directory):
+    paths = []
+    for path, _, files in os.walk(directory):
+        for file in files:
+            paths.append(os.path.join("..", path, file))
+
+    return paths
+
+
+setuptools.setup(
+    name="wasmpy-build",
+    version="0.3.0",
+    author="Olivia Ryan",
+    author_email="olivia.r.dev@gmail.com",
+    description="WebAssembly build tool for CPython C extensions",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/olivi-r/wasmpy-build",
+    packages=["wasmpy_build"],
+    package_data={"wasmpy_build": recurse_files("wasmpy_build/include")},
+    entry_points={"console_scripts": ["wasmpy-build=wasmpy_build:build"]},
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "License :: OSI Approved :: MIT License",
+    ],
+    license="MIT",
+    python_requires=">=3.8",
+)
```

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/LICENSE` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/Python.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/boolobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cellobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/classobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/codecs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/complexobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/frameobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/odictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/picklebufobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pyctype.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pydebug.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/pytime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/cpython/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/datetime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/descrobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/dynamic_annotations.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/errcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/eval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/exports.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/funcobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/genobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_accu.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_asdl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ast_state.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_atomic.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_bitutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_call.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_condvar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_dtoa.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_gc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_gil.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_hamt.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_hashtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_interp.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_long.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_parser.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pyarena.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_runtime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_symtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_unionobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/internal/pycore_warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/intrcheck.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/iterobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/longintrepr.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/longobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/marshal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/memoryobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/modsupport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/opcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/osdefs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/patchlevel.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/py_curses.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pycapsule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pydtrace.d` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pydtrace.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyexpat.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymacconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymacro.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymath.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pyport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystrhex.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pystrtod.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/pythread.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/rangeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/setobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/sliceobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/structmember.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/structseq.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/token.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/tracemalloc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/typeslots.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp310/weakrefobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp310/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/LICENSE` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/Python.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/boolobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/codecs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/complexobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/cellobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/classobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/complexobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/descrobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/frameobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/funcobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/genobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/longintrepr.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/longobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/modsupport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/odictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/picklebufobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pthread_stubs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pthread_stubs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyctype.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pydebug.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pyframe.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pythread.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/pytime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/setobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/cpython/weakrefobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/cpython/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/datetime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/descrobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/dynamic_annotations.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/errcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/exports.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_accu.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_asdl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ast_state.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ast_state.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_atomic.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_atomic_funcs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bitutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bitutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_blocks_output_buffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_call.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_condvar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_dict.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_dict.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_dtoa.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_emscripten_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_exceptions.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_exceptions.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_frame.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_frame.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_gc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_genobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_gil.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_global_objects.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_global_objects.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_global_strings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_global_strings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_hamt.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_hashtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_interp.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_interpreteridobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_list.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_list.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_long.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_opcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_parser.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_parser.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pyarena.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pymath.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_runtime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_runtime_init.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_runtime_init.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_signal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_signal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_strhex.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_strhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_structseq.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_symtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_tuple.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_tuple.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_typeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_typeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_ucnhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_unionobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_unionobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/internal/pycore_warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/intrcheck.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/iterobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/longobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/marshal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/memoryobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/modsupport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/opcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/osdefs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/patchlevel.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/py_curses.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pybuffer.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pybuffer.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pycapsule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pydtrace.d` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pydtrace.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyexpat.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyframe.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyframe.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymacconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymacro.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymath.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pyport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pystrtod.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pythread.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/pytypedefs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/pytypedefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/rangeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/setobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/sliceobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/structmember.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/structseq.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/token.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/tracemalloc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/typeslots.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp311/weakrefobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp311/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/LICENSE` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/Python-ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/Python.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/asdl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/boolobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytes_methods.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cellobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/classobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/codecs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/complexobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/cpython/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/datetime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/descrobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/dynamic_annotations.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/errcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/eval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/frameobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/funcobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/genobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/graminit.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/grammar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_accu.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_atomic.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_condvar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_gil.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_hamt.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_long.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/internal/pycore_warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/intrcheck.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/iterobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/longintrepr.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/longobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/marshal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/memoryobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/modsupport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/node.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/odictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/opcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/osdefs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/parsetok.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/patchlevel.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/picklebufobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/py_curses.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyarena.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pycapsule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyctype.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydebug.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydtrace.d` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pydtrace.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyexpat.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymacconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymacro.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymath.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pyport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystrhex.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pystrtod.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pythread.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/pytime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/rangeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/setobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/sliceobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/structmember.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/structseq.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/symtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/token.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/tracemalloc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/typeslots.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/ucnhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp38/weakrefobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp38/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/LICENSE` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/Python-ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/Python-ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/Python.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/Python.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/asdl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/asdl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/ast.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/ast.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/boolobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/boolobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cellobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cellobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/classobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/classobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/codecs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/codecs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/compile.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/compile.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/complexobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/complexobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/abstract.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/abstract.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/bytearrayobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/bytearrayobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/bytesobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/bytesobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/frameobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/frameobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/cpython/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/cpython/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/datetime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/datetime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/descrobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/descrobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/dictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/dictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/dynamic_annotations.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/dynamic_annotations.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/errcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/errcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/eval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/eval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/exports.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/exports.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/fileobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/fileobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/floatobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/floatobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/funcobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/funcobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/genobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/genobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/graminit.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/graminit.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/grammar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/grammar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/import.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/import.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pegen_interface.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pegen_interface.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_accu.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_accu.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_atomic.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_atomic.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_bytes_methods.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_byteswap.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_byteswap.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_call.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_call.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_ceval.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_ceval.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_code.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_code.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_condvar.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_condvar.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_context.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_context.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_dtoa.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_dtoa.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_fileutils.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_fileutils.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_gc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_gc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_gil.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_gil.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_hamt.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_hamt.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_hashtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_hashtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_initconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_initconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_interp.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_interp.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_long.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_long.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pathconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pathconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_runtime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_runtime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/internal/pycore_warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/internal/pycore_warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/intrcheck.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/intrcheck.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/iterobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/iterobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/listobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/listobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/longintrepr.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/longintrepr.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/longobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/longobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/marshal.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/marshal.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/memoryobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/memoryobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/methodobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/methodobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/modsupport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/modsupport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/moduleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/moduleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/node.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/node.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/object.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/object.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/objimpl.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/objimpl.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/odictobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/odictobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/opcode.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/opcode.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/osdefs.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/osdefs.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/parsetok.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/parsetok.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/patchlevel.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/patchlevel.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/picklebufobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/picklebufobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/py_curses.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/py_curses.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyarena.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyarena.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pycapsule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pycapsule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyctype.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyctype.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydebug.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydebug.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydtrace.d` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydtrace.d`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pydtrace.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pydtrace.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyerrors.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyerrors.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyexpat.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyexpat.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pylifecycle.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pylifecycle.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymacconfig.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymacconfig.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymacro.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymacro.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymath.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymath.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pymem.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pymem.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pyport.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pyport.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystate.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystate.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystrhex.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystrhex.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pystrtod.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pystrtod.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pythonrun.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pythonrun.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pythread.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pythread.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/pytime.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/pytime.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/rangeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/rangeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/setobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/setobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/sliceobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/sliceobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/structmember.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/structmember.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/structseq.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/structseq.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/symtable.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/symtable.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/sysmodule.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/sysmodule.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/token.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/token.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/traceback.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/traceback.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/tracemalloc.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/tracemalloc.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/tupleobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/tupleobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/typeslots.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/typeslots.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/ucnhash.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/ucnhash.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/unicodeobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/unicodeobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/warnings.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/warnings.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build/include/cp39/weakrefobject.h` & `wasmpy-build-0.3.0/wasmpy_build/include/cp39/weakrefobject.h`

 * *Files identical despite different names*

### Comparing `wasmpy-build-0.2.1/wasmpy_build.egg-info/PKG-INFO` & `wasmpy-build-0.3.0/wasmpy_build.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 Metadata-Version: 2.1
 Name: wasmpy-build
-Version: 0.2.1
-Summary: Emscripten compatible build script for CPython C extensions
+Version: 0.3.0
+Summary: WebAssembly build tool for CPython C extensions
 Home-page: https://github.com/olivi-r/wasmpy-build
 Author: Olivia Ryan
 Author-email: olivia.r.dev@gmail.com
 License: MIT
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WasmPy-Build
+# wasmpy-build
 
 This tool can compile CPython C extension files, such as the ones created by Cython, to WebAssembly so that the extensions are platform independent.
 
-The created `.wasm` files can be imported by [WasmPy](https://github.com/olivi-r/wasmpy) in a simmilar manner to native C extensions.
-
 This project contains modified CPython header files as well as a build script to ease the creation of `.wasm` extension files.
 
-Currently this project only supports CPython 3.8, 3.9 and 3.10 but I'm hoping to add support for older versions.
-
-# Installation
+Currently this project only supports CPython 3.8, 3.9, 3.10 and 3.11 but I'm hoping to add support for older and future versions.
 
-To install WasmPy-Build you will first need to install the [Emscripten SDK](https://emscripten.org/docs/getting_started/downloads.html#installation-instructions).
+The project will automatically download [wasi-sdk](https://github.com/WebAssembly/wasi-sdk) on first use.
 
-### Install WasmPy-Build from pip
+# Installation
+### Install from pip
 
 ```bash
-$ pip install wasmpy-build
+pip install wasmpy-build
 ```
 
-### ... or build from source
+### or build from source
 
 ```bash
-$ git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
-$ cd wasmpy-build
-$ python -m pip install -r requirements.txt
-$ python patch_headers.py
-$ python setup.py install
+git clone --recurse-submodules https://github.com/olivi-r/wasmpy-build
+cd wasmpy-build
+python -m pip install -r requirements.txt
+python patch_headers.py
+python setup.py install
 ```
```

### Comparing `wasmpy-build-0.2.1/wasmpy_build.egg-info/SOURCES.txt` & `wasmpy-build-0.3.0/wasmpy_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

