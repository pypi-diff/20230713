# Comparing `tmp/jsonmerge-1.9.0.tar.gz` & `tmp/jsonmerge-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonmerge-1.9.0.tar", last modified: Wed Nov  2 06:32:46 2022, max compression
+gzip compressed data, was "dist/jsonmerge-1.9.1.tar", last modified: Thu Jul 13 09:37:37 2023, max compression
```

## Comparing `jsonmerge-1.9.0.tar` & `jsonmerge-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/
--rw-r--r--   0 avian     (1000) avian     (1000)     3902 2022-11-02 06:27:25.000000 jsonmerge-1.9.0/ChangeLog
--rw-r--r--   0 avian     (1000) avian     (1000)     1098 2022-10-22 14:31:04.000000 jsonmerge-1.9.0/LICENSE
--rw-r--r--   0 avian     (1000) avian     (1000)       82 2018-01-31 17:33:19.000000 jsonmerge-1.9.0/MANIFEST.in
--rw-r--r--   0 avian     (1000) avian     (1000)    23753 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/PKG-INFO
--rw-r--r--   0 avian     (1000) avian     (1000)    19312 2022-10-22 15:59:38.000000 jsonmerge-1.9.0/README.rst
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge/
--rw-r--r--   0 avian     (1000) avian     (1000)    13486 2022-11-01 08:55:31.000000 jsonmerge-1.9.0/jsonmerge/__init__.py
--rw-r--r--   0 avian     (1000) avian     (1000)     4217 2022-11-01 08:47:21.000000 jsonmerge-1.9.0/jsonmerge/descenders.py
--rw-r--r--   0 avian     (1000) avian     (1000)      566 2019-07-19 14:32:45.000000 jsonmerge-1.9.0/jsonmerge/exceptions.py
--rw-r--r--   0 avian     (1000) avian     (1000)     2012 2022-10-22 15:10:14.000000 jsonmerge-1.9.0/jsonmerge/jsonvalue.py
--rw-r--r--   0 avian     (1000) avian     (1000)      810 2022-10-22 14:31:04.000000 jsonmerge-1.9.0/jsonmerge/resolver.py
--rw-r--r--   0 avian     (1000) avian     (1000)    12662 2022-10-22 15:58:03.000000 jsonmerge-1.9.0/jsonmerge/strategies.py
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge.egg-info/
--rw-r--r--   0 avian     (1000) avian     (1000)    23753 2022-11-02 06:32:45.000000 jsonmerge-1.9.0/jsonmerge.egg-info/PKG-INFO
--rw-r--r--   0 avian     (1000) avian     (1000)      439 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge.egg-info/SOURCES.txt
--rw-r--r--   0 avian     (1000) avian     (1000)        1 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge.egg-info/dependency_links.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       17 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge.egg-info/requires.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       10 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/jsonmerge.egg-info/top_level.txt
--rw-r--r--   0 avian     (1000) avian     (1000)       38 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/setup.cfg
--rw-r--r--   0 avian     (1000) avian     (1000)      684 2022-11-02 06:28:02.000000 jsonmerge-1.9.0/setup.py
-drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2022-11-02 06:32:46.000000 jsonmerge-1.9.0/tests/
--rw-r--r--   0 avian     (1000) avian     (1000)        0 2018-01-31 17:33:19.000000 jsonmerge-1.9.0/tests/__init__.py
--rw-r--r--   0 avian     (1000) avian     (1000)    72698 2022-11-01 08:55:37.000000 jsonmerge-1.9.0/tests/test_jsonmerge.py
--rw-r--r--   0 avian     (1000) avian     (1000)     2652 2022-10-22 15:09:10.000000 jsonmerge-1.9.0/tests/test_jsonvalue.py
--rw-r--r--   0 avian     (1000) avian     (1000)      131 2020-09-24 17:13:51.000000 jsonmerge-1.9.0/tests/test_readme.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/
+-rw-r--r--   0 avian     (1000) avian     (1000)     4037 2023-07-13 09:32:02.000000 jsonmerge-1.9.1/ChangeLog
+-rw-r--r--   0 avian     (1000) avian     (1000)     1098 2022-10-22 14:31:04.000000 jsonmerge-1.9.1/LICENSE
+-rw-r--r--   0 avian     (1000) avian     (1000)       82 2018-01-31 17:33:19.000000 jsonmerge-1.9.1/MANIFEST.in
+-rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/PKG-INFO
+-rw-r--r--   0 avian     (1000) avian     (1000)    21373 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/README.rst
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge/
+-rw-r--r--   0 avian     (1000) avian     (1000)    13486 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/jsonmerge/__init__.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     4217 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/jsonmerge/descenders.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      566 2019-07-19 14:32:45.000000 jsonmerge-1.9.1/jsonmerge/exceptions.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     2012 2022-10-22 15:10:14.000000 jsonmerge-1.9.1/jsonmerge/jsonvalue.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      810 2022-10-22 14:31:04.000000 jsonmerge-1.9.1/jsonmerge/resolver.py
+-rw-r--r--   0 avian     (1000) avian     (1000)    12662 2022-10-22 15:58:03.000000 jsonmerge-1.9.1/jsonmerge/strategies.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge.egg-info/
+-rw-r--r--   0 avian     (1000) avian     (1000)    26190 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/PKG-INFO
+-rw-r--r--   0 avian     (1000) avian     (1000)      439 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/jsonmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)        1 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       26 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/requires.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       10 2023-07-13 09:37:36.000000 jsonmerge-1.9.1/jsonmerge.egg-info/top_level.txt
+-rw-r--r--   0 avian     (1000) avian     (1000)       38 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/setup.cfg
+-rw-r--r--   0 avian     (1000) avian     (1000)      693 2023-07-13 09:32:06.000000 jsonmerge-1.9.1/setup.py
+drwxr-sr-x   0 avian     (1000) avian     (1000)        0 2023-07-13 09:37:37.000000 jsonmerge-1.9.1/tests/
+-rw-r--r--   0 avian     (1000) avian     (1000)        0 2018-01-31 17:33:19.000000 jsonmerge-1.9.1/tests/__init__.py
+-rw-r--r--   0 avian     (1000) avian     (1000)    72698 2022-11-21 14:40:26.000000 jsonmerge-1.9.1/tests/test_jsonmerge.py
+-rw-r--r--   0 avian     (1000) avian     (1000)     2652 2022-10-22 15:09:10.000000 jsonmerge-1.9.1/tests/test_jsonvalue.py
+-rw-r--r--   0 avian     (1000) avian     (1000)      131 2020-09-24 17:13:51.000000 jsonmerge-1.9.1/tests/test_readme.py
```

### Comparing `jsonmerge-1.9.0/ChangeLog` & `jsonmerge-1.9.1/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-13	jsonmerge	1.9.1
+	* Require jsonschema 4.17.3 or earlier since some tests currently fail
+	  with 4.18.0 and later releases.
+
 2022-11-02	jsonmerge	1.9.0
 
 	* Add sortByRef and sortReverse options for the append and
 	  arrayMergeById strategies.
 	* Fix failing tests with jsonschema>=4.15.0.
 	* Fix warning about iter_errors use that was deprecated around
 	  jsonschema 4.10.1.
```

### Comparing `jsonmerge-1.9.0/LICENSE` & `jsonmerge-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/PKG-INFO` & `jsonmerge-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jsonmerge
-Version: 1.9.0
+Version: 1.9.1
 Summary: Merge a series of JSON documents.
 Home-page: UNKNOWN
 Author: Tomaz Solc
 Author-email: tomaz.solc@tablix.org
 License: MIT
 Description: Merge a series of JSON documents
         ================================
@@ -440,31 +440,77 @@
             pip install .
         
         *jsonmerge* uses `Tox`_ for testing. To run the test suite run::
         
             tox
         
         
+        Troubleshooting
+        ---------------
+        
+        The most common problem with *jsonmerge* is getting unexpected results from
+        a merge. Finding the exact reason why *jsonmerge* produced a particular
+        result can be complicated, especially when head and base structures are
+        very large. Most often the cause is a problem with either the schema or
+        head and base that is passed to *jsonmerge*, not a bug in *jsonmerge*
+        itself.
+        
+        Here are some tips for debugging issues with *jsonmerge*:
+        
+        * Try to minimize the problem. Prune branches of head and base structures
+          that are not relevant to your issue and re-run the merge. Often just
+          getting a clearer view of the relevant parts exposes the problem.
+        
+        * *jsonmerge* uses the standard `logging`_ Python module to print out what
+          it is doing during the merge. You need to increase verbosity to DEBUG
+          level to see the messages.
+        
+        * A very common mistake is misunderstanding which part of the schema
+          applies to which part of the head and base structures. Debug logs
+          mentioned in the previous point can be very helpful with that, since they
+          show how merge descends into hierarchies of all involved structures and
+          when a default strategy is used.
+        
+        * With large head and base it's common that parts of them are not what you
+          think they are. Validate your inputs against your schema using the
+          *jsonschema* library before passing them onto *jsonmerge*. Make sure your
+          schema is restrictive enough.
+        
+        * Pay special attention to parts of the schema that use *oneOf*, *anyOf*,
+          *allOf* keywords. These can sometimes validate in unexpected ways.
+        
+        * Another problem point can be *$ref* pointers if they can cause recursion.
+          Using recursive schemas with *jsonmerge* is fine, but they can often
+          product unexpected results.
+        
+        
         Reporting bugs and contributing code
         ------------------------------------
         
         Thank you for contributing to *jsonmerge*! Free software wouldn't be
         possible without contributions from users like you. However, please consider
         that I maintain this project in my free time. Hence I ask you to follow
         this simple etiquette to minimize the amount of effort needed to include
         your contribution.
         
-        Please use `GitHub issues`_ to report bugs. Make sure that your report
-        includes:
+        Please use `GitHub issues`_ to report bugs.
+        
+        Before reporting the bug, please make sure that:
+        
+        * You've read this entire README file.
+        * You've read the Troubleshooting section of the README file.
+        * You've looked at existing issues if the bug has already been reported.
+        
+        Make sure that your report includes:
         
         * A *minimal*, but complete, code example that reproduces the problem,
           including any JSON data required to run it. It should be something I can
           copy-paste into a .py file and run.
-        * Relevant version of *jsonmerge* - either release number on PyPi or git
-          commit hash.
+        * Relevant versions of *jsonmerge* and *jsonschema* - either release number
+          on PyPi or the git commit hash.
         * Copy of the traceback, in case you are reporting an unhandled exception.
         * Example of what you think should be the correct output, in case you are
           reporting wrong result of a merge or schema generation.
         
         Please use `GitHub pull requests`_ to contribute code. Make sure that your
         pull request:
         
@@ -498,14 +544,15 @@
         THE SOFTWARE.
         
         .. _JSON schema: http://json-schema.org
         .. _Draft 4: http://json-schema.org/specification-links.html#draft-4
         .. _Tox: https://tox.readthedocs.io/en/latest/
         .. _GitHub issues: https://github.com/avian2/jsonmerge/issues
         .. _GitHub pull requests: https://github.com/avian2/jsonmerge/pulls
+        .. _logging: https://docs.python.org/3/library/logging.html
         
         ..
             vim: tw=75 ts=4 sw=4 expandtab softtabstop=4
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `jsonmerge-1.9.0/README.rst` & `jsonmerge-1.9.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -432,31 +432,77 @@
     pip install .
 
 *jsonmerge* uses `Tox`_ for testing. To run the test suite run::
 
     tox
 
 
+Troubleshooting
+---------------
+
+The most common problem with *jsonmerge* is getting unexpected results from
+a merge. Finding the exact reason why *jsonmerge* produced a particular
+result can be complicated, especially when head and base structures are
+very large. Most often the cause is a problem with either the schema or
+head and base that is passed to *jsonmerge*, not a bug in *jsonmerge*
+itself.
+
+Here are some tips for debugging issues with *jsonmerge*:
+
+* Try to minimize the problem. Prune branches of head and base structures
+  that are not relevant to your issue and re-run the merge. Often just
+  getting a clearer view of the relevant parts exposes the problem.
+
+* *jsonmerge* uses the standard `logging`_ Python module to print out what
+  it is doing during the merge. You need to increase verbosity to DEBUG
+  level to see the messages.
+
+* A very common mistake is misunderstanding which part of the schema
+  applies to which part of the head and base structures. Debug logs
+  mentioned in the previous point can be very helpful with that, since they
+  show how merge descends into hierarchies of all involved structures and
+  when a default strategy is used.
+
+* With large head and base it's common that parts of them are not what you
+  think they are. Validate your inputs against your schema using the
+  *jsonschema* library before passing them onto *jsonmerge*. Make sure your
+  schema is restrictive enough.
+
+* Pay special attention to parts of the schema that use *oneOf*, *anyOf*,
+  *allOf* keywords. These can sometimes validate in unexpected ways.
+
+* Another problem point can be *$ref* pointers if they can cause recursion.
+  Using recursive schemas with *jsonmerge* is fine, but they can often
+  product unexpected results.
+
+
 Reporting bugs and contributing code
 ------------------------------------
 
 Thank you for contributing to *jsonmerge*! Free software wouldn't be
 possible without contributions from users like you. However, please consider
 that I maintain this project in my free time. Hence I ask you to follow
 this simple etiquette to minimize the amount of effort needed to include
 your contribution.
 
-Please use `GitHub issues`_ to report bugs. Make sure that your report
-includes:
+Please use `GitHub issues`_ to report bugs.
+
+Before reporting the bug, please make sure that:
+
+* You've read this entire README file.
+* You've read the Troubleshooting section of the README file.
+* You've looked at existing issues if the bug has already been reported.
+
+Make sure that your report includes:
 
 * A *minimal*, but complete, code example that reproduces the problem,
   including any JSON data required to run it. It should be something I can
   copy-paste into a .py file and run.
-* Relevant version of *jsonmerge* - either release number on PyPi or git
-  commit hash.
+* Relevant versions of *jsonmerge* and *jsonschema* - either release number
+  on PyPi or the git commit hash.
 * Copy of the traceback, in case you are reporting an unhandled exception.
 * Example of what you think should be the correct output, in case you are
   reporting wrong result of a merge or schema generation.
 
 Please use `GitHub pull requests`_ to contribute code. Make sure that your
 pull request:
 
@@ -490,10 +536,11 @@
 THE SOFTWARE.
 
 .. _JSON schema: http://json-schema.org
 .. _Draft 4: http://json-schema.org/specification-links.html#draft-4
 .. _Tox: https://tox.readthedocs.io/en/latest/
 .. _GitHub issues: https://github.com/avian2/jsonmerge/issues
 .. _GitHub pull requests: https://github.com/avian2/jsonmerge/pulls
+.. _logging: https://docs.python.org/3/library/logging.html
 
 ..
     vim: tw=75 ts=4 sw=4 expandtab softtabstop=4
```

### Comparing `jsonmerge-1.9.0/jsonmerge/__init__.py` & `jsonmerge-1.9.1/jsonmerge/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge/descenders.py` & `jsonmerge-1.9.1/jsonmerge/descenders.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge/exceptions.py` & `jsonmerge-1.9.1/jsonmerge/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge/jsonvalue.py` & `jsonmerge-1.9.1/jsonmerge/jsonvalue.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge/resolver.py` & `jsonmerge-1.9.1/jsonmerge/resolver.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge/strategies.py` & `jsonmerge-1.9.1/jsonmerge/strategies.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/jsonmerge.egg-info/PKG-INFO` & `jsonmerge-1.9.1/jsonmerge.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jsonmerge
-Version: 1.9.0
+Version: 1.9.1
 Summary: Merge a series of JSON documents.
 Home-page: UNKNOWN
 Author: Tomaz Solc
 Author-email: tomaz.solc@tablix.org
 License: MIT
 Description: Merge a series of JSON documents
         ================================
@@ -440,31 +440,77 @@
             pip install .
         
         *jsonmerge* uses `Tox`_ for testing. To run the test suite run::
         
             tox
         
         
+        Troubleshooting
+        ---------------
+        
+        The most common problem with *jsonmerge* is getting unexpected results from
+        a merge. Finding the exact reason why *jsonmerge* produced a particular
+        result can be complicated, especially when head and base structures are
+        very large. Most often the cause is a problem with either the schema or
+        head and base that is passed to *jsonmerge*, not a bug in *jsonmerge*
+        itself.
+        
+        Here are some tips for debugging issues with *jsonmerge*:
+        
+        * Try to minimize the problem. Prune branches of head and base structures
+          that are not relevant to your issue and re-run the merge. Often just
+          getting a clearer view of the relevant parts exposes the problem.
+        
+        * *jsonmerge* uses the standard `logging`_ Python module to print out what
+          it is doing during the merge. You need to increase verbosity to DEBUG
+          level to see the messages.
+        
+        * A very common mistake is misunderstanding which part of the schema
+          applies to which part of the head and base structures. Debug logs
+          mentioned in the previous point can be very helpful with that, since they
+          show how merge descends into hierarchies of all involved structures and
+          when a default strategy is used.
+        
+        * With large head and base it's common that parts of them are not what you
+          think they are. Validate your inputs against your schema using the
+          *jsonschema* library before passing them onto *jsonmerge*. Make sure your
+          schema is restrictive enough.
+        
+        * Pay special attention to parts of the schema that use *oneOf*, *anyOf*,
+          *allOf* keywords. These can sometimes validate in unexpected ways.
+        
+        * Another problem point can be *$ref* pointers if they can cause recursion.
+          Using recursive schemas with *jsonmerge* is fine, but they can often
+          product unexpected results.
+        
+        
         Reporting bugs and contributing code
         ------------------------------------
         
         Thank you for contributing to *jsonmerge*! Free software wouldn't be
         possible without contributions from users like you. However, please consider
         that I maintain this project in my free time. Hence I ask you to follow
         this simple etiquette to minimize the amount of effort needed to include
         your contribution.
         
-        Please use `GitHub issues`_ to report bugs. Make sure that your report
-        includes:
+        Please use `GitHub issues`_ to report bugs.
+        
+        Before reporting the bug, please make sure that:
+        
+        * You've read this entire README file.
+        * You've read the Troubleshooting section of the README file.
+        * You've looked at existing issues if the bug has already been reported.
+        
+        Make sure that your report includes:
         
         * A *minimal*, but complete, code example that reproduces the problem,
           including any JSON data required to run it. It should be something I can
           copy-paste into a .py file and run.
-        * Relevant version of *jsonmerge* - either release number on PyPi or git
-          commit hash.
+        * Relevant versions of *jsonmerge* and *jsonschema* - either release number
+          on PyPi or the git commit hash.
         * Copy of the traceback, in case you are reporting an unhandled exception.
         * Example of what you think should be the correct output, in case you are
           reporting wrong result of a merge or schema generation.
         
         Please use `GitHub pull requests`_ to contribute code. Make sure that your
         pull request:
         
@@ -498,14 +544,15 @@
         THE SOFTWARE.
         
         .. _JSON schema: http://json-schema.org
         .. _Draft 4: http://json-schema.org/specification-links.html#draft-4
         .. _Tox: https://tox.readthedocs.io/en/latest/
         .. _GitHub issues: https://github.com/avian2/jsonmerge/issues
         .. _GitHub pull requests: https://github.com/avian2/jsonmerge/pulls
+        .. _logging: https://docs.python.org/3/library/logging.html
         
         ..
             vim: tw=75 ts=4 sw=4 expandtab softtabstop=4
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `jsonmerge-1.9.0/setup.py` & `jsonmerge-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/python
 # vim:ts=4 sw=4 expandtab softtabstop=4
 
 from setuptools import setup
 
 setup(name='jsonmerge',
-    version='1.9.0',
+    version='1.9.1',
     description='Merge a series of JSON documents.',
     license='MIT',
     long_description=open("README.rst").read(),
     author='Tomaz Solc',
     author_email='tomaz.solc@tablix.org',
     packages = [ 'jsonmerge' ],
-    install_requires = [ 'jsonschema>2.4.0' ],
+    install_requires = [ 'jsonschema>2.4.0,<=4.17.3' ],
     test_suite = 'tests',
     classifiers = [
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
```

### Comparing `jsonmerge-1.9.0/tests/test_jsonmerge.py` & `jsonmerge-1.9.1/tests/test_jsonmerge.py`

 * *Files identical despite different names*

### Comparing `jsonmerge-1.9.0/tests/test_jsonvalue.py` & `jsonmerge-1.9.1/tests/test_jsonvalue.py`

 * *Files identical despite different names*

