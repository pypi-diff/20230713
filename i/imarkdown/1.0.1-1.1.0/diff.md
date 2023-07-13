# Comparing `tmp/imarkdown-1.0.1.tar.gz` & `tmp/imarkdown-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imarkdown-1.0.1.tar", last modified: Fri Jul  7 02:00:52 2023, max compression
+gzip compressed data, was "imarkdown-1.1.0.tar", last modified: Thu Jul 13 09:34:00 2023, max compression
```

## Comparing `imarkdown-1.0.1.tar` & `imarkdown-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.431477 imarkdown-1.0.1/
--rw-rw-rw-   0        0        0     5881 2023-07-07 02:00:52.430468 imarkdown-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5012 2023-07-06 05:36:56.000000 imarkdown-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.406475 imarkdown-1.0.1/imarkdown/
--rw-rw-rw-   0        0        0       74 2023-07-06 09:58:57.000000 imarkdown-1.0.1/imarkdown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.420476 imarkdown-1.0.1/imarkdown/adapter/
--rw-rw-rw-   0        0        0      476 2023-07-06 15:57:43.000000 imarkdown-1.0.1/imarkdown/adapter/__init__.py
--rw-rw-rw-   0        0        0     2756 2023-07-06 17:20:25.000000 imarkdown-1.0.1/imarkdown/adapter/aliyun_adapter.py
--rw-rw-rw-   0        0        0      722 2023-07-06 16:49:13.000000 imarkdown-1.0.1/imarkdown/adapter/base.py
--rw-rw-rw-   0        0        0      408 2023-07-06 16:37:08.000000 imarkdown-1.0.1/imarkdown/adapter/local_adapter.py
--rw-rw-rw-   0        0        0     1367 2023-07-06 15:57:43.000000 imarkdown-1.0.1/imarkdown/config.py
--rw-rw-rw-   0        0        0      267 2023-07-06 13:32:07.000000 imarkdown-1.0.1/imarkdown/constant.py
--rw-rw-rw-   0        0        0     7836 2023-07-06 17:27:46.000000 imarkdown-1.0.1/imarkdown/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.425464 imarkdown-1.0.1/imarkdown/utils/
--rw-rw-rw-   0        0        0      276 2023-07-06 16:22:43.000000 imarkdown-1.0.1/imarkdown/utils/__init__.py
--rw-rw-rw-   0        0        0      282 2023-07-06 15:57:43.000000 imarkdown-1.0.1/imarkdown/utils/cache.py
--rw-rw-rw-   0        0        0     1403 2023-07-02 17:09:48.000000 imarkdown-1.0.1/imarkdown/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.414466 imarkdown-1.0.1/imarkdown.egg-info/
--rw-rw-rw-   0        0        0     5881 2023-07-07 02:00:52.000000 imarkdown-1.0.1/imarkdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-07-07 02:00:52.000000 imarkdown-1.0.1/imarkdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:00:52.000000 imarkdown-1.0.1/imarkdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-07 02:00:52.000000 imarkdown-1.0.1/imarkdown.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 02:00:52.000000 imarkdown-1.0.1/imarkdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.0.1/license
--rw-rw-rw-   0        0        0       42 2023-07-07 02:00:52.431477 imarkdown-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1909 2023-07-07 02:00:25.000000 imarkdown-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 02:00:52.428472 imarkdown-1.0.1/tests/
--rw-rw-rw-   0        0        0     1326 2023-07-06 17:20:23.000000 imarkdown-1.0.1/tests/test_adapter.py
--rw-rw-rw-   0        0        0     1192 2023-07-06 17:27:46.000000 imarkdown-1.0.1/tests/test_converter.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.076101 imarkdown-1.1.0/
+-rw-rw-rw-   0        0        0    17228 2023-07-13 09:34:00.075103 imarkdown-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16366 2023-07-13 09:18:34.000000 imarkdown-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.046037 imarkdown-1.1.0/imarkdown/
+-rw-rw-rw-   0        0        0      464 2023-07-12 09:17:55.000000 imarkdown-1.1.0/imarkdown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.060212 imarkdown-1.1.0/imarkdown/adapter/
+-rw-rw-rw-   0        0        0      476 2023-07-06 15:57:43.000000 imarkdown-1.1.0/imarkdown/adapter/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-07-12 09:17:55.000000 imarkdown-1.1.0/imarkdown/adapter/aliyun_adapter.py
+-rw-rw-rw-   0        0        0      835 2023-07-12 14:17:49.000000 imarkdown-1.1.0/imarkdown/adapter/base.py
+-rw-rw-rw-   0        0        0      755 2023-07-09 06:11:27.000000 imarkdown-1.1.0/imarkdown/adapter/local_adapter.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.061115 imarkdown-1.1.0/imarkdown/client/
+-rw-rw-rw-   0        0        0        0 2023-07-12 09:17:53.000000 imarkdown-1.1.0/imarkdown/client/__init__.py
+-rw-rw-rw-   0        0        0     1371 2023-07-12 10:24:22.000000 imarkdown-1.1.0/imarkdown/config.py
+-rw-rw-rw-   0        0        0      267 2023-07-06 13:32:07.000000 imarkdown-1.1.0/imarkdown/constant.py
+-rw-rw-rw-   0        0        0    12736 2023-07-13 06:24:26.000000 imarkdown-1.1.0/imarkdown/converter.py
+-rw-rw-rw-   0        0        0     9764 2023-07-12 10:45:20.000000 imarkdown-1.1.0/imarkdown/schema.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.065101 imarkdown-1.1.0/imarkdown/utils/
+-rw-rw-rw-   0        0        0     2784 2023-07-12 10:45:20.000000 imarkdown-1.1.0/imarkdown/utils/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-07-06 15:57:43.000000 imarkdown-1.1.0/imarkdown/utils/cache.py
+-rw-rw-rw-   0        0        0     1403 2023-07-02 17:09:48.000000 imarkdown-1.1.0/imarkdown/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.053581 imarkdown-1.1.0/imarkdown.egg-info/
+-rw-rw-rw-   0        0        0    17228 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 09:33:59.000000 imarkdown-1.1.0/imarkdown.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.0/license
+-rw-rw-rw-   0        0        0       42 2023-07-13 09:34:00.076101 imarkdown-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1904 2023-07-13 09:00:03.000000 imarkdown-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 09:34:00.073104 imarkdown-1.1.0/tests/
+-rw-rw-rw-   0        0        0     2379 2023-07-12 09:57:46.000000 imarkdown-1.1.0/tests/test_adapter.py
+-rw-rw-rw-   0        0        0     2273 2023-07-12 09:17:55.000000 imarkdown-1.1.0/tests/test_image_converter.py
+-rw-rw-rw-   0        0        0     2235 2023-07-12 09:21:39.000000 imarkdown-1.1.0/tests/test_md_file.py
+-rw-rw-rw-   0        0        0     2957 2023-07-12 08:04:11.000000 imarkdown-1.1.0/tests/test_utils.py
```

### Comparing `imarkdown-1.0.1/imarkdown/adapter/aliyun_adapter.py` & `imarkdown-1.1.0/imarkdown/adapter/aliyun_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Optional, Any, Dict
 
-from pydantic import root_validator, validator
+from pydantic import root_validator
 
 from imarkdown.adapter.base import BaseMdAdapter
 from imarkdown.config import IMarkdownConfig
 from imarkdown.utils import polish_path
 
 logger = logging.getLogger(__name__)
 cfg: IMarkdownConfig = IMarkdownConfig()
@@ -27,18 +27,23 @@
     """Necessary parameter when initialization."""
     endpoint: Optional[str] = None
     auth: Any
     bucket: Any
 
     @root_validator(pre=True)
     def validate_environment(cls, values: Optional[Dict]) -> Dict:
-        if values:
-            cfg.store_variable(cls.__name__, values)
-        else:
-            values: Dict = cfg.load_variable(cls.__name__)
+        env_config: Dict[str, Any] = cfg.load_variable(cls.__name__)
+        if env_config:
+            if not values:
+                values = {}
+            for env_key in env_config.keys():
+                if env_key not in values:
+                    values.update({env_key: env_config[env_key]})
+        cfg.store_variable(cls.__name__, values)
+
         if not values:
             raise ValueError("Please initialize your AliyunAdapter with parameters.")
         logger.debug(f"[imarkdown aliyun adapter] params: {values}")
 
         try:
             import oss2
 
@@ -52,28 +57,27 @@
         except ImportError:
             raise ValueError(
                 "Could not import oss2 python package. "
                 "Please install it with `pip install oss2`."
             )
         return values
 
-    @validator("enable_https")
-    def update_url_prefix(cls, v: bool, values: Dict[str, Any]) -> bool:
+    def set_enable_https(cls, v: bool, values: Dict[str, Any]) -> bool:
         import oss2
 
         if v:
             cls.url_prefix = "https"
         else:
             cls.url_prefix = "http"
 
         values["endpoint"] = f'{cls.url_prefix}://oss-cn-{values["place"]}.aliyuncs.com'
         values["bucket"] = oss2.Bucket(
             values["auth"], values["endpoint"], values["bucket_name"]
         )
         return v
 
     def upload(self, key: str, file):
-        path = polish_path(f"{self.path_prefix}/{key}", enable_suffix=False)
+        path = polish_path(f"{self.storage_path_prefix}/{key}", enable_suffix=False)
         self.bucket.put_object(path, file)
 
     def get_replaced_url(self, key):
-        return f"{self.url_prefix}://{self.bucket_name}.oss-cn-{self.place}.aliyuncs.com/{self.path_prefix}/{key}"
+        return f"{self.url_prefix}://{self.bucket_name}.oss-cn-{self.place}.aliyuncs.com/{self.storage_path_prefix}/{key}"
```

### Comparing `imarkdown-1.0.1/imarkdown/adapter/base.py` & `imarkdown-1.1.0/imarkdown/adapter/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 from pydantic import BaseModel
 
 
 class BaseMdAdapter(BaseModel):
     name: str
     """Adapter name"""
-    path_prefix: str = ""
-    """Image path file prefix. Final image name is `{path_prefix}/{key}`"""
+    storage_path_prefix: str = ""
+    """Image path file prefix. Final image name is `{storage_path_prefix}/{key}`"""
 
     class Config:
         arbitrary_types_allowed = True
 
     @abstractmethod
     def upload(self, key: str, file):
-        """upload image to Image Server"""
+        """Upload image to Image Server.
+
+        Args:
+            key: image name
+            file: markdown string data
+        """
         raise NotImplementedError("Your adapter should implement `upload` method")
 
     @abstractmethod
     def get_replaced_url(self, key):
         """get replaced url or image path"""
         raise NotImplementedError(
             "Your adapter should implement `get_replaced_url` method"
```

### Comparing `imarkdown-1.0.1/imarkdown/config.py` & `imarkdown-1.1.0/imarkdown/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         logger.debug(f"[imarkdown] get last adapter <{adapter_name}>")
         if not adapter_name or adapter_name not in _MdAdapterType.keys():
             return MdAdapterType.Local
         return _MdAdapterType[str(adapter_name)]
 
     @last_adapter_name.setter
     def last_adapter_name(self, value: str):
-        if value not in _MdAdapterType.keys():
-            raise ValueError(f"<{value}> type adapter not exist.")
+        # if value not in _MdAdapterType.keys():
+        #     raise ValueError(f"<{value}> type adapter not exist.")
         self.cache["last_adapter"] = value
 
     def load_variable(self, key: str) -> Any:
         return self.cache.get(key, None)
 
     def store_variable(self, key: str, value: Any) -> Any:
         self.cache[key] = value
```

### Comparing `imarkdown-1.0.1/imarkdown/utils/singleton.py` & `imarkdown-1.1.0/imarkdown/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `imarkdown-1.0.1/imarkdown.egg-info/SOURCES.txt` & `imarkdown-1.1.0/imarkdown.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 README.md
 license
 setup.py
 imarkdown/__init__.py
 imarkdown/config.py
 imarkdown/constant.py
 imarkdown/converter.py
+imarkdown/schema.py
 imarkdown.egg-info/PKG-INFO
 imarkdown.egg-info/SOURCES.txt
 imarkdown.egg-info/dependency_links.txt
 imarkdown.egg-info/requires.txt
 imarkdown.egg-info/top_level.txt
 imarkdown/adapter/__init__.py
 imarkdown/adapter/aliyun_adapter.py
 imarkdown/adapter/base.py
 imarkdown/adapter/local_adapter.py
+imarkdown/client/__init__.py
 imarkdown/utils/__init__.py
 imarkdown/utils/cache.py
 imarkdown/utils/singleton.py
 tests/test_adapter.py
-tests/test_converter.py
+tests/test_image_converter.py
+tests/test_md_file.py
+tests/test_utils.py
```

### Comparing `imarkdown-1.0.1/license` & `imarkdown-1.1.0/license`

 * *Files identical despite different names*

### Comparing `imarkdown-1.0.1/setup.py` & `imarkdown-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 import setuptools
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="imarkdown",
-    version="1.0.1",
+    version="1.1.0",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A practical Markdown image url converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Undertone0809/md-img-converter",
+    url="https://github.com/Undertone0809/imarkdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
         "pydantic==1.10.0",
         "cushy-storage"
+
     ],
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

