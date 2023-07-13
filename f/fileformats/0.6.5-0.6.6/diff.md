# Comparing `tmp/fileformats-0.6.5.tar.gz` & `tmp/fileformats-0.6.6.tar.gz`

## Comparing `fileformats-0.6.5.tar` & `fileformats-0.6.6.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/_version.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/converter.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/datatype.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/field.py
--rw-r--r--   0        0        0    42571 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/fileset.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/mark.py
--rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/mixin.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.5/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.5/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.5/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.5/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.5/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.5/pyproject.toml
--rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/field.py
+-rw-r--r--   0        0        0    42563 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/converters.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/headers.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.6/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.6/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.6/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.6/README.rst
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 fileformats-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0    22460 2020-02-02 00:00:00.000000 fileformats-0.6.6/PKG-INFO
```

### Comparing `fileformats-0.6.5/fileformats/archive/__init__.py` & `fileformats-0.6.6/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/archive/converters.py` & `fileformats-0.6.6/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.6/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/audio/__init__.py` & `fileformats-0.6.6/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/converter.py` & `fileformats-0.6.6/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/datatype.py` & `fileformats-0.6.6/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/field.py` & `fileformats-0.6.6/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/fileset.py` & `fileformats-0.6.6/fileformats/core/fileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     # Store converters registered by @converter decorator that convert to FileSet
     # NB: each class will have its own version of this dictionary
     converters = {}
 
     is_fileset = True
 
     def __hash__(self):
-        return hash(sorted(self.fspaths))
+        return hash(self.fspaths)
 
     def __repr__(self):
         return (
             f"{type(self).__name__}('"
             + "', '".join(str(p) for p in self.fspaths)
             + "')"
         )
```

### Comparing `fileformats-0.6.5/fileformats/core/mark.py` & `fileformats-0.6.6/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/mixin.py` & `fileformats-0.6.6/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/utils.py` & `fileformats-0.6.6/fileformats/core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,34 @@
     FileFormatsError,
 )
 import fileformats.core
 
 logger = logging.getLogger("fileformats")
 
 
+_excluded_subpackages = set(["core", "testing"])
+
+
+def include_testing_package(flag: bool = True):
+    """Include testing package in list of sub-packages. Typically set in conftest.py
+    or similar when setting up unittesting. Must be set globally before any methods are
+    called within the package as member classes are cached.
+
+    Parameters
+    ----------
+    flag : bool
+        whether to include the testing package or not
+    """
+    global _excluded_subpackages
+    if flag:
+        _excluded_subpackages.remove("testing")
+    else:
+        _excluded_subpackages.add("testing")
+
+
 def find_matching(
     fspaths: ty.List[Path], standard_only: bool = False, include_generic: bool = False
 ):
     """Detect the corresponding file format from a set of file-system paths
 
     Parameters
     ----------
@@ -45,26 +65,31 @@
     return matches
 
 
 def from_mime(mime_str: str):
     return fileformats.core.DataType.from_mime(mime_str)
 
 
-def subpackages():
+def subpackages(exclude: ty.Sequence[str] = _excluded_subpackages):
     """Iterates over all subpackages within the fileformats namespace
 
+    Parameters
+    ----------
+    exclude : ty.Sequence[str], optional
+        whether to include the testing subpackage, by default ["core", "testing"]
+
     Yields
     ------
     module
         all modules within the package
     """
     for mod_info in pkgutil.iter_modules(
         fileformats.__path__, prefix=fileformats.__package__ + "."
     ):
-        if mod_info.name == "core":
+        if mod_info.name.split(".")[-1] in exclude:
             continue
         yield importlib.import_module(mod_info.name)
 
 
 @contextmanager
 def set_cwd(path: Path):
     """Sets the current working directory to `path` and back to original
@@ -172,48 +197,14 @@
     format_name = format_name.capitalize()
     format_name = re.sub(r"(\.)(\w)", lambda m: "_" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(\+)(\w)", lambda m: "__" + m.group(2).upper(), format_name)
     format_name = re.sub(r"(-)(\w)", lambda m: m.group(2).upper(), format_name)
     return format_name
 
 
-# def hash_file(fspath: Path, chunk_len: int, crypto: ty.Callable):
-#     crypto_obj = crypto()
-#     with open(fspath, "rb") as fp:
-#         for chunk in iter(lambda: fp.read(chunk_len), b""):
-#             crypto_obj.update(chunk)
-#     return crypto_obj.hexdigest()
-
-
-# def hash_dir(
-#     fspath: Path,
-#     chunk_len: int,
-#     crypto: ty.Callable,
-#     ignore_hidden_files: bool = False,
-#     ignore_hidden_dirs: bool = False,
-#     relative_to: ty.Optional[Path] = None,
-# ):
-#     if relative_to is None:
-#         relative_to = fspath
-#     file_hashes = {}
-#     for dpath, _, filenames in sorted(os.walk(fspath)):
-#         # Sort in-place to guarantee order.
-#         filenames.sort()
-#         dpath = Path(dpath)
-#         if ignore_hidden_dirs and dpath.name.startswith(".") and str(dpath) != fspath:
-#             continue
-#         for filename in filenames:
-#             if ignore_hidden_files and filename.startswith("."):
-#                 continue
-#             file_hashes[str((dpath / filename).relative_to(relative_to))] = hash_file(
-#                 dpath / filename, crypto=crypto, chunk_len=chunk_len
-#             )
-#     return file_hashes
-
-
 def add_exc_note(e, note):
     """Adds a note to an exception in a Python <3.11 compatible way
 
     Parameters
     ----------
     e : Exception
         the exception to add the note to
```

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.6/fileformats/core/tests/test_classifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     with pytest.raises(FormatConversionError):
         L[C, D].get_converter(K[C, D])
 
     L[C, A].get_converter(K[A, C, B])
     L[C, A].get_converter(K[A, E, B])  # E is a subtype of C
 
 
-def test_mime_rountrips():
+def test_mime_roundtrips():
     assert DirectoryContaining[F].mime_like == "testing/f+directory-containing"
     assert from_mime("testing/f+directory-containing") is DirectoryContaining[F]
 
     # Directory is unordered so sort classifiers to create unique mime
     assert DirectoryContaining[H, F].mime_like == "testing/f.h+directory-containing"
     assert from_mime("testing/f.h+directory-containing") is DirectoryContaining[F, H]
```

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_converter.py` & `fileformats-0.6.6/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_detection.py` & `fileformats-0.6.6/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_mime.py` & `fileformats-0.6.6/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.6/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/core/tests/test_utils.py` & `fileformats-0.6.6/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/document/__init__.py` & `fileformats-0.6.6/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/field/__init__.py` & `fileformats-0.6.6/fileformats/field/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import typing as ty
 import attrs
 from fileformats.core import Field
 from fileformats.core.mixin import WithClassifiers
 from fileformats.core.exceptions import FormatMismatchError
 
 
-@attrs.define
 class Singular(Field):
     pass
 
 
 class LogicalMixin:
     def __bool__(self):
         return bool(self.value)
@@ -108,30 +107,33 @@
 
 def array_converter(value):
     if isinstance(value, str):
         if value.startswith("[") and value.endswith("]"):
             value = value[1:-1]
         elif value.startswith("[") or value.endswith("]"):
             raise FormatMismatchError(f"Unmatched brackets in array field {value}")
-        value = [v.strip() for v in value.split(",")]
+        value = tuple(v.strip() for v in value.split(","))
     else:
         try:
-            value = list(value)
+            value = tuple(value)
         except ValueError as e:
             raise FormatMismatchError(str(e)) from None
     return value
 
 
 @attrs.define
 class Text(Singular):
 
     value: str = attrs.field(converter=text_converter)
 
     primitive = str
 
+    def __hash__(self):
+        return hash(self.value)
+
 
 @attrs.define
 class Integer(Singular, ScalarMixin):
 
     value: int = attrs.field(converter=integer_converter)
 
     primitive = int
@@ -141,60 +143,69 @@
 
     def __float__(self):
         return float(self.value)
 
     def __bool__(self):
         return bool(self.value)
 
+    def __hash__(self):
+        return hash(self.value)
+
 
 @attrs.define
 class Decimal(Singular, ScalarMixin):
 
     value: decimal.Decimal = attrs.field(converter=decimal_converter)
 
     primitive = float
 
     def __float__(self):
         return float(self.value)
 
     def __bool__(self):
         return bool(self.value)
 
+    def __hash__(self):
+        return hash(self.value)
+
 
 @attrs.define
 class Boolean(Singular, LogicalMixin):
 
     primitive = bool
 
     value: bool = attrs.field(converter=boolean_converter)
 
     def __str__(self):
         return str(self.value).lower()
 
     def __bool__(self):
         return self.value
 
+    def __hash__(self):
+        return hash(self.value)
+
 
 @attrs.define(auto_attribs=False)
 class Array(WithClassifiers, Field):
 
     # WithClassifiers class attrs
     classifiers_attr_name: str = "item_type"
     multiple_classifiers: bool = False
     allowed_classifiers: ty.Tuple[ty.Type[Singular]] = (Singular,)
     item_type: ty.Union[ty.Type[Singular], None] = None
 
-    primitive = list
+    primitive = tuple
 
-    value: list = attrs.field(converter=array_converter)
+    value: tuple = attrs.field(converter=array_converter)
 
     def __attrs_post_init__(self):
         # Ensure items are of the correct type
         if self.item_type is not None:
-            self.value = [self.item_type(i).value for i in self.value]
+            self.value = tuple(self.item_type(i).value for i in self.value)
 
     def __str__(self):
         return (
             "["
             + ",".join(
                 str(self.item_type(i))
                 if self.item_type is not None
@@ -202,7 +213,10 @@
                 for i in self.value
             )
             + "]"
         )
 
     def __iter__(self):
         return iter(self.value)
+
+    def __hash__(self):
+        return hash(self.value)
```

### Comparing `fileformats-0.6.5/fileformats/field/tests/test_fields.py` & `fileformats-0.6.6/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.6/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/generic/__init__.py` & `fileformats-0.6.6/fileformats/generic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from fileformats.core.fileset import FileSet
 from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
 from fileformats.core import mark
 from fileformats.core.utils import classproperty
 from fileformats.core.mixin import WithClassifiers
 
 
-@attrs.define
 class FsObject(FileSet, os.PathLike):
     "Generic file-system object, can be either a file or a directory"
 
     @mark.required
     @property
     def fspath(self):
         if len(self.fspaths) > 1:
@@ -31,15 +30,14 @@
         return str(self)
 
     @property
     def stem(self):
         return self.fspath.with_suffix("").name
 
 
-@attrs.define
 class File(FsObject):
     """Generic file type"""
 
     binary = False
     is_dir = False
 
     @mark.required
@@ -138,15 +136,14 @@
         if self.actual_ext:
             stem = self.fspath.name[: -len(self.actual_ext)]
         else:
             stem = self.fspath
         return stem
 
 
-@attrs.define
 class Directory(FsObject):
     """Base directory to be overridden by subtypes that represent directories but don't
     want to inherit content type "qualifers" (i.e. most of them)"""
 
     is_dir = True
 
     content_types = ()
```

### Comparing `fileformats-0.6.5/fileformats/image/converters.py` & `fileformats-0.6.6/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/image/raster.py` & `fileformats-0.6.6/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.6/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.6/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/serialization/__init__.py` & `fileformats-0.6.6/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/serialization/converters.py` & `fileformats-0.6.6/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.6/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/fileformats/text/__init__.py` & `fileformats-0.6.6/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/LICENSE` & `fileformats-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/README.rst` & `fileformats-0.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.5/pyproject.toml` & `fileformats-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "fileformats[extended]",
     "fileformats[test]",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
-    "fileformats-testing",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
```

### Comparing `fileformats-0.6.5/PKG-INFO` & `fileformats-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.5
+Version: 0.6.6
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -132,15 +132,14 @@
 Requires-Dist: sphinx-click>=3.1; extra == 'docs'
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
 Provides-Extra: extended
 Requires-Dist: imageio>=2.24.0; extra == 'extended'
 Requires-Dist: pydra>=0.20.0; extra == 'extended'
 Requires-Dist: pyyaml>=6.0; extra == 'extended'
 Provides-Extra: test
-Requires-Dist: fileformats-testing; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats
 ===========
```

