# Comparing `tmp/PyMenus-0.1.0.tar.gz` & `tmp/PyMenus-66.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMenus-0.1.0.tar", last modified: Thu Jul 13 21:26:41 2023, max compression
+gzip compressed data, was "PyMenus-66.0.0.tar", last modified: Wed Feb  8 15:28:24 2023, max compression
```

## Comparing `PyMenus-0.1.0.tar` & `PyMenus-66.0.0.tar`

### file list

```diff
@@ -1,21 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 21:26:41.007486 PyMenus-0.1.0/
--rw-rw-rw-   0        0        0       66 2023-07-10 08:42:05.000000 PyMenus-0.1.0/.gitattributes
--rw-rw-rw-   0        0        0     2915 2023-07-10 08:42:05.000000 PyMenus-0.1.0/.gitignore
--rw-rw-rw-   0        0        0    27011 2023-07-10 08:42:05.000000 PyMenus-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2642 2023-07-13 21:26:41.004495 PyMenus-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 21:26:40.977487 PyMenus-0.1.0/PyMenus.egg-info/
--rw-rw-rw-   0        0        0     2642 2023-07-13 21:26:40.000000 PyMenus-0.1.0/PyMenus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-07-13 21:26:40.000000 PyMenus-0.1.0/PyMenus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 21:26:40.000000 PyMenus-0.1.0/PyMenus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 21:26:40.000000 PyMenus-0.1.0/PyMenus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 21:26:40.000000 PyMenus-0.1.0/PyMenus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2143 2023-07-13 20:57:34.000000 PyMenus-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 21:26:40.990493 PyMenus-0.1.0/examples/
--rw-rw-rw-   0        0        0      226 2023-07-10 13:19:01.000000 PyMenus-0.1.0/examples/1_Simple.py
--rw-rw-rw-   0        0        0      662 2023-07-10 14:09:17.000000 PyMenus-0.1.0/examples/2_Options.py
--rw-rw-rw-   0        0        0     1428 2023-07-10 14:14:57.000000 PyMenus-0.1.0/examples/3_Dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:26:40.997485 PyMenus-0.1.0/pymenus/
--rw-rw-rw-   0        0        0       19 2023-07-10 09:15:31.000000 PyMenus-0.1.0/pymenus/__init__.py
--rw-rw-rw-   0        0        0     5931 2023-07-13 20:57:15.000000 PyMenus-0.1.0/pymenus/menu.py
--rw-rw-rw-   0        0        0      776 2023-07-13 21:25:06.000000 PyMenus-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 21:26:41.007486 PyMenus-0.1.0/setup.cfg
+drwxrwxr-x   0 ezzer     (1000) ezzer     (1001)        0 2023-02-08 15:28:24.608459 PyMenus-66.0.0/
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      482 2023-02-08 15:28:24.608459 PyMenus-66.0.0/PKG-INFO
+drwxrwxr-x   0 ezzer     (1000) ezzer     (1001)        0 2023-02-08 15:28:24.608459 PyMenus-66.0.0/PyMenus.egg-info/
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      482 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/PKG-INFO
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      142 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)        1 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)        1 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/top_level.txt
+-rw-r--r--   0 ezzer     (1000) ezzer     (1001)      172 2023-02-08 15:28:24.000000 PyMenus-66.0.0/README.md
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)       38 2023-02-08 15:28:24.608459 PyMenus-66.0.0/setup.cfg
+-rw-r--r--   0 ezzer     (1000) ezzer     (1001)      526 2023-02-08 15:28:24.000000 PyMenus-66.0.0/setup.py
```

