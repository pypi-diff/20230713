# Comparing `tmp/notros2-23.7.13.85757.tar.gz` & `tmp/notros2-23.7.13.85806-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.13.85757.tar", last modified: Thu Jul 13 08:57:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

