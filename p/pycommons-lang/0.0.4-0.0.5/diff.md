# Comparing `tmp/pycommons_lang-0.0.4.tar.gz` & `tmp/pycommons_lang-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_lang-0.0.4.tar", max compression
+gzip compressed data, was "pycommons_lang-0.0.5.tar", max compression
```

## Comparing `pycommons_lang-0.0.4.tar` & `pycommons_lang-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,17 @@
--rw-r--r--   0        0        0    11346 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/LICENSE
--rw-r--r--   0        0        0     1343 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/README.md
--rw-r--r--   0        0        0      431 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/pycommons/lang/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 16:12:10.109142 pycommons_lang-0.0.4/pycommons/lang/utils/__init__.py
--rw-r--r--   0        0        0      399 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/arrayutils.py
--rw-r--r--   0        0        0     2380 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/charutils.py
--rw-r--r--   0        0        0    11143 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/lang/utils/stringutils.py
--rw-r--r--   0        0        0        0 2023-06-11 16:12:10.113144 pycommons_lang-0.0.4/pycommons/py.typed
--rw-r--r--   0        0        0     1823 2023-06-11 16:12:26.394337 pycommons_lang-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 pycommons_lang-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1343 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/README.md
+-rw-r--r--   0        0        0      783 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/arrayutils.py
+-rw-r--r--   0        0        0    10142 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/booleanutils.py
+-rw-r--r--   0        0        0     2380 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/charutils.py
+-rw-r--r--   0        0        0      197 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/exception/__init__.py
+-rw-r--r--   0        0        0     1751 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/exception/contexted.py
+-rw-r--r--   0        0        0      654 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/exception/exception.py
+-rw-r--r--   0        0        0     1805 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/exception/exceptionutils.py
+-rw-r--r--   0        0        0    11742 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/stringutils.py
+-rw-r--r--   0        0        0      208 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/tuple/__init__.py
+-rw-r--r--   0        0        0     2242 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/tuple/pair.py
+-rw-r--r--   0        0        0     2507 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/lang/tuple/triple.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:50:00.684033 pycommons_lang-0.0.5/pycommons/py.typed
+-rw-r--r--   0        0        0     1823 2023-07-13 18:50:13.500182 pycommons_lang-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 pycommons_lang-0.0.5/PKG-INFO
```

### Comparing `pycommons_lang-0.0.4/LICENSE` & `pycommons_lang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycommons_lang-0.0.4/README.md` & `pycommons_lang-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pycommons_lang-0.0.4/pycommons/lang/utils/charutils.py` & `pycommons_lang-0.0.5/pycommons/lang/charutils.py`

 * *Files identical despite different names*

### Comparing `pycommons_lang-0.0.4/pycommons/lang/utils/stringutils.py` & `pycommons_lang-0.0.5/pycommons/lang/stringutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 
 from .arrayutils import ArrayUtils
 from .charutils import CharUtils
 
 
 class StringUtils(UtilityClass):
     """
-    The StringUtils `UtilityClass` that holds the utility methods for string observation,
-    manipulation, conversion etc. This class is inspired by the
-    [`StringUtils`](https://commons.apache.org/proper/commons-lang/apidocs/index.html)
-    class in the Apache Commons Lang package. Provides `None` safe methods to perform operations on
-    `str` object
+    The StringUtils holds the utility methods for string observation,
+    manipulation, conversion etc. This class is inspired by the `StringUtils`
+    class in the Apache Commons Lang package. Provides `None` safe methods
+    to perform operations on `str` object
 
     References:
-        https://commons.apache.org/proper/commons-lang/apidocs/index.html
+        https://commons.apache.org/proper/commons-lang/apidocs/org/apache/commons/lang3/StringUtils.html
     """
 
     EMPTY: str = ""
 
     @classmethod
     def abbreviate(
         cls,
@@ -326,11 +325,33 @@
                     tmp_length -= 1
                 return True
             return False
         return False
 
     @classmethod
     def to_character(cls, c: Optional[str]) -> Optional[Char]:
+        """
+        `None` safe conversion of a character to `pycommons.base.Character
+        Args:
+            c:
+
+        Returns:
+
+        """
         if cls.is_empty(c):
             return None
 
         return CharUtils.to_character(typing.cast(str, c)[0])
+
+    @classmethod
+    def default_string(cls, char_sequence: Optional[str], default_string: str = EMPTY) -> str:
+        """
+        Returns the default string if the passed string is `None`.
+
+        Args:
+            char_sequence: The string
+            default_string: Default string to be returned when `char_sequence` is None
+
+        Returns:
+            The `char_sequence` if it's not None, else the default string
+        """
+        return char_sequence if char_sequence is not None else default_string
```

### Comparing `pycommons_lang-0.0.4/pyproject.toml` & `pycommons_lang-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.lang"
-version = "0.0.4"
+version = "0.0.5"
 homepage = "https://github.com/shashankrnr32/pycommons-lang"
 description = "Python Commons Lang"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -21,15 +21,15 @@
     "LICENSE",
     "pycommons/py.typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 importlib_metadata = "*"
-pycommons-base = "0.0.5"
+pycommons-base = "0.0.6"
 
 [tool.poetry.dev-dependencies]
 mkdocs-material = ">7.0.0"
 mkdocstrings = { version = ">0.18", extras = ["python-legacy"] }
 mkdocs-awesome-pages-plugin = "*"
 markdown-include = "*"
 livereload = "*"
@@ -53,15 +53,15 @@
 disable = "C0103, C0116, C0114, C0115, R0801, R0903"
 max-public-methods = 50
 max-args = 8
 max-locals = 20
 min-public-method = 0
 
 [tool.pytest.ini_options]
-addopts = "--cov=pycommons --cov-branch --cov-report term-missing --cov-report xml -vv --color=yes --cov-fail-under 10"
+addopts = "--cov=pycommons --cov-branch --cov-report term-missing --cov-report xml -vv --color=yes --cov-fail-under 50"
 python_files = "tests.py test_*.py *_tests.py *Test.py"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy.overrides]
```

### Comparing `pycommons_lang-0.0.4/PKG-INFO` & `pycommons_lang-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycommons-lang
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Commons Lang
 Home-page: https://github.com/shashankrnr32/pycommons-lang
 License: Apache-2.0
 Author: Shashank Sharma
 Author-email: shashankrnr32@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: importlib_metadata
-Requires-Dist: pycommons-base (==0.0.5)
+Requires-Dist: pycommons-base (==0.0.6)
 Description-Content-Type: text/markdown
 
 # pycommons-lang
 
 [![PyPI](https://img.shields.io/pypi/v/pycommons-lang)](https://pypi.org/project/pycommons-lang/)
 ![versions](https://img.shields.io/pypi/pyversions/pycommons-lang.svg)
 ![PyPI - License](https://img.shields.io/pypi/l/pycommons-lang)
```

