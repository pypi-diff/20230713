# Comparing `tmp/notros2-23.7.13.84657.tar.gz` & `tmp/notros2-23.7.13.84704-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.13.84657.tar", last modified: Thu Jul 13 08:46:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

