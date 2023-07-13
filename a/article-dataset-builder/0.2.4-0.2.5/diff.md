# Comparing `tmp/article_dataset_builder-0.2.4.tar.gz` & `tmp/article_dataset_builder-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_dataset_builder-0.2.4.tar", last modified: Tue Jun 27 18:31:43 2023, max compression
+gzip compressed data, was "article_dataset_builder-0.2.5.tar", last modified: Thu Jul 13 18:35:05 2023, max compression
```

## Comparing `article_dataset_builder-0.2.4.tar` & `article_dataset_builder-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.4/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.4/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25390 2023-06-27 18:24:00.000000 article_dataset_builder-0.2.4/Readme.md
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/article_dataset_builder/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.4/article_dataset_builder/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.4/article_dataset_builder/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.4/article_dataset_builder/check_cord19_coverage.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    85040 2023-06-27 18:28:07.000000 article_dataset_builder-0.2.4/article_dataset_builder/harvest.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6700 2023-03-07 15:08:08.000000 article_dataset_builder-0.2.4/article_dataset_builder/nlm2tei.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-06-27 18:31:43.000000 article_dataset_builder-0.2.4/article_dataset_builder.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-07 16:15:48.000000 article_dataset_builder-0.2.4/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      102 2023-03-05 14:33:42.000000 article_dataset_builder-0.2.4/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-06-27 18:31:43.149557 article_dataset_builder-0.2.4/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      978 2023-06-27 16:39:57.000000 article_dataset_builder-0.2.4/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.5/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.5/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25390 2023-06-27 18:24:00.000000 article_dataset_builder-0.2.5/Readme.md
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/article_dataset_builder/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.5/article_dataset_builder/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.5/article_dataset_builder/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.5/article_dataset_builder/check_cord19_coverage.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    85040 2023-06-27 19:24:50.000000 article_dataset_builder-0.2.5/article_dataset_builder/harvest.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6812 2023-07-13 18:32:01.000000 article_dataset_builder-0.2.5/article_dataset_builder/nlm2tei.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-07 16:15:48.000000 article_dataset_builder-0.2.5/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 18:31:48.000000 article_dataset_builder-0.2.5/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      979 2023-07-13 18:33:03.000000 article_dataset_builder-0.2.5/setup.py
```

### Comparing `article_dataset_builder-0.2.4/LICENSE` & `article_dataset_builder-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/PKG-INFO` & `article_dataset_builder-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article_dataset_builder
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `article_dataset_builder-0.2.4/Readme.md` & `article_dataset_builder-0.2.5/Readme.md`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/article_dataset_builder/S3.py` & `article_dataset_builder-0.2.5/article_dataset_builder/S3.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/article_dataset_builder/check_cord19_coverage.py` & `article_dataset_builder-0.2.5/article_dataset_builder/check_cord19_coverage.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/article_dataset_builder/harvest.py` & `article_dataset_builder-0.2.5/article_dataset_builder/harvest.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/article_dataset_builder/nlm2tei.py` & `article_dataset_builder-0.2.5/article_dataset_builder/nlm2tei.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         try:  
             os.makedirs(temp_dir_out)
         except OSError:  
             print ("Creation of the directory %s failed" % temp_dir_out)
 
         cmd = "java -jar " + os.path.join(self.config["pub2tei_path"],"Samples","saxon9he.jar") + " -s:" + dir_path + \
             " -xsl:" + os.path.join(self.config["pub2tei_path"],"Stylesheets","Publishers.xsl") + \
-            " -o:" + temp_dir_out + " -dtd:off -a:off -expand:off -t"
+            " -o:" + temp_dir_out + " -dtd:off -a:off -expand:off " + \
+            " --parserFeature?uri=http%3A//apache.org/xml/features/nonvalidating/load-external-dtd:false -t" 
         #print(cmd)
         try:
             result = subprocess.check_call(cmd, shell=True)
         except subprocess.CalledProcessError as e:   
             print("e.returncode", e.returncode)
             print("e.output", e.output)
             #if e.output is not None and e.output.startswith('error: {'):
```

### Comparing `article_dataset_builder-0.2.4/article_dataset_builder.egg-info/PKG-INFO` & `article_dataset_builder-0.2.5/article_dataset_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: article-dataset-builder
-Version: 0.2.4
+Version: 0.2.5
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `article_dataset_builder-0.2.4/config.json` & `article_dataset_builder-0.2.5/config.json`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.4/setup.py` & `article_dataset_builder-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="article_dataset_builder",
-    version="0.2.4",
+    version="0.2.5",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="Open Access scholar PDF harvester, metadata aggregator and full-text ingester",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/kermitt2/article_dataset_builder",
     packages=find_packages(exclude=['test', '*.test', '*.test.*']),  
     include_package_data=True,
     python_requires='>=3.5',
     install_requires=[
         'boto3',
         'python-magic==0.4.15',
-        'lmdb==0.94',
+        'lmdb==1.4.1',
         'tqdm==4.21',
         'requests',
         'cloudscraper==1.2.69',
         'beautifulsoup4==4.11.2'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.5",
```

