# Comparing `tmp/mysqlx-1.5.0.tar.gz` & `tmp/mysqlx-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.0.tar", last modified: Thu Jul 13 04:06:39 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.1.tar", last modified: Thu Jul 13 06:08:33 2023, max compression
```

## Comparing `mysqlx-1.5.0.tar` & `mysqlx-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx/
--rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.0/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19297 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/db.py
--rw-rw-rw-   0        0        0    13010 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     4026 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    36873 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.0/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.0/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4183 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4183 2023-07-13 04:06:39.000000 mysqlx-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3660 2023-07-11 02:06:29.000000 mysqlx-1.5.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-13 04:06:39.000000 mysqlx-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-12 13:50:31.000000 mysqlx-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:08:33.000000 mysqlx-1.5.1/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx/
+-rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.1/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19297 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13010 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     4026 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    36873 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.1/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.1/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.1/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.1/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4272 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 06:08:33.000000 mysqlx-1.5.1/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4272 2023-07-13 06:08:33.000000 mysqlx-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3747 2023-07-13 06:07:01.000000 mysqlx-1.5.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-13 06:08:33.000000 mysqlx-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-13 06:08:28.000000 mysqlx-1.5.1/setup.py
```

### Comparing `mysqlx-1.5.0/LICENSE` & `mysqlx-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/constant.py` & `mysqlx-1.5.1/mysqlx/constant.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/db.py` & `mysqlx-1.5.1/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/dbx.py` & `mysqlx-1.5.1/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/log_support.py` & `mysqlx-1.5.1/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/orm.py` & `mysqlx-1.5.1/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/snowflake.py` & `mysqlx-1.5.1/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/sql_mapper.py` & `mysqlx-1.5.1/mysqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx/support.py` & `mysqlx-1.5.1/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.0/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.1/mysqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.0
+Version: 1.5.1
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Mapper file
 '''''''''''
 
-Create a mapper file in ‘mapper’ folder, you can named
-‘user_mapper.xml’, like follow:
+Create a mapper file in 'mapper' folder, you can named
+'user_mapper.xml', like follow:
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mysqlx.dtd">
    <mapper namespace="user">
        <select id="select_all">
@@ -143,8 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 Learn more: https://gitee.com/summry/mysqlx/
 
+You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysqlx-1.5.0/PKG-INFO` & `mysqlx-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.0
+Version: 1.5.1
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Mapper file
 '''''''''''
 
-Create a mapper file in ‘mapper’ folder, you can named
-‘user_mapper.xml’, like follow:
+Create a mapper file in 'mapper' folder, you can named
+'user_mapper.xml', like follow:
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mysqlx.dtd">
    <mapper namespace="user">
        <select id="select_all">
@@ -143,8 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 Learn more: https://gitee.com/summry/mysqlx/
 
+You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysqlx-1.5.0/README.rst` & `mysqlx-1.5.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Mapper file
 '''''''''''
 
-Create a mapper file in ‘mapper’ folder, you can named
-‘user_mapper.xml’, like follow:
+Create a mapper file in 'mapper' folder, you can named
+'user_mapper.xml', like follow:
 
 .. code:: xml
 
    <?xml version="1.0" encoding="UTF-8"?>
    <!DOCTYPE mapper PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN" "https://gitee.com/summry/mysqlx/blob/master/dtd/mysqlx.dtd">
    <mapper namespace="user">
        <select id="select_all">
@@ -128,7 +128,9 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 Learn more: https://gitee.com/summry/mysqlx/
+
+You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysqlx-1.5.0/setup.py` & `mysqlx-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.0',
+    version='1.5.1',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

