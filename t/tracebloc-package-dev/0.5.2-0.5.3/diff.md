# Comparing `tmp/tracebloc_package-dev-0.5.2.tar.gz` & `tmp/tracebloc_package-dev-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.2.tar", last modified: Mon Jul 10 04:43:01 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.3.tar", last modified: Thu Jul 13 07:56:19 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.2.tar` & `tracebloc_package-dev-0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.396218 tracebloc_package-dev-0.5.2/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.2/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-10 04:43:01.396308 tracebloc_package-dev-0.5.2/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.2/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-07-10 04:43:01.396578 tracebloc_package-dev-0.5.2/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-07-10 04:41:35.000000 tracebloc_package-dev-0.5.2/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.395278 tracebloc_package-dev-0.5.2/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.2/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.2/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    24334 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    59315 2023-07-10 04:42:36.000000 tracebloc_package-dev-0.5.2/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.2/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.2/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-07-06 09:36:33.000000 tracebloc_package-dev-0.5.2/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.2/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-10 04:43:01.396103 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-07-10 04:43:01.000000 tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.517095 tracebloc_package-dev-0.5.3/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.3/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-07-13 07:56:19.517203 tracebloc_package-dev-0.5.3/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.3/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-07-13 07:56:19.517907 tracebloc_package-dev-0.5.3/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-07-13 07:56:12.000000 tracebloc_package-dev-0.5.3/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.515689 tracebloc_package-dev-0.5.3/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.3/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.3/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    24334 2023-07-04 07:32:00.000000 tracebloc_package-dev-0.5.3/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    59195 2023-07-13 07:56:12.000000 tracebloc_package-dev-0.5.3/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.5.3/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10936 2023-06-23 11:15:51.000000 tracebloc_package-dev-0.5.3/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.3/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     6712 2023-06-23 11:15:51.000000 tracebloc_package-dev-0.5.3/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.3/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-07-13 07:56:19.516931 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-07-13 07:56:19.000000 tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.2/LICENSE.txt` & `tracebloc_package-dev-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/PKG-INFO` & `tracebloc_package-dev-0.5.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.2
+Version: 0.5.3
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.2/setup.py` & `tracebloc_package-dev-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.2",
+    version="0.5.3",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,31 +183,31 @@
         creates sub dataset of the current dataset of the no of images per class selected by user
         Please provide number of images per class
         example: dataset: {'car': 65, 'person': 42}
         Classes in dataset car, person
 
         trainingObject.trainingClasses({'car': 30, 'person': 30})
         """
-        checkeligible = True
+        check_eligible = True
         class_names = self.__class_names.keys()
         for class_name in class_names:
             num_images = int(self.__class_names[class_name])
             if class_name in training_dataset.keys():
                 value = training_dataset[class_name]
                 if 0 < value <= num_images:
                     pass
                 else:
-                    checkeligible = False
+                    check_eligible = False
                     error_msg = f"Please provide num of images for class {class_name} greater than 0 and less than equal to {num_images}"
                     self.__print_error(error_msg)
             else:
-                checkeligible = False
+                check_eligible = False
                 error_msg = "trainingDatasetSize dictionary must contain all classes that are present in the dataset. Customisation in terms of classes is not allowed."
                 self.__print_error(error_msg)
-        if checkeligible:
+        if check_eligible:
             self.__trainingClasses = training_dataset
             self.__trainingDatasetSize = getImagesCount(training_dataset)
             self.__subdataset = json.dumps(
                 {
                     "trainingDatasetSize": self.__trainingDatasetSize,
                     "trainingClasses": self.__trainingClasses,
                 }
@@ -289,28 +289,25 @@
         """
         Set image type to be used for training
         parameters: string type values.
         supported type: ['rgb', 'gray']
         example: trainingObject.imageType('rgb')
         default: rgb
         """
-        if self.__framework == TENSORFLOW_FRAMEWORK:
-            allowed_types = ["rgb", "grayscale"]
-            try:
-                if type(image_type) is str:
-                    allowed_types.index(image_type.lower())
-                    self.__image_type = image_type.lower()
+        allowed_types = ["rgb", "grayscale"]
+        try:
+            if type(image_type) is str:
+                allowed_types.index(image_type.lower())
+                self.__image_type = image_type.lower()
+                if self.__framework == TENSORFLOW_FRAMEWORK:
                     self.__update_image_model()
-                    self.__remove_error_method()
-            except:
-                error_msg = "Enter values from supported values only "
-                self.__print_error(error_msg)
-        else:
-            error_msg = "for pytorch only rgb is supported"
-            self.__not_supported_parameters(error_msg)
+                self.__remove_error_method()
+        except:
+            error_msg = "Enter values from supported values only "
+            self.__print_error(error_msg)
 
     def seed(self, seed: bool):
         """
         Boolean.
         Sets the global random seed when selected
         default: False
         example:trainingObject.seed(True)
@@ -1339,14 +1336,15 @@
             "epochs": self.__epochs,
             "cycles": self.__cycles,
             "modelName": self.__modelId,
             "optimizer": self.__optimizer,
             "lossFunction": json.dumps(self.__lossFunction),
             "learningRate": json.dumps(self.__learningRate),
             "batchSize": self.__batchSize,
+            "seed": self.__seed,
             "featurewise_center": self.__featurewise_center,
             "samplewise_center": self.__samplewise_center,
             "featurewise_std_normalization": self.__featurewise_std_normalization,
             "samplewise_std_normalization": self.__samplewise_std_normalization,
             "zca_whitening": self.__zca_whitening,
             "rotation_range": self.__rotation_range,
             "width_shift_range": self.__width_shift_range,
```

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.3/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.2
+Version: 0.5.3
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.2/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.3/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

