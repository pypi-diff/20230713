# Comparing `tmp/ML-Algo-1.2.6.tar.gz` & `tmp/ML-Algo-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.6.tar", last modified: Thu Jul 13 06:49:07 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.7.tar", last modified: Thu Jul 13 09:37:57 2023, max compression
```

## Comparing `ML-Algo-1.2.6.tar` & `ML-Algo-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.382434 ML-Algo-1.2.6/
-drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.368728 ML-Algo-1.2.6/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.6/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.6/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.6/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.6/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.6/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0     2124 2023-07-13 06:48:22.000000 ML-Algo-1.2.6/ML_Algo/TestRun.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.6/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.379432 ML-Algo-1.2.6/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0     2155 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2155 2023-07-13 06:49:07.381433 ML-Algo-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-13 06:49:07.382434 ML-Algo-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-07-13 06:47:24.000000 ML-Algo-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/
+drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.026329 ML-Algo-1.2.7/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.7/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.7/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.7/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.7/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.7/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0     2186 2023-07-13 09:36:50.000000 ML-Algo-1.2.7/ML_Algo/TestRun.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.7/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:37:57.031331 ML-Algo-1.2.7/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0     2155 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 09:37:56.000000 ML-Algo-1.2.7/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2155 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:37:57.032328 ML-Algo-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-13 09:37:06.000000 ML-Algo-1.2.7/setup.py
```

### Comparing `ML-Algo-1.2.6/ML_Algo/DataCleaning.py` & `ML-Algo-1.2.7/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.6/ML_Algo/FetchData.py` & `ML-Algo-1.2.7/ML_Algo/FetchData.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.6/ML_Algo/Predictions.py` & `ML-Algo-1.2.7/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.6/ML_Algo/Series_Data.py` & `ML-Algo-1.2.7/ML_Algo/Series_Data.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.6/ML_Algo/Series_Time.py` & `ML-Algo-1.2.7/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.6/ML_Algo/TestRun.py` & `ML-Algo-1.2.7/ML_Algo/TestRun.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,23 +29,23 @@
     elif t >= 3:
         pred = pred_data.iloc[:,t-2:t+1]
         return pred.stack().dropna().tolist()
     
 def get_test_next_pred(pred,next_pred_intervals=8,t=0):
     return pred.iloc[:,t:t+next_pred_intervals].stack().dropna().tolist()    
 
-def Test_Predict(combine_df,jump=8):
+def Test_Predict(combine_df,jump=8,next_pred_intervals=8):
     yesterday = combine_df.iloc[2:,:]
     today = combine_df.iloc[1:2,:]
     pred_data = combine_df.iloc[:1,:]
     Complete_Day = []
     for i in range (0,97,jump):
         l = get_test_live_data(yesterday,today,t=i)
         p = get_test_pred_data(yesterday,pred_data,t=i)
-        n = get_test_next_pred(pred_data,t=i)
+        n = get_test_next_pred(pred_data,next_pred_intervals=next_pred_intervals,t=i)
         # print(i)
         prev_day_err = (np.array(l)-np.array(p))/np.array(l)
         prev_day_err = prev_day_err.mean()
         # print(prev_day_err)
         # print(n)
         output_values= []
         for i in n:
```

### Comparing `ML-Algo-1.2.6/ML_Algo.egg-info/PKG-INFO` & `ML-Algo-1.2.7/ML_Algo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.6
+Version: 1.2.7
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.6 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.7 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
```

### Comparing `ML-Algo-1.2.6/PKG-INFO` & `ML-Algo-1.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ML-Algo
-Version: 1.2.6
+Version: 1.2.7
 Summary: A package for calculating Series Time Data
 Author: Mr Raj
 Author-email: arunraj14092002@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.6 Summary: A package for
+Metadata-Version: 2.1 Name: ML-Algo Version: 1.2.7 Summary: A package for
 calculating Series Time Data Author: Mr Raj Author-email:
 arunraj14092002@gmail.com Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
```

### Comparing `ML-Algo-1.2.6/setup.py` & `ML-Algo-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ML-Algo',
-    version='1.2.6',
+    version='1.2.7',
     author='Mr Raj',
     author_email='arunraj14092002@gmail.com',
     description='A package for calculating Series Time Data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['ML_Algo'],
     install_requires=['pandas','requests'],
```

