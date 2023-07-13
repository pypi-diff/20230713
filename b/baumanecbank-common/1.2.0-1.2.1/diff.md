# Comparing `tmp/baumanecbank_common-1.2.0.tar.gz` & `tmp/baumanecbank_common-1.2.1.tar.gz`

## Comparing `baumanecbank_common-1.2.0.tar` & `baumanecbank_common-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/Makefile
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/abstract.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/application.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/application_create.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/filter.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/handlers.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/i18n.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/log.py
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/postgres.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/src/baumanecbank_common/qr.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/.gitignore
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/Makefile
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/abstract.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/application.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/application_create.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/filter.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/handlers.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/i18n.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/log.py
+-rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/postgres.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/src/baumanecbank_common/qr.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/.gitignore
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 baumanecbank_common-1.2.1/PKG-INFO
```

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/__init__.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/__init__.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/application.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,29 @@
         self.pgcon:   PgCon = None
         self.i18n:    I18n  = None
         self.update:  Callable[[ApplicationBb], Coroutine[Any, Any, None]] = None
 
         self.reply_keyboard_keys = []
         self.reply_keyboard      = ReplyKeyboardRemove()
     
+    def get_keyboard_by_condition(self, condition: bool, condition_name: str = 'conditional_buttons', from_config: str = 'keyboard') -> ReplyKeyboardMarkup|ReplyKeyboardRemove:
+        if from_config not in self.i18n.app:
+            return ReplyKeyboardRemove()
+        
+        show_all_buttons = condition_name not in self.i18n.app or condition == True
+        keyboard_keys = [
+            val for fun,val in self.i18n.app[from_config].items()
+            if show_all_buttons or fun not in self.i18n.app[condition_name]
+        ] if from_config in self.i18n.app else []
+
+        return ReplyKeyboardMarkup([
+            keyboard_keys[idx:idx+2]
+            for idx in range(0,len(keyboard_keys),2)
+        ])
+    
     def init_keyboard(self, from_config: str = 'keyboard', attr_name: str = 'reply_keyboard') -> None:
         keyboard_keys = [
             val for _,val in self.i18n.app[from_config].items()
         ] if from_config in self.i18n.app else []
         setattr(self, f"{attr_name}_keys", keyboard_keys)
 
         if from_config not in self.i18n.app:
```

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/application_create.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/application_create.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/filter.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/filter.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/handlers.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/handlers.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/i18n.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/i18n.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/log.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/log.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/postgres.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,27 @@
                 "SELECT * "
                 "FROM active_clients_card_codes_balances "
                 f"WHERE chat_id = '{chat_id}'"
             ))
             if cursor.rowcount == 0:
                 return None
             return cursor.fetchone()
+
+    @retry(stop=stop_after_attempt(3), wait=wait_exponential())
+    @reconnect
+    def check_if_client_is_master_by_chat_id(self, chat_id: str|int) -> bool:
+        with self._connection.cursor(cursor_factory=psycopg2.extras.NamedTupleCursor) as cursor:
+            cursor.execute((
+                "SELECT is_master "
+                "FROM active_clients_card_codes_balances "
+                f"WHERE chat_id = '{chat_id}'"
+            ))
+            if cursor.rowcount == 0:
+                return False
+            return cursor.fetchone()[0]
     
     @retry(stop=stop_after_attempt(3), wait=wait_exponential())
     @reconnect
     def check_if_account_exists_by_chat_id(self, chat_id: str|int) -> bool:
         repl = self._get_exactly_one_or_none(
             f"select true from active_accounts_card_codes_balances where client_chat_id = '{chat_id}'"
         )
```

### Comparing `baumanecbank_common-1.2.0/src/baumanecbank_common/qr.py` & `baumanecbank_common-1.2.1/src/baumanecbank_common/qr.py`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/README.md` & `baumanecbank_common-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `baumanecbank_common-1.2.0/pyproject.toml` & `baumanecbank_common-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baumanecbank_common"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Egor Dubrovin", email="dubrovin.en@ya.ru" },
 ]
 description = "Common funcions package for Baumanec Bank bots"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `baumanecbank_common-1.2.0/PKG-INFO` & `baumanecbank_common-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baumanecbank_common
-Version: 1.2.0
+Version: 1.2.1
 Summary: Common funcions package for Baumanec Bank bots
 Project-URL: Homepage, https://github.com/twobrowin-study/baumanec-bank
 Project-URL: Bug Tracker, https://github.com/twobrowin-study/baumanec-bank/issues
 Author-email: Egor Dubrovin <dubrovin.en@ya.ru>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

