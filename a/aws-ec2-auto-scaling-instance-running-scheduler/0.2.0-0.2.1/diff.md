# Comparing `tmp/aws-ec2-auto-scaling-instance-running-scheduler-0.2.0.tar.gz` & `tmp/aws-ec2-auto-scaling-instance-running-scheduler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ec2-auto-scaling-instance-running-scheduler-0.2.0.tar", last modified: Thu Jul 13 10:34:31 2023, max compression
+gzip compressed data, was "aws-ec2-auto-scaling-instance-running-scheduler-0.2.1.tar", last modified: Thu Jul 13 19:16:20 2023, max compression
```

## Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0.tar` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:34:31.003472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 10:34:31.003472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:34:31.003472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:34:30.999472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:34:30.999472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:34:31.003472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.2.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:34:14.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:34:31.003472 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 10:34:30.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 10:34:30.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:34:30.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 10:34:30.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 10:34:30.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.2.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:16:07.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:16:20.498695 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-13 19:16:20.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-13 19:16:20.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:16:20.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 19:16:20.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 19:16:20.000000 aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/LICENSE` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/PKG-INFO` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-auto-scaling-instance-running-scheduler
-Version: 0.2.0
+Version: 0.2.1
 Summary: AWS EC2 AutoScaling Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/README.md` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/setup.py` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ec2-auto-scaling-instance-running-scheduler",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "description": "AWS EC2 AutoScaling Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_ec2_auto_scaling_instance_running_scheduler",
         "aws_ec2_auto_scaling_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "aws_ec2_auto_scaling_instance_running_scheduler._jsii": [
-            "aws-ec2-auto-scaling-instance-running-scheduler@0.2.0.jsii.tgz"
+            "aws-ec2-auto-scaling-instance-running-scheduler@0.2.1.jsii.tgz"
         ],
         "aws_ec2_auto_scaling_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-auto-scaling-instance-running-scheduler
-Version: 0.2.0
+Version: 0.2.1
 Summary: AWS EC2 AutoScaling Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-ec2-auto-scaling-instance-running-scheduler-0.2.0/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt` & `aws-ec2-auto-scaling-instance-running-scheduler-0.2.1/src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
 src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO
 src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
 src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
 src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
 src/aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
 src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
-src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.2.0.jsii.tgz
+src/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.2.1.jsii.tgz
```

