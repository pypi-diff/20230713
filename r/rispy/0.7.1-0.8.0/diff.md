# Comparing `tmp/rispy-0.7.1.tar.gz` & `tmp/rispy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rispy-0.7.1.tar", last modified: Wed Jun  2 01:52:22 2021, max compression
+gzip compressed data, was "rispy-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rispy-0.7.1.tar` & `rispy-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,31 @@
-drwxr-xr-x   0 shapiromatron   (501) staff       (20)        0 2021-06-02 01:52:22.000000 rispy-0.7.1/
-drwxr-xr-x   0 shapiromatron   (501) staff       (20)        0 2021-06-02 01:52:22.000000 rispy-0.7.1/rispy/
--rw-r--r--   0 shapiromatron   (501) staff       (20)     5713 2021-06-01 20:21:10.000000 rispy-0.7.1/rispy/config.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)      513 2021-06-02 01:51:01.000000 rispy-0.7.1/rispy/__init__.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)    12227 2021-06-01 20:21:10.000000 rispy-0.7.1/rispy/parser.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1624 2021-06-01 20:21:10.000000 rispy-0.7.1/rispy/utils.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)     7206 2021-06-01 21:14:41.000000 rispy-0.7.1/rispy/writer.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)    11195 2021-06-02 01:52:22.000000 rispy-0.7.1/PKG-INFO
--rw-r--r--   0 shapiromatron   (501) staff       (20)       42 2019-03-21 21:47:19.000000 rispy-0.7.1/pytest.ini
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1070 2021-06-01 21:27:13.000000 rispy-0.7.1/LICENSE
--rw-r--r--   0 shapiromatron   (501) staff       (20)      195 2021-06-02 01:34:52.000000 rispy-0.7.1/pyproject.toml
-drwxr-xr-x   0 shapiromatron   (501) staff       (20)        0 2021-06-02 01:52:22.000000 rispy-0.7.1/tests/
--rw-r--r--   0 shapiromatron   (501) staff       (20)    15243 2021-06-01 20:21:10.000000 rispy-0.7.1/tests/test_parser.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)     3487 2021-06-01 20:21:10.000000 rispy-0.7.1/tests/test_writer.py
-drwxr-xr-x   0 shapiromatron   (501) staff       (20)        0 2021-06-02 01:52:22.000000 rispy-0.7.1/tests/data/
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1757 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_full_without_whitespace.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)       98 2021-06-01 20:21:10.000000 rispy-0.7.1/tests/data/example_custom_list_tags.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      202 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_single_unknown_tag.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1901 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_extraneous_data.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      192 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_multi_unknown_tags.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      910 2021-06-01 20:21:10.000000 rispy-0.7.1/tests/data/example_utf_chars.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)       54 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_bom.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)    16195 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_wos.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1759 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_full.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)     1617 2021-06-02 01:30:40.000000 rispy-0.7.1/tests/data/example_full_write.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      170 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_starting_newlines.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      302 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/multiline.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      168 2021-04-01 19:59:20.000000 rispy-0.7.1/tests/data/example_basic.ris
--rw-r--r--   0 shapiromatron   (501) staff       (20)      121 2019-03-21 21:47:19.000000 rispy-0.7.1/MANIFEST.in
--rw-r--r--   0 shapiromatron   (501) staff       (20)       69 2021-06-01 21:10:34.000000 rispy-0.7.1/setup.py
--rw-r--r--   0 shapiromatron   (501) staff       (20)     2568 2021-06-02 01:51:52.000000 rispy-0.7.1/HISTORY.rst
--rw-r--r--   0 shapiromatron   (501) staff       (20)      886 2021-06-02 01:52:22.000000 rispy-0.7.1/setup.cfg
-drwxr-xr-x   0 shapiromatron   (501) staff       (20)        0 2021-06-02 01:52:22.000000 rispy-0.7.1/rispy.egg-info/
--rw-r--r--   0 shapiromatron   (501) staff       (20)    11195 2021-06-02 01:52:21.000000 rispy-0.7.1/rispy.egg-info/PKG-INFO
--rw-r--r--   0 shapiromatron   (501) staff       (20)      808 2021-06-02 01:52:21.000000 rispy-0.7.1/rispy.egg-info/SOURCES.txt
--rw-r--r--   0 shapiromatron   (501) staff       (20)       80 2021-06-02 01:52:21.000000 rispy-0.7.1/rispy.egg-info/requires.txt
--rw-r--r--   0 shapiromatron   (501) staff       (20)        6 2021-06-02 01:52:21.000000 rispy-0.7.1/rispy.egg-info/top_level.txt
--rw-r--r--   0 shapiromatron   (501) staff       (20)        1 2021-06-02 01:52:21.000000 rispy-0.7.1/rispy.egg-info/dependency_links.txt
--rw-r--r--   0 shapiromatron   (501) staff       (20)    10453 2021-06-02 01:48:12.000000 rispy-0.7.1/README.rst
+-rw-r--r--   0        0        0       95 2023-06-07 11:31:31.290631 rispy-0.8.0/.flake8
+-rw-r--r--   0        0        0      573 2023-07-13 19:04:25.612108 rispy-0.8.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      245 2023-06-07 11:31:31.290980 rispy-0.8.0/.gitignore
+-rw-r--r--   0        0        0     3183 2023-07-13 19:04:35.135681 rispy-0.8.0/HISTORY.rst
+-rw-r--r--   0        0        0     1070 2023-07-13 19:04:25.612752 rispy-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1328 2023-07-13 19:04:25.613134 rispy-0.8.0/Makefile
+-rw-r--r--   0        0        0    10490 2023-07-13 19:04:25.613611 rispy-0.8.0/README.rst
+-rw-r--r--   0        0        0     1291 2023-07-13 19:04:25.614044 rispy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-07 11:31:31.291777 rispy-0.8.0/pytest.ini
+-rw-r--r--   0        0        0      525 2023-07-13 19:04:35.135988 rispy-0.8.0/rispy/__init__.py
+-rw-r--r--   0        0        0     5780 2023-07-13 16:16:46.968010 rispy-0.8.0/rispy/config.py
+-rw-r--r--   0        0        0    13412 2023-07-13 19:04:25.614790 rispy-0.8.0/rispy/parser.py
+-rw-r--r--   0        0        0     1640 2023-07-13 19:04:25.615134 rispy-0.8.0/rispy/utils.py
+-rw-r--r--   0        0        0     7552 2023-07-13 19:04:25.615512 rispy-0.8.0/rispy/writer.py
+-rw-r--r--   0        0        0      168 2023-06-07 11:31:31.292903 rispy-0.8.0/tests/data/example_basic.ris
+-rw-r--r--   0        0        0       54 2023-06-07 11:31:31.293000 rispy-0.8.0/tests/data/example_bom.ris
+-rw-r--r--   0        0        0       98 2023-06-07 11:31:31.293092 rispy-0.8.0/tests/data/example_custom_list_tags.ris
+-rw-r--r--   0        0        0     1901 2023-06-07 11:31:31.293273 rispy-0.8.0/tests/data/example_extraneous_data.ris
+-rw-r--r--   0        0        0     1759 2023-06-07 11:31:31.293426 rispy-0.8.0/tests/data/example_full.ris
+-rw-r--r--   0        0        0     1757 2023-06-07 11:31:31.293549 rispy-0.8.0/tests/data/example_full_without_whitespace.ris
+-rw-r--r--   0        0        0     1617 2023-07-13 19:04:52.587777 rispy-0.8.0/tests/data/example_full_write.ris
+-rw-r--r--   0        0        0      192 2023-06-07 11:31:31.293736 rispy-0.8.0/tests/data/example_multi_unknown_tags.ris
+-rw-r--r--   0        0        0      202 2023-06-07 11:31:31.293831 rispy-0.8.0/tests/data/example_single_unknown_tag.ris
+-rw-r--r--   0        0        0      170 2023-06-07 11:31:31.293924 rispy-0.8.0/tests/data/example_starting_newlines.ris
+-rw-r--r--   0        0        0      847 2023-07-11 15:17:37.154523 rispy-0.8.0/tests/data/example_urls.ris
+-rw-r--r--   0        0        0      910 2023-06-07 11:31:31.294031 rispy-0.8.0/tests/data/example_utf_chars.ris
+-rw-r--r--   0        0        0    16195 2023-06-07 11:31:31.294243 rispy-0.8.0/tests/data/example_wos.ris
+-rw-r--r--   0        0        0      302 2023-06-07 11:31:31.294342 rispy-0.8.0/tests/data/multiline.ris
+-rw-r--r--   0        0        0    15625 2023-07-13 19:04:25.615918 rispy-0.8.0/tests/test_parser.py
+-rw-r--r--   0        0        0     5270 2023-07-13 19:04:25.616266 rispy-0.8.0/tests/test_writer.py
+-rw-r--r--   0        0        0    11449 1970-01-01 00:00:00.000000 rispy-0.8.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rispy-0.7.1/rispy/config.py` & `rispy-0.8.0/rispy/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,21 @@
     "A1",
     "A2",
     "A3",
     "A4",
     "AU",
     "KW",
     "N1",
+    "UR",
 ]
 
+DELIMITED_TAG_MAPPING = {
+    "UR": ";",
+}
+
 TAG_KEY_MAPPING = {
     "TY": "type_of_reference",
     "A1": "first_authors",  # ListType
     "A2": "secondary_authors",  # ListType
     "A3": "tertiary_authors",  # ListType
     "A4": "subsidiary_authors",  # ListType
     "AB": "abstract",
@@ -66,15 +71,15 @@
     "ST": "short_title",
     "T1": "primary_title",
     "T2": "secondary_title",
     "T3": "tertiary_title",
     "TA": "translated_author",
     "TI": "title",
     "TT": "translated_title",
-    "UR": "url",
+    "UR": "urls",  # ListType
     "VL": "volume",
     "Y1": "publication_year",
     "Y2": "access_date",
     "ER": "end_of_reference",
     "UK": "unknown_tag",
 }
```

### Comparing `rispy-0.7.1/rispy/parser.py` & `rispy-0.8.0/rispy/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 """RIS Parser."""
 
-from collections import defaultdict
+import re
 from abc import ABC, abstractmethod
+from collections import defaultdict
 from pathlib import Path
-from typing import Dict, List, TextIO, Union, Optional
-import re
-
-from .config import LIST_TYPE_TAGS, TAG_KEY_MAPPING, WOK_TAG_KEY_MAPPING, WOK_LIST_TYPE_TAGS
+from typing import ClassVar, Dict, List, Optional, TextIO, Type, Union
 
+from .config import (
+    DELIMITED_TAG_MAPPING,
+    LIST_TYPE_TAGS,
+    TAG_KEY_MAPPING,
+    WOK_LIST_TYPE_TAGS,
+    WOK_TAG_KEY_MAPPING,
+)
 
 __all__ = ["load", "loads", "BaseParser", "WokParser", "RisParser"]
 
 
 class NextLine(Exception):
     pass
 
 
+class ParseError(Exception):
+    pass
+
+
 class BaseParser(ABC):
     """Base parser class. Create a subclass to use.
 
     When creating a new implementation class, some variables and classes need
     to be overridden. This docstring documents how to override these
     parameters when creating a subclass.
 
@@ -47,33 +56,36 @@
                     it removes UTF-BOM characters.
 
     """
 
     START_TAG: str
     END_TAG: str = "ER"
     PATTERN: str
-    DEFAULT_IGNORE: List[str] = []
+    DEFAULT_IGNORE: ClassVar[List[str]] = []
     DEFAULT_MAPPING: Dict
     DEFAULT_LIST_TAGS: List[str]
+    DEFAULT_DELIMITER_MAPPING: Dict
 
     def __init__(
         self,
         *,
         mapping: Optional[Dict] = None,
         list_tags: Optional[List[str]] = None,
+        delimiter_mapping: Optional[Dict] = None,
         ignore: Optional[List[str]] = None,
         skip_missing_tags: bool = False,
         skip_unknown_tags: bool = False,
         enforce_list_tags: bool = True,
     ):
         """Initialize the parser function.
 
         Args:
             mapping (dict, optional): Map tags to tag names.
             list_tags (list, optional): List of list-type tags.
+            delimiter_mapping (dict, optional): Map of delimiters to tags.
             ignore (list, optional): List of tags to ignore.
             skip_missing_tags (bool, optional): Bool to skip lines that don't have
                                                 valid tags, regardless of whether
                                                 of where they are in a reference.
                                                 This is the inverse of the former
                                                 `strict` parameter. If the goal is
                                                 to skip reference headers, see the
@@ -83,24 +95,27 @@
                                                 `TAG_KEY_MAPPING`. If unknown tags
                                                 are not skipped, they will be added
                                                 to the `unknown_tag` key.
                                                 Defaults to `False`.
             enforce_list_tags (bool, optional): Bool for choosing whether to
                                                 strictly enforce list type tags.
                                                 If this is `False`, tags that
-                                                occur mutliple times in a reference
+                                                occur multiple times in a reference
                                                 will be converted to a list instead
-                                                of being overriden. Values set to
+                                                of being overridden. Values set to
                                                 be list tags will still be read as
                                                 list tags. Defaults to `True`.
 
         """
         self.pattern = re.compile(self.PATTERN)
         self.mapping = mapping if mapping is not None else self.DEFAULT_MAPPING
         self.list_tags = list_tags if list_tags is not None else self.DEFAULT_LIST_TAGS
+        self.delimiter_map = (
+            delimiter_mapping if delimiter_mapping is not None else self.DEFAULT_DELIMITER_MAPPING
+        )
         self.ignore = ignore if ignore is not None else self.DEFAULT_IGNORE
         self.skip_missing_tags = skip_missing_tags
         self.skip_unknown_tags = skip_unknown_tags
         self.enforce_list_tags = enforce_list_tags
 
     def parse(self, text: str) -> List[Dict]:
         """Parse RIS string."""
@@ -138,21 +153,21 @@
 
         if tag == self.END_TAG:
             return self.current
 
         if tag == self.START_TAG:
             # New entry
             if self.in_ref:
-                raise IOError(f"Missing end of record tag in line {line_number}:\n {line}")
+                raise ParseError(f"Missing end of record tag in line {line_number}:\n {line}")
             self._add_tag(tag, line)
             self.in_ref = True
             raise NextLine
 
         if not self.in_ref:
-            raise IOError(f"Invalid start tag in line {line_number}:\n {line}")
+            raise ParseError(f"Invalid start tag in line {line_number}:\n {line}")
 
         if tag in self.mapping:
             self._add_tag(tag, line)
             raise NextLine
         elif not self.skip_unknown_tags:
             self._add_unknown_tag(tag, line)
             raise NextLine
@@ -161,59 +176,72 @@
 
     def _parse_other(self, line, line_number):
         if self.skip_missing_tags:
             raise NextLine
         if self.in_ref:
             # Active reference
             if self.last_tag is None:
-                raise IOError(f"Expected tag in line {line_number}:\n {line}")
+                raise ParseError(f"Expected tag in line {line_number}:\n {line}")
             # Active tag
             self._add_tag(self.last_tag, line, all_line=True)
             raise NextLine
 
         if self.is_header(line):
             raise NextLine
-        raise IOError(f"Expected start tag in line {line_number}:\n {line}")
+        raise ParseError(f"Expected start tag in line {line_number}:\n {line}")
 
     def _add_single_value(self, name, value, is_multi=False):
+        """Process a single line.
+
+        This method is only run on tags where repeated tags are not expected.
+        The output for a tag can be a list when a delimiter is specified,
+        even if it is not a list tag.
+        """
         if not is_multi:
             if self.enforce_list_tags or name not in self.current:
                 ignore_this_if_has_one = value
                 self.current.setdefault(name, ignore_this_if_has_one)
             else:
                 self._add_list_value(name, value)
-            return
-
-        value_must_exist_or_is_bug = self.current[name]
-        self.current[name] = " ".join((value_must_exist_or_is_bug, value))
+        else:
+            value_must_exist_or_is_bug = self.current[name]
+            if isinstance(value, list):
+                self.current[name].extend(value)
+            else:
+                self.current[name] = " ".join((value_must_exist_or_is_bug, value))
 
     def _add_list_value(self, name, value):
+        """Process tags with multiple values."""
+        value_list = value if isinstance(value, list) else [value]
         try:
-            self.current[name].append(value)
+            self.current[name].extend(value_list)
         except KeyError:
-            self.current[name] = [value]
+            self.current[name] = value_list
         except AttributeError:
             if not isinstance(self.current[name], str):
                 raise
             must_exist = self.current[name]
-            self.current[name] = [must_exist] + [value]
+            self.current[name] = [must_exist, *value_list]
 
     def _add_tag(self, tag, line, all_line=False):
         self.last_tag = tag
         name = self.mapping[tag]
         if all_line:
             new_value = line.strip()
         else:
             new_value = self.get_content(line)
 
-        if tag not in self.list_tags:
-            self._add_single_value(name, new_value, is_multi=all_line)
-            return
+        delimiter = self.delimiter_map.get(tag)
+        if delimiter is not None:
+            new_value = [i.strip() for i in new_value.split(delimiter)]
 
-        self._add_list_value(name, new_value)
+        if tag in self.list_tags:
+            self._add_list_value(name, new_value)
+        else:
+            self._add_single_value(name, new_value, is_multi=all_line)
 
     def _add_unknown_tag(self, tag, line):
         name = self.mapping["UK"]
         value = self.get_content(line)
         # check if unknown_tag dict exists
         if name not in self.current:
             self.current[name] = defaultdict(list)
@@ -248,17 +276,18 @@
 
 
 class WokParser(BaseParser):
     """Subclass of Base for reading Wok RIS files."""
 
     START_TAG = "PT"
     PATTERN = r"^[A-Z][A-Z0-9] |^ER\s?|^EF\s?"
-    DEFAULT_IGNORE = ["FN", "VR", "EF"]
+    DEFAULT_IGNORE: ClassVar[List[str]] = ["FN", "VR", "EF"]
     DEFAULT_MAPPING = WOK_TAG_KEY_MAPPING
     DEFAULT_LIST_TAGS = WOK_LIST_TYPE_TAGS
+    DEFAULT_DELIMITER_MAPPING: ClassVar[Dict] = {}
 
     def get_content(self, line):
         return line[2:].strip()
 
     def is_header(self, line):
         return True
 
@@ -266,14 +295,15 @@
 class RisParser(BaseParser):
     """Subclass of Base for reading base RIS files."""
 
     START_TAG = "TY"
     PATTERN = r"^[A-Z][A-Z0-9]  - |^ER  -\s*$"
     DEFAULT_MAPPING = TAG_KEY_MAPPING
     DEFAULT_LIST_TAGS = LIST_TYPE_TAGS
+    DEFAULT_DELIMITER_MAPPING = DELIMITED_TAG_MAPPING
 
     counter_re = re.compile("^[0-9]+.")
 
     def get_content(self, line):
         return line[6:].strip()
 
     def is_header(self, line):
@@ -308,15 +338,15 @@
     Returns:
         list: Returns list of RIS entries.
     """
     text = file.read_text(encoding=encoding) if isinstance(file, Path) else file.read()
     return loads(text, implementation=implementation, **kw)
 
 
-def loads(text: str, *, implementation: Optional[BaseParser] = None, **kw) -> List[Dict]:
+def loads(text: str, *, implementation: Optional[Type[BaseParser]] = None, **kw) -> List[Dict]:
     """Load a RIS file and return a list of entries.
 
     Entries are codified as dictionaries whose keys are the
     different tags. For single line and singly occurring tags,
     the content is codified as a string. In the case of multiline
     or multiple key occurrences, the content is returned as a list
     of strings.
```

### Comparing `rispy-0.7.1/rispy/utils.py` & `rispy-0.8.0/rispy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Miscellaneous functions."""
 
-from typing import Dict, List
 from copy import deepcopy
+from typing import Dict, List
 
 from .config import TYPE_OF_REFERENCE_MAPPING
 
 
 def invert_dictionary(mapping: Dict) -> Dict:
     """Invert the keys and values of a dictionary."""
     remap = {v: k for k, v in mapping.items()}
@@ -37,16 +37,16 @@
 
     """
 
     def convert(ref, d=type_map):
         old_type = ref["type_of_reference"]
         try:
             ref["type_of_reference"] = d[old_type]
-        except KeyError:
+        except KeyError as err:
             if strict and old_type not in d.values():
-                raise KeyError(f'Type "{old_type}" not found.')
+                raise KeyError(f'Type "{old_type}" not found.') from err
         return ref
 
     if not reverse:
         return [convert(r) for r in deepcopy(reference_list)]
     else:
         return [convert(r, invert_dictionary(type_map)) for r in deepcopy(reference_list)]
```

### Comparing `rispy-0.7.1/rispy/writer.py` & `rispy-0.8.0/rispy/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """RIS Writer."""
 
 import warnings
-from typing import Dict, List, TextIO, Optional
 from abc import ABC
+from typing import ClassVar, Dict, List, Optional, TextIO, Type
 
 from .config import LIST_TYPE_TAGS, TAG_KEY_MAPPING
 from .utils import invert_dictionary
 
-
 __all__ = ["dump", "dumps", "BaseWriter", "RisWriter"]
 
 
 class BaseWriter(ABC):
     """Base writer class. Create a subclass to use.
 
     When creating a new implementation class, some variables and classes need
@@ -37,15 +36,15 @@
                     number as a parameter.
 
     """
 
     START_TAG: str
     END_TAG: str = "ER"
     PATTERN: str
-    DEFAULT_IGNORE: List[str] = []
+    DEFAULT_IGNORE: ClassVar[List[str]] = []
     DEFAULT_MAPPING: Dict
     DEFAULT_LIST_TAGS: List[str]
     DEFAULT_REFERENCE_TYPE: str = "JOUR"
     SEPARATOR: Optional[str] = "\n"
 
     def __init__(
         self,
@@ -74,70 +73,74 @@
         self.list_tags = list_tags if list_tags is not None else self.DEFAULT_LIST_TAGS
         self.ignore = ignore if ignore is not None else self.DEFAULT_IGNORE
         self._rev_mapping = invert_dictionary(self.mapping)
         self.skip_unknown_tags = skip_unknown_tags
         self.enforce_list_tags = enforce_list_tags
 
     def _get_reference_type(self, ref):
-
         if "type_of_reference" in ref.keys():
             # TODO add check
             return ref["type_of_reference"]
 
         if self.DEFAULT_REFERENCE_TYPE is not None:
             return self.DEFAULT_REFERENCE_TYPE
         else:
             raise ValueError("Unknown type of reference")
 
     def _format_line(self, tag, value=""):
         """Format a RIS line."""
         return self.PATTERN.format(tag=tag, value=value)
 
     def _format_reference(self, ref, count):
-
         lines = []
 
         header = self.set_header(count)
         if header is not None:
             lines.append(header)
         lines.append(self._format_line(self.START_TAG, self._get_reference_type(ref)))
 
-        tags_to_skip = [self.START_TAG] + self.ignore
+        tags_to_skip = [self.START_TAG, *self.ignore]
         if self.skip_unknown_tags:
             tags_to_skip.append("UK")
 
         for label, value in ref.items():
-
             # not available
             try:
                 tag = self._rev_mapping[label.lower()]
             except KeyError:
-                warnings.warn(UserWarning(f"label `{label}` not exported"))
+                warnings.warn(UserWarning(f"label `{label}` not exported"), stacklevel=2)
                 continue
 
             # ignore
             if tag in tags_to_skip:
                 continue
 
             # list tag
             if tag in self.list_tags or (not self.enforce_list_tags and isinstance(value, list)):
                 for val_i in value:
                     lines.append(self._format_line(tag, val_i))
+
+            # unknown tag(s), which are lists held in a defaultdict
+            elif tag == "UK":
+                for unknown_tag in value.keys():
+                    for val_i in value[unknown_tag]:
+                        lines.append(self._format_line(unknown_tag, val_i))
+
+            # all non-list tags
             else:
                 lines.append(self._format_line(tag, value))
 
         lines.append(self._format_line("ER"))
 
         if self.SEPARATOR is not None:
             lines.append(self.SEPARATOR.replace("\n", "", 1))
 
         return lines
 
     def _format_all_references(self, references):
-
         for i, ref in enumerate(references):
             lines_ref = self._format_reference(ref, count=i + 1)
             for line in lines_ref:
                 yield line
 
     def formats(self, references: List[Dict]) -> str:
         """Format a list of references into an RIS string."""
@@ -154,15 +157,15 @@
 
     START_TAG = "TY"
     PATTERN = "{tag}  - {value}"
     DEFAULT_MAPPING = TAG_KEY_MAPPING
     DEFAULT_LIST_TAGS = LIST_TYPE_TAGS
 
     def set_header(self, count):
-        return "{i}.".format(i=count)
+        return f"{count}."
 
 
 def dump(
     references: List[Dict],
     file: TextIO,
     *,
     implementation: Optional[BaseWriter] = None,
@@ -182,15 +185,17 @@
         implementation (RisImplementation): RIS implementation; base by
                                             default.
     """
     text = dumps(references, implementation=implementation, **kw)
     file.writelines(text)
 
 
-def dumps(references: List[Dict], *, implementation: Optional[BaseWriter] = None, **kw) -> str:
+def dumps(
+    references: List[Dict], *, implementation: Optional[Type[BaseWriter]] = None, **kw
+) -> str:
     """Return an RIS formatted string.
 
     Entries are codified as dictionaries whose keys are the
     different tags. For single line and singly occurring tags,
     the content is codified as a string. In the case of multiline
     or multiple key occurrences, the content is returned as a list
     of strings.
```

### Comparing `rispy-0.7.1/PKG-INFO` & `rispy-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: rispy
-Version: 0.7.1
+Version: 0.8.0
 Summary: A Python reader/writer of RIS reference files
-Home-page: https://github.com/mrtango/rispy
-Author: Maik Derstappen (MrTango)
-Author-email: md@derico.de
-License: MIT
 Keywords: RIS,parser,bibliograph
-Platform: UNKNOWN
+Author-email: Maik Derstappen <md@derico.de>
+Maintainer-email: Andy Shapiro <shapiromatron@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytest ~=7.4.0 ; extra == "dev"
+Requires-Dist: flit ~= 3.9.0 ; extra == "dev"
+Requires-Dist: black ~= 23.7.0 ; extra == "dev"
+Requires-Dist: ruff ~= 0.0.278 ; extra == "dev"
+Requires-Dist: coverage ~= 7.2.7 ; extra == "dev"
+Project-URL: Source, https://github.com/mrtango/rispy
 Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
 
 Python RIS files parser and reader
 ==================================
 
 .. image:: https://badge.fury.io/py/rispy.svg
    :target: https://badge.fury.io/py/rispy
 
-A Python 3.6+ reader/writer of RIS reference files.
+A Python 3.8+ reader/writer of RIS reference files.
 
 Usage
 -----
 
 Parsing:
 
 .. code:: python
@@ -76,15 +77,15 @@
    ...  'id': '43',
    ...  'primary_title': 'Reference 43',
    ...  'abstract': 'Lorem ipsum'
    ...  }]
    >>> filepath = 'export.ris'
    >>> with open(filepath, 'w') as bibliography_file:
    ...     rispy.dump(entries, bibliography_file)
-   
+
 
 Example RIS entry
 -----------------
 
 .. code:: text
 
    1.
@@ -133,15 +134,15 @@
 Complete list of ListType tags
 ******************************
 
 .. code:: python
 
     >>> from rispy import LIST_TYPE_TAGS
     >>> print(LIST_TYPE_TAGS)
-    ['A1', 'A2', 'A3', 'A4', 'AU', 'KW', 'N1']
+    ['A1', 'A2', 'A3', 'A4', 'AU', 'KW', 'N1', 'UR']
 
 
 Complete default mapping
 ************************
 
 .. code:: python
 
@@ -205,15 +206,15 @@
      'T2': 'secondary_title',
      'T3': 'tertiary_title',
      'TA': 'translated_author',
      'TI': 'title',
      'TT': 'translated_title',
      'TY': 'type_of_reference',
      'UK': 'unknown_tag',
-     'UR': 'url',
+     'UR': 'urls',
      'VL': 'volume',
      'Y1': 'publication_year',
      'Y2': 'access_date'}
 
 Override key mapping
 ********************
 
@@ -244,15 +245,15 @@
     'pages_this_is_my_fun',
     'place_published',
     'primary_title',
     'publication_year',
     'publisher',
     'secondary_authors',
     'type_of_reference',
-    'url',
+    'urls',
     'volume']
 
 List tags can be customized in the same way, by passing a list to the ``list_tags`` parameter.
 
 Changing rispy behavior
 ***********************
 
@@ -271,15 +272,15 @@
 Parsing
 ^^^^^^^
 Custom parsers can inherit ``RisParser`` (the default parser) or ``BaseParser``. Various parameters and methods can be overridden when creating a new parser. These are documented in the ``BaseParser`` docstring.
 
 Examples:
 
 .. code:: python
-   
+
    class WokParser(BaseParser):
        """Subclass of Base for reading Wok RIS files."""
 
        START_TAG = "PT"
        IGNORE = ["FN", "VR", "EF"]
        PATTERN = r"^[A-Z][A-Z0-9] |^ER\s?|^EF\s?"
        DEFAULT_MAPPING = WOK_TAG_KEY_MAPPING
@@ -343,21 +344,21 @@
 Common developer commands are in the provided `Makefile`; if you don't have `make` installed, you can view the make commands and run the commands from the command-line manually:
 
 .. code:: bash
 
    # setup environment
    python -m venv venv
    source venv/bin/activate
-   pip install -e .[dev,test]
+   python -m pip install -U pip
+   python -m pip install -e ".[dev]"
 
    # check if code format changes are required
    make lint
-   
+
    # reformat code
    make format
 
    # run tests
-   make test 
+   make test
 
 Github Actions are currently enabled to run `lint` and `test` when submitting a pull-request.
 
-
```

### Comparing `rispy-0.7.1/LICENSE` & `rispy-0.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 rispy authors
+Copyright (c) 2023 rispy authors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rispy-0.7.1/tests/test_parser.py` & `rispy-0.8.0/tests/test_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
-import rispy
 import pytest
 
+import rispy
 
 DATA_DIR = Path(__file__).parent.resolve() / "data"
 
 
 def test_load_example_basic_ris():
     filepath = DATA_DIR / "example_basic.ris"
     expected = {
@@ -17,15 +17,15 @@
         "alternate_title3": "Bell System Technical Journal",
         "start_page": "379",
         "end_page": "423",
         "volume": "27",
     }
 
     # test with file object
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
     assert expected == entries[0]
 
     # test with pathlib object
     p = Path(filepath)
     entries = rispy.load(p)
     assert expected == entries[0]
@@ -41,15 +41,15 @@
         "alternate_title3": "Bell System Technical Journal",
         "start_page": "379",
         "end_page": "423",
         "notes_abstract": "first line, then second line and at the end the last line",
         "notes": ["first line", "* second line", "* last line"],
         "volume": "27",
     }
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
 
     assert expected == entries[0]
 
 
 def test_load_example_full_ris():
     filepath = DATA_DIR / "example_full.ris"
@@ -69,15 +69,15 @@
             "number": "3",
             "start_page": "e0815",
             "place_published": "United States",
             "publisher": "Fun Factory",
             "issn": "1932-6208",
             "note": "1008150341",
             "file_attachments2": "http://example.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
         {
             "type_of_reference": "JOUR",
             "id": "12345",
             "primary_title": "The title of the reference",
             "first_authors": ["Marxus, Karlus", "Lindgren, Astrid"],
             "secondary_authors": ["Glattauer, Daniel"],
@@ -90,19 +90,19 @@
             "number": "3",
             "start_page": "e0815341",
             "place_published": "Germany",
             "publisher": "Dark Factory",
             "issn": "1732-4208",
             "note": "1228150341",
             "file_attachments2": "http://example2.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
     ]
 
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
     assert expected == entries
 
 
 def test_load_example_extraneous_data_ris():
     filepath = DATA_DIR / "example_extraneous_data.ris"
     expected = [
@@ -121,15 +121,15 @@
             "number": "3",
             "start_page": "e0815",
             "place_published": "United States",
             "publisher": "Fun Factory",
             "issn": "1932-6208",
             "note": "1008150341",
             "file_attachments2": "http://example.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
         {
             "type_of_reference": "JOUR",
             "id": "12345",
             "primary_title": "The title of the reference",
             "first_authors": ["Marxus, Karlus", "Lindgren, Astrid"],
             "secondary_authors": ["Glattauer, Daniel"],
@@ -142,25 +142,24 @@
             "number": "3",
             "start_page": "e0815341",
             "place_published": "Germany",
             "publisher": "Dark Factory",
             "issn": "1732-4208",
             "note": "1228150341",
             "file_attachments2": "http://example2.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
     ]
 
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f, skip_missing_tags=True)
     assert expected == entries
 
 
 def test_load_example_full_ris_without_whitespace():
-
     # Parse files without whitespace after ER tag.
     # Resolves https://github.com/MrTango/rispy/pull/25
 
     filepath = DATA_DIR / "example_full_without_whitespace.ris"
     expected = [
         {
             "type_of_reference": "JOUR",
@@ -177,15 +176,15 @@
             "number": "3",
             "start_page": "e0815",
             "place_published": "United States",
             "publisher": "Fun Factory",
             "issn": "1932-6208",
             "note": "1008150341",
             "file_attachments2": "http://example.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
         {
             "type_of_reference": "JOUR",
             "id": "12345",
             "primary_title": "The title of the reference",
             "first_authors": ["Marxus, Karlus", "Lindgren, Astrid"],
             "secondary_authors": ["Glattauer, Daniel"],
@@ -198,19 +197,19 @@
             "number": "3",
             "start_page": "e0815341",
             "place_published": "Germany",
             "publisher": "Dark Factory",
             "issn": "1732-4208",
             "note": "1228150341",
             "file_attachments2": "http://example2.com",
-            "url": "http://example_url.com",
+            "urls": ["http://example_url.com"],
         },
     ]
 
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
     assert expected == entries
 
 
 def test_load_single_unknown_tag_ris():
     filepath = DATA_DIR / "example_single_unknown_tag.ris"
     expected = {
@@ -221,15 +220,15 @@
         "alternate_title3": "Bell System Technical Journal",
         "start_page": "379",
         "end_page": "423",
         "volume": "27",
         "unknown_tag": {"JP": ["CRISPR", "Direct Current"]},
     }
 
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
 
     assert expected == entries[0]
 
 
 def test_load_multiple_unknown_tags_ris():
     filepath = DATA_DIR / "example_multi_unknown_tags.ris"
@@ -239,45 +238,44 @@
         "year": "1948/07//",
         "title": "A Mathematical Theory of Communication",
         "alternate_title3": "Bell System Technical Journal",
         "end_page": "423",
         "volume": "27",
         "unknown_tag": {"JP": ["CRISPR"], "DC": ["Direct Current"]},
     }
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f)
     assert expected == entries[0]
 
 
 def test_starting_newline():
     fn = DATA_DIR / "example_starting_newlines.ris"
-    with open(fn, "r") as f:
+    with open(fn) as f:
         entries = rispy.load(f)
     assert len(entries) == 1
 
 
 def test_strip_bom():
     expected = {
         "type_of_reference": "JOUR",
         "doi": "10.1186/s40981-020-0316-0",
     }
 
     filepath = DATA_DIR / "example_bom.ris"
 
     # we properly decode the content of this file as UTF-8, but leave the BOM
-    with open(filepath, "r", encoding="utf-8") as f:
+    with open(filepath, encoding="utf-8") as f:
         entries = rispy.load(f)
 
-    print(entries)
     assert expected == entries[0]
 
 
 def test_wos_ris():
     fn = DATA_DIR / "example_wos.ris"
-    with open(fn, "r") as f:
+    with open(fn) as f:
         entries = rispy.load(f, implementation=rispy.WokParser)
 
     assert len(entries) == 2
 
     title = "Interactions stabilizing the structure of the core light-harvesting complex (LHl) of photosynthetic bacteria and its subunit (B820)"  # noqa: E501
     assert entries[0]["document_title"] == title
 
@@ -293,15 +291,15 @@
         "year": "1948/07//",
         "title": "A Mathematical Theory of Communication",
         "alternate_title3": "Bell System Technical Journal",
         "end_page": "423",
         "volume": "27",
     }
 
-    with open(filepath, "r") as f:
+    with open(filepath) as f:
         entries = rispy.load(f, skip_unknown_tags=True)
     assert expected == entries[0]
 
 
 def test_type_conversion():
     refs = [
         {"type_of_reference": "JOUR", "id": "12345", "primary_title": "Title of reference"},
@@ -322,15 +320,14 @@
         "Whole book",
         "Journal",
         "TEST",
     ]
 
     # test reverse
     test2 = rispy.utils.convert_reference_types(test1, reverse=True)
-    print(test2)
     assert test2[0:2] == refs[0:2]
     assert test2[3] == refs[3]
     assert test2[2]["type_of_reference"] == "JOUR"
 
     # test strict
     with pytest.raises(KeyError):
         rispy.utils.convert_reference_types(refs, strict=True)
@@ -343,15 +340,15 @@
     assert test4[2]["type_of_reference"] == "JOUR"
 
 
 def test_encodings():
     fn = DATA_DIR / "example_utf_chars.ris"
     p = Path(fn)
 
-    with open(fn, "r", encoding="utf-8") as file:
+    with open(fn, encoding="utf-8") as file:
         expected = rispy.load(file)
 
     with pytest.raises(UnicodeDecodeError):
         rispy.load(p, encoding="cp1252")
 
     entries = rispy.load(p, encoding="utf-8")
 
@@ -365,7 +362,19 @@
         "type_of_reference": "JOUR",
         "authors": ["Marx, Karl", "Marxus, Karlus"],
         "issn": ["12345", "ABCDEFG", "666666"],
     }
 
     entries = rispy.load(filepath, enforce_list_tags=False, list_tags=[])
     assert expected == entries[0]
+
+
+def test_url_tag():
+    filepath = DATA_DIR / "example_urls.ris"
+    with open(filepath) as f:
+        entries = rispy.load(f)
+
+    assert len(entries) == 4
+    assert entries[0]["urls"] == ["http://example.com"]
+    assert entries[1]["urls"] == ["http://example.com", "http://www.example.com"]
+    assert entries[2]["urls"] == ["http://example.com", "http://www.example.com"]
+    assert entries[3]["urls"] == ["http://example.com", "http://www.example.com"]
```

### Comparing `rispy-0.7.1/tests/test_writer.py` & `rispy-0.8.0/tests/test_writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from pathlib import Path
 from copy import deepcopy
+from pathlib import Path
+from typing import ClassVar, List
 
 import pytest
-import rispy
 
+import rispy
 
 DATA_DIR = Path(__file__).parent.resolve() / "data"
 
 
 def test_dump_and_load():
     # check that we can write the same file we read
     source_fp = DATA_DIR / "example_full.ris"
@@ -19,15 +20,14 @@
     entries = rispy.loads(actual)
     export = rispy.dumps(entries)
 
     assert actual == export
 
 
 def test_dumps_multiple_unknown_tags_ris(tmp_path):
-
     fp = tmp_path / "test_dump_unknown_tags.ris"
 
     results = [{"title": "my-title", "abstract": "my-abstract", "does_not_exists": "test"}]
 
     # check that we get a warning
     with pytest.warns(UserWarning, match="label `does_not_exists` not exported"):
         with open(fp, "w") as f:
@@ -105,27 +105,89 @@
     export = rispy.dumps(expected, enforce_list_tags=False, list_tags=[])
     entries = rispy.loads(export, list_tags=["AU", "SN"])
     assert expected == entries
 
 
 def test_file_implementation_write():
     class CustomParser(rispy.RisParser):
-        DEFAULT_IGNORE = ["JF", "ID", "KW"]
+        DEFAULT_IGNORE: ClassVar[List[str]] = ["JF", "ID", "KW"]
 
     class CustomWriter(rispy.RisWriter):
-        DEFAULT_IGNORE = ["JF", "ID", "KW"]
+        DEFAULT_IGNORE: ClassVar[List[str]] = ["JF", "ID", "KW"]
 
     list_tags = ["SN", "T1", "A1", "UR"]
 
     fn = DATA_DIR / "example_full.ris"
-    with open(fn, "r") as f:
+    with open(fn) as f:
         entries = rispy.load(f, implementation=CustomParser, list_tags=list_tags)
 
     fn_write = DATA_DIR / "example_full_write.ris"
 
     with open(fn_write, "w") as f:
         rispy.dump(entries, f, implementation=CustomWriter, list_tags=list_tags)
 
-    with open(fn_write, "r") as f:
+    with open(fn_write) as f:
         reload = rispy.load(f, implementation=CustomParser, list_tags=list_tags)
 
     assert reload == entries
+
+
+def test_write_single_unknown_tag():
+    entries = [
+        {
+            "type_of_reference": "JOUR",
+            "authors": ["Shannon, Claude E."],
+            "year": "1948/07//",
+            "title": "A Mathematical Theory of Communication",
+            "start_page": "379",
+            "unknown_tag": {"JP": ["CRISPR"]},
+        }
+    ]
+
+    text_output = rispy.dumps(entries)
+
+    # check output is as expected
+    lines = text_output.splitlines()
+    assert lines[6] == "JP  - CRISPR"
+    assert len(lines) == 8
+
+
+def test_write_multiple_unknown_tag_same_type():
+    entries = [
+        {
+            "type_of_reference": "JOUR",
+            "authors": ["Shannon, Claude E."],
+            "year": "1948/07//",
+            "title": "A Mathematical Theory of Communication",
+            "start_page": "379",
+            "unknown_tag": {"JP": ["CRISPR", "PEOPLE"]},
+        }
+    ]
+
+    text_output = rispy.dumps(entries)
+
+    # check output is as expected
+    lines = text_output.splitlines()
+    assert lines[6] == "JP  - CRISPR"
+    assert lines[7] == "JP  - PEOPLE"
+    assert len(lines) == 9
+
+
+def test_write_multiple_unknown_tag_diff_type():
+    entries = [
+        {
+            "type_of_reference": "JOUR",
+            "authors": ["Shannon, Claude E."],
+            "year": "1948/07//",
+            "title": "A Mathematical Theory of Communication",
+            "start_page": "379",
+            "unknown_tag": {"JP": ["CRISPR"], "ED": ["Swinburne, Ricardo"]},
+        }
+    ]
+
+    text_output = rispy.dumps(entries)
+
+    # check output is as expected
+    lines = text_output.splitlines()
+    assert lines[6] == "JP  - CRISPR"
+    assert lines[7] == "ED  - Swinburne, Ricardo"
+    assert len(lines) == 9
```

### Comparing `rispy-0.7.1/tests/data/example_full_without_whitespace.ris` & `rispy-0.8.0/tests/data/example_full_without_whitespace.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/tests/data/example_extraneous_data.ris` & `rispy-0.8.0/tests/data/example_extraneous_data.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/tests/data/example_utf_chars.ris` & `rispy-0.8.0/tests/data/example_utf_chars.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/tests/data/example_wos.ris` & `rispy-0.8.0/tests/data/example_wos.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/tests/data/example_full.ris` & `rispy-0.8.0/tests/data/example_full.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/tests/data/example_full_write.ris` & `rispy-0.8.0/tests/data/example_full_write.ris`

 * *Files identical despite different names*

### Comparing `rispy-0.7.1/HISTORY.rst` & `rispy-0.8.0/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 History
 =======
 
+v0.8.0 (2023-07-13)
+-------------------
+
+Breaking changes:
+
+* Update minimum python version from 3.6 to 3.8
+* Improve URL parsing to be more robust and consistent with the spec; saved as a plural "urls" dictionary key instead of the singular "url" (@scott-8/shapiromatron #52)
+* Throw a `rispy.paser.ParseError` instead of a IOError for invalid parsing (@shapiromatron #54)
+
+Additional updates:
+
+* Write RIS unknown tags (@simon-20 #50)
+
+Tooling updates:
+
+* Support and test python 3.8 through 3.11
+* Update black
+* Switch to ruff from flake8 + isort
+* Switch to flit
+* Add basic coverage reports to github actions
+
 v0.7.1 (2021-06-01)
 -------------------
 
-* README.rst formatting fixes 
+* README.rst formatting fixes
 
 v0.7.0 (2021-06-01)
 -------------------
 
 New features:
 
 * Allow for subclassing of readers and writers for custom implementations and greater flexibility; these custom classes can be used in all high-level commands (load/loads/dump/dumps)  (@scott-8 #36)
```

### Comparing `rispy-0.7.1/rispy.egg-info/PKG-INFO` & `rispy-0.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,14 @@
-Metadata-Version: 2.1
-Name: rispy
-Version: 0.7.1
-Summary: A Python reader/writer of RIS reference files
-Home-page: https://github.com/mrtango/rispy
-Author: Maik Derstappen (MrTango)
-Author-email: md@derico.de
-License: MIT
-Keywords: RIS,parser,bibliograph
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 Python RIS files parser and reader
 ==================================
 
 .. image:: https://badge.fury.io/py/rispy.svg
    :target: https://badge.fury.io/py/rispy
 
-A Python 3.6+ reader/writer of RIS reference files.
+A Python 3.8+ reader/writer of RIS reference files.
 
 Usage
 -----
 
 Parsing:
 
 .. code:: python
@@ -76,15 +53,15 @@
    ...  'id': '43',
    ...  'primary_title': 'Reference 43',
    ...  'abstract': 'Lorem ipsum'
    ...  }]
    >>> filepath = 'export.ris'
    >>> with open(filepath, 'w') as bibliography_file:
    ...     rispy.dump(entries, bibliography_file)
-   
+
 
 Example RIS entry
 -----------------
 
 .. code:: text
 
    1.
@@ -133,15 +110,15 @@
 Complete list of ListType tags
 ******************************
 
 .. code:: python
 
     >>> from rispy import LIST_TYPE_TAGS
     >>> print(LIST_TYPE_TAGS)
-    ['A1', 'A2', 'A3', 'A4', 'AU', 'KW', 'N1']
+    ['A1', 'A2', 'A3', 'A4', 'AU', 'KW', 'N1', 'UR']
 
 
 Complete default mapping
 ************************
 
 .. code:: python
 
@@ -205,15 +182,15 @@
      'T2': 'secondary_title',
      'T3': 'tertiary_title',
      'TA': 'translated_author',
      'TI': 'title',
      'TT': 'translated_title',
      'TY': 'type_of_reference',
      'UK': 'unknown_tag',
-     'UR': 'url',
+     'UR': 'urls',
      'VL': 'volume',
      'Y1': 'publication_year',
      'Y2': 'access_date'}
 
 Override key mapping
 ********************
 
@@ -244,15 +221,15 @@
     'pages_this_is_my_fun',
     'place_published',
     'primary_title',
     'publication_year',
     'publisher',
     'secondary_authors',
     'type_of_reference',
-    'url',
+    'urls',
     'volume']
 
 List tags can be customized in the same way, by passing a list to the ``list_tags`` parameter.
 
 Changing rispy behavior
 ***********************
 
@@ -271,15 +248,15 @@
 Parsing
 ^^^^^^^
 Custom parsers can inherit ``RisParser`` (the default parser) or ``BaseParser``. Various parameters and methods can be overridden when creating a new parser. These are documented in the ``BaseParser`` docstring.
 
 Examples:
 
 .. code:: python
-   
+
    class WokParser(BaseParser):
        """Subclass of Base for reading Wok RIS files."""
 
        START_TAG = "PT"
        IGNORE = ["FN", "VR", "EF"]
        PATTERN = r"^[A-Z][A-Z0-9] |^ER\s?|^EF\s?"
        DEFAULT_MAPPING = WOK_TAG_KEY_MAPPING
@@ -343,21 +320,20 @@
 Common developer commands are in the provided `Makefile`; if you don't have `make` installed, you can view the make commands and run the commands from the command-line manually:
 
 .. code:: bash
 
    # setup environment
    python -m venv venv
    source venv/bin/activate
-   pip install -e .[dev,test]
+   python -m pip install -U pip
+   python -m pip install -e ".[dev]"
 
    # check if code format changes are required
    make lint
-   
+
    # reformat code
    make format
 
    # run tests
-   make test 
+   make test
 
 Github Actions are currently enabled to run `lint` and `test` when submitting a pull-request.
-
-
```

