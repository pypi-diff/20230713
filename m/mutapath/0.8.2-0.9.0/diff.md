# Comparing `tmp/mutapath-0.8.2.tar.gz` & `tmp/mutapath-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mutapath-0.8.2.tar", last modified: Wed Oct 16 20:00:18 2019, max compression
+gzip compressed data, was "dist/mutapath-0.9.0.tar", last modified: Fri Oct 18 00:01:01 2019, max compression
```

## Comparing `mutapath-0.8.2.tar` & `mutapath-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-16 20:00:18.000000 mutapath-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4593 2019-10-16 20:00:18.000000 mutapath-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3184 2019-10-16 19:59:58.000000 mutapath-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2346 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/decorator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      139 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16766 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/immutapath.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/lock_dummy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2019-10-16 19:59:58.000000 mutapath-0.8.2/mutapath/mutapath.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4593 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      426 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2019-10-16 20:00:18.000000 mutapath-0.8.2/mutapath.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2019-10-16 20:00:18.000000 mutapath-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2019-10-16 19:59:58.000000 mutapath-0.8.2/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-16 20:00:18.000000 mutapath-0.8.2/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-10-16 19:59:58.000000 mutapath-0.8.2/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1503 2019-10-16 19:59:58.000000 mutapath-0.8.2/tests/helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6233 2019-10-16 19:59:58.000000 mutapath-0.8.2/tests/test_immutapath.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5692 2019-10-16 19:59:58.000000 mutapath-0.8.2/tests/test_mutapath.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6489 2019-10-16 19:59:58.000000 mutapath-0.8.2/tests/test_with_path.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-18 00:01:01.000000 mutapath-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4769 2019-10-18 00:01:01.000000 mutapath-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3297 2019-10-18 00:00:28.000000 mutapath-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/decorator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      139 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16338 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/immutapath.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/lock_dummy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1145 2019-10-18 00:00:28.000000 mutapath-0.9.0/mutapath/mutapath.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4769 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      426 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       72 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       15 2019-10-18 00:01:01.000000 mutapath-0.9.0/mutapath.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      103 2019-10-18 00:01:01.000000 mutapath-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1482 2019-10-18 00:00:28.000000 mutapath-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2019-10-18 00:01:01.000000 mutapath-0.9.0/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2019-10-18 00:00:28.000000 mutapath-0.9.0/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1503 2019-10-18 00:00:28.000000 mutapath-0.9.0/tests/helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6233 2019-10-18 00:00:28.000000 mutapath-0.9.0/tests/test_immutapath.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5692 2019-10-18 00:00:28.000000 mutapath-0.9.0/tests/test_mutapath.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6489 2019-10-18 00:00:28.000000 mutapath-0.9.0/tests/test_with_path.py
```

### Comparing `mutapath-0.8.2/PKG-INFO` & `mutapath-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutapath
-Version: 0.8.2
+Version: 0.9.0
 Summary: Mutable Pathlib
 Home-page: https://github.com/matfax/mutapath
 Author: matfax
 Author-email: matthias.fax@gmail.com
 License: lgpl-3.0
 Description: # mutapath
         
@@ -24,86 +24,92 @@
         
         ## MutaPath Class
         
         The MutaPath Class allows direct manipulation of its attributes at any time, just as any mutable object.
         Once a file operation is called that is intended to modify its path, the underlying path is also mutated.
         
         ```python
-        
         >>> from mutapath import MutaPath
-        
+        ```
+        ```python
         >>> folder = MutaPath("/home/joe/doe/folder/sub")
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> folder.name = "top"
         >>> folder
         Path('/home/joe/doe/folder/top')
-        
+        ```
+        ```python
         >>> next = MutaPath("/home/joe/doe/folder/next")
         >>> next
         Path('/home/joe/doe/folder/next')
-        
+        ```
+        ```python
         >>> next.rename(folder)
         >>> next
         Path('/home/joe/doe/folder/top')
         >>> next.exists()
         True
         >>> Path('/home/joe/doe/folder/sub').exists()
         False
-        
         ```
         
         ## Path Class
         
         This class is immutable by default, just as the `pathlib.Path`. However, it allows to open a editing context via `mutate()`.
         Moreover, there are additional contexts for file operations. They update the file and its path while closing the context.
         If the file operations don't succeed, they throw an exception and fall back to the original path value.
         
         ```python
-        
         >>> from mutapath import Path
-        
+        ```
+        ```python
         >>> folder = Path("/home/joe/doe/folder/sub")
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> folder.name = "top"
         AttributeError: mutapath.Path is an immutable class, unless mutate() context is used.
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> with folder.mutate() as m:
         ...     m.name = "top"
         >>> folder
         Path('/home/joe/doe/folder/top')
-        
+        ```
+        ```python
         >>> next = Path("/home/joe/doe/folder/next")
         >>> next.copy(folder)
         >>> next
         Path('/home/joe/doe/folder/next')
         >>> folder.exists()
         True
         >>> folder.remove()
-        
+        ```
+        ```python
         >>> with next.renaming() as m:
         ...     m.stem = folder.stem
         ...     m.suffix = ".txt"
         >>> next
         Path("/home/joe/doe/folder/sub.txt")
         >>> next.exists()
         True
         >>> next.with_name("next").exists()
         False
-        
         ```
         
 Keywords: pathlib,mutable,path
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mutapath-0.8.2/README.md` & `mutapath-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,75 +16,80 @@
 
 ## MutaPath Class
 
 The MutaPath Class allows direct manipulation of its attributes at any time, just as any mutable object.
 Once a file operation is called that is intended to modify its path, the underlying path is also mutated.
 
 ```python
-
 >>> from mutapath import MutaPath
-
+```
+```python
 >>> folder = MutaPath("/home/joe/doe/folder/sub")
 >>> folder
 Path('/home/joe/doe/folder/sub')
-
+```
+```python
 >>> folder.name = "top"
 >>> folder
 Path('/home/joe/doe/folder/top')
-
+```
+```python
 >>> next = MutaPath("/home/joe/doe/folder/next")
 >>> next
 Path('/home/joe/doe/folder/next')
-
+```
+```python
 >>> next.rename(folder)
 >>> next
 Path('/home/joe/doe/folder/top')
 >>> next.exists()
 True
 >>> Path('/home/joe/doe/folder/sub').exists()
 False
-
 ```
 
 ## Path Class
 
 This class is immutable by default, just as the `pathlib.Path`. However, it allows to open a editing context via `mutate()`.
 Moreover, there are additional contexts for file operations. They update the file and its path while closing the context.
 If the file operations don't succeed, they throw an exception and fall back to the original path value.
 
 ```python
-
 >>> from mutapath import Path
-
+```
+```python
 >>> folder = Path("/home/joe/doe/folder/sub")
 >>> folder
 Path('/home/joe/doe/folder/sub')
-
+```
+```python
 >>> folder.name = "top"
 AttributeError: mutapath.Path is an immutable class, unless mutate() context is used.
 >>> folder
 Path('/home/joe/doe/folder/sub')
-
+```
+```python
 >>> with folder.mutate() as m:
 ...     m.name = "top"
 >>> folder
 Path('/home/joe/doe/folder/top')
-
+```
+```python
 >>> next = Path("/home/joe/doe/folder/next")
 >>> next.copy(folder)
 >>> next
 Path('/home/joe/doe/folder/next')
 >>> folder.exists()
 True
 >>> folder.remove()
-
+```
+```python
 >>> with next.renaming() as m:
 ...     m.stem = folder.stem
 ...     m.suffix = ".txt"
 >>> next
 Path("/home/joe/doe/folder/sub.txt")
 >>> next.exists()
 True
 >>> next.with_name("next").exists()
 False
-
 ```
```

### Comparing `mutapath-0.8.2/mutapath/immutapath.py` & `mutapath-0.9.0/mutapath/immutapath.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,28 @@
 import contextlib
 import io
 import os
 import pathlib
 import shutil
 from contextlib import contextmanager
 from dataclasses import dataclass
-from types import GeneratorType
-from typing import Union, Iterable, ClassVar, Callable, List
-from xml.dom.minicompat import StringTypes
+from typing import Union, Iterable, ClassVar, Callable
 
 import filelock
 import path
 from cached_property import cached_property
 from filelock import SoftFileLock
 
 import mutapath
-from mutapath.decorator import path_wrap, _convert_path
+from mutapath.decorator import path_wrapper, wrap_attribute
 from mutapath.exceptions import PathException
 from mutapath.lock_dummy import DummyFileLock
 
 
-@path_wrap
+@path_wrapper
 @dataclass(repr=False, eq=False)
 class Path(object):
     """Immutable Path"""
     __mutable: ClassVar[object]
     _contained: Union[path.Path, pathlib.Path, str] = ""
 
     def __post_init__(self):
@@ -41,31 +39,17 @@
                 self._contained = self._contained._contained
             if isinstance(self._contained, pathlib.Path):
                 self._contained = path.Path(str(self._contained))
 
     def __dir__(self) -> Iterable[str]:
         return sorted(super(Path, self).__dir__()) + dir(path.Path)
 
-    @staticmethod
-    def __wrap_attribute(orig_func):
-        def __wrap_decorator(*args, **kwargs):
-            result = orig_func(*args, **kwargs)
-            if isinstance(result, List) and not isinstance(result, StringTypes):
-                return list(map(_convert_path, result))
-            if isinstance(result, Iterable) and not isinstance(result, StringTypes):
-                return iter(map(_convert_path, result))
-            if isinstance(result, GeneratorType):
-                return map(_convert_path, result)
-            return _convert_path(result)
-
-        return __wrap_decorator
-
     def __getattr__(self, item):
         attr = getattr(self._contained, item)
-        return Path.__wrap_attribute(attr)
+        return wrap_attribute(attr)
 
     def __setattr__(self, key, value):
         if key == "_contained":
             lock = self.__dict__.get("lock", None)
             if lock is not None:
                 if self.lock.is_locked:
                     self.lock.release()
@@ -142,25 +126,25 @@
     def _norm(pathly: path.Path):
         return path.Path(path.Path.module.normpath(pathly))
 
     def with_name(self, new_name) -> Path:
         """
         Clone this path with a new name
 
-        .. seealso:: :func:`pathlib.Path.with_name`
+        .. seealso:: :py:func:`pathlib.Path.with_name`
         """
         return self.base.joinpath(str(new_name))
 
     def with_stem(self, new_stem) -> Path:
         """Clone this path with a new stem"""
         return self.base.joinpath(str(new_stem)).with_suffix(self.ext)
 
     def with_parent(self, new_parent) -> Path:
         """Clone this path with a new parent"""
-        return Path(new_parent).joinpath(str(self.name))
+        return Path(new_parent) / self.name
 
     def with_base(self, base, strip_length: int = 0):
         """
         Clone this path with a new base.
 
         The given path is used in its full length as base of this path, if strip_length is not specified.
         If strip_length is specified, the given number of path elements are stripped from the left side,
@@ -244,155 +228,151 @@
         self._contained = self.with_name(value)
 
     @property
     def base(self) -> Path:
         """
         Get path base (i.e., the parent of the file)
 
-        seealso:: :func:`pathlib.Path.parent`
+        .. seealso:: :py:func:`pathlib.Path.parent`
         """
         return Path(self._contained.parent)
 
     @base.setter
     def base(self, value):
         """
         Set a new file base
 
-        seealso:: :func:`mutapath.Path.with_base`
+        .. seealso:: :func:`mutapath.Path.with_base`
         """
         self._contained = self.with_base(value)
 
     @property
     def uncshare(self) -> Path:
         """
         Get this path as UNC mount point
 
-        seealso:: :func:`pathlib.Path.uncshare`
+        .. seealso:: :py:func:`pathlib.Path.uncshare`
         """
         return Path(self._contained.uncshare)
 
     @property
     def stem(self) -> str:
         """
         Get path stem
 
-        seealso:: :func:`pathlib.Path.stem`
+        .. seealso:: :py:func:`pathlib.Path.stem`
         """
         return self._contained.stem
 
     @stem.setter
     def stem(self, value):
-        """
-        Set a new file stem
-
-        seealso:: :func:`mutapath.Path.with_stem`
-        """
         self._contained = self.with_stem(value)
 
     @property
     def drive(self) -> Path:
         """
         Get path drive
 
-        seealso:: :func:`pathlib.Path.drive`
+        .. seealso:: :py:func:`pathlib.Path.drive`
         """
         return Path(self._contained.drive)
 
     @property
     def parent(self) -> Path:
         """
         Get the parent path
 
-        seealso:: :func:`pathlib.Path.parent`
+        .. seealso:: :attr:`pathlib.PurePath.parent`, :func:`os.path.dirname`
         """
         return Path(self._contained.parent)
 
     @parent.setter
     def parent(self, value):
-        """
-        Set a new file parent
-
-        seealso:: :func:`mutapath.Path.with_parent`
-        """
         self._contained = self.with_parent(value)
 
     @property
     def parents(self) -> Iterable[Path]:
         """
         Get a list of all parent paths
 
-        seealso:: :func:`pathlib.Path.parents`
+        .. seealso:: :py:func:`pathlib.Path.parents`
         """
         result = pathlib.Path(self._contained).parents
         return iter(map(Path, result))
 
     @property
     def dirname(self) -> Path:
         """
         Get the parent path
 
-        seealso:: :func:`pathlib.Path.dirname`
+        .. seealso:: :attr:`parent`, :func:`os.path.dirname`
         """
         return Path(self._contained.dirname())
 
     @property
     def size(self) -> int:
         """
         Get the size of the file
 
-        seealso:: :func:`path.Path.size`
+        .. seealso:: :func:`path.Path.size`
         """
         return self._contained.size
 
     @property
     def ctime(self) -> float:
         """
         Get the creation time of the file
 
-        seealso:: :func:`os.path.getctime`
+        .. seealso:: :func:`os.path.getctime`
         """
         return self._contained.ctime
 
     @property
     def mtime(self) -> float:
         """
         Get the mtime of the file
 
-        seealso:: :func:`os.path.getmtime`
+        .. seealso:: :func:`os.path.getmtime`
         """
         return self._contained.mtime
 
     @property
     def atime(self) -> float:
         """
         Get the atime of the file
 
-        seealso:: :func:`os.path.getatime`
+        .. seealso:: :func:`os.path.getatime`
         """
         return self._contained.atime
 
     @property
     def owner(self):
         """
         Get the owner of the file.
         """
         return self._contained.owner
 
     def open(self, *args, **kwargs):
         """
         Open a file and return a stream to its content.
 
-        seealso:: :func:`io.open`
+        .. seealso:: :func:`io.open`
         """
         return io.open(str(self), *args, **kwargs)
 
     @cached_property
-    def lock(self) -> SoftFileLock:
+    def lock(self) -> filelock.BaseFileLock:
         """
-        Get a file lock holder for this file.
+        Generate a cached file locker for this file with the additional suffix '.lock'.
+        If this path refers not to an existing file or to an existing folder,
+        a dummy lock is returned that does not do anything.
+
+        Once this path os modified (cloning is not modifying), the lock is released and regenerated for the new path.
+
+        .. seealso:: :class:`~filelock.SoftFileLock`, :class:`~mutapath.lock_dummy.DummyFileLock`
         """
         lock_file = self._contained.with_suffix(self.suffix + ".lock")
         if not self.isfile():
             return DummyFileLock(lock_file)
         return SoftFileLock(lock_file)
 
     @contextmanager
@@ -403,15 +383,15 @@
         >>> with Path('/home/doe/folder/sub').mutate() as mut:
         ...     mut.name = "top"
         Path('/home/doe/folder/top')
 
         """
         self.__mutable = mutapath.MutaPath(self)
         yield self.__mutable
-        self._contained = getattr(self.__mutable, "_contained")
+        self._contained = self.__mutable._contained
 
     @contextmanager
     def _op_context(self, name: str, timeout: float, lock: bool,
                     operation:
                     Callable[[Union[os.PathLike, path.Path], Union[os.PathLike, path.Path]], Union[str, path.Path]]):
         """
         Acquire a file mutation context that is bound to a file.
@@ -432,15 +412,15 @@
                     raise PathException(
                         f"{name.capitalize()} {self._contained} failed because the file could not be locked.") from t
 
             self.__mutable = mutapath.MutaPath(self)
             yield self.__mutable
 
             current_file = self._contained
-            target_file = getattr(self.__mutable, "_contained")
+            target_file = self.__mutable._contained
 
             try:
                 current_file = path.Path(operation(current_file, target_file))
 
             except FileExistsError as e:
                 raise PathException(
                     f"{name.capitalize()} to {current_file.normpath()} failed because the file already exists. "
@@ -466,15 +446,14 @@
         :param lock: if the source file should be locked as long as this context is open
         :param method: an alternative method that renames the path (e.g., os.renames)
 
         :Example:
         >>> with Path('/home/doe/folder/a.txt').renaming() as mut:
         ...     mut.stem = "b"
         Path('/home/doe/folder/b.txt')
-
         """
 
         def checked_rename(cls: path.Path, target: path.Path):
             target_lock_file = target.with_suffix(target.ext + ".lock")
             target_lock = SoftFileLock(target_lock_file)
             if lock and cls.isfile():
                 try:
```

### Comparing `mutapath-0.8.2/mutapath/mutapath.py` & `mutapath-0.9.0/mutapath/mutapath.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 
 import mutapath
-from mutapath.decorator import path_mutable
+from mutapath.decorator import mutable_path_wrapper
 
 
-@path_mutable
+@mutable_path_wrapper
 @dataclass(repr=False, eq=False)
 class MutaPath(mutapath.Path):
     """Mutable Path"""
 
     def __post_init__(self):
         if isinstance(self._contained, MutaPath):
             self._contained = self._contained._contained
```

### Comparing `mutapath-0.8.2/mutapath.egg-info/PKG-INFO` & `mutapath-0.9.0/mutapath.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutapath
-Version: 0.8.2
+Version: 0.9.0
 Summary: Mutable Pathlib
 Home-page: https://github.com/matfax/mutapath
 Author: matfax
 Author-email: matthias.fax@gmail.com
 License: lgpl-3.0
 Description: # mutapath
         
@@ -24,86 +24,92 @@
         
         ## MutaPath Class
         
         The MutaPath Class allows direct manipulation of its attributes at any time, just as any mutable object.
         Once a file operation is called that is intended to modify its path, the underlying path is also mutated.
         
         ```python
-        
         >>> from mutapath import MutaPath
-        
+        ```
+        ```python
         >>> folder = MutaPath("/home/joe/doe/folder/sub")
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> folder.name = "top"
         >>> folder
         Path('/home/joe/doe/folder/top')
-        
+        ```
+        ```python
         >>> next = MutaPath("/home/joe/doe/folder/next")
         >>> next
         Path('/home/joe/doe/folder/next')
-        
+        ```
+        ```python
         >>> next.rename(folder)
         >>> next
         Path('/home/joe/doe/folder/top')
         >>> next.exists()
         True
         >>> Path('/home/joe/doe/folder/sub').exists()
         False
-        
         ```
         
         ## Path Class
         
         This class is immutable by default, just as the `pathlib.Path`. However, it allows to open a editing context via `mutate()`.
         Moreover, there are additional contexts for file operations. They update the file and its path while closing the context.
         If the file operations don't succeed, they throw an exception and fall back to the original path value.
         
         ```python
-        
         >>> from mutapath import Path
-        
+        ```
+        ```python
         >>> folder = Path("/home/joe/doe/folder/sub")
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> folder.name = "top"
         AttributeError: mutapath.Path is an immutable class, unless mutate() context is used.
         >>> folder
         Path('/home/joe/doe/folder/sub')
-        
+        ```
+        ```python
         >>> with folder.mutate() as m:
         ...     m.name = "top"
         >>> folder
         Path('/home/joe/doe/folder/top')
-        
+        ```
+        ```python
         >>> next = Path("/home/joe/doe/folder/next")
         >>> next.copy(folder)
         >>> next
         Path('/home/joe/doe/folder/next')
         >>> folder.exists()
         True
         >>> folder.remove()
-        
+        ```
+        ```python
         >>> with next.renaming() as m:
         ...     m.stem = folder.stem
         ...     m.suffix = ".txt"
         >>> next
         Path("/home/joe/doe/folder/sub.txt")
         >>> next.exists()
         True
         >>> next.with_name("next").exists()
         False
-        
         ```
         
 Keywords: pathlib,mutable,path
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mutapath-0.8.2/tests/helper.py` & `mutapath-0.9.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `mutapath-0.8.2/tests/test_immutapath.py` & `mutapath-0.9.0/tests/test_immutapath.py`

 * *Files identical despite different names*

### Comparing `mutapath-0.8.2/tests/test_mutapath.py` & `mutapath-0.9.0/tests/test_mutapath.py`

 * *Files identical despite different names*

### Comparing `mutapath-0.8.2/tests/test_with_path.py` & `mutapath-0.9.0/tests/test_with_path.py`

 * *Files identical despite different names*

