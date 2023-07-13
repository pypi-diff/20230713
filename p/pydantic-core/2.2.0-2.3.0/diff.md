# Comparing `tmp/pydantic_core-2.2.0.tar.gz` & `tmp/pydantic_core-2.3.0-cp38-cp38-manylinux_2_24_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

