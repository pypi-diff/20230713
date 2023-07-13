# Comparing `tmp/zipp-3.9.0.tar.gz` & `tmp/zipp-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipp-3.9.0.tar", last modified: Sat Oct  8 18:06:18 2022, max compression
+gzip compressed data, was "zipp-3.9.1.tar", last modified: Mon Oct 24 01:14:13 2022, max compression
```

## Comparing `zipp-3.9.0.tar` & `zipp-3.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 18:06:18.884553 zipp-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-08 18:05:38.000000 zipp-3.9.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-08 18:05:38.000000 zipp-3.9.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-08 18:05:38.000000 zipp-3.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 18:06:18.880552 zipp-3.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-08 18:05:38.000000 zipp-3.9.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-08 18:05:38.000000 zipp-3.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 18:06:18.880552 zipp-3.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-08 18:05:38.000000 zipp-3.9.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-08 18:05:38.000000 zipp-3.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-08 18:05:38.000000 zipp-3.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3915 2022-10-08 18:05:38.000000 zipp-3.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-08 18:05:38.000000 zipp-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-08 18:06:18.884553 zipp-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-10-08 18:05:38.000000 zipp-3.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-10-08 18:05:38.000000 zipp-3.9.0/_test_params.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-08 18:05:38.000000 zipp-3.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 18:06:18.880552 zipp-3.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-08 18:05:38.000000 zipp-3.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-08 18:05:38.000000 zipp-3.9.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-08 18:05:38.000000 zipp-3.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-08 18:05:38.000000 zipp-3.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-08 18:05:38.000000 zipp-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-10-08 18:05:38.000000 zipp-3.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-10-08 18:06:18.884553 zipp-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    12748 2022-10-08 18:05:38.000000 zipp-3.9.0/test_zipp.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-08 18:05:38.000000 zipp-3.9.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-08 18:06:18.884553 zipp-3.9.0/zipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-08 18:06:18.000000 zipp-3.9.0/zipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-08 18:06:18.000000 zipp-3.9.0/zipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-08 18:06:18.000000 zipp-3.9.0/zipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-08 18:06:18.000000 zipp-3.9.0/zipp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-08 18:06:18.000000 zipp-3.9.0/zipp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8467 2022-10-08 18:05:38.000000 zipp-3.9.0/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 01:14:13.336493 zipp-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-24 01:13:32.000000 zipp-3.9.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-10-24 01:13:32.000000 zipp-3.9.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-24 01:13:32.000000 zipp-3.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 01:14:13.336493 zipp-3.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-24 01:13:32.000000 zipp-3.9.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-24 01:13:32.000000 zipp-3.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 01:14:13.336493 zipp-3.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-24 01:13:32.000000 zipp-3.9.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-24 01:13:32.000000 zipp-3.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-24 01:13:32.000000 zipp-3.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-10-24 01:13:32.000000 zipp-3.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-24 01:13:32.000000 zipp-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-24 01:14:13.336493 zipp-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-10-24 01:13:32.000000 zipp-3.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-10-24 01:13:32.000000 zipp-3.9.1/_test_params.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 01:13:32.000000 zipp-3.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 01:14:13.336493 zipp-3.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-24 01:13:32.000000 zipp-3.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-24 01:13:32.000000 zipp-3.9.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-24 01:13:32.000000 zipp-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-24 01:13:32.000000 zipp-3.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-24 01:13:32.000000 zipp-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-10-24 01:13:32.000000 zipp-3.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-10-24 01:14:13.336493 zipp-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    12850 2022-10-24 01:13:32.000000 zipp-3.9.1/test_zipp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-24 01:13:32.000000 zipp-3.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 01:14:13.336493 zipp-3.9.1/zipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-24 01:14:13.000000 zipp-3.9.1/zipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-10-24 01:14:13.000000 zipp-3.9.1/zipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 01:14:13.000000 zipp-3.9.1/zipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-24 01:14:13.000000 zipp-3.9.1/zipp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-24 01:14:13.000000 zipp-3.9.1/zipp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8912 2022-10-24 01:13:32.000000 zipp-3.9.1/zipp.py
```

### Comparing `zipp-3.9.0/.github/workflows/main.yml` & `zipp-3.9.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/CHANGES.rst` & `zipp-3.9.1/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v3.9.1
+======
+
+* Removed 'print' expression in test_pickle.
+
+* bpo-43651: Apply ``io.text_encoding`` on Python 3.10 and later.
+
 v3.9.0
 ======
 
 * #81: ``Path`` objects are now pickleable if they've been
   constructed from pickleable objects. Any restored objects
   will re-construct the zip file with the original arguments.
```

### Comparing `zipp-3.9.0/LICENSE` & `zipp-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/PKG-INFO` & `zipp-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipp
-Version: 3.9.0
+Version: 3.9.1
 Summary: Backport of pathlib-compatible object wrapper for zip files
 Home-page: https://github.com/jaraco/zipp
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zipp-3.9.0/README.rst` & `zipp-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/_test_params.py` & `zipp-3.9.1/_test_params.py`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/docs/conf.py` & `zipp-3.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/pytest.ini` & `zipp-3.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/setup.cfg` & `zipp-3.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/test_zipp.py` & `zipp-3.9.1/test_zipp.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,27 +134,27 @@
         assert (root / 'g').is_dir()
         assert (root / 'g/').is_dir()
 
     @pass_alpharep
     def test_open(self, alpharep):
         root = zipp.Path(alpharep)
         a, b, g = root.iterdir()
-        with a.open() as strm:
+        with a.open(encoding="utf-8") as strm:
             data = strm.read()
         assert data == "content of a"
 
     def test_open_write(self):
         """
         If the zipfile is open for write, it should be possible to
         write bytes or text to it.
         """
         zf = zipp.Path(zipfile.ZipFile(io.BytesIO(), mode='w'))
         with zf.joinpath('file.bin').open('wb') as strm:
             strm.write(b'binary contents')
-        with zf.joinpath('file.txt').open('w') as strm:
+        with zf.joinpath('file.txt').open('w', encoding="utf-8") as strm:
             strm.write('text file')
 
     def test_open_extant_directory(self):
         """
         Attempting to open a directory raises IsADirectoryError.
         """
         zf = zipp.Path(add_dirs(build_alpharep_fixture()))
@@ -177,38 +177,38 @@
         with self.assertRaises(FileNotFoundError):
             zf.joinpath('z').open()
 
     @pass_alpharep
     def test_read(self, alpharep):
         root = zipp.Path(alpharep)
         a, b, g = root.iterdir()
-        assert a.read_text() == "content of a"
+        assert a.read_text(encoding="utf-8") == "content of a"
         assert a.read_bytes() == b"content of a"
 
     @pass_alpharep
     def test_joinpath(self, alpharep):
         root = zipp.Path(alpharep)
         a = root.joinpath("a.txt")
         assert a.is_file()
         e = root.joinpath("b").joinpath("d").joinpath("e.txt")
-        assert e.read_text() == "content of e"
+        assert e.read_text(encoding="utf-8") == "content of e"
 
     @pass_alpharep
     def test_joinpath_multiple(self, alpharep):
         root = zipp.Path(alpharep)
         e = root.joinpath("b", "d", "e.txt")
-        assert e.read_text() == "content of e"
+        assert e.read_text(encoding="utf-8") == "content of e"
 
     @pass_alpharep
     def test_traverse_truediv(self, alpharep):
         root = zipp.Path(alpharep)
         a = root / "a.txt"
         assert a.is_file()
         e = root / "b" / "d" / "e.txt"
-        assert e.read_text() == "content of e"
+        assert e.read_text(encoding="utf-8") == "content of e"
 
     @pass_alpharep
     def test_traverse_simplediv(self, alpharep):
         """
         Disable the __future__.division when testing traversal.
         """
         code = compile(
@@ -257,17 +257,17 @@
         reflect that change.
         """
         root = zipp.Path(alpharep)
         a, b, g = root.iterdir()
         alpharep.writestr('foo.txt', 'foo')
         alpharep.writestr('bar/baz.txt', 'baz')
         assert any(child.name == 'foo.txt' for child in root.iterdir())
-        assert (root / 'foo.txt').read_text() == 'foo'
+        assert (root / 'foo.txt').read_text(encoding="utf-8") == 'foo'
         (baz,) = (root / 'bar').iterdir()
-        assert baz.read_text() == 'baz'
+        assert baz.read_text(encoding="utf-8") == 'baz'
 
     HUGE_ZIPFILE_NUM_ENTRIES = 2**13
 
     def huge_zipfile(self):
         """Create a read-only zipfile with a huge number of entries entries."""
         strm = io.BytesIO()
         zf = zipfile.ZipFile(strm, "w")
@@ -293,15 +293,15 @@
         zipp.CompleteDirs._implied_dirs(data)
 
     @pass_alpharep
     def test_read_does_not_close(self, alpharep):
         alpharep = self.zipfile_ondisk(alpharep)
         with zipfile.ZipFile(alpharep) as file:
             for rep in range(2):
-                zipp.Path(file, 'a.txt').read_text()
+                zipp.Path(file, 'a.txt').read_text(encoding="utf-8")
 
     @pass_alpharep
     def test_subclass(self, alpharep):
         class Subclass(zipp.Path):
             pass
 
         root = Subclass(alpharep)
@@ -414,14 +414,13 @@
         itertools.product(
             alpharep_generators,
             [str, pathlib.Path],
             ['', 'b/'],
         ),
     )
     def test_pickle(self, alpharep, path_type, subpath):
-        print(alpharep, path_type, subpath)
         zipfile_ondisk = path_type(self.zipfile_ondisk(alpharep))
 
         saved_1 = pickle.dumps(zipp.Path(zipfile_ondisk, at=subpath))
         restored_1 = pickle.loads(saved_1)
         first, *rest = restored_1.iterdir()
         assert first.read_text().startswith('content of ')
```

### Comparing `zipp-3.9.0/tox.ini` & `zipp-3.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `zipp-3.9.0/zipp.egg-info/PKG-INFO` & `zipp-3.9.1/zipp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipp
-Version: 3.9.0
+Version: 3.9.1
 Summary: Backport of pathlib-compatible object wrapper for zip files
 Home-page: https://github.com/jaraco/zipp
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zipp-3.9.0/zipp.py` & `zipp-3.9.1/zipp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import io
+import sys
 import posixpath
 import zipfile
 import itertools
 import contextlib
 import pathlib
 
 
 __all__ = ['Path']
 
 
+te_impl = 'lambda encoding, stacklevel=2, /: encoding'
+te_impl_37 = te_impl.replace(', /', '')
+_text_encoding = eval(te_impl if sys.version_info > (3, 8) else te_impl_37)
+
+
+text_encoding = (
+    io.text_encoding if sys.version_info > (3, 10) else _text_encoding  # type: ignore
+)
+
+
 def _parents(path):
     """
     Given a path with elements separated by
     posixpath.sep, generate all parents of that path.
 
     >>> list(_parents('b/d'))
     ['b']
@@ -253,14 +264,16 @@
         if not self.exists() and zip_mode == 'r':
             raise FileNotFoundError(self)
         stream = self.root.open(self.at, zip_mode, pwd=pwd)
         if 'b' in mode:
             if args or kwargs:
                 raise ValueError("encoding args invalid for binary operation")
             return stream
+        else:
+            kwargs["encoding"] = text_encoding(kwargs.get("encoding"))
         return io.TextIOWrapper(stream, *args, **kwargs)
 
     @property
     def name(self):
         return pathlib.Path(self.at).name or self.filename.name
 
     @property
@@ -276,14 +289,15 @@
         return pathlib.Path(self.at).stem or self.filename.stem
 
     @property
     def filename(self):
         return pathlib.Path(self.root.filename).joinpath(self.at)
 
     def read_text(self, *args, **kwargs):
+        kwargs["encoding"] = text_encoding(kwargs.get("encoding"))
         with self.open('r', *args, **kwargs) as strm:
             return strm.read()
 
     def read_bytes(self):
         with self.open('rb') as strm:
             return strm.read()
```

