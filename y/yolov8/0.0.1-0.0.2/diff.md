# Comparing `tmp/yolov8-0.0.1.tar.gz` & `tmp/yolov8-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov8-0.0.1.tar", last modified: Sat Jul  9 17:24:27 2022, max compression
+gzip compressed data, was "yolov8-0.0.2.tar", last modified: Thu Jul 13 20:19:50 2023, max compression
```

## Comparing `yolov8-0.0.1.tar` & `yolov8-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 17:24:27.157753 yolov8-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-07-09 17:24:27.157753 yolov8-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-09 17:24:19.000000 yolov8-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-07-09 17:24:27.157753 yolov8-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-07-09 17:24:19.000000 yolov8-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 17:24:27.157753 yolov8-0.0.1/yolov8/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-09 17:24:19.000000 yolov8-0.0.1/yolov8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-09 17:24:27.157753 yolov8-0.0.1/yolov8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-07-09 17:24:27.000000 yolov8-0.0.1/yolov8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-07-09 17:24:27.000000 yolov8-0.0.1/yolov8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-09 17:24:27.000000 yolov8-0.0.1/yolov8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-09 17:24:27.000000 yolov8-0.0.1/yolov8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-09 17:24:27.000000 yolov8-0.0.1/yolov8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:19:50.403950 yolov8-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-13 20:19:50.403950 yolov8-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 20:19:39.000000 yolov8-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 20:19:50.407950 yolov8-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-13 20:19:39.000000 yolov8-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:19:50.403950 yolov8-0.0.2/yolov8/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 20:19:39.000000 yolov8-0.0.2/yolov8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:19:50.403950 yolov8-0.0.2/yolov8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-13 20:19:50.000000 yolov8-0.0.2/yolov8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 20:19:50.000000 yolov8-0.0.2/yolov8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:19:50.000000 yolov8-0.0.2/yolov8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 20:19:50.000000 yolov8-0.0.2/yolov8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 20:19:50.000000 yolov8-0.0.2/yolov8.egg-info/top_level.txt
```

### Comparing `yolov8-0.0.1/setup.py` & `yolov8-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 setuptools.setup(
     name="yolov8",
     version=get_version(),
     author="",
     license="",
-    description="Wrapper for incomming yolov8",
+    description=(':warning: The `yolov8` package is a placeholder, not the official Ultralytics version. Please install the official `ultralytics` package via `pip install ultralytics` instead.'),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires=">=3.7",
     install_requires=get_requirements(),
     extras_require={"tests": ["pytest"]},
```

