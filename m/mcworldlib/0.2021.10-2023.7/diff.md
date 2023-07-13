# Comparing `tmp/mcworldlib-0.2021.10.tar.gz` & `tmp/mcworldlib-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rodrigo/work/minecraft/mcworldlib/dist/tmp3zkbgojh/mcworldlib-0.2021.10.tar", last modified: Sun Oct 31 22:03:42 2021, max compression
+gzip compressed data, was "/home/rodrigo/work/minecraft/mcworldlib/dist/.tmp-ontvqx11/mcworldlib-2023.7.tar", last modified: Thu Jul 13 01:09:16 2023, max compression
```

## Comparing `mcworldlib-0.2021.10.tar` & `mcworldlib-2023.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1067 2021-10-20 11:36:27.000000 mcworldlib-0.2021.10/mcworldlib/player.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1672 2021-10-17 15:13:52.000000 mcworldlib-0.2021.10/mcworldlib/entity.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1536 2021-10-31 04:36:50.000000 mcworldlib-0.2021.10/mcworldlib/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    12279 2021-10-27 04:04:00.000000 mcworldlib-0.2021.10/mcworldlib/util.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4739 2021-10-31 21:37:43.000000 mcworldlib-0.2021.10/mcworldlib/chunk.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    10799 2021-10-31 21:33:00.000000 mcworldlib-0.2021.10/mcworldlib/world.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    11447 2021-10-31 21:17:17.000000 mcworldlib-0.2021.10/mcworldlib/nbt.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2183 2021-10-10 01:17:47.000000 mcworldlib-0.2021.10/mcworldlib/cli.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     8135 2021-10-31 21:26:47.000000 mcworldlib-0.2021.10/mcworldlib/tree.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    18899 2021-10-31 21:36:14.000000 mcworldlib-0.2021.10/mcworldlib/anvil.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1616 2021-10-26 20:59:27.000000 mcworldlib-0.2021.10/mcworldlib/level.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14459 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1337 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      497 2021-10-28 05:28:12.000000 mcworldlib-0.2021.10/pyproject.toml
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2019-12-10 03:18:22.000000 mcworldlib-0.2021.10/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    13214 2021-10-31 03:07:19.000000 mcworldlib-0.2021.10/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      430 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14459 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       25 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       11 2021-10-31 22:03:42.000000 mcworldlib-0.2021.10/mcworldlib.egg-info/top_level.txt
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2019-12-10 03:18:22.000000 mcworldlib-2023.7/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14435 2023-07-13 01:09:16.610249 mcworldlib-2023.7/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    13211 2023-07-13 00:36:20.000000 mcworldlib-2023.7/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/mcworldlib/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1536 2021-10-31 04:36:50.000000 mcworldlib-2023.7/mcworldlib/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    18899 2021-10-31 21:36:14.000000 mcworldlib-2023.7/mcworldlib/anvil.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4789 2023-07-12 19:16:33.000000 mcworldlib-2023.7/mcworldlib/chunk.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2183 2021-10-10 01:17:47.000000 mcworldlib-2023.7/mcworldlib/cli.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1672 2021-10-17 15:13:52.000000 mcworldlib-2023.7/mcworldlib/entity.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1616 2021-10-26 20:59:27.000000 mcworldlib-2023.7/mcworldlib/level.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     9469 2023-07-13 00:59:22.000000 mcworldlib-2023.7/mcworldlib/nbt.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1067 2021-10-20 11:36:27.000000 mcworldlib-2023.7/mcworldlib/player.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     8135 2021-10-31 21:26:47.000000 mcworldlib-2023.7/mcworldlib/tree.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    12279 2021-10-27 04:04:00.000000 mcworldlib-2023.7/mcworldlib/util.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    10808 2021-11-01 01:25:32.000000 mcworldlib-2023.7/mcworldlib/world.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/mcworldlib.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14435 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      445 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       25 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       11 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      544 2021-10-31 22:06:22.000000 mcworldlib-2023.7/pyproject.toml
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1336 2023-07-13 01:09:16.610249 mcworldlib-2023.7/setup.cfg
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/tests/
+-rwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)     6834 2021-10-31 21:27:07.000000 mcworldlib-2023.7/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mcworldlib-0.2021.10/mcworldlib/player.py` & `mcworldlib-2023.7/mcworldlib/player.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/entity.py` & `mcworldlib-2023.7/mcworldlib/entity.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/__init__.py` & `mcworldlib-2023.7/mcworldlib/__init__.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/util.py` & `mcworldlib-2023.7/mcworldlib/util.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/chunk.py` & `mcworldlib-2023.7/mcworldlib/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         for section in self.data_root['Sections']:
             # noinspection PyPep8Naming
             Y = int(section['Y'])
             palette, indexes = self.get_section_blocks(Y, _section=section)
             if palette:
                 blocks[Y] = palette, indexes
         for Y in sorted(blocks):
+            # noinspection PyRedundantParentheses
             yield (Y, *blocks[Y])
 
     # noinspection PyPep8Naming
     def get_section_blocks(self, Y: int, _section=None):
         """Return a (Palette, BlockState Indexes Array) tuple for a chunk section.
 
         Palette: NBT List of Block States, straight from NBT data
```

### Comparing `mcworldlib-0.2021.10/mcworldlib/world.py` & `mcworldlib-2023.7/mcworldlib/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     @property
     def chunk_count(self):  # FIXME!
         return sum(len(_) for _ in self.regions)
 
     def get_chunks(self, progress=True, dimension=OVERWORLD, category='region'):
         """Yield all chunks in a given dimension and category, Overworld Regions by default"""
-        regions = self.dimensions[dimension][category]
+        regions = self.dimensions[dimension][category].values()
         if progress:
             regions = tqdm.tqdm(regions)
         for region in regions:
             for chunk in region.values():
                 yield chunk
 
     def get_all_chunks(self, progress=True
```

### Comparing `mcworldlib-0.2021.10/mcworldlib/nbt.py` & `mcworldlib-2023.7/mcworldlib/nbt.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,30 +17,17 @@
 import zlib    as _zlib
 
 # TODO: (and suggest to nbtlib)
 # - Auto-casting value to tag on assignment based on current type
 #   - compound['string'] = 'foo' -> compound['string'] = String('foo')
 #   - maybe this is only meant for nbtlib.Schema?
 
-# not in nbtlib.tag.__all__ and only used here
-# noinspection PyProtectedMember
-from nbtlib.tag import (
-    Base as _Base,
-    BYTE as _BYTE,
-    read_numeric  as _read_numeric,
-    read_string   as _read_string,
-    write_numeric as _write_numeric,
-    write_string  as _write_string,
-)
 from nbtlib.tag import *
-# noinspection PyProtectedMember, PyUnresolvedReferences
 from nbtlib.tag import Array  # Not in __all__, but used by others
-# noinspection PyUnresolvedReferences
 from nbtlib.nbt import File as _File  # intentionally not importing load
-# noinspection PyUnresolvedReferences
 from nbtlib.path import Path
 from nbtlib.literal.serializer import serialize_tag as _serialize_tag
 
 from . import tree as _tree
 
 _log = _logging.getLogger(__name__)
 
@@ -68,21 +55,15 @@
 
 RT = t.TypeVar('RT', bound='Root')
 
 
 class Root(Compound):
     """Unnamed Compound tag, the root tag in files and chunks"""
 
-    __slots__ = (
-        'root_name',
-    )
-
-    def __init__(self, *args, root_name: str = "", **kwargs):
-        super().__init__(*args, **kwargs)
-        self.root_name: str = root_name
+    __slots__ = ()
 
     @property
     def data_root(self) -> Compound:
         """Root itself or the child containing all data apart from DataVersion.
 
         A convenience shortcut for root compounds that contains just DataVersion
         and another tag, and all relevant data is in that tag, as is the case for
@@ -106,43 +87,23 @@
         tags = self.keys() - {'DataVersion'}
         if not len(tags) == 1:
             return "", self
         name = next(iter(tags))
         # FIXME: Should make sure it's actually a Compound and not just AnyTag
         return name, self[name]
 
-    @classmethod
-    def parse(cls: t.Type[RT], buff, byteorder='big') -> RT:
-        # For the typing dance, see https://stackoverflow.com/a/44644576/624066
-        tag_id = _read_numeric(_BYTE, buff, byteorder)
-        if not tag_id == cls.tag_id:
-            # Possible issues with a non-Compound root:
-            # - root_name might not be in __slots__(), and thus not assignable
-            # - not returning a superclass might be surprising and have side effects
-            raise TypeError("Non-Compound root tags is not supported:"
-                            f"{cls.get_tag(tag_id).__name__}")
-        name = _read_string(buff, byteorder)
-        self: RT = super().parse(buff, byteorder)
-        self.root_name = name
-        return self
-
-    def write(self, buff, byteorder='big') -> None:
-        _write_numeric(_BYTE, self.tag_id, buff, byteorder)
-        _write_string(getattr(self, 'root_name', "") or "", buff, byteorder)
-        super().write(buff, byteorder)
-        print(f"writing end tag: {self.end_tag!r}, {len(self.end_tag)} bytes")
-        buff.write(4 * self.end_tag)
-        buff.write(b'rodrigo')
+    # Move some methods from File. Keeping them there would confuse super() calls
+    parse = _File.parse; del _File.parse
+    write = _File.write; del _File.write
 
     def __repr__(self):
         key, data = self._data_root  # save refs for efficiency
         if key:
             key = f" ({len(data)} in {key!r})"
-        name = f" {self.root_name!r}" if self.root_name else ""
-        return f'<{self.__class__.__name__}{name} tags: {len(self)}{key}>'
+        return f'<{self.__class__.__name__} tags: {len(self)}{key}>'
 
 
 # Overrides and extensions
 
 class File(Root, _File):
     # Lame overload so it inherits from Root
     __slots__ = ()
@@ -152,15 +113,15 @@
         # make gzipped an optional argument, defaulting to True
         return super().load(filename, gzipped=gzipped, *args, **kwargs)
 
     @classmethod
     def load_mcc(cls, filename):
         with open(filename, 'rb') as buff:
             data = _io.BytesIO(_zlib.decompress(buff.read()))
-        self = cls.from_buffer(data)
+        self = cls.parse(data)
         self.filename = filename
         return self
 
     def __repr__(self):
         name = self.__class__.__name__
         return super().__repr__().replace(f"<{name}", f"<{name} {self.filename!r}", 1)
 
@@ -291,30 +252,19 @@
         show_root_as=root_name,
         width=width,
         indent_first_gen=False,
     )
 
 
 # Add .pretty() method to all NBT tags
-_Base.pretty = lambda self, indent=4: _serialize_tag(self, indent=indent)
+Base.pretty = lambda self, indent=4: _serialize_tag(self, indent=indent)
 
-_Base.is_leaf = property(
+Base.is_leaf = property(
     fget=lambda _: not isinstance(_, (Compound, List, Array)),
     doc="If this tag an immutable tag and not a Mutable Collection."
         " Non-leaves are the containers excluding String: Compound, List, Array")
 
-# Fix String.__str__. Not needed in modern nbtlib versions
-String.__str__ = lambda self: str.__str__(self)
-
-# Ensure the trailing End Tag gets written.
-# See https://github.com/vberlier/nbtlib/issues/153
-del _File.end_tag
-
-# Just in case, as now we have a very different meaning for .root_name
-delattr(_File, 'root')
-delattr(_File, 'root_name')
-
 # Convenience shortcuts
 load_mcc = File.load_mcc
 load_dat = File.load
 
 del t
```

### Comparing `mcworldlib-0.2021.10/mcworldlib/cli.py` & `mcworldlib-2023.7/mcworldlib/cli.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/tree.py` & `mcworldlib-2023.7/mcworldlib/tree.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/anvil.py` & `mcworldlib-2023.7/mcworldlib/anvil.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/mcworldlib/level.py` & `mcworldlib-2023.7/mcworldlib/level.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/PKG-INFO` & `mcworldlib-2023.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: mcworldlib
-Version: 0.2021.10
+Version: 2023.7
 Summary: Yet another python library to manipulate Minecraft save data
 Home-page: https://github.com/MestreLion/mcworldlib
 Author: Rodrigo Silva (MestreLion)
 Author-email: minecraft@rodrigosilva.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/MestreLion/mcworldlib/issues
 Project-URL: Source Code, https://github.com/MestreLion/mcworldlib
 Keywords: minecraft,save,nbt,chunk,region,world,library
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mcworldlib - Minecraft World Library
 
 Yet another library to manipulate Minecraft data, inspired by the now-defunct
 [pymclevel](https://github.com/mcedit/pymclevel), building on top of the amazing
@@ -392,15 +391,15 @@
   blocks, entities and so on.
 
 - **CLI**: Add a command-line interface for commonly used operations.
 
 See the [To-Do List](./TODO.txt) for more updated technical information and
 planned features.
 
-If you find a bug or have any enhancement request, please to open a
+If you find a bug or have any enhancement request, please open a
 [new issue](https://github.com/MestreLion/mcworldlib/issues/new)
 
 
 Author
 ------
 
 Rodrigo Silva (MestreLion) <linux@rodrigosilva.com>
@@ -412,9 +411,7 @@
 
 License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
 
 This is free software: you are free to change and redistribute it.
 
 There is NO WARRANTY, to the extent permitted by law.
 ```
-
-
```

### Comparing `mcworldlib-0.2021.10/setup.cfg` & `mcworldlib-2023.7/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mcworldlib
-version = 0.2021.10
+version = 2023.7
 author = Rodrigo Silva (MestreLion)
 author_email = minecraft@rodrigosilva.com
 description = Yet another python library to manipulate Minecraft save data
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3+
 license_files = LICENSE
@@ -24,27 +24,27 @@
 	Development Status :: 1 - Planning
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Games/Entertainment
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
-	nbtlib <= 1.6.3
+	nbtlib >= 2.0.4
 	numpy
 	tqdm
 
 [options.package_data]
 * = *.md, LICENSE*, */py.typed
 
 [egg_info]
```

### Comparing `mcworldlib-0.2021.10/LICENSE` & `mcworldlib-2023.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mcworldlib-0.2021.10/README.md` & `mcworldlib-2023.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
   blocks, entities and so on.
 
 - **CLI**: Add a command-line interface for commonly used operations.
 
 See the [To-Do List](./TODO.txt) for more updated technical information and
 planned features.
 
-If you find a bug or have any enhancement request, please to open a
+If you find a bug or have any enhancement request, please open a
 [new issue](https://github.com/MestreLion/mcworldlib/issues/new)
 
 
 Author
 ------
 
 Rodrigo Silva (MestreLion) <linux@rodrigosilva.com>
```

### Comparing `mcworldlib-0.2021.10/mcworldlib.egg-info/PKG-INFO` & `mcworldlib-2023.7/mcworldlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: mcworldlib
-Version: 0.2021.10
+Version: 2023.7
 Summary: Yet another python library to manipulate Minecraft save data
 Home-page: https://github.com/MestreLion/mcworldlib
 Author: Rodrigo Silva (MestreLion)
 Author-email: minecraft@rodrigosilva.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/MestreLion/mcworldlib/issues
 Project-URL: Source Code, https://github.com/MestreLion/mcworldlib
 Keywords: minecraft,save,nbt,chunk,region,world,library
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mcworldlib - Minecraft World Library
 
 Yet another library to manipulate Minecraft data, inspired by the now-defunct
 [pymclevel](https://github.com/mcedit/pymclevel), building on top of the amazing
@@ -392,15 +391,15 @@
   blocks, entities and so on.
 
 - **CLI**: Add a command-line interface for commonly used operations.
 
 See the [To-Do List](./TODO.txt) for more updated technical information and
 planned features.
 
-If you find a bug or have any enhancement request, please to open a
+If you find a bug or have any enhancement request, please open a
 [new issue](https://github.com/MestreLion/mcworldlib/issues/new)
 
 
 Author
 ------
 
 Rodrigo Silva (MestreLion) <linux@rodrigosilva.com>
@@ -412,9 +411,7 @@
 
 License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>.
 
 This is free software: you are free to change and redistribute it.
 
 There is NO WARRANTY, to the extent permitted by law.
 ```
-
-
```

