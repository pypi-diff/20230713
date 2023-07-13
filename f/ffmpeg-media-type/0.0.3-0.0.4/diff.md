# Comparing `tmp/ffmpeg_media_type-0.0.3.tar.gz` & `tmp/ffmpeg_media_type-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-0.0.3.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-0.0.4.tar", max compression
```

## Comparing `ffmpeg_media_type-0.0.3.tar` & `ffmpeg_media_type-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1066 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/LICENSE
--rw-r--r--   0        0        0       84 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/README.md
--rw-r--r--   0        0        0      869 2023-07-13 07:39:37.324092 ffmpeg_media_type-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/__init__.py
--rw-r--r--   0        0        0    89367 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.2.json
--rw-r--r--   0        0        0    91003 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.3.json
--rw-r--r--   0        0        0    92339 2023-07-13 07:39:16.375638 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.4.json
--rw-r--r--   0        0        0    94852 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.0.json
--rw-r--r--   0        0        0    95951 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.1.json
--rw-r--r--   0        0        0    97292 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.2.json
--rw-r--r--   0        0        0   100111 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.3.json
--rw-r--r--   0        0        0   106316 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.4.json
--rw-r--r--   0        0        0   107177 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-5.0.json
--rw-r--r--   0        0        0   109161 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-5.1.json
--rw-r--r--   0        0        0   120284 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-6.0.json
--rw-r--r--   0        0        0     3780 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0      378 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/main.py
--rw-r--r--   0        0        0        0 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     5956 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/ffmpeg.py
--rw-r--r--   0        0        0     2977 2023-07-13 07:39:16.379639 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/table.py
--rw-r--r--   0        0        0     1790 2023-07-13 07:39:16.479641 ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/wiki_ext.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-13 15:50:52.894261 ffmpeg_media_type-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4026 2023-07-13 15:50:52.894261 ffmpeg_media_type-0.0.4/README.md
+-rw-r--r--   0        0        0      869 2023-07-13 15:51:17.946539 ffmpeg_media_type-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/__init__.py
+-rw-r--r--   0        0        0    89367 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.2.json
+-rw-r--r--   0        0        0    91003 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.3.json
+-rw-r--r--   0        0        0    92339 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.4.json
+-rw-r--r--   0        0        0    94852 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.0.json
+-rw-r--r--   0        0        0    95951 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.1.json
+-rw-r--r--   0        0        0    97292 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.2.json
+-rw-r--r--   0        0        0   100111 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.3.json
+-rw-r--r--   0        0        0   106316 2023-07-13 15:50:52.898261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.4.json
+-rw-r--r--   0        0        0   107177 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.0.json
+-rw-r--r--   0        0        0   109161 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.1.json
+-rw-r--r--   0        0        0   120284 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-6.0.json
+-rw-r--r--   0        0        0     3780 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0      378 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/main.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0        0 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     5956 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/ffmpeg.py
+-rw-r--r--   0        0        0     2977 2023-07-13 15:50:52.902261 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/table.py
+-rw-r--r--   0        0        0     1790 2023-07-13 15:50:53.022262 ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/wiki_ext.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.4/PKG-INFO
```

### Comparing `ffmpeg_media_type-0.0.3/LICENSE` & `ffmpeg_media_type-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/pyproject.toml` & `ffmpeg_media_type-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffmpeg-media-type"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg_media_type", from = "src" }]
 include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/data/*.json"]
 exclude = ["**/tests"]
```

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.2.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.3.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-3.4.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-3.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.0.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.1.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.2.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.3.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-4.4.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-4.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-5.0.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-5.1.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-5.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/data/ffmpeg-6.0.json` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/data/ffmpeg-6.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/info.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/ffmpeg.py` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/table.py` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/table.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.3/src/ffmpeg_media_type/utils/wiki_ext.py` & `ffmpeg_media_type-0.0.4/src/ffmpeg_media_type/utils/wiki_ext.py`

 * *Files identical despite different names*

