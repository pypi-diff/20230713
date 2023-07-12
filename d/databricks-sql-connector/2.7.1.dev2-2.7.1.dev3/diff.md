# Comparing `tmp/databricks_sql_connector-2.7.1.dev2.tar.gz` & `tmp/databricks_sql_connector-2.7.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.7.1.dev2.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.7.1.dev3.tar", max compression
```

## Comparing `databricks_sql_connector-2.7.1.dev2.tar` & `databricks_sql_connector-2.7.1.dev3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     5070 2023-07-12 01:05:48.311672 databricks_sql_connector-2.7.1.dev2/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev2/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev2/README.md
--rw-r--r--   0        0        0     1593 2023-07-12 13:58:42.950327 databricks_sql_connector-2.7.1.dev2/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev2/src/databricks/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-12 13:58:37.675891 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4421 2023-07-11 02:39:13.117511 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6192 2023-07-11 02:39:13.117899 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     3790 2023-07-11 02:39:13.118139 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9989 2023-07-12 01:04:46.051969 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     6036 2023-07-12 01:04:46.052362 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    37992 2023-07-12 00:32:42.468464 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/client.py
--rw-r--r--   0        0        0     6547 2023-07-12 00:32:42.468765 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/download_manager.py
--rw-r--r--   0        0        0     6374 2023-07-12 00:32:42.469030 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/downloader.py
--rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2023-07-11 02:39:13.120777 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    40111 2023-07-12 00:32:42.469577 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/types.py
--rw-r--r--   0        0        0    17993 2023-07-12 00:32:42.470095 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10687 2023-07-12 01:04:46.082556 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0     5497 2023-07-12 21:59:42.567864 databricks_sql_connector-2.7.1.dev3/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev3/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev3/README.md
+-rw-r--r--   0        0        0     1697 2023-07-12 22:02:32.029669 databricks_sql_connector-2.7.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev3/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-12 22:02:40.220905 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-07-12 21:51:15.071834 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-07-12 21:51:15.072262 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-07-12 21:51:15.072498 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9989 2023-07-12 21:51:15.072984 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     6036 2023-07-12 21:51:15.073407 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    37996 2023-07-12 21:51:15.074009 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     6547 2023-07-12 21:51:15.074368 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/download_manager.py
+-rw-r--r--   0        0        0     6374 2023-07-12 21:51:15.074646 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/downloader.py
+-rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-12 21:51:15.075093 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41011 2023-07-12 21:51:15.075657 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/types.py
+-rw-r--r--   0        0        0    17993 2023-07-12 21:51:15.076152 databricks_sql_connector-2.7.1.dev3/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10729 2023-07-12 21:59:42.568504 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev3/PKG-INFO
```

### Comparing `databricks_sql_connector-2.7.1.dev2/CHANGELOG.md` & `databricks_sql_connector-2.7.1.dev3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Release History
 
 ## 2.7.x (Unreleased)
 
-- Add support for Cloud Fetch
-- SQLAlchemy has_table function now honours schema= argument and adds catalog= argument
-- Fix: Revised SQLAlchemy dialect and examples for compatibility with SQLAlchemy==1.3.x
-- Fix: oauth would fail if expired credentials appeared in ~/.netrc
-- Fix: Python HTTP proxies were broken after switch to urllib3
+- Add support for Cloud Fetch (#146, #151, #154)
+- SQLAlchemy has_table function now honours schema= argument and adds catalog= argument (#174)
+- SQLAlchemy set non_native_boolean_check_constraint False as it's not supported by Databricks (#120)
+- Fix: Revised SQLAlchemy dialect and examples for compatibility with SQLAlchemy==1.3.x (#173)
+- Fix: oauth would fail if expired credentials appeared in ~/.netrc (#122)
+- Fix: Python HTTP proxies were broken after switch to urllib3 (#158)
+- Other: remove unused import in SQLAlchemy dialect
+- Other: Relax pandas dependency constraint to allow ^2.0.0 (#164)
+- Other: Connector now logs operation handle guids as hexadecimal instead of bytes (#170)
+- Other: test_socket_timeout_user_defined e2e test was broken (#144)
 
 ## 2.7.0 (2023-06-26)
 
 - Fix: connector raised exception when calling close() on a closed Thrift session
 - Improve e2e test development ergonomics
 - Redact logged thrift responses by default
 - Add support for OAuth on Databricks Azure
```

### Comparing `databricks_sql_connector-2.7.1.dev2/LICENSE` & `databricks_sql_connector-2.7.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/README.md` & `databricks_sql_connector-2.7.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/pyproject.toml` & `databricks_sql_connector-2.7.1.dev3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.7.1.dev2"
+version = "2.7.1.dev3"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 thrift = "^0.16.0"
-pandas = "^1.2.5"
+pandas = [
+    {version = ">=1.2.5,<1.4.0", python = ">=3.7,<3.8"},
+    {version =">=1.2.5,<3.0.0", python = ">=3.8"}
+]
+
 pyarrow = [
     {version = ">=6.0.0", python = ">=3.7,<3.11"},
     {version = ">=10.0.1", python = ">=3.11"}
 ]
 lz4 = "^4.0.2"
 requests="^2.18.1"
 oauthlib="^3.1.0"
 numpy = [
     {version = ">=1.16.6", python = ">=3.7,<3.11"},
     {version = ">=1.23.4", python = ">=3.11"}
 ]
-sqlalchemy = "^1.3.24"
+sqlalchemy = ">=1.3.24"
 openpyxl = "^3.0.10"
 alembic = "^1.0.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 mypy = "^0.950"
 pylint = ">=2.12.0"
```

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.7.1.dev2"
+__version__ = "2.7.1.dev3"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/client.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __del__(self):
         if self.open:
             logger.debug(
                 "Closing unclosed connection for session "
-                "{}".format(self.get_session_id())
+                "{}".format(self.get_session_id_hex())
             )
             try:
                 self._close(close_cursors=False)
             except OperationalError as e:
                 # Close on best-effort basis.
                 logger.debug("Couldn't close unclosed connection: {}".format(e.message))
```

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/download_manager.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/download_manager.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/downloader.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/cloudfetch/downloader.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/exc.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/thrift_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,32 +528,37 @@
         self, op_handle, get_operations_resp
     ):
         if get_operations_resp.operationState == ttypes.TOperationState.ERROR_STATE:
             if get_operations_resp.displayMessage:
                 raise ServerOperationError(
                     get_operations_resp.displayMessage,
                     {
-                        "operation-id": op_handle and op_handle.operationId.guid,
+                        "operation-id": op_handle
+                        and self.guid_to_hex_id(op_handle.operationId.guid),
                         "diagnostic-info": get_operations_resp.diagnosticInfo,
                     },
                 )
             else:
                 raise ServerOperationError(
                     get_operations_resp.errorMessage,
                     {
-                        "operation-id": op_handle and op_handle.operationId.guid,
+                        "operation-id": op_handle
+                        and self.guid_to_hex_id(op_handle.operationId.guid),
                         "diagnostic-info": None,
                     },
                 )
         elif get_operations_resp.operationState == ttypes.TOperationState.CLOSED_STATE:
             raise DatabaseError(
                 "Command {} unexpectedly closed server side".format(
-                    op_handle and op_handle.operationId.guid
+                    op_handle and self.guid_to_hex_id(op_handle.operationId.guid)
                 ),
-                {"operation-id": op_handle and op_handle.operationId.guid},
+                {
+                    "operation-id": op_handle
+                    and self.guid_to_hex_id(op_handle.operationId.guid)
+                },
             )
 
     def _poll_for_status(self, op_handle):
         req = ttypes.TGetOperationStatusReq(
             operationHandle=op_handle,
             getProgressUpdate=False,
         )
@@ -938,19 +943,43 @@
 
     def close_command(self, op_handle):
         req = ttypes.TCloseOperationReq(operationHandle=op_handle)
         resp = self.make_request(self._client.CloseOperation, req)
         return resp.status
 
     def cancel_command(self, active_op_handle):
-        logger.debug("Cancelling command {}".format(active_op_handle.operationId.guid))
+        logger.debug(
+            "Cancelling command {}".format(
+                self.guid_to_hex_id(active_op_handle.operationId.guid)
+            )
+        )
         req = ttypes.TCancelOperationReq(active_op_handle)
         self.make_request(self._client.CancelOperation, req)
 
     @staticmethod
     def handle_to_id(session_handle):
         return session_handle.sessionId.guid
 
     @staticmethod
     def handle_to_hex_id(session_handle: TCLIService.TSessionHandle):
         this_uuid = uuid.UUID(bytes=session_handle.sessionId.guid)
         return str(this_uuid)
+
+    @staticmethod
+    def guid_to_hex_id(guid: bytes) -> str:
+        """Return a hexadecimal string instead of bytes
+
+        Example:
+            IN   b'\x01\xee\x1d)\xa4\x19\x1d\xb6\xa9\xc0\x8d\xf1\xfe\xbaB\xdd'
+            OUT  '01ee1d29-a419-1db6-a9c0-8df1feba42dd'
+
+        If conversion to hexadecimal fails, the original bytes are returned
+        """
+
+        this_uuid: Union[bytes, uuid.UUID]
+
+        try:
+            this_uuid = uuid.UUID(bytes=guid)
+        except Exception as e:
+            logger.debug(f"Unable to convert bytes to UUID: {bytes} -- {str(e)}")
+            this_uuid = guid
+        return str(this_uuid)
```

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/types.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/utils.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module's layout loosely follows example of SQLAlchemy's postgres dialect
 """
 
 import decimal, re, datetime
 from dateutil.parser import parse
 
 import sqlalchemy
-from sqlalchemy import types, processors, event
+from sqlalchemy import types, event
 from sqlalchemy.engine import default, Engine
 from sqlalchemy.exc import DatabaseError, SQLAlchemyError
 from sqlalchemy.engine import reflection
 
 from databricks import sql
 
 
@@ -77,14 +77,15 @@
     preparer = DatabricksIdentifierPreparer
     type_compiler = DatabricksTypeCompiler
     ddl_compiler = DatabricksDDLCompiler
     supports_statement_cache: bool = True
     supports_multivalues_insert: bool = True
     supports_native_decimal: bool = True
     supports_sane_rowcount: bool = False
+    non_native_boolean_check_constraint: bool = False
 
     @classmethod
     def dbapi(cls):
         return sql
 
     def create_connect_args(self, url):
         # TODO: can schema be provided after HOST?
```

### Comparing `databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.7.1.dev3/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev2/PKG-INFO` & `databricks_sql_connector-2.7.1.dev3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.7.1.dev2
+Version: 2.7.1.dev3
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.0.11,<2.0.0)
 Requires-Dist: lz4 (>=4.0.2,<5.0.0)
 Requires-Dist: numpy (>=1.16.6) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: numpy (>=1.23.4) ; python_version >= "3.11"
 Requires-Dist: oauthlib (>=3.1.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=1.2.5,<2.0.0)
+Requires-Dist: pandas (>=1.2.5,<1.4.0) ; python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: pandas (>=1.2.5,<3.0.0) ; python_version >= "3.8"
 Requires-Dist: pyarrow (>=10.0.1) ; python_version >= "3.11"
 Requires-Dist: pyarrow (>=6.0.0) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: requests (>=2.18.1,<3.0.0)
-Requires-Dist: sqlalchemy (>=1.3.24,<2.0.0)
+Requires-Dist: sqlalchemy (>=1.3.24)
 Requires-Dist: thrift (>=0.16.0,<0.17.0)
 Project-URL: Bug Tracker, https://github.com/databricks/databricks-sql-python/issues
 Project-URL: Homepage, https://github.com/databricks/databricks-sql-python
 Description-Content-Type: text/markdown
 
 # Databricks SQL Connector for Python
```

