# Comparing `tmp/ezsmdeploy-1.8.dev0.tar.gz` & `tmp/ezsmdeploy-1.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploy-1.8.dev0.tar", last modified: Sat Jul  8 16:43:59 2023, max compression
+gzip compressed data, was "ezsmdeploy-1.9.dev0.tar", last modified: Thu Jul 13 20:56:03 2023, max compression
```

## Comparing `ezsmdeploy-1.8.dev0.tar` & `ezsmdeploy-1.9.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-08 16:43:59.658506 ezsmdeploy-1.8.dev0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16845 2023-07-08 16:43:59.654505 ezsmdeploy-1.8.dev0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16356 2023-07-08 16:40:19.000000 ezsmdeploy-1.8.dev0/README.rst
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-08 16:43:59.654505 ezsmdeploy-1.8.dev0/ezsmdeploy/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    45923 2023-07-08 16:40:17.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-08 16:43:59.654505 ezsmdeploy-1.8.dev0/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/conversation.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-08 14:37:12.000000 ezsmdeploy-1.8.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-08 16:43:59.654505 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16845 2023-07-08 16:43:59.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-08 16:43:59.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-08 16:43:59.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-08 16:36:05.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-08 16:43:59.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-08 16:43:59.000000 ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-08 16:43:59.658506 ezsmdeploy-1.8.dev0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1273 2023-07-08 16:39:42.000000 ezsmdeploy-1.8.dev0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16911 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16422 2023-07-13 20:44:23.000000 ezsmdeploy-1.9.dev0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.275466 ezsmdeploy-1.9.dev0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    47399 2023-07-13 20:30:04.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16911 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:11:33.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1273 2023-07-13 20:11:18.000000 ezsmdeploy-1.9.dev0/setup.py
```

### Comparing `ezsmdeploy-1.8.dev0/PKG-INFO` & `ezsmdeploy-1.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.8.dev0
+Version: 1.9.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -56,17 +56,19 @@
 -------------------
 1. Added support for SageMaker Jumpstart foundational models
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
+    - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
-    - openchat/openchat, ml.g5.2xlarge
+    - openchat/openchat, ml.g5.24xlarge
+    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
```

### Comparing `ezsmdeploy-1.8.dev0/README.rst` & `ezsmdeploy-1.9.dev0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,19 @@
 -------------------
 1. Added support for SageMaker Jumpstart foundational models
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
+    - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
-    - openchat/openchat, ml.g5.2xlarge
+    - openchat/openchat, ml.g5.24xlarge
+    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
```

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/__init__.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import boto3
 import glob
 import os
 import shutil
 import pkg_resources
 import subprocess
 from sagemaker.multidatamodel import MultiDataModel
+from sagemaker.serverless import ServerlessInferenceConfig
 from sagemaker.model import Model
 import ast
 import csv
 import json
 import pickle
 import time
 import cmd
@@ -54,14 +55,17 @@
         model,
         script=None,
         framework=None,
         requirements=None,
         name=None,
         autoscale=False,
         autoscaletarget=1000,
+        serverless=False,
+        serverless_memory=4096,
+        serverless_concurrency=100,
         wait=True,
         bucket=None,
         prefix='',
         session=None,
         image=None,
         dockerfilepath=None,
         instance_type=None,
@@ -95,15 +99,22 @@
         self.monitor = monitor
         self.deployed = False
         self.autoscaletarget = autoscaletarget
         self.foundation_model = foundation_model
         self.foundation_model_version = foundation_model_version
         self.huggingface_model = huggingface_model
         self.huggingface_model_task = huggingface_model_task
+        self.serverless = serverless
         
+        if serverless:
+            self.serverless_config = ServerlessInferenceConfig(
+                memory_size_in_mb=serverless_memory, max_concurrency=serverless_concurrency)
+        else:
+            self.serverless_config = None
+            
         self.huggingface_model_quantize = huggingface_model_quantize
 
         # ------ load cost types dict ---------
         costpath = pkg_resources.resource_filename("ezsmdeploy", "data/cost.csv")
         self.costdict = {}
         with open(costpath, mode="r") as infile:
             reader = csv.reader(infile)
@@ -251,75 +262,76 @@
         self.wait = wait
         self.deploy()
 
     
     
     def deploy_huggingface_model(self):
         
-        if self.instance_type == None:
+        if self.instance_type == None and not self.serverless:
             raise ValueError("Please enter a valid instance type, not [None]")
         
         # from sagemaker.huggingface.model import HuggingFaceModel, get_huggingface_llm_image_uri
         from sagemaker.huggingface import HuggingFaceModel, get_huggingface_llm_image_uri
         
         self.model = self.model[0]
         hub = {
             'HF_MODEL_ID':self.model,                # model_id from hf.co/models
         }
         
         
         if self.huggingface_model_task is not None:
              hub['HF_TASK'] = self.huggingface_model_task    # NLP task you want to use for predictions
+        
+        if not self.serverless: #ignore instance type checks, and ignore fallback. Also ignore quantization
+            try:
+                ec2_client = boto3.client("ec2")
+                resp = ec2_client.describe_instance_types(InstanceTypes=[self.instance_type.strip("ml.")])['InstanceTypes'][0]
+                if 'GpuInfo' in resp:
+                    hub['SM_NUM_GPUS']= json.dumps(resp['GpuInfo']['Gpus'][0]['Count'])
+                else:
+                    pass
+            except Exception as e:
+                print(e, end=" ... ")
+                print("Trying fallback to figure out number of GPUs in the instance type you chose - ")
+                hub['SM_NUM_GPUS']= json.dumps(0) # Use at least 0 GPU by default. else:
+                if 'g' in self.instance_type:
+                    hub['SM_NUM_GPUS']= json.dumps(1)
+                    if '12x' in self.instance_type:
+                        hub['SM_NUM_GPUS']= json.dumps(4)
+                    elif '24x' in self.instance_type:
+                        hub['SM_NUM_GPUS']= json.dumps(4)
+                    elif '48x' in self.instance_type:
+                        hub['SM_NUM_GPUS']= json.dumps(4)
+                elif 'p2' in self.instance_type:
+                    hub['SM_NUM_GPUS']= json.dumps(1)
+                    if '8x' in self.instance_type:
+                        hub['SM_NUM_GPUS']=json.dumps(8)
+                    elif '16x' in self.instance_type:
+                        hub['SM_NUM_GPUS']=json.dumps(16)
+                elif 'p3' in self.instance_type:
+                    hub['SM_NUM_GPUS']= json.dumps(1)
+                    if '8x' in self.instance_type:
+                        hub['SM_NUM_GPUS']=json.dumps(4)
+                    elif '16x' in self.instance_type:
+                        hub['SM_NUM_GPUS']=json.dumps(8)
+                    elif '24x' in self.instance_type:
+                        hub['SM_NUM_GPUS']=json.dumps(8)
+                elif 'p4' in self.instance_type:
+                    hub['SM_NUM_GPUS']=json.dumps(8)
 
-        try:
-            ec2_client = boto3.client("ec2")
-            resp = ec2_client.describe_instance_types(InstanceTypes=[self.instance_type.strip("ml.")])['InstanceTypes'][0]
-            if 'GpuInfo' in resp:
-                hub['SM_NUM_GPUS']= json.dumps(resp['GpuInfo']['Gpus'][0]['Count'])
-            else:
+
+
+
+            if self.huggingface_model_quantize in ['bitsandbytes', 'gptq']:
+                hub['HF_MODEL_QUANTIZE'] = self.huggingface_model_quantize
+            elif self.huggingface_model_quantize==None:
                 pass
-        except Exception as e:
-            print(e, end=" ... ")
-            print("Trying fallback to figure out number of GPUs in the instance type you chose - ")
-            hub['SM_NUM_GPUS']= json.dumps(0) # Use at least 0 GPU by default. else:
-            if 'g' in self.instance_type:
-                hub['SM_NUM_GPUS']= json.dumps(1)
-                if '12x' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(4)
-                elif '24x' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(4)
-                elif '48x' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(4)
-            elif 'p2' in self.instance_type:
-                hub['SM_NUM_GPUS']= json.dumps(1)
-                if '8x' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(8)
-                elif '16x' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(16)
-            elif 'p3' in self.instance_type:
-                hub['SM_NUM_GPUS']= json.dumps(1)
-                if '8x' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(4)
-                elif '16x' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(8)
-                elif '24x' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(8)
-            elif 'p4' in self.instance_type:
-                hub['SM_NUM_GPUS']=json.dumps(8)
-            
-                
+            else:
+                raise ValueError(f"huggingface_model_quantize needs to be one of bitsandbytes, gptq, not {self.huggingface_model_quantize}")
 
-                
-        if self.huggingface_model_quantize in ['bitsandbytes', 'gptq']:
-            hub['HF_MODEL_QUANTIZE'] = self.huggingface_model_quantize
-        elif self.huggingface_model_quantize==None:
-            pass
-        else:
-            raise ValueError(f"huggingface_model_quantize needs to be one of bitsandbytes, gptq, not {self.huggingface_model_quantize}")
-        
         
         
         aws_role = sagemaker.get_execution_role()
         endpoint_name = name="hf-model-" + self.name
         
         # create Hugging Face Model Class
         self.sagemakermodel = HuggingFaceModel(
@@ -573,50 +585,62 @@
             data_capture_config = DataCaptureConfig(
                 enable_capture=True,
                 sampling_percentage=100,
                 destination_s3_uri=tmps3uri
             )
         else:
             data_capture_config = None
-
+        
+        if self.instance_type is not None:
+                if "p3" in self.instance_type or "16x" in self.instance_type or "24x" in self.instance_type or "48x" in self.instance_type or self.foundation_model:
+                    volume_size = 256 
+                else:
+                    volume_size = None
+        else:
+            volume_size = None 
+            
+        
         if self.foundation_model:
             # deploy the Model. Note that we need to pass Predictor class when we deploy model through Model class,
             # for being able to run inference through the sagemaker API.
-            volume_size = 256 if "p3" in self.instance_type else None
-            
+
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 predictor_cls=sagemaker.predictor.Predictor,
                 endpoint_name="ezsm-foundation-endpoint-" + self.name,
                 volume_size=volume_size,
+                # serverless_inference_config=self.serverless_config, #ignoring serverless inference
                 wait=self.wait
             )
         elif self.huggingface_model:
-            volume_size = 256 if "p3" in self.instance_type else None
+            
             
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 endpoint_name="ezsm-hf-endpoint-" + self.name,
                 volume_size=volume_size,
+                serverless_inference_config=self.serverless_config,
                 wait=self.wait,
                 container_startup_health_check_timeout=300,
             )
                 
             
         else:
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 accelerator_type=self.ei,
                 endpoint_name="ezsm-endpoint-" + self.name,
                 update_endpoint=False,
                 wait=self.wait,
+                volume_size=volume_size,
                 data_capture_config=data_capture_config,
+                serverless_inference_config=self.serverless_config,
                 container_startup_health_check_timeout=300,
             )
 
         self.endpoint_name = "ezsm-endpoint-" + self.name
 
     def get_size(self, bucket, path):
         s3 = boto3.resource("s3")
@@ -1005,19 +1029,26 @@
                     self.deploy_foundation_model()
                 elif self.huggingface_model:
                     self.deploy_huggingface_model()
                 else:
                     raise ValueError("Did not find model artifact, or foundation/huggingface model")
                 
             sp.hide()
-            sp.write(
-                str(datetime.datetime.now() - start)
-                + " | created model(s). Now deploying on "
-                + self.instance_type
-            )
+            
+            if not self.serverless:
+                sp.write(
+                    str(datetime.datetime.now() - start)
+                    + " | created model(s). Now deploying on "
+                    + self.instance_type
+                )
+            else:
+                sp.write(
+                    str(datetime.datetime.now() - start)
+                    + " | created model(s). Now deploying on Serverless!"
+                )
             sp.show()
 
             # deploy model
             self.deploy_model()
             sp.hide()
             sp.write(str(datetime.datetime.now() - start) + " | deployed model")
             sp.show()
```

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/serve` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploy-1.9.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.8.dev0
+Version: 1.9.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -56,17 +56,19 @@
 -------------------
 1. Added support for SageMaker Jumpstart foundational models
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
+    - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
-    - openchat/openchat, ml.g5.2xlarge
+    - openchat/openchat, ml.g5.24xlarge
+    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
```

### Comparing `ezsmdeploy-1.8.dev0/ezsmdeploy.egg-info/SOURCES.txt` & `ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.8.dev0/setup.py` & `ezsmdeploy-1.9.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.8dev',
+      version='1.9dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
```

