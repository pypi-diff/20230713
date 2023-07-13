# Comparing `tmp/ir_digit-0.0.9.tar.gz` & `tmp/ir_digit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_digit-0.0.9.tar", last modified: Mon Mar 27 13:56:32 2023, max compression
+gzip compressed data, was "ir_digit-1.0.0.tar", last modified: Thu Jul 13 10:07:35 2023, max compression
```

## Comparing `ir_digit-0.0.9.tar` & `ir_digit-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.418610 ir_digit-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      414 2023-03-27 13:56:32.418610 ir_digit-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.412085 ir_digit-0.0.9/digit/
--rw-rw-rw-   0        0        0      144 2023-03-27 12:13:29.000000 ir_digit-0.0.9/digit/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-03-27 13:54:45.000000 ir_digit-0.0.9/digit/code.py
--rw-rw-rw-   0        0        0      550 2023-03-27 13:54:36.000000 ir_digit-0.0.9/digit/data_access.py
--rw-rw-rw-   0        0        0     1117 2023-03-27 13:54:36.000000 ir_digit-0.0.9/digit/download_repo.py
--rw-rw-rw-   0        0        0      468 2023-03-27 13:52:53.000000 ir_digit-0.0.9/digit/load_config.py
-drwxrwxrwx   0        0        0        0 2023-03-27 13:56:32.417610 ir_digit-0.0.9/ir_digit.egg-info/
--rw-rw-rw-   0        0        0      414 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-27 13:56:32.000000 ir_digit-0.0.9/ir_digit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 13:56:32.418610 ir_digit-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      550 2023-03-27 13:56:19.000000 ir_digit-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.328215 ir_digit-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-03-28 12:17:48.000000 ir_digit-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      506 2023-07-13 10:07:35.325153 ir_digit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.305707 ir_digit-1.0.0/digit/
+-rw-rw-rw-   0        0        0      244 2023-06-30 08:41:10.000000 ir_digit-1.0.0/digit/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-07-07 06:05:06.000000 ir_digit-1.0.0/digit/base_data.py
+-rw-rw-rw-   0        0        0     1786 2023-06-01 06:11:19.000000 ir_digit-1.0.0/digit/child_base_data.py
+-rw-rw-rw-   0        0        0     3206 2023-07-07 06:26:49.000000 ir_digit-1.0.0/digit/core.py
+-rw-rw-rw-   0        0        0     7225 2023-07-07 06:11:22.000000 ir_digit-1.0.0/digit/data.py
+-rw-rw-rw-   0        0        0     4987 2023-06-01 08:52:58.000000 ir_digit-1.0.0/digit/download.py
+-rw-rw-rw-   0        0        0      252 2023-06-01 09:12:08.000000 ir_digit-1.0.0/digit/info.json
+-rw-rw-rw-   0        0        0     2155 2023-07-13 09:55:44.000000 ir_digit-1.0.0/digit/info.py
+-rw-rw-rw-   0        0        0     4894 2023-06-30 03:59:09.000000 ir_digit-1.0.0/digit/query.py
+-rw-rw-rw-   0        0        0     2937 2023-07-13 07:20:47.000000 ir_digit-1.0.0/digit/scripts.py
+-rw-rw-rw-   0        0        0     2315 2023-07-13 09:53:29.000000 ir_digit-1.0.0/digit/setting.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.322604 ir_digit-1.0.0/ir_digit.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-13 10:07:35.000000 ir_digit-1.0.0/ir_digit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:07:35.329228 ir_digit-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      940 2023-07-13 10:07:18.000000 ir_digit-1.0.0/setup.py
```

### Comparing `ir_digit-0.0.9/LICENSE` & `ir_digit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_digit-0.0.9/setup.py` & `ir_digit-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 import setuptools
 
+
 setuptools.setup(
     name="ir_digit",
-    version="0.0.9",
+    version="1.0.0",
     author="FKLiu",
     author_email="fkliu001@outlook.com",
     description="digit package",
-    long_description="digit package ……",
+    long_description="digit package 与 digit web 配套使用，下载其digit web中的数据资源并在本地运行",
     long_description_content_type="text",
-    url="https://example.com",
+    url="https://pypi.org/project/ir-digit/",
     packages=setuptools.find_packages(),
+    include_package_data=True,
+    install_requires = [
+        "gitpython",
+        "numpy",
+        "pandas",
+        "matplotlib",
+        "seaborn"
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
+    entry_points={
+            'console_scripts': [
+                'digit=digit.scripts:main',
+            ],
+        },
+
 )
```

