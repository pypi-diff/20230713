# Comparing `tmp/hyload-0.0.5.tar.gz` & `tmp/hyload-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyload-0.0.5.tar", last modified: Tue Jul 12 12:05:07 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

