# Comparing `tmp/torchmetrics-1.0.0rc1.tar.gz` & `tmp/torchmetrics-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmetrics-1.0.0rc1.tar", last modified: Thu Jun 29 07:21:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

