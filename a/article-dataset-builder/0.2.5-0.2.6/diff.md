# Comparing `tmp/article_dataset_builder-0.2.5.tar.gz` & `tmp/article_dataset_builder-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_dataset_builder-0.2.5.tar", last modified: Thu Jul 13 18:35:05 2023, max compression
+gzip compressed data, was "article_dataset_builder-0.2.6.tar", last modified: Thu Jul 13 19:57:05 2023, max compression
```

## Comparing `article_dataset_builder-0.2.5.tar` & `article_dataset_builder-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.5/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.5/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25390 2023-06-27 18:24:00.000000 article_dataset_builder-0.2.5/Readme.md
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/article_dataset_builder/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.5/article_dataset_builder/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.5/article_dataset_builder/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.5/article_dataset_builder/check_cord19_coverage.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    85040 2023-06-27 19:24:50.000000 article_dataset_builder-0.2.5/article_dataset_builder/harvest.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6812 2023-07-13 18:32:01.000000 article_dataset_builder-0.2.5/article_dataset_builder/nlm2tei.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    25949 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-07-13 18:35:05.000000 article_dataset_builder-0.2.5/article_dataset_builder.egg-info/top_level.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-07 16:15:48.000000 article_dataset_builder-0.2.5/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 18:31:48.000000 article_dataset_builder-0.2.5/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 18:35:05.882353 article_dataset_builder-0.2.5/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      979 2023-07-13 18:33:03.000000 article_dataset_builder-0.2.5/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 19:57:05.642088 article_dataset_builder-0.2.6/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    11178 2023-03-05 12:27:19.000000 article_dataset_builder-0.2.6/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       91 2023-03-07 14:43:21.000000 article_dataset_builder-0.2.6/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25912 2023-07-13 19:57:05.642088 article_dataset_builder-0.2.6/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25390 2023-06-27 18:24:00.000000 article_dataset_builder-0.2.6/Readme.md
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 19:57:05.638088 article_dataset_builder-0.2.6/article_dataset_builder/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3431 2020-03-21 07:36:05.000000 article_dataset_builder-0.2.6/article_dataset_builder/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2023-03-05 13:54:10.000000 article_dataset_builder-0.2.6/article_dataset_builder/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     8009 2021-08-30 09:04:38.000000 article_dataset_builder-0.2.6/article_dataset_builder/check_cord19_coverage.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    85040 2023-06-27 19:24:50.000000 article_dataset_builder-0.2.6/article_dataset_builder/harvest.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6899 2023-07-13 19:54:41.000000 article_dataset_builder-0.2.6/article_dataset_builder/nlm2tei.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 19:57:05.642088 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    25912 2023-07-13 19:57:05.000000 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      486 2023-07-13 19:57:05.000000 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 19:57:05.000000 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 19:57:05.000000 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       24 2023-07-13 19:57:05.000000 article_dataset_builder-0.2.6/article_dataset_builder.egg-info/top_level.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      777 2023-03-07 16:15:48.000000 article_dataset_builder-0.2.6/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      103 2023-07-13 18:31:48.000000 article_dataset_builder-0.2.6/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 19:57:05.642088 article_dataset_builder-0.2.6/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      979 2023-07-13 19:54:48.000000 article_dataset_builder-0.2.6/setup.py
```

### Comparing `article_dataset_builder-0.2.5/LICENSE` & `article_dataset_builder-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/PKG-INFO` & `article_dataset_builder-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: article_dataset_builder
-Version: 0.2.5
+Version: 0.2.6
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -470,9 +468,7 @@
 ```
 
 ## License and contact
 
 Distributed under [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0).
 
 Main author and contact: Patrice Lopez (<patrice.lopez@science-miner.com>)
-
-
```

### Comparing `article_dataset_builder-0.2.5/Readme.md` & `article_dataset_builder-0.2.6/Readme.md`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/article_dataset_builder/S3.py` & `article_dataset_builder-0.2.6/article_dataset_builder/S3.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/article_dataset_builder/check_cord19_coverage.py` & `article_dataset_builder-0.2.6/article_dataset_builder/check_cord19_coverage.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/article_dataset_builder/harvest.py` & `article_dataset_builder-0.2.6/article_dataset_builder/harvest.py`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/article_dataset_builder/nlm2tei.py` & `article_dataset_builder-0.2.6/article_dataset_builder/nlm2tei.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                     #print(root, the_file)
                     if not os.path.isfile(os.path.join(temp_dir,the_file)):
                         shutil.copy(os.path.join(root,the_file), temp_dir)
 
         # add dummy DTD files for JATS to avoid errors and crazy online DTD download
         open(os.path.join(temp_dir,"JATS-archivearticle1.dtd"), 'a').close()
         open(os.path.join(temp_dir,"JATS-archivearticle1-mathml3.dtd"), 'a').close()
+        open(os.path.join(temp_dir,"JATS-archivearticle1-3-mathml3.dtd"), 'a').close()
         open(os.path.join(temp_dir,"archivearticle1-mathml3.dtd"), 'a').close()
         open(os.path.join(temp_dir,"archivearticle1.dtd"), 'a').close()
         open(os.path.join(temp_dir,"archivearticle3.dtd"), 'a').close()
         open(os.path.join(temp_dir,"journalpublishing.dtd"), 'a').close()
         open(os.path.join(temp_dir,"archivearticle.dtd"), 'a').close()
         return temp_dir
 
@@ -81,16 +82,16 @@
         try:  
             os.makedirs(temp_dir_out)
         except OSError:  
             print ("Creation of the directory %s failed" % temp_dir_out)
 
         cmd = "java -jar " + os.path.join(self.config["pub2tei_path"],"Samples","saxon9he.jar") + " -s:" + dir_path + \
             " -xsl:" + os.path.join(self.config["pub2tei_path"],"Stylesheets","Publishers.xsl") + \
-            " -o:" + temp_dir_out + " -dtd:off -a:off -expand:off " + \
-            " --parserFeature?uri=http%3A//apache.org/xml/features/nonvalidating/load-external-dtd:false -t" 
+            " -o:" + temp_dir_out + " -dtd:off -a:off -expand:off -t " + \
+            " --parserFeature?uri=http%3A//apache.org/xml/features/nonvalidating/load-external-dtd:false" 
         #print(cmd)
         try:
             result = subprocess.check_call(cmd, shell=True)
         except subprocess.CalledProcessError as e:   
             print("e.returncode", e.returncode)
             print("e.output", e.output)
             #if e.output is not None and e.output.startswith('error: {'):
```

### Comparing `article_dataset_builder-0.2.5/article_dataset_builder.egg-info/PKG-INFO` & `article_dataset_builder-0.2.6/article_dataset_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: article-dataset-builder
-Version: 0.2.5
+Version: 0.2.6
 Summary: Open Access scholar PDF harvester, metadata aggregator and full-text ingester
 Home-page: https://github.com/kermitt2/article_dataset_builder
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -470,9 +468,7 @@
 ```
 
 ## License and contact
 
 Distributed under [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0).
 
 Main author and contact: Patrice Lopez (<patrice.lopez@science-miner.com>)
-
-
```

### Comparing `article_dataset_builder-0.2.5/config.json` & `article_dataset_builder-0.2.6/config.json`

 * *Files identical despite different names*

### Comparing `article_dataset_builder-0.2.5/setup.py` & `article_dataset_builder-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="article_dataset_builder",
-    version="0.2.5",
+    version="0.2.6",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="Open Access scholar PDF harvester, metadata aggregator and full-text ingester",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/kermitt2/article_dataset_builder",
     packages=find_packages(exclude=['test', '*.test', '*.test.*']),
```

