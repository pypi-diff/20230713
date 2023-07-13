# Comparing `tmp/pymongo-4.4.0b0.tar.gz` & `tmp/pymongo-4.4.1-cp37-cp37m-manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymongo-4.4.0b0.tar", last modified: Wed Jan 25 22:41:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

