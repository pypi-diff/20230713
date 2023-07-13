# Comparing `tmp/sdss-tree-4.0.0.tar.gz` & `tmp/sdss-tree-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-tree-4.0.0.tar", last modified: Thu Jun  1 19:38:32 2023, max compression
+gzip compressed data, was "dist/sdss-tree-4.0.1.tar", last modified: Thu Jul 13 14:25:47 2023, max compression
```

## Comparing `sdss-tree-4.0.0.tar` & `sdss-tree-4.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/bin/setup_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr10.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr11.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr12.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr13.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr14.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr15.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr16.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr17.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr18.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr7.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr9.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/ipl1.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/ipl2.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/sdsswork.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/etc/tree.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/misc/docutree.py
--rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/bin/setup_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/sdss_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/tree/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr10.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr11.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr12.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr13.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr14.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr15.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr16.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr17.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr18.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr7.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/dr9.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/ipl1.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/ipl2.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    25860 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/data/sdsswork.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/tree/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/etc/tree.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/python/tree/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/misc/docutree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/python/tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 14:25:47.000000 sdss-tree-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-13 14:25:33.000000 sdss-tree-4.0.1/setup.py
```

### Comparing `sdss-tree-4.0.0/LICENSE.md` & `sdss-tree-4.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/PKG-INFO` & `sdss-tree-4.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-tree
-Version: 4.0.0
+Version: 4.0.1
 Summary: Control and setup of SDSS tree environment and modules
 Home-page: https://github.com/sdss/tree
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/tree
 Project-URL: Documentation, https://sdss-tree.readthedocs.org
@@ -19,22 +19,41 @@
         This product contains the definition(s) of the SDSS Science Archiver Server (SAS) filesystem environment tree(s).  It
         sets up the SDSS environment configuration files for loading either via the [Modules Environment Manager](http://modules.sourceforge.net/) or dynamically with a ``tree.Tree`` python package.  Available environments are a SDSS "working" environment, i.e. ``sdsswork`` or any number of environments for public Data
         Releases, i.e. ``dr16.cfg``.  See full documentation at http://sdss-tree.readthedocs.io/en/latest/.
         
         
         ## Developer Install
         
-        To install tree for development:
+        ### Local Install
+        
+        To install tree for development locally:
         
         ```
         git clone https://github.com/sdss/tree
         cd tree
         pip install -e ".[dev,docs]"
         ```
         
+        ### Install at Utah
+        
+        To install at Utah for use with modules,
+        ```
+        git clone https://github.com/sdss/tree main
+        cd main
+        python bin/setup_tree.py -v
+        ```
+        Replace `main` with the desired branch or tag name as needed. Also, see the instructions on the [Wiki](https://wiki.sdss.org/display/DATA/tree#tree-InstallationofthetreeproductatUtah)
+        
+        ### Install as a Dependency
+        
+        To install as a Python package dedendency for software use, install the latest tag straight from PyPi:
+        ```
+        pip install sdss-tree
+        ```
+        
         ## Build Sphinx Docs
         
         Within the top level repo directory, run the `sdsstools` commands:
         ```
         # build the Sphinx documentation
         sdss docs.build
```

### Comparing `sdss-tree-4.0.0/README.md` & `sdss-tree-4.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,41 @@
 This product contains the definition(s) of the SDSS Science Archiver Server (SAS) filesystem environment tree(s).  It
 sets up the SDSS environment configuration files for loading either via the [Modules Environment Manager](http://modules.sourceforge.net/) or dynamically with a ``tree.Tree`` python package.  Available environments are a SDSS "working" environment, i.e. ``sdsswork`` or any number of environments for public Data
 Releases, i.e. ``dr16.cfg``.  See full documentation at http://sdss-tree.readthedocs.io/en/latest/.
 
 
 ## Developer Install
 
-To install tree for development:
+### Local Install
+
+To install tree for development locally:
 
 ```
 git clone https://github.com/sdss/tree
 cd tree
 pip install -e ".[dev,docs]"
 ```
 
+### Install at Utah
+
+To install at Utah for use with modules,
+```
+git clone https://github.com/sdss/tree main
+cd main
+python bin/setup_tree.py -v
+```
+Replace `main` with the desired branch or tag name as needed. Also, see the instructions on the [Wiki](https://wiki.sdss.org/display/DATA/tree#tree-InstallationofthetreeproductatUtah)
+
+### Install as a Dependency
+
+To install as a Python package dedendency for software use, install the latest tag straight from PyPi:
+```
+pip install sdss-tree
+```
+
 ## Build Sphinx Docs
 
 Within the top level repo directory, run the `sdsstools` commands:
 ```
 # build the Sphinx documentation
 sdss docs.build
```

### Comparing `sdss-tree-4.0.0/bin/setup_tree.py` & `sdss-tree-4.0.1/bin/setup_tree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/sdss_tree.egg-info/PKG-INFO` & `sdss-tree-4.0.1/python/sdss_tree.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-tree
-Version: 4.0.0
+Version: 4.0.1
 Summary: Control and setup of SDSS tree environment and modules
 Home-page: https://github.com/sdss/tree
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/tree
 Project-URL: Documentation, https://sdss-tree.readthedocs.org
@@ -19,22 +19,41 @@
         This product contains the definition(s) of the SDSS Science Archiver Server (SAS) filesystem environment tree(s).  It
         sets up the SDSS environment configuration files for loading either via the [Modules Environment Manager](http://modules.sourceforge.net/) or dynamically with a ``tree.Tree`` python package.  Available environments are a SDSS "working" environment, i.e. ``sdsswork`` or any number of environments for public Data
         Releases, i.e. ``dr16.cfg``.  See full documentation at http://sdss-tree.readthedocs.io/en/latest/.
         
         
         ## Developer Install
         
-        To install tree for development:
+        ### Local Install
+        
+        To install tree for development locally:
         
         ```
         git clone https://github.com/sdss/tree
         cd tree
         pip install -e ".[dev,docs]"
         ```
         
+        ### Install at Utah
+        
+        To install at Utah for use with modules,
+        ```
+        git clone https://github.com/sdss/tree main
+        cd main
+        python bin/setup_tree.py -v
+        ```
+        Replace `main` with the desired branch or tag name as needed. Also, see the instructions on the [Wiki](https://wiki.sdss.org/display/DATA/tree#tree-InstallationofthetreeproductatUtah)
+        
+        ### Install as a Dependency
+        
+        To install as a Python package dedendency for software use, install the latest tag straight from PyPi:
+        ```
+        pip install sdss-tree
+        ```
+        
         ## Build Sphinx Docs
         
         Within the top level repo directory, run the `sdsstools` commands:
         ```
         # build the Sphinx documentation
         sdss docs.build
```

### Comparing `sdss-tree-4.0.0/python/sdss_tree.egg-info/SOURCES.txt` & `sdss-tree-4.0.1/python/sdss_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/sdss_tree.egg-info/requires.txt` & `sdss-tree-4.0.1/python/sdss_tree.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/changelog.py` & `sdss-tree-4.0.1/python/tree/changelog.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr10.cfg` & `sdss-tree-4.0.1/python/tree/data/dr10.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr11.cfg` & `sdss-tree-4.0.1/python/tree/data/dr11.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr12.cfg` & `sdss-tree-4.0.1/python/tree/data/dr12.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr13.cfg` & `sdss-tree-4.0.1/python/tree/data/dr13.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr14.cfg` & `sdss-tree-4.0.1/python/tree/data/dr14.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr15.cfg` & `sdss-tree-4.0.1/python/tree/data/dr15.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr16.cfg` & `sdss-tree-4.0.1/python/tree/data/dr16.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr17.cfg` & `sdss-tree-4.0.1/python/tree/data/dr17.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr18.cfg` & `sdss-tree-4.0.1/python/tree/data/dr18.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr7.cfg` & `sdss-tree-4.0.1/python/tree/data/dr7.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr8.cfg` & `sdss-tree-4.0.1/python/tree/data/dr8.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/dr9.cfg` & `sdss-tree-4.0.1/python/tree/data/dr9.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/ipl1.cfg` & `sdss-tree-4.0.1/python/tree/data/ipl1.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/ipl2.cfg` & `sdss-tree-4.0.1/python/tree/data/ipl2.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/data/sdsswork.cfg` & `sdss-tree-4.0.1/python/tree/data/sdsswork.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,14 @@
 AllStarSSPP = $MWM_SSPP/{v_sspp}/allStar-SSPP-{v_sspp}.fits
 
 # LVM paths
 lvm_lab = $LVM_DATA_LAB/{mjd}/sdR-{hemi}-{camspec}-{expnum:0>8}.fits.gz
 lvm_raw = $LVM_DATA_S/{mjd}/sdR-{hemi}-{camspec}-{expnum:0>8}.fits.gz
 lvm_anc = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/ancillary/lvm-{kind}{imagetype}-{camera}-{expnum:0>8}.fits
 lvm_cal = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-{kind}-{camera}-{expnum:0>8}.{ext}
-lvm_cal_mbias = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-mbias-{camera}.fits
+lvm_master = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-{kind}-{camera}.fits
 lvm_cal_time = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-{kind}-{camera}-{exptime}.fits
 lvm_cal_pix = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-pixwave-{lamp}-{camera}-{expnum:0>8}.fits
 lvm_cal_through = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-throughput-{expnum:0>8}.fits
 
 # HIPS paths
 sdss_moc = $SDSS_HIPS/{release}/{survey}/Moc.{ext}
```

### Comparing `sdss-tree-4.0.0/python/tree/misc/docutree.py` & `sdss-tree-4.0.1/python/tree/misc/docutree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/python/tree/tree.py` & `sdss-tree-4.0.1/python/tree/tree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-4.0.0/setup.cfg` & `sdss-tree-4.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-tree
-version = 4.0.0
+version = 4.0.1
 author = Brian Cherinka
 author_email = bcherinka@stsci.edu
 description = Control and setup of SDSS tree environment and modules
 url = https://github.com/sdss/tree
 project_urls = 
 	Repository = https://github.com/sdss/tree
 	Documentation = https://sdss-tree.readthedocs.org
```

