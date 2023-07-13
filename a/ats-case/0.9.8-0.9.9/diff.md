# Comparing `tmp/ats_case-0.9.8.tar.gz` & `tmp/ats_case-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.8.tar", last modified: Tue Jul  4 00:54:45 2023, max compression
+gzip compressed data, was "ats_case-0.9.9.tar", last modified: Tue Jul  4 02:42:05 2023, max compression
```

## Comparing `ats_case-0.9.8.tar` & `ats_case-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.472667 ats_case-0.9.8/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.8/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-07-04 00:54:45.470339 ats_case-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.077017 ats_case-0.9.8/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.8/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.300824 ats_case-0.9.8/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.8/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    20212 2023-07-03 09:42:05.000000 ats_case-0.9.8/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11204 2023-07-01 07:55:39.000000 ats_case-0.9.8/ats_case/case/context.py
--rw-rw-rw-   0        0        0     8333 2023-06-21 09:21:03.000000 ats_case-0.9.8/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5968 2023-06-29 07:45:53.000000 ats_case-0.9.8/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.364868 ats_case-0.9.8/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.8/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.8/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.8/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.428697 ats_case-0.9.8/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.8/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.8/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.8/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.460576 ats_case-0.9.8/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.8/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.8/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-07-04 00:54:45.182486 ats_case-0.9.8/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 00:54:44.000000 ats_case-0.9.8/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 00:54:45.472667 ats_case-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-29 07:33:27.000000 ats_case-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.598356 ats_case-0.9.9/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-07-04 02:42:05.596399 ats_case-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.251349 ats_case-0.9.9/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.9/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.446828 ats_case-0.9.9/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.9/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    20220 2023-07-04 02:41:34.000000 ats_case-0.9.9/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11204 2023-07-01 07:55:39.000000 ats_case-0.9.9/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     8333 2023-06-21 09:21:03.000000 ats_case-0.9.9/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     6784 2023-07-04 02:40:16.000000 ats_case-0.9.9/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.501682 ats_case-0.9.9/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.9/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.9/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.9/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.554335 ats_case-0.9.9/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.9/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.9/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.9/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.583257 ats_case-0.9.9/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.9/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-21 00:44:19.000000 ats_case-0.9.9/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-07-04 02:42:05.343104 ats_case-0.9.9/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-07-04 02:42:04.000000 ats_case-0.9.9/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-04 02:42:04.000000 ats_case-0.9.9/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 02:42:04.000000 ats_case-0.9.9/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-04 02:42:04.000000 ats_case-0.9.9/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-04 02:42:04.000000 ats_case-0.9.9/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 02:42:05.599353 ats_case-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-07-04 02:41:34.000000 ats_case-0.9.9/setup.py
```

### Comparing `ats_case-0.9.8/PKG-INFO` & `ats_case-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.8
+Version: 0.9.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.8/README.md` & `ats_case-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/case/command.py` & `ats_case-0.9.9/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,7 +597,11 @@
             sleep(self._secs)
 
     def exec(self, context: Context):
         self.build_in(context)
         self.flush(context)
         self.set(context)
         self.sleep()
+
+
+
+
```

### Comparing `ats_case-0.9.8/ats_case/case/context.py` & `ats_case-0.9.9/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/case/executor.py` & `ats_case-0.9.9/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/case/translator.py` & `ats_case-0.9.9/ats_case/case/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 
 from pathlib import Path
 
 from ats_base.common import func
 from ats_case.case.context import Context
 from ats_case.common.enum import OperationClazz
 
@@ -79,14 +80,41 @@
         opt = OperationClazz(op.get('type').upper())
 
         code = eval('{}(self._context).translate(op)'.format(opt.name))
 
         return code + self.LINE
 
 
+def _replace_context(context: Context, data: dict):
+    sd = str(data)
+
+    re_list = re.findall(r"#(.+?)\'", sd)
+    for r in re_list:
+        v = eval(r)
+        if type(v) is str:
+            sd = sd.replace('#{}'.format(r), v)
+        else:
+            sd = sd.replace('\'#{}\''.format(r), str(v))
+
+    return eval(sd)
+
+
+def _replace_global(context: Context, data: dict):
+    sd = str(data)
+
+    re_list = re.findall(r"~(.+?)\'", sd)
+    for r in re_list:
+        index = r.find('.')
+        if index > 0:
+            key = r[index + 1:]
+            sd = sd.replace('\'~{}\''.format(r), 'context.runtime.glo.get({})'.format(key))
+
+    return eval(sd)
+
+
 class Operation(object):
     def __init__(self, context: Context):
         self._context = context
 
     def translate(self, op: dict):
         pass
 
@@ -188,20 +216,23 @@
         glo = op.get('cache')
         ctx = op.get('set')
         secs = op.get('sleep')
 
         code = "command.ats().operation('{}')".format(opt)
 
         if param is not None:
+            param = _replace_global(self._context, param)
+            param = _replace_context(self._context, param)
             code += ".parameter({})".format(param)
         if glo is not None:
             code += ".glo({})".format(glo)
         if ctx is not None:
             code += ".ctx({})".format(ctx)
         if secs is not None:
             code += ".secs({})".format(secs)
 
         code += ".exec(context)"
 
         return code
 
 
+
```

### Comparing `ats_case-0.9.8/ats_case/common/error.py` & `ats_case-0.9.9/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/manage/core.py` & `ats_case-0.9.9/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/manage/start.py` & `ats_case-0.9.9/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.9/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.9/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.8
+Version: 0.9.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.8/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.9/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.8/setup.py` & `ats_case-0.9.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.8",
+    version="0.9.9",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

