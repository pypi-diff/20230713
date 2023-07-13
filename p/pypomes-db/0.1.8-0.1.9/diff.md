# Comparing `tmp/pypomes_db-0.1.8.tar.gz` & `tmp/pypomes_db-0.1.9.tar.gz`

## Comparing `pypomes_db-0.1.8.tar` & `pypomes_db-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    15349 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.9/PKG-INFO
```

### Comparing `pypomes_db-0.1.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.9/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,36 +70,39 @@
     :return: tuple containing the search result, or None if there was an error, or if the search was empty
     """
     # initialize the return variable
     result: tuple | None = None
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1", 1)
                 cursor.execute(sel_stmt, where_vals)
 
                 # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
                     errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
-                                  f"for {__db_build_query_msg(sel_stmt, where_vals)}")
+                                  f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
 
                 # has 'require_singleton' been defined, and more the one tuple was returned ?
                 elif require_singleton and cursor.rowcount > 0:
                     # yes, report the error
                     errors.append(f"Singleton expected, but {cursor.rowcount} tuples returned "
                                   f"('{DB_NAME}' at '{DB_HOST}', for '{__db_msg_clean(sel_stmt)}')")
 
                 else:
                     # obtain the first tuple returned (None if no tuple was returned)
                     rec: Row = cursor.fetchone()
                     if rec is not None:
                         result = tuple(rec)
+            conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_select_all(errors: list[str], sel_stmt: str,  where_vals: tuple,
@@ -110,22 +113,24 @@
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
-    :param require_count: defines the number of tuples expected, lest it be considered an error
+    :param require_count: optionally defines the number of tuples required to be returned
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
 
                 # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
@@ -140,14 +145,15 @@
                                   f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
 
                 else:
                     # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
                     for row in rows:
                         result.append(tuple(row))
+            conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_insert(errors: list[str], insert_stmt: str, insert_vals: tuple) -> int:
@@ -209,21 +215,20 @@
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             cursor: Cursor = conn.cursor()
             cursor.fast_executemany = True
             try:
                 cursor.executemany(insert_stmt, insert_vals)
+                cursor.close()
                 result = len(insert_vals)
-                cursor.commit()
             except Exception:
                 conn.rollback()
                 raise
-            finally:
-                cursor.close()
+            conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_exec_stored_procedure(errors: list[str], proc_name: str, proc_vals: tuple,
@@ -231,15 +236,15 @@
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param require_nonempty: defines whether an empty search should be considered an error
-    :param require_count: defines the number of tuples expected, lest it be considered an error
+    :param require_count: optionally defines the number of tuples required to be returned
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
@@ -283,19 +288,21 @@
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(modify_stmt, bind_vals)
                 result = cursor.rowcount
-                conn.commit()
+            conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def __db_msg_clean(msg: str) -> str:
@@ -316,17 +323,15 @@
     """
     Formats and returns the error message corresponding to the exception raised
     while accessing the database.
 
     :param exception: the exception raised
     :return:the formatted error message
     """
-    result = f"Error accessing {DB_NAME} at {DB_HOST}: {__db_msg_clean(f'{exception}')}"
-
-    return result
+    return f"Error accessing {DB_NAME} at {DB_HOST}: {__db_msg_clean(f'{exception}')}"
 
 
 def __db_build_query_msg(sel_stmt: str, where_vals: tuple) -> str:
     """
     Formats and returns the message indicative of an empty search.
 
     :param sel_stmt: the search command
```

### Comparing `pypomes_db-0.1.8/LICENSE` & `pypomes_db-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.8/pyproject.toml` & `pypomes_db-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.8/PKG-INFO` & `pypomes_db-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

