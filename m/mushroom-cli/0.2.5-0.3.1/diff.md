# Comparing `tmp/mushroom_cli-0.2.5.tar.gz` & `tmp/mushroom_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mushroom_cli-0.2.5.tar", last modified: Tue Nov 22 02:19:02 2022, max compression
+gzip compressed data, was "mushroom_cli-0.3.1.tar", last modified: Thu Jul 13 03:10:55 2023, max compression
```

## Comparing `mushroom_cli-0.2.5.tar` & `mushroom_cli-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-22 02:19:02.054768 mushroom_cli-0.2.5/
--rw-rw-rw-   0        0        0      274 2022-11-22 02:19:02.055199 mushroom_cli-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6029 2022-09-14 07:29:06.000000 mushroom_cli-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2022-11-22 02:19:02.045921 mushroom_cli-0.2.5/mushroom/
--rw-rw-rw-   0        0        0      178 2022-11-16 08:57:07.000000 mushroom_cli-0.2.5/mushroom/__init__.py
--rw-rw-rw-   0        0        0     6595 2022-11-16 08:56:55.000000 mushroom_cli-0.2.5/mushroom/arg_builder.py
--rw-rw-rw-   0        0        0      998 2022-09-14 06:28:07.000000 mushroom_cli-0.2.5/mushroom/arg_textwrap.py
--rw-rw-rw-   0        0        0      973 2022-09-14 09:49:55.000000 mushroom_cli-0.2.5/mushroom/args_fetch.py
--rw-rw-rw-   0        0        0     1515 2022-09-14 10:09:56.000000 mushroom_cli-0.2.5/mushroom/core.py
--rw-rw-rw-   0        0        0     1827 2022-09-14 10:14:04.000000 mushroom_cli-0.2.5/mushroom/func_parser.py
-drwxrwxrwx   0        0        0        0 2022-11-22 02:19:02.053674 mushroom_cli-0.2.5/mushroom_cli.egg-info/
--rw-rw-rw-   0        0        0      274 2022-11-22 02:19:00.000000 mushroom_cli-0.2.5/mushroom_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2022-11-22 02:19:00.000000 mushroom_cli-0.2.5/mushroom_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-22 02:19:00.000000 mushroom_cli-0.2.5/mushroom_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-19 02:25:29.000000 mushroom_cli-0.2.5/mushroom_cli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-11-22 02:19:00.000000 mushroom_cli-0.2.5/mushroom_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-11-22 02:19:02.055921 mushroom_cli-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      352 2022-11-16 08:57:14.000000 mushroom_cli-0.2.5/setup.py
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1066 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/LICENSE.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/PKG-INFO
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     5786 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/README.md
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/mushroom/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      173 2023-07-13 03:08:06.000000 mushroom_cli-0.3.1/mushroom/__init__.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     6439 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_builder.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)       49 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_exceptions.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      969 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_textwrap.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1285 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/args_fetch.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1622 2023-07-13 02:16:32.000000 mushroom_cli-0.3.1/mushroom/core.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1788 2023-07-13 02:08:59.000000 mushroom_cli-0.3.1/mushroom/func_parser.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     3524 2023-07-13 03:01:10.000000 mushroom_cli-0.3.1/mushroom/traceback_module.py
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/mushroom_cli.egg-info/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/PKG-INFO
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      409 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-13 03:06:01.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/not-zip-safe
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        9 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/top_level.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)       79 2023-07-13 03:10:55.777349 mushroom_cli-0.3.1/setup.cfg
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      339 2023-07-13 03:08:00.000000 mushroom_cli-0.3.1/setup.py
```

### Comparing `mushroom_cli-0.2.5/mushroom/arg_builder.py` & `mushroom_cli-0.3.1/mushroom/arg_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-# build the argparse object according to the function
-import argparse
-import re
-import typing, types
-from collections import Counter
-from mushroom.arg_textwrap import RawDescriptionHelpFormatter as HelpFormatter
-import mushroom.args_fetch as args_fetch
-
-
-def build_blank_parser(func_name, func_doc=""):
-    """
-    No arguments, just return the parser object
-    :return: argparse object
-    """
-    if not func_doc:
-        func_doc = 'Function {} No arguments, run directly'.format(func_name)
-
-    parser = argparse.ArgumentParser(description=func_doc, formatter_class=HelpFormatter)
-    return parser
-
-
-def build_args_parser(func_vars, func_dtypes, func_default_vars, func_name, func_doc="", mode="number"):
-    """
-    Build a parser according to the function vars
-    : return: argparse object
-    """
-    if not func_doc:
-        func_doc = 'Function {} Arguments parser, if args are not given, it will be regarded as a string.'.format(func_name)
-
-    parser = argparse.ArgumentParser(description=func_doc, formatter_class=HelpFormatter)
-    abbr_names_mapper = args_abbreviate(func_vars, mode=mode)
-    helper_mapper = helper_builder_from_doc(func_doc=func_doc)
-    for var_name in func_vars:
-        argument_add(parser, var_name, func_dtypes.get(var_name, str), func_default_vars.get(var_name, None), abbr_names_mapper[var_name], helper=helper_mapper.get(var_name, ""))
-    return parser
-
-
-def build_class_init_method(class_):
-    """
-    """
-    args_cnt, func_varnames, args_dtypes, default_flags = args_fetch.args_status_fetch(class_.__init__, isClass=True)
-    help_text = "MAIN PROGRAM" if not class_.__doc__ else class_.__doc__
-    if args_cnt == 0:
-        parser = build_blank_parser(func_name="", func_doc=help_text)
-            
-    else:
-        parser = build_args_parser(func_varnames, args_dtypes, default_flags, func_name="", func_doc=help_text)
-
-    subparser = parser.add_subparsers(help='sub command')    
-    return parser, subparser
-
-
-def build_blank_sub_parser(func:types.FunctionType, main_parser):
-    """
-    Build a blank sub command function
-    function should be a instance method
-    : return : argparse object
-    """
-    help_text = "sub command:{}, run directly".format(func.__name__) if not func.__doc__ else func.__doc__
-    sub_parser = main_parser.add_parser(func.__name__, help=help_text)
-    sub_parser.set_defaults(func=func)
-    return main_parser
-
-
-def build_args_sub_parser(func, main_parser, func_vars, func_dtypes, func_default_vars, mode="number"):
-    """
-    """
-    help_text = 'Function {} Arguments parser, if args are not given, it will be regarded as a string.'.format(func.__name__) if not func.__doc__ else func.__doc__
-    sub_parser = main_parser.add_parser(func.__name__, help=help_text)
-    sub_parser.set_defaults(func=func)
-    abbr_names_mapper = args_abbreviate(func_vars, mode=mode)
-    helper_mapper = helper_builder_from_doc(func.__doc__)
-    for var_name in func_vars:
-        argument_add(sub_parser, var_name, func_dtypes.get(var_name, str), func_default_vars.get(var_name, None), abbr_names_mapper[var_name], helper=helper_mapper.get(var_name, ""))
-    return main_parser
-
-
-def argument_add(parser, var_name, var_dtype, func_default_var, abbr_name, helper=""):
-    """
-    """
-    type_dict = {
-        "int" : int,
-        "str" : str,
-        "bool" : bool,
-        "float" : float,
-    }
-
-    if var_dtype == bool:
-        # bool type
-        flag = "True" if func_default_var else "False"
-        actions = {
-            "False": "store_true",
-            "True": "store_false",
-        }
-        parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), action=actions[flag], help='{}, deafult:{}, it will be {} if it\'s applied.'.format(var_name if not helper else helper, flag, "False" if flag == "True" else "True"))
-    elif isinstance(var_dtype, typing._GenericAlias):
-        # list type
-        dtype_fetch = re.findall(r'\[(.*)\]', str(var_dtype))
-        dtype = dtype_fetch[0] if dtype_fetch else str
-        parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), nargs='+', type=type_dict[dtype], help='{}, element type: {}'.format(var_name if not helper else helper, dtype))
-    else:
-        # other type
-        if func_default_var != None:
-            parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), type=var_dtype, default=func_default_var, help='{}, default:{}, type:{}'.format(var_name if not helper else helper, func_default_var, var_dtype.__name__))
-        else:
-            parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), type=var_dtype, required=True, help='{}, type:{}'.format(var_name if not helper else helper, var_dtype.__name__))
-
-
-def args_abbreviate(func_vars, mode="number"):
-    """
-    构建一个变量简称的mapper
-    """
-    abbr_names_cnt = Counter()
-    abbreviate_mapper = {}
-    alphabet_marker = [0] * 26
-
-    for var in func_vars:
-        abbr_name = ''.join(part[0] for part in var.split("_"))
-        if abbr_names_cnt[abbr_name] == 0:
-            if len(abbr_name) == 1:
-                alphabet_marker[ord(abbr_name) - ord('a')] = 1
-            abbreviate_mapper[var] = abbr_name
-            abbr_names_cnt[abbr_name] += 1
-        
-        else:
-            if mode == "number":
-                # 如果简称已经存在，则添加一个数字
-                abbr_names_cnt[abbr_name] += 1
-                abbreviate_mapper[var] = "{}{}".format(abbr_name, abbr_names_cnt[abbr_name])
-
-            elif mode == "letter":
-                # 如果简称已经存在，则寻找下一个不存在的字母
-                init_cnt = 0
-                while init_cnt < 26 and alphabet_marker[init_cnt] == 1:
-                    init_cnt += 1
-                
-                if init_cnt >= 26:
-                    raise ValueError("Too many arguments, cannot abbreviate.")
-
-                abbreviate_mapper[var] = chr(ord('a') + init_cnt)
-
-    return abbreviate_mapper
-
-
-def helper_builder_from_doc(func_doc):
-    """
-    如果文档里面有特殊的flag，可以将其转为说明
-    """
-    var_helper = {}
-
-    if func_doc is None:
-        return var_helper
-        
-    for line in func_doc.split("\n"):
-        if line.strip().startswith("@para"):
-            match = re.search("@para\s*:\s*([A-Za-z_]*)\s*:(.*)", line)
-            if match:
-                var_helper[match.group(1)] = match.group(2)
-
-    return var_helper
+# build the argparse object according to the function
+import argparse
+import re
+import typing, types
+from collections import Counter
+from mushroom.arg_textwrap import RawDescriptionHelpFormatter as HelpFormatter
+import mushroom.args_fetch as args_fetch
+
+
+def build_blank_parser(func_name, func_doc=""):
+    """
+    No arguments, just return the parser object
+    :return: argparse object
+    """
+    if not func_doc:
+        func_doc = 'Function {} No arguments, run directly'.format(func_name)
+
+    parser = argparse.ArgumentParser(description=func_doc, formatter_class=HelpFormatter)
+    return parser
+
+
+def build_args_parser(func_vars, func_dtypes, func_default_vars, func_name, func_doc="", mode="number"):
+    """
+    Build a parser according to the function vars
+    : return: argparse object
+    """
+    if not func_doc:
+        func_doc = 'Function {} Arguments parser, if args are not given, it will be regarded as a string.'.format(func_name)
+
+    parser = argparse.ArgumentParser(description=func_doc, formatter_class=HelpFormatter)
+    abbr_names_mapper = args_abbreviate(func_vars, mode=mode)
+    helper_mapper = helper_builder_from_doc(func_doc=func_doc)
+    for var_name in func_vars:
+        argument_add(parser, var_name, func_dtypes.get(var_name, str), func_default_vars.get(var_name, None), abbr_names_mapper[var_name], helper=helper_mapper.get(var_name, ""))
+    return parser
+
+
+def build_class_init_method(class_):
+    """
+    """
+    args_cnt, func_varnames, args_dtypes, default_flags = args_fetch.args_status_fetch(class_.__init__, isClass=True)
+    help_text = "MAIN PROGRAM" if not class_.__doc__ else class_.__doc__
+    if args_cnt == 0:
+        parser = build_blank_parser(func_name="", func_doc=help_text)
+            
+    else:
+        parser = build_args_parser(func_varnames, args_dtypes, default_flags, func_name="", func_doc=help_text)
+
+    subparser = parser.add_subparsers(help='sub command')    
+    return parser, subparser
+
+
+def build_blank_sub_parser(func:types.FunctionType, main_parser):
+    """
+    Build a blank sub command function
+    function should be a instance method
+    : return : argparse object
+    """
+    help_text = "sub command:{}, run directly".format(func.__name__) if not func.__doc__ else func.__doc__
+    sub_parser = main_parser.add_parser(func.__name__, help=help_text)
+    sub_parser.set_defaults(func=func)
+    return main_parser
+
+
+def build_args_sub_parser(func, main_parser, func_vars, func_dtypes, func_default_vars, mode="number"):
+    """
+    """
+    help_text = 'Function {} Arguments parser, if args are not given, it will be regarded as a string.'.format(func.__name__) if not func.__doc__ else func.__doc__
+    sub_parser = main_parser.add_parser(func.__name__, help=help_text)
+    sub_parser.set_defaults(func=func)
+    abbr_names_mapper = args_abbreviate(func_vars, mode=mode)
+    helper_mapper = helper_builder_from_doc(func.__doc__)
+    for var_name in func_vars:
+        argument_add(sub_parser, var_name, func_dtypes.get(var_name, str), func_default_vars.get(var_name, None), abbr_names_mapper[var_name], helper=helper_mapper.get(var_name, ""))
+    return main_parser
+
+
+def argument_add(parser, var_name, var_dtype, func_default_var, abbr_name, helper=""):
+    """
+    """
+    type_dict = {
+        "int" : int,
+        "str" : str,
+        "bool" : bool,
+        "float" : float,
+    }
+
+    if var_dtype == bool:
+        # bool type
+        flag = "True" if func_default_var else "False"
+        actions = {
+            "False": "store_true",
+            "True": "store_false",
+        }
+        parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), action=actions[flag], help='{}, deafult:{}, it will be {} if it\'s applied.'.format(var_name if not helper else helper, flag, "False" if flag == "True" else "True"))
+    elif isinstance(var_dtype, typing._GenericAlias):
+        # list type
+        dtype_fetch = re.findall(r'\[(.*)\]', str(var_dtype))
+        dtype = dtype_fetch[0] if dtype_fetch else str
+        parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), nargs='+', type=type_dict[dtype], help='{}, element type: {}'.format(var_name if not helper else helper, dtype))
+    else:
+        # other type
+        if func_default_var is not None:
+            parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), type=var_dtype, default=func_default_var, help='{}, default:{}, type:{}'.format(var_name if not helper else helper, func_default_var, var_dtype.__name__))
+        else:
+            parser.add_argument('--{}'.format(var_name), '-{}'.format(abbr_name), type=var_dtype, required=True, help='{}, type:{}'.format(var_name if not helper else helper, var_dtype.__name__))
+
+
+def args_abbreviate(func_vars, mode="number"):
+    """
+    构建一个变量简称的mapper
+    """
+    abbr_names_cnt = Counter()
+    abbreviate_mapper = {}
+    alphabet_marker = [0] * 26
+
+    for var in func_vars:
+        abbr_name = ''.join(part[0] for part in var.split("_"))
+        if abbr_names_cnt[abbr_name] == 0:
+            if len(abbr_name) == 1:
+                alphabet_marker[ord(abbr_name) - ord('a')] = 1
+            abbreviate_mapper[var] = abbr_name
+            abbr_names_cnt[abbr_name] += 1
+        
+        else:
+            if mode == "number":
+                # 如果简称已经存在，则添加一个数字
+                abbr_names_cnt[abbr_name] += 1
+                abbreviate_mapper[var] = "{}{}".format(abbr_name, abbr_names_cnt[abbr_name])
+
+            elif mode == "letter":
+                # 如果简称已经存在，则寻找下一个不存在的字母
+                init_cnt = 0
+                while init_cnt < 26 and alphabet_marker[init_cnt] == 1:
+                    init_cnt += 1
+                
+                if init_cnt >= 26:
+                    raise ValueError("Too many arguments, cannot abbreviate.")
+
+                abbreviate_mapper[var] = chr(ord('a') + init_cnt)
+
+    return abbreviate_mapper
+
+
+def helper_builder_from_doc(func_doc):
+    """
+    如果文档里面有特殊的flag，可以将其转为说明
+    """
+    var_helper = {}
+
+    if func_doc is None:
+        return var_helper
+        
+    for line in func_doc.split("\n"):
+        if line.strip().startswith("@para"):
+            match = re.search("@para\s*:\s*([A-Za-z_]*)\s*:(.*)", line)
+            if match:
+                var_helper[match.group(1)] = match.group(2)
+
+    return var_helper
```

### Comparing `mushroom_cli-0.2.5/mushroom/args_fetch.py` & `mushroom_cli-0.3.1/mushroom/args_fetch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# 处理函数的参数
-import types
-
-
-def args_status_fetch(func:types.FunctionType, isClass=False):
-    """
-    """
-    # if contains self argument, it's a class method
-    start_idx = 1 if isClass else 0
-    args_cnt = func.__code__.co_argcount
-    func_varnames = func.__code__.co_varnames[start_idx:args_cnt]
-    args_dtypes = func.__annotations__
-    default_flags = fetch_defaults(func, func_varnames)
-
-    return args_cnt, func_varnames, args_dtypes, default_flags
-
-
-
-def fetch_defaults(func, func_varnames):
-    """
-    fetch default values for the function
-    return a dict
-    """
-    func_defaults = func.__defaults__
-
-    func_defaults_dict = {}
-    if not func_defaults:
-        return func_defaults_dict
-
-    func_defaults = func_defaults[::-1]
-    func_varnames = func_varnames[::-1]
-    for i in range(len(func_defaults)):
-        func_defaults_dict[func_varnames[i]] = func_defaults[i]
-
-    return func_defaults_dict
-
+# 处理函数的参数
+import types
+from mushroom.arg_exceptions import TypeNotMatchException
+
+
+def args_status_fetch(func:types.FunctionType, isClass=False):
+    """
+    """
+    # if contains self argument, it's a class method
+    start_idx = 1 if isClass else 0
+    args_cnt = func.__code__.co_argcount
+    func_varnames = func.__code__.co_varnames[start_idx:args_cnt]
+    args_dtypes = func.__annotations__
+    default_flags = fetch_defaults(func, func_varnames, args_dtypes)
+
+    return args_cnt, func_varnames, args_dtypes, default_flags
+
+
+
+def fetch_defaults(func, func_varnames, args_dtypes):
+    """
+    fetch default values for the function
+    return a dict
+    """
+    func_defaults = func.__defaults__
+
+    func_defaults_dict = {}
+    if not func_defaults:
+        return func_defaults_dict
+
+    func_defaults = func_defaults[::-1]
+    func_varnames = func_varnames[::-1]
+    for i in range(len(func_defaults)):
+        if not isinstance(func_defaults[i], args_dtypes.get(func_varnames[i], str)):
+            raise TypeNotMatchException("arg '{}' default value {} can not match the type {} ".format(func_varnames[i], func_defaults[i], args_dtypes.get(func_varnames[i], str)))
+        func_defaults_dict[func_varnames[i]] = func_defaults[i]
+
+    return func_defaults_dict
+
```

### Comparing `mushroom_cli-0.2.5/mushroom/core.py` & `mushroom_cli-0.3.1/mushroom/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-from __future__ import absolute_import
-import time
-from functools import wraps
-import types
-from mushroom.func_parser import func_parser, run_func, class_parser
-
-
-
-def Mushroom(func, timer=False):
-    """
-    one command type console app
-    """
-    rslt = None
-    if timer:
-        start_time = time.perf_counter()
-
-    if isinstance(func, types.FunctionType):
-        # function type
-        argparser = func_parser(func)
-        args = argparser.parse_args()
-        rslt = run_func(args, func)
-    elif type(func) == type:
-        # class type
-        argparser = class_parser(func)
-        args = argparser.parse_args()
-        # initialize first
-        kwargs = {var_name: getattr(args, var_name) for var_name in func.__init__.__code__.co_varnames[1:] if getattr(args, var_name)}
-        instance_ = func(**kwargs)
-        #fetch the function
-        if not hasattr(args, 'func'):
-            print("Subcommand not found, plz type -h or --help to get more information")
-            return
-        rslt = run_func(args, args.func, isClass=True, self=instance_)
-    else:
-        raise Exception("func must be function or class type")
-
-    if rslt:
-        print(rslt)
-
-    if timer:
-        print("[INFO] Time cost: {}s".format(time.perf_counter() - start_time))
-
-
-
-def mushroom(timer=False):
-    def main_func(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            Mushroom(func, timer)
-        return wrapper
-    return main_func
-
+from __future__ import absolute_import
+import sys
+import time
+from functools import wraps
+import types
+from mushroom.func_parser import func_parser, run_func, class_parser
+import mushroom.traceback_module as tb
+
+
+def Mushroom(func, timer=False, traceback=False):
+    """
+    one command type console app
+    """
+    rslt = None
+    if timer:
+        start_time = time.perf_counter()
+
+    if traceback:
+        sys.excepthook = tb.global_excepthook
+
+    if isinstance(func, types.FunctionType):
+        # function type
+        argparser = func_parser(func)
+        args = argparser.parse_args()
+        rslt = run_func(args, func)
+    elif type(func) == type:
+        # class type
+        argparser = class_parser(func)
+        args = argparser.parse_args()
+        # initialize first
+        kwargs = {var_name: getattr(args, var_name) for var_name in func.__init__.__code__.co_varnames[1:] if getattr(args, var_name)}
+        instance_ = func(**kwargs)
+        #fetch the function
+        if not hasattr(args, 'func'):
+            print("Subcommand not found, plz type -h or --help to get more information")
+            return
+        rslt = run_func(args, args.func, isClass=True, self=instance_)
+    else:
+        raise Exception("func must be function or class type")
+
+    if rslt:
+        print(rslt)
+
+    if timer:
+        print("[INFO] Time cost: {}s".format(time.perf_counter() - start_time))
+
+
+
+def mushroom(timer=False, traceback=False):
+    def main_func(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            Mushroom(func, timer, traceback)
+        return wrapper
+    return main_func
+
```

### Comparing `mushroom_cli-0.2.5/mushroom/func_parser.py` & `mushroom_cli-0.3.1/mushroom/func_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-# one command type console app
-from __future__ import absolute_import
-from types import FunctionType as function
-import mushroom.arg_builder as arg_builder
-import mushroom.args_fetch as args_fetch
-
-
-def func_parser(func:function):
-    """
-
-    """
-    args_cnt, func_varnames, args_dtypes, default_flags = args_fetch.args_status_fetch(func, isClass=False)
-
-    if args_cnt == 0:
-        # can run directly
-        arg_parser = arg_builder.build_blank_parser(func.__name__, func.__doc__)
-    else:
-        arg_parser = arg_builder.build_args_parser(func_varnames, args_dtypes, default_flags, func.__name__, func.__doc__)
-
-    return arg_parser
-
-
-def class_parser(class_):
-    """
-    """
-    # initialize first
-    parser, subparser = arg_builder.build_class_init_method(class_)
-    # iter the method of class
-    for func_name, func in class_.__dict__.items():
-        if isinstance(func, function) and not func_name.startswith("_"):
-            # function type
-            args_cnt, func_vars, func_dtypes, func_default_vars = args_fetch.args_status_fetch(func, isClass=True)
-            if args_cnt == 0:
-                # can run directly
-                arg_builder.build_blank_sub_parser(func, subparser)
-            else:
-                # need args parser
-                arg_builder.build_args_sub_parser(func, subparser, func_vars, func_dtypes, func_default_vars)
-    return parser
-        
-
-def run_func(args, func, isClass=False, self=None):
-    """
-    run the function
-    """
-    start_idx = 1 if isClass else 0
-    args_cnt = func.__code__.co_argcount
-    kwargs = {var_name: getattr(args, var_name) for var_name in func.__code__.co_varnames[start_idx:args_cnt] if hasattr(args, var_name)}
-    if self:
-        kwargs['self'] = self
-    return func(**kwargs)
-
+# one command type console app
+from __future__ import absolute_import
+from types import FunctionType as function
+import mushroom.arg_builder as arg_builder
+import mushroom.args_fetch as args_fetch
+
+
+def func_parser(func:function):
+    """
+
+    """
+    args_cnt, func_varnames, args_dtypes, default_flags = args_fetch.args_status_fetch(func, isClass=False)
+
+    if args_cnt == 0:
+        # can run directly
+        arg_parser = arg_builder.build_blank_parser(func.__name__, func.__doc__)
+    else:
+        arg_parser = arg_builder.build_args_parser(func_varnames, args_dtypes, default_flags, func.__name__, func.__doc__)
+
+    return arg_parser
+
+
+def class_parser(class_):
+    """
+    """
+    # initialize first
+    parser, subparser = arg_builder.build_class_init_method(class_)
+    # iter the method of class
+    for func_name, func in class_.__dict__.items():
+        if isinstance(func, function) and not func_name.startswith("_"):
+            # function type
+            args_cnt, func_vars, func_dtypes, func_default_vars = args_fetch.args_status_fetch(func, isClass=True)
+            if args_cnt == 0:
+                # can run directly
+                arg_builder.build_blank_sub_parser(func, subparser)
+            else:
+                # need args parser
+                arg_builder.build_args_sub_parser(func, subparser, func_vars, func_dtypes, func_default_vars)
+    return parser
+        
+
+def run_func(args, func, isClass=False, self=None):
+    """
+    run the function
+    """
+    start_idx = 1 if isClass else 0
+    args_cnt = func.__code__.co_argcount
+    kwargs = {var_name: getattr(args, var_name) for var_name in func.__code__.co_varnames[start_idx:args_cnt] if hasattr(args, var_name)}
+    if self:
+        kwargs['self'] = self
+            
+    return func(**kwargs)
+
```

