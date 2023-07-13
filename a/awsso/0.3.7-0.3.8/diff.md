# Comparing `tmp/awsso-0.3.7.tar.gz` & `tmp/awsso-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsso-0.3.7.tar", last modified: Wed Mar 29 10:27:56 2023, max compression
+gzip compressed data, was "awsso-0.3.8.tar", last modified: Thu Jul 13 06:20:04 2023, max compression
```

## Comparing `awsso-0.3.7.tar` & `awsso-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-03-29 10:27:56.501994 awsso-0.3.7/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-03-29 10:27:56.501275 awsso-0.3.7/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.3.7/README.md
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-03-29 10:27:56.496610 awsso-0.3.7/awsso/
--rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.3.7/awsso/__init__.py
--rwxr-xr-x   0 hanpenny   (501) staff       (20)    29585 2023-03-29 10:20:27.000000 awsso-0.3.7/awsso/awsso.py
-drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-03-29 10:27:56.500666 awsso-0.3.7/awsso.egg-info/
--rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/PKG-INFO
--rw-r--r--   0 hanpenny   (501) staff       (20)      227 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/SOURCES.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        1 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/dependency_links.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       43 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/entry_points.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       60 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/requires.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)        6 2023-03-29 10:27:56.000000 awsso-0.3.7/awsso.egg-info/top_level.txt
--rw-r--r--   0 hanpenny   (501) staff       (20)       38 2023-03-29 10:27:56.502122 awsso-0.3.7/setup.cfg
--rw-r--r--   0 hanpenny   (501) staff       (20)      986 2023-03-29 10:27:43.000000 awsso-0.3.7/setup.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.842235 awsso-0.3.8/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:20:04.841743 awsso-0.3.8/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      611 2023-02-06 15:29:04.000000 awsso-0.3.8/README.md
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.837230 awsso-0.3.8/awsso/
+-rw-r--r--   0 hanpenny   (501) staff       (20)        0 2023-02-06 14:12:11.000000 awsso-0.3.8/awsso/__init__.py
+-rwxr-xr-x   0 hanpenny   (501) staff       (20)    32318 2023-07-13 06:19:31.000000 awsso-0.3.8/awsso/awsso.py
+drwxr-xr-x   0 hanpenny   (501) staff       (20)        0 2023-07-13 06:20:04.841126 awsso-0.3.8/awsso.egg-info/
+-rw-r--r--   0 hanpenny   (501) staff       (20)     1028 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/PKG-INFO
+-rw-r--r--   0 hanpenny   (501) staff       (20)      227 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/SOURCES.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        1 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/dependency_links.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       43 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/entry_points.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       60 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/requires.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)        6 2023-07-13 06:20:04.000000 awsso-0.3.8/awsso.egg-info/top_level.txt
+-rw-r--r--   0 hanpenny   (501) staff       (20)       38 2023-07-13 06:20:04.842391 awsso-0.3.8/setup.cfg
+-rw-r--r--   0 hanpenny   (501) staff       (20)      986 2023-07-13 06:04:51.000000 awsso-0.3.8/setup.py
```

### Comparing `awsso-0.3.7/PKG-INFO` & `awsso-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.3.7
+Version: 0.3.8
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.3.7/README.md` & `awsso-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `awsso-0.3.7/awsso/awsso.py` & `awsso-0.3.8/awsso/awsso.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,14 +154,31 @@
     parser_sm_update.set_defaults(func=_sm_update)
 
     parser_sm_delete = parser_sm_sub.add_parser('delete',
                         help='delete secrets manager')
     parser_sm_delete.add_argument('secret')
     parser_sm_delete.set_defaults(func=_sm_delete)
 
+    parser_ssm = subparsers.add_parser('ssm')
+    parser_ssm_sub = parser_ssm.add_subparsers()
+    parser_ssm_search = parser_ssm_sub.add_parser('search',
+                        help='search parameters')
+    parser_ssm_search.add_argument('parameter')
+    parser_ssm_search.set_defaults(func=_ssm_search)
+
+    parser_ssm_get = parser_ssm_sub.add_parser('get',
+                        help='get parameter value')
+    parser_ssm_get.add_argument('parameter')
+    parser_ssm_get.set_defaults(func=_ssm_get)
+
+    parser_ssm_delete = parser_ssm_sub.add_parser('delete',
+                        help='delete parameter value')
+    parser_ssm_delete.add_argument('parameter')
+    parser_ssm_delete.set_defaults(func=_ssm_delete)
+
     parser_image = subparsers.add_parser('image')
     parser_image_sub = parser_image.add_subparsers()
     parser_image_list = parser_image_sub.add_parser('list',
                         help='list service images.')
     parser_image_list.add_argument('service')
     parser_image_list.set_defaults(func=_image_list)
 
@@ -225,14 +242,20 @@
             _sm_get(args.secret)
         if args.func == _sm_create:
             _sm_create()
         if args.func == _sm_update:
             _sm_update(args.secret)
         if args.func == _sm_delete:
             _sm_delete(args.secret)
+        if args.func == _ssm_search:
+            _ssm_search(args.parameter)
+        if args.func == _ssm_get:
+            _ssm_get(args.parameter)
+        if args.func == _ssm_delete:
+            _ssm_delete(args.parameter)
         if args.func == _image_list:
             _image_list(args.service)
         if args.func == _image_pull:
             _image_pull(args.image)
         if args.func == _image_run:
             _image_run(args.service, args.tag)
 
@@ -685,14 +708,71 @@
             ForceDeleteWithoutRecovery=True
         )
         print(ret)
     else:
         print('The sm: {} will not be deleted'.format(keyword))
         sys.exit()
 
+def _ssm_search(keyword):
+    client = boto3.client('ssm', region_name=CURRENT_REGION)
+    _filter = [
+        {
+            'Key': 'Name',
+            'Option': 'Contains',
+            'Values': [ keyword ]
+        }
+    ]
+    ret = client.describe_parameters(ParameterFilters=_filter, MaxResults=50)
+    _ret_list = ret['Parameters']
+    _next = ret.get('NextToken')
+    while _next:
+        ret_tmp = client.describe_parameters(ParameterFilters=_filter, MaxResults=50, NextToken=_next)
+        _ret_list.extend(ret_tmp['Parameters'])
+        _next = ret_tmp.get('NextToken')
+
+    ret_list = [ i['Name'] for i in _ret_list ]
+
+    if len(ret_list) == 0:
+        print('Did not find any parameters.')
+        sys.exit()
+    questions = [
+        inquirer.List(
+            'name',
+            message='Please select parameter',
+            choices=ret_list
+        ),
+    ]
+    answer = inquirer.prompt(questions)
+    ret = client.get_parameter(Name=answer['name'], WithDecryption=True)
+    print(ret['Parameter']['Value'])
+
+def _ssm_get(keyword):
+    client = boto3.client('ssm', region_name=CURRENT_REGION)
+    try:
+        ret = client.get_parameter(Name=keyword, WithDecryption=True)
+        print(ret['Parameter']['Value'])
+    except:
+        print('Get parameter error.')
+        sys.exit(1)
+
+def _ssm_delete(keyword):
+    client = boto3.client('ssm', region_name=CURRENT_REGION)
+    data = input('Please confirm this deletion[y/n]: ')
+    if data.strip().lower() == 'y':
+        print('The ssm: {} will be deleted'.format(keyword))
+        try:
+            ret = client.delete_parameter(Name=keyword)
+            print(ret)
+        except client.exceptions.ParameterNotFound:
+            print('Pamameter not found.')
+    else:
+        print('Cancelled.')
+        sys.exit()
+
+
 def _env_get(service):
 
     def GetPathToken(path, Token):
 
         try:
             client = boto3.client('ssm')
             rc = client.get_parameters_by_path(
```

### Comparing `awsso-0.3.7/awsso.egg-info/PKG-INFO` & `awsso-0.3.8/awsso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsso
-Version: 0.3.7
+Version: 0.3.8
 Summary: aws command line tool
 Home-page: https://github.com/Hireteammate/tools.git
 Author: linhan
 Author-email: lynnpen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `awsso-0.3.7/setup.py` & `awsso-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import awsso
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="awsso",
-    version="0.3.7",
+    version="0.3.8",
     author="linhan",
     author_email="lynnpen@gmail.com",  
     description="aws command line tool",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/Hireteammate/tools.git",
     packages=setuptools.find_packages(),
```

