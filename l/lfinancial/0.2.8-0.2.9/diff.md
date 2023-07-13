# Comparing `tmp/lfinancial-0.2.8.tar.gz` & `tmp/lfinancial-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.2.8.tar", last modified: Tue Jul 11 14:39:17 2023, max compression
+gzip compressed data, was "lfinancial-0.2.9.tar", last modified: Thu Jul 13 03:50:35 2023, max compression
```

## Comparing `lfinancial-0.2.8.tar` & `lfinancial-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-11 14:39:00.000000 lfinancial-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 14:39:17.766598 lfinancial-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-11 14:39:00.000000 lfinancial-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.762598 lfinancial-0.2.8/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-11 14:39:00.000000 lfinancial-0.2.8/lfinancial/generators/timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.762598 lfinancial-0.2.8/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 14:39:17.000000 lfinancial-0.2.8/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:39:17.766598 lfinancial-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 14:39:00.000000 lfinancial-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:39:17.766598 lfinancial-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 14:39:00.000000 lfinancial-0.2.8/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:35.863874 lfinancial-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-13 03:50:17.000000 lfinancial-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-13 03:50:35.863874 lfinancial-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 03:50:17.000000 lfinancial-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:35.859874 lfinancial-0.2.9/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:35.863874 lfinancial-0.2.9/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-13 03:50:17.000000 lfinancial-0.2.9/lfinancial/generators/timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:35.859874 lfinancial-0.2.9/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-13 03:50:35.000000 lfinancial-0.2.9/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-13 03:50:35.000000 lfinancial-0.2.9/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 03:50:35.000000 lfinancial-0.2.9/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 03:50:35.000000 lfinancial-0.2.9/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 03:50:35.863874 lfinancial-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-13 03:50:17.000000 lfinancial-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 03:50:35.863874 lfinancial-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-13 03:50:17.000000 lfinancial-0.2.9/tests/test_document.py
```

### Comparing `lfinancial-0.2.8/LICENSE.txt` & `lfinancial-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/PKG-INFO` & `lfinancial-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -96,8 +96,11 @@
 # Asia/Baku
 
 f.locale()
 # zh-CN
 
 f.product()
 # Shares
+
+f.gender()
+# Cis Man
 ```
```

### Comparing `lfinancial-0.2.8/README.md` & `lfinancial-0.2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -84,8 +84,11 @@
 # Asia/Baku
 
 f.locale()
 # zh-CN
 
 f.product()
 # Shares
+
+f.gender()
+# Cis Man
 ```
```

### Comparing `lfinancial-0.2.8/lfinancial/factory.py` & `lfinancial-0.2.9/lfinancial/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from lfinancial.generators.bank import BankGenerator
 from lfinancial.generators.contry import CountryGenerator
 from lfinancial.generators.currency import CurrencyGenerator
 from lfinancial.generators.document import IDCodeGenerator
+from lfinancial.generators.gender import GenderGenerator
 from lfinancial.generators.locale import LocaleGenerator
 from lfinancial.generators.mail import EmailGenerator
 from lfinancial.generators.name import NameGenerator
 from lfinancial.generators.phone import PhoneGenerator
 from lfinancial.generators.stock import StockGenerator, TradeProduct
 from lfinancial.generators.swift import SwiftGenerator
 from lfinancial.generators.timezone import TimeZoneGenerator
@@ -32,14 +33,15 @@
             "currency": CurrencyGenerator(),
             "swift_code": SwiftGenerator(),
             "stock_exchange": StockGenerator(),
             "ticker_symbol": StockGenerator(),
             "tz_identifier": TimeZoneGenerator(),
             "locale": LocaleGenerator(),
             "product": StockGenerator(),
+            "gender": GenderGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.2.8/lfinancial/financial.py` & `lfinancial-0.2.9/lfinancial/financial.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
     def locale(self, country=None):
         return self._generate("locale", country)
 
     def product(self, country=None):
         return self._generate("product", country)
 
+    def gender(self, country=None):
+        return self.__generate("gender", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -96,7 +99,8 @@
     print(f.currency())
     print(f.swift_code())
     print(f.stock_exchange())
     print(f.ticker_symbol())
     print(f.tz_identifier())
     print(f.locale())
     print(f.product())
+    print(f.gender())
```

### Comparing `lfinancial-0.2.8/lfinancial/generators/bank.py` & `lfinancial-0.2.9/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/const.py` & `lfinancial-0.2.9/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/contry.py` & `lfinancial-0.2.9/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/currency.py` & `lfinancial-0.2.9/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/document.py` & `lfinancial-0.2.9/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/locale.py` & `lfinancial-0.2.9/lfinancial/generators/locale.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/mail.py` & `lfinancial-0.2.9/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/name.py` & `lfinancial-0.2.9/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/phone.py` & `lfinancial-0.2.9/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/stock.py` & `lfinancial-0.2.9/lfinancial/generators/stock.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/swift.py` & `lfinancial-0.2.9/lfinancial/generators/swift.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial/generators/timezone.py` & `lfinancial-0.2.9/lfinancial/generators/timezone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.2.8/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.2.9/lfinancial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -96,8 +96,11 @@
 # Asia/Baku
 
 f.locale()
 # zh-CN
 
 f.product()
 # Shares
+
+f.gender()
+# Cis Man
 ```
```

### Comparing `lfinancial-0.2.8/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.2.9/lfinancial.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 lfinancial.egg-info/top_level.txt
 lfinancial/generators/__init__.py
 lfinancial/generators/bank.py
 lfinancial/generators/const.py
 lfinancial/generators/contry.py
 lfinancial/generators/currency.py
 lfinancial/generators/document.py
+lfinancial/generators/gender.py
 lfinancial/generators/locale.py
 lfinancial/generators/mail.py
 lfinancial/generators/name.py
 lfinancial/generators/phone.py
 lfinancial/generators/stock.py
 lfinancial/generators/swift.py
 lfinancial/generators/timezone.py
```

### Comparing `lfinancial-0.2.8/setup.py` & `lfinancial-0.2.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.2.8',
+    version='0.2.9',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

