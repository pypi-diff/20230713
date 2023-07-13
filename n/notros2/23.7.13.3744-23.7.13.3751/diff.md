# Comparing `tmp/notros2-23.7.13.3744.tar.gz` & `tmp/notros2-23.7.13.3751-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.13.3744.tar", last modified: Thu Jul 13 00:37:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

