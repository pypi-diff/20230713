# Comparing `tmp/chiapos-2.0.0b3.tar.gz` & `tmp/chiapos-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-2.0.0b3.tar", last modified: Fri Jul  7 21:03:02 2023, max compression
+gzip compressed data, was "chiapos-2.0.0b4.tar", last modified: Wed Jul 12 23:36:44 2023, max compression
```

## Comparing `chiapos-2.0.0b3.tar` & `chiapos-2.0.0b4.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/.github/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/actions/fetch_bladebit_harvester.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/build-test-cplusplus.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/plot-k27-no-bitfield.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/plot-k27.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/chiapos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 21:03:02.000000 chiapos-2.0.0b3/chiapos.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/docker-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/docker-test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.769746 chiapos-2.0.0b3/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/bucket_graph.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/code_documentation.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/documents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/aesctr.png
--rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/beyondhellman.png
--rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/beyondhellman2.png
--rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/pointerformat.png
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/images/proofofspace.png
--rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/proof_of_space.html
--rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/documents/proof_of_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/hellman_example/
--rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/aes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/hellman.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/hellman_example/verifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lgtm.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/lib/FiniteStateEntropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.765746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.773746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.777746 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/lib/include/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.781746 chiapos-2.0.0b3/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/python-bindings/chiapos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.785746 chiapos-2.0.0b3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/src/b3/
--rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3.h
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx512.c
--rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_portable.c
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_sse41.c
--rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bitfield.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bitfield_index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chacha8.c
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chacha8.h
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/chia_filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/entry_sizes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase1.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/phases.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/progress.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/quicksort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/serialize.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/sort_manager.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/threading.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/uniformsort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/src/verifier.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/plot-resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tests/test_python_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tools/disk.gnuplot
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/tools/parse_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 21:03:02.789746 chiapos-2.0.0b3/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/endianness.h
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 21:02:49.000000 chiapos-2.0.0b3/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.889790 chiapos-2.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.861790 chiapos-2.0.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.865790 chiapos-2.0.0b4/.github/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/actions/fetch_bladebit_harvester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.869790 chiapos-2.0.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/build-test-cplusplus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/plot-k27-no-bitfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/plot-k27.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-12 23:36:44.889790 chiapos-2.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.869790 chiapos-2.0.0b4/chiapos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-12 23:36:44.000000 chiapos-2.0.0b4/chiapos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-12 23:36:44.000000 chiapos-2.0.0b4/chiapos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:36:44.000000 chiapos-2.0.0b4/chiapos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 23:36:44.000000 chiapos-2.0.0b4/chiapos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 23:36:44.000000 chiapos-2.0.0b4/chiapos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/docker-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/docker-test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.869790 chiapos-2.0.0b4/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/bucket_graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/code_documentation.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.869790 chiapos-2.0.0b4/documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/images/aesctr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/images/beyondhellman.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/images/pointerformat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/images/proofofspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/proof_of_space.html
+-rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/documents/proof_of_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/hellman_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/aes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/hellman.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/hellman_example/verifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lgtm.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.865790 chiapos-2.0.0b4/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.865790 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.873790 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.877790 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.877790 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.881790 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.881790 chiapos-2.0.0b4/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/lib/include/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.881790 chiapos-2.0.0b4/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/python-bindings/chiapos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 23:36:44.889790 chiapos-2.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.885790 chiapos-2.0.0b4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b17phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b17phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b17phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.885790 chiapos-2.0.0b4/src/b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_portable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/bitfield.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/bitfield_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/chacha8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/chacha8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/chia_filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/entry_sizes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/phase1.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/quicksort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/serialize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/sort_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/threading.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/uniformsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/src/verifier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.885790 chiapos-2.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tests/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tests/plot-resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tests/test_python_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.885790 chiapos-2.0.0b4/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tools/disk.gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/tools/parse_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 23:36:44.885790 chiapos-2.0.0b4/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/endianness.h
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 23:36:35.000000 chiapos-2.0.0b4/uint128_t/uint128_t_config.include
```

### Comparing `chiapos-2.0.0b3/.github/actions/fetch_bladebit_harvester.sh` & `chiapos-2.0.0b4/.github/actions/fetch_bladebit_harvester.sh`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/build-test-cplusplus.yml` & `chiapos-2.0.0b4/.github/workflows/build-test-cplusplus.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/build-wheels.yml` & `chiapos-2.0.0b4/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/doc-html-pdf.yml` & `chiapos-2.0.0b4/.github/workflows/doc-html-pdf.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/manual-plot.yml` & `chiapos-2.0.0b4/.github/workflows/manual-plot.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/plot-k27-no-bitfield.yaml` & `chiapos-2.0.0b4/.github/workflows/plot-k27-no-bitfield.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/plot-k27.yaml` & `chiapos-2.0.0b4/.github/workflows/plot-k27.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/.github/workflows/stale-issue.yml` & `chiapos-2.0.0b4/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/CMakeLists.txt` & `chiapos-2.0.0b4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/Dockerfile` & `chiapos-2.0.0b4/Dockerfile`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/LICENSE` & `chiapos-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/PKG-INFO` & `chiapos-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b3/README.md` & `chiapos-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/chiapos.egg-info/PKG-INFO` & `chiapos-2.0.0b4/chiapos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b3/chiapos.egg-info/SOURCES.txt` & `chiapos-2.0.0b4/chiapos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/bucket_graph.pdf` & `chiapos-2.0.0b4/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/code_documentation.pdf` & `chiapos-2.0.0b4/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/images/aesctr.png` & `chiapos-2.0.0b4/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/images/beyondhellman.png` & `chiapos-2.0.0b4/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/images/beyondhellman2.png` & `chiapos-2.0.0b4/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/images/pointerformat.png` & `chiapos-2.0.0b4/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/images/proofofspace.png` & `chiapos-2.0.0b4/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/proof_of_space.html` & `chiapos-2.0.0b4/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/documents/proof_of_space.md` & `chiapos-2.0.0b4/documents/proof_of_space.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/Hellman attacks.pdf` & `chiapos-2.0.0b4/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/aes.hpp` & `chiapos-2.0.0b4/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/bits.hpp` & `chiapos-2.0.0b4/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/calculate_bucket.hpp` & `chiapos-2.0.0b4/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/cli.cpp` & `chiapos-2.0.0b4/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/cxxopts.hpp` & `chiapos-2.0.0b4/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/encoding.hpp` & `chiapos-2.0.0b4/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/hellman.hpp` & `chiapos-2.0.0b4/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/picosha2.hpp` & `chiapos-2.0.0b4/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/plotter_disk.hpp` & `chiapos-2.0.0b4/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/pos_constants.hpp` & `chiapos-2.0.0b4/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/prover_disk.hpp` & `chiapos-2.0.0b4/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/sort_on_disk.hpp` & `chiapos-2.0.0b4/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/util.hpp` & `chiapos-2.0.0b4/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/hellman_example/verifier.hpp` & `chiapos-2.0.0b4/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/LICENSE` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/README.md` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/README.md` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/bitstream.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/compiler.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/debug.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/entropy_common.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_private.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/error_public.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fseU16.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_compress.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/hist.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_compress.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/lib/mem.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/COPYING` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/bench.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/commandline.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/cpu.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fileio.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fseDist.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fullbench.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzer.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/xxhash.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.c` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/FiniteStateEntropy/programs/zlibh.h` & `chiapos-2.0.0b4/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/lib/include/picosha2.hpp` & `chiapos-2.0.0b4/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/python-bindings/chiapos.cpp` & `chiapos-2.0.0b4/python-bindings/chiapos.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -179,11 +179,11 @@
                 py::bytes quality_py = py::bytes(reinterpret_cast<char *>(quality_buf), 32);
                 delete[] quality_buf;
                 return stdx::optional<py::bytes>(quality_py);
             });
 
     py::class_<ContextQueue>(m, "ContextQueue")
         .def("init", &ContextQueue::init);
-    m.attr("decompresser_context_queue") = &decompresser_context_queue;
+    m.attr("decompressor_context_queue") = &decompressor_context_queue;
 }
 
 #endif  // PYTHON_BINDINGS_PYTHON_BINDINGS_HPP_
```

### Comparing `chiapos-2.0.0b3/setup.py` & `chiapos-2.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b17phase2.hpp` & `chiapos-2.0.0b4/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b17phase3.hpp` & `chiapos-2.0.0b4/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b17phase4.hpp` & `chiapos-2.0.0b4/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b17sort_manager.hpp` & `chiapos-2.0.0b4/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3.c` & `chiapos-2.0.0b4/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3.h` & `chiapos-2.0.0b4/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_avx2.c` & `chiapos-2.0.0b4/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_avx2_x86-64_unix.S` & `chiapos-2.0.0b4/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_avx512.c` & `chiapos-2.0.0b4/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_avx512_x86-64_unix.S` & `chiapos-2.0.0b4/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_dispatch.c` & `chiapos-2.0.0b4/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_impl.h` & `chiapos-2.0.0b4/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_portable.c` & `chiapos-2.0.0b4/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_sse41.c` & `chiapos-2.0.0b4/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/b3/blake3_sse41_x86-64_unix.S` & `chiapos-2.0.0b4/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/bitfield.hpp` & `chiapos-2.0.0b4/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/bitfield_index.hpp` & `chiapos-2.0.0b4/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/bits.hpp` & `chiapos-2.0.0b4/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/calculate_bucket.hpp` & `chiapos-2.0.0b4/src/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/chacha8.c` & `chiapos-2.0.0b4/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/chia_filesystem.hpp` & `chiapos-2.0.0b4/src/chia_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/cli.cpp` & `chiapos-2.0.0b4/src/cli.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 // Not thread safe
 inline void InitDecompresserQueueDefault(bool no_cuda = false)
 {
     static bool initialized = false;
     if (initialized) {
         return;
     }
-    decompresser_context_queue.init(1, (uint32_t)std::thread::hardware_concurrency(), false, 9, !no_cuda, 0, false);
+    decompressor_context_queue.init(1, (uint32_t)std::thread::hardware_concurrency(), false, 9, !no_cuda, 0, false);
     initialized = true;
 }
 
 int main(int argc, char *argv[]) try {
     cxxopts::Options options(
         "ProofOfSpace", "Utility for plotting, generating and verifying proofs of space.");
     options.positional_help("(create/prove/verify/check) param1 param2 ")
```

### Comparing `chiapos-2.0.0b3/src/disk.hpp` & `chiapos-2.0.0b4/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/encoding.hpp` & `chiapos-2.0.0b4/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/entry_sizes.hpp` & `chiapos-2.0.0b4/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/exceptions.hpp` & `chiapos-2.0.0b4/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/phase1.hpp` & `chiapos-2.0.0b4/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/phase2.hpp` & `chiapos-2.0.0b4/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/phase3.hpp` & `chiapos-2.0.0b4/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/phase4.hpp` & `chiapos-2.0.0b4/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/phases.hpp` & `chiapos-2.0.0b4/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/plotter_disk.hpp` & `chiapos-2.0.0b4/src/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/pos_constants.hpp` & `chiapos-2.0.0b4/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/prover_disk.hpp` & `chiapos-2.0.0b4/src/prover_disk.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     ) 
     {
         return false;
     }
 };
 #endif // USE_GREEN_REAPER
 
-ContextQueue decompresser_context_queue;
+ContextQueue decompressor_context_queue;
 
 
 // The DiskProver, given a correctly formatted plot file, can efficiently generate valid proofs
 // of space, for a given challenge.
 class DiskProver {
 public:
     static const uint16_t VERSION{1};
@@ -596,19 +596,19 @@
                         req.xLinePoints[0].lo = (uint64_t)new_line_point;
                         if (compression_level >= 6) {
                             uint128_t alt_line_point = ReadLinePoint(disk_file, GetEndTable(), alt_position);
                             req.xLinePoints[1].hi = (uint64_t)(alt_line_point >> 64);
                             req.xLinePoints[1].lo = (uint64_t)alt_line_point;
                         }
 
-                        GreenReaperContext* gr = decompresser_context_queue.pop();
+                        GreenReaperContext* gr = decompressor_context_queue.pop();
                         assert(gr);
 
                         auto res = grGetFetchQualitiesXPair(gr, &req);
-                        decompresser_context_queue.push(gr);
+                        decompressor_context_queue.push(gr);
 
                         if (res != GRResult_OK) {
                             // Expect this will result in failure in a later step.
                             x1x2.first = x1x2.second = 0;
                         } else {
                             x1x2.first = req.x1;
                             x1x2.second = req.x2;
@@ -680,27 +680,27 @@
                 xs = GetInputs(p7_entries[index], 6, nullptr);
             } else {
                 xs = GetInputs(p7_entries[index], 6, &disk_file); // Passing in a disk_file disabled the parallel reads
             }
 
             #if USE_GREEN_REAPER
                 if (compression_level > 0) {
-                    auto gr = decompresser_context_queue.pop();
+                    auto gr = decompressor_context_queue.pop();
 
                     GRCompressedProofRequest req{};
                     req.compressionLevel = compression_level;
                     req.plotId = id.data();
 
                     uint8_t compressed_proof_size = (compression_level <= 8 ? GR_POST_PROOF_CMP_X_COUNT : (GR_POST_PROOF_CMP_X_COUNT / 2));
                     for (int i = 0; i < compressed_proof_size; i++) {
                         req.compressedProof[i] = xs[i].GetValue();
                     }
 
                     GRResult res = grFetchProofForChallenge(gr, &req);
-                    decompresser_context_queue.push(gr);
+                    decompressor_context_queue.push(gr);
 
                     if (res != GRResult_OK) {
                         if (res == GRResult_NoProof) {
                             throw std::runtime_error("GRResult_NoProof received");
                         }
                         if (res == GRResult_Failed) {
                             throw std::runtime_error("GRResult is not GRResult_OK, received GRResult_Failed");
```

### Comparing `chiapos-2.0.0b3/src/quicksort.hpp` & `chiapos-2.0.0b4/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/serialize.hpp` & `chiapos-2.0.0b4/src/serialize.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/sort_manager.hpp` & `chiapos-2.0.0b4/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/threading.hpp` & `chiapos-2.0.0b4/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/uniformsort.hpp` & `chiapos-2.0.0b4/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/util.hpp` & `chiapos-2.0.0b4/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/src/verifier.hpp` & `chiapos-2.0.0b4/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/tests/plot-resources.py` & `chiapos-2.0.0b4/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/tests/test.cpp` & `chiapos-2.0.0b4/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/tests/test_python_bindings.py` & `chiapos-2.0.0b4/tests/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/tools/disk.gnuplot` & `chiapos-2.0.0b4/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/tools/parse_disk.py` & `chiapos-2.0.0b4/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/LICENSE` & `chiapos-2.0.0b4/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/README.md` & `chiapos-2.0.0b4/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/endianness.h` & `chiapos-2.0.0b4/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/uint128_t.cpp` & `chiapos-2.0.0b4/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/uint128_t.include` & `chiapos-2.0.0b4/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b3/uint128_t/uint128_t_config.include` & `chiapos-2.0.0b4/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

