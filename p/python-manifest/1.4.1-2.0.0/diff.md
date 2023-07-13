# Comparing `tmp/python_manifest-1.4.1-py3-none-any.whl.zip` & `tmp/python_manifest-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 20072 bytes, number of entries: 22
+Zip file size: 20074 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      230 b- defN 80-Jan-01 00:00 manifest/__init__.py
--rw-r--r--  2.0 unx    10821 b- defN 80-Jan-01 00:00 manifest/base.py
+-rw-r--r--  2.0 unx    10691 b- defN 80-Jan-01 00:00 manifest/base.py
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 manifest/hooks/__init__.py
 -rw-r--r--  2.0 unx      549 b- defN 80-Jan-01 00:00 manifest/hooks/builtin.py
 -rw-r--r--  2.0 unx      382 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/__init__.py
 -rw-r--r--  2.0 unx     4581 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/operations.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 manifest/hooks/expressions/resolve.py
 -rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 manifest/hooks/interface.py
--rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 manifest/instantiable.py
--rw-r--r--  2.0 unx    12327 b- defN 80-Jan-01 00:00 manifest/parse.py
+-rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 manifest/instantiable.py
+-rw-r--r--  2.0 unx    12323 b- defN 80-Jan-01 00:00 manifest/parse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 manifest/py.typed
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 manifest/serializers/__init__.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 manifest/serializers/base.py
 -rw-r--r--  2.0 unx      503 b- defN 80-Jan-01 00:00 manifest/serializers/jsons.py
 -rw-r--r--  2.0 unx      353 b- defN 80-Jan-01 00:00 manifest/serializers/noop.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 manifest/serializers/tomls.py
 -rw-r--r--  2.0 unx      350 b- defN 80-Jan-01 00:00 manifest/serializers/yamls.py
 -rw-r--r--  2.0 unx     8185 b- defN 80-Jan-01 00:00 manifest/utils.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5565 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-1.4.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1820 b- defN 16-Jan-01 00:00 python_manifest-1.4.1.dist-info/RECORD
-22 files, 55757 bytes uncompressed, 17112 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 python_manifest-2.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5564 b- defN 80-Jan-01 00:00 python_manifest-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 python_manifest-2.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1820 b- defN 16-Jan-01 00:00 python_manifest-2.0.0.dist-info/RECORD
+22 files, 55665 bytes uncompressed, 17114 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: manifest/serializers/yamls.py
 Comment: 
 
 Filename: manifest/utils.py
 Comment: 
 
-Filename: python_manifest-1.4.1.dist-info/LICENSE
+Filename: python_manifest-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: python_manifest-1.4.1.dist-info/METADATA
+Filename: python_manifest-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: python_manifest-1.4.1.dist-info/WHEEL
+Filename: python_manifest-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: python_manifest-1.4.1.dist-info/RECORD
+Filename: python_manifest-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## manifest/base.py

```diff
@@ -1,11 +1,11 @@
 import os
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from pathlib import Path
-from typing import TypeVar, Type, Any, Union, Mapping, AbstractSet, Callable, cast
+from typing import TypeVar, Type, Any, Callable, cast
 from dotenv import dotenv_values
 
 from manifest.parse import (
     parse_files,
     parse_key_values,
     parse_env_vars,
     dump_to_file,
@@ -17,53 +17,47 @@
     get_by_dot_path,
     set_by_dot_path,
     unset_by_dot_path
 )
 
 T = TypeVar("T", bound="Manifest")
 
-class Manifest(
-    BaseModel,
-    arbitrary_types_allowed=True,
-    validate_assignment=True
-):
+class Manifest(BaseModel):
+    model_config = ConfigDict(
+        {"arbitrary_types_allowed": True, "validate_assignment": True, "extra": "allow"}
+    )
+
     def normalize(
         self,
         *,
-        include: Union[AbstractSet[int | str], Mapping[int | str, Any], None] = None,
-        exclude: Union[AbstractSet[int | str], Mapping[int | str, Any], None] = None,
+        include: set[str] | set[int] | dict[int, Any] | dict[str, Any] | None = None,
+        exclude: set[str] | set[int] | dict[int, Any] | dict[str, Any] | None = None,
         by_alias: bool = True,
-        skip_defaults: bool | None = None,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
     ) -> dict[str, Any]:
         """
         Return a dictionary representation of the Manifest
         with the values coerced to basic types.
         """
-        model_dict = super().dict(
+        model_dict = super().model_dump(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
-            skip_defaults=skip_defaults,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
         return cast(dict, coerce_to_basic_types(model_dict))
 
     @property
     def extra_fields(self) -> dict[str, Any]:
         # Get any extra fields that were set but not defined in the model
-        return {
-            k: v
-            for k, v in self.__dict__.items()
-            if k not in type(self).__fields__.keys()
-        }
+        return self.__pydantic_extra__ or {}
 
     @classmethod
     async def build(
         cls: Type[T],
         files: list[str | Path] = [],
         dotenv_files: list[str] = [],
         key_values: list[str] = [],
@@ -255,15 +249,15 @@
 
         :param key: The key to set which looks like `a.b.c` for nested parameters
         :type key: str
         :param value: The value to set
         :type value: Any
         :return: A copy of the Manifest with the given key set to the given value
         """
-        return self.copy(
+        return self.model_copy(
             update=set_by_dot_path(
                 self.normalize(),
                 key,
                 value
             )
         )
```

## manifest/instantiable.py

```diff
@@ -1,22 +1,24 @@
 from typing import Generic, TypeVar, Any
-from pydantic import Field, validator, BaseModel
-from pydantic.generics import GenericModel
+from pydantic import Field, validator, BaseModel, ConfigDict
 
 from manifest.utils import import_from_string
 
 T = TypeVar("T")
 
 
-class Instantiable(Generic[T], GenericModel, extra='allow', allow_population_by_field_name=True):
+class Instantiable(BaseModel, Generic[T]):
     """
     Instantiable is a generic model that can be used to instantiate objects from a model. It
     requires that the model specify a `target` attribute, which is used to import the class, and the
     model's fields are used as keyword arguments to the class constructor.
     """
+    model_config = ConfigDict(
+        {"extra": "allow", "arbitrary_types_allowed": True, "populate_by_name": True}
+    )
     target: str = Field(alias="__target__")
 
     @validator("target", pre=True)
     def validate_target(cls, v: str) -> str:
         if not v:
             raise ValueError("target must be a non-empty string")
         return v
@@ -33,15 +35,15 @@
     :type model: BaseModel
     :param extra: Extra keyword arguments to pass to the object constructor.
     :type extra: dict
     :param skip: Whether to skip the target check.
     :type skip: bool
     :return: The instantiated object.
     """
-    object_info = model.copy()
+    object_info = model.model_copy()
 
     if not hasattr(object_info, "target") or not object_info.target:
         if skip:
             return object_info
         raise ValueError("`model` must specify a `target` attribute")
 
     target = import_from_string(object_info.target)
```

## manifest/parse.py

```diff
@@ -198,15 +198,15 @@
 
 
 async def load_from_file(
     file: str | Path,
     pre_process_hooks: list[Callable] = [],
     post_process_hooks: list[Callable] = [],
     default_serializer: Any = Undefined,
-    root_alias: str = "__root__",
+    root_alias: str = "root",
     **kwargs
 ) -> Any:
     """
     Parse a file by loading it, deserializing it, and returning the resulting dictionary.
 
     :param file: The path to the file to be parsed.
     :type file: str
```

## Comparing `python_manifest-1.4.1.dist-info/LICENSE` & `python_manifest-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `python_manifest-1.4.1.dist-info/METADATA` & `python_manifest-2.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: python-manifest
-Version: 1.4.1
+Version: 2.0.0
 Summary: A modern toolkit for working with application manifests and configurations.
 Home-page: https://github.com/emergentmethods/python-manifest
 License: MIT
 Author: Timothy Pogue
 Author-email: tim@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-rapidjson (>=1.10,<2.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/emergentmethods/python-manifest
 Description-Content-Type: text/markdown
```

## Comparing `python_manifest-1.4.1.dist-info/RECORD` & `python_manifest-2.0.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 manifest/__init__.py,sha256=lPR8D6XQ8nBPlRQEKelo78kQ0gMKANeprcMEZKRevwo,230
-manifest/base.py,sha256=uUGZG_F3ysyNFDMza-QzxgVtEZibERIIZaI2POQ7jOs,10821
+manifest/base.py,sha256=-jtu92f0z-X6cq0L42Do0iSRQ7aNLOKJdFQISdzUqM4,10691
 manifest/hooks/__init__.py,sha256=xGWUkgzWM7Dp_cMDvqk8bRzi9fiX8GYBzOcVmtWJwuo,460
 manifest/hooks/builtin.py,sha256=EqeD6B9BnA21MdVZiZ54Gz1w7hNnjMBkc64PIzKC-Zw,549
 manifest/hooks/expressions/__init__.py,sha256=hvVL1tr9aCSH7EFeph99CJvKWCP_V4m5KStZx9Hmsqw,382
 manifest/hooks/expressions/operations.py,sha256=PoVZ69D7MTrl5iWze34Gl10WA6sdH7l505T1jKQNiUU,4581
 manifest/hooks/expressions/resolve.py,sha256=VF0l2MTeGGVqCCjQEeFj0Dxqlbz4Hq_jX022Dr0gIu8,3238
 manifest/hooks/interface.py,sha256=xKE-3E3yUV4FuLJWPiMR5UCe6pa-cwSIoP4zK0zxzuM,2128
-manifest/instantiable.py,sha256=TlzW04amYQF26X_iqJU2MMsvplCMogUM6XTwljdwFcc,2085
-manifest/parse.py,sha256=ldOn4HRMcgORIhtMRShB8XxD1axoy9h-ZH-zMKyOHFM,12327
+manifest/instantiable.py,sha256=hAHQ_utXoalt4o8Sc3T4gId6NdMI-AqfwZaAwlrrWh4,2128
+manifest/parse.py,sha256=zBUJnkgZqPv2P7oYwSqHjDjGI7nEujF5kCxU-48cWY4,12323
 manifest/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 manifest/serializers/__init__.py,sha256=4d2mNeR4nZTdHC7Dg5ab7_whcXF_BsXvrhm8whJMeas,386
 manifest/serializers/base.py,sha256=So6sMP502D0fXN84Np0a_c5IGyq4gLWmMXfDwN6xAPg,272
 manifest/serializers/jsons.py,sha256=iK5Tswidrc3CLqeg4YaBNH7Ev6C7cVAQo6pEmDjncIM,503
 manifest/serializers/noop.py,sha256=x0sqDyLDFI-g6K5EnXUex3UVmwLvq-nMFoBj_iNpTys,353
 manifest/serializers/tomls.py,sha256=QxSGa4nWs3SqJAF-Y_64zGfEn_BgPOVs5-bxvS7X6Ro,356
 manifest/serializers/yamls.py,sha256=th77AOLV4I10t_SOLIlqQAsiSGzACzia71vGIi-1Cf0,350
 manifest/utils.py,sha256=C5LvlfKPvPEQwBQ7Uq_h4OPNjt-plquJff7qNdHtVHg,8185
-python_manifest-1.4.1.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
-python_manifest-1.4.1.dist-info/METADATA,sha256=p6gM0dWnVkDSXjTg9xS5bIHN8Ff9VNsGMf-ZtCQRYNE,5565
-python_manifest-1.4.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-python_manifest-1.4.1.dist-info/RECORD,,
+python_manifest-2.0.0.dist-info/LICENSE,sha256=DEqEB7tSTdQp6PHFAw4I1MyZU02bPaXoSULcNI_49bw,1078
+python_manifest-2.0.0.dist-info/METADATA,sha256=s7cxqMsTpKr-2wHpKy7ZxuKtBfLJEBOsHwiDvnvs8l0,5564
+python_manifest-2.0.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+python_manifest-2.0.0.dist-info/RECORD,,
```

