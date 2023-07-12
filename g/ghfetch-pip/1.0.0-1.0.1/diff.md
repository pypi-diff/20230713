# Comparing `tmp/ghfetch-pip-1.0.0.tar.gz` & `tmp/ghfetch-pip-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfetch-pip-1.0.0.tar", last modified: Wed Jul 12 21:33:31 2023, max compression
+gzip compressed data, was "ghfetch-pip-1.0.1.tar", last modified: Wed Jul 12 22:06:31 2023, max compression
```

## Comparing `ghfetch-pip-1.0.0.tar` & `ghfetch-pip-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 21:33:31.069087 ghfetch-pip-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-07-08 19:21:46.000000 ghfetch-pip-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      242 2023-07-12 21:33:31.069087 ghfetch-pip-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2023-07-12 20:59:19.000000 ghfetch-pip-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 21:33:31.062080 ghfetch-pip-1.0.0/ghfetch/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:59:28.000000 ghfetch-pip-1.0.0/ghfetch/__init__.py
--rw-rw-rw-   0        0        0    10827 2023-07-12 20:59:28.000000 ghfetch-pip-1.0.0/ghfetch/main.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:33:31.068087 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/
--rw-rw-rw-   0        0        0      242 2023-07-12 21:33:31.000000 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-12 21:33:31.000000 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 21:33:31.000000 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-12 21:33:31.000000 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 21:33:31.000000 ghfetch-pip-1.0.0/ghfetch_pip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-12 21:33:31.070088 ghfetch-pip-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-12 21:31:38.000000 ghfetch-pip-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:06:31.072801 ghfetch-pip-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-08 19:21:46.000000 ghfetch-pip-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      242 2023-07-12 22:06:31.072801 ghfetch-pip-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2023-07-12 20:59:19.000000 ghfetch-pip-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 22:06:31.059789 ghfetch-pip-1.0.1/ghfetch/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:59:28.000000 ghfetch-pip-1.0.1/ghfetch/__init__.py
+-rw-rw-rw-   0        0        0    10827 2023-07-12 20:59:28.000000 ghfetch-pip-1.0.1/ghfetch/main.py
+drwxrwxrwx   0        0        0        0 2023-07-12 22:06:31.071800 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-07-12 22:06:30.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-12 22:06:31.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 22:06:30.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-12 22:06:30.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-12 22:06:30.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 22:06:30.000000 ghfetch-pip-1.0.1/ghfetch_pip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-07-12 22:06:31.073802 ghfetch-pip-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      503 2023-07-12 22:06:28.000000 ghfetch-pip-1.0.1/setup.py
```

### Comparing `ghfetch-pip-1.0.0/LICENSE` & `ghfetch-pip-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.0.0/README.md` & `ghfetch-pip-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.0.0/ghfetch/main.py` & `ghfetch-pip-1.0.1/ghfetch/main.py`

 * *Files identical despite different names*

