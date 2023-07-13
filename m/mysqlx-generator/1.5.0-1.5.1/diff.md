# Comparing `tmp/mysqlx-generator-1.5.0.tar.gz` & `tmp/mysqlx-generator-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.5.0.tar", last modified: Thu Jul 13 05:58:51 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.5.1.tar", last modified: Thu Jul 13 06:10:12 2023, max compression
```

## Comparing `mysqlx-generator-1.5.0.tar` & `mysqlx-generator-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.5.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator/
--rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.0/mysqlx_generator/generator.tpl
--rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.0/mysqlx_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2796 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      325 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2796 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2302 2023-07-13 05:58:31.000000 mysqlx-generator-1.5.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-07-13 05:56:03.000000 mysqlx-generator-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-generator-1.5.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator/
+-rw-rw-rw-   0        0        0     1653 2023-07-11 02:11:20.000000 mysqlx-generator-1.5.1/mysqlx_generator/generator.tpl
+-rw-rw-rw-   0        0        0     5830 2023-07-11 01:46:17.000000 mysqlx-generator-1.5.1/mysqlx_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 05:58:51.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2848 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      325 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2848 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2354 2023-07-13 06:07:01.000000 mysqlx-generator-1.5.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-13 06:10:12.000000 mysqlx-generator-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-07-13 06:10:05.000000 mysqlx-generator-1.5.1/setup.py
```

### Comparing `mysqlx-generator-1.5.0/LICENSE` & `mysqlx-generator-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.0/mysqlx_generator/generator.tpl` & `mysqlx-generator-1.5.1/mysqlx_generator/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.0/mysqlx_generator/__init__.py` & `mysqlx-generator-1.5.1/mysqlx_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.5.0/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.5.1/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.0
+Version: 1.5.1
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
@@ -25,19 +25,19 @@
 .. code:: python
 
    from mysqlx_generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
-       # you can generate one table
+       # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
-       # you can generate many tables
+       # you can generate model classes for tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. default current schema if not given
+       # you can generate model classes for all tables from a given schema. default current schema if not given
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.5.0/PKG-INFO` & `mysqlx-generator-1.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.5.0
+Version: 1.5.1
 Summary: mysqlx-generator is a model code generator from db tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Install
 '''''''
 
 .. code:: shell
@@ -25,19 +25,19 @@
 .. code:: python
 
    from mysqlx_generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
-       # you can generate one table
+       # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
-       # you can generate many tables
+       # you can generate model classes for tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. default current schema if not given
+       # you can generate model classes for all tables from a given schema. default current schema if not given
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.5.0/README.rst` & `mysqlx-generator-1.5.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 .. code:: python
 
    from mysqlx_generator import Generator
 
 
    if __name__ == '__main__':
        coder = Generator(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test')
-       # you can generate one table
+       # you can generate a model class for one table
        coder.generate_with_tables(tables='user', path='models.py')
-       # you can generate many tables
+       # you can generate model classes for tables
        coder.generate_with_tables(tables=['user', 'person'], path='models.py')
-       # you can generate all tables for given schema. default current schema if not given
+       # you can generate model classes for all tables from a given schema. default current schema if not given
        coder.generate_with_schema(schema='test', path='models.py')
 
 If you run last code, then generate a file 'models.py' in current
 directory like follow:
 
 .. code:: python
```

### Comparing `mysqlx-generator-1.5.0/setup.py` & `mysqlx-generator-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     packages=['mysqlx_generator'],
     description="mysqlx-generator is a model code generator from db tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'mysqlx>=1.3.9',
     ],
-    version='1.5.0',
+    version='1.5.1',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
-    python_requires='>=3.7',
+    python_requires='>=3.5',
     zip_safe=False
 )
```

