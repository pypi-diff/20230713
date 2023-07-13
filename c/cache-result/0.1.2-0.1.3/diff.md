# Comparing `tmp/cache-result-0.1.2.tar.gz` & `tmp/cache-result-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.2.tar", last modified: Thu Jul 13 15:03:10 2023, max compression
+gzip compressed data, was "cache-result-0.1.3.tar", last modified: Thu Jul 13 15:46:14 2023, max compression
```

## Comparing `cache-result-0.1.2.tar` & `cache-result-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:03:10.435145 cache-result-0.1.2/
--rw-rw-rw-   0        0        0     1740 2023-07-13 15:03:10.434145 cache-result-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 15:03:10.420147 cache-result-0.1.2/cache_result/
--rw-rw-rw-   0        0        0     2585 2023-07-13 14:58:33.000000 cache-result-0.1.2/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 15:03:10.432144 cache-result-0.1.2/cache_result.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-07-13 15:03:09.000000 cache-result-0.1.2/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-13 15:03:10.000000 cache-result-0.1.2/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:03:09.000000 cache-result-0.1.2/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 15:03:09.000000 cache-result-0.1.2/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 15:03:10.436144 cache-result-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-07-13 15:02:14.000000 cache-result-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.278815 cache-result-0.1.3/
+-rw-rw-rw-   0        0        0     1740 2023-07-13 15:46:14.277815 cache-result-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.264824 cache-result-0.1.3/cache_result/
+-rw-rw-rw-   0        0        0     2676 2023-07-13 15:42:42.000000 cache-result-0.1.3/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.274815 cache-result-0.1.3/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-13 15:46:14.000000 cache-result-0.1.3/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:46:14.278815 cache-result-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-07-13 15:45:45.000000 cache-result-0.1.3/setup.py
```

### Comparing `cache-result-0.1.2/PKG-INFO` & `cache-result-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: cache-result
-Version: 0.1.2
-Summary: A decorator for caching the results of functions
-Author: glwhappen
-Author-email: 1597721684@qq.com
-Description-Content-Type: text/markdown
-
 # Cache Function Result
 
 ## Description
 
 这是一个Python包，它提供了一个装饰器用于缓存函数的返回结果。缓存的结果可以指定任意位置，非常的自由，缓存的键则是根据函数名、源代码和参数来控制的。你可以选择排除某些元素，例如函数名、源代码、参数或者关键字参数。
 
 This is a Python package that provides a decorator for caching the results of functions. The cache is stored in a specified directory, and the cache key is generated based on the function name, source code, and arguments. The decorator allows you to exclude certain elements from the cache key, such as the function name, source code, arguments, or keyword arguments.
```

### Comparing `cache-result-0.1.2/README.md` & `cache-result-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: cache-result
+Version: 0.1.3
+Summary: A decorator for caching the results of functions
+Author: glwhappen
+Author-email: 1597721684@qq.com
+Description-Content-Type: text/markdown
+
 # Cache Function Result
 
 ## Description
 
 这是一个Python包，它提供了一个装饰器用于缓存函数的返回结果。缓存的结果可以指定任意位置，非常的自由，缓存的键则是根据函数名、源代码和参数来控制的。你可以选择排除某些元素，例如函数名、源代码、参数或者关键字参数。
 
 This is a Python package that provides a decorator for caching the results of functions. The cache is stored in a specified directory, and the cache key is generated based on the function name, source code, and arguments. The decorator allows you to exclude certain elements from the cache key, such as the function name, source code, arguments, or keyword arguments.
```

### Comparing `cache-result-0.1.2/cache_result/__init__.py` & `cache-result-0.1.3/cache_result/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         def wrapper(*args, **kwargs):
             # 获取函数的源代码，并删除所有空格和空行
             source_code = inspect.getsource(func)
 
             # 获取函数的参数名
             params = inspect.signature(func).parameters
             # 创建一个字典，将参数名和值对应起来
-            args_dict = {list(params.keys())[i]: arg for i, arg in enumerate(args)}
+            args_dict = {name: kwargs.get(name, param.default) if param.default is not inspect.Parameter.empty else args[i] for i, (name, param) in enumerate(params.items())}
             args_dict.update(kwargs)
 
             # 使用参数值来修改路径
             modified_cache_dir = cache_dir.format(**args_dict)
 
 
             hash_key = []
```

### Comparing `cache-result-0.1.2/cache_result.egg-info/PKG-INFO` & `cache-result-0.1.3/cache_result.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.2
+Version: 0.1.3
 Summary: A decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

