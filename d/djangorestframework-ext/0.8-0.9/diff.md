# Comparing `tmp/djangorestframework-ext-0.8.tar.gz` & `tmp/djangorestframework-ext-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-ext-0.8.tar", last modified: Mon Jun 28 06:36:39 2021, max compression
+gzip compressed data, was "djangorestframework-ext-0.9.tar", last modified: Wed Jul 14 08:14:20 2021, max compression
```

## Comparing `djangorestframework-ext-0.8.tar` & `djangorestframework-ext-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-06-28 06:36:39.130824 djangorestframework-ext-0.8/
--rw-rw-rw-   0        0        0     1064 2021-01-08 05:37:04.000000 djangorestframework-ext-0.8/LICENSE
--rw-rw-rw-   0        0        0     4549 2021-06-28 06:36:39.129825 djangorestframework-ext-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3293 2021-06-16 06:50:44.000000 djangorestframework-ext-0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-06-28 06:36:39.116860 djangorestframework-ext-0.8/djangorestframework_ext/
--rw-rw-rw-   0        0        0       94 2021-06-28 06:36:27.000000 djangorestframework-ext-0.8/djangorestframework_ext/__init__.py
--rw-rw-rw-   0        0        0      391 2020-11-18 03:22:36.000000 djangorestframework-ext-0.8/djangorestframework_ext/pagination.py
--rw-rw-rw-   0        0        0      502 2021-01-04 07:14:02.000000 djangorestframework-ext-0.8/djangorestframework_ext/permissions.py
--rw-rw-rw-   0        0        0     1921 2021-06-28 06:32:11.000000 djangorestframework-ext-0.8/djangorestframework_ext/serializers.py
--rw-rw-rw-   0        0        0      241 2021-01-04 07:12:00.000000 djangorestframework-ext-0.8/djangorestframework_ext/settings.py
--rw-rw-rw-   0        0        0      617 2021-06-23 02:21:17.000000 djangorestframework-ext-0.8/djangorestframework_ext/views.py
-drwxrwxrwx   0        0        0        0 2021-06-28 06:36:39.128828 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/
--rw-rw-rw-   0        0        0     4549 2021-06-28 06:36:39.000000 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2021-06-28 06:36:39.000000 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-28 06:36:39.000000 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2021-06-28 06:36:39.000000 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2021-06-28 06:36:39.000000 djangorestframework-ext-0.8/djangorestframework_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-28 06:36:39.130824 djangorestframework-ext-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1351 2021-06-28 06:36:27.000000 djangorestframework-ext-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-14 08:14:20.112099 djangorestframework-ext-0.9/
+-rw-rw-rw-   0        0        0     1064 2021-01-08 05:37:04.000000 djangorestframework-ext-0.9/LICENSE
+-rw-rw-rw-   0        0        0     4549 2021-07-14 08:14:20.112099 djangorestframework-ext-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3293 2021-06-16 06:50:44.000000 djangorestframework-ext-0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-07-14 08:14:20.095168 djangorestframework-ext-0.9/djangorestframework_ext/
+-rw-rw-rw-   0        0        0       94 2021-07-14 08:11:10.000000 djangorestframework-ext-0.9/djangorestframework_ext/__init__.py
+-rw-rw-rw-   0        0        0      391 2020-11-18 03:22:36.000000 djangorestframework-ext-0.9/djangorestframework_ext/pagination.py
+-rw-rw-rw-   0        0        0      502 2021-01-04 07:14:02.000000 djangorestframework-ext-0.9/djangorestframework_ext/permissions.py
+-rw-rw-rw-   0        0        0     1926 2021-07-14 08:11:10.000000 djangorestframework-ext-0.9/djangorestframework_ext/serializers.py
+-rw-rw-rw-   0        0        0      241 2021-01-04 07:12:00.000000 djangorestframework-ext-0.9/djangorestframework_ext/settings.py
+-rw-rw-rw-   0        0        0      617 2021-06-23 02:21:17.000000 djangorestframework-ext-0.9/djangorestframework_ext/views.py
+drwxrwxrwx   0        0        0        0 2021-07-14 08:14:20.110103 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/
+-rw-rw-rw-   0        0        0     4549 2021-07-14 08:14:19.000000 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2021-07-14 08:14:20.000000 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-14 08:14:19.000000 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2021-07-14 08:14:19.000000 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2021-07-14 08:14:19.000000 djangorestframework-ext-0.9/djangorestframework_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-14 08:14:20.112099 djangorestframework-ext-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2021-07-14 08:11:10.000000 djangorestframework-ext-0.9/setup.py
```

### Comparing `djangorestframework-ext-0.8/LICENSE` & `djangorestframework-ext-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-ext-0.8/PKG-INFO` & `djangorestframework-ext-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-ext
-Version: 0.8
+Version: 0.9
 Summary: Extensions of Django Rest framework
 Home-page: https://github.com/zengqiu/django-rest-framework-ext
 Author: zengqiu
 Author-email: zengqiu@qq.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangorestframework-ext-0.8/README.md` & `djangorestframework-ext-0.9/README.md`

 * *Files identical despite different names*

### Comparing `djangorestframework-ext-0.8/djangorestframework_ext/serializers.py` & `djangorestframework-ext-0.9/djangorestframework_ext/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         result = dict()
         for k, v in data.items():
             field = self.get_fields()[k]
             if isinstance(field, serializers.DateTimeField) and v:
                 value = dateformat.format(parse_datetime(v), 'Y-m-d H:i:s')
             else:
                 value = v
-            result[getattr(field, 'label') or k] = value
+            result[str(getattr(field, 'label') or k)] = value
         return result
 
 
 # https://www.django-rest-framework.org/api-guide/serializers/#dynamically-modifying-fields
 class DynamicFieldsModelSerializer(serializers.ModelSerializer):
     """
     A ModelSerializer that takes an additional `fields` argument that
```

### Comparing `djangorestframework-ext-0.8/djangorestframework_ext/views.py` & `djangorestframework-ext-0.9/djangorestframework_ext/views.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-ext-0.8/djangorestframework_ext.egg-info/PKG-INFO` & `djangorestframework-ext-0.9/djangorestframework_ext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-ext
-Version: 0.8
+Version: 0.9
 Summary: Extensions of Django Rest framework
 Home-page: https://github.com/zengqiu/django-rest-framework-ext
 Author: zengqiu
 Author-email: zengqiu@qq.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangorestframework-ext-0.8/setup.py` & `djangorestframework-ext-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
     name='djangorestframework-ext',
-    version='0.8',
+    version='0.9',
     url='https://github.com/zengqiu/django-rest-framework-ext',
     license='MIT',
     author='zengqiu',
     author_email='zengqiu@qq.com',
     description='Extensions of Django Rest framework',
     long_description=readme,
     long_description_content_type='text/markdown',
```

