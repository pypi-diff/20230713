# Comparing `tmp/hoppr_cop-1.1.7.tar.gz` & `tmp/hoppr_cop-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.1.7.tar", max compression
+gzip compressed data, was "hoppr_cop-1.1.8.tar", max compression
```

## Comparing `hoppr_cop-1.1.7.tar` & `hoppr_cop-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/LICENSE.md
--rw-r--r--   0        0        0       55 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     3336 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     4488 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0     9223 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1134 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/models.py
--rwxr-xr-x   0        0        0      113 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     5953 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     5289 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/grype/models.py
--rw-r--r--   0        0        0     9731 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0      478 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9487 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    11624 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     3147 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     4924 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0     5591 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0      853 2023-06-01 19:06:34.000000 hoppr_cop-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/LICENSE.md
+-rw-r--r--   0        0        0       55 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     3336 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     4488 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0     9326 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1134 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/models.py
+-rwxr-xr-x   0        0        0      113 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     5953 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     5289 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/grype/models.py
+-rw-r--r--   0        0        0     9337 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0      478 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9487 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    11624 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     3147 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     4923 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0     5590 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0      854 2023-07-13 16:05:12.000000 hoppr_cop-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1083 1970-01-01 00:00:00.000000 hoppr_cop-1.1.8/PKG-INFO
```

### Comparing `hoppr_cop-1.1.7/LICENSE.md` & `hoppr_cop-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/combined/cli.py` & `hoppr_cop-1.1.8/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.1.8/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.1.8/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 from security_commons.common.vulnerability_scanner import VulnerabilitySuper
 from hopprcop.gemnasium.models import GemnasiumVulnerability
 
 
 class GemnasiumScanner(VulnerabilitySuper):
     """A Vulnerability Scanner for Gitlab's Gemnasiumm Database"""
 
-    supported_formats = ["npm", "maven", "pypi", "gem", "golang", "connan"]
+    supported_formats = ["npm", "maven", "pypi", "gem", "golang", "conan"]
+    # TODO: supported_formats is not used; should get_vulnerabilities_by_purl be filtering purls by it?
 
     database_path = None
     # url = "https://gitlab.com/gitlab-org/security-products/gemnasium-db/-/archive/master/gemnasium-db-master.zip"
     url = os.getenv(
         "GEMNASIUM_DATABASE_ZIP",
         "https://gitlab.com/gitlab-org/advisories-community/-/archive/main/advisories-community-main.zip",
     )
```

### Comparing `hoppr_cop-1.1.7/hopprcop/gemnasium/models.py` & `hoppr_cop-1.1.8/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.1.8/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/grype/models.py` & `hoppr_cop-1.1.8/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.1.8/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,25 +21,14 @@
     """
 
     EMBEDDED_VEX = "embedded_cyclone_dx_vex"
     LINKED_VEX = "linked_cyclone_dx_vex"
 
     bom_access = BomAccess.FULL_ACCESS
 
-    supported_purl_types = [
-        "golang",
-        "npm",
-        "maven",
-        "pypi",
-        "nuget",
-        "gem",
-        "rpm",
-        "deb",
-    ]
-
     def get_version(self) -> str:
         """
         __version__ required for all HopprPlugin implementations
         """
         return __version__
 
     @hoppr_process
@@ -61,22 +50,14 @@
         output_dir.mkdir(parents=True, exist_ok=True)
 
         reporting = Reporting(output_dir, base_report_name)
         combined = CombinedScanner()
         combined.set_scanners(scanners)
         parsed_bom = self.context.delivered_sbom
 
-        parsed_bom.components = list(
-            filter(
-                lambda x: PackageURL.from_string(x.purl).type
-                in self.supported_purl_types,
-                parsed_bom.components,
-            )
-        )
-
         results = combined.get_vulnerabilities_by_sbom(parsed_bom)
 
         # Map bom ref to results - uses purl as ref
         bom_ref_to_results = dict[str, self.ComponentVulnerabilityWrapper]()
 
         # Map purls to components, try to normalize purls to lowercase
         purl_to_component = {
```

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.7/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.1.8/hopprcop/ossindex/oss_index_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         "npm",
         "maven",
         "pypi",
         "gem",
         "golang",
         "nuget",
         "rpm",
-        "connan",
+        "conan",
     ]
 
     def get_vulnerabilities_by_purl(
         self, purls: list[PackageURL]
     ) -> dict[str, Optional[list[Vulnerability]]]:
         """Get the vulnerabilities for a list of package URLS (purls)
         This function will return a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found
```

### Comparing `hoppr_cop-1.1.7/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.1.8/hopprcop/trivy/trivy_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     supported_types = [
         "npm",
         "maven",
         "pypi",
         "gem",
         "golang",
         "nuget",
-        "connan",
+        "conan",
         "rpm",
         "deb",
     ]
 
     def get_vulnerabilities_by_purl(
         self, purls: list[PackageURL]
     ) -> dict[str, Optional[list[Vulnerability]]]:
```

### Comparing `hoppr_cop-1.1.7/pyproject.toml` & `hoppr_cop-1.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.1.7"
+version = "1.1.8"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "hopprcop"
 
@@ -22,15 +22,15 @@
 mkdocs-mermaid2-plugin = "^0.6.0"
 hoppr = "^1.8.0"
 pytest = "7.3.1"
 coverage = "^7.0.0"
 hoppr-security-commons = "^0.0.13"
 mkdocs-glightbox = "^0.3.1"
 pygments = "^2.14.0"
-pymdown-extensions = "^9.9.2"
+pymdown-extensions = "^10.0.0"
 
 [tool.poetry.scripts]
 hoppr-cop = "hopprcop.combined.cli:app"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 black = "^23.0.0"
```

### Comparing `hoppr_cop-1.1.7/PKG-INFO` & `hoppr_cop-1.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.1.7
+Version: 1.1.8
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,13 +17,13 @@
 Requires-Dist: hoppr-cyclonedx-models (>=0.4.7)
 Requires-Dist: hoppr-security-commons (>=0.0.13,<0.0.14)
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0)
 Requires-Dist: mkdocs-glightbox (>=0.3.1,<0.4.0)
 Requires-Dist: mkdocs-mermaid2-plugin (>=0.6.0,<0.7.0)
 Requires-Dist: packageurl-python (>=0.10.1,<0.11.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
-Requires-Dist: pymdown-extensions (>=9.9.2,<10.0.0)
+Requires-Dist: pymdown-extensions (>=10.0.0,<11.0.0)
 Requires-Dist: pytest (==7.3.1)
 Requires-Dist: rich (>12.5.1)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

