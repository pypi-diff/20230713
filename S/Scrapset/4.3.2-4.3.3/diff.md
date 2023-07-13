# Comparing `tmp/Scrapset-4.3.2.tar.gz` & `tmp/Scrapset-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.3.2.tar", last modified: Thu Jul 13 17:01:05 2023, max compression
+gzip compressed data, was "Scrapset-4.3.3.tar", last modified: Thu Jul 13 17:01:54 2023, max compression
```

## Comparing `Scrapset-4.3.2.tar` & `Scrapset-4.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:05.869440 Scrapset-4.3.2/
--rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:05.870450 Scrapset-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:05.858027 Scrapset-4.3.2/Scrapset/
--rw-rw-rw-   0        0        0    10289 2023-07-13 17:00:31.000000 Scrapset-4.3.2/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.2/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:01:05.868427 Scrapset-4.3.2/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:05.000000 Scrapset-4.3.2/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-13 17:01:05.000000 Scrapset-4.3.2/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:01:05.000000 Scrapset-4.3.2/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 16:58:08.000000 Scrapset-4.3.2/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-13 17:01:05.000000 Scrapset-4.3.2/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 17:01:05.000000 Scrapset-4.3.2/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.2/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-13 17:01:05.871961 Scrapset-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-13 17:00:41.000000 Scrapset-4.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.156991 Scrapset-4.3.3/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:54.156991 Scrapset-4.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.144313 Scrapset-4.3.3/Scrapset/
+-rw-rw-rw-   0        0        0    10289 2023-07-13 17:00:31.000000 Scrapset-4.3.3/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       61 2023-07-13 16:57:26.000000 Scrapset-4.3.3/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 17:01:54.154990 Scrapset-4.3.3/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 17:01:54.000000 Scrapset-4.3.3/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.3.3/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-13 17:01:54.158987 Scrapset-4.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-13 17:01:45.000000 Scrapset-4.3.3/setup.py
```

### Comparing `Scrapset-4.3.2/PKG-INFO` & `Scrapset-4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.2
+Version: 4.3.3
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.2/README.md` & `Scrapset-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-4.3.2/Scrapset/Scrapset.py` & `Scrapset-4.3.3/Scrapset/Scrapset.py`

 * *Files identical despite different names*

### Comparing `Scrapset-4.3.2/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.3.3/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.3.2
+Version: 4.3.3
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.3.2/licence.txt` & `Scrapset-4.3.3/licence.txt`

 * *Files identical despite different names*

