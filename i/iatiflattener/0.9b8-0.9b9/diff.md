# Comparing `tmp/iatiflattener-0.9b8.tar.gz` & `tmp/iatiflattener-0.9b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iatiflattener-0.9b8.tar", last modified: Sun Oct  3 20:00:26 2021, max compression
+gzip compressed data, was "iatiflattener-0.9b9.tar", last modified: Sun Oct  3 22:56:18 2021, max compression
```

## Comparing `iatiflattener-0.9b8.tar` & `iatiflattener-0.9b9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 20:00:26.234037 iatiflattener-0.9b8/
--rw-r--r--   0 mark       (502) staff       (20)    34522 2021-02-06 12:28:29.000000 iatiflattener-0.9b8/LICENSE
--rw-r--r--   0 mark       (502) staff       (20)      517 2021-10-03 20:00:26.233747 iatiflattener-0.9b8/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      313 2021-02-18 15:26:42.000000 iatiflattener-0.9b8/README.md
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 20:00:26.224813 iatiflattener-0.9b8/iatiflattener/
--rw-r--r--   0 mark       (502) staff       (20)     7024 2021-10-03 13:33:15.000000 iatiflattener-0.9b8/iatiflattener/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)     5986 2021-09-29 12:52:08.000000 iatiflattener-0.9b8/iatiflattener/__init__old.py
--rw-r--r--   0 mark       (502) staff       (20)     3313 2021-09-29 08:34:32.000000 iatiflattener-0.9b8/iatiflattener/activity.py
--rw-r--r--   0 mark       (502) staff       (20)    10983 2021-09-28 14:12:36.000000 iatiflattener-0.9b8/iatiflattener/budget.py
--rw-r--r--   0 mark       (502) staff       (20)    10983 2021-10-01 12:10:10.000000 iatiflattener-0.9b8/iatiflattener/budget_old.py
--rw-r--r--   0 mark       (502) staff       (20)     4625 2021-09-29 15:53:45.000000 iatiflattener-0.9b8/iatiflattener/data_quality.py
--rw-r--r--   0 mark       (502) staff       (20)     7451 2021-10-03 19:59:02.000000 iatiflattener-0.9b8/iatiflattener/group_data.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 20:00:26.231430 iatiflattener-0.9b8/iatiflattener/lib/
--rw-r--r--   0 mark       (502) staff       (20)        0 2021-02-06 13:04:04.000000 iatiflattener-0.9b8/iatiflattener/lib/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)     3439 2021-09-30 13:37:53.000000 iatiflattener-0.9b8/iatiflattener/lib/iati_budget_helpers.py
--rw-r--r--   0 mark       (502) staff       (20)     4828 2021-10-01 23:23:38.000000 iatiflattener-0.9b8/iatiflattener/lib/iati_helpers.py
--rw-r--r--   0 mark       (502) staff       (20)     4885 2021-10-01 11:55:49.000000 iatiflattener-0.9b8/iatiflattener/lib/iati_transaction_helpers.py
--rw-r--r--   0 mark       (502) staff       (20)      706 2021-02-06 12:28:29.000000 iatiflattener-0.9b8/iatiflattener/lib/utils.py
--rw-r--r--   0 mark       (502) staff       (20)     5044 2021-10-02 20:08:00.000000 iatiflattener-0.9b8/iatiflattener/lib/variables.py
--rw-r--r--   0 mark       (502) staff       (20)    43136 2021-10-03 13:20:49.000000 iatiflattener-0.9b8/iatiflattener/model.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 20:00:26.233121 iatiflattener-0.9b8/iatiflattener/tests/
--rw-r--r--   0 mark       (502) staff       (20)        0 2021-09-28 14:42:11.000000 iatiflattener-0.9b8/iatiflattener/tests/__init__.py
--rw-r--r--   0 mark       (502) staff       (20)     2286 2021-10-01 12:21:30.000000 iatiflattener-0.9b8/iatiflattener/tests/test_budget.py
--rw-r--r--   0 mark       (502) staff       (20)     3212 2021-10-01 12:21:28.000000 iatiflattener-0.9b8/iatiflattener/tests/test_transaction.py
--rw-r--r--   0 mark       (502) staff       (20)    10100 2021-09-28 19:47:21.000000 iatiflattener-0.9b8/iatiflattener/transaction.py
--rw-r--r--   0 mark       (502) staff       (20)    10100 2021-09-29 12:07:52.000000 iatiflattener-0.9b8/iatiflattener/transaction_new.py
--rw-r--r--   0 mark       (502) staff       (20)    10100 2021-10-01 12:10:20.000000 iatiflattener-0.9b8/iatiflattener/transaction_old.py
-drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 20:00:26.228065 iatiflattener-0.9b8/iatiflattener.egg-info/
--rw-r--r--   0 mark       (502) staff       (20)      517 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/PKG-INFO
--rw-r--r--   0 mark       (502) staff       (20)      917 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/namespace_packages.txt
--rw-r--r--   0 mark       (502) staff       (20)        1 2021-02-06 12:42:28.000000 iatiflattener-0.9b8/iatiflattener.egg-info/not-zip-safe
--rw-r--r--   0 mark       (502) staff       (20)      129 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/requires.txt
--rw-r--r--   0 mark       (502) staff       (20)       14 2021-10-03 20:00:26.000000 iatiflattener-0.9b8/iatiflattener.egg-info/top_level.txt
--rw-r--r--   0 mark       (502) staff       (20)       38 2021-10-03 20:00:26.234164 iatiflattener-0.9b8/setup.cfg
--rw-r--r--   0 mark       (502) staff       (20)      932 2021-10-03 19:59:41.000000 iatiflattener-0.9b8/setup.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 22:56:18.853467 iatiflattener-0.9b9/
+-rw-r--r--   0 mark       (502) staff       (20)    34522 2021-02-06 12:28:29.000000 iatiflattener-0.9b9/LICENSE
+-rw-r--r--   0 mark       (502) staff       (20)      517 2021-10-03 22:56:18.853223 iatiflattener-0.9b9/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      313 2021-02-18 15:26:42.000000 iatiflattener-0.9b9/README.md
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 22:56:18.845504 iatiflattener-0.9b9/iatiflattener/
+-rw-r--r--   0 mark       (502) staff       (20)     7024 2021-10-03 13:33:15.000000 iatiflattener-0.9b9/iatiflattener/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     5986 2021-09-29 12:52:08.000000 iatiflattener-0.9b9/iatiflattener/__init__old.py
+-rw-r--r--   0 mark       (502) staff       (20)     3313 2021-09-29 08:34:32.000000 iatiflattener-0.9b9/iatiflattener/activity.py
+-rw-r--r--   0 mark       (502) staff       (20)    10983 2021-09-28 14:12:36.000000 iatiflattener-0.9b9/iatiflattener/budget.py
+-rw-r--r--   0 mark       (502) staff       (20)    10983 2021-10-01 12:10:10.000000 iatiflattener-0.9b9/iatiflattener/budget_old.py
+-rw-r--r--   0 mark       (502) staff       (20)     4625 2021-09-29 15:53:45.000000 iatiflattener-0.9b9/iatiflattener/data_quality.py
+-rw-r--r--   0 mark       (502) staff       (20)     7529 2021-10-03 22:54:10.000000 iatiflattener-0.9b9/iatiflattener/group_data.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 22:56:18.851013 iatiflattener-0.9b9/iatiflattener/lib/
+-rw-r--r--   0 mark       (502) staff       (20)        0 2021-02-06 13:04:04.000000 iatiflattener-0.9b9/iatiflattener/lib/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     3439 2021-09-30 13:37:53.000000 iatiflattener-0.9b9/iatiflattener/lib/iati_budget_helpers.py
+-rw-r--r--   0 mark       (502) staff       (20)     4828 2021-10-01 23:23:38.000000 iatiflattener-0.9b9/iatiflattener/lib/iati_helpers.py
+-rw-r--r--   0 mark       (502) staff       (20)     4885 2021-10-01 11:55:49.000000 iatiflattener-0.9b9/iatiflattener/lib/iati_transaction_helpers.py
+-rw-r--r--   0 mark       (502) staff       (20)      706 2021-02-06 12:28:29.000000 iatiflattener-0.9b9/iatiflattener/lib/utils.py
+-rw-r--r--   0 mark       (502) staff       (20)     5044 2021-10-02 20:08:00.000000 iatiflattener-0.9b9/iatiflattener/lib/variables.py
+-rw-r--r--   0 mark       (502) staff       (20)    43136 2021-10-03 13:20:49.000000 iatiflattener-0.9b9/iatiflattener/model.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 22:56:18.852537 iatiflattener-0.9b9/iatiflattener/tests/
+-rw-r--r--   0 mark       (502) staff       (20)        0 2021-09-28 14:42:11.000000 iatiflattener-0.9b9/iatiflattener/tests/__init__.py
+-rw-r--r--   0 mark       (502) staff       (20)     2286 2021-10-01 12:21:30.000000 iatiflattener-0.9b9/iatiflattener/tests/test_budget.py
+-rw-r--r--   0 mark       (502) staff       (20)     3212 2021-10-01 12:21:28.000000 iatiflattener-0.9b9/iatiflattener/tests/test_transaction.py
+-rw-r--r--   0 mark       (502) staff       (20)    10100 2021-09-28 19:47:21.000000 iatiflattener-0.9b9/iatiflattener/transaction.py
+-rw-r--r--   0 mark       (502) staff       (20)    10100 2021-09-29 12:07:52.000000 iatiflattener-0.9b9/iatiflattener/transaction_new.py
+-rw-r--r--   0 mark       (502) staff       (20)    10100 2021-10-01 12:10:20.000000 iatiflattener-0.9b9/iatiflattener/transaction_old.py
+drwxr-xr-x   0 mark       (502) staff       (20)        0 2021-10-03 22:56:18.848454 iatiflattener-0.9b9/iatiflattener.egg-info/
+-rw-r--r--   0 mark       (502) staff       (20)      517 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (502) staff       (20)      917 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/namespace_packages.txt
+-rw-r--r--   0 mark       (502) staff       (20)        1 2021-02-06 12:42:28.000000 iatiflattener-0.9b9/iatiflattener.egg-info/not-zip-safe
+-rw-r--r--   0 mark       (502) staff       (20)      129 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/requires.txt
+-rw-r--r--   0 mark       (502) staff       (20)       14 2021-10-03 22:56:18.000000 iatiflattener-0.9b9/iatiflattener.egg-info/top_level.txt
+-rw-r--r--   0 mark       (502) staff       (20)       38 2021-10-03 22:56:18.853568 iatiflattener-0.9b9/setup.cfg
+-rw-r--r--   0 mark       (502) staff       (20)      932 2021-10-03 22:55:38.000000 iatiflattener-0.9b9/setup.py
```

### Comparing `iatiflattener-0.9b8/LICENSE` & `iatiflattener-0.9b9/LICENSE`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/PKG-INFO` & `iatiflattener-0.9b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iatiflattener
-Version: 0.9b8
+Version: 0.9b9
 Summary: A set of tools to flatten IATI data.
 Home-page: https://github.com/iati-data-access/iati-flattener
 Author: Mark Brough
 Author-email: mark@brough.io
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `iatiflattener-0.9b8/iatiflattener/__init__.py` & `iatiflattener-0.9b9/iatiflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/__init__old.py` & `iatiflattener-0.9b9/iatiflattener/__init__old.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/activity.py` & `iatiflattener-0.9b9/iatiflattener/activity.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/budget.py` & `iatiflattener-0.9b9/iatiflattener/budget.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/budget_old.py` & `iatiflattener-0.9b9/iatiflattener/budget_old.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/data_quality.py` & `iatiflattener-0.9b9/iatiflattener/data_quality.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/group_data.py` & `iatiflattener-0.9b9/iatiflattener/group_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,20 @@
 
     def group_results(self, country_code):
         for lang in self.langs:
             df_transaction = self.get_dataframe(country_code, 'transaction', lang)
             df_budget = self.get_dataframe(country_code, 'budget', lang)
             if (df_transaction is None) and (df_budget is None):
                 continue
-            elif (df_transaction is None) or (df_budget is None):
-                df = df_transaction or df_budget
-            else:
+            elif (df_transaction is not None) and (df_budget is not None):
                 df = pd.concat([df_transaction, df_budget], ignore_index=True)
+            else:
+                if df_transaction is not None:
+                    df = df_transaction
+                df = df_budget
 
             self.write_dataframe_to_excel(
                 dataframe = df,
                 filename = "output/xlsx/{}/{}.xlsx".format(lang, country_code),
                 lang = lang)
```

### Comparing `iatiflattener-0.9b8/iatiflattener/lib/iati_budget_helpers.py` & `iatiflattener-0.9b9/iatiflattener/lib/iati_budget_helpers.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/lib/iati_helpers.py` & `iatiflattener-0.9b9/iatiflattener/lib/iati_helpers.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/lib/iati_transaction_helpers.py` & `iatiflattener-0.9b9/iatiflattener/lib/iati_transaction_helpers.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/lib/utils.py` & `iatiflattener-0.9b9/iatiflattener/lib/utils.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/lib/variables.py` & `iatiflattener-0.9b9/iatiflattener/lib/variables.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/model.py` & `iatiflattener-0.9b9/iatiflattener/model.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/tests/test_budget.py` & `iatiflattener-0.9b9/iatiflattener/tests/test_budget.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/tests/test_transaction.py` & `iatiflattener-0.9b9/iatiflattener/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/transaction.py` & `iatiflattener-0.9b9/iatiflattener/transaction.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/transaction_new.py` & `iatiflattener-0.9b9/iatiflattener/transaction_new.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener/transaction_old.py` & `iatiflattener-0.9b9/iatiflattener/transaction_old.py`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/iatiflattener.egg-info/PKG-INFO` & `iatiflattener-0.9b9/iatiflattener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iatiflattener
-Version: 0.9b8
+Version: 0.9b9
 Summary: A set of tools to flatten IATI data.
 Home-page: https://github.com/iati-data-access/iati-flattener
 Author: Mark Brough
 Author-email: mark@brough.io
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `iatiflattener-0.9b8/iatiflattener.egg-info/SOURCES.txt` & `iatiflattener-0.9b9/iatiflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iatiflattener-0.9b8/setup.py` & `iatiflattener-0.9b9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 openpyxl>=3.0.5
 iatikit>=2.3.0
 """
 
 setup(
     name="iatiflattener",
     packages=find_packages(exclude=['ez_setup', 'examples']),
-    version='0.9b8',
+    version='0.9b9',
     description="A set of tools to flatten IATI data.",
     author="Mark Brough",
     author_email="mark@brough.io",
     url="https://github.com/iati-data-access/iati-flattener",
     license="AGPLv3+",
     install_requires=requirements.strip().splitlines(),
     classifiers=(
```

