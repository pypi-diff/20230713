# Comparing `tmp/zcb_dbutils-0.0.6.tar.gz` & `tmp/zcb_dbutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcb_dbutils-0.0.6.tar", last modified: Wed Jul 12 10:42:18 2023, max compression
+gzip compressed data, was "zcb_dbutils-0.0.7.tar", last modified: Wed Jul 12 22:27:51 2023, max compression
```

## Comparing `zcb_dbutils-0.0.6.tar` & `zcb_dbutils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.808517 zcb_dbutils-0.0.6/
--rwxrwxrwx   0 root         (0) root         (0)     1083 2023-06-28 11:16:31.000000 zcb_dbutils-0.0.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-12 10:42:18.807002 zcb_dbutils-0.0.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      956 2023-07-12 10:39:53.000000 zcb_dbutils-0.0.6/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-12 10:42:18.809525 zcb_dbutils-0.0.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-07-12 10:36:39.000000 zcb_dbutils-0.0.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.705244 zcb_dbutils-0.0.6/test/
--rwxrwxrwx   0 root         (0) root         (0)      935 2023-07-12 10:39:00.000000 zcb_dbutils-0.0.6/test/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.728337 zcb_dbutils-0.0.6/zcb_dbutils/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.6/zcb_dbutils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6123 2023-07-12 10:36:39.000000 zcb_dbutils-0.0.6/zcb_dbutils/dbutils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.792945 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      260 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-13 00:58:44.487549 zcb_dbutils-0.0.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1083 2023-06-28 11:16:31.000000 zcb_dbutils-0.0.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-13 00:58:44.484549 zcb_dbutils-0.0.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      956 2023-07-12 10:39:53.000000 zcb_dbutils-0.0.7/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-13 00:58:44.488549 zcb_dbutils-0.0.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-07-13 00:58:43.000000 zcb_dbutils-0.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-13 00:58:44.373082 zcb_dbutils-0.0.7/test/
+-rwxrwxrwx   0 root         (0) root         (0)     1062 2023-07-13 00:58:01.000000 zcb_dbutils-0.0.7/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-13 00:58:44.400082 zcb_dbutils-0.0.7/zcb_dbutils/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.7/zcb_dbutils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7382 2023-07-13 00:57:56.000000 zcb_dbutils-0.0.7/zcb_dbutils/dbutils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-13 00:58:44.465547 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-13 00:58:44.000000 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      260 2023-07-13 00:58:44.000000 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-13 00:58:44.000000 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-13 00:58:44.000000 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-13 00:58:44.000000 zcb_dbutils-0.0.7/zcb_dbutils.egg-info/top_level.txt
```

### Comparing `zcb_dbutils-0.0.6/LICENSE` & `zcb_dbutils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zcb_dbutils-0.0.6/PKG-INFO` & `zcb_dbutils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcb_dbutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: db utils with pymysql by chzcb
 Home-page: https://github.com/chzcb/dbutils
 Author: chzcb
 Author-email: chzcb.04@163.com
 License: MIT
 Keywords: python,pymysql,zcb_dbutils
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `zcb_dbutils-0.0.6/README.md` & `zcb_dbutils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `zcb_dbutils-0.0.6/setup.py` & `zcb_dbutils-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'db utils with pymysql by chzcb'
 
 setup(
     name="zcb_dbutils",
     version=VERSION,
     author="chzcb",
     author_email="chzcb.04@163.com",
```

### Comparing `zcb_dbutils-0.0.6/test/test.py` & `zcb_dbutils-0.0.7/test/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,10 +17,16 @@
 
 ret = dbconn.show_table_index('basic', 'tb_user')
 print(pd.DataFrame.from_dict(ret))
 
 rows = dbconn.fetch_list('select user_id,id from tb_user')
 print(rows)
 
-id = dbconn.insert('insert into tb_role (org_id,role_no,role_name,role_type,remark_info,created,updated) value (1,1,%s,1,%s,0,0)',('xxx', 'xxxx'))
-dbconn.commit()
-print(id)
+# id = dbconn.insert('insert into tb_role (org_id,role_no,role_name,role_type,remark_info,created,updated) value (1,1,%s,1,%s,0,0)',('xxx', 'xxxx'))
+# dbconn.commit()
+# print(id)
+
+ret1 = []
+ret2 = []
+dbconn.batch_exec("select * from tb_user;select * from tb_role;", [])
+print(ret1)
+print(ret2)
```

### Comparing `zcb_dbutils-0.0.6/zcb_dbutils/dbutils.py` & `zcb_dbutils-0.0.7/zcb_dbutils/dbutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,22 +46,69 @@
         try:
             self.cursor.execute(sql, args)
             return self.cursor.lastrowid
         except Exception as e:
             logging.info(e, exc_info=True, stack_info=True)
             return None
 
+    def update(self, sql, args=None):
+        """
+        更新，返回影响行数
+        :param sql:
+        :param args:
+        :return:
+        """
+        try:
+            self.cursor.execute(sql, args)
+            return self.cursor.rowcount
+        except Exception as e:
+            logging.info(e, exc_info=True, stack_info=True)
+            return None
+
+    def delete(self, sql, args=None):
+        """
+        删除，返回影响行数
+        :param sql:
+        :param args:
+        :return:
+        """
+        try:
+            self.cursor.execute(sql, args)
+            return self.cursor.rowcount
+        except Exception as e:
+            logging.info(e, exc_info=True, stack_info=True)
+            return None
+
     def exec_sql(self, command):
+        """
+        执行一条语句语句
+        :param command:
+        :return:
+        """
         try:
             self.cursor.execute(command)
             return True
         except Exception as e:
             logging.info(e, exc_info=True, stack_info=True)
             return False
 
+    def batch_exec(self, command, args=[]):
+        """
+        批量执行，依赖args的数量
+        :param args:
+        :param command:
+        :return:
+        """
+        try:
+            self.cursor.executemany(command, args)
+            return True
+        except Exception as e:
+            logging.info(e, exc_info=True, stack_info=True)
+            return False
+
     def fetch_one(self, sql, args=None):
         """
         查询一行数据，如果有多个结果，也只取第一行
         :param sql:
         :param args:
         :return:
         """
```

### Comparing `zcb_dbutils-0.0.6/zcb_dbutils.egg-info/PKG-INFO` & `zcb_dbutils-0.0.7/zcb_dbutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcb-dbutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: db utils with pymysql by chzcb
 Home-page: https://github.com/chzcb/dbutils
 Author: chzcb
 Author-email: chzcb.04@163.com
 License: MIT
 Keywords: python,pymysql,zcb_dbutils
 Classifier: Development Status :: 3 - Alpha
```

