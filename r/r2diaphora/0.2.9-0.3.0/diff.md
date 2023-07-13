# Comparing `tmp/r2diaphora-0.2.9.tar.gz` & `tmp/r2diaphora-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2diaphora-0.2.9.tar", last modified: Wed May 31 14:17:17 2023, max compression
+gzip compressed data, was "r2diaphora-0.3.0.tar", last modified: Thu Jul 13 09:08:13 2023, max compression
```

## Comparing `r2diaphora-0.2.9.tar` & `r2diaphora-0.3.0.tar`

### file list

```diff
@@ -1,184 +1,36 @@
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/LICENSE
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/MANIFEST.in
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/README.md
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/__init__.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94459 2023-05-22 08:45:18.000000 r2diaphora-0.2.9/r2diaphora/diaphora.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/diaphora_heuristics.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41947 2023-05-31 10:24:37.000000 r2diaphora-0.2.9/r2diaphora/diaphora_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/difflibparser.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/html_diff.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/idaapi/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/idaapi/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    22997 2023-05-31 10:23:39.000000 r2diaphora-0.2.9/r2diaphora/idaapi/idaapi_to_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/idaapi/instructions.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/jkutils/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/factor.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/graph_hashes.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/jkutils/kfuzzy.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora/others/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/others/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/others/tarjan_sort.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.641971 r2diaphora-0.2.9/r2diaphora/pycparser/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.661973 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_ansi.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/_syslist.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/aio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/alloca.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/argz.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/arpa/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/asm-generic/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/assert.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/complex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/cpio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/dirent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/dlfcn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/emmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/endian.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/envz.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/errno.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fastmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fcntl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/features.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fenv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/float.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/fnmatch.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ftw.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/getopt.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/glob.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/grp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/iconv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ieeefp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/immintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/inttypes.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/iso646.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/langinfo.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/libgen.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/libintl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/limits.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/linux/version.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/locale.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/malloc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/math.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/monetary.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/mqueue.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ndbm.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/net/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/net/if.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netdb.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/in.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/newlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/nl_types.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.665974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/err.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/paths.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/process.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/pthread.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/pwd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/reent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/regdef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/regex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sched.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/search.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/semaphore.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/setjmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/signal.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/smmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/spawn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdarg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdatomic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdbool.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stddef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdint.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/string.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/strings.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/stropts.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.669974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/mman.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/msg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/resource.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/select.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/sem.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/shm.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/stat.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/times.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/uio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/un.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/sys/wait.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/syslog.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/tar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/termios.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/tgmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/threads.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/trace.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/ulimit.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/unctrl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/unistd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utime.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/utmpx.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wchar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/wordexp.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.669974 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/xcb/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/pycparser/fake_libc_include/zlib.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.641971 r2diaphora-0.2.9/r2diaphora/signatures/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/r2diaphora/signatures/flirt/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_arm.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_mips.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_ppc.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_sh4.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86-64.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/r2diaphora/signatures/flirt/uclibc_x86.sig
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.645972 r2diaphora-0.2.9/r2diaphora.egg-info/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/SOURCES.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/dependency_links.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/entry_points.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/requires.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-05-31 14:17:17.000000 r2diaphora-0.2.9/r2diaphora.egg-info/top_level.txt
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/scripts/
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/scripts/r2diaphora-bulk
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-05-16 15:00:43.000000 r2diaphora-0.2.9/scripts/r2diaphora-db
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-05-31 14:17:17.673975 r2diaphora-0.2.9/setup.cfg
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-05-31 14:17:02.000000 r2diaphora-0.2.9/setup.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/LICENSE
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/MANIFEST.in
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      584 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/README.md
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.480360 r2diaphora-0.3.0/r2diaphora/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/__init__.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94459 2023-05-22 08:45:18.000000 r2diaphora-0.3.0/r2diaphora/diaphora.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/diaphora_heuristics.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    42812 2023-07-11 08:32:33.000000 r2diaphora-0.3.0/r2diaphora/diaphora_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/difflibparser.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/html_diff.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.484362 r2diaphora-0.3.0/r2diaphora/idaapi/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/idaapi/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    21956 2023-07-11 12:46:42.000000 r2diaphora-0.3.0/r2diaphora/idaapi/idaapi_to_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/idaapi/instructions.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/r2diaphora/jkutils/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/factor.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/graph_hashes.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/jkutils/kfuzzy.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/r2diaphora/others/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/others/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/r2diaphora/others/tarjan_sort.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.484362 r2diaphora-0.3.0/r2diaphora.egg-info/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      584 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      743 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       60 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/entry_points.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       91 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/requires.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-07-13 09:08:13.000000 r2diaphora-0.3.0/r2diaphora.egg-info/top_level.txt
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/scripts/
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/scripts/r2diaphora-bulk
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-05-16 15:00:43.000000 r2diaphora-0.3.0/scripts/r2diaphora-db
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-07-13 09:08:13.488363 r2diaphora-0.3.0/setup.cfg
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2226 2023-07-11 12:39:20.000000 r2diaphora-0.3.0/setup.py
```

### Comparing `r2diaphora-0.2.9/LICENSE` & `r2diaphora-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/README.md` & `r2diaphora-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/diaphora.py` & `r2diaphora-0.3.0/r2diaphora/diaphora.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/diaphora_heuristics.py` & `r2diaphora-0.3.0/r2diaphora/diaphora_heuristics.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/diaphora_r2.py` & `r2diaphora-0.3.0/r2diaphora/diaphora_r2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 import os
 import re
-import sys
+import math
 import time
 import math
 import json
 import signal
 import decimal
 import difflib
 import logging
@@ -55,15 +55,15 @@
 def raise_timeout(signum, frame):
     raise TimeoutError
 
 #-----------------------------------------------------------------------
 g_bindiff_opts = {
     "decompiler_command": "pdg",
     "use_decompiler": True,
-    "rebuild_ast": False,
+    "rebuild_ast": True,
 }
 
 def round_up_to_even(f):
     return math.ceil(f / 2.) * 2
 
 #-----------------------------------------------------------------------
 class CIDABinDiff(diaphora.CBinDiff):
@@ -257,32 +257,48 @@
         return code.replace("sym.imp.", "")\
                    .replace("sym.", "")\
                    .replace("fcn.", "fcn_")\
                    .replace("flirt.", "")\
                    .replace("obj.", "")\
                    .replace("noreturn", "")
 
-    def decompile_and_get(self, ea):
-        sv = decompile(ea, decompiler_command=self.decompiler_command);
+    def decompile_and_get(self, ea, timeout = 15):
+        # Register a function to raise a TimeoutError on the signal.
+        signal.signal(signal.SIGALRM, raise_timeout)
+        # Schedule the signal to be sent after `timeout`.
+        signal.alarm(timeout)
+        sv = None
+        try:
+            sv = decompile(ea, decompiler_command=self.decompiler_command);
+        except TimeoutError:
+            log.warning(
+                "Timeout (%ds) while attempting to decompile 0x%x",
+                timeout, ea
+            )
+        finally:
+            # Unregister the signal so it won't be triggered
+            # if the timeout is not reached.
+            signal.signal(signal.SIGALRM, signal.SIG_IGN)
+
         if sv is None:
             # Failed to decompile
             return None
 
+        self.pseudo_hash[ea] = 1
         if self.rebuild_ast:
-            visitor = CAstVisitor()
-            visitor.apply_to(
-                f"""
-                {self.clean_pseudocode(sv)}
-                """
-            )
-            self.pseudo_hash[ea] = visitor.primes_hash
-        else:
-            self.pseudo_hash[ea] = 1
-        self.pseudo[ea] = []
+            try:
+                self.pseudo_hash[ea] = calc_pseudo_hash(ea)
+            except Exception:
+                log.exception(
+                    "Exception while calculating pseudocode primes hash for function 0x%x",
+                    ea
+                )
+                self.pseudo_hash[ea] = 1
 
+        self.pseudo[ea] = []
         first_line = None
         for line in sv.split("\n"):
             if line == "" or line.startswith("//"):
                 continue
 
             if first_line is None:
                 first_line = line
@@ -349,15 +365,15 @@
             log.warning(
                 "Timeout while reading function at 0x%s from file %s",
                 f, log_exec_r2_cmdj("ij").get("core", {}).get("file", "PATH ERROR")
             )
         except Exception:
             log.exception(
                 "Exception while trying to read function at 0x%x in sample %s",
-                f, log_exec_r2_cmdj("ij").get("core", {}).get("file", "PATH ERROR")
+                int(f), log_exec_r2_cmdj("ij").get("core", {}).get("file", "PATH ERROR")
             )
         finally:
             # Unregister the signal so it won't be triggered
             # if the timeout is not reached.
             signal.signal(signal.SIGALRM, signal.SIG_IGN)
         return ret
 
@@ -440,15 +456,19 @@
             instructions_data = []
 
             block_ea = block["start"] - image_base
             idx = len(bb_topological)
             bb_topological[idx] = []
             bb_topo_num[block_ea] = idx
 
-            for x in block["instrs"]:
+            instrs = block.get("instrs", [])
+            if not instrs:
+                log.warning("No instrs for block at 0x%x", block["addr"])
+
+            for x in instrs:
                 _, ins = diaphora_decode(x)
                 mnem   = ins["mnemonic"]
                 disasm = ins["disasm"]
 
                 if "call" in ins.get("type"):
                     kgh_hash *= FEATURE_CALL
 
@@ -467,15 +487,20 @@
                             assembly[block_ea] = [f"loc_{x}:", disasm]
 
                 for oper in ins.get("opex", {}).get("operands", []):
                     if oper["type"] == "imm":
                         if self.is_constant(oper, x) and self.constant_filter(oper["value"]):
                             constants.append(oper["value"])
 
-                mnem_bytes = ins["bytes"][ins["mask"].find("f"):ins["mask"].rfind("f") + 1]
+                ins_bytes  = int(ins["bytes"], 16)
+                mask       = int(ins["mask"], 16)
+                mnem_bytes = hex(ins_bytes & mask)[2:]
+                # If len of mnem_bytes is uneven, pad to next even number
+                pad_len    = math.ceil(len(mnem_bytes) / 2.) * 2
+                mnem_bytes = mnem_bytes.rjust(pad_len, "0")
                 curr_bytes = bytes.fromhex(mnem_bytes)
 
                 bytes_hash.append(curr_bytes)
                 bytes_sum += sum(curr_bytes)
 
                 function_hash.append(bytes.fromhex(ins["bytes"]))
                 outdegree += len(CodeRefsFrom(x, 0))
@@ -900,15 +925,15 @@
         opts.file_out = dbname
     bd = None
 
     try:
         bd = CIDABinDiff(opts.file_out)
         bd.use_decompiler_always = (get_arch() != "sh") and g_bindiff_opts.get("use_decompiler", True)
         bd.decompiler_command = g_bindiff_opts.get("decompiler_command", "pdg")
-        bd.rebuild_ast = g_bindiff_opts.get("rebuild_ast", False)
+        bd.rebuild_ast = g_bindiff_opts.get("rebuild_ast", True)
         bd.exclude_library_thunk = opts.exclude_library_thunk
         bd.unreliable = opts.unreliable
         bd.slow_heuristics = opts.slow
         bd.relaxed_ratio = opts.relax
         bd.experimental = opts.experimental
         bd.min_ea = opts.min_ea
         bd.max_ea = opts.max_ea
@@ -1068,30 +1093,23 @@
     parser.add_argument(
         "-a",
         dest='analyze_all',
         action='store_true',
         help="Analyze ALL functions (by default library functions are skipped)"
     )
 
-    parser.add_argument(
-        "--ast",
-        action='store_true',
-        help="Attempt to rebuild AST from the decompiler output for additional function traits"
-    )
-
     args = parser.parse_args()
     args.file1 = args.file1[0]
     decompiler_commands = {
         "ghidra": "pdg",
         "pdc": "pdc"
     }
 
     g_bindiff_opts["decompiler_command"] = decompiler_commands.get(args.decompiler)
     g_bindiff_opts["use_decompiler"] = not args.no_decompiler
-    g_bindiff_opts["rebuild_ast"] = args.ast
 
     db1name = dbname_for_file(args.file1)
     bd = diaphora.CBinDiff(db1name)
 
     fn_filter = lambda fn: (
         not fn["name"].startswith("flirt.") and fn["nbbs"] >= args.nbbs
     )
```

### Comparing `r2diaphora-0.2.9/r2diaphora/difflibparser.py` & `r2diaphora-0.3.0/r2diaphora/difflibparser.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/html_diff.py` & `r2diaphora-0.3.0/r2diaphora/html_diff.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/idaapi/instructions.py` & `r2diaphora-0.3.0/r2diaphora/idaapi/instructions.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/jkutils/factor.py` & `r2diaphora-0.3.0/r2diaphora/jkutils/factor.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/jkutils/graph_hashes.py` & `r2diaphora-0.3.0/r2diaphora/jkutils/graph_hashes.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/jkutils/kfuzzy.py` & `r2diaphora-0.3.0/r2diaphora/jkutils/kfuzzy.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/r2diaphora/others/tarjan_sort.py` & `r2diaphora-0.3.0/r2diaphora/others/tarjan_sort.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/scripts/r2diaphora-bulk` & `r2diaphora-0.3.0/scripts/r2diaphora-bulk`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/scripts/r2diaphora-db` & `r2diaphora-0.3.0/scripts/r2diaphora-db`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.9/setup.py` & `r2diaphora-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
-import shutil
-import glob
+from distutils.dir_util import copy_tree
 
 from setuptools import setup
 from setuptools.command.install import install
+
 class CustomInstall(install):
 
     def run(self):
         install.run(self)
         self.__post_install()
 
     def __post_install(self):
@@ -23,23 +23,25 @@
                     )
                 )
             except FileExistsError:
                 pass
 
         dirname  = os.path.dirname(__file__)
         sigs_dir = os.path.join(dirname, "r2diaphora", "signatures", "flirt")
-        for f in glob.glob(f"{sigs_dir}/*.sig"):
-            shutil.copy2(
-                f,
-                os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt")
-            )
+        for _, dirs, _ in os.walk(sigs_dir):
+            for d in dirs:
+                dir_path = os.path.join(sigs_dir, d)
+                copy_tree(
+                    dir_path,
+                    os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt", d)
+                )
 
 setup(
     name="r2diaphora",
-    version="0.2.9",
+    version="0.3.0",
     description="radare2 port of diaphora",
     url="https://github.com/FernandoDoming/r2diaphora",
     author="Fernando Domínguez",
     author_email="fernando.dom.del@gmail.com",
     license="GNU GPL v3",
     packages=[
         "r2diaphora",
@@ -49,23 +51,23 @@
     ],
     install_requires=[
         "chardet>=4.0.0",
         "r2pipe>=1.6.3",
         "colorama>=0.4.4",
         "yattag>=1.14.0",
         "mysql-connector-python>=8.0.26",
-        "python_magic>=0.4.24",
-        "pycparser>=2.21"
     ],
 
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 
     entry_points = {
         "console_scripts": ["r2diaphora=r2diaphora.diaphora_r2:main"]
     },
 
     scripts=[
```

