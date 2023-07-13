# Comparing `tmp/reasoner_validator-3.7.2.tar.gz` & `tmp/reasoner_validator-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.2.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.3.tar", max compression
```

## Comparing `reasoner_validator-3.7.2.tar` & `reasoner_validator-3.7.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1153 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/LICENSE
--rw-r--r--   0        0        0    12703 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/README.md
--rw-r--r--   0        0        0      131 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/conf.py
--rw-r--r--   0        0        0    19869 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36258 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2177 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/pyproject.toml
--rw-r--r--   0        0        0    38452 2023-07-13 04:51:55.952885 reasoner_validator-3.7.2/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    75092 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39514 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/message.py
--rw-r--r--   0        0        0    29568 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11643 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    12532 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      774 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/conftest.py
--rw-r--r--   0        0        0   117951 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    40085 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2023-07-13 04:51:55.956885 reasoner_validator-3.7.2/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26808 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_validate.py
--rw-r--r--   0        0        0    21570 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-13 04:51:55.960885 reasoner_validator-3.7.2/tests/test_workflows.py
--rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/LICENSE
+-rw-r--r--   0        0        0    12703 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/README.md
+-rw-r--r--   0        0        0      131 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/conf.py
+-rw-r--r--   0        0        0    19869 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36258 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2177 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/pyproject.toml
+-rw-r--r--   0        0        0    38452 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    76464 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39514 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/message.py
+-rw-r--r--   0        0        0    29568 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11622 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    12532 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      774 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/conftest.py
+-rw-r--r--   0        0        0   117433 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40085 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26808 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_validate.py
+-rw-r--r--   0        0        0    21570 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_workflows.py
+-rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.3/PKG-INFO
```

### Comparing `reasoner_validator-3.7.2/LICENSE` & `reasoner_validator-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/README.md` & `reasoner_validator-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/docs/Makefile` & `reasoner_validator-3.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/docs/conf.py` & `reasoner_validator-3.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/docs/index.rst` & `reasoner_validator-3.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/docs/make.bat` & `reasoner_validator-3.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.3/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/pyproject.toml` & `reasoner_validator-3.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.2"
+version = "3.7.3"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.7.2/reasoner_validator/__init__.py` & `reasoner_validator-3.7.3/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.3/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,14 +479,20 @@
             self.report(
                 code="warning.knowledge_graph.edge.provenance.multiple_primary",
                 source_trail=source_trail,
                 identifier=edge_id,
                 sources=",".join(found_primary_knowledge_source)
             )
 
+    # TODO: 13-July-2023: Certain attribute_type_id's are slated for future implementation in the Biolink Model
+    #                     but not in the current model release; however, some teams have started to use the terms.
+    #                     We therefore put them on a special "inclusion list" (like the CATEGORY_INCLUSIONS below)
+    #                     to permit them to pass through the validation without any complaints.
+    ATTRIBUTE_TYPE_ID_INCLUSIONS = ["biolink:knowledge_level", "biolink:agent_type"]
+
     def validate_attributes(
             self,
             edge_id: str,
             edge: Dict,
             source_trail: Optional[str] = None
     ) -> Optional[str]:
         """
@@ -600,81 +606,89 @@
                             edge_id=edge_id,
                             source_trail=source_trail
                         )
                     elif self.validate_biolink():
                         # 'attribute_type_id' is a CURIE, but how well does it map?
                         prefix = attribute_type_id.split(":", 1)[0]
                         if prefix == 'biolink':
-                            biolink_class = self.validate_element_status(
-                                context="knowledge_graph.edge.attribute.type_id",
-                                identifier=attribute_type_id,
-                                edge_id=edge_id,
-                                source_trail=source_trail
-                            )
-                            if biolink_class:
-                                if not self.bmt.is_association_slot(attribute_type_id):
-                                    self.report(
-                                        code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
-                                        identifier=attribute_type_id,
-                                        edge_id=edge_id,
-                                        source_trail=source_trail
-                                    )
-
-                                else:
-                                    # it is a Biolink 'association_slot' but now, validate what kind?
-
-                                    # TODO: only check knowledge_source provenance here for now.
-                                    #       Are there other association_slots to be validated here too?
-
-                                    # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
-                                    if not self.minimum_required_trapi_version("1.4.0-beta"):
-
-                                        if attribute_type_id not in \
-                                                [
-                                                    "biolink:aggregator_knowledge_source",
-                                                    "biolink:primary_knowledge_source",
-
-                                                    # Note: deprecated since Biolink release 3.0.2
-                                                    #       but this is probably caught above in the
-                                                    #       'validate_element_status' method predicate
-                                                    "biolink:original_knowledge_source"
-
-                                                ]:
-
-                                            # TODO: not interested here in any other
-                                            #       attribute_type_id's at this moment
-                                            continue
-
-                                        # ... now, check the infores values against various expectations
-                                        for infores in value:
-                                            if not infores.startswith("infores:"):
-                                                self.report(
-                                                    code="error.knowledge_graph.edge.provenance.infores.missing",
-                                                    identifier=str(infores),
-                                                    edge_id=edge_id,
-                                                    source_trail=source_trail
-                                                )
-                                            else:
-                                                if attribute_type_id == "biolink:primary_knowledge_source":
-                                                    found_primary_knowledge_source.append(infores)
-
-                                                if ara_source and \
-                                                        attribute_type_id == "biolink:aggregator_knowledge_source" and \
-                                                        infores == ara_source:
-                                                    found_ara_knowledge_source = True
-                                                elif kp_source and \
-                                                        attribute_type_id == kp_source_type and \
-                                                        infores == kp_source:
-                                                    found_kp_knowledge_source = True
+                            # We will skip further validation of terms in the ATTRIBUTE_TYPE_ID_INCLUSIONS list...
+                            if attribute_type_id not in self.ATTRIBUTE_TYPE_ID_INCLUSIONS:
 
-                        # if not a Biolink 'association_slot', at least, check if the 'attribute_type_id' has a
-                        # namespace (prefix) known to Biolink. We won't call it a hard error, but issue a warning
+                                # ... but further validate everything else...
+                                biolink_class = self.validate_element_status(
+                                    context="knowledge_graph.edge.attribute.type_id",
+                                    identifier=attribute_type_id,
+                                    edge_id=edge_id,
+                                    source_trail=source_trail
+                                )
+                                if biolink_class:
+                                    if not self.bmt.is_association_slot(attribute_type_id):
+                                        self.report(
+                                            code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
+                                            identifier=attribute_type_id,
+                                            edge_id=edge_id,
+                                            source_trail=source_trail
+                                        )
+                                    else:
+                                        # attribute_type_id is a Biolink 'association_slot': validate it further...
+
+                                        # TODO: only check knowledge_source provenance here for now.
+                                        #       Are there other association_slots to be validated here too?
+                                        #       For example, once new terms with defined value ranges are published
+                                        #       in the Biolink Model, then perhaps 'value' validation will be feasible.
+
+                                        # Edge provenance tags only recorded in
+                                        # Edge attributes prior to TRAPI 1.4.0-beta
+                                        if not self.minimum_required_trapi_version("1.4.0-beta"):
+
+                                            if attribute_type_id not in \
+                                                    [
+                                                        "biolink:aggregator_knowledge_source",
+                                                        "biolink:primary_knowledge_source",
+
+                                                        # Note: deprecated since Biolink release 3.0.2
+                                                        #       but this is probably caught above in the
+                                                        #       'validate_element_status' method predicate
+                                                        "biolink:original_knowledge_source"
+
+                                                    ]:
+
+                                                # TODO: not interested here in any other
+                                                #       attribute_type_id's at this moment
+                                                continue
+
+                                            # ... now, check the infores values against various expectations
+                                            for infores in value:
+                                                if not infores.startswith("infores:"):
+                                                    self.report(
+                                                        code="error.knowledge_graph.edge.provenance.infores.missing",
+                                                        identifier=str(infores),
+                                                        edge_id=edge_id,
+                                                        source_trail=source_trail
+                                                    )
+                                                else:
+                                                    if attribute_type_id == "biolink:primary_knowledge_source":
+                                                        found_primary_knowledge_source.append(infores)
+
+                                                    if ara_source and \
+                                                       attribute_type_id == "biolink:aggregator_knowledge_source" and \
+                                                       infores == ara_source:
+                                                        found_ara_knowledge_source = True
+                                                    elif kp_source and \
+                                                            attribute_type_id == kp_source_type and \
+                                                            infores == kp_source:
+                                                        found_kp_knowledge_source = True
+
+                        # if not a Biolink model defined attribute term, at least, check if
+                        # the 'attribute_type_id' has a namespace (prefix) known to Biolink.
+                        # We won't call it a hard error, but issue a warning
                         elif not self.bmt.get_element_by_prefix(attribute_type_id):
                             self.report(
-                                code="warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
+                                code="warning.knowledge_graph.edge." +
+                                     "attribute.type_id.non_biolink_prefix",
                                 identifier=attribute_type_id,
                                 edge_id=edge_id,
                                 source_trail=source_trail
                             )
 
             # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
             if not self.minimum_required_trapi_version("1.4.0-beta") and self.validate_biolink():
```

### Comparing `reasoner_validator-3.7.2/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.3/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/message.py` & `reasoner_validator-3.7.3/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/report.py` & `reasoner_validator-3.7.3/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.3/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.3/reasoner_validator/trapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
 
 # patch version to fix '#components/schemas/AuxiliaryGraph' bug
 TRAPI_1_4_2_SEMVER = SemVer.from_string("v1.4.2")
 TRAPI_1_4_2: str = str(TRAPI_1_4_2_SEMVER)
 
 LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_2_SEMVER
-LATEST_TRAPI_RELEASE: str = str(LATEST_TRAPI_RELEASE_SEMVER)
+LATEST_TRAPI_RELEASE: str = TRAPI_1_4_2
 
 LATEST_TRAPI_MAJOR_RELEASE_SEMVER: SemVer = SemVer.from_string("v1.4", core_fields=['major', 'minor'])
 LATEST_TRAPI_MAJOR_RELEASE: str = str(LATEST_TRAPI_MAJOR_RELEASE_SEMVER)
 
 # For testing, set TRAPI API query POST timeouts to 10 minutes == 600 seconds
 DEFAULT_TRAPI_POST_TIMEOUT = 600.0
```

### Comparing `reasoner_validator-3.7.2/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.3/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.3/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/reasoner_validator/versioning.py` & `reasoner_validator-3.7.3/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/__init__.py` & `reasoner_validator-3.7.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.3/tests/test_biolink_compliance_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pprint import PrettyPrinter
 import logging
 import pytest
 from bmt import Toolkit
 from linkml_runtime.linkml_model import SlotDefinition
 
 from reasoner_validator import TRAPISchemaValidator
-from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_0_BETA
+from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_0_BETA, LATEST_TRAPI_RELEASE
 from reasoner_validator.biolink import (
     TRAPIGraphType,
     BiolinkValidator,
     get_biolink_model_toolkit,
     check_biolink_model_compliance_of_input_edge,
     check_biolink_model_compliance_of_query_graph,
     check_biolink_model_compliance_of_knowledge_graph
@@ -951,118 +951,103 @@
 #         biolink_version=LATEST_BIOLINK_MODEL
 #     )
 #     validator.validate_attribute_constraints(edge_id="test_validate_attributes unit test", edge=query[0])
 #     check_messages(validator, query[1])
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edge_data,validation_code",
     [
         # (
         #         "mock_edge",  # mock data has dumb edges: don't worry about the S-P-O, just the attributes
         #         "mock_context",
         #         "AssertError_message"
         # ),   # set 3rd argument to AssertError message if test edge should 'fail'; otherwise, empty string (for pass)
         (
             # Query 0. 'attributes' key missing in edge record is None
             {},
-            get_ara_test_case(),
             # "Edge has no 'attributes' key!"
             "error.knowledge_graph.edge.attribute.missing"
         ),
         (
             # Query 1. Empty attributes
             {
                 "attributes": None
             },
-            get_ara_test_case(),
             # "Edge has empty attributes!"
             "error.knowledge_graph.edge.attribute.empty"
         ),
         (
             # Query 2. Empty attributes
             {
                 "attributes": []
             },
-            get_ara_test_case(),
             # "Edge has empty attributes!"
             "error.knowledge_graph.edge.attribute.empty"
-        ),
+        )
     ]
 )
-def test_pre_trapi_1_4_0_validate_missing_or_empty_attributes(query: Tuple):
-    validator = BiolinkValidator(
-        graph_type=TRAPIGraphType.Knowledge_Graph,
-        trapi_version=TRAPI_1_3_0,
-        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        target_provenance=query[1]
-    )
-    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
-    check_messages(validator, query[2])
+def test_pre_trapi_1_4_0_validate_missing_or_empty_attributes(edge_data: Dict, validation_code: str):
+    validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph, trapi_version=TRAPI_1_3_0)
+    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=edge_data)
+    check_messages(validator, validation_code)
 
 
 @pytest.mark.parametrize(
-    "query",
+    "edge_data",
     [
-        # These tests should all pass in TRAPI releases >= 1.4.0-beta
-        # (
-        #         "mock_edge",  # mock data has dumb edges: don't worry about the S-P-O, just the attributes
-        #         "mock_context",
-        #         "AssertError_message"
-        # ),   # set 3rd argument to AssertError message if test edge should 'fail'; otherwise, empty string (for pass)
+        # These tests should all pass in TRAPI releases 'default' >= 1.4.0-beta
         (
             # Query 0. 'attributes' key missing in edge record is None
-            {},
-            get_ara_test_case(),
-            # "Edge has no 'attributes' key!"
-            ""
+            {}
         ),
         (
             # Query 1. Empty attributes
             {
                 "attributes": None
-            },
-            get_ara_test_case(),
-            # "Edge has empty attributes!"
-            ""
+            }
         ),
         (
             # Query 2. Empty attributes
             {
                 "attributes": []
-            },
-            get_ara_test_case(),
-            # "Edge has empty attributes!" Allowed
-            ""
+            }
         ),
         (
             # Query 3. EDAM-DATA:2526 ought to have an acceptable namespace
             {
                 "attributes": [
                     {
                         "attribute_type_id": "EDAM-DATA:2526",
                         "value": "some-value"
                     }
                 ]
-            },
-            get_ara_test_case(),
-            # "Edge has an acceptable namespace prefix
-            ""
+            }
+        ),
+        (
+            # Query 4. Validating terms in the ATTRIBUTE_TYPE_ID_INCLUSIONS list
+            {
+                "attributes": [
+                    {
+                        "attribute_type_id": "biolink:knowledge_level",
+                        "value": "knowledge_assertion"
+                    },
+                    {
+                        "attribute_type_id": "biolink:agent_type",
+                        "value": "manual_agent"
+                    }
+                ]
+            }
         )
-        # CHEMBL.COMPOUND:CHEMBL112--biolink:occurs_together_in_literature_with->NCBIGene:762
     ]
 )
-def test_post_1_4_0_trapi_validate_attributes(query: Tuple):
-    validator = BiolinkValidator(
-        graph_type=TRAPIGraphType.Knowledge_Graph,
-        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
-        target_provenance=query[1]
-    )
-    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=query[0])
-    check_messages(validator, query[2])
+def test_post_1_4_0_trapi_validate_attributes(edge_data: Dict):
+    validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
+    validator.validate_attributes(edge_id="test_validate_attributes unit test", edge=edge_data)
+    check_messages(validator, "")
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (
             # Query 0. Missing ARA knowledge source provenance?
```

### Comparing `reasoner_validator-3.7.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_response_validator.py` & `reasoner_validator-3.7.3/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_semver.py` & `reasoner_validator-3.7.3/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.3/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_validate.py` & `reasoner_validator-3.7.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_validation_report.py` & `reasoner_validator-3.7.3/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/tests/test_workflows.py` & `reasoner_validator-3.7.3/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.2/PKG-INFO` & `reasoner_validator-3.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.2
+Version: 3.7.3
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

