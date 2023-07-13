# Comparing `tmp/py3seed-0.1.1.tar.gz` & `tmp/py3seed-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.1.1.tar", last modified: Tue Jul 11 02:54:02 2023, max compression
+gzip compressed data, was "py3seed-0.1.2.tar", last modified: Thu Jul 13 03:24:38 2023, max compression
```

## Comparing `py3seed-0.1.1.tar` & `py3seed-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.523413 py3seed-0.1.1/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.1/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-11 02:54:02.523547 py3seed-0.1.1/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.1/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.1/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-11 02:54:02.524201 py3seed-0.1.1/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.1/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.499305 py3seed-0.1.1/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.514749 py3seed-0.1.1/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.1/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.1/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.1/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.1/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.518930 py3seed-0.1.1/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.1/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20310 2023-07-11 02:45:05.000000 py3seed-0.1.1/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.1/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.1/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.1/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.1/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57499 2023-07-10 03:52:03.000000 py3seed-0.1.1/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.1/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14529 2023-07-11 02:00:45.000000 py3seed-0.1.1/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.1/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.517989 py3seed-0.1.1/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-11 02:54:02.000000 py3seed-0.1.1/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-11 02:54:02.522873 py3seed-0.1.1/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.1/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6093 2023-07-11 01:48:21.000000 py3seed-0.1.1/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.1/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.1/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.1/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.708893 py3seed-0.1.2/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.2/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-13 03:24:38.709233 py3seed-0.1.2/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.2/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.2/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-13 03:24:38.710668 py3seed-0.1.2/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.2/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.683329 py3seed-0.1.2/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.698010 py3seed-0.1.2/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.2/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.2/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.2/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.2/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.703729 py3seed-0.1.2/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.2/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20279 2023-07-13 03:08:33.000000 py3seed-0.1.2/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.2/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.2/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.2/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.2/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.2/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.2/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14437 2023-07-13 03:03:17.000000 py3seed-0.1.2/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.2/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.702476 py3seed-0.1.2/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.707848 py3seed-0.1.2/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.2/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6126 2023-07-13 03:08:09.000000 py3seed-0.1.2/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.2/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.2/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.2/tests/test_mongosupport.py
```

### Comparing `py3seed-0.1.1/LICENSE` & `py3seed-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/PKG-INFO` & `py3seed-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.1/setup.cfg` & `py3seed-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.1.1
+version = 0.1.2
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.1.1/src/py3seed/__init__.py` & `py3seed-0.1.2/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/__main__.py` & `py3seed-0.1.2/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/admin.py` & `py3seed-0.1.2/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/cachesupport.py` & `py3seed-0.1.2/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/commands/gen.py` & `py3seed-0.1.2/src/py3seed/commands/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 return f
         # If no matching, return nothing
         return None
 
     def parse_layout_fields(schema, action):
         """ Parse layout fields.
 
-        each column in layout can be blank('')/hyphen(-)/summary($)/group(number)/field(string)/inner fields(has children) suffixed with query and span string
+        each column in layout can be blank('')/hyphen(-)/group(integer&float)/field(string) suffixed with query and span string
         this function will return a list of field names.
         """
         return list(iterate_layout(schema[action], schema['groups']))
 
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
     env.globals['match_field'] = match_field
```

### Comparing `py3seed-0.1.1/src/py3seed/error.py` & `py3seed-0.1.2/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/inflection.py` & `py3seed-0.1.2/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/log.py` & `py3seed-0.1.2/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/merge3.py` & `py3seed-0.1.2/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/model.py` & `py3seed-0.1.2/src/py3seed/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,30 +104,30 @@
     """ Parent class for simple enum fields. """
     pass
 
 
 class Format(SimpleEnum):
     """ Predefined available formats, which should be used to control ui or api generation.
 
-    Below values are the same with OAS 3.0
-    https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#data-types
-    https://swagger.io/docs/specification/data-models/data-types/
+    NOTE: Name of format can NOT end with interger, as #FormatInteger has special meaning in view layout, e.g, '#summary4' means with summary format and 4 span
     """
+    # Below values are the same with OAS 3.0
+    # - https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#data-types
+    # - https://swagger.io/docs/specification/data-models/data-types/
     DATETIME = 'datetime'  # Default format for datetime
     DATE = 'date'
     PASSWORD = 'password'
     BYTE = 'byte'
     # Below values are self-defined
     TEXT = 'text'  # Default format for str
     INT = 'int'  # Default format for int
     FLOAT = 'float'  # Default format for float
     SELECT = 'select'  # Default format for SimpleEnum
     BUTTONGROUP = 'buttongroup'
     TAG = 'tag'  # Tag input
-    PASSWORD = 'password'
     TEXTAREA = 'textarea'
     RTE = 'rte'
     MARKDOWN = 'markdown'
     IMAGE = 'image'  # Image upload support
     AVATAR = 'avatar'  # User avatar
     FILE = 'file'  # File upload support
     VIDEO = 'video'  # Video upload support
@@ -137,14 +137,15 @@
     SWITCH = 'switch'
     HIDDEN = 'hidden'  # Hidden input
     LINK = 'link'  # Text input with an extenral link
     TIME = 'time'  # Time picker
     METRIC = 'metric'  # Statistic card for simple or object
     RANGE = 'range'  # Range picker
     # Below values are used for inner model/dict or list of model/dict
+    SUMMARY = 'summary'  # Summary of a object, i.e, {}
     TAB = 'tab'  # Objects with tabs nav, i.e, [{}]
     TABLE = 'table'  # Objects in table, i.e, [{}]
     MODAL = 'modal'  # Objects with some fields in table and all fields in modal, i.e, [{}]
     GRID = 'grid'  # Objects in grid, i.e, [{}]
     TIMELINE = 'timeline'  # Objects in timeline, i.e, [{}]
     CALENDAR = 'calendar'  # Objects in calendar, i.e, [{}]
     MEDIA = 'media'  # Objects in media components like blog comments, tweets and the like, i.e, [{}]
```

### Comparing `py3seed-0.1.1/src/py3seed/mongosupport.py` & `py3seed-0.1.2/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed/utils.py` & `py3seed-0.1.2/src/py3seed/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             'name_title': name_title,  # => Sample Model
             'name_title_lower': name_title.lower(),  # => sample model
             'name_title_lower_plural': inflection.pluralize(name_title.lower()),  # => sample models
         }
 
 
 # Match span
-SPAN_REGEX = re.compile(r'^(.*)#([0-9]+)$')
+SPAN_REGEX = re.compile(r'^(.*)#([a-zA-Z_-]*)([0-9]+)$')
 
 
 def parse_layout(body, schema):
     """ Parse layout defined in a model action.
     e.g,
     'demo/user-profile': {              # action name
         'domains': ['www'],             # domains that this action is available
@@ -148,19 +148,16 @@
                 col_name = column['name']
                 # Blank column
                 if not col_name:
                     pass
                 # Hyphen column
                 elif col_name == '-':
                     pass
-                # Summary column
-                elif col_name == '$':
-                    pass
-                # Group column
-                elif col_name.isdigit():
+                # Group column, e.g, 1, 1.1, 1.2, 2, 2.1
+                elif col_name.replace('.', '').isdigit():
                     pass
                 else:
                     keys = _schema['properties'].keys()  # type of _schema is always a object
                     if col_name not in keys:
                         raise LayoutError(f'Field {col_name} not found in schema')
             # Has inner layout
             if len(segment) > 1:
@@ -182,16 +179,15 @@
                         continue
                     #
                     logger.debug(f'{leading} Column ({i},{j}): {col_name}\n' + '\n'.join(col_lines))
                     #
                     # Column name possible values:
                     # 1) blank column prints only a placeholder
                     # 2) hyphen(-) prints line separator, i.e, <hr/>
-                    # 3) group column(digit) combines multiple columns
-                    # 4) summary column($) prints model's summary
+                    # 3) group column(integer/float) combines multiple columns
                     #
                     # While schema is a subset of Object Schema from OAS 3.0,
                     # In order to keep all the things simple, we do not use complex keywords such as oneOf, patternProperties, additionalProperties, etc.
                     # - https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#schemaObject
                     # - https://swagger.io/docs/specification/data-models/
                     # e.g,
                     # _schema = {
@@ -221,19 +217,16 @@
                     # }
                     # Blank column
                     if not col_name:
                         pass
                     # Hyphen column
                     elif col_name == '-':
                         pass
-                    # Summary column
-                    elif col_name == '$':
-                        column['rows'] = _parse_lines(level + 1, col_lines, _schema)
                     # Group column
-                    elif col_name.isdigit():
+                    elif col_name.replace('.', '').isdigit():
                         column['rows'] = _parse_lines(level + 1, col_lines, _schema)
                     else:
                         inner_schema = _schema['properties'][col_name]
                         inner_type = inner_schema['type']
                         if inner_type in ['object', 'array']:
                             if not col_lines:
                                 raise LayoutError(f'Field {col_name} should have layout')
@@ -248,23 +241,26 @@
 
     def _parse_column(column_str):
         """ Parse column string, having params and span, e.g, a?param=1#4. """
         column_str = column_str.strip()
         ret = {
             'raw': column_str,
         }
-        # Parse span at the end, e.g, a?param=1#4
+        # Parse span at the end, e.g, a?param=1#summary4
         span_match = SPAN_REGEX.match(column_str)
         if span_match:
             column_str = span_match.group(1)
-            ret.update({'span': int(span_match.group(2))})
+            if span_match.group(2):
+                ret.update({'format': span_match.group(2)})  # -> summary
+            #
+            ret.update({'span': int(span_match.group(3))})  # -> 4
         # Parse params, e.g, a?param=1#4
         if '?' in column_str:
-            column_str, params = _parse_query_str(column_str)
-            ret.update({'params': params})
+            column_str, column_params = _parse_query_str(column_str)
+            ret.update({'params': column_params})
         #
         ret.update({'name': column_str})
         #
         return ret
 
     def _parse_query_str(_query_str):
         """ Parse query string. """
```

### Comparing `py3seed-0.1.1/src/py3seed/websupport.py` & `py3seed-0.1.2/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.2/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.1/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.1.2/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/tests/test_cachesupport.py` & `py3seed-0.1.2/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/tests/test_gen.py` & `py3seed-0.1.2/tests/test_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from .core.models import User, Team
 
 
 def test_layout_parsing():
     """ Test layout parsing. """
     # User profile
     user_profile_layout = '''#!form?title=User
-        $#4,           0#8                                           
-          avatar         name  
-          name           phone                                                  
-          status         intro                                                 
-          roles          avatar                                                
+        1#summary4,  2#8                                           
+          avatar       name  
+          name         phone                                                  
+          status       intro                                                 
+          roles        avatar                                                
           email
           phone
           create_time
     '''
     user_schema = User.schema()
     # Team members
     team_members_layout = '''#!read?title=Members
-        $#4,           members#8                                                  
-          logo           avatar, name, status, roles, email, phone, team_join_time
+        1#summary4,  members#8                                                  
+          logo         avatar, name, status, roles, email, phone, team_join_time
           name
           phone                                                              
           members                                                                 
           create_time
     '''
     team_schema = Team.schema()
 
@@ -78,15 +78,16 @@
 
     # User profile layout
     layout = parse_layout(user_profile_layout, user_schema)
     assert layout['action'] == 'form'
     assert layout['params']['title'] == 'User'
     assert len(layout['rows']) == 1
     first_row = layout['rows'][0]
-    assert first_row[0]['name'] == '$'
+    assert first_row[0]['name'] == '1'
+    assert first_row[0]['format'] == 'summary'
     assert first_row[0]['span'] == 4
     assert len(first_row[0]['rows']) == 7
     assert first_row[0]['rows'][0][0]['name'] == 'avatar'
     assert len(first_row[1]['rows']) == 4
     assert first_row[1]['rows'][1][0]['name'] == 'phone'
 
     # Team member layout
@@ -113,15 +114,15 @@
 <head>
     <title>Members</title>
 </head>
 <body>
     <h1 class="base">Members</h1>
     <h2>read</h2>
     <div class="row">
-        <div class="column">$</div>
+        <div class="column">1</div>
         <div class="column">members</div>
     </div>
 </body>
 </html>'''
     #
     with open('www/templates/public/team-members.html.1', 'w', encoding='utf-8') as f:
         f.write(base)
@@ -130,15 +131,15 @@
 <head>
     <title>Members</title>
 </head>
 <body>
     <h1 class="this">Members</h1>
     <h2>read</h2>
     <div class="row">
-        <div class="column">$</div>
+        <div class="column">1</div>
         <div class="column">members</div>
     </div>
 </body>
 </html>'''
     with open('www/templates/public/team-members.html', 'w', encoding='utf-8') as f:
         f.write(this)
     #
@@ -174,16 +175,16 @@
 <head>
     <title>User</title>
 </head>
 <body>
     <h1 class="page-header">User</h1>
     <h2>form</h2>
     <div class="row">
-        <div class="column">$</div>
-        <div class="column">0</div>
+        <div class="column">1</div>
+        <div class="column">2</div>
     </div>
 </body>
 </html>'''
     # team-members.html should be 3-way merged with conflicts
     team_members_html = open('www/templates/public/team-members.html', encoding='utf-8').read()
     assert team_members_html == '''<html>
 <head>
@@ -193,15 +194,15 @@
 <<<<<<< OTHER
     <h1>Members</h1>
 =======
     <h1 class="this">Members</h1>
 >>>>>>> THIS
     <h2>read</h2>
     <div class="row">
-        <div class="column">$</div>
+        <div class="column">1</div>
         <div class="column">members</div>
     </div>
 </body>
 </html>'''
     # enum.js should be rendered every time
     enums_js = open('www/static/js/enums.js', encoding='utf-8').read()
     assert enums_js == '''//
```

### Comparing `py3seed-0.1.1/tests/test_merge3.py` & `py3seed-0.1.2/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/tests/test_model.py` & `py3seed-0.1.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.1/tests/test_mongosupport.py` & `py3seed-0.1.2/tests/test_mongosupport.py`

 * *Files identical despite different names*

