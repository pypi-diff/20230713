# Comparing `tmp/mcworldlib-2023.7.tar.gz` & `tmp/mcworldlib-2023.7.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rodrigo/work/minecraft/mcworldlib/dist/.tmp-ontvqx11/mcworldlib-2023.7.tar", last modified: Thu Jul 13 01:09:16 2023, max compression
+gzip compressed data, was "/home/rodrigo/work/minecraft/mcworldlib/dist/.tmp-tnml7qgz/mcworldlib-2023.7.13.tar", last modified: Thu Jul 13 05:38:25 2023, max compression
```

## Comparing `mcworldlib-2023.7.tar` & `mcworldlib-2023.7.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2019-12-10 03:18:22.000000 mcworldlib-2023.7/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14435 2023-07-13 01:09:16.610249 mcworldlib-2023.7/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    13211 2023-07-13 00:36:20.000000 mcworldlib-2023.7/README.md
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/mcworldlib/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1536 2021-10-31 04:36:50.000000 mcworldlib-2023.7/mcworldlib/__init__.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    18899 2021-10-31 21:36:14.000000 mcworldlib-2023.7/mcworldlib/anvil.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4789 2023-07-12 19:16:33.000000 mcworldlib-2023.7/mcworldlib/chunk.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2183 2021-10-10 01:17:47.000000 mcworldlib-2023.7/mcworldlib/cli.py
--rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1672 2021-10-17 15:13:52.000000 mcworldlib-2023.7/mcworldlib/entity.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1616 2021-10-26 20:59:27.000000 mcworldlib-2023.7/mcworldlib/level.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     9469 2023-07-13 00:59:22.000000 mcworldlib-2023.7/mcworldlib/nbt.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1067 2021-10-20 11:36:27.000000 mcworldlib-2023.7/mcworldlib/player.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     8135 2021-10-31 21:26:47.000000 mcworldlib-2023.7/mcworldlib/tree.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    12279 2021-10-27 04:04:00.000000 mcworldlib-2023.7/mcworldlib/util.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    10808 2021-11-01 01:25:32.000000 mcworldlib-2023.7/mcworldlib/world.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/mcworldlib.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14435 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      445 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       25 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/requires.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       11 2023-07-13 01:09:16.000000 mcworldlib-2023.7/mcworldlib.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      544 2021-10-31 22:06:22.000000 mcworldlib-2023.7/pyproject.toml
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1336 2023-07-13 01:09:16.610249 mcworldlib-2023.7/setup.cfg
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 01:09:16.610249 mcworldlib-2023.7/tests/
--rwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)     6834 2021-10-31 21:27:07.000000 mcworldlib-2023.7/tests/tests.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 05:38:25.590999 mcworldlib-2023.7.13/
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2019-12-10 03:18:22.000000 mcworldlib-2023.7.13/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14529 2023-07-13 05:38:25.590999 mcworldlib-2023.7.13/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    13302 2023-07-13 05:05:47.000000 mcworldlib-2023.7.13/README.md
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 05:38:25.586998 mcworldlib-2023.7.13/mcworldlib/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1536 2021-10-31 04:36:50.000000 mcworldlib-2023.7.13/mcworldlib/__init__.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    18916 2023-07-13 04:26:57.000000 mcworldlib-2023.7.13/mcworldlib/anvil.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     4789 2023-07-13 04:28:26.000000 mcworldlib-2023.7.13/mcworldlib/chunk.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     2183 2021-10-10 01:17:47.000000 mcworldlib-2023.7.13/mcworldlib/cli.py
+-rw-r--r--   0 rodrigo   (1000) rodrigo   (1000)     1672 2021-10-17 15:13:52.000000 mcworldlib-2023.7.13/mcworldlib/entity.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1616 2021-10-26 20:59:27.000000 mcworldlib-2023.7.13/mcworldlib/level.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    11078 2023-07-13 05:33:59.000000 mcworldlib-2023.7.13/mcworldlib/nbt.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1067 2021-10-20 11:36:27.000000 mcworldlib-2023.7.13/mcworldlib/player.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     8135 2021-10-31 21:26:47.000000 mcworldlib-2023.7.13/mcworldlib/tree.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    12279 2021-10-27 04:04:00.000000 mcworldlib-2023.7.13/mcworldlib/util.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    10808 2021-11-01 01:25:32.000000 mcworldlib-2023.7.13/mcworldlib/world.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 05:38:25.586998 mcworldlib-2023.7.13/mcworldlib.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    14529 2023-07-13 05:38:25.000000 mcworldlib-2023.7.13/mcworldlib.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      445 2023-07-13 05:38:25.000000 mcworldlib-2023.7.13/mcworldlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-07-13 05:38:25.000000 mcworldlib-2023.7.13/mcworldlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       25 2023-07-13 05:38:25.000000 mcworldlib-2023.7.13/mcworldlib.egg-info/requires.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       11 2023-07-13 05:38:25.000000 mcworldlib-2023.7.13/mcworldlib.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      544 2021-10-31 22:06:22.000000 mcworldlib-2023.7.13/pyproject.toml
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1339 2023-07-13 05:38:25.590999 mcworldlib-2023.7.13/setup.cfg
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-07-13 05:38:25.590999 mcworldlib-2023.7.13/tests/
+-rwxr-xr-x   0 rodrigo   (1000) rodrigo   (1000)     6834 2021-10-31 21:27:07.000000 mcworldlib-2023.7.13/tests/tests.py
```

### Comparing `mcworldlib-2023.7/LICENSE` & `mcworldlib-2023.7.13/LICENSE`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/PKG-INFO` & `mcworldlib-2023.7.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcworldlib
-Version: 2023.7
+Version: 2023.7.13
 Summary: Yet another python library to manipulate Minecraft save data
 Home-page: https://github.com/MestreLion/mcworldlib
 Author: Rodrigo Silva (MestreLion)
 Author-email: minecraft@rodrigosilva.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/MestreLion/mcworldlib/issues
 Project-URL: Source Code, https://github.com/MestreLion/mcworldlib
@@ -96,30 +96,30 @@
 
 `World.dimensions` is a dictionary mapping each dimension to categorized Region files:
 ```pycon
 >>> mc.pretty(world.dimensions)
 {   <Dimension.OVERWORLD: 0>: {   'entities': <Regions(6 regions)>,
                                   'poi': <Regions(0 regions)>,
                                   'region': <Regions(6 regions)>},
-    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
-                                'poi': <Regions(0 regions)>,
-                                'region': <Regions(0 regions)>},
     <Dimension.THE_NETHER: -1>: {   'entities': <Regions(0 regions)>,
                                     'poi': <Regions(0 regions)>,
-                                    'region': <Regions(0 regions)>}}
+                                    'region': <Regions(0 regions)>},
+    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
+                                'poi': <Regions(0 regions)>,
+                                'region': <Regions(0 regions)>}}
 
 ```
 
 And `World.regions` is handy view of that dictionary containing only the 'region'
 category, similarly with `World.entities` and `World.poi`:
 ```pycon
 >>> mc.pretty(world.regions)
 {   <Dimension.OVERWORLD: 0>: <Regions(6 regions)>,
-    <Dimension.THE_END: 1>: <Regions(0 regions)>,
-    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>}
+    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>,
+    <Dimension.THE_END: 1>: <Regions(0 regions)>}
 
 >>> regions = world.regions[mc.OVERWORLD]
 >>> regions is world.dimensions[mc.OVERWORLD]['region']
 True
 
 ```
 
@@ -202,15 +202,15 @@
 
 ```
 
 Get the block info at any coordinate:
 ```pycon
 >>> block = world.get_block_at((100, 60, 100))
 >>> print(block)
-{Name: "minecraft:stone"}
+Compound({'Name': String('minecraft:stone')})
 
 ```
 
 Remember the automatic, lazy-loading feature of `Regions`? In the above examples
 a few chunks from distinct regions were accessed. So what is the state of the
 `regions` dictionary now?
 
@@ -324,49 +324,49 @@
 │  ├──⊟ Disabled: 1 entry
 │  │  ╰─── 0: Fabric Mods
 │  ╰──⊟ Enabled: 1 entry
 │     ╰─── 0: vanilla
 ...
 ├──⊟ Player: 37 entries
 │  ├──⊟ abilities: 7 entries
-│  │  ├─── flying: 0b
+│  │  ├─── flying: Byte(0)
 ...
-│  │  ╰─── walkSpeed: 0.10000000149011612f
+│  │  ╰─── walkSpeed: Float(0.10000000149011612)
 │  ├──⊟ Brain: 1 entry
 │  │  ╰──⊞ memories: 0 entries
 ...
 │  ├──⊟ Inventory: 11 entries
 │  │  ├──⊟  0: 4 entries
 │  │  │  ├──⊟ tag: 1 entry
-│  │  │  │  ╰─── Damage: 0
-│  │  │  ├─── Count: 1b
+│  │  │  │  ╰─── Damage: Int(0)
+│  │  │  ├─── Count: Byte(1)
 │  │  │  ├─── id: minecraft:stone_axe
-│  │  │  ╰─── Slot: 0b
+│  │  │  ╰─── Slot: Byte(0)
 ...
 │  │  ╰──⊟ 10: 4 entries
 │  │     ├──⊟ tag: 1 entry
-│  │     │  ╰─── Damage: 18
-│  │     ├─── Count: 1b
+│  │     │  ╰─── Damage: Int(18)
+│  │     ├─── Count: Byte(1)
 │  │     ├─── id: minecraft:wooden_pickaxe
-│  │     ╰─── Slot: 28b
+│  │     ╰─── Slot: Byte(28)
 ...
-│  ├─── XpTotal: 37
+│  ├─── XpTotal: Int(37)
 │  ╰──⊕ UUID: 4 entries
 ├──⊟ Version: 3 entries
-│  ├─── Id: 2730
+│  ├─── Id: Int(2730)
 │  ├─── Name: 1.17.1
-│  ╰─── Snapshot: 0b
+│  ╰─── Snapshot: Byte(0)
 ...
 ├──⊞ ScheduledEvents: 0 entries
 ├──⊟ ServerBrands: 1 entry
 │  ╰─── 0: fabric
-├─── allowCommands: 0b
+├─── allowCommands: Byte(0)
 ...
-├─── WanderingTraderSpawnDelay: 19200
-╰─── WasModded: 1b
+├─── WanderingTraderSpawnDelay: Int(19200)
+╰─── WasModded: Byte(1)
 
 ```
 You want to click that tree, don't you? Sweet `Array` "icon" for `UUID`!
 
 Test yourself all the examples in this document:
 
     python3 -m doctest -f -o ELLIPSIS -o NORMALIZE_WHITESPACE README.md
```

### Comparing `mcworldlib-2023.7/README.md` & `mcworldlib-2023.7.13/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,30 +68,30 @@
 
 `World.dimensions` is a dictionary mapping each dimension to categorized Region files:
 ```pycon
 >>> mc.pretty(world.dimensions)
 {   <Dimension.OVERWORLD: 0>: {   'entities': <Regions(6 regions)>,
                                   'poi': <Regions(0 regions)>,
                                   'region': <Regions(6 regions)>},
-    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
-                                'poi': <Regions(0 regions)>,
-                                'region': <Regions(0 regions)>},
     <Dimension.THE_NETHER: -1>: {   'entities': <Regions(0 regions)>,
                                     'poi': <Regions(0 regions)>,
-                                    'region': <Regions(0 regions)>}}
+                                    'region': <Regions(0 regions)>},
+    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
+                                'poi': <Regions(0 regions)>,
+                                'region': <Regions(0 regions)>}}
 
 ```
 
 And `World.regions` is handy view of that dictionary containing only the 'region'
 category, similarly with `World.entities` and `World.poi`:
 ```pycon
 >>> mc.pretty(world.regions)
 {   <Dimension.OVERWORLD: 0>: <Regions(6 regions)>,
-    <Dimension.THE_END: 1>: <Regions(0 regions)>,
-    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>}
+    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>,
+    <Dimension.THE_END: 1>: <Regions(0 regions)>}
 
 >>> regions = world.regions[mc.OVERWORLD]
 >>> regions is world.dimensions[mc.OVERWORLD]['region']
 True
 
 ```
 
@@ -174,15 +174,15 @@
 
 ```
 
 Get the block info at any coordinate:
 ```pycon
 >>> block = world.get_block_at((100, 60, 100))
 >>> print(block)
-{Name: "minecraft:stone"}
+Compound({'Name': String('minecraft:stone')})
 
 ```
 
 Remember the automatic, lazy-loading feature of `Regions`? In the above examples
 a few chunks from distinct regions were accessed. So what is the state of the
 `regions` dictionary now?
 
@@ -296,49 +296,49 @@
 │  ├──⊟ Disabled: 1 entry
 │  │  ╰─── 0: Fabric Mods
 │  ╰──⊟ Enabled: 1 entry
 │     ╰─── 0: vanilla
 ...
 ├──⊟ Player: 37 entries
 │  ├──⊟ abilities: 7 entries
-│  │  ├─── flying: 0b
+│  │  ├─── flying: Byte(0)
 ...
-│  │  ╰─── walkSpeed: 0.10000000149011612f
+│  │  ╰─── walkSpeed: Float(0.10000000149011612)
 │  ├──⊟ Brain: 1 entry
 │  │  ╰──⊞ memories: 0 entries
 ...
 │  ├──⊟ Inventory: 11 entries
 │  │  ├──⊟  0: 4 entries
 │  │  │  ├──⊟ tag: 1 entry
-│  │  │  │  ╰─── Damage: 0
-│  │  │  ├─── Count: 1b
+│  │  │  │  ╰─── Damage: Int(0)
+│  │  │  ├─── Count: Byte(1)
 │  │  │  ├─── id: minecraft:stone_axe
-│  │  │  ╰─── Slot: 0b
+│  │  │  ╰─── Slot: Byte(0)
 ...
 │  │  ╰──⊟ 10: 4 entries
 │  │     ├──⊟ tag: 1 entry
-│  │     │  ╰─── Damage: 18
-│  │     ├─── Count: 1b
+│  │     │  ╰─── Damage: Int(18)
+│  │     ├─── Count: Byte(1)
 │  │     ├─── id: minecraft:wooden_pickaxe
-│  │     ╰─── Slot: 28b
+│  │     ╰─── Slot: Byte(28)
 ...
-│  ├─── XpTotal: 37
+│  ├─── XpTotal: Int(37)
 │  ╰──⊕ UUID: 4 entries
 ├──⊟ Version: 3 entries
-│  ├─── Id: 2730
+│  ├─── Id: Int(2730)
 │  ├─── Name: 1.17.1
-│  ╰─── Snapshot: 0b
+│  ╰─── Snapshot: Byte(0)
 ...
 ├──⊞ ScheduledEvents: 0 entries
 ├──⊟ ServerBrands: 1 entry
 │  ╰─── 0: fabric
-├─── allowCommands: 0b
+├─── allowCommands: Byte(0)
 ...
-├─── WanderingTraderSpawnDelay: 19200
-╰─── WasModded: 1b
+├─── WanderingTraderSpawnDelay: Int(19200)
+╰─── WasModded: Byte(1)
 
 ```
 You want to click that tree, don't you? Sweet `Array` "icon" for `UUID`!
 
 Test yourself all the examples in this document:
 
     python3 -m doctest -f -o ELLIPSIS -o NORMALIZE_WHITESPACE README.md
```

### Comparing `mcworldlib-2023.7/mcworldlib/__init__.py` & `mcworldlib-2023.7.13/mcworldlib/__init__.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/anvil.py` & `mcworldlib-2023.7.13/mcworldlib/anvil.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,16 +433,18 @@
         except struct.error as e:
             raise ChunkError(f"chunk header has {len(header)} bytes" +
                              (f"({''.join(f'{_:X}' for _ in header)})"
                               if header else "") + f", {e}")
 
         external, compression = cls._unpack_compression(compression)
         if compression not in COMPRESSION_TYPES:
-            raise ChunkError('Invalid compression type, must be one of'
-                             f' {COMPRESSION_TYPES}: {compression}')
+            raise ChunkError(
+                "Invalid compression type, must be one of "
+                f"{COMPRESSION_TYPES}: {compression}"
+            )
 
         if external:
             raise ChunkError('External MCC data file is not yet supported')
 
         data = cls.decompress[compression](buff.read(length))
         self: T = super().parse(io.BytesIO(data), *args, **kwargs)
```

### Comparing `mcworldlib-2023.7/mcworldlib/chunk.py` & `mcworldlib-2023.7.13/mcworldlib/chunk.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/cli.py` & `mcworldlib-2023.7.13/mcworldlib/cli.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/entity.py` & `mcworldlib-2023.7.13/mcworldlib/entity.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/level.py` & `mcworldlib-2023.7.13/mcworldlib/level.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/nbt.py` & `mcworldlib-2023.7.13/mcworldlib/nbt.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 import zlib    as _zlib
 
 # TODO: (and suggest to nbtlib)
 # - Auto-casting value to tag on assignment based on current type
 #   - compound['string'] = 'foo' -> compound['string'] = String('foo')
 #   - maybe this is only meant for nbtlib.Schema?
 
+# not in nbtlib.tag.__all__ and only used in Root
+# noinspection PyProtectedMember
+from nbtlib.tag import (
+    BYTE as _BYTE,
+    read_numeric as _read_numeric,
+    read_string as _read_string,
+    write_numeric as _write_numeric,
+    write_string as _write_string,
+)
+
 from nbtlib.tag import *
 from nbtlib.tag import Array  # Not in __all__, but used by others
 from nbtlib.nbt import File as _File  # intentionally not importing load
 from nbtlib.path import Path
 from nbtlib.literal.serializer import serialize_tag as _serialize_tag
 
 from . import tree as _tree
@@ -55,15 +65,21 @@
 
 RT = t.TypeVar('RT', bound='Root')
 
 
 class Root(Compound):
     """Unnamed Compound tag, the root tag in files and chunks"""
 
-    __slots__ = ()
+    __slots__ = (
+        'root_name',
+    )
+
+    def __init__(self, *args, root_name: str = "", **kwargs):
+        super().__init__(*args, **kwargs)
+        self.root_name: str = root_name
 
     @property
     def data_root(self) -> Compound:
         """Root itself or the child containing all data apart from DataVersion.
 
         A convenience shortcut for root compounds that contains just DataVersion
         and another tag, and all relevant data is in that tag, as is the case for
@@ -87,23 +103,45 @@
         tags = self.keys() - {'DataVersion'}
         if not len(tags) == 1:
             return "", self
         name = next(iter(tags))
         # FIXME: Should make sure it's actually a Compound and not just AnyTag
         return name, self[name]
 
-    # Move some methods from File. Keeping them there would confuse super() calls
-    parse = _File.parse; del _File.parse
-    write = _File.write; del _File.write
+    # Copy parse() and write() methods from _File
+
+    @classmethod
+    def parse(cls: t.Type[RT], fileobj, byteorder='big') -> RT:
+        """Override :meth:`nbtlib.tag.Base.parse` for nbt files."""
+        # For the typing dance, see https://stackoverflow.com/a/44644576/624066
+        tag_id = _read_numeric(_BYTE, fileobj, byteorder)
+        if not tag_id == cls.tag_id:
+            # Possible issues with a non-Compound root:
+            # - root_name might not be in __slots__(), and thus not assignable
+            # - not returning a superclass might be surprising and have side effects
+            raise TypeError(
+                f"Non-Compound root tag is not supported: {cls.get_tag(tag_id)}"
+            )
+        name = _read_string(fileobj, byteorder)
+        self: RT = super().parse(fileobj, byteorder)
+        self.root_name = name
+        return self
+
+    def write(self, fileobj, byteorder="big"):
+        """Override :meth:`nbtlib.tag.Base.write` for nbt files."""
+        _write_numeric(_BYTE, self.tag_id, fileobj, byteorder)
+        _write_string(self.root_name, fileobj, byteorder)
+        super().write(fileobj, byteorder)
 
     def __repr__(self):
         key, data = self._data_root  # save refs for efficiency
         if key:
             key = f" ({len(data)} in {key!r})"
-        return f'<{self.__class__.__name__} tags: {len(self)}{key}>'
+        name = f" {self.root_name!r}" if self.root_name else ""
+        return f'<{self.__class__.__name__}{name} tags: {len(self)}{key}>'
 
 
 # Overrides and extensions
 
 class File(Root, _File):
     # Lame overload so it inherits from Root
     __slots__ = ()
@@ -259,12 +297,16 @@
 Base.pretty = lambda self, indent=4: _serialize_tag(self, indent=indent)
 
 Base.is_leaf = property(
     fget=lambda _: not isinstance(_, (Compound, List, Array)),
     doc="If this tag an immutable tag and not a Mutable Collection."
         " Non-leaves are the containers excluding String: Compound, List, Array")
 
+# Remove _File methods copied to Root so super() calls from File works properly
+del _File.parse
+del _File.write
+
 # Convenience shortcuts
 load_mcc = File.load_mcc
 load_dat = File.load
 
 del t
```

### Comparing `mcworldlib-2023.7/mcworldlib/player.py` & `mcworldlib-2023.7.13/mcworldlib/player.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/tree.py` & `mcworldlib-2023.7.13/mcworldlib/tree.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/util.py` & `mcworldlib-2023.7.13/mcworldlib/util.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib/world.py` & `mcworldlib-2023.7.13/mcworldlib/world.py`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/mcworldlib.egg-info/PKG-INFO` & `mcworldlib-2023.7.13/mcworldlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcworldlib
-Version: 2023.7
+Version: 2023.7.13
 Summary: Yet another python library to manipulate Minecraft save data
 Home-page: https://github.com/MestreLion/mcworldlib
 Author: Rodrigo Silva (MestreLion)
 Author-email: minecraft@rodrigosilva.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/MestreLion/mcworldlib/issues
 Project-URL: Source Code, https://github.com/MestreLion/mcworldlib
@@ -96,30 +96,30 @@
 
 `World.dimensions` is a dictionary mapping each dimension to categorized Region files:
 ```pycon
 >>> mc.pretty(world.dimensions)
 {   <Dimension.OVERWORLD: 0>: {   'entities': <Regions(6 regions)>,
                                   'poi': <Regions(0 regions)>,
                                   'region': <Regions(6 regions)>},
-    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
-                                'poi': <Regions(0 regions)>,
-                                'region': <Regions(0 regions)>},
     <Dimension.THE_NETHER: -1>: {   'entities': <Regions(0 regions)>,
                                     'poi': <Regions(0 regions)>,
-                                    'region': <Regions(0 regions)>}}
+                                    'region': <Regions(0 regions)>},
+    <Dimension.THE_END: 1>: {   'entities': <Regions(0 regions)>,
+                                'poi': <Regions(0 regions)>,
+                                'region': <Regions(0 regions)>}}
 
 ```
 
 And `World.regions` is handy view of that dictionary containing only the 'region'
 category, similarly with `World.entities` and `World.poi`:
 ```pycon
 >>> mc.pretty(world.regions)
 {   <Dimension.OVERWORLD: 0>: <Regions(6 regions)>,
-    <Dimension.THE_END: 1>: <Regions(0 regions)>,
-    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>}
+    <Dimension.THE_NETHER: -1>: <Regions(0 regions)>,
+    <Dimension.THE_END: 1>: <Regions(0 regions)>}
 
 >>> regions = world.regions[mc.OVERWORLD]
 >>> regions is world.dimensions[mc.OVERWORLD]['region']
 True
 
 ```
 
@@ -202,15 +202,15 @@
 
 ```
 
 Get the block info at any coordinate:
 ```pycon
 >>> block = world.get_block_at((100, 60, 100))
 >>> print(block)
-{Name: "minecraft:stone"}
+Compound({'Name': String('minecraft:stone')})
 
 ```
 
 Remember the automatic, lazy-loading feature of `Regions`? In the above examples
 a few chunks from distinct regions were accessed. So what is the state of the
 `regions` dictionary now?
 
@@ -324,49 +324,49 @@
 │  ├──⊟ Disabled: 1 entry
 │  │  ╰─── 0: Fabric Mods
 │  ╰──⊟ Enabled: 1 entry
 │     ╰─── 0: vanilla
 ...
 ├──⊟ Player: 37 entries
 │  ├──⊟ abilities: 7 entries
-│  │  ├─── flying: 0b
+│  │  ├─── flying: Byte(0)
 ...
-│  │  ╰─── walkSpeed: 0.10000000149011612f
+│  │  ╰─── walkSpeed: Float(0.10000000149011612)
 │  ├──⊟ Brain: 1 entry
 │  │  ╰──⊞ memories: 0 entries
 ...
 │  ├──⊟ Inventory: 11 entries
 │  │  ├──⊟  0: 4 entries
 │  │  │  ├──⊟ tag: 1 entry
-│  │  │  │  ╰─── Damage: 0
-│  │  │  ├─── Count: 1b
+│  │  │  │  ╰─── Damage: Int(0)
+│  │  │  ├─── Count: Byte(1)
 │  │  │  ├─── id: minecraft:stone_axe
-│  │  │  ╰─── Slot: 0b
+│  │  │  ╰─── Slot: Byte(0)
 ...
 │  │  ╰──⊟ 10: 4 entries
 │  │     ├──⊟ tag: 1 entry
-│  │     │  ╰─── Damage: 18
-│  │     ├─── Count: 1b
+│  │     │  ╰─── Damage: Int(18)
+│  │     ├─── Count: Byte(1)
 │  │     ├─── id: minecraft:wooden_pickaxe
-│  │     ╰─── Slot: 28b
+│  │     ╰─── Slot: Byte(28)
 ...
-│  ├─── XpTotal: 37
+│  ├─── XpTotal: Int(37)
 │  ╰──⊕ UUID: 4 entries
 ├──⊟ Version: 3 entries
-│  ├─── Id: 2730
+│  ├─── Id: Int(2730)
 │  ├─── Name: 1.17.1
-│  ╰─── Snapshot: 0b
+│  ╰─── Snapshot: Byte(0)
 ...
 ├──⊞ ScheduledEvents: 0 entries
 ├──⊟ ServerBrands: 1 entry
 │  ╰─── 0: fabric
-├─── allowCommands: 0b
+├─── allowCommands: Byte(0)
 ...
-├─── WanderingTraderSpawnDelay: 19200
-╰─── WasModded: 1b
+├─── WanderingTraderSpawnDelay: Int(19200)
+╰─── WasModded: Byte(1)
 
 ```
 You want to click that tree, don't you? Sweet `Array` "icon" for `UUID`!
 
 Test yourself all the examples in this document:
 
     python3 -m doctest -f -o ELLIPSIS -o NORMALIZE_WHITESPACE README.md
```

### Comparing `mcworldlib-2023.7/pyproject.toml` & `mcworldlib-2023.7.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcworldlib-2023.7/setup.cfg` & `mcworldlib-2023.7.13/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mcworldlib
-version = 2023.7
+version = 2023.7.13
 author = Rodrigo Silva (MestreLion)
 author_email = minecraft@rodrigosilva.com
 description = Yet another python library to manipulate Minecraft save data
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3+
 license_files = LICENSE
```

### Comparing `mcworldlib-2023.7/tests/tests.py` & `mcworldlib-2023.7.13/tests/tests.py`

 * *Files identical despite different names*

