# Comparing `tmp/pypomes_db-0.1.7.tar.gz` & `tmp/pypomes_db-0.1.8.tar.gz`

## Comparing `pypomes_db-0.1.7.tar` & `pypomes_db-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    13982 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    15051 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pypomes_db-0.1.8/PKG-INFO
```

### Comparing `pypomes_db-0.1.7/src/pypomes_db/db_pomes.py` & `pypomes_db-0.1.8/src/pypomes_db/db_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1", 1)
                 cursor.execute(sel_stmt, where_vals)
 
-                # 'require_nonempty' has been defined, and the search is empty ?
+                # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
                     errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
                                   f"for {__db_build_query_msg(sel_stmt, where_vals)}")
 
-                # 'require_singleton' has been defined, and more the one tuple was returned ?
+                # has 'require_singleton' been defined, and more the one tuple was returned ?
                 elif require_singleton and cursor.rowcount > 0:
                     # yes, report the error
                     errors.append(f"Singleton expected, but {cursor.rowcount} tuples returned "
                                   f"('{DB_NAME}' at '{DB_HOST}', for '{__db_msg_clean(sel_stmt)}')")
 
                 else:
                     # obtain the first tuple returned (None if no tuple was returned)
@@ -98,44 +98,53 @@
                         result = tuple(rec)
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
-def db_select_all(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, require_nonempty: bool = False) -> list[tuple]:
+def db_select_all(errors: list[str], sel_stmt: str,  where_vals: tuple,
+                  require_nonempty: bool = False, require_count: int = None) -> list[tuple]:
     """
     Searches the database and returns all tuples that satisfy the *sel_stmt* search command.
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
+    :param require_count: defines the number of tuples expected, lest it be considered an error
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
 
-                # 'require_nonempty' has been defined, and the search is empty ?
+                # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
-                    errors.append( f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
-                                   f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
+                    errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
+                                  f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
+
+                # has 'require_count' been defined, and a different number of tuples was returned ?
+                elif isinstance(require_count, int) and require_count != cursor.rowcount:
+                    # yes, report the error
+                    errors.append(f"{cursor.rowcount} tuples returned, "
+                                  f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
+                                  f"for '{__db_build_query_msg(sel_stmt, where_vals)}'")
+
                 else:
-                    # no, obtain the returned tuples
+                    # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
                     for row in rows:
                         result.append(tuple(row))
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
@@ -201,60 +210,65 @@
             conn.autocommit = False
             # obtain the cursor and execute the operation
             cursor: Cursor = conn.cursor()
             cursor.fast_executemany = True
             try:
                 cursor.executemany(insert_stmt, insert_vals)
                 result = len(insert_vals)
-                # use either the connection or the cursor to commit
-                conn.commit()
+                cursor.commit()
             except Exception:
-                # use the connection to rollback, not the cursor
                 conn.rollback()
                 raise
             finally:
                 cursor.close()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
-def db_exec_stored_procedure(errors: list[str], proc_name: str,
-                             proc_vals: tuple, require_nonempty: bool = False) -> list[tuple]:
+def db_exec_stored_procedure(errors: list[str], proc_name: str, proc_vals: tuple,
+                             require_nonempty: bool = False, require_count: int = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param require_nonempty: defines whether an empty search should be considered an error
+    :param require_count: defines the number of tuples expected, lest it be considered an error
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     try:
         with connect(__CONNECTION_KWARGS) as conn:
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
                 cursor.execute(stmt, proc_vals)
 
-                # 'require_nonempty' has been defined, and the search is empty ?
+                # has 'require_nonempty' been defined, and the search is empty ?
                 if require_nonempty and cursor.rowcount == 0:
                     # yes, report the error
                     errors.append(f"No tuple returned in '{DB_NAME}' at '{DB_HOST}', "
                                   f"for executing stored procedure '{proc_name}', with values '{proc_vals}'")
+
+                # has 'require_count' been defined, and a different number of tuples was returned ?
+                elif isinstance(require_count, int) and require_count != cursor.rowcount:
+                    # yes, report the error
+                    errors.append(f"{cursor.rowcount} tuples returned, "
+                                  f"but {require_count} expected, in '{DB_NAME}' at '{DB_HOST}', "
+                                  f"for executing stored procedure '{proc_name}', with values '{proc_vals}'")
                 else:
-                    # no, obtain the returned tuples
+                    # obtain the returned tuples
                     rows: list[Row] = cursor.fetchall()
                     for row in rows:
-                        values: list = [item for item in row]
-                        result.append(tuple(values))
+                        result.append(tuple(row))
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple) -> int:
```

### Comparing `pypomes_db-0.1.7/LICENSE` & `pypomes_db-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.1.7/pyproject.toml` & `pypomes_db-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (DB modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.1.7/PKG-INFO` & `pypomes_db-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_db
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (DB modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

