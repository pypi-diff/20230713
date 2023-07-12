# Comparing `tmp/configzen-0.6.0.tar.gz` & `tmp/configzen-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.6.0.tar", max compression
+gzip compressed data, was "configzen-0.6.1.tar", max compression
```

## Comparing `configzen-0.6.0.tar` & `configzen-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      560 2023-07-12 17:05:42.365663 configzen-0.6.0/configzen/__init__.py
--rw-r--r--   0        0        0      901 2023-07-06 04:46:24.689646 configzen-0.6.0/configzen/__main__.py
--rw-r--r--   0        0        0     1677 2023-07-12 16:47:13.813568 configzen-0.6.0/configzen/_detach.py
--rw-r--r--   0        0        0     3295 2023-07-12 15:49:28.622492 configzen-0.6.0/configzen/_setup.py
--rw-r--r--   0        0        0     4997 2023-07-06 04:46:31.747498 configzen-0.6.0/configzen/decorators.py
--rw-r--r--   0        0        0     4294 2023-07-06 04:46:34.678790 configzen-0.6.0/configzen/errors.py
--rw-r--r--   0        0        0      475 2023-07-06 04:46:37.882744 configzen-0.6.0/configzen/field.py
--rw-r--r--   0        0        0    14453 2023-07-12 17:06:16.632311 configzen-0.6.0/configzen/interpolation.py
--rw-r--r--   0        0        0    77237 2023-07-12 17:17:27.067524 configzen-0.6.0/configzen/model.py
--rw-r--r--   0        0        0     3752 2023-07-12 16:47:14.105134 configzen-0.6.0/configzen/module.py
--rw-r--r--   0        0        0    25405 2023-07-06 04:46:48.597531 configzen-0.6.0/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.6.0/configzen/py.typed
--rw-r--r--   0        0        0     4568 2023-07-06 04:47:00.398626 configzen-0.6.0/configzen/route.py
--rw-r--r--   0        0        0     1160 2023-07-06 04:46:57.057284 configzen-0.6.0/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.6.0/LICENSE
--rw-r--r--   0        0        0     1683 2023-07-12 17:18:17.998544 configzen-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    14309 2023-07-12 17:20:51.907213 configzen-0.6.0/README.md
--rw-r--r--   0        0        0    15240 1970-01-01 00:00:00.000000 configzen-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-07-12 21:53:25.233305 configzen-0.6.1/configzen/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-12 21:52:27.881323 configzen-0.6.1/configzen/__main__.py
+-rw-r--r--   0        0        0     1677 2023-07-12 21:55:34.687190 configzen-0.6.1/configzen/_detach.py
+-rw-r--r--   0        0        0     3295 2023-07-12 21:52:44.538365 configzen-0.6.1/configzen/_setup.py
+-rw-r--r--   0        0        0     4997 2023-07-12 21:52:41.108165 configzen-0.6.1/configzen/decorators.py
+-rw-r--r--   0        0        0     4294 2023-07-12 21:53:19.301659 configzen-0.6.1/configzen/errors.py
+-rw-r--r--   0        0        0      475 2023-07-12 21:53:14.010654 configzen-0.6.1/configzen/field.py
+-rw-r--r--   0        0        0    14453 2023-07-12 21:53:28.633194 configzen-0.6.1/configzen/interpolation.py
+-rw-r--r--   0        0        0    77295 2023-07-12 22:06:37.878842 configzen-0.6.1/configzen/model.py
+-rw-r--r--   0        0        0     3968 2023-07-12 22:06:37.859841 configzen-0.6.1/configzen/module.py
+-rw-r--r--   0        0        0    25405 2023-07-12 21:53:33.061934 configzen-0.6.1/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.6.1/configzen/py.typed
+-rw-r--r--   0        0        0     4568 2023-07-12 21:53:50.319255 configzen-0.6.1/configzen/route.py
+-rw-r--r--   0        0        0     1160 2023-07-12 21:53:55.822202 configzen-0.6.1/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1683 2023-07-12 22:12:32.782198 configzen-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    14372 2023-07-12 22:11:01.433766 configzen-0.6.1/README.md
+-rw-r--r--   0        0        0    15303 1970-01-01 00:00:00.000000 configzen-0.6.1/PKG-INFO
```

### Comparing `configzen-0.6.0/configzen/__init__.py` & `configzen-0.6.1/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/__main__.py` & `configzen-0.6.1/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/_detach.py` & `configzen-0.6.1/configzen/_detach.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/_setup.py` & `configzen-0.6.1/configzen/_setup.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/decorators.py` & `configzen-0.6.1/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/errors.py` & `configzen-0.6.1/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/interpolation.py` & `configzen-0.6.1/configzen/interpolation.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/model.py` & `configzen-0.6.1/configzen/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2231,16 +2231,16 @@
             wrapped_module = getattr(self, MODULE, None)
             if wrapped_module is None:
                 raise
             importlib.reload(wrapped_module)
             self.update(
                 {
                     key: value
-                    for key, value in wrapped_module.__dict__.items()
-                    if key in self.__fields__
+                    for key, value in vars(wrapped_module).items()
+                    if key in {field.alias for field in self.__fields__.values()}
                 }
             )
             return self
         current_context.set(get_context(context.owner))
         if context.owner is self:
             changed = context.agent.read(config_class=type(self), **kwargs)
         else:
@@ -2408,23 +2408,23 @@
             target_type=target_type,
         )
 
     @classmethod
     def wrap_module(
         cls: type[ConfigModelT],
         module_name: str | types.ModuleType,
+        package: str | None = None,
         /,
         **values: Any,
     ) -> ConfigModelT:
         module_vars = None
         if isinstance(module_name, str):
             module_name = module_name
             if module_name not in sys.modules:
-                package = None
-                if module_name.startswith("."):
+                if package is None and module_name.startswith("."):
                     current_frame = inspect.currentframe()
                     assert current_frame is not None
                     frame_back = current_frame.f_back
                     assert frame_back is not None
                     package = frame_back.f_globals["__package__"]
                 module_vars = vars(
                     importlib.import_module(module_name, package=package)
```

### Comparing `configzen-0.6.0/configzen/module.py` & `configzen-0.6.1/configzen/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,21 @@
                 __ns = locals()
                 for key in __annotations__:
                     __ns[key] = module_vars[key]  # type: ignore[index]
                 del __ns
 
             model_class = cast(type[ConfigModelT], ModuleConfigModel)
 
+        module_values = {}
+        for key, value in module_vars.items():
+            if key in {field.alias for field in model_class.__fields__.values()}:
+                module_values[key] = value
+
         config_module = cls(
-            model=cast(ConfigModelT, model_class).parse_obj(values),
+            model=cast(ConfigModelT, model_class).parse_obj(module_values | values),
             module_vars=module_vars,
             name=module_vars["__name__"],
             doc=module_vars["__doc__"],
         )
         return config_module
 
     @classmethod
```

### Comparing `configzen-0.6.0/configzen/processor.py` & `configzen-0.6.1/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/route.py` & `configzen-0.6.1/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/configzen/typedefs.py` & `configzen-0.6.1/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/LICENSE` & `configzen-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.6.0/pyproject.toml` & `configzen-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.6.0"
+version = "0.6.1"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.6.0/README.md` & `configzen-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -261,29 +261,34 @@
 
 1) Without writing a model class:
 
 ```python
 # config.py
 from configzen import ConfigModule
 
+# Annotate config fields
 HOST: str = "localhost"
 PORT: int = 8000
 
 ConfigModule.wrap_this_module()
 ```
 
 2) With a model class:
 
 ```python
 # config.py
 from configzen import ConfigModel
 
+# Annotations are optional
+HOST = "localhost"
+PORT = 8000
+
 class AppConfig(ConfigModel):
-    HOST: str = "localhost"
-    PORT: int = 8000
+    HOST: str
+    PORT: int
     
 AppConfig.wrap_this_module()
 ```
 
 Now values `HOST` and `PORT` will be validated as `str` and `int` data types, respectively:
 
 ```python
```

### Comparing `configzen-0.6.0/PKG-INFO` & `configzen-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.6.0
+Version: 0.6.1
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -285,29 +285,34 @@
 
 1) Without writing a model class:
 
 ```python
 # config.py
 from configzen import ConfigModule
 
+# Annotate config fields
 HOST: str = "localhost"
 PORT: int = 8000
 
 ConfigModule.wrap_this_module()
 ```
 
 2) With a model class:
 
 ```python
 # config.py
 from configzen import ConfigModel
 
+# Annotations are optional
+HOST = "localhost"
+PORT = 8000
+
 class AppConfig(ConfigModel):
-    HOST: str = "localhost"
-    PORT: int = 8000
+    HOST: str
+    PORT: int
     
 AppConfig.wrap_this_module()
 ```
 
 Now values `HOST` and `PORT` will be validated as `str` and `int` data types, respectively:
 
 ```python
```

