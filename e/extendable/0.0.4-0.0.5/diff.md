# Comparing `tmp/extendable-0.0.4.tar.gz` & `tmp/extendable-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extendable-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "extendable-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `extendable-0.0.4.tar` & `extendable-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1081 2021-12-20 15:39:04.562356 extendable-0.0.4/LICENSE
--rw-r--r--   0        0        0     3245 2022-06-15 14:05:15.059085 extendable-0.0.4/README.md
--rw-r--r--   0        0        0     1457 2022-06-15 14:16:33.525761 extendable-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      393 2021-12-24 12:52:24.034138 extendable-0.0.4/src/extendable/__init__.py
--rw-r--r--   0        0        0      298 2021-12-22 17:48:19.539244 extendable-0.0.4/src/extendable/context.py
--rw-r--r--   0        0        0     9093 2023-06-26 08:24:33.249690 extendable-0.0.4/src/extendable/main.py
--rw-r--r--   0        0        0        0 2021-12-27 11:01:43.563093 extendable-0.0.4/src/extendable/py.typed
--rw-r--r--   0        0        0     8193 2023-06-26 08:24:33.249690 extendable-0.0.4/src/extendable/registry.py
--rw-r--r--   0        0        0     1059 2021-12-22 18:05:10.232479 extendable-0.0.4/src/extendable/utils.py
--rw-r--r--   0        0        0       22 2023-06-26 08:25:35.874619 extendable-0.0.4/src/extendable/version.py
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-13 15:24:28.911025 extendable-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3245 2023-07-13 15:24:28.911025 extendable-0.0.5/README.md
+-rw-r--r--   0        0        0     1457 2023-07-13 15:24:28.911025 extendable-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      393 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/__init__.py
+-rw-r--r--   0        0        0      298 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/context.py
+-rw-r--r--   0        0        0     9418 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/main.py
+-rw-r--r--   0        0        0        0 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/py.typed
+-rw-r--r--   0        0        0     8212 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/registry.py
+-rw-r--r--   0        0        0     1059 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/utils.py
+-rw-r--r--   0        0        0       22 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/version.py
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-0.0.5/PKG-INFO
```

### Comparing `extendable-0.0.4/LICENSE` & `extendable-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable-0.0.4/README.md` & `extendable-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `extendable-0.0.4/pyproject.toml` & `extendable-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable-0.0.4/src/extendable/main.py` & `extendable-0.0.5/src/extendable/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,32 @@
     base_names: List[str]
     namespace: Dict[str, Any]
     original_name: str
     others_bases: List[Any]
     hierarchy: List["ExtendableClassDef"]
     metaclass: "ExtendableMeta"
     original_cls: Type["ExtendableMeta"]
+    kwargs: Dict[str, Any]
 
     def __init__(
         self,
         original_name: str,
         bases: List[Any],
         namespace: Dict[str, Any],
         metaclass: "ExtendableMeta",
+        kwargs: Dict[str, Any],
     ) -> None:
         self.namespace = namespace
         self.name = namespace["__xreg_name__"]
         self.original_name = original_name
         self.others_bases = bases
         self.base_names = namespace["__xreg_base_names__"] or []
         self.hierarchy = [self]
         self.metaclass = metaclass
+        self.kwargs = kwargs
 
     def add_child(self, cls_def: "ExtendableClassDef") -> None:
         self.hierarchy.append(cls_def)
         for name in cls_def.base_names:
             if name not in self.base_names:
                 self.base_names.append(name)
 
@@ -65,15 +68,19 @@
 
         This is used to allow to recompute the registry from scratch by
         starting from the original class definition. This definition is
         then modified by the build process to define the class
         hierarchy.
         """
         clone = ExtendableClassDef(
-            self.original_name, self.others_bases, self.namespace, self.metaclass
+            self.original_name,
+            self.others_bases,
+            self.namespace,
+            self.metaclass,
+            self.kwargs,
         )
         clone.original_cls = self.original_cls
         return clone
 
 
 _extendable_class_defs_by_module: OrderedDict[
     str, List[ExtendableClassDef]
@@ -150,16 +157,17 @@
         # we are into the loading process of original Extendable
         # For each defined Extendable class, we keep a copy of the class
         # definition. This copy will be used to create the aggregated class
         other_bases = [b for b in bases if not metacls._is_extendable(b)]
         cls_def = ExtendableClassDef(
             original_name=name,
             bases=tuple(other_bases),
-            namespace=namespace,
+            namespace=namespace.copy(),
             metaclass=metacls,
+            kwargs=kwargs,
         )
         __register_class_def__(
             namespace["__module__"],
             cls_def,
         )
         return cls_def
 
@@ -187,17 +195,20 @@
                 @no_type_check
                 def new_method(
                     cls, *args, _method_name=None, _initial_func=None, **kwargs
                 ):
                     # ensure that arggs and kwargs are conform to the
                     # initial signature
                     inspect.signature(_initial_func).bind(cls, *args, **kwargs)
-                    return getattr(cls._get_assembled_cls(), _method_name)(
-                        *args, **kwargs
-                    )
+                    try:
+                        return getattr(cls._get_assembled_cls(), _method_name)(
+                            *args, **kwargs
+                        )
+                    except KeyError:
+                        return _initial_func(cls, *args, **kwargs)
 
                 new_method_def = functools.partial(
                     new_method, _method_name=key, _initial_func=func
                 )
                 # preserve signature for IDE
                 functools.update_wrapper(new_method_def, func)
                 new_namespace[key] = classmethod(new_method_def)
```

### Comparing `extendable-0.0.4/src/extendable/registry.py` & `extendable-0.0.5/src/extendable/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     "_is_aggregated_class": True,
                     "_original_cls": cls_def.original_cls,
                 }
             )
             extendableClass = types.new_class(
                 simple_name,
                 tuple(bases),
-                kwds={"metaclass": cls_def.metaclass},
+                kwds=dict(class_def.kwargs, metaclass=cls_def.metaclass),
                 exec_body=(
                     lambda ns, namespace=namespace: ns.update(namespace)  # type: ignore
                 ),
             )
             base = cast(main.ExtendableMeta, extendableClass)
             self[name] = base
         base.__xreg_all_base_names__ = set(class_def.base_names)
```

### Comparing `extendable-0.0.4/src/extendable/utils.py` & `extendable-0.0.5/src/extendable/utils.py`

 * *Files identical despite different names*

### Comparing `extendable-0.0.4/PKG-INFO` & `extendable-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable
-Version: 0.0.4
+Version: 0.0.5
 Summary: A lib to define class extendable at runtime.
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

