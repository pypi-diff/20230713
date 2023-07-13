# Comparing `tmp/timespan-0.1.tar.gz` & `tmp/timespan-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/timespan-0.1.tar", last modified: Fri Mar 30 03:44:25 2012, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

