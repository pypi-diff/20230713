# Comparing `tmp/pypomes_db-0.1.6.tar.gz` & `tmp/pypomes_db-0.1.7.tar.gz`

## Comparing `pypomes_db-0.1.6.tar` & `pypomes_db-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    13982 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/PKG-INFO
```

### Comparing `pypomes_db-0.1.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.7/src/pypomes_db/db_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # noinspection PyProtectedMember
 from pyodbc import connect, Connection, Cursor, Row
 from typing import Final
 from pypomes_core import APP_PREFIX, env_get_int, env_get_str
 
-# dados para acesso ao BD
 DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
 DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
 DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
 DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
 DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
 DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER")
 
@@ -51,90 +50,98 @@
         sel_stmt += " WHERE " + "".join(f"{attr} = ? AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors, sel_stmt, where_vals)
     result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
-def db_select_one(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, required: bool = False) -> tuple:
+def db_select_one(errors: list[str], sel_stmt: str, where_vals: tuple,
+                  require_nonempty: bool = False, require_singleton: bool = False) -> tuple:
     """
     Searches the database and returns the first tuple that satisfies the *sel_stmt* search command.
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
-    :param required: defines whether an empty search should be considered an error
+    :param require_nonempty: defines whether an empty search should be considered an error
+    :param require_singleton: defines whether a non-singleton search should be considered an error
     :return: tuple containing the search result, or None if there was an error, or if the search was empty
     """
-    # inicialize the return variable
+    # initialize the return variable
     result: tuple | None = None
 
-    exc: bool = False
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1", 1)
                 cursor.execute(sel_stmt, where_vals)
-                # obtain the first tuple returned (None se no tuple was returned)
-                rec: Row = cursor.fetchone()
-                if rec is not None:
-                    result = tuple(rec)
+
+                # 'require_nonempty' has been defined, and the search is empty ?
+                if require_nonempty and cursor.rowcount == 0:
+                    # yes, report the error
+                    errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
+                                  f"for {__db_build_query_msg(sel_stmt, where_vals)}")
+
+                # 'require_singleton' has been defined, and more the one tuple was returned ?
+                elif require_singleton and cursor.rowcount > 0:
+                    # yes, report the error
+                    errors.append(f"Singleton expected, but {cursor.rowcount} tuples returned "
+                                  f"('{DB_NAME}' at '{DB_HOST}', for '{__db_msg_clean(sel_stmt)}')")
+
+                else:
+                    # obtain the first tuple returned (None if no tuple was returned)
+                    rec: Row = cursor.fetchone()
+                    if rec is not None:
+                        result = tuple(rec)
     except Exception as e:
-        exc = True
         errors.append(__db_except_msg(e))
 
-    # o parâmetro 'required' foi definido e nenhum registro foi obtido?
-    if required and not exc and result is None:
-        # sim, reporte o erro
-        errors.append(__db_required_msg(sel_stmt, where_vals))
-
     return result
 
 
 def db_select_all(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, required: bool = False) -> list[tuple]:
+                  where_vals: tuple, require_nonempty: bool = False) -> list[tuple]:
     """
     Searches the database and returns all tuples that satisfy the *sel_stmt* search command.
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
-    :param required: defines whether an empty search should be considered an error
+    :param require_nonempty: defines whether an empty search should be considered an error
     :return: list of tuples containing the search result, or [] if the search is empty
     """
-    # inicialize the return variable
+    # initialize the return variable
     result: list[tuple] = []
 
-    exc: bool = False
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
-                # obtain the returned tuples
-                rows: list[Row] = cursor.fetchall()
-                for row in rows:
-                    result.append(tuple(row))
+
+                # 'require_nonempty' has been defined, and the search is empty ?
+                if require_nonempty and cursor.rowcount == 0:
+                    # yes, report the error
+                    errors.append( f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
+                                   f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
+                else:
+                    # no, obtain the returned tuples
+                    rows: list[Row] = cursor.fetchall()
+                    for row in rows:
+                        result.append(tuple(row))
     except Exception as e:
-        exc = True
         errors.append(__db_except_msg(e))
 
-    # no errors, the 'required' parameter has been defined, and the search is empty ?
-    if required and not exc and len(result) == 0:
-        # yes, report the error
-        errors.append(__db_required_msg(sel_stmt, where_vals))
-
     return result
 
 
 def db_insert(errors: list[str], insert_stmt: str, insert_vals: tuple) -> int:
     """
     Inserts a tuple, with values defined in *insert_vals*, into the database.
 
@@ -181,60 +188,73 @@
     Inserts the tuples, with values defined in *insert_vals*, into the database.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :return: the number of inserted tuples, or None if an error occurred
     """
-    # inicialize the return variable
+    # initialize the return variable
     result: int | None = None
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             cursor: Cursor = conn.cursor()
             cursor.fast_executemany = True
             try:
                 cursor.executemany(insert_stmt, insert_vals)
                 result = len(insert_vals)
+                # use either the connection or the cursor to commit
                 conn.commit()
             except Exception:
+                # use the connection to rollback, not the cursor
                 conn.rollback()
                 raise
+            finally:
+                cursor.close()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
-def db_exec_stored_procedure(errors: list[str], proc_name: str, proc_vals: tuple) -> list[tuple]:
+def db_exec_stored_procedure(errors: list[str], proc_name: str,
+                             proc_vals: tuple, require_nonempty: bool = False) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
+    :param require_nonempty: defines whether an empty search should be considered an error
     :return: list of tuples containing the search result, or [] if the search is empty
     """
-    # inicialize the return variable
+    # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
                 cursor.execute(stmt, proc_vals)
-                # obtain the tuples returned
-                rows: list[Row] = cursor.fetchall()
-                for row in rows:
-                    values: list = [item for item in row]
-                    result.append(tuple(values))
+
+                # 'require_nonempty' has been defined, and the search is empty ?
+                if require_nonempty and cursor.rowcount == 0:
+                    # yes, report the error
+                    errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
+                                  f"for executing stored procedure '{proc_name}', with values '{proc_vals}'")
+                else:
+                    # no, obtain the returned tuples
+                    rows: list[Row] = cursor.fetchall()
+                    for row in rows:
+                        values: list = [item for item in row]
+                        result.append(tuple(values))
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple) -> int:
@@ -244,15 +264,15 @@
     values for selecting tuples are in *bind_vals*.
 
     :param errors: incidental error messages
     :param modify_stmt: INSERT, UPDATE, or DELETE command
     :param bind_vals: values for database modification, and for tuples selection
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
-    # inicialize the return variable
+    # initialize the return variable
     result: int | None = None
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(modify_stmt, bind_vals)
@@ -260,47 +280,52 @@
                 conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
+def __db_msg_clean(msg: str) -> str:
+    """
+    Clean the given *msg* string, by replacing double quotes with single quotes,
+    and newlines and tabs with whitespace, and by removing backslashes.
+
+    :param msg: the string to be cleaned
+    :return: the cleaned string
+    """
+    return msg.replace('"', "'") \
+              .replace("\n", " ") \
+              .replace("\t", " ") \
+              .replace("\\", "")
+
+
 def __db_except_msg(exception: Exception) -> str:
     """
     Formats and returns the error message corresponding to the exception raised
     while accessing the database.
 
     :param exception: the exception raised
     :return:the formatted error message
     """
-    exc_msg: str = f"{exception}"
-    exc_msg = exc_msg.replace('"', "'") \
-                     .replace('\n', " ") \
-                     .replace('\t', " ") \
-                     .replace("\\", "")
-    result = f"Error accessing {DB_NAME} at {DB_HOST}: {exc_msg}"
+    result = f"Error accessing {DB_NAME} at {DB_HOST}: {__db_msg_clean(f'{exception}')}"
 
     return result
 
 
-def __db_required_msg(sel_stmt: str, where_vals: tuple) -> str:
+def __db_build_query_msg(sel_stmt: str, where_vals: tuple) -> str:
     """
     Formats and returns the message indicative of an empty search.
 
     :param sel_stmt: the search command
     :param where_vals: values associated with the search criteria
     :return: message indicative of empty search
     """
-    stmt: str = sel_stmt.replace('"', "'") \
-                        .replace('\n', " ") \
-                        .replace('\t', " ") \
-                        .replace("\\", "")
-    result: str = f"No record found in {DB_NAME} at {DB_HOST}, for {stmt}"
+    result: str = __db_msg_clean(sel_stmt)
 
     for val in where_vals:
         if isinstance(val, str):
             val = f"'{val}'"
         else:
             val = str(val)
-        result = result.replace("%s", val, 1)
+        result = result.replace("?", val, 1)
 
     return result
```

### Comparing `pypomes_db-0.1.6/LICENSE` & `pypomes_db-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.6/pyproject.toml` & `pypomes_db-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.6/PKG-INFO` & `pypomes_db-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

