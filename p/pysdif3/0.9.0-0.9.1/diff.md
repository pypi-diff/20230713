# Comparing `tmp/pysdif3-0.9.0.tar.gz` & `tmp/pysdif3-0.9.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdif3-0.9.0.tar", last modified: Wed Mar  8 19:07:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

