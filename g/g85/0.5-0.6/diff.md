# Comparing `tmp/g85-0.5.tar.gz` & `tmp/g85-0.6.tar.gz`

## Comparing `g85-0.5.tar` & `g85-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 g85-0.5/.flake8
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 g85-0.5/g85/LICENSE.md -> ../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 g85-0.5/g85/README.md -> ../README.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 g85-0.5/g85/__init__.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 g85-0.5/g85/main.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 g85-0.5/g85/read.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 g85-0.5/g85/write.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 g85-0.5/samples/ex.xml
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 g85-0.5/samples/ex2.xml
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 g85-0.5/.gitignore
--rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 g85-0.5/LICENSE.md
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 g85-0.5/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 g85-0.5/pyproject.toml
--rw-r--r--   0        0        0    40859 2020-02-02 00:00:00.000000 g85-0.5/PKG-INFO
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 g85-0.6/.flake8
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 g85-0.6/g85/LICENSE.md -> ../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 g85-0.6/g85/README.md -> ../README.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 g85-0.6/g85/__init__.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 g85-0.6/g85/main.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 g85-0.6/g85/read.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 g85-0.6/g85/write.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 g85-0.6/samples/ex.xml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 g85-0.6/samples/ex2.xml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 g85-0.6/.gitignore
+-rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 g85-0.6/LICENSE.md
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 g85-0.6/README.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 g85-0.6/pyproject.toml
+-rw-r--r--   0        0        0    40885 2020-02-02 00:00:00.000000 g85-0.6/PKG-INFO
```

### Comparing `g85-0.5/.flake8` & `g85-0.6/.flake8`

 * *Files identical despite different names*

### Comparing `g85-0.5/g85/read.py` & `g85-0.6/g85/read.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import List, Union, TextIO, Any
+from typing import TextIO, Any
 import logging
 import datetime
 from dataclasses import fields
 from xml.etree import ElementTree
 
 from .main import Map, Device
 
 
 logger = logging.getLogger(__name__)
 
 
-def read(stream: TextIO) -> List[Map]:
+def read(stream: TextIO) -> list[Map]:
     tree = ElementTree.parse(stream)
     el_root = tree.getroot()
 
     if _tag(el_root) != 'Maps':
         logger.warning(f'Root tag is "{_tag(el_root)}", expected "Maps"')
 
     maps = read_wmaps(el_root)
     return maps
 
 
-def read_wmaps(el_root: ElementTree.Element) -> List[Map]:
+def read_wmaps(el_root: ElementTree.Element) -> list[Map]:
     map_fields = [ff.name for ff in fields(Map)]
     maps = []
     for el_map in el_root:
         if _tag(el_map) != 'Map':
             logger.warning(f'Skipping map-level tag "{_tag(el_map)}"')
             continue
 
@@ -37,24 +37,24 @@
             else:
                 wmap.misc[key] = val
         wmap.devices = read_devices(el_map)
         maps.append(wmap)
     return maps
 
 
-def read_devices(el_map: ElementTree.Element) -> List[Device]:
+def read_devices(el_map: ElementTree.Element) -> list[Device]:
     dev_fields = [ff.name for ff in fields(Device)]
     devices = []
     for el_device in el_map:
         if _tag(el_device) != 'Device':
             logger.warning(f'Skipping device-level tag "{_tag(el_device)}"')
             continue
 
         bin_type = el_device.attrib['BinType']
-        null_bin: Union[int, str]
+        null_bin: int | str
         if bin_type == 'Decimal':
             null_bin = int(el_device.attrib['NullBin'])
         else:
             null_bin = el_device.attrib['NullBin']
 
         device = Device(BinType=bin_type, NullBin=null_bin)
 
@@ -95,34 +95,40 @@
                     logger.error(f'Bin without any associated BinCode, '
                                  f'with attributes {el_entry.attrib}')
                     continue
 
                 if bin_type == 'Decimal':
                     bin_code = int(attrib['BinCode'])
                 else:
-                    bin_code = int(attrib['BinCode'])
+                    bin_code = attrib['BinCode']
 
                 if bin_code in device.bin_pass:
                     logger.error(f'Bin code {bin_code} was repeated; ignoring later entry!')
                     continue
 
                 device.bin_pass[bin_code] = attrib['BinQuality'].lower() == 'pass'
             elif tag == 'Data':
                 data_strs = [read_row(rr) for rr in el_entry]
-                data: Union[List[List[str]], List[List[int]]]
+                data: list[list[str]] | list[list[int]]
                 if device.BinType == 'Decimal':
                     data = [[int(vv) for vv in rr] for rr in data_strs]
                 else:
                     data = data_strs
                 device.map = data
+                for key, value in attrib.items():
+                    device.data_misc[key] = value
+            elif tag == 'SupplierData':
+                for key, value in attrib.items():
+                    device.supplier_data[key] = value
+
         devices.append(device)
     return devices
 
 
-def read_row(el_row: ElementTree.Element) -> List[str]:
+def read_row(el_row: ElementTree.Element) -> list[str]:
     assert _tag(el_row) == 'Row'
 
     row_stripped = (el_row.text or '').strip()
     if ' ' in row_stripped or '\t' in row_stripped:
         row_data = row_stripped.split()
     else:
         row_data = list(row_stripped)
```

### Comparing `g85-0.5/g85/write.py` & `g85-0.6/g85/write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence, Tuple, List, TextIO, Union
+from typing import Sequence, TextIO, cast
 import logging
 import math
 from dataclasses import fields
 from xml.etree import ElementTree
 
 from .main import Map, Device
 
@@ -37,15 +37,15 @@
 def write_wmap(wmap: Map, el_root: ElementTree.Element) -> None:
     el_map = ElementTree.SubElement(el_root, 'Map')
 
     write_devices(wmap.devices, el_map)
 
     map_fields = [ff.name for ff in fields(wmap)]
     for field in map_fields:
-        if field[0].isupper():
+        if field[0].isupper() or field == 'xmlns':
             val = getattr(wmap, field)
             if val is None:
                 continue
             el_map.set(field, val)
     for key, value in wmap.misc.items():
         if key[0].isupper() and key in map_fields:
             continue
@@ -80,16 +80,17 @@
             if is_decimal:
                 el_bin.set('BinCode', str(bin_code).zfill(bin_length))
             else:
                 el_bin.set('BinCode', str(bin_code))
             el_bin.set('BinQuality', 'Pass' if passed else 'Fail')
             el_bin.set('BinCount', str(bin_counts[bin_code]))
 
+        el_data = ElementTree.SubElement(el_device, 'Data')
         for row_text in row_texts:
-            el_row = ElementTree.SubElement(el_device, 'Row')
+            el_row = ElementTree.SubElement(el_data, 'Row')
             el_row.text = f'<![CDATA[{row_text}]]>'
 
         # Device attribs
         dev_fields = [ff.name for ff in fields(device)]
         for field in dev_fields:
             if field[0].isupper():
                 val = getattr(device, field)
@@ -108,31 +109,38 @@
                 el_device.set(field, val)
 
         for key, value in device.misc.items():
             if key[0].isupper() and key in dev_fields:
                 continue
             el_device.set(key, value)
 
+        for key, value in device.data_misc.items():
+            el_data.set(key, value)
 
-def prepare_data(data: List[List[Union[str, int]]], decimal: bool) -> Tuple[List[str], int]:
+        if device.supplier_data:
+            el_suppdata = ElementTree.SubElement(el_device, 'SupplierData')
+            for key, value in device.data_misc.items():
+                el_suppdata.set(key, value)
+
+
+def prepare_data(data: list[list[str]] | list[list[int]], decimal: bool) -> tuple[list[str], int]:
     is_char = isinstance(data[0][0], str)
 
+    row_texts = []
     if is_char:
+        data = cast(list[list[str]], data)
         char_len = len(data[0][0])
+        for srow in data:
+            if char_len == 1:
+                row_text = ''.join(srow)
+            else:
+                row_text = ' '.join(srow) + ' '
+            row_texts.append(row_text)
+        return row_texts, char_len
     else:
+        data = cast(list[list[int]], data)
         max_value = max(max(rr) for rr in data)
         max_digits = math.ceil(math.log10(max_value))
-
-    row_texts = []
-    for row in data:
-        if is_char and char_len == 1:
-            row_text = ''.join(row)
-        elif is_char:
-            row_text = ' '.join(row) + ' '
-        else:
-            row_text = ' '.join(str(vv).zfill(max_digits) for vv in row) + ' '
-        row_texts.append(row_text)
-
-    if is_char:
-        return row_texts, char_len
-    else:
+        for irow in data:
+            row_text = ' '.join(str(vv).zfill(max_digits) for vv in irow) + ' '
+            row_texts.append(row_text)
         return row_texts, max_digits
```

### Comparing `g85-0.5/samples/ex.xml` & `g85-0.6/samples/ex.xml`

 * *Files identical despite different names*

### Comparing `g85-0.5/samples/ex2.xml` & `g85-0.6/samples/ex2.xml`

 * *Files identical despite different names*

### Comparing `g85-0.5/LICENSE.md` & `g85-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `g85-0.5/pyproject.toml` & `g85-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Manufacturing",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
     ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dynamic = ["version"]
 dependencies = [
     "numpy~=1.21",
     ]
 
 [tool.hatch.version]
 path = "g85/__init__.py"
```

### Comparing `g85-0.5/PKG-INFO` & `g85-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g85
-Version: 0.5
+Version: 0.6
 Summary: G85 wafer map reader / writer
 Author-email: Jan Petykiewicz <jan@mpxd.net>
 License: GNU General Public License
         ==========================
         
         _Version 3, 29 June 2007_  
         _Copyright © 2007 Free Software Foundation, Inc. &lt;<http://fsf.org/>&gt;_
@@ -594,24 +594,25 @@
         
         The GNU General Public License does not permit incorporating your program into
         proprietary programs. If your program is a subroutine library, you may consider it
         more useful to permit linking proprietary applications with the library. If this is
         what you want to do, use the GNU Lesser General Public License instead of this
         License. But first, please read
         &lt;<http://www.gnu.org/philosophy/why-not-lgpl.html>&gt;.
+License-File: LICENSE.md
 Keywords: CAD,EDA,G85,IC,design,electronics,map,mask,photonics,wafer,wmap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: numpy~=1.21
 Description-Content-Type: text/markdown
 
 # g85 README
 
 `g85` is a Python module for reading and writing to the G85 XML wafer map format.
```

