# Comparing `tmp/py-xbrl-2.2.7.tar.gz` & `tmp/py-xbrl-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-xbrl-2.2.7.tar", last modified: Mon Jul 10 10:18:32 2023, max compression
+gzip compressed data, was "py-xbrl-2.2.8.tar", last modified: Thu Jul 13 13:49:48 2023, max compression
```

## Comparing `py-xbrl-2.2.7.tar` & `py-xbrl-2.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/
--rw-rw-rw-   0        0        0    35821 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/LICENSE
--rw-rw-rw-   0        0        0     4006 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2941 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.326031 py-xbrl-2.2.7/py_xbrl.egg-info/
--rw-rw-rw-   0        0        0     4006 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 10:18:32.000000 py-xbrl-2.2.7/py_xbrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 10:18:32.406223 py-xbrl-2.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1733 2023-07-10 09:02:28.000000 py-xbrl-2.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.362889 py-xbrl-2.2.7/tests/
--rw-rw-rw-   0        0        0     2504 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_cache.py
--rw-rw-rw-   0        0        0     1436 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_instance.py
--rw-rw-rw-   0        0        0     1670 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_linkbase.py
--rw-rw-rw-   0        0        0     1157 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_local_taxonomy.py
--rw-rw-rw-   0        0        0     2616 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_instance.py
--rw-rw-rw-   0        0        0     2238 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_linkbase.py
--rw-rw-rw-   0        0        0     2193 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_remote_taxonomy.py
--rw-rw-rw-   0        0        0    16117 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_transformation.py
--rw-rw-rw-   0        0        0     4603 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/tests/test_uri_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.385845 py-xbrl-2.2.7/xbrl/
--rw-rw-rw-   0        0        0     2701 2023-07-10 09:02:28.000000 py-xbrl-2.2.7/xbrl/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.400066 py-xbrl-2.2.7/xbrl/helper/
--rw-rw-rw-   0        0        0        0 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/__init__.py
--rw-rw-rw-   0        0        0     2929 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/connection_manager.py
--rw-rw-rw-   0        0        0     2976 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/text2num.py
--rw-rw-rw-   0        0        0     2785 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/uri_helper.py
--rw-rw-rw-   0        0        0      986 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/helper/xml_parser.py
--rw-rw-rw-   0        0        0    33142 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/instance.py
--rw-rw-rw-   0        0        0    27789 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/linkbase.py
--rw-rw-rw-   0        0        0    53683 2023-07-10 08:50:01.000000 py-xbrl-2.2.7/xbrl/taxonomy.py
-drwxrwxrwx   0        0        0        0 2023-07-10 10:18:32.405216 py-xbrl-2.2.7/xbrl/transformations/
--rw-rw-rw-   0        0        0    21966 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/transformations/__init__.py
--rw-rw-rw-   0        0        0     3497 2023-05-06 19:08:12.000000 py-xbrl-2.2.7/xbrl/transformations/text2num.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:48.037039 py-xbrl-2.2.8/
+-rw-rw-rw-   0        0        0    35821 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/LICENSE
+-rw-rw-rw-   0        0        0     4006 2023-07-13 13:49:48.037039 py-xbrl-2.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2941 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:47.956839 py-xbrl-2.2.8/py_xbrl.egg-info/
+-rw-rw-rw-   0        0        0     4006 2023-07-13 13:49:47.000000 py-xbrl-2.2.8/py_xbrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-07-13 13:49:47.000000 py-xbrl-2.2.8/py_xbrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:49:47.000000 py-xbrl-2.2.8/py_xbrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-13 13:49:47.000000 py-xbrl-2.2.8/py_xbrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-13 13:49:47.000000 py-xbrl-2.2.8/py_xbrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:49:48.037039 py-xbrl-2.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1733 2023-07-13 13:48:28.000000 py-xbrl-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:47.994365 py-xbrl-2.2.8/tests/
+-rw-rw-rw-   0        0        0     2504 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1436 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_local_instance.py
+-rw-rw-rw-   0        0        0     1670 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_local_linkbase.py
+-rw-rw-rw-   0        0        0     1157 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_local_taxonomy.py
+-rw-rw-rw-   0        0        0     2616 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_remote_instance.py
+-rw-rw-rw-   0        0        0     2238 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_remote_linkbase.py
+-rw-rw-rw-   0        0        0     2193 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_remote_taxonomy.py
+-rw-rw-rw-   0        0        0    16117 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_transformation.py
+-rw-rw-rw-   0        0        0     4603 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/tests/test_uri_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:48.011054 py-xbrl-2.2.8/xbrl/
+-rw-rw-rw-   0        0        0     2701 2023-07-13 13:48:28.000000 py-xbrl-2.2.8/xbrl/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:48.028533 py-xbrl-2.2.8/xbrl/helper/
+-rw-rw-rw-   0        0        0        0 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/helper/__init__.py
+-rw-rw-rw-   0        0        0     2929 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/helper/connection_manager.py
+-rw-rw-rw-   0        0        0     2976 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/helper/text2num.py
+-rw-rw-rw-   0        0        0     2785 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/helper/uri_helper.py
+-rw-rw-rw-   0        0        0      986 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/helper/xml_parser.py
+-rw-rw-rw-   0        0        0    33142 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/instance.py
+-rw-rw-rw-   0        0        0    27789 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/linkbase.py
+-rw-rw-rw-   0        0        0    60368 2023-07-13 13:25:47.000000 py-xbrl-2.2.8/xbrl/taxonomy.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:49:48.035536 py-xbrl-2.2.8/xbrl/transformations/
+-rw-rw-rw-   0        0        0    21966 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/transformations/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-05-06 19:08:12.000000 py-xbrl-2.2.8/xbrl/transformations/text2num.py
```

### Comparing `py-xbrl-2.2.7/LICENSE` & `py-xbrl-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/PKG-INFO` & `py-xbrl-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-xbrl
-Version: 2.2.7
+Version: 2.2.8
 Summary: Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).
 Home-page: https://github.com/manusimidt/xbrl_parser
 Author: Manuel Schmidt
 Author-email: hello@schmidt-manuel.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-xbrl-2.2.7/README.md` & `py-xbrl-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/py_xbrl.egg-info/PKG-INFO` & `py-xbrl-2.2.8/py_xbrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-xbrl
-Version: 2.2.7
+Version: 2.2.8
 Summary: Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).
 Home-page: https://github.com/manusimidt/xbrl_parser
 Author: Manuel Schmidt
 Author-email: hello@schmidt-manuel.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-xbrl-2.2.7/py_xbrl.egg-info/SOURCES.txt` & `py-xbrl-2.2.8/py_xbrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/setup.py` & `py-xbrl-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="py-xbrl",
-    version="2.2.7",
+    version="2.2.8",
     url="https://github.com/manusimidt/xbrl_parser",
     license='GNU General Public License v3 (GPLv3)',
     author="Manuel Schmidt",
     author_email="hello@schmidt-manuel.de",
 
     description="Parser for parsing XBRL and iXBRL files (instance documents, taxonomy schemas, taxonomy linkbases).",
     long_description_content_type="text/markdown",
```

### Comparing `py-xbrl-2.2.7/tests/test_cache.py` & `py-xbrl-2.2.8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_local_instance.py` & `py-xbrl-2.2.8/tests/test_local_instance.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_local_linkbase.py` & `py-xbrl-2.2.8/tests/test_local_linkbase.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_local_taxonomy.py` & `py-xbrl-2.2.8/tests/test_local_taxonomy.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_remote_instance.py` & `py-xbrl-2.2.8/tests/test_remote_instance.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_remote_linkbase.py` & `py-xbrl-2.2.8/tests/test_remote_linkbase.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_remote_taxonomy.py` & `py-xbrl-2.2.8/tests/test_remote_taxonomy.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_transformation.py` & `py-xbrl-2.2.8/tests/test_transformation.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/tests/test_uri_helper.py` & `py-xbrl-2.2.8/tests/test_uri_helper.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/__init__.py` & `py-xbrl-2.2.8/xbrl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class ContextParseException(InstanceParseException):
     """
     Exception thrown when a Context could not be parsed
     """
     pass
 
 
-__version__ = '2.2.7'
+__version__ = '2.2.8'
 __author__ = 'Manuel Schmidt <hello@schmidt-manuel.de>'
 __all__ = [
     XbrlParseException,
     TaxonomyParseException,
     TaxonomyNotFound,
     InstanceParseException,
     ContextParseException,
```

### Comparing `py-xbrl-2.2.7/xbrl/cache.py` & `py-xbrl-2.2.8/xbrl/cache.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/helper/connection_manager.py` & `py-xbrl-2.2.8/xbrl/helper/connection_manager.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/helper/text2num.py` & `py-xbrl-2.2.8/xbrl/helper/text2num.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/helper/uri_helper.py` & `py-xbrl-2.2.8/xbrl/helper/uri_helper.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/helper/xml_parser.py` & `py-xbrl-2.2.8/xbrl/helper/xml_parser.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/instance.py` & `py-xbrl-2.2.8/xbrl/instance.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/linkbase.py` & `py-xbrl-2.2.8/xbrl/linkbase.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/taxonomy.py` & `py-xbrl-2.2.8/xbrl/taxonomy.py`

 * *Files 5% similar despite different names*

```diff
@@ -186,15 +186,14 @@
     "http://fasb.org/us-gaap/2018-01-31": "http://xbrl.fasb.org/us-gaap/2018/elts/us-gaap-2018-01-31.xsd",
     "http://fasb.org/us-gaap/2019-01-31": "http://xbrl.fasb.org/us-gaap/2019/elts/us-gaap-2019-01-31.xsd",
     "http://fasb.org/us-gaap/2020-01-31": "http://xbrl.fasb.org/us-gaap/2020/elts/us-gaap-2020-01-31.xsd",
     "http://fasb.org/us-gaap/2021-01-31": "http://xbrl.fasb.org/us-gaap/2021/elts/us-gaap-2021-01-31.xsd",
     "http://fasb.org/us-gaap/2022-01-31": "https://xbrl.fasb.org/us-gaap/2022/elts/us-gaap-2022.xsd",
     "http://fasb.org/us-gaap/2022": "https://xbrl.fasb.org/us-gaap/2022/elts/us-gaap-2022.xsd",
     "http://fasb.org/us-gaap/2023": "https://xbrl.fasb.org/us-gaap/2023/elts/us-gaap-2023.xsd",
-
     "http://fasb.org/us-roles/2011-01-31": "http://xbrl.fasb.org/us-gaap/2011/elts/us-roles-2011-01-31.xsd",
     "http://fasb.org/us-roles/2012-01-31": "http://xbrl.fasb.org/us-gaap/2012/elts/us-roles-2012-01-31.xsd",
     "http://fasb.org/us-roles/2013-01-31": "http://xbrl.fasb.org/us-gaap/2013/elts/us-roles-2013-01-31.xsd",
     "http://fasb.org/us-roles/2014-01-31": "http://xbrl.fasb.org/us-gaap/2014/elts/us-roles-2014-01-31.xsd",
     "http://fasb.org/us-roles/2015-01-31": "http://xbrl.fasb.org/us-gaap/2015/elts/us-roles-2015-01-31.xsd",
     "http://fasb.org/us-roles/2016-01-31": "http://xbrl.fasb.org/us-gaap/2016/elts/us-roles-2016-01-31.xsd",
     "http://fasb.org/us-roles/2017-01-31": "http://xbrl.fasb.org/us-gaap/2017/elts/us-roles-2017-01-31.xsd",
@@ -248,14 +247,16 @@
     "http://xbrl.ifrs.org/taxonomy/2016-03-31/ifrs-full": "http://xbrl.ifrs.org/taxonomy/2016-03-31/full_ifrs/full_ifrs-cor_2016-03-31.xsd",
     "http://xbrl.ifrs.org/taxonomy/2017-03-09/ifrs-full": "http://xbrl.ifrs.org/taxonomy/2017-03-09/full_ifrs/full_ifrs-cor_2017-03-09.xsd",
     "http://xbrl.ifrs.org/taxonomy/2018-03-16/ifrs-full": "http://xbrl.ifrs.org/taxonomy/2018-03-16/full_ifrs/full_ifrs-cor_2018-03-16.xsd",
     "http://xbrl.ifrs.org/taxonomy/2019-03-27/ifrs-full": "http://xbrl.ifrs.org/taxonomy/2019-03-27/full_ifrs/full_ifrs-cor_2019-03-27.xsd",
     "http://xbrl.ifrs.org/taxonomy/2020-03-16/ifrs-full": "http://xbrl.ifrs.org/taxonomy/2020-03-16/full_ifrs/full_ifrs-cor_2020-03-16.xsd",
     "http://xbrl.org/2005/xbrldt": "http://www.xbrl.org/2005/xbrldt-2005.xsd",
     "http://xbrl.org/2006/xbrldi": "http://www.xbrl.org/2006/xbrldi-2006.xsd",
+    "http://xbrl.org/2023/calculation-1.1": "https://www.xbrl.org/2023/calculation-1.1.xsd",
+    "http://xbrl.org/2014/extensible-enumerations": "http://www.xbrl.org/2014/extensible-enumerations.xsd",
     "http://xbrl.org/2020/extensible-enumerations-2.0": "http://www.xbrl.org/2020/extensible-enumerations-2.0.xsd",
     "http://xbrl.sec.gov/country/2011-01-31": "https://xbrl.sec.gov/country/2011/country-2011-01-31.xsd",
     "http://xbrl.sec.gov/country/2012-01-31": "https://xbrl.sec.gov/country/2012/country-2012-01-31.xsd",
     "http://xbrl.sec.gov/country/2013-01-31": "https://xbrl.sec.gov/country/2013/country-2013-01-31.xsd",
     "http://xbrl.sec.gov/country/2016-01-31": "https://xbrl.sec.gov/country/2016/country-2016-01-31.xsd",
     "http://xbrl.sec.gov/country/2017-01-31": "https://xbrl.sec.gov/country/2017/country-2017-01-31.xsd",
     "http://xbrl.sec.gov/country/2020-01-31": "https://xbrl.sec.gov/country/2020/country-2020-01-31.xsd",
@@ -333,15 +334,15 @@
     "http://xbrl.sec.gov/rr-pre/2021": "https://xbrl.sec.gov/rr/2021/rr-2021_pre.xsd",
     "http://xbrl.sec.gov/sic/2011-01-31": "https://xbrl.sec.gov/sic/2011/sic-2011-01-31.xsd",
     "http://xbrl.sec.gov/sic/2020-01-31": "https://xbrl.sec.gov/sic/2020/sic-2020-01-31.xsd",
     "http://xbrl.sec.gov/sic/2021": "https://xbrl.sec.gov/sic/2021/sic-2021.xsd",
     "http://xbrl.sec.gov/stpr/2011-01-31": "https://xbrl.sec.gov/stpr/2011/stpr-2011-01-31.xsd",
     "http://xbrl.sec.gov/stpr/2018-01-31": "https://xbrl.sec.gov/stpr/2018/stpr-2018-01-31.xsd",
     "http://xbrl.sec.gov/stpr/2021": "https://xbrl.sec.gov/stpr/2021/stpr-2021.xsd",
-    # Replace draft taxonomy with official STPR 2021 one once it is released
+    "http://xbrl.sec.gov/stpr/2022": "https://xbrl.sec.gov/stpr/2022/stpr-2022.xsd",
     "http://xbrl.us/ar/2008-03-31": "http://xbrl.us/us-gaap/1.0/non-gaap/ar-2008-03-31.xsd",
     "http://xbrl.us/ar/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/non-gaap/ar-2009-01-31.xsd",
     "http://xbrl.us/country/2008-03-31": "http://xbrl.us/us-gaap/1.0/non-gaap/country-2008-03-31.xsd",
     "http://xbrl.us/country/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/non-gaap/country-2009-01-31.xsd",
     "http://xbrl.us/currency/2008-03-31": "http://xbrl.us/us-gaap/1.0/non-gaap/currency-2008-03-31.xsd",
     "http://xbrl.us/currency/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/non-gaap/currency-2009-01-31.xsd",
     "http://xbrl.us/dei/2008-03-31": "http://xbrl.us/us-gaap/1.0/non-gaap/dei-2008-03-31.xsd",
@@ -371,14 +372,84 @@
     "http://xbrl.us/us-gaap/2008-03-31": "http://xbrl.us/us-gaap/1.0/elts/us-gaap-2008-03-31.xsd",
     "http://xbrl.us/us-gaap/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/elts/us-gaap-2009-01-31.xsd",
     "http://xbrl.us/us-gaap/negated/2008-03-31": "http://www.xbrl.org/lrr/role/negated-2008-03-31.xsd",
     "http://xbrl.us/us-roles/2008-03-31": "http://xbrl.us/us-gaap/1.0/elts/us-roles-2008-03-31.xsd",
     "http://xbrl.us/us-roles/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/elts/us-roles-2009-01-31.xsd",
     "http://xbrl.us/us-types/2008-03-31": "http://xbrl.us/us-gaap/1.0/elts/us-types-2008-03-31.xsd",
     "http://xbrl.us/us-types/2009-01-31": "http://taxonomies.xbrl.us/us-gaap/2009/elts/us-types-2009-01-31.xsd",
+    'http://xbrl.sec.gov/rxp/2023': 'https://xbrl.sec.gov/rxp/2023/rxp-2023.xsd',
+    'http://xbrl.sec.gov/snj/2023': 'https://xbrl.sec.gov/snj/2023/snj-2023.xsd',
+    'http://xbrl.sec.gov/snj-def/2023': 'https://xbrl.sec.gov/snj/2023/snj-2023_def.xsd',
+    'http://xbrl.sec.gov/country-def/2023': 'https://xbrl.sec.gov/country/2023/country-2023_def.xsd',
+    'http://xbrl.sec.gov/oef/2023': 'https://xbrl.sec.gov/oef/2023/oef-2023.xsd',
+    'http://xbrl.sec.gov/oef-rr/2023': 'https://xbrl.sec.gov/oef/2023/oef-rr-2023.xsd',
+    'http://xbrl.sec.gov/oef-sr/2023': 'https://xbrl.sec.gov/oef/2023/oef-sr-2023.xsd',
+    'http://xbrl.sec.gov/oef-lab/2023': 'https://xbrl.sec.gov/oef/2023/oef-2023_lab.xsd',
+    'http://xbrl.sec.gov/oef-cal/2023': 'https://xbrl.sec.gov/oef/2023/oef-2023_cal.xsd',
+    'https://xbrl.ifrs.org/taxonomy/2023-03-23/ifrs-full': 'https://xbrl.ifrs.org/taxonomy/2023-03-23/full_ifrs/full_ifrs-cor_2023-03-23.xsd',
+    'http://xbrl.sec.gov/rr-sub/2023': 'https://xbrl.sec.gov/rr/2023/rr-sub-2023.xsd',
+    'http://xbrl.sec.gov/rr-cal/2023': 'https://xbrl.sec.gov/rr/2023/rr-2023_cal.xsd',
+    'http://xbrl.sec.gov/dei-sub/2023': 'https://xbrl.sec.gov/dei/2023/dei-sub-2023.xsd',
+    'http://xbrl.sec.gov/dei-def/2023': 'https://xbrl.sec.gov/dei/2023/dei-2023_def.xsd',
+    'http://xbrl.sec.gov/dei-lab/2023': 'https://xbrl.sec.gov/dei/2023/dei-2023_lab.xsd',
+    'http://xbrl.sec.gov/dei-pre/2023': 'https://xbrl.sec.gov/dei/2023/dei-2023_pre.xsd',
+    'http://xbrl.sec.gov/dei/2022q4': 'https://xbrl.sec.gov/dei/2022q4/dei-2022q4.xsd',
+    'http://xbrl.sec.gov/dei-sub/2022q4': 'https://xbrl.sec.gov/dei/2022q4/dei-sub-2022q4.xsd',
+    'http://xbrl.sec.gov/dei-def/2022q4': 'https://xbrl.sec.gov/dei/2022q4/dei-2022q4_def.xsd',
+    'http://xbrl.sec.gov/dei-lab/2022q4': 'https://xbrl.sec.gov/dei/2022q4/dei-2022q4_lab.xsd',
+    'http://xbrl.sec.gov/dei-pre/2022q4': 'https://xbrl.sec.gov/dei/2022q4/dei-2022q4_pre.xsd',
+    'http://xbrl.sec.gov/ecd/2023': 'https://xbrl.sec.gov/ecd/2023/ecd-2023.xsd',
+    'http://xbrl.sec.gov/ecd-sub/2023': 'https://xbrl.sec.gov/ecd/2023/ecd-sub-2023.xsd',
+    'http://xbrl.sec.gov/ecd/2022q4': 'https://xbrl.sec.gov/ecd/2022q4/ecd-2022q4.xsd',
+    'http://xbrl.sec.gov/ecd-sub/2022q4': 'https://xbrl.sec.gov/ecd/2022q4/ecd-sub-2022q4.xsd',
+    'http://fasb.org/srt-sup/2022q3': 'https://xbrl.fasb.org/srt/2022q3/srt-sup-2022q3.xsd',
+    'http://fasb.org/us-gaap-sup/2022q3': 'https://xbrl.fasb.org/us-gaap/2022q3/us-gaap-sup-2022q3.xsd',
+    'http://xbrl.sec.gov/vip/2023': 'https://xbrl.sec.gov/vip/2023/vip-2023.xsd',
+    'http://xbrl.sec.gov/vip-n3/2023': 'https://xbrl.sec.gov/vip/2023/vip-n3-2023.xsd',
+    'http://xbrl.sec.gov/vip-n4/2023': 'https://xbrl.sec.gov/vip/2023/vip-n4-2023.xsd',
+    'http://xbrl.sec.gov/vip-n6/2023': 'https://xbrl.sec.gov/vip/2023/vip-n6-2023.xsd',
+    'http://xbrl.sec.gov/country/2023': 'https://xbrl.sec.gov/country/2023/country-2023.xsd',
+    'http://xbrl.sec.gov/currency/2023': 'https://xbrl.sec.gov/currency/2023/currency-2023.xsd',
+    'http://xbrl.sec.gov/vip/2022q2': 'https://xbrl.sec.gov/vip/2022q2/vip-2022q2.xsd',
+    'http://xbrl.sec.gov/vip-n3/2022q2': 'https://xbrl.sec.gov/vip/2022q2/vip-n3-2022q2.xsd',
+    'http://xbrl.sec.gov/vip-n4/2022q2': 'https://xbrl.sec.gov/vip/2022q2/vip-n4-2022q2.xsd',
+    'http://xbrl.sec.gov/vip-n6/2022q2': 'https://xbrl.sec.gov/vip/2022q2/vip-n6-2022q2.xsd',
+    'http://xbrl.sec.gov/country/2022': 'https://xbrl.sec.gov/country/2022/country-2022.xsd',
+    'http://xbrl.sec.gov/sic/2022': 'https://xbrl.sec.gov/sic/2022/sic-2022.xsd',
+    'https://xbrl.ifrs.org/taxonomy/2022-03-24/ifrs-full': 'https://xbrl.ifrs.org/taxonomy/2022-03-24/full_ifrs/full_ifrs-cor_2022-03-24.xsd',
+    'http://xbrl.sec.gov/dei-lab/2022': 'https://xbrl.sec.gov/dei/2022/dei-2022_lab.xsd',
+    'http://xbrl.sec.gov/dei-pre/2022': 'https://xbrl.sec.gov/dei/2022/dei-2022_pre.xsd',
+    'http://xbrl.sec.gov/dei-def/2022': 'https://xbrl.sec.gov/dei/2022/dei-2022_def.xsd',
+    'http://xbrl.sec.gov/sic/2023': 'https://xbrl.sec.gov/sic/2023/sic-2023.xsd',
+    'http://xbrl.sec.gov/stpr/2023': 'https://xbrl.sec.gov/stpr/2023/stpr-2023.xsd',
+    'http://fasb.org/us-types/2023': 'https://xbrl.fasb.org/us-gaap/2023/elts/us-types-2023.xsd',
+    'http://fasb.org/us-roles/2023': 'https://xbrl.fasb.org/us-gaap/2023/elts/us-roles-2023.xsd',
+    'http://fasb.org/srt-types/2023': 'https://xbrl.fasb.org/srt/2023/elts/srt-types-2023.xsd',
+    'http://fasb.org/srt-roles/2023': 'https://xbrl.fasb.org/srt/2023/elts/srt-roles-2023.xsd',
+    'http://xbrl.sec.gov/dei-sub/2022': 'https://xbrl.sec.gov/dei/2022/dei-sub-2022.xsd',
+    'http://fasb.org/us-types/2022': 'https://xbrl.fasb.org/us-gaap/2022/elts/us-types-2022.xsd',
+    'http://fasb.org/us-roles/2022': 'https://xbrl.fasb.org/us-gaap/2022/elts/us-roles-2022.xsd',
+    'http://fasb.org/srt-types/2022': 'https://xbrl.fasb.org/srt/2022/elts/srt-types-2022.xsd',
+    'http://fasb.org/srt-roles/2022': 'https://xbrl.fasb.org/srt/2022/elts/srt-roles-2022.xsd',
+    'http://xbrl.sec.gov/cef/2023': 'https://xbrl.sec.gov/cef/2023/cef-2023.xsd',
+    'http://xbrl.sec.gov/cef-pre/2023': 'https://xbrl.sec.gov/cef/2023/cef-2023_pre.xsd',
+    'http://xbrl.sec.gov/cef/2022': 'https://xbrl.sec.gov/cef/2022/cef-2022.xsd',
+    'http://xbrl.sec.gov/vip/2022': 'https://xbrl.sec.gov/vip/2022/vip-2022.xsd',
+    'http://xbrl.sec.gov/vip-n3/2022': 'https://xbrl.sec.gov/vip/2022/vip-n3-2022.xsd',
+    'http://xbrl.sec.gov/vip-n4/2022': 'https://xbrl.sec.gov/vip/2022/vip-n4-2022.xsd',
+    'http://xbrl.sec.gov/vip-n6/2022': 'https://xbrl.sec.gov/vip/2022/vip-n6-2022.xsd',
+    'http://xbrl.sec.gov/rr/2023': 'https://xbrl.sec.gov/rr/2023/rr-2023.xsd',
+    'http://xbrl.sec.gov/rr-lab/2023': 'https://xbrl.sec.gov/rr/2023/rr-2023_lab.xsd',
+    'http://xbrl.sec.gov/rr-pre/2023': 'https://xbrl.sec.gov/rr/2023/rr-2023_pre.xsd',
+    'http://xbrl.sec.gov/rr-def/2023': 'https://xbrl.sec.gov/rr/2023/rr-2023_def.xsd',
+    'http://xbrl.sec.gov/rr/2022': 'https://xbrl.sec.gov/rr/2022/rr-2022.xsd',
+    'http://xbrl.sec.gov/rr-lab/2022': 'https://xbrl.sec.gov/rr/2022/rr-2022_lab.xsd',
+    'http://xbrl.sec.gov/rr-pre/2022': 'https://xbrl.sec.gov/rr/2022/rr-2022_pre.xsd',
+    'http://xbrl.sec.gov/rr-def/2022': 'https://xbrl.sec.gov/rr/2022/rr-2022_def.xsd',
+    'http://www.xbrl.org/dtr/type/2022-03-31': 'https://www.xbrl.org/dtr/type/2022-03-31/types.xsd'
 }
 
 
 class Concept:
     """
     Class representing a Concept defined in the schema (xs:element)
     i.e:
```

### Comparing `py-xbrl-2.2.7/xbrl/transformations/__init__.py` & `py-xbrl-2.2.8/xbrl/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `py-xbrl-2.2.7/xbrl/transformations/text2num.py` & `py-xbrl-2.2.8/xbrl/transformations/text2num.py`

 * *Files identical despite different names*

