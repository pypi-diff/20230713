# Comparing `tmp/interval_sdk-1.4.4.tar.gz` & `tmp/interval_sdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.4.4.tar", max compression
+gzip compressed data, was "interval_sdk-1.5.0.tar", max compression
```

## Comparing `interval_sdk-1.4.4.tar` & `interval_sdk-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.4.4/README.md
--rw-r--r--   0        0        0     1890 2023-06-29 17:32:55.183140 interval_sdk-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-06-29 16:59:09.177636 interval_sdk-1.4.4/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7597 2023-06-05 17:42:55.806119 interval_sdk-1.4.4/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    61129 2023-06-05 17:42:55.806119 interval_sdk-1.4.4/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8970 2023-06-15 17:48:44.597413 interval_sdk-1.4.4/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      548 2023-06-05 17:42:55.806119 interval_sdk-1.4.4/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.4.4/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     8223 2023-06-29 17:30:26.574206 interval_sdk-1.4.4/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.4.4/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3468 2023-06-05 17:42:55.806119 interval_sdk-1.4.4/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.4.4/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.4.4/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.4.4/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.4.4/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    15453 2023-06-29 16:59:09.177636 interval_sdk-1.4.4/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    26126 2023-06-05 17:42:55.806119 interval_sdk-1.4.4/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    67369 2023-06-29 17:07:07.887509 interval_sdk-1.4.4/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.4.4/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.4.4/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.4.4/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.4.4/src/interval_sdk/util.py
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.4.4/setup.py
--rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     5078 2023-05-02 17:56:21.969548 interval_sdk-1.5.0/README.md
+-rw-r--r--   0        0        0     1890 2023-07-13 20:20:01.577979 interval_sdk-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      453 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7551 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    63769 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8970 2023-07-07 18:28:50.854385 interval_sdk-1.5.0/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      548 2023-06-05 17:42:55.806119 interval_sdk-1.5.0/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.5.0/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     8223 2023-07-11 18:23:33.895414 interval_sdk-1.5.0/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1162 2023-05-02 17:56:24.302863 interval_sdk-1.5.0/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3468 2023-06-05 17:42:55.806119 interval_sdk-1.5.0/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.5.0/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.5.0/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.5.0/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.5.0/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15654 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    26676 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    67612 2023-07-13 18:58:54.765524 interval_sdk-1.5.0/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.5.0/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5935 2023-05-02 17:56:24.302863 interval_sdk-1.5.0/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-28 17:09:46.534136 interval_sdk-1.5.0/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7342 2023-05-02 17:56:24.302863 interval_sdk-1.5.0/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.5.0/setup.py
+-rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.5.0/PKG-INFO
```

### Comparing `interval_sdk-1.4.4/README.md` & `interval_sdk-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/pyproject.toml` & `interval_sdk-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.4.4"
+version = "1.5.0"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/component.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,14 @@
             return_schema = Optional[return_schema]
 
         if value is None:
             if not self.instance.is_optional and self.schema.returns is not None:
                 raise ValueError("Received invalid None return value")
             return None
 
-        print("return_schema", return_schema)
         return parse_obj_as(return_schema, dict_keys_to_snake(value))
 
     def set_optional(self, optional: bool):
         self.instance.is_optional = optional
 
     def set_multiple(self, multiple: bool):
         self.instance.is_multiple = multiple
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/io.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,29 @@
     ButtonItemModel,
     CredentialsProps,
     CredentialsReturns,
     CurrencyCode,
     DeserializableRecordModel,
     DisplayGridProps,
     DisplayGridState,
+    DisplayHTMLProps,
     DisplayHeadingProps,
     DisplayTableState,
     FileState,
     FileUrlSet,
     GridItem,
     InputTextProps,
     InternalTableRow,
     MetaItemDefinition,
     MetaItemDefinitionModel,
     SelectTableReturnModel,
     SelectTableState,
     InputEmailProps,
     InputNumberProps,
+    InputSliderProps,
     InputBooleanProps,
     InputRichTextProps,
     InputUrlProps,
     DateModel,
     TableMenuItem,
     TimeModel,
     DateTimeModel,
@@ -274,14 +276,80 @@
                 if decimals is None:
                     return int(val)
 
                 return val
 
             return InputIOPromise(c, renderer=self._renderer, get_value=get_value)
 
+        @overload
+        def slider(
+            self,
+            label: str,
+            *,
+            min: int,
+            max: int,
+            step: Optional[int] = None,
+            help_text: Optional[str] = None,
+            default_value: Optional[int] = None,
+            disabled: Optional[bool] = None,
+        ) -> InputIOPromise[Literal["INPUT_SLIDER"], int]:
+            ...
+
+        @overload
+        def slider(
+            self,
+            label: str,
+            *,
+            min: Union[int, float],
+            max: Union[int, float],
+            step: Optional[Union[int, float]] = None,
+            help_text: Optional[str] = None,
+            default_value: Optional[Union[int, float]] = None,
+            disabled: Optional[bool] = None,
+        ) -> InputIOPromise[Literal["INPUT_SLIDER"], float]:
+            ...
+
+        def slider(
+            self,
+            label: str,
+            *,
+            min: Union[float, int],
+            max: Union[float, int],
+            step: Optional[Union[float, int]] = None,
+            help_text: Optional[str] = None,
+            default_value: Optional[Union[float, int]] = None,
+            disabled: Optional[bool] = None,
+        ):
+            c = Component(
+                method_name="INPUT_SLIDER",
+                label=label,
+                initial_props=InputSliderProps(
+                    min=min,
+                    max=max,
+                    step=step,
+                    help_text=help_text,
+                    default_value=default_value,
+                    disabled=disabled,
+                ),
+                display_resolves_immediately=self._display_resolves_immediately,
+            )
+
+            def get_value(val: float):
+                if (
+                    isinstance(min, int)
+                    and isinstance(max, int)
+                    and (step is None or isinstance(step, int))
+                    and (default_value is None or isinstance(default_value, int))
+                ):
+                    return int(val)
+
+                return val
+
+            return InputIOPromise(c, renderer=self._renderer, get_value=get_value)
+
         def boolean(
             self,
             label: str,
             *,
             help_text: Optional[str] = None,
             default_value: Optional[str] = None,
             disabled: Optional[bool] = None,
@@ -952,14 +1020,25 @@
                 method_name="DISPLAY_MARKDOWN",
                 label=label,
                 initial_props=None,
                 display_resolves_immediately=self._display_resolves_immediately,
             )
             return DisplayIOPromise(c, renderer=self._renderer)
 
+        def html(
+            self, label: str, *, html: str
+        ) -> DisplayIOPromise[Literal["DISPLAY_HTML"], None]:
+            c = Component(
+                method_name="DISPLAY_HTML",
+                label=label,
+                initial_props=DisplayHTMLProps(html=html),
+                display_resolves_immediately=self._display_resolves_immediately,
+            )
+            return DisplayIOPromise(c, renderer=self._renderer)
+
         def metadata(
             self,
             label: str,
             *,
             data: Iterable[MetaItemDefinition],
             layout: MetadataLayout = "grid",
         ) -> DisplayIOPromise[Literal["DISPLAY_METADATA"], None]:
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/io_client.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/io_error.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/io_error.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/isocket.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/layout.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/logger.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/page.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.5.0/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/components/grid.py` & `interval_sdk-1.5.0/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/components/table.py` & `interval_sdk-1.5.0/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/handlers.py` & `interval_sdk-1.5.0/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.5.0/src/interval_sdk/internal_rpc_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
 class ActionDefinition(BaseModel):
     group_slug: Optional[str] = None
     slug: str
     name: Optional[str] = None
     description: Optional[str] = None
     backgroundable: bool = False
+    warn_on_close: bool = True
     unlisted: bool = False
     access: Optional[AccessControlDefinition] = None
 
 
 class PageDefinition(BaseModel):
     slug: str
     name: str
@@ -371,25 +372,32 @@
 
 
 class IOResponseInputs(BaseModel):
     value: str
     transaction_id: str
 
 
+ContextUserRole: TypeAlias = Literal["admin", "developer", "member"]
+
+
 @dataclass
 class ContextUser:
     email: str
+    role: ContextUserRole
+    teams: list[str]
     first_name: Optional[str] = None
     last_name: Optional[str] = None
 
 
 class ContextUserModel(BaseModel):
     email: str
     first_name: Optional[str] = None
     last_name: Optional[str] = None
+    role: ContextUserRole
+    teams: list[str]
 
 
 @dataclass
 class ActionInfo:
     slug: str
     url: str
 
@@ -575,15 +583,15 @@
 
 
 class OpenPageInputs(BaseModel):
     page_key: str
     client_id: Optional[str] = None
     page: PageInfo
     environment: ActionEnvironment
-    user: ContextUser
+    user: ContextUserModel
     params: SerializableRecord
     params_meta: Optional[Any] = None
 
 
 class OpenPageReturnsSuccess(BaseModel):
     type: Literal["SUCCESS"] = "SUCCESS"
     page_key: str
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/io_schema.py` & `interval_sdk-1.5.0/src/interval_sdk/io_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 # TODO: Try generating most of this with datamode-code-generator
 # https://github.com/koxudaxi/datamodel-code-generator/
 
 InputMethodName = Literal[
     "INPUT_TEXT",
     "INPUT_EMAIL",
     "INPUT_NUMBER",
+    "INPUT_SLIDER",
     "INPUT_BOOLEAN",
     "INPUT_RICH_TEXT",
     "INPUT_SPREADSHEET",
     "INPUT_URL",
     "INPUT_DATE",
     "INPUT_TIME",
     "INPUT_DATETIME",
@@ -72,14 +73,15 @@
 
 DisplayMethodName = Literal[
     "DISPLAY_CODE",
     "DISPLAY_HEADING",
     "DISPLAY_IMAGE",
     "DISPLAY_LINK",
     "DISPLAY_MARKDOWN",
+    "DISPLAY_HTML",
     "DISPLAY_METADATA",
     "DISPLAY_OBJECT",
     "DISPLAY_GRID",
     "DISPLAY_TABLE",
     "DISPLAY_VIDEO",
     "DISPLAY_PROGRESS_STEPS",
     "DISPLAY_PROGRESS_INDETERMINATE",
@@ -526,14 +528,23 @@
     placeholder: Optional[str]
     default_value: Optional[Union[float, int]]
     decimals: Optional[int]
     currency: Optional[CurrencyCode]
     disabled: Optional[bool]
 
 
+class InputSliderProps(BaseModel):
+    min: Union[float, int]
+    max: Union[float, int]
+    step: Optional[Union[float, int]]
+    help_text: Optional[str]
+    default_value: Optional[Union[float, int]]
+    disabled: Optional[bool]
+
+
 class InputBooleanProps(BaseModel):
     help_text: Optional[str]
     default_value: Optional[str]
     disabled: Optional[bool]
 
 
 class InputRichTextProps(BaseModel):
@@ -701,14 +712,18 @@
     image: Optional[ImageDefinitionModel] = None
     route: Optional[str] = None
     params: Optional[SerializableRecord] = None
     # private prop
     error: Optional[str] = None
 
 
+class DisplayHTMLProps(BaseModel):
+    html: str
+
+
 class DisplayMetadataProps(BaseModel):
     data: list[MetaItemDefinitionModel]
     layout: MetadataLayout
 
 
 class DisplayObjectProps(BaseModel):
     data: KeyValueObjectModel
@@ -805,14 +820,19 @@
         returns=str,
     ),
     "INPUT_NUMBER": MethodDef(
         props=InputNumberProps,
         state=None,
         returns=float,
     ),
+    "INPUT_SLIDER": MethodDef(
+        props=InputSliderProps,
+        state=None,
+        returns=float,
+    ),
     "INPUT_BOOLEAN": MethodDef(
         props=InputBooleanProps,
         state=None,
         returns=bool,
     ),
     "INPUT_RICH_TEXT": MethodDef(
         props=InputRichTextProps,
@@ -907,14 +927,19 @@
         returns=None,
     ),
     "DISPLAY_MARKDOWN": MethodDef(
         props={},
         state=None,
         returns=None,
     ),
+    "DISPLAY_HTML": MethodDef(
+        props=DisplayHTMLProps,
+        state=None,
+        returns=None,
+    ),
     "DISPLAY_METADATA": MethodDef(
         props=DisplayMetadataProps,
         state=None,
         returns=None,
     ),
     "DISPLAY_IMAGE": MethodDef(
         props=DisplayImageProps,
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/main.py` & `interval_sdk-1.5.0/src/interval_sdk/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,15 @@
                     action_definitions.append(
                         ActionDefinition(
                             group_slug=group_slug,
                             slug=slug,
                             name=route.name,
                             description=route.description,
                             backgroundable=route.backgroundable,
+                            warn_on_close=route.warn_on_close,
                             unlisted=route.unlisted,
                             access=route.access,
                         )
                     )
 
                     action_handlers[f"{group_slug}/{slug}"] = route.handler
 
@@ -297,14 +298,15 @@
             else:
                 action_definitions.append(
                     ActionDefinition(
                         slug=slug,
                         name=route.name,
                         description=route.description,
                         backgroundable=route.backgroundable,
+                        warn_on_close=route.warn_on_close,
                         unlisted=route.unlisted,
                         access=route.access,
                     )
                 )
 
                 action_handlers[slug] = route.handler
 
@@ -317,14 +319,15 @@
         self,
         handler_or_slug: Optional[Union[IntervalActionHandler, str]] = None,
         *,
         slug: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
         backgroundable: bool = False,
+        warn_on_close: bool = True,
         unlisted: bool = False,
         access: Optional[AccessControlDefinition] = None,
     ) -> Callable[[IntervalActionHandler], IntervalActionHandler]:
         def action_adder(handler: IntervalActionHandler):
             self.routes.add(
                 slug
                 if slug is not None
@@ -332,14 +335,15 @@
                 if (handler_or_slug is not None and isinstance(handler_or_slug, str))
                 else handler.__name__,
                 Action(
                     handler=handler,
                     name=name,
                     description=description,
                     backgroundable=backgroundable,
+                    warn_on_close=warn_on_close,
                     unlisted=unlisted,
                     access=access,
                 ),
             )
             return handler
 
         if handler_or_slug is not None and isfunction(handler_or_slug):
@@ -1103,15 +1107,15 @@
             params = inputs.params
             if params is not None and inputs.params_meta is not None:
                 params = superjson.deserialize(params, inputs.params_meta)
 
             page_ctx = PageContext(
                 page_key=inputs.page_key,
                 logger=self._logger,
-                user=inputs.user,
+                user=ContextUser(**inputs.user.dict(by_alias=False)),
                 params=deserialize_dates(inputs.params),
                 environment=inputs.environment,
                 organization=self.organization,
                 page=inputs.page,
                 send_redirect=self._send_redirect,
                 loading=TransactionLoadingState(
                     logger=self._logger,
```

### Comparing `interval_sdk-1.4.4/src/interval_sdk/superjson/main.py` & `interval_sdk-1.5.0/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.5.0/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.5.0/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.5.0/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/types.py` & `interval_sdk-1.5.0/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/src/interval_sdk/util.py` & `interval_sdk-1.5.0/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.4.4/setup.py` & `interval_sdk-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.4.4',
+    'version': '1.5.0',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '<a href="https://interval.com">\n  <img alt="Interval" width="100" height="100" style="border-radius: 6px;" src="https://interval.com/img/readme-assets/interval-avatar.png">\n</a>\n\n# Interval Python SDK\n\n[![pypi version](https://img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/twitter/follow/useinterval.svg?color=%2338A1F3&label=twitter&style=flat)](https://twitter.com/useinterval) [![Discord](https://img.shields.io/badge/discord-join-blueviolet)](https://interval.com/discord)\n\n[Interval](https://interval.com) lets you quickly build internal web apps (think: customer support tools, admin panels, etc.) just by writing backend Python code.\n\nThis is our Python SDK which connects to the interval.com web app. If you don\'t have an Interval account, you can [create one here](https://interval.com/signup). All core features are free to use.\n\n## Why choose Interval?\n\n_"Python code > no-code"_\n\nInterval is an alternative to no-code/low-code UI builders. Modern frontend development is inherently complicated, and teams rightfully want to spend minimal engineering resources on internal dashboards. No-code tools attempt to solve this problem by allowing you to build UIs in a web browser without writing any frontend code.\n\nWe don\'t think this is the right solution. **Building UIs for mission-critical tools in your web browser** — often by non-technical teammates, outside of your codebase, without versioning or code review — **is an anti-pattern.** Apps built in this manner are brittle and break in unexpected ways.\n\nWith Interval, **all of the code for generating your web UIs lives within your app\'s codebase.** Tools built with Interval (we call these [actions](https://interval.com/docs/concepts/actions)) are just asynchronous functions that run in your backend. Because these are plain old functions, you can access the complete power of your Python app. You can loop, conditionally branch, access shared functions, and so on. When you need to request input or display output, `await` any of our [I/O methods](https://interval.com/docs/io-methods/) to present a form to the user and your script will pause execution until input is received.\n\nHere\'s a simple app with a single "Hello, world" action:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval(api_key="<YOUR API KEY>")\n\n@interval.action\nasync def hello_world(io: IO):\n    name = await io.input.text("Your name")\n    return f"Hello, {name}"\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\nInterval:\n\n- Makes creating full-stack apps as easy as writing CLI scripts.\n- Can scale from a handful of scripts to robust multi-user dashboards.\n- Lets you build faster than no-code, without leaving your codebase & IDE.\n\nWith Interval, you do not need to:\n\n- Write REST or GraphQL API endpoints to connect internal functionality to no-code tools.\n- Give Interval write access to your database (or give us _any_ of your credentials, for that matter).\n- Build web UIs with a drag-and-drop interface.\n\n## More about Interval\n\n- 📖 [Documentation](https://interval.com/docs)\n- 🌐 [Interval website](https://interval.com)\n- 💬 [Discord community](https://interval.com/discord)\n- 📰 [Product updates](https://interval.com/blog)\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['interval_sdk', 'interval_sdk.classes',
 'interval_sdk.components', 'interval_sdk.superjson',
 'interval_sdk.superjson.tests'] package_data = \ {'': ['*']} install_requires =
 \ ['aiohttp>=3.8.1,<4.0.0', 'pydantic>=1.9.0,<2.0.0', 'typing-
 extensions>=4.4.0,<5.0.0', 'websockets>=10.1,<11.0'] setup_kwargs = { 'name':
-'interval-sdk', 'version': '1.4.4', 'description': "The frontendless framework
+'interval-sdk', 'version': '1.5.0', 'description': "The frontendless framework
 for high growth companies. Interval automatically generates apps by inlining
 the UI in your backend code. It's a faster and more maintainable way to build
 internal tools, rapid prototypes, and more.", 'long_description': '\n_
 [Interval]\n\n\n# Interval Python SDK\n\n[![pypi version](https://
 img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/
 interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-
 informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/
```

### Comparing `interval_sdk-1.4.4/PKG-INFO` & `interval_sdk-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.4.4
+Version: 1.5.0
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: interval-sdk Version: 1.4.4 Summary: The
+Metadata-Version: 2.1 Name: interval-sdk Version: 1.5.0 Summary: The
 frontendless framework for high growth companies. Interval automatically
 generates apps by inlining the UI in your backend code. It's a faster and more
 maintainable way to build internal tools, rapid prototypes, and more. Home-
 page: https://interval.com Keywords: internal tool,app,ui,ui builder Author:
 Jacob Mischka Author-email: jacob@interval.com Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

