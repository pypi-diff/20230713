# Comparing `tmp/automslc-3.7.tar.gz` & `tmp/automslc-3.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automslc-3.7.tar", last modified: Tue Apr 13 06:18:12 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

