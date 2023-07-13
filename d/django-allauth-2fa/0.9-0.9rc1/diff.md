# Comparing `tmp/django-allauth-2fa-0.9.tar.gz` & `tmp/django_allauth_2fa-0.9rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allauth-2fa-0.9.tar", last modified: Mon Apr 11 12:27:36 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

