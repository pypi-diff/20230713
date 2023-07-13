# Comparing `tmp/libhxl-5.0.1.tar.gz` & `tmp/libhxl-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libhxl-5.0.1.tar", last modified: Thu Jun  1 16:04:10 2023, max compression
+gzip compressed data, was "libhxl-5.0.2.tar", last modified: Thu Jul 13 14:34:34 2023, max compression
```

## Comparing `libhxl-5.0.1.tar` & `libhxl-5.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/
--rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:20:29.000000 libhxl-5.0.1/LICENSE.md
--rw-rw-r--   0 david     (1001) david     (1001)       28 2022-10-28 23:20:29.000000 libhxl-5.0.1/MANIFEST.in
--rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-06-01 16:04:10.749013 libhxl-5.0.1/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)     6000 2022-10-28 23:20:29.000000 libhxl-5.0.1/README.md
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/hxl/
--rw-rw-r--   0 david     (1001) david     (1001)     3641 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/__init__.py
--rw-rw-r--   0 david     (1001) david     (1001)     6595 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/converters.py
--rw-rw-r--   0 david     (1001) david     (1001)    13116 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/datatypes.py
--rw-rw-r--   0 david     (1001) david     (1001)   105695 2023-03-10 15:48:58.000000 libhxl-5.0.1/hxl/filters.py
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/hxl/formulas/
--rw-rw-r--   0 david     (1001) david     (1001)        0 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/formulas/__init__.py
--rw-rw-r--   0 david     (1001) david     (1001)      703 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/eval.py
--rw-rw-r--   0 david     (1001) david     (1001)    12791 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/formulas/functions.py
--rw-rw-r--   0 david     (1001) david     (1001)     1010 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/lexer.py
--rw-rw-r--   0 david     (1001) david     (1001)     1820 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/formulas/parser.py
--rw-rw-r--   0 david     (1001) david     (1001)     3919 2022-10-28 23:20:50.000000 libhxl-5.0.1/hxl/formulas/parsetab.py
--rw-rw-r--   0 david     (1001) david     (1001)     5788 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/geo.py
--rw-rw-r--   0 david     (1001) david     (1001)     1983 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/hxl-default-schema.json
--rw-rw-r--   0 david     (1001) david     (1001)    67060 2023-06-01 16:03:34.000000 libhxl-5.0.1/hxl/input.py
--rw-rw-r--   0 david     (1001) david     (1001)    51976 2023-03-10 15:35:47.000000 libhxl-5.0.1/hxl/model.py
--rw-rw-r--   0 david     (1001) david     (1001)    79626 2023-05-18 15:23:18.000000 libhxl-5.0.1/hxl/scripts.py
--rw-rw-r--   0 david     (1001) david     (1001)      605 2022-11-25 16:01:58.000000 libhxl-5.0.1/hxl/util.py
--rw-rw-r--   0 david     (1001) david     (1001)    62582 2022-10-28 23:20:29.000000 libhxl-5.0.1/hxl/validation.py
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:04:10.749013 libhxl-5.0.1/libhxl.egg-info/
--rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)      541 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1001) david     (1001)        1 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1001) david     (1001)      663 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1001) david     (1001)      118 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/requires.txt
--rw-rw-r--   0 david     (1001) david     (1001)        4 2023-06-01 16:04:10.000000 libhxl-5.0.1/libhxl.egg-info/top_level.txt
--rw-rw-r--   0 david     (1001) david     (1001)       38 2023-06-01 16:04:10.749013 libhxl-5.0.1/setup.cfg
--rwxrwxr-x   0 david     (1001) david     (1001)     2355 2023-06-01 16:03:34.000000 libhxl-5.0.1/setup.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-07-13 14:34:34.444733 libhxl-5.0.2/
+-rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:20:29.000000 libhxl-5.0.2/LICENSE.md
+-rw-rw-r--   0 david     (1001) david     (1001)       28 2022-10-28 23:20:29.000000 libhxl-5.0.2/MANIFEST.in
+-rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-07-13 14:34:34.444733 libhxl-5.0.2/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     6000 2022-10-28 23:20:29.000000 libhxl-5.0.2/README.md
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-07-13 14:34:34.440733 libhxl-5.0.2/hxl/
+-rw-rw-r--   0 david     (1001) david     (1001)     3641 2023-07-13 14:34:14.000000 libhxl-5.0.2/hxl/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)     6595 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/converters.py
+-rw-rw-r--   0 david     (1001) david     (1001)    13116 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/datatypes.py
+-rw-rw-r--   0 david     (1001) david     (1001)   105695 2023-06-20 16:07:05.000000 libhxl-5.0.2/hxl/filters.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-07-13 14:34:34.444733 libhxl-5.0.2/hxl/formulas/
+-rw-rw-r--   0 david     (1001) david     (1001)        0 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/formulas/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)      703 2022-11-25 16:01:58.000000 libhxl-5.0.2/hxl/formulas/eval.py
+-rw-rw-r--   0 david     (1001) david     (1001)    12791 2023-06-01 16:03:34.000000 libhxl-5.0.2/hxl/formulas/functions.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1010 2022-11-25 16:01:58.000000 libhxl-5.0.2/hxl/formulas/lexer.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1820 2022-11-25 16:01:58.000000 libhxl-5.0.2/hxl/formulas/parser.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3919 2022-10-28 23:20:50.000000 libhxl-5.0.2/hxl/formulas/parsetab.py
+-rw-rw-r--   0 david     (1001) david     (1001)     5788 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/geo.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1983 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/hxl-default-schema.json
+-rw-rw-r--   0 david     (1001) david     (1001)    67022 2023-07-13 14:34:14.000000 libhxl-5.0.2/hxl/input.py
+-rw-rw-r--   0 david     (1001) david     (1001)    51976 2023-03-10 15:35:47.000000 libhxl-5.0.2/hxl/model.py
+-rw-rw-r--   0 david     (1001) david     (1001)    79826 2023-07-13 14:34:14.000000 libhxl-5.0.2/hxl/scripts.py
+-rw-rw-r--   0 david     (1001) david     (1001)      605 2022-11-25 16:01:58.000000 libhxl-5.0.2/hxl/util.py
+-rw-rw-r--   0 david     (1001) david     (1001)    62582 2022-10-28 23:20:29.000000 libhxl-5.0.2/hxl/validation.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-07-13 14:34:34.444733 libhxl-5.0.2/libhxl.egg-info/
+-rw-rw-r--   0 david     (1001) david     (1001)     6634 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)      541 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        1 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      663 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      118 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/requires.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        4 2023-07-13 14:34:34.000000 libhxl-5.0.2/libhxl.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       38 2023-07-13 14:34:34.444733 libhxl-5.0.2/setup.cfg
+-rwxrwxr-x   0 david     (1001) david     (1001)     2355 2023-07-13 14:34:14.000000 libhxl-5.0.2/setup.py
```

### Comparing `libhxl-5.0.1/LICENSE.md` & `libhxl-5.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/PKG-INFO` & `libhxl-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libhxl
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python
 Home-page: http://hxlproject.org
 Author: David Megginson
 Author-email: megginson@un.org
 License: UNKNOWN
 Project-URL: Documentation, https://hxlstandard.github.io/libhxl-python/index.html
 Project-URL: GitHub, https://github.com/HXLStandard/libhxl-python/
```

### Comparing `libhxl-5.0.1/README.md` & `libhxl-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/__init__.py` & `libhxl-5.0.2/hxl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 """
 
 import sys
 
 if sys.version_info < (3,):
     raise RuntimeError("libhxl requires Python 3 or higher")
 
-__version__="5.0.1"
+__version__="5.0.2"
 """Module version number
 see https://www.python.org/dev/peps/pep-0396/
 """
 
 # Flatten out common items for easier access
 
 class HXLException(Exception):
```

### Comparing `libhxl-5.0.1/hxl/converters.py` & `libhxl-5.0.2/hxl/converters.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/datatypes.py` & `libhxl-5.0.2/hxl/datatypes.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/filters.py` & `libhxl-5.0.2/hxl/filters.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/formulas/eval.py` & `libhxl-5.0.2/hxl/formulas/eval.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/formulas/functions.py` & `libhxl-5.0.2/hxl/formulas/functions.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/formulas/lexer.py` & `libhxl-5.0.2/hxl/formulas/lexer.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/formulas/parser.py` & `libhxl-5.0.2/hxl/formulas/parser.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/formulas/parsetab.py` & `libhxl-5.0.2/hxl/formulas/parsetab.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/geo.py` & `libhxl-5.0.2/hxl/geo.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/hxl-default-schema.json` & `libhxl-5.0.2/hxl/hxl-default-schema.json`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/input.py` & `libhxl-5.0.2/hxl/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 ]
 
 CSV_FILE_EXTS = [
     'ssv',
     'csv',
     'tsv',
     'txt',
+    'hxl',
 ]
 
 CSV_MIME_TYPES = (
     'text/plain',
     'text/csv',
     'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
     'application/vnd.ms-excel',
@@ -1501,15 +1502,15 @@
             """
             columns = self.outer.columns
             values = self.outer._get_row()
             self.row_number += 1
             return hxl.model.Row(columns=columns, values=values, row_number=self.row_number, source_row_number=self.outer._source_row_number)
 
 
-def from_spec(spec, allow_local_ok=False):
+def from_spec(spec, input=None, allow_local_ok=False):
     """Build a full spec (including source) from a JSON-like data structure.
 
     The JSON spec can have the following top-level properties:
 
     - **input:** the source-data location (which is typically a URL or a nested JSON spec)
     - **allow_local:** if 1 (true), allow local filenames
     - **sheet_index:** the 0-based index of a sheet in an Excel workbook
@@ -1560,34 +1561,31 @@
     """
 
     if isinstance(spec, six.string_types):
         # a JSON string (parse it first)
         spec = json.loads(spec)
 
     # source
-    input_spec = spec.get('input')
+    input_spec = spec.get('input', None)
     allow_local = spec.get('allow_local', False) and allow_local_ok
     sheet_index = spec.get('sheet_index', None)
     timeout = spec.get('timeout', None)
     verify_ssl = spec.get('verify_ssl', True)
     http_headers = spec.get('http_headers', None)
     encoding = spec.get('encoding', None)
     expand_merged = spec.get('expand_merged', False)
     scan_ckan_resources = spec.get('scan_ckan_resources', False)
 
     # recipe
     tagger_spec = spec.get('tagger', None)
     recipe_spec = spec.get('recipe', [])
 
-    if not input_spec:
-        raise hxl.HXLException("No input property specified.")
-
     # set up the input
     input = make_input(
-        raw_source=input_spec,
+        raw_source=input if input else input_spec,
         input_options = InputOptions(
             allow_local=allow_local,
             sheet_index=sheet_index,
             timeout=timeout,
             verify_ssl=verify_ssl,
             http_headers=http_headers,
             encoding=encoding,
```

### Comparing `libhxl-5.0.1/hxl/model.py` & `libhxl-5.0.2/hxl/model.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/scripts.py` & `libhxl-5.0.2/hxl/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1889,23 +1889,30 @@
             response.raise_for_status()
             return response.json()
         else:
             with open(url_or_filename, "r") as input:
                 return json.load(input)
 
     parser = make_args('Process a HXL JSON spec')
+    parser.add_argument(
+        '-s',
+        '--spec',
+        help="JSON processing specification",
+        required=True,
+        metavar="spec.json",
+        type=get_json,
+    )
+
     args = parser.parse_args(args)
 
     do_common_args(args)
 
-    spec = get_json(args.infile)
-    source = hxl.input.from_spec(spec, allow_local_ok=True)
-
-    with make_output(args, stdout) as output:
-        hxl.input.write_hxl(output.output, source, show_tags=not args.strip_tags)
+    with make_input(args, stdin) as input, make_output(args, stdout) as output:
+        source = hxl.input.from_spec(args.spec, input=input, allow_local_ok=True)
+        hxl.input.write_hxl(output, source, show_tags=not args.strip_tags)
 
 
 def hxltag_main(args, stdin=STDIN, stdout=sys.stdout, stderr=sys.stderr):
     """
     Run hxltag with command-line arguments.
 
     Add tags to a non-HXLated file (accepts non-HXL input).
```

### Comparing `libhxl-5.0.1/hxl/util.py` & `libhxl-5.0.2/hxl/util.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/hxl/validation.py` & `libhxl-5.0.2/hxl/validation.py`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/libhxl.egg-info/PKG-INFO` & `libhxl-5.0.2/libhxl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libhxl
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python
 Home-page: http://hxlproject.org
 Author: David Megginson
 Author-email: megginson@un.org
 License: UNKNOWN
 Project-URL: Documentation, https://hxlstandard.github.io/libhxl-python/index.html
 Project-URL: GitHub, https://github.com/HXLStandard/libhxl-python/
```

### Comparing `libhxl-5.0.1/libhxl.egg-info/SOURCES.txt` & `libhxl-5.0.2/libhxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/libhxl.egg-info/entry_points.txt` & `libhxl-5.0.2/libhxl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `libhxl-5.0.1/setup.py` & `libhxl-5.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     raise RuntimeError("libhxl requires Python 3 or higher")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='libhxl',
-    version="5.0.1",
+    version="5.0.2",
     description='Python support library for the Humanitarian Exchange Language (HXL). See http://hxlstandard.org and https://github.com/HXLStandard/libhxl-python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Documentation': 'https://hxlstandard.github.io/libhxl-python/index.html',
         'GitHub': 'https://github.com/HXLStandard/libhxl-python/',
         'Changelog': 'https://github.com/HXLStandard/libhxl-python/blob/prod/CHANGELOG',
```

