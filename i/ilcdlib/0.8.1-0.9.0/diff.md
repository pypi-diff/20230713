# Comparing `tmp/ilcdlib-0.8.1.tar.gz` & `tmp/ilcdlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.8.1.tar", max compression
+gzip compressed data, was "ilcdlib-0.9.0.tar", max compression
```

## Comparing `ilcdlib-0.8.1.tar` & `ilcdlib-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    11357 2023-06-21 15:54:54.299496 ilcdlib-0.8.1/LICENSE
--rw-r--r--   0        0        0     4949 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/README.md
--rw-r--r--   0        0        0     3489 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17413 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1773 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4431 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6375 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     2665 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     3638 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2023-06-21 15:54:54.303496 ilcdlib-0.8.1/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     2749 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3774 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2596 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2051 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    31853 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2050 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0     9638 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     1206 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3329 2023-06-21 15:54:54.307497 ilcdlib-0.8.1/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-06-21 15:54:54.311497 ilcdlib-0.8.1/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 ilcdlib-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/README.md
+-rw-r--r--   0        0        0     3489 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17413 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1796 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-07-12 11:22:43.103499 ilcdlib-0.9.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4431 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6375 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     2665 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3638 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2749 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     3304 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2051 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    32071 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2050 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-07-12 11:22:43.107499 ilcdlib-0.9.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    10655 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     1206 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-07-12 11:22:43.111499 ilcdlib-0.9.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 ilcdlib-0.9.0/PKG-INFO
```

### Comparing `ilcdlib-0.8.1/LICENSE` & `ilcdlib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/README.md` & `ilcdlib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/pyproject.toml` & `ilcdlib-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.8.1"
+version = "0.9.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -60,15 +60,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.8.1"
+version = "0.9.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/__main__.py` & `ilcdlib-0.9.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/__version__.py` & `ilcdlib-0.9.0/src/ilcdlib/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.8.1"
+VERSION = "0.9.0"
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/cli.py` & `ilcdlib-0.9.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/common.py` & `ilcdlib-0.9.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/const.py` & `ilcdlib-0.9.0/src/ilcdlib/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
 ILCD_IDENTIFICATION: tuple[str] = ("ILCD_EPD",)
 PDF_ATTACHMENT = "PDF"
+URL_ATTACHMENT = "URL"
 
 
 class IlcdContactClass(StrEnum):
     """Enumeration of ILCD contact classes."""
 
     Person = "Persons"
     Company = "Organisations"
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.9.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/dto.py` & `ilcdlib-0.9.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/category.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/compliance.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/contact.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/exchage.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/flow.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/material.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/source.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/unit.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/entity/validation.py` & `ilcdlib-0.9.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/cli.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,21 +16,43 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 
 from ilcdlib.epd.reader import IlcdEpdReader
+from ilcdlib.type import LangDef
 
 
 class EnvirondecIlcdXmlEpdReader(IlcdEpdReader):
     """Reader for EPDs in the Environdec specific ILCD XML format."""
 
     _TIME_REPR_DESC_DELIMITER = "\r\n"
 
+    def get_url_attachment(self, lang: LangDef) -> str | None:
+        """Return URL attachment if exists."""
+        element = self._get_external_tree(
+            self.epd_el_tree,
+            (
+                "process:modellingAndValidation",
+                "process:dataSourcesTreatmentAndRepresentativeness",
+                "process:referenceToDataSource",
+            ),
+        )
+
+        return (
+            self._get_localized_text(
+                element,
+                ("source:sourceInformation", "source:dataSetInformation", "source:sourceDescriptionOrComment"),
+                lang,
+            )
+            if element
+            else None
+        )
+
     def get_validity_ends_date(self) -> datetime.date | None:
         """Return the date the EPD is valid until."""
         descr = self.__get_time_repr_description()
         if descr and self._TIME_REPR_DESC_DELIMITER in descr:
             try:
                 date_str = descr.split(self._TIME_REPR_DESC_DELIMITER)[1].strip().rsplit(" ", 1)[-1].strip()
                 return datetime.date.fromisoformat(date_str)
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/factory.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/epd/reader.py` & `ilcdlib-0.9.0/src/ilcdlib/epd/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,18 @@
             self._get_text(
                 self.epd_el_tree,
                 ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "process:typeOfDataSet"),
             )
             == "EPD"
         )
 
+    def get_url_attachment(self, lang: LangDef) -> str | None:
+        """Return URL attachment if exists."""
+        return None
+
     def get_dataset_type(self) -> str | None:
         """Return the ILCD dataset type. e.g. 'average dataset', 'industry dataset', 'generic dataset', etc."""
         return self._get_text(
             self.epd_el_tree,
             ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "common:other", "epd2013:subType"),
         )
 
@@ -716,14 +720,15 @@
             compliance=compliance,
         )
         if own_ref:
             epd.set_alt_id(provider_domain, own_ref.entity_id)
 
         pdf_url = self.data_provider.get_pdf_url()
         epd.set_attachment_if_any(const.PDF_ATTACHMENT, pdf_url)
+        epd.set_attachment_if_any(const.URL_ATTACHMENT, self.get_url_attachment(lang))
 
         ilcd_ext = IlcdEpdExtension(
             dataset_type=self.get_dataset_type(),
             dataset_version=self.get_version(),
             dataset_uuid=self.get_uuid(),
             production_location=self.get_production_location(),
             epd_verifiers=ilcd_validations,
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/extension.py` & `ilcdlib-0.9.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/http_common.py` & `ilcdlib-0.9.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/common.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/compliance.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/flows.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/indicators.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/properties.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/mapping/units.py` & `ilcdlib-0.9.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/medium/archive.py` & `ilcdlib-0.9.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.9.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/reference_data.py` & `ilcdlib-0.9.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.9.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.9.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/sanitizing/text.py` & `ilcdlib-0.9.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-0.9.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-0.9.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,35 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from hashlib import sha1
 from io import BytesIO
 from typing import IO, Iterable, Type
 from urllib.parse import urlencode
 
-from requests import HTTPError
+from requests import HTTPError, Response
 
 from ilcdlib.dto import Category, IlcdReference, ListResponseMeta, ProcessBasicInfo, ProcessSearchResponse
 from ilcdlib.entity.category import CategorySystemReader
 from ilcdlib.http_common import BaseApiClient
+from ilcdlib.xml_parser import T_ET
 
 
 class Soda4LcaXmlApiClient(BaseApiClient):
     """
     API client for Soda4LCA.
 
     Documentation for the API is available at https://bitbucket.org/okusche/soda4lca/src/7.x-branch/Doc/src/Service_API/Service_API.md.
     """
 
+    ns = {
+        "p": "http://www.ilcd-network.org/ILCD/ServiceAPI/Process",
+        "sapi": "http://www.ilcd-network.org/ILCD/ServiceAPI",
+        "epd": "http://www.iai.kit.edu/EPD/2013",
+    }
+
     def __init__(
         self, base_url: str, *, category_reader_cls: Type[CategorySystemReader] = CategorySystemReader, **kwargs
     ) -> None:
         """
         Create a new API client.
 
         :param base_url: Base API endpoint should be something like https://your-host.tld/resource
@@ -145,43 +152,58 @@
         :param offset: offset from the beginning of the dataset
         :param page_size: size of the page
         :param lang: language code (2 letters)
         :param other_params: refer to Soda4LCA documentation for other parameters
         :return:
         """
         params = dict(
-            format="json",
+            format="xml",
             startIndex=offset,
             pageSize=page_size,
             search="true",
             **other_params,
         )
         if lang is not None:
             params["lang"] = lang
             params["langFallback"] = True
         response = self._do_request("get", "/processes", params=params)
-        obj = response.json()
+
+        return self.__search_processes_xml(response)
+
+    def __get_element_text(self, elem: T_ET.Element, path: str) -> str | None:
+        child = elem.find(path, namespaces=self.ns)
+
+        if child is not None:
+            return child.text
+        return None
+
+    def __search_processes_xml(self, response: Response) -> ProcessSearchResponse:
+        obj = response.text
+
+        tree = T_ET.fromstring(obj)
+
+        processes = tree.findall("p:process", namespaces=self.ns)
+
         meta = ListResponseMeta(
-            offset=obj.get("startIndex", 0),
-            page_size=obj.get("pageSize", 0),
-            total_items_count=obj.get("totalCount", 0),
+            offset=tree.attrib.get(f"{{{self.ns['sapi']}}}startIndex", 0),
+            page_size=tree.attrib.get(f"{{{self.ns['sapi']}}}pageSize", 0),
+            total_items_count=tree.attrib.get(f"{{{self.ns['sapi']}}}totalSize", 0),
         )
         items = []
-        for x in obj.get("data", []):
+        for process in processes:
             items.append(
                 ProcessBasicInfo(
-                    uuid=x.get("uuid"),
-                    name=x.get("name"),
-                    version=x.get("version"),
-                    class_id=x.get("classificId"),
-                    class_name=x.get("classific"),
-                    classification_system=x.get("classificSystem"),
-                    type=x.get("type"),
-                    sub_type=x.get("subType"),
-                    original=x,
+                    uuid=self.__get_element_text(process, "sapi:uuid"),
+                    name=self.__get_element_text(process, "sapi:name"),
+                    version=self.__get_element_text(process, "sapi:dataSetVersion"),
+                    class_id=self.__get_element_text(process, "sapi:classId"),
+                    class_name=self.__get_element_text(process, "sapi:classific"),
+                    classification_system=self.__get_element_text(process, "sapi:classificSystem"),
+                    type=self.__get_element_text(process, "p:type"),
+                    sub_type=self.__get_element_text(process, "sapi:other/epd:subType"),
                 )
             )
         return ProcessSearchResponse(meta=meta, items=items)
 
     def get_processes_iter(
         self, offset: int = 0, page_size: int = 100, **search_params
     ) -> tuple[Iterable[ProcessBasicInfo], int]:
```

### Comparing `ilcdlib-0.8.1/src/ilcdlib/type.py` & `ilcdlib-0.9.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/utils.py` & `ilcdlib-0.9.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/src/ilcdlib/xml_parser.py` & `ilcdlib-0.9.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.8.1/PKG-INFO` & `ilcdlib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.8.1 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.9.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

