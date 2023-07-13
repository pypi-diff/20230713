# Comparing `tmp/gpassw-0.1.12.tar.gz` & `tmp/gpassw-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpassw-0.1.12.tar", last modified: Wed Jul 12 13:26:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

