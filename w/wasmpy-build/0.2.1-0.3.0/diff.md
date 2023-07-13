# Comparing `tmp/wasmpy-build-0.2.1.tar.gz` & `tmp/wasmpy_build-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-build-0.2.1.tar", last modified: Mon May 22 11:37:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

