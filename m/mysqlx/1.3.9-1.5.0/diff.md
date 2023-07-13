# Comparing `tmp/mysqlx-1.3.9.tar.gz` & `tmp/mysqlx-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.3.9.tar", last modified: Tue Jul 11 23:57:23 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.0.tar", last modified: Thu Jul 13 04:06:39 2023, max compression
```

## Comparing `mysqlx-1.3.9.tar` & `mysqlx-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 23:57:23.000000 mysqlx-1.3.9/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.3.9/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx/
--rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.3.9/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19126 2023-07-11 03:25:48.000000 mysqlx-1.3.9/mysqlx/db.py
--rw-rw-rw-   0        0        0    12866 2023-07-10 17:10:18.000000 mysqlx-1.3.9/mysqlx/dbx.py
--rw-rw-rw-   0        0        0    36893 2023-07-11 13:16:22.000000 mysqlx-1.3.9/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.3.9/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4052 2023-07-10 13:42:49.000000 mysqlx-1.3.9/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0    10641 2023-07-11 13:43:05.000000 mysqlx-1.3.9/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.3.9/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4183 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      343 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 23:57:23.000000 mysqlx-1.3.9/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4183 2023-07-11 23:57:23.000000 mysqlx-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3660 2023-07-11 02:06:29.000000 mysqlx-1.3.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 23:57:23.000000 mysqlx-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-11 23:54:58.000000 mysqlx-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx/
+-rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.0/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19297 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13010 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     4026 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    36873 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.0/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.0/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4183 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 04:06:39.000000 mysqlx-1.5.0/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4183 2023-07-13 04:06:39.000000 mysqlx-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3660 2023-07-11 02:06:29.000000 mysqlx-1.5.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-13 04:06:39.000000 mysqlx-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-12 13:50:31.000000 mysqlx-1.5.0/setup.py
```

### Comparing `mysqlx-1.3.9/LICENSE` & `mysqlx-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.9/mysqlx/constant.py` & `mysqlx-1.5.0/mysqlx/constant.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.9/mysqlx/db.py` & `mysqlx-1.5.0/mysqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import functools
 from typing import Sequence
 from .constant import LIMIT_1, MAPPER_PATH, PK_SQL
+from .log_support import logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
-    DB_LOCK, get_batch_args, logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
+    DB_LOCK, get_batch_args
 
 _DB_CTX = None
 _SHOW_SQL = False
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=5, use_unicode=True, show_sql=False, **kwargs):
+    global _DB_CTX
+    global _SHOW_SQL
     use_mysql_connector = False
     try:
         from mysql.connector import connect
         use_mysql_connector = True
     except ImportError:
-        from pymysql import connect
-
-    global _DB_CTX
-    global _SHOW_SQL
+        try:
+            from pymysql import connect
+        except ImportError:
+            raise DBError("Please install mysql-connector-python or PyMySQL, and mysql-connector-python >= 8.0.13, PyMySQL >= 0.9.0.")
 
     if 'debug' in kwargs:
         if kwargs['debug']:
             from logging import DEBUG
             logger.setLevel(DEBUG)
         del kwargs['debug']
 
@@ -332,25 +335,25 @@
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_get', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_get_with_limit(sql, *args)
+    return do_get_limit(sql, *args)
 
 
-def do_get_with_limit(sql: str, *args):
+def do_get_limit(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_get_with_limit', sql, *args)
-    result = do_select_one_with_limit(sql, *args)
+    result = do_select_one_limit(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'mysqlx.db.%s' expect only one column but %d." % ('do_get_with_limit', len(result))
         logger.error('%s  \n\t\t sql: %s \n\t\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
@@ -383,19 +386,19 @@
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_query_one', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_query_one_with_limit(sql, *args)
+    return do_query_one_limit(sql, *args)
 
 
 @with_connection
-def do_query_one_with_limit(sql: str, *args):
+def do_query_one_limit(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_query_one_with_limit', sql.strip(), *args)
@@ -433,19 +436,19 @@
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
     sql, args = _limit_one_sql_args(sql, *args)
-    return do_select_one_with_limit(sql, *args)
+    return do_select_one_limit(sql, *args)
 
 
 @with_connection
-def do_select_one_with_limit(sql: str, *args):
+def do_select_one_limit(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
     sql = _before_execute('do_select_one_with_limit', sql.strip(), *args)
```

### Comparing `mysqlx-1.3.9/mysqlx/dbx.py` & `mysqlx-1.5.0/mysqlx/dbx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 from typing import Mapping
 from jinja2 import Template
-from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction, logger, sql_id_log, page_sql_id_log
+from .log_support import logger, sql_id_log, page_sql_id_log
+from .support import get_named_sql_args, SqlModel, MapperError, is_dynamic_sql, get_batch_args, SqlAction
 from .db import do_get, do_query, do_query_one, do_execute, do_select_page, do_select, do_select_one, do_query_page, init_db as _init_db, \
     get_connection as _get_connection, insert as _insert, save as _save, batch_insert as _batch_insert, batch_execute as _batch_execute
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
@@ -174,14 +175,16 @@
     :param batch: bool, is batch or not
     :param param_names: original function parameter names
     :param args:
     :param kwargs:
     :return:
     """
     if sql_model.dynamic:
+        if not kwargs:
+            raise MapperError("Parameter 'kwargs' must not be empty when named mapping sql.")
         sql = sql_model.sql.render(**kwargs)
         logger.debug("Original sql: {}".format(sql))
         return get_named_sql_args(sql, **kwargs)
     else:
         logger.debug("Original sql: {}".format(sql_model.sql))
         if sql_model.mapping and kwargs:
             return get_named_sql_args(sql_model.sql, **kwargs)
```

### Comparing `mysqlx-1.3.9/mysqlx/orm.py` & `mysqlx-1.5.0/mysqlx/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
+from .support import DBError, simple_sql
 from typing import Sequence, Union, List, Tuple
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
     COLUMN_SQL
-from .db import do_get_with_limit, do_query, do_query_one_with_limit, do_execute, insert, save, do_select, do_select_one_with_limit, transaction, \
-    batch_insert, do_query_page, do_select_page, do_get
-from .support import DBError, simple_sql, logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, \
-    orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_id_log, orm_find_by_ids_log
+from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
+    do_query_page, do_select_page, do_get
+from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
+    orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
@@ -359,15 +360,15 @@
         count = User.count(name='张三', age=55)
         """
         orm_count_log('count', cls.__name__, **kwargs)
         table = cls._get_table()
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
         sql = _select_sql(table, where, LIMIT_1, fields)
-        return do_get_with_limit(sql, *args, LIMIT_1)
+        return do_get_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = User.count_by('where name=?', '李四')
         """
@@ -488,15 +489,15 @@
         users = User.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('query_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_query_one_with_limit(sql, *args, LIMIT_1)
+        return do_query_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.query_by('where name=?', '李四')
         """
@@ -539,15 +540,15 @@
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_query_one_with_limit(sql, _id, LIMIT_1)
+        return do_query_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         users = User.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
@@ -587,15 +588,15 @@
         row = User.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('select_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
         table = cls._get_table()
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_select_one_with_limit(sql, *args, LIMIT_1)
+        return do_select_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by('where name=?', '李四')
         """
@@ -638,15 +639,15 @@
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}`=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
-        return do_select_one_with_limit(sql, _id, LIMIT_1)
+        return do_select_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = User.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
@@ -808,15 +809,15 @@
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
 
 
 @lru_cache(maxsize=128)
 def _get_table_columns(table: str):
-    return do_get_with_limit(COLUMN_SQL, table, LIMIT_1)
+    return do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _delete_by_id_sql(table, pk):
     return 'DELETE FROM `{}` WHERE `{}`=? limit ?'.format(table, pk)
 
 
 def _get_condition_arg(k: str, v: object):
```

### Comparing `mysqlx-1.3.9/mysqlx/snowflake.py` & `mysqlx-1.5.0/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.9/mysqlx/sql_mapper.py` & `mysqlx-1.5.0/mysqlx/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import functools
+from .log_support import logger
 from .dbx import get_sql_model, do_get_sql, build_sql_id
-from .support import SqlAction, get_named_sql_args, simple_sql, logger, MapperError
+from .support import SqlAction, get_named_sql_args, simple_sql, MapperError
 from .db import do_get, do_query, do_query_one, do_execute, do_batch_execute, do_select, do_select_one, batch_execute, do_save
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_pk=False):
     def _decorator(func):
```

### Comparing `mysqlx-1.3.9/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.0/mysqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.9
+Version: 1.5.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.3.9/PKG-INFO` & `mysqlx-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.3.9
+Version: 1.5.0
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.3.9/README.rst` & `mysqlx-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.3.9/setup.py` & `mysqlx-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'mysql-connector-python>=8.0.20',
+        # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.3.9',
+    version='1.5.0',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

