# Comparing `tmp/LundPDFMaster-1.1.0.tar.gz` & `tmp/LundPDFMaster-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LundPDFMaster-1.1.0.tar", last modified: Fri Jul  7 10:14:01 2023, max compression
+gzip compressed data, was "LundPDFMaster-1.1.1.tar", last modified: Thu Jul 13 15:51:14 2023, max compression
```

## Comparing `LundPDFMaster-1.1.0.tar` & `LundPDFMaster-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-07 10:14:01.460882 LundPDFMaster-1.1.0/
--rw-rw-r--   0 ensar     (1000) ensar     (1000)     1067 2023-07-06 14:25:06.000000 LundPDFMaster-1.1.0/LICENSE.txt
-drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-07 10:14:01.456882 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/
--rw-rw-r--   0 ensar     (1000) ensar     (1000)     1356 2023-07-07 10:14:01.000000 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/PKG-INFO
--rw-rw-r--   0 ensar     (1000) ensar     (1000)      318 2023-07-07 10:14:01.000000 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 ensar     (1000) ensar     (1000)        1 2023-07-07 10:14:01.000000 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 ensar     (1000) ensar     (1000)        9 2023-07-07 10:14:01.000000 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/requires.txt
--rw-rw-r--   0 ensar     (1000) ensar     (1000)       22 2023-07-07 10:14:01.000000 LundPDFMaster-1.1.0/LundPDFMaster.egg-info/top_level.txt
--rw-rw-r--   0 ensar     (1000) ensar     (1000)     1356 2023-07-07 10:14:01.460882 LundPDFMaster-1.1.0/PKG-INFO
--rw-rw-r--   0 ensar     (1000) ensar     (1000)      876 2023-07-07 10:06:40.000000 LundPDFMaster-1.1.0/README.md
-drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-07 10:14:01.456882 LundPDFMaster-1.1.0/lund_pdf_master/
--rw-rw-r--   0 ensar     (1000) ensar     (1000)     7924 2023-06-30 11:14:32.000000 LundPDFMaster-1.1.0/lund_pdf_master/OfficeToPDFConverter.py
--rw-rw-r--   0 ensar     (1000) ensar     (1000)        0 2023-06-23 10:45:13.000000 LundPDFMaster-1.1.0/lund_pdf_master/__init__.py
--rw-rw-r--   0 ensar     (1000) ensar     (1000)       38 2023-07-07 10:14:01.460882 LundPDFMaster-1.1.0/setup.cfg
--rw-rw-r--   0 ensar     (1000) ensar     (1000)      782 2023-07-07 10:13:39.000000 LundPDFMaster-1.1.0/setup.py
-drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-07 10:14:01.456882 LundPDFMaster-1.1.0/tests/
--rw-rw-r--   0 ensar     (1000) ensar     (1000)        0 2023-06-23 10:45:13.000000 LundPDFMaster-1.1.0/tests/__init__.py
--rw-rw-r--   0 ensar     (1000) ensar     (1000)     2159 2023-07-06 14:01:52.000000 LundPDFMaster-1.1.0/tests/test_api.py
+drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)     1067 2023-07-06 14:25:06.000000 LundPDFMaster-1.1.1/LICENSE.txt
+drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)     1356 2023-07-13 15:51:14.000000 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)      318 2023-07-13 15:51:14.000000 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)        1 2023-07-13 15:51:14.000000 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)        9 2023-07-13 15:51:14.000000 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/requires.txt
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)       22 2023-07-13 15:51:14.000000 LundPDFMaster-1.1.1/LundPDFMaster.egg-info/top_level.txt
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)     1356 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/PKG-INFO
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)      876 2023-07-07 10:06:40.000000 LundPDFMaster-1.1.1/README.md
+drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/lund_pdf_master/
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)     7068 2023-07-13 15:48:37.000000 LundPDFMaster-1.1.1/lund_pdf_master/OfficeToPDFConverter.py
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)        0 2023-06-23 10:45:13.000000 LundPDFMaster-1.1.1/lund_pdf_master/__init__.py
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)       38 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/setup.cfg
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)      782 2023-07-13 13:48:00.000000 LundPDFMaster-1.1.1/setup.py
+drwxrwxr-x   0 ensar     (1000) ensar     (1000)        0 2023-07-13 15:51:14.120735 LundPDFMaster-1.1.1/tests/
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)        0 2023-06-23 10:45:13.000000 LundPDFMaster-1.1.1/tests/__init__.py
+-rw-rw-r--   0 ensar     (1000) ensar     (1000)     2159 2023-07-13 15:48:15.000000 LundPDFMaster-1.1.1/tests/test_api.py
```

### Comparing `LundPDFMaster-1.1.0/LICENSE.txt` & `LundPDFMaster-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LundPDFMaster-1.1.0/LundPDFMaster.egg-info/PKG-INFO` & `LundPDFMaster-1.1.1/LundPDFMaster.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LundPDFMaster
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for converting office files to PDF using the iLovePDF API
 Home-page: https://github.com/LundIT/LundPDFMaster
 Author: Ensar Kaya
 Author-email: e.kaya@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LundPDFMaster-1.1.0/PKG-INFO` & `LundPDFMaster-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LundPDFMaster
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for converting office files to PDF using the iLovePDF API
 Home-page: https://github.com/LundIT/LundPDFMaster
 Author: Ensar Kaya
 Author-email: e.kaya@lund-it.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LundPDFMaster-1.1.0/README.md` & `LundPDFMaster-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `LundPDFMaster-1.1.0/lund_pdf_master/OfficeToPDFConverter.py` & `LundPDFMaster-1.1.1/lund_pdf_master/OfficeToPDFConverter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
+import traceback
 import requests
 import logging
 import concurrent.futures
+from rest_framework.exceptions import APIException
 
 class OfficeToPDFConverter:
     def __init__(self, public_key, secret_key):
         """
         Initialize the converter with the public and secret keys.
 
         Parameters:
@@ -145,15 +147,20 @@
         Parameters:
         file_path (str): The path of the office file to convert.
         output_path (str): The path where the PDF should be saved.
 
         Returns:
         None
         """
+        # Create output directory if it doesn't exist
         try:
+            last_slash_index = output_path.rfind("/")
+            output_path_dir = output_path[:last_slash_index + 1]
+            os.makedirs(output_path_dir, exist_ok=True)
+
             logging.info("Starting conversion task...")
             server, task = self.start_task("officepdf")
             logging.info("Task started successfully.")
 
             logging.info("Uploading file...")
             server_filename = self.upload_file(server, task, file_path)
             logging.info("File uploaded successfully.")
@@ -163,51 +170,22 @@
             logging.info("File processed successfully.")
 
             logging.info("Downloading file...")
             self.download_file(server, task, output_path)
             logging.info("File downloaded successfully.")
         except Exception as e:
             logging.error(f"An error occurred: {e}")
-
-    def convert_bulk_to_pdf_not_working(self, file_paths, output_path):
-        """
-        Convert multiple office files to PDF in a bulk operation.
-
-        This method performs the following steps:
-        1. Starts a new 'officepdf' task.
-        2. Uploads each office file to the iLovePDF API.
-        3. Processes the uploaded files with the 'officepdf' tool.
-        4. Downloads the processed files as a ZIP archive from the iLovePDF API.
-
-        Parameters:
-        file_paths (list[str]): The list of file paths to convert.
-        output_path (str): The path where the resulting ZIP file should be saved.
-
-        Returns:
-        None
-        """
-        logging.info("Starting bulk conversion task...")
-        server, task = self.start_task("officepdf")
-        files = []
-        for file_path in file_paths:
-            server_filename = self.upload_file(server, task, file_path)
-            filename = os.path.basename(file_path)  # Get the original filename
-            files.append((server_filename, filename))
-            print('upload done: ' + server_filename + ' - ' + filename)
-        print(files)
-        self.process_files(server, task, files)
-        print("process files done")
-        logging.info("Downloading files for {}".format(task))
-        self.download_file(server, task, output_path)
-        print("download done")
+            raise APIException({"error": f"An error occurred:", "traceback": traceback.format_exc()})
 
     def convert_multiple_to_pdf(self, file_paths, output_dir):
         """
         Convert multiple office files to PDF.
         """
+        # Create output directory if it doesn't exist
+        os.makedirs(output_dir, exist_ok=True)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
             for file_path in file_paths:
                 filename = os.path.splitext(os.path.basename(file_path))[0]  # Get the original filename without the extension
                 output_path = os.path.join(output_dir, f"{filename}.pdf")
                 futures.append(executor.submit(self.convert_to_pdf, file_path, output_path))
```

### Comparing `LundPDFMaster-1.1.0/setup.py` & `LundPDFMaster-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="LundPDFMaster",
-    version="1.1.0",
+    version="1.1.1",
     author="Ensar Kaya",
     author_email="e.kaya@lund-it.com",
     description="A Python library for converting office files to PDF using the iLovePDF API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LundIT/LundPDFMaster",
     packages=find_packages(),
```

### Comparing `LundPDFMaster-1.1.0/tests/test_api.py` & `LundPDFMaster-1.1.1/tests/test_api.py`

 * *Files identical despite different names*

