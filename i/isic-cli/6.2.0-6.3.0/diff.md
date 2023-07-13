# Comparing `tmp/isic-cli-6.2.0.tar.gz` & `tmp/isic-cli-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-6.2.0.tar", last modified: Wed Jul 12 21:10:56 2023, max compression
+gzip compressed data, was "isic-cli-6.3.0.tar", last modified: Thu Jul 13 17:28:08 2023, max compression
```

## Comparing `isic-cli-6.2.0.tar` & `isic-cli-6.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/zip_and_upload_package.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:10:32.000000 isic-cli-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 21:10:56.472213 isic-cli-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-12 21:10:32.000000 isic-cli-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-12 21:10:32.000000 isic-cli-6.2.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 21:10:32.000000 isic-cli-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:10:56.472213 isic-cli-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 21:10:32.000000 isic-cli-6.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.890811 isic-cli-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.886811 isic-cli-6.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.886811 isic-cli-6.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.github/workflows/release.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.github/zip_and_upload_package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-13 17:27:48.000000 isic-cli-6.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 17:27:48.000000 isic-cli-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 17:28:08.890811 isic-cli-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-13 17:27:48.000000 isic-cli-6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.886811 isic-cli-6.3.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.890811 isic-cli-6.3.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.890811 isic-cli-6.3.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.890811 isic-cli-6.3.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-13 17:27:48.000000 isic-cli-6.3.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.886811 isic-cli-6.3.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 17:28:08.000000 isic-cli-6.3.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-13 17:27:48.000000 isic-cli-6.3.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-13 17:27:48.000000 isic-cli-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:28:08.890811 isic-cli-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-13 17:27:48.000000 isic-cli-6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:28:08.890811 isic-cli-6.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-13 17:27:48.000000 isic-cli-6.3.0/tox.ini
```

### Comparing `isic-cli-6.2.0/.github/workflows/ci.yml` & `isic-cli-6.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/.github/workflows/package.yml` & `isic-cli-6.3.0/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/.github/workflows/release.yml` & `isic-cli-6.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/.gitignore` & `isic-cli-6.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/LICENSE` & `isic-cli-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/PKG-INFO` & `isic-cli-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.2.0
+Version: 6.3.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.2.0/README.md` & `isic-cli-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/__init__.py` & `isic-cli-6.3.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/accession.py` & `isic-cli-6.3.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/collection.py` & `isic-cli-6.3.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/image.py` & `isic-cli-6.3.0/isic_cli/cli/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,25 +100,25 @@
         download_num_images = archive_num_images if limit == 0 else min(archive_num_images, limit)
         nice_num_images = intcomma(download_num_images)
         task = progress.add_task(
             f"Downloading images (and metadata) ({nice_num_images} total)",
             total=download_num_images,
         )
         # the futures ThreadPoolExecutor doesn't allow one to easily Ctrl-c
-        thread_pool = ThreadPool(max(10, os.cpu_count() or 10))
         images_iterator = itertools.islice(
             get_images(ctx.session, search, collections), download_num_images
         )
 
         # See comment above _extract_metadata for why this is necessary
         images = []
         func = functools.partial(download_image, to=outdir, progress=progress, task=task)
-        for image_chunk in chunked(images_iterator, 100):
-            images.extend(image_chunk)
-            thread_pool.map(func, image_chunk)
+        with ThreadPool(max(10, os.cpu_count() or 10)) as thread_pool:
+            for image_chunk in chunked(images_iterator, 100):
+                images.extend(image_chunk)
+                thread_pool.map(func, image_chunk)
 
         headers, records = _extract_metadata(images)
         with (outdir / "metadata.csv").open("w", encoding="utf8") as outfile:
             writer = csv.DictWriter(outfile, headers)
             writer.writeheader()
             writer.writerows(records)
```

### Comparing `isic-cli-6.2.0/isic_cli/cli/metadata.py` & `isic-cli-6.3.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/types.py` & `isic-cli-6.3.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/user.py` & `isic-cli-6.3.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/cli/utils.py` & `isic-cli-6.3.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/io/http.py` & `isic-cli-6.3.0/isic_cli/io/http.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/session.py` & `isic-cli-6.3.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli/utils/version.py` & `isic-cli-6.3.0/isic_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-6.3.0/isic_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.2.0
+Version: 6.3.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-6.2.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-6.3.0/isic_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/pyproject.toml` & `isic-cli-6.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/setup.py` & `isic-cli-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/conftest.py` & `isic-cli-6.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/test_cli_base.py` & `isic-cli-6.3.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/test_cli_collection.py` & `isic-cli-6.3.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/test_cli_image.py` & `isic-cli-6.3.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/test_cli_metadata.py` & `isic-cli-6.3.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tests/test_utils.py` & `isic-cli-6.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.2.0/tox.ini` & `isic-cli-6.3.0/tox.ini`

 * *Files identical despite different names*

