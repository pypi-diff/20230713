# Comparing `tmp/wizata-dsapi-0.2.8.tar.gz` & `tmp/wizata-dsapi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.8.tar", last modified: Tue Jul 11 12:31:02 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.2.9.tar", last modified: Wed Jul 12 20:16:16 2023, max compression
```

## Comparing `wizata-dsapi-0.2.8.tar` & `wizata-dsapi-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.322145 wizata-dsapi-0.2.8/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-11 12:31:02.321662 wizata-dsapi-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.2.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 12:31:02.322641 wizata-dsapi-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-11 12:30:48.000000 wizata-dsapi-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.298178 wizata-dsapi-0.2.8/wizata_dsapi/
--rw-rw-rw-   0        0        0     1014 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-19 13:45:53.000000 wizata-dsapi-0.2.8/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     6145 2023-07-11 12:30:48.000000 wizata-dsapi-0.2.8/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.8/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.2.8/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-21 05:55:35.000000 wizata-dsapi-0.2.8/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-06-21 08:28:14.000000 wizata-dsapi-0.2.8/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-06 16:17:20.000000 wizata-dsapi-0.2.8/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.2.8/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     7221 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-06-22 14:06:45.000000 wizata-dsapi-0.2.8/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2762 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.2.8/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56463 2023-07-11 07:58:59.000000 wizata-dsapi-0.2.8/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-11 12:31:02.319690 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-11 12:31:02.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-11 12:31:01.000000 wizata-dsapi-0.2.8/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.624118 wizata-dsapi-0.2.9/
+-rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      176 2023-07-12 20:16:16.621516 wizata-dsapi-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-12 20:16:16.624118 wizata-dsapi-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-07-12 20:15:59.000000 wizata-dsapi-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.572322 wizata-dsapi-0.2.9/wizata_dsapi/
+-rw-rw-rw-   0        0        0     1014 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.9/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.9/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     6145 2023-07-12 07:57:04.000000 wizata-dsapi-0.2.9/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.9/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.9/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.9/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.9/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.9/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.9/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.9/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     7221 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2762 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.9/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56573 2023-07-12 20:15:59.000000 wizata-dsapi-0.2.9/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.614691 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.8/LICENSE.txt` & `wizata-dsapi-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/setup.py` & `wizata-dsapi-0.2.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.2.8',
+    version='0.2.9',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/__init__.py` & `wizata-dsapi-0.2.9/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.2.9/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.2.9/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.2.9/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.2.9/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.2.9/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/execution.py` & `wizata-dsapi-0.2.9/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/experiment.py` & `wizata-dsapi-0.2.9/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.2.9/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.2.9/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.2.9/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/plot.py` & `wizata-dsapi-0.2.9/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/request.py` & `wizata-dsapi-0.2.9/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/script.py` & `wizata-dsapi-0.2.9/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/template.py` & `wizata-dsapi-0.2.9/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/twin.py` & `wizata-dsapi-0.2.9/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.2.9/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.2.9/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,14 +477,16 @@
                                      data=dill.dumps(obj))
             if response.status_code == 200:
                 obj.script_id = uuid.UUID(response.json()["id"])
                 return obj.script_id
             else:
                 raise self.__raise_error(response)
         elif isinstance(obj, Experiment):
+            if len(obj.key) > 16:
+                raise ValueError('experiment key is limited to 16 char.')
             response = requests.post(self.__url() + "experiments/",
                                      headers=self.__header(),
                                      data=json.dumps(obj.to_json()))
             if response.status_code == 200:
                 return
             else:
                 raise self.__raise_error(response)
```

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.2.9/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.2.8/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.2.9/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

