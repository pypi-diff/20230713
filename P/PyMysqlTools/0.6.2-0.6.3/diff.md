# Comparing `tmp/PyMysqlTools-0.6.2.tar.gz` & `tmp/PyMysqlTools-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.6.2.tar", last modified: Wed Jul 12 09:26:50 2023, max compression
+gzip compressed data, was "PyMysqlTools-0.6.3.tar", last modified: Thu Jul 13 10:02:42 2023, max compression
```

## Comparing `PyMysqlTools-0.6.2.tar` & `PyMysqlTools-0.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.142478 PyMysqlTools-0.6.2/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/LICENSE
--rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2601 2023-07-12 09:26:50.141197 PyMysqlTools-0.6.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.132426 PyMysqlTools-0.6.2/PyMysqlTools/
--rw-rw-rw-   0        0        0      424 2023-07-12 09:21:06.000000 PyMysqlTools-0.6.2/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.2/PyMysqlTools/actuator.py
--rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.2/PyMysqlTools/exceptions.py
--rw-rw-rw-   0        0        0     6039 2023-07-12 06:20:01.000000 PyMysqlTools-0.6.2/PyMysqlTools/generator.py
--rw-rw-rw-   0        0        0    14473 2023-07-12 09:18:09.000000 PyMysqlTools-0.6.2/PyMysqlTools/main.py
--rw-rw-rw-   0        0        0     4185 2023-07-11 02:31:54.000000 PyMysqlTools-0.6.2/PyMysqlTools/result_set.py
--rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.2/PyMysqlTools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.139379 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2601 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1998 2023-07-12 09:26:16.000000 PyMysqlTools-0.6.2/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 09:26:50.142478 PyMysqlTools-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.972197 PyMysqlTools-0.6.3/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2601 2023-07-13 10:02:41.971223 PyMysqlTools-0.6.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.962233 PyMysqlTools-0.6.3/PyMysqlTools/
+-rw-rw-rw-   0        0        0      424 2023-07-13 10:01:02.000000 PyMysqlTools-0.6.3/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-07-13 09:00:04.000000 PyMysqlTools-0.6.3/PyMysqlTools/actuator.py
+-rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.3/PyMysqlTools/exceptions.py
+-rw-rw-rw-   0        0        0     6137 2023-07-13 08:59:01.000000 PyMysqlTools-0.6.3/PyMysqlTools/generator.py
+-rw-rw-rw-   0        0        0    14535 2023-07-13 08:54:50.000000 PyMysqlTools-0.6.3/PyMysqlTools/main.py
+-rw-rw-rw-   0        0        0     3871 2023-07-13 09:58:45.000000 PyMysqlTools-0.6.3/PyMysqlTools/result_set.py
+-rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.3/PyMysqlTools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.970201 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2601 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1998 2023-07-12 09:26:16.000000 PyMysqlTools-0.6.3/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:02:41.972197 PyMysqlTools-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/setup.py
```

### Comparing `PyMysqlTools-0.6.2/LICENSE` & `PyMysqlTools-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.2/PKG-INFO` & `PyMysqlTools-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools/actuator.py` & `PyMysqlTools-0.6.3/PyMysqlTools/actuator.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,13 +13,13 @@
         return rows
 
     def actuator_dql(self, sql: str, args=None) -> tuple:
         self._cursor.execute(sql, args)
         data = self._cursor.fetchall()
         return data
 
-    def actuator(self, type_: str):
+    def actuator(self, type_: str) -> any:
         func_dict = {
             'DML': self.actuator_dml,
             'DQL': self.actuator_dql
         }
         return func_dict[type_.upper()]
```

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools/generator.py` & `PyMysqlTools-0.6.3/PyMysqlTools/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 class SqlGenerator:
 
     def __init__(self):
         self.sql = ""
         self._clause_generator = ClauseGenerator()
 
-    def insert_one(self, tb_name, data: dict):
+    def insert_one(self, tb_name, data: dict) -> str:
         fields = self._clause_generator.get_fields(list(data.keys()))
         values = self._clause_generator.get_values(list(data.values()))
         self.sql = f"""INSERT INTO `{tb_name}` ({fields}) VALUES ({values})"""
         return self.sql.strip()
 
-    def delete_by(self, tb_name: str, condition=None):
+    def delete_by(self, tb_name: str, condition=None) -> str:
         where = self._clause_generator.build_where_clause(condition)
         self.sql = f"""DELETE FROM `{tb_name}` {where}"""
         return self.sql.strip()
 
-    def update_by(self, tb_name: str, data: dict, condition=None):
+    def update_by(self, tb_name: str, data: dict, condition=None) -> str:
         self.sql = f"""UPDATE `{tb_name}` """
         set_ = self._clause_generator.build_set_clause(data)
         self.sql += set_
         if condition:
             where = self._clause_generator.build_where_clause(condition)
             self.sql += where
         return self.sql.strip()
 
-    def find_by(self, tb_name: str, fields: list = None, condition=None):
+    def find_by(self, tb_name: str, fields: list = None, condition=None) -> str:
         if not fields:
             fields = ['*']
         fields = self._clause_generator.get_fields(fields)
         where = self._clause_generator.build_where_clause(condition)
         self.sql = f"""SELECT {fields} FROM `{tb_name}` {where}"""
         return self.sql.strip()
 
@@ -62,55 +62,55 @@
         return self.sql.strip()
 
     def show_table_primary_field(self, db_name: str, tb_name: str):
         self.sql = self.show_table_fields(db_name, tb_name)
         self.sql += " AND COLUMN_KEY = 'PRI'"
         return self.sql.strip()
 
-    def create_table(self, tb_name: str, schema):
+    def create_table(self, tb_name: str, schema) -> str:
         schema = self._clause_generator.get_schema(schema)
         self.sql = f"""
         CREATE TABLE `{tb_name}` (\n{schema}\n) DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci
         """
         return self.sql.strip()
 
-    def create_table_not_exists(self, tb_name: str, schema):
+    def create_table_not_exists(self, tb_name: str, schema) -> str:
         schema = self._clause_generator.get_schema(schema)
         self.sql = f"""
         CREATE TABLE IF NOT EXISTS `{tb_name}` (\n{schema}\n) DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci
         """
         return self.sql.strip()
 
-    def truncate_table(self, tb_name: str):
+    def truncate_table(self, tb_name: str) -> str:
         self.sql = f"""TRUNCATE TABLE `{tb_name}`"""
         return self.sql.strip()
 
-    def delete_table(self, tb_name: str):
+    def delete_table(self, tb_name: str) -> str:
         self.sql = f"""DELETE TABLE `{tb_name}`"""
         return self.sql.strip()
 
 
 class ClauseGenerator:
 
     def __init__(self):
         self.clause = ""
 
     @staticmethod
-    def get_fields(fields):
+    def get_fields(fields) -> str:
         if isinstance(fields, dict):
             fields = list(fields.values())
         return f"""{", ".join([f"`{i}`" if '*' not in i else f"{i}" for i in fields])}"""
 
     @staticmethod
-    def get_values(values):
+    def get_values(values) -> str:
         if isinstance(values, dict):
             values = list(values.values())
         return f"""{", ".join([f"%s" for _ in values])}"""
 
-    def get_schema(self, data):
+    def get_schema(self, data) -> str:
         schema = []
         if isinstance(data, list):
             for i in data:
                 if i == 'id':
                     schema.append(f""" `{i}` int NOT NULL AUTO_INCREMENT""")
                 else:
                     schema.append(f""" `{i}` varchar(255) DEFAULT NULL""")
@@ -126,15 +126,15 @@
                 schema.append(f""" `{key}` {value}""")
 
             self.clause = ',\n'.join(schema)
             return self.clause
 
         raise TypeMismatchError("'schema' 只能是 list/dict 类型")
 
-    def build_where_clause(self, condition):
+    def build_where_clause(self, condition) -> str:
         condition_str = ''
 
         if not condition:
             return condition_str
 
         if isinstance(condition, dict):
             temp = []
@@ -147,15 +147,15 @@
             condition_str = condition
         else:
             raise TypeMismatchError("'condition' 参数必须是 dict/list/str 类型")
 
         self.clause = f"""WHERE {condition_str}"""
         return self.clause
 
-    def build_set_clause(self, data: dict):
+    def build_set_clause(self, data: dict) -> str:
         temp = []
         for k, v in data.items():
             temp.append(f"""`{k}`=%s""")
 
         self.clause = f""" SET {', '.join(temp)} """
         return self.clause
 
@@ -165,12 +165,12 @@
 
     def build_group_clause(self):
         pass
 
     def build_order_clause(self):
         pass
 
-    def build_limit_clause(self, index: int, step: int = None):
+    def build_limit_clause(self, index: int, step: int = None) -> str:
         self.clause = f""" LIMIT {index}"""
         if step:
             self.clause += f""", {step}"""
         return self.clause
```

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools/main.py` & `PyMysqlTools-0.6.3/PyMysqlTools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,25 +51,27 @@
         self._clause_generator = ClauseGenerator()
         self._sql_generator = SqlGenerator()
         self._sql_actuator = SqlActuator(self._connect)
 
     def insert_one(self, tb_name, data: dict) -> int:
         """
         插入单条记录
+
         :param tb_name: 表名
         :param data: 待插入的数据
         :return: 受影响的行数
         """
         sql = self._sql_generator.insert_one(tb_name, data)
         args = list(data.values())
         return self._sql_actuator.actuator_dml(sql, args)
 
     def batch_insert(self, tb_name: str, data) -> int:
         """
         批量插入记录
+
         :param tb_name: 表名
         :param data: 待插入的数据
         :return: 受影响的行数
         """
         row_num = -1
         data_list = []
 
@@ -97,14 +99,15 @@
         if row_num == -1:
             raise TypeMismatchError("'data' 只能是 dict{str: list}/list[dict]/ResultSet 的类型格式")
         return row_num + 1
 
     def update_insert(self, tb_name: str, data: dict):
         """
         插入单条记录, 如果存在则更新, 不存在则插入
+
         :param tb_name: 表名
         :param data: 待插入/更新的数据
         :return: None
         """
         try:
             self.insert_one(tb_name, data)
         except pymysql.err.IntegrityError as err:
@@ -113,55 +116,60 @@
                 data,
                 {self.show_table_primary_field(tb_name).all()[0]: err.args[1].split("'")[1]}
             )
 
     def delete_by(self, tb_name: str, condition=None) -> int:
         """
         根据条件删除记录
+
         :param tb_name: 表名
         :param condition: 删除条件
         :return: 受影响的行数
         """
         sql = self._sql_generator.delete_by(tb_name, condition)
         return self._sql_actuator.actuator_dml(sql)
 
     def delete_by_id(self, tb_name: str, id_: int) -> int:
         """
         根据id删除记录
+
         :param tb_name: 表名
         :param id_: id
         :return: 受影响的行数
         """
         return self.delete_by(tb_name, {'id': id_})
 
     def update_by(self, tb_name: str, data: dict, condition=None) -> int:
         """
         根据条件更新记录
+
         :param tb_name: 表名
         :param data: 待更新的数据
         :param condition: 更新条件
         :return: 受影响的行数
         """
         sql = self._sql_generator.update_by(tb_name, data, condition)
         args = list(data.values())
         return self._sql_actuator.actuator_dml(sql, args)
 
     def update_by_id(self, tb_name: str, data: dict, id_: int) -> int:
         """
         根据id更新记录
+
         :param tb_name: 表名
         :param data: 待更新的数据
         :param id_: id
         :return: 受影响的行数
         """
         return self.update_by(tb_name, data, {'id': id_})
 
     def find_by(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询记录
+
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         if type_ is None:
@@ -173,27 +181,29 @@
             type_=type_,
             fields=fields or self.show_table_fields(tb_name).all()
         )
 
     def find_by_id(self, tb_name: str, id_: int, fields: list = None, type_=None) -> ResultSet:
         """
         根据id查询记录
+
         :param tb_name: 表名
         :param id_: id
         :param fields: 需要查询的字段
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         if type_ is None:
             type_ = settings.DEFAULT_RESULT_SET_TYPE
         return self.find_by(tb_name, fields, {'id': id_}, type_=type_)
 
     def find_one(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
         """
         根据条件查询单条记录
+
         :param tb_name: 表名
         :param fields: 需要查询的字段
         :param condition: 查询条件
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         if type_ is None:
@@ -206,194 +216,215 @@
             type_=type_,
             fields=fields or self.show_table_fields(tb_name).all()
         )
 
     def find_all(self, tb_name: str, type_=None) -> ResultSet:
         """
         查询全表记录
+
         :param tb_name: 表名
         :param type_: 返回集结构类型 [dict/list]
         :return: 结果集
         """
         if type_ is None:
             type_ = settings.DEFAULT_RESULT_SET_TYPE
         return self.find_by(tb_name, type_=type_)
 
     def show_table_fields(self, tb_name: str) -> ResultSet:
         """
         查看表字段
+
         :param tb_name:表名
         :return: 结果集
         """
         sql = self._sql_generator.show_table_fields(self.connect_args['database'], tb_name)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=list
         )
 
     def show_table_desc(self, tb_name: str) -> ResultSet:
         """
         查看表结构
+
         :param tb_name: 表名
         :return: 表结构
         """
         sql = self._sql_generator.desc_table(tb_name)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=list
         )
 
     def show_table_size(self, tb_name: str) -> int:
         """
         查询表有多少条记录
+
         :param tb_name: 表名
         :return: 记录数
         """
         sql = self._sql_generator.show_table_size(tb_name)
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
 
     def show_table_vague_size(self, tb_name: str) -> int:
         """
         估算表有多少条记录, 准确度低, 但速度快
+
         :param tb_name:
         :return: 记录数
         """
         sql = self._sql_generator.show_table_vague_size(tb_name)
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
 
     def show_databases(self) -> ResultSet:
         """
         查看所有数据库
+
         :return: 所有数据库
         """
         sql = self._clause_generator.build_show_clause('DATABASES')
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
 
     def show_tables(self) -> ResultSet:
         """
         查看所有数据表
+
         :return: 所有数据表
         """
         sql = self._clause_generator.build_show_clause('TABLES')
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
 
     def show_table_primary_field(self, tb_name: str) -> ResultSet:
         """
         查询主键字段名称
+
         :param tb_name: 表名
         :return: 结果集
         """
         sql = self._sql_generator.show_table_primary_field(self.connect_args['database'], tb_name)
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
 
     def is_exist_database(self, db_name: str) -> bool:
         """
         判断数据库是否存在
+
         :param db_name:
         :return: True: 存在<br>False: 不存在
         """
         return db_name in self.show_databases()
 
     def is_exist_table(self, tb_name: str) -> bool:
         """
         判断数据表是否存在
+
         :param tb_name: 表名
         :return: True: 存在<br>False: 不存在
         """
         return tb_name in self.show_tables()
 
     def truncate_table(self, tb_name: str) -> bool:
         """
         清空表数据
+
         :param tb_name: 表名
         :return: 执行结果
         """
         sql = self._sql_generator.truncate_table(tb_name)
         return self._sql_actuator.actuator_dml(sql) > 0
 
     def delete_table(self, tb_name: str) -> bool:
         """
         删除表所有记录
+
         :param tb_name: 表名
         :return: 执行结果
         """
         sql = self._sql_generator.delete_table(tb_name)
         return self._sql_actuator.actuator_dml(sql) > 0
 
     def create_table(self, tb_name: str, schema) -> int:
         """
         创建数据表
+
         :param tb_name: 表名
         :param schema: 表结构
         :return: 0表示创建成功
         """
         sql = self._sql_generator.create_table(tb_name, schema)
         return self._sql_actuator.actuator_dml(sql)
 
     def create_table_not_exists(self, tb_name: str, schema) -> int:
         """
         如果表不存在就创建数据表
+
         :param tb_name: 表名
         :param schema: 表结构
         :return: 0表示创建成功
         """
         sql = self._sql_generator.create_table(tb_name, schema)
         return self._sql_actuator.actuator_dml(sql)
 
     def migration_table(self, for_tb_name: str, to_tb_name: str) -> int:
         """
         将一张表的数据迁移到另一张表中
+
         :param for_tb_name: 数据源表的表名
         :param to_tb_name: 目标表的表名
         :return: 已迁移的数据行数
         """
         row_num = 0
         for row in self.find_all(for_tb_name):
             self.insert_one(to_tb_name, dict(zip(self.show_table_fields(to_tb_name), row)))
             row_num += 1
         return row_num
 
     def close(self):
         """
         关闭数据库连接
+
         :return:
         """
         self._connect.close()
 
     def reconnect(self):
         """
         重新与MySQL服务建立连接
+
         :return:
         """
         self._connect.ping(reconnect=True)
 
     def debugger_connect(self):
         """
         这个方法是方便作者debugger用的, 未来可能会移除
+
         :return:
         """
         return self._connect
 
     def debugger_cursor(self):
         """
         这个方法是方便作者debugger用的, 未来可能会移除
+
         :return:
         """
         return self._cursor
 
     def debugger_sql_actuator(self):
         """
         这个方法是方便作者debugger用的, 未来可能会移除
+
         :return:
         """
         return self._sql_actuator
 
     def debugger_sql_generator(self):
         """
         这个方法是方便作者debugger用的, 未来可能会移除
+
         :return:
         """
         return self._sql_generator
 
 
 class Connect(BaseConnect):
```

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools/result_set.py` & `PyMysqlTools-0.6.3/PyMysqlTools/result_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,47 +8,47 @@
             self,
             result=None,
             type_=settings.DEFAULT_RESULT_SET_TYPE,
             fields=None
     ):
         """
         ResultSet 结果集
+
         :param result: 结果集
         :param type_: 期望返回的结果集结构
         :param fields: 当type_为dict时, 需要字段名
         """
         if result is None:
             result = []
 
         self._result = []
+        self._index = 0
         self._type = type_
 
         if self._type == list:
             for row in result:
                 if len(row) > 1:
                     self._result.append(list(row))
                 elif len(row) == 1:
                     self._result.append(row[0])
                 else:
                     self._result.append([None])
         elif self._type == dict:
             if fields is None:
-                raise ParameterError("'type_'为dict时 'fields' 需要传入参数")
+                raise ParameterError("'type_' 为dict时 'fields' 需要传入参数")
             else:
                 if isinstance(fields[0], list):
                     self._fields = fields[0]
                 else:
                     self._fields = fields
                 for row in result:
                     self._result.append(_extract_as_dict(self._fields, row))
         else:
             raise TypeMismatchError("'type_' 只能是 list/dict 类型")
 
-        self._index = 0
-
     def __iter__(self):
         return self
 
     def __next__(self):
         if not isinstance(self._result, list):
             return self._result
         if self._index < len(self._result):
@@ -63,66 +63,62 @@
 
     def __len__(self):
         return len(self._result)
 
     def all(self):
         """
         获取结果集, 并将结果集转换为一个方便迭代的结构(List)
+
         :return: List结果集
         """
-        if not self._result:
-            return []
         if self._type == list and not isinstance(self._result, list):
             return [self._result]
-        if isinstance(self._result, dict):
+        if self._type == dict:
             return [self._result]
         return self._result
 
+    def get(self, index: int = 0):
+        """
+        获取特定索引位置的结果
+
+        :param index: 索引
+        :return: 索引行数据
+        """
+        if self._type == list:
+            return self._result[index]
+        if self._type == dict or len(self._result) == 1:
+            return self._result
+
     def limit(self, num: int = 1):
         """
         截取结果集的前n个结果
+
         :param num: 需要截取的结果的数量
         :return: 截取后的结果集
         """
         if not isinstance(self._result, list):
             raise ValueError('结果集结构类型不为 `list`, 不支持使用limit')
         if num > 0:
             return self._result[: num]
         else:
-            raise ValueError("'num' 参数的值必须大于 0 ！")
+            raise ParameterError("'num' 参数的值必须大于 0 ！")
 
     def next(self):
         """
         获取结果集中的下一个结果
-        :return: 下一行数据
-        """
-        if not isinstance(self._result, list):
-            return self._result
-        if self._index < len(self._result):
-            next_ = self._result[self._index]
-            self._index += 1
-            return next_
 
-    def get(self, index: int = 0):
-        """
-        获取特定索引位置的结果
-        :param index: 索引
-        :return: 索引行数据
+        :return: 下一行数据
         """
-        if not self._result:
-            return None
-        if isinstance(self._result, list):
-            return self._result[index]
-        if self._type == dict or len(self._result) == 1:
-            return self._result
+        return self.__next__()
 
 
 def _extract_as_dict(fields: list, value: list):
     """
     提取字段名和字段值组合后转换为dict结构
+
     :param fields: 字段名
     :param value: 字段值
     :return: dict结构的单行数据
     """
     fields_len = len(fields)
     value_len = len(value)
```

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools/settings.py` & `PyMysqlTools-0.6.3/PyMysqlTools/settings.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.2/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.6.3/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.2/README.md` & `PyMysqlTools-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.2/setup.py` & `PyMysqlTools-0.6.3/setup.py`

 * *Files identical despite different names*

