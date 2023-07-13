# Comparing `tmp/efrem_utils-0.0.8.tar.gz` & `tmp/efrem_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.0.8.tar", max compression
+gzip compressed data, was "efrem_utils-0.0.9.tar", max compression
```

## Comparing `efrem_utils-0.0.8.tar` & `efrem_utils-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2193 2023-07-13 11:16:44.521483 efrem_utils-0.0.8/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0      361 2023-07-13 11:15:39.178764 efrem_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      191 2023-07-12 23:48:56.145597 efrem_utils-0.0.8/README.md
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 efrem_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2189 2023-07-13 15:07:11.403793 efrem_utils-0.0.9/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0      361 2023-07-13 15:08:13.495597 efrem_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      192 2023-07-13 15:06:47.791531 efrem_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 efrem_utils-0.0.9/PKG-INFO
```

### Comparing `efrem_utils-0.0.8/efrem_utils.py` & `efrem_utils-0.0.9/efrem_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable, TypeVar, Iterable
 
 T = TypeVar("T")
 W = TypeVar("W")
 
-def get_validated_input(msg: str | None = None, *, validators: Iterable[tuple[Callable[[T], bool], str | Callable[[T], str] | None]] | None = None, constructor: Callable[[T], W] = str, precomp: Callable[[str], T] | None = None) -> Callable[[], W]:
+def validated_input(msg: str | None = None, *, validators: Iterable[tuple[Callable[[T], bool], str | Callable[[T], str] | None]] | None = None, constructor: Callable[[T], W] = str, precomp: Callable[[str], T] | None = None) -> Callable[[], W]:
     """
     An attempt at abstracting the case of using input() repeatedly until it is valid;
     Returns a function (to use instead of input()), but the message is specified at the part of calling this function,
     not the function you get itself, mostly because the error messages in the validator argument should be related to the input message.
 
     When validators aren't specified, it uses the constructor as the validator. I.e, if you use constructor=int, the validator will check if the input is an integer.
```

### Comparing `efrem_utils-0.0.8/LICENSE` & `efrem_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.0.8/PKG-INFO` & `efrem_utils-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efrem-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Efrem's utilities
 Home-page: https://github.com/NikitaNightBot/efrem-utils
 Author: lone_druid
 Author-email: enikita332@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -13,8 +13,8 @@
 
 # `efrem-utils`
 
 A package with utility functions to abstract some logic. 
 
 ## `examples`
 
-Check: [`examples directory`](https://github.com/NikitaNightBot/EfremUtils/tree/main/examples)
+Check: [`examples directory`](https://github.com/NikitaNightBot/efrem-utils/tree/main/examples)
```

