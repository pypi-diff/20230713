# Comparing `tmp/nicknames-0.1.4.tar.gz` & `tmp/nicknames-0.1.5.tar.gz`

## Comparing `nicknames-0.1.4.tar` & `nicknames-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.4/test_package.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/_compat.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/_version.py
--rw-r--r--   0        0        0    22788 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/names.csv
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.4/.gitignore
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.4/hatch_build.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 nicknames-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.4/../README.md
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nicknames-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.5/test_package.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/_compat.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/_version.py
+-rw-r--r--   0        0        0    22798 2020-02-02 00:00:00.000000 nicknames-0.1.5/src/nicknames/names.csv
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.5/hatch_build.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 nicknames-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.5/../README.md
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nicknames-0.1.5/PKG-INFO
```

### Comparing `nicknames-0.1.4/test_package.py` & `nicknames-0.1.5/test_package.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/src/nicknames/__init__.py` & `nicknames-0.1.5/src/nicknames/__init__.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/src/nicknames/_compat.py` & `nicknames-0.1.5/src/nicknames/_compat.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/src/nicknames/names.csv` & `nicknames-0.1.5/src/nicknames/names.csv`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 amanda,mandy,manda
 ambrose,brose
 amelia,amy,mel,millie,emily
 amos,moses
 anastasia,ana,stacy
 anderson,andy
 andre,drea
-andrea,drea,rea,andrew
+andrea,drea,rea,andrew,andi,andy
 andrew,andy,drew
 andriane,ada,adri,rienne
 angela,angel,angie
 angelica,angie,angel
 angelina,angel,angie,lina
 ann,annie,nan
 anna,anne,ann,annie,nan
```

### Comparing `nicknames-0.1.4/hatch_build.py` & `nicknames-0.1.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/pyproject.toml` & `nicknames-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/../README.md` & `nicknames-0.1.5/../README.md`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.4/PKG-INFO` & `nicknames-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicknames
-Version: 0.1.4
+Version: 0.1.5
 Summary: Hand-curated dataset of English given names and nicknames
 Project-URL: Homepage, https://github.com/carltonnorthern/nicknames
 Project-URL: Bug Tracker, https://github.com/carltonnorthern/nicknames/issues
 Author-email: Carlton Northern <carlton.northern@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

