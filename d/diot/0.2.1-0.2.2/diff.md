# Comparing `tmp/diot-0.2.1.tar.gz` & `tmp/diot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diot-0.2.1.tar", max compression
+gzip compressed data, was "diot-0.2.2.tar", max compression
```

## Comparing `diot-0.2.1.tar` & `diot-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-24 16:39:13.792367 diot-0.2.1/LICENSE
--rw-r--r--   0        0        0     5283 2023-06-24 16:39:13.792367 diot-0.2.1/README.md
--rw-r--r--   0        0        0      195 2023-06-24 16:39:13.792367 diot-0.2.1/diot/__init__.py
--rw-r--r--   0        0        0    28577 2023-06-24 16:39:13.792367 diot-0.2.1/diot/diot.py
--rw-r--r--   0        0        0     3070 2023-06-24 16:39:13.792367 diot-0.2.1/diot/transforms.py
--rw-r--r--   0        0        0     1587 2023-06-24 16:39:13.792367 diot-0.2.1/diot/utils.py
--rw-r--r--   0        0        0     1059 2023-06-24 16:39:13.792367 diot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 diot-0.2.1/setup.py
--rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-13 20:06:11.567139 diot-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5283 2023-07-13 20:06:11.567139 diot-0.2.2/README.md
+-rw-r--r--   0        0        0      195 2023-07-13 20:06:11.567139 diot-0.2.2/diot/__init__.py
+-rw-r--r--   0        0        0    28618 2023-07-13 20:06:11.567139 diot-0.2.2/diot/diot.py
+-rw-r--r--   0        0        0     3070 2023-07-13 20:06:11.567139 diot-0.2.2/diot/transforms.py
+-rw-r--r--   0        0        0     1587 2023-07-13 20:06:11.567139 diot-0.2.2/diot/utils.py
+-rw-r--r--   0        0        0     1058 2023-07-13 20:06:11.571139 diot-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 diot-0.2.2/setup.py
+-rw-r--r--   0        0        0     5995 1970-01-01 00:00:00.000000 diot-0.2.2/PKG-INFO
```

### Comparing `diot-0.2.1/LICENSE` & `diot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diot-0.2.1/README.md` & `diot-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `diot-0.2.1/diot/diot.py` & `diot-0.2.2/diot/diot.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,18 @@
         self.__diot__["transform"] = kwargs.pop("diot_transform", "safe")
         self.__diot__["frozen"] = False
         self.__diot__["missing"] = kwargs.pop("diot_missing", KeyError)
         diot_frozen = kwargs.pop("diot_frozen", False)
         if isinstance(self.__diot__["transform"], str):
             self.__diot__["transform"] = TRANSFORMS[self.__diot__["transform"]]
 
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            *(arg for arg in args if arg is not None),
+            **kwargs,
+        )
 
         for key in self:
             transformed_key = self.__diot__["transform"](key)
             if transformed_key in self.__diot__["keymaps"]:
                 raise KeyError(
                     f"Keys {self.__diot__['keymaps'][transformed_key]!r} and "
                     f"{key!r} will be transformed to the same attribute. "
@@ -215,16 +218,16 @@
         )
 
     def __getattr__(self, name: str) -> Any:
         if name == "__diot__":
             return self.__dict__["__diot__"]
         try:
             return self[name]
-        except Exception as exc:
-            raise AttributeError(name) from exc
+        except Exception:
+            raise AttributeError(name) from None
 
     def __getitem__(self, name: str) -> Any:
         original_key = self.__diot__["keymaps"].get(name, name)
         try:
             return super().__getitem__(original_key)
         except KeyError as keyerr:
             missing_handler = self.__diot__["missing"]
@@ -608,18 +611,18 @@
             **yaml_kwargs: Other kwargs for `yaml.dump`
 
         Returns:
             The yaml string with filename is not given
         """
         try:
             import yaml  # type: ignore[import]
-        except ImportError as exc:  # pragma: no cover
+        except ImportError:  # pragma: no cover
             raise ImportError(
                 "You need pyyaml installed to export Diot as yaml."
-            ) from exc
+            ) from None
         yaml_dump = self.to_dict()
         if not filename:
             return yaml.dump(
                 yaml_dump, default_flow_style=default_flow_style, **yaml_kwargs
             )
         with open(filename, "w", encoding=encoding, errors=errors) as fyml:
             yaml.dump(
@@ -648,18 +651,18 @@
                 See python's open function
 
         Returns:
             The toml string with filename is not given
         """
         try:
             import rtoml  # type: ignore[import]
-        except ImportError as exc:  # pragma: no cover
+        except ImportError:  # pragma: no cover
             raise ImportError(
                 "You need rtoml installed to export Diot as toml."
-            ) from exc
+            ) from None
         toml_dump = self.to_dict()
         if not filename:
             return rtoml.dumps(toml_dump)
         with open(filename, "w", encoding=encoding, errors=errors) as ftml:
             rtoml.dump(toml_dump, ftml)
         return None
 
@@ -791,16 +794,16 @@
 
         Raises:
             KeyError: when existing key does not exist
             KeyError: when name is an existing key
         """
         try:
             position = self.__diot__["orderedkeys"].index(existing_key)
-        except ValueError as vex:
-            raise KeyError("No such key: %s" % existing_key) from vex
+        except ValueError:
+            raise KeyError("No such key: %s" % existing_key) from None
         if name in self.__diot__["orderedkeys"]:
             raise KeyError("Key already exists: %s" % name)
         self.insert(position, name, value)
 
     def insert_after(
         self, existing_key: str, name: str, value: Any = None
     ) -> None:
@@ -814,16 +817,16 @@
 
         Raises:
             KeyError: when existing key does not exist
             KeyError: when name is an existing key
         """
         try:
             position = self.__diot__["orderedkeys"].index(existing_key)
-        except ValueError as vex:
-            raise KeyError("No such key: %s" % existing_key) from vex
+        except ValueError:
+            raise KeyError("No such key: %s" % existing_key) from None
         if name in self.__diot__["orderedkeys"]:
             raise KeyError("Key already exists: %s" % name)
         self.insert(position + 1, name, value)
 
     def keys(self) -> Iterable:  # type: ignore[override]
         """Get the keys in the order they are added
```

### Comparing `diot-0.2.1/diot/transforms.py` & `diot-0.2.2/diot/transforms.py`

 * *Files identical despite different names*

### Comparing `diot-0.2.1/diot/utils.py` & `diot-0.2.2/diot/utils.py`

 * *Files identical despite different names*

### Comparing `diot-0.2.1/pyproject.toml` & `diot-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "poetry>=0.12",]
+requires = [ "poetry>=1.0",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "diot"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python dictionary with dot notation."
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/diot"
 repository = "https://github.com/pwwang/diot"
```

### Comparing `diot-0.2.1/setup.py` & `diot-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['inflection>=0.5,<0.6']
 
 setup_kwargs = {
     'name': 'diot',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python dictionary with dot notation.',
     'long_description': '![Logo](https://raw.githubusercontent.com/pwwang/diot/master/logo.png)\n\n[![pypi][1]][2] [![tag][3]][4] [![codacy quality][7]][8] [![coverage][9]][8] ![pyver][10] ![building][6] ![docs][5]\n\nPython dictionary with dot notation (A re-implementation of [python-box](https://github.com/cdgriffith/Box) with some issues fixed and simplified)\n\n```python\nfrom diot import Diot\n\nmovie_data = {\n  "movies": {\n    "Spaceballs": {\n      "imdb stars": 7.1,\n      "rating": "PG",\n      "length": 96,\n      "director": "Mel Brooks",\n      "stars": [{"name": "Mel Brooks", "imdb": "nm0000316", "role": "President Skroob"},\n                {"name": "John Candy","imdb": "nm0001006", "role": "Barf"},\n                {"name": "Rick Moranis", "imdb": "nm0001548", "role": "Dark Helmet"}\n      ]\n    },\n    "Robin Hood: Men in Tights": {\n      "imdb stars": 6.7,\n      "rating": "PG-13",\n      "length": 104,\n      "director": "Mel Brooks",\n      "stars": [\n                {"name": "Cary Elwes", "imdb": "nm0000144", "role": "Robin Hood"},\n                {"name": "Richard Lewis", "imdb": "nm0507659", "role": "Prince John"},\n                {"name": "Roger Rees", "imdb": "nm0715953", "role": "Sheriff of Rottingham"},\n                {"name": "Amy Yasbeck", "imdb": "nm0001865", "role": "Marian"}\n      ]\n    }\n  }\n}\n\n# Box is a conversion_box by default, pass in `conversion_box=False` to disable that behavior\n# Explicitly tell Diot to convert dict/list inside\nmovie_diot = Diot(movie_data)\n\nmovie_diot.movies.Robin_Hood_Men_in_Tights.imdb_stars\n# 6.7\n\nmovie_diot.movies.Spaceballs.stars[0].name\n# \'Mel Brooks\'\n\n# Different as box, you have to use Diot for new data in a list\nmovie_diot.movies.Spaceballs.stars.append(\n\tDiot({"name": "Bill Pullman", "imdb": "nm0000597", "role": "Lone Starr"}))\nmovie_diot.movies.Spaceballs.stars[-1].role\n# \'Lone Starr\'\n```\n\n## Install\n```shell\npip install -U diot\n```\n\n## API\n\nhttps://pwwang.github.io/diot/api/diot/\n\n\n## Usage\n\n### Diot\n\nInstantiated the same ways as `dict`\n```python\nDiot({\'data\': 2, \'count\': 5})\nDiot(data=2, count=5)\nDiot({\'data\': 2, \'count\': 1}, count=5)\nDiot([(\'data\', 2), (\'count\', 5)])\n\n# All will create\n# Diot([(\'data\', 2), (\'count\', 5)], diot_nest = True, diot_transform = \'safe\')\n```\n\nSame as `python-box`, `Diot` is a subclass of dict which overrides some base functionality to make sure everything stored in the dict can be accessed as an attribute or key value.\n\n```python\ndiot = Diot({\'data\': 2, \'count\': 5})\ndiot.data == diot[\'data\'] == getattr(diot, \'data\')\n```\n\nBy default, diot uses a safe transformation to transform keys into safe names that can be accessed by `diot.xxx`\n```python\ndt = Diot({"321 Is a terrible Key!": "yes, really"})\ndt._321_Is_a_terrible_Key_\n# \'yes, really\'\n```\n\nDifferent as `python-box`, duplicate attributes are not allowed.\n```python\ndt = Diot({"!bad!key!": "yes, really", ".bad.key.": "no doubt"})\n# KeyError\n```\n\nUse different transform functions:\n\n```python\ndt = Diot(oneTwo = 12, diot_transform = \'snake_case\')\n# or use alias:\n# dt = SnakeDiot(oneTwo = 12)\ndt.one_two == dt[\'one_two\'] == dt[\'oneTwo\'] == 12\n\ndt = Diot(one_two = 12, diot_transform = \'camel_case\')\n# or use alias:\n# dt = CamelDiot(one_two = 12)\ndt.oneTwo == dt[\'one_two\'] == dt[\'oneTwo\'] == 12\n\ndt = Diot(one_two = 12, diot_transform = \'upper\')\ndt.ONE_TWO == dt[\'one_two\'] == dt[\'ONETWO\'] == 12\n\ndt = Diot(ONE_TWO = 12, diot_transform = \'lower\')\ndt.one_two == dt[\'ONE_TWO\'] == dt[\'one_two\'] == 12\n```\n\nUse your own transform function:\n\n```python\nimport inflection\n\ndt = Diot(post = 10, diot_transform = inflection.pluralize)\ndt.posts == dt[\'posts\'] == dt[\'post\'] == 10\n```\n\n### OrderedDiot\n```python\ndiot_of_order = OrderedDiot()\ndiot_of_order.c = 1\ndiot_of_order.a = 2\ndiot_of_order.d = 3\n\nlist(diot_of_order.keys()) == [\'c\', \'a\', \'d\']\n\n# insertion allowed for OrderedDiot\nod = OrderedDiot()\nod.insert(0, "c", "d")\nod.insert(None, "x", "y")\nod.insert_before(\'c\', "e", "f")\nod.insert_after("a", ("g", "h"))\n\nod2 = OrderedDiot()\nod2.a1 = \'b1\'\nod2.c1 = \'d1\'\nod.insert(-1, od2)\n\nod3 = OrderedDiot()\nod3.a2 = \'b2\'\nod3.c2 = \'d2\'\nod.insert_before(\'c\', od3)\n```\n\n### FrozenDiot\n\n```python\nfd = FrozenDiot(a=1, b=3)\nfd.c = 3 # DiotFrozenError\nwith fd.thaw():\n    fd.c = 3\nfd.c == 3\n```\n\n### Missing key handler\n\n```python\nd = Diot(a=1, b=2, diot_missing=ValueError)\nd[\'c\'] # ValueError\nd.c # AttributeError from ValueError\n\nd = Diot(a=1, b=2, diot_missing=ValueError("Custom message"))\n\nd = Diot(a=1, b=2, diot_missing=None)\n# d.c is None\n\nd = Diot(a=1, b=2, diot_missing=lambda key, diot: diot.a + diot.b)\n# d.c == 3\n```\n\n[1]: https://img.shields.io/pypi/v/diot?style=flat-square\n[2]: https://pypi.org/project/diot/\n[3]: https://img.shields.io/github/tag/pwwang/diot?style=flat-square\n[4]: https://github.com/pwwang/diot\n[5]: https://img.shields.io/github/actions/workflow/status/pwwang/diot/docs.yml?label=docs&style=flat-square\n[6]: https://img.shields.io/github/actions/workflow/status/pwwang/diot/build.yml?style=flat-square\n[7]: https://img.shields.io/codacy/grade/738e49b9cc1745c4ae6a7bb3b198cc3d?style=flat-square\n[8]: https://app.codacy.com/gh/pwwang/diot/dashboard\n[9]: https://img.shields.io/codacy/coverage/738e49b9cc1745c4ae6a7bb3b198cc3d?style=flat-square\n[10]: https://img.shields.io/pypi/pyversions/diot?style=flat-square\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/diot',
```

### Comparing `diot-0.2.1/PKG-INFO` & `diot-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diot
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python dictionary with dot notation.
 Home-page: https://github.com/pwwang/diot
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

