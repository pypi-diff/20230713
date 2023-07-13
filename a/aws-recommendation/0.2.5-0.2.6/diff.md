# Comparing `tmp/aws_recommendation-0.2.5.tar.gz` & `tmp/aws_recommendation-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_recommendation-0.2.5.tar", last modified: Wed Jul 12 10:02:27 2023, max compression
+gzip compressed data, was "aws_recommendation-0.2.6.tar", last modified: Thu Jul 13 04:22:49 2023, max compression
```

## Comparing `aws_recommendation-0.2.5.tar` & `aws_recommendation-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/
--rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.5/LICENCE
--rw-rw-rw-   0        0        0     1220 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.003237 aws_recommendation-0.2.5/aws_recommendation/
--rw-rw-rw-   0        0        0     2329 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/aws_recommendation/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/cloudwatch.py
--rw-rw-rw-   0        0        0    11769 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/cost_estimations.py
--rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/aws_recommendation/dynamodb.py
--rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/ebs.py
--rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/ec2.py
--rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/elb.py
--rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/kms.py
--rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/rds.py
--rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/redshift.py
--rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/s3.py
--rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/truted_advisor.py
--rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.5/aws_recommendation/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/aws_recommendation.egg-info/
--rw-rw-rw-   0        0        0     1220 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-12 10:02:26.000000 aws_recommendation-0.2.5/aws_recommendation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      525 2023-07-12 09:59:38.000000 aws_recommendation-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 10:02:27.021112 aws_recommendation-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.647840 aws_recommendation-0.2.6/
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:22:06.000000 aws_recommendation-0.2.6/LICENCE
+-rw-rw-rw-   0        0        0     1220 2023-07-13 04:22:49.646837 aws_recommendation-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-04-04 11:43:43.000000 aws_recommendation-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.628540 aws_recommendation-0.2.6/aws_recommendation/
+-rw-rw-rw-   0        0        0     2329 2023-07-13 04:20:27.000000 aws_recommendation-0.2.6/aws_recommendation/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/cloudwatch.py
+-rw-rw-rw-   0        0        0    11861 2023-07-13 04:02:57.000000 aws_recommendation-0.2.6/aws_recommendation/cost_estimations.py
+-rw-rw-rw-   0        0        0     4296 2023-07-12 09:59:38.000000 aws_recommendation-0.2.6/aws_recommendation/dynamodb.py
+-rw-rw-rw-   0        0        0    15213 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/ebs.py
+-rw-rw-rw-   0        0        0    26661 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/ec2.py
+-rw-rw-rw-   0        0        0     8961 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/elb.py
+-rw-rw-rw-   0        0        0     4208 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/kms.py
+-rw-rw-rw-   0        0        0    11638 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/rds.py
+-rw-rw-rw-   0        0        0     5955 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/redshift.py
+-rw-rw-rw-   0        0        0    11003 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/s3.py
+-rw-rw-rw-   0        0        0     1726 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/truted_advisor.py
+-rw-rw-rw-   0        0        0     5821 2023-04-12 12:09:37.000000 aws_recommendation-0.2.6/aws_recommendation/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 04:22:49.642866 aws_recommendation-0.2.6/aws_recommendation.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-13 04:22:49.000000 aws_recommendation-0.2.6/aws_recommendation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      525 2023-07-13 04:20:27.000000 aws_recommendation-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 04:22:49.648356 aws_recommendation-0.2.6/setup.cfg
```

### Comparing `aws_recommendation-0.2.5/PKG-INFO` & `aws_recommendation-0.2.6/aws_recommendation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws_recommendation
-Version: 0.2.5
+Name: aws-recommendation
+Version: 0.2.6
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.5/README.md` & `aws_recommendation-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/__init__.py` & `aws_recommendation-0.2.6/aws_recommendation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Any
 
 from botocore.exceptions import ClientError
 
 from boto3 import session
 
 __author__ = "Dheeraj Banodha"
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 import logging
 
 from aws_recommendation.cloudwatch import cloudwatch
 from aws_recommendation.dynamodb import dynamodb
 from aws_recommendation.ebs import ebs
 from aws_recommendation.ec2 import ec2
```

### Comparing `aws_recommendation-0.2.5/aws_recommendation/cloudwatch.py` & `aws_recommendation-0.2.6/aws_recommendation/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/cost_estimations.py` & `aws_recommendation-0.2.6/aws_recommendation/cost_estimations.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,22 @@
     client = self.session.client('pricing', region_name='us-east-1')
     price1 = get_price(client=client, region=get_region_name(region), instance=from_instance, os=os)
 
     price2 = get_price(client=client, region=get_region_name(region), instance=to_instance, os=os)
 
     savings = ((float(price1) - float(price2)) / float(price1)) * 100
 
-    instance_list = list_instances(self, region)
+    instance_list = self.list_instances([region])
 
     count = 0
 
-    for instance in instance_list:
-        if instance['InstanceType'] == from_instance:
-            count = count + 1
+    for region, instances in instance_list.items():
+        for instance in instances:
+            if instance['InstanceType'] == from_instance:
+                count = count + 1
 
     if count == 0:
         return {
             'Flag' : False
         }
 
     # print(region)
@@ -225,37 +226,37 @@
                     try:
                         response = get_savings(self, region, instance_type, up[1], 'Linux')
                         response['upgrade_from'] = instance_type
                         response['upgrade_to'] = up[1]
                         if response['Flag']:
                             temp = merge(temp, response)
                     except botocore.exceptions.ClientError as e:
-                        logger.error("Something went wrong {}".format(e))
+                        logger.error("Something went wrong {}-{}".format('232', e))
                         temp = {
                             'Flag': True,
                             'current_cost': 0,
                             'Estimated Savings in %': 0,
                             'Estimated Monthly Saving': 0,
                             'Effective Monthly cost': 0,
                             'Number of Instances': count_instance,
                             'upgrade_from': instance_type,
                             'upgrade_to': up[1],
                             'reason': e.response['Error']['Code']
                         }
                     except IndexError as e:
-                        logger.error("Something went wrong {}".format(e))
+                        logger.error("Something went wrong {}-{}".format('245', e))
                     except Exception as e:
-                        logger.error("Something went wrong {}".format(e))
+                        logger.error("Something went wrong {}-{}".format('247', e))
                 # print(temp)
                 # print(len(temp))
-
-                recommendations.append(temp)
+                if temp:
+                    recommendations.append(temp)
 
     response = []
-    # print(recommendations)
+
     for recommendation in recommendations:
         # print('reason' in recommendation.keys())
         if 'reason' in recommendation:
             temp = {
                 'Service Name': 'EC2',
                 'Id': 'Generic',
                 'Recommendation': recommendation['reason'],
```

### Comparing `aws_recommendation-0.2.5/aws_recommendation/dynamodb.py` & `aws_recommendation-0.2.6/aws_recommendation/dynamodb.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/ebs.py` & `aws_recommendation-0.2.6/aws_recommendation/ebs.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/ec2.py` & `aws_recommendation-0.2.6/aws_recommendation/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/elb.py` & `aws_recommendation-0.2.6/aws_recommendation/elb.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/kms.py` & `aws_recommendation-0.2.6/aws_recommendation/kms.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/rds.py` & `aws_recommendation-0.2.6/aws_recommendation/rds.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/redshift.py` & `aws_recommendation-0.2.6/aws_recommendation/redshift.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/s3.py` & `aws_recommendation-0.2.6/aws_recommendation/s3.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/truted_advisor.py` & `aws_recommendation-0.2.6/aws_recommendation/truted_advisor.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation/utils.py` & `aws_recommendation-0.2.6/aws_recommendation/utils.py`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/aws_recommendation.egg-info/PKG-INFO` & `aws_recommendation-0.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aws-recommendation
-Version: 0.2.5
+Name: aws_recommendation
+Version: 0.2.6
 Summary: Provides AWS recommendations
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `aws_recommendation-0.2.5/aws_recommendation.egg-info/SOURCES.txt` & `aws_recommendation-0.2.6/aws_recommendation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_recommendation-0.2.5/pyproject.toml` & `aws_recommendation-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_recommendation"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="dheeraj.banodha", email="dheerajmbanodha@gmail.com" },
 ]
 description = "Provides AWS recommendations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

