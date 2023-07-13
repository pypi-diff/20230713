# Comparing `tmp/pysros-23.3.3.tar.gz` & `tmp/pysros-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-23.3.3.tar", last modified: Thu Jun  1 23:31:46 2023, max compression
+gzip compressed data, was "pysros-23.7.1.tar", last modified: Thu Jul 13 12:30:02 2023, max compression
```

## Comparing `pysros-23.3.3.tar` & `pysros-23.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-06-01 23:31:33.000000 pysros-23.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 23:31:46.587482 pysros-23.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-01 23:31:33.000000 pysros-23.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/pysros/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    58672 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31722 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    46780 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-06-01 23:31:33.000000 pysros-23.3.3/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:31:46.587482 pysros-23.3.3/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 23:31:46.000000 pysros-23.3.3/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:31:46.587482 pysros-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:31:33.000000 pysros-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:30:02.898876 pysros-23.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-07-13 12:29:49.000000 pysros-23.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 12:30:02.898876 pysros-23.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-13 12:29:49.000000 pysros-23.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:30:02.894876 pysros-23.7.1/pysros/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58908 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20965 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31735 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-13 12:29:49.000000 pysros-23.7.1/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:30:02.898876 pysros-23.7.1/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-13 12:30:02.000000 pysros-23.7.1/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-13 12:30:02.000000 pysros-23.7.1/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:30:02.000000 pysros-23.7.1/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 12:30:02.000000 pysros-23.7.1/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 12:30:02.000000 pysros-23.7.1/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:30:02.898876 pysros-23.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-13 12:29:49.000000 pysros-23.7.1/setup.py
```

### Comparing `pysros-23.3.3/LICENSE.md` & `pysros-23.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/PKG-INFO` & `pysros-23.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.3
+Version: 23.7.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Python 3 for Nokia Service Router Operating System (pySROS) #
 
 ## Overview ##
 
@@ -38,15 +38,15 @@
 In order to use the pySROS library the following pre-requisites must be met:
 
 - One or more SR OS node
     - Running in model-driven mode
     - Running SR OS 21.7.R1 or greater (to execute applications on the SR OS device)
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
-- A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
+- A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
 Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
```

### Comparing `pysros-23.3.3/README.md` & `pysros-23.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 In order to use the pySROS library the following pre-requisites must be met:
 
 - One or more SR OS node
     - Running in model-driven mode
     - Running SR OS 21.7.R1 or greater (to execute applications on the SR OS device)
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
-- A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
+- A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
 Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
```

### Comparing `pysros-23.3.3/pysros/errors.py` & `pysros-23.7.1/pysros/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 .. reviewed by TechComms 20211202
 """
 
 pysros_err_action_subtree_not_supported = (SrosMgmtError, """Md-compare subtree-path is not supported in action method, use compare method instead""")
 pysros_err_arg_must_be_string = (TypeError, """Argument "module" must be a string""")
 pysros_err_attr_cannot_be_deleted = (AttributeError, "'{obj}' object attribute '{attribute}' cannot be deleted")
 pysros_err_attr_is_read_only = (AttributeError, "'{obj:.50}' object attribute '{attribute:.100}' is read-only")
+pysros_err_attr_object_has_no_attribute = (AttributeError, "'{obj}' object has no attribute '{attribute}'")
 pysros_err_can_check_state_from_running_only = (SrosMgmtError, "State can be checked from running datastore only")
 pysros_err_can_get_state_from_running_only = (LookupError, "State can be retrieved from running datastore only")
 pysros_err_can_have_one_semicolon = (InvalidPathError, "Identifier can contain only one ':'")
 pysros_err_can_not_find_yang = (ModelProcessingError, "Cannot find yang '{yang_name}'")
 pysros_err_cannot_call_go_to_parent = (InvalidPathError, "Cannot call go_to_parent on root")
 pysros_err_cannot_delete_from_state = (SrosMgmtError, "Cannot delete from state tree")
 pysros_err_cannot_lock_and_unlock_running = (SrosMgmtError, "Cannot lock and unlock running config")
 pysros_err_cannot_modify_config = (SrosMgmtError, "Cannot modify running config")
 pysros_err_cannot_modify_state = (SrosMgmtError, "Cannot modify state tree")
 pysros_err_cannot_pars_path = (ModelProcessingError, "Cannot parse path {path!r}")
 pysros_err_cannot_remove_node = (ModelProcessingError, "Cannot remove {node}")
 pysros_err_cannot_specify_non_key_leaf = (InvalidPathError, "Cannot specify non-key leaf as path attribute")
 pysros_err_commit_conflicts_detected = (SrosConfigConflictError, "Commit failed - conflict detected, configuration changes cleared")
+pysros_err_convert_invalid_value_for_type = (SrosMgmtError, "Invalid value for {name}")
+pysros_err_convert_root_not_support_pysros = (SrosMgmtError, "'pysros' format is not supported for root")
+pysros_err_convert_wrong_payload_type = (TypeError, "Invalid payload type for convert")
 pysros_err_could_not_create_conn = (RuntimeError, "Cannot create connection - {reason}")
 pysros_err_data_missing = (SrosMgmtError, "Entry does not exist")
 pysros_err_depth_must_be_positive = (ValueError, "Depth must be > 0")
 pysros_err_duplicate_found = (SrosMgmtError, "Entry cannot contain duplicates - {duplicate}")
 pysros_err_empty_path = (InvalidPathError, "Empty path")
 pysros_err_entry_does_not_exists = (KeyError, "Entry does not exist")
 pysros_err_even_num_of_columns_required = (ValueError, "Even number of data columns required")
@@ -46,60 +50,58 @@
 pysros_err_invalid_identifier = (InvalidPathError, "Invalid identifier")
 pysros_err_invalid_json_structure = (ValueError, "Invalid JSON structure")
 pysros_err_invalid_key_in_path = (SrosMgmtError, "Invalid key value in path")
 pysros_err_invalid_module_set_id_or_content_id = (RuntimeError, "Invalid module-set-id")
 pysros_err_invalid_operation_on_key = (InvalidPathError, "Operation cannot be performed on key")
 pysros_err_invalid_operation_on_leaflist = (InvalidPathError, "Operation cannot be performed on leaflist")
 pysros_err_invalid_path_operation_missing_keys = (InvalidPathError, "Cannot perform operation on list without specifying keys")
+pysros_err_invalid_rd_state = (InternalError, "Invalid database state")
 pysros_err_invalid_target = (ValueError, "Invalid target")
 pysros_err_invalid_transport = (TypeError, "Currently only NETCONF transport is supported")
 pysros_err_invalid_value = (TypeError, "MO contents not a dict '{data}'")
 pysros_err_invalid_value_for_type = (TypeError, "Invalid value for {type}: {value}")
+pysros_err_invalid_xml_element = (ValueError, 'XML element {element} can be empty or contain another XML element')
+pysros_err_invalid_xml_root = (ValueError, 'XML root element can be empty or contain another XML element')
 pysros_err_invalid_yang_path = (ModelProcessingError, "Invalid path {path!r}")
 pysros_err_key_val_mismatch = (SrosMgmtError, "Cannot change value of key-leaf '{key_name}'")
 pysros_err_leaflist_should_be_list = (TypeError, "expected list object but got {type_name}")
 pysros_err_malformed_keys = (TypeError, "Malformed keys for '{full_path}' with value '{value}'")
+pysros_err_malformed_xml = (ValueError, "Malformed XML")
 pysros_err_missing_keys = (InvalidPathError, "Missing keys on element '{element}'")
+pysros_err_multiple_occurences_of_entry = (SrosMgmtError, "Multiple occurrences of list entry")
+pysros_err_multiple_occurences_of_node = (SrosMgmtError, "Multiple occurrences of node")
 pysros_err_no_data_found = (LookupError, "No data found")
 pysros_err_not_connected = (RuntimeError, "Not connected")
 pysros_err_not_found_slash_before_name = (InvalidPathError, "'/' not found before element name")
 pysros_err_path_should_be_string = (TypeError, "path argument should be a string")
 pysros_err_prefix_does_not_have_ns = (LookupError, "prefix '{prefix}' of '{name}' does not have corresponding namespace")
 pysros_err_root_path = (InvalidPathError, "Operation cannot be performed on root")
 pysros_err_target_should_be_list = (InvalidPathError, "Target should be a list")
 pysros_err_type_must_be = (TypeError, "must be {expected:.50s}, not {actual:.50s}")
 pysros_err_unended_quoted_string = (InvalidPathError, "Unended quoted string")
 pysros_err_unexpected_change_of_path_ctx = (ModelProcessingError, "Unexpected change of path ctx")
 pysros_err_unexpected_end_of_yang = (ModelProcessingError, "Unexpected end of YANG")
 pysros_err_unexpected_token = (ModelProcessingError, "Unexpected token {token}")
 pysros_err_unexpected_value_of_type = (TypeError, "Unexpected value of type '{val_type}' in '{type}'")
 pysros_err_unknown_child = (SrosMgmtError, "Cannot find child with name '{child_name}' in path '{path}'")
+pysros_err_unknown_field = (SrosMgmtError, "Cannot find field with name '{field_name}' in path '{path}'")
 pysros_err_unknown_dds = (InternalError, "Unknown data definition statement type {dds}")
 pysros_err_unknown_dev_statement = (ModelProcessingError, "Unknown deviate statement: {stmt!r}'")
 pysros_err_unknown_element = (InvalidPathError, "Unknown element '{element}'")
 pysros_err_unknown_identityref = (ModelProcessingError, "Unknown identityref {identifier}")
 pysros_err_unknown_key = (InvalidPathError, "Unknown key '{key_name}'")
 pysros_err_unknown_prefix_for_name = (ModelProcessingError, "Unknown prefix '{prefix}' for '{name}'")
 pysros_err_unresolved_augment = (InternalError, "Augments cannot be resolved")
 pysros_err_unresolved_leafref = (InternalError, "Unresolved leafref {type}")
 pysros_err_unresolved_type = (InternalError, "Unresolved type in schema: {type}")
+pysros_err_unsupported_action_io = (SrosMgmtError, "Unsupported value of argument action_io")
+pysros_err_unsupported_action_path = (InvalidPathError, "Path does not point to an action")
+pysros_err_unsupported_compare_datastore = (SrosMgmtError, "Compare is only supported against the candidate datastore")
+pysros_err_unsupported_compare_endpoint = (InvalidPathError, "Unsupported compare path endpoint")
+pysros_err_unsupported_compare_method = (SrosMgmtError, "Unsupported compare method")
+pysros_err_unsupported_convert_method = (SrosMgmtError, "Unsupported convert method")
 pysros_err_unsupported_set_method = (SrosMgmtError, "Unsupported set method")
 pysros_err_unsupported_type_for_wrapper = (TypeError, "Unsupported type for {wrapper_name} data")
 pysros_err_use_deepcopy = (NotImplementedError, "Use '.deepcopy' instead")
+pysros_err_wrong_json_root = (JsonDecodeError, "JSON root must be object")
 pysros_err_wrong_netconf_response = (SrosMgmtError, "Wrong NETCONF response")
 pysros_err_wrong_rhs = (ModelProcessingError, "Invalid argument to the right of the plus symbol")
-pysros_err_unsupported_compare_method = (SrosMgmtError, "Unsupported compare method")
-pysros_err_unsupported_compare_datastore = (SrosMgmtError, "Compare is only supported against the candidate datastore")
-pysros_err_unsupported_compare_endpoint = (InvalidPathError, "Unsupported compare path endpoint")
-pysros_err_unsupported_action_path = (InvalidPathError, "Path does not point to an action")
-pysros_err_unsupported_convert_method = (SrosMgmtError, "Unsupported convert method")
-pysros_err_unsupported_action_io = (SrosMgmtError, "Unsupported value of argument action_io")
-pysros_err_invalid_rd_state = (InternalError, "Invalid database state")
-pysros_err_convert_root_not_support_pysros = (SrosMgmtError, "'pysros' format is not supported for root")
-pysros_err_convert_wrong_payload_type = (TypeError, "Invalid payload type for convert")
-pysros_err_wrong_json_root = (JsonDecodeError, "JSON root must be object")
-pysros_err_malformed_xml = (ValueError, "Malformed XML")
-pysros_err_multiple_occurences_of_node = (SrosMgmtError, "Multiple occurrences of node")
-pysros_err_multiple_occurences_of_entry = (SrosMgmtError, "Multiple occurrences of list entry")
-pysros_err_convert_invalid_value_for_type = (SrosMgmtError, "Invalid value for {name}")
-pysros_err_invalid_xml_element = (ValueError, 'XML element {element} can be empty or contain another XML element')
-pysros_err_invalid_xml_root = (ValueError, 'XML root element can be empty or contain another XML element')
```

### Comparing `pysros-23.3.3/pysros/exceptions.py` & `pysros-23.7.1/pysros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/identifier.py` & `pysros-23.7.1/pysros/identifier.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/management.py` & `pysros-23.7.1/pysros/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,24 +192,25 @@
 
     def __init__(self, *args, yang_directory, rebuild, **kwargs):
         try:
             self._nc        = manager.connect_ssh(*args, **kwargs)
         except Exception as e:
             raise make_exception(pysros_err_could_not_create_conn, reason=e) from None
 
-        self.running    = Datastore(self, 'running')
-        self.candidate  = Datastore(self, 'candidate')
+        self.running                = Datastore(self, 'running')
+        self.candidate              = Datastore(self, 'candidate')
 
-        self.yang_directory = yang_directory
-        self.rebuild = rebuild
-        self._models    = self._get_yang_models()
-        self._ns_map    = types.MappingProxyType({model.name: model.namespace for model in self._models})
-        self._mod_revs  = {model.name: model.revision for model in self._models}
-        self.root = self._get_root(self._models)
-        self.debug      = False
+        self.yang_directory         = yang_directory
+        self.rebuild                = rebuild
+        self._models                = self._get_yang_models()
+        self._ns_map                = types.MappingProxyType({model.name: model.namespace for model in self._models})
+        self._ns_map_rev            = {v : k for k, v in self._ns_map.items()}
+        self._mod_revs              = {model.name: model.revision for model in self._models}
+        self.root                   = self._get_root(self._models)
+        self.debug                  = False
 
     def _get_root(self, modules):
         hasher = hashlib.sha256()
         yangs = sorted(modules, key = lambda m: m.name)
         hasher.update(b"Schema ver 5\n")
         for m in yangs:
             hasher.update(f"mod:{m.name};rev:{m.revision};".encode())
@@ -303,16 +304,19 @@
                 name       = get_text(m, "./library:name"),
                 namespace  = get_text(m, "./library:namespace"),
                 revision   = get_text(m, "./library:revision"),
                 submodules = tuple(submodules)
             ))
         return tuple(result)
 
+    def _request_data(self, **kwargs):
+        return RequestData(self.root, self._ns_map, self._ns_map_rev, **kwargs)
+
     def _action(self, path, value):
-        rd = RequestData(self.root, self._ns_map, walker=ActionInputFilteredDataModelWalker)
+        rd = self._request_data(walker=ActionInputFilteredDataModelWalker)
         current = rd.process_path(path)
         if not current.is_action():
             raise make_exception(pysros_err_unsupported_action_path)
         if current._walker.current.name.name == "md-compare" and "path" in value and "subtree-path" in value["path"]:
             raise make_exception(pysros_err_action_subtree_not_supported)
         current.set(value)
 
@@ -326,30 +330,32 @@
         response = self._nc.rpc(xml_action)
 
         if self.debug:
             print("ACTION response")
             print(response)
 
         del rd
-        rd = RequestData(self.root, self._ns_map, walker=ActionOutputFilteredDataModelWalker)
+        rd = self._request_data(walker=ActionOutputFilteredDataModelWalker)
+        #data should be wrapped in dummy root. RPC reply can be dummy root if does not have attributes
+        response.xpath('.')[0].attrib.clear()
         rd.set_action_as_xml(path, response)
         current = rd.process_path(path, strict=True)
         return current.to_model()
 
     def _convert(self, path, payload, src_fmt, dst_fmt, pretty_print, action_io):
         def convert_walker(action_io):
             if action_io == "input":
                 return ActionInputFilteredDataModelWalker
             elif action_io == "output":
                 return ActionOutputFilteredDataModelWalker
             raise make_exception(pysros_err_unsupported_action_io)
 
         if not all(fmt in ("xml", "json", "pysros") for fmt in (src_fmt, dst_fmt)):
             raise make_exception(pysros_err_unsupported_convert_method)
-        rd = RequestData(self.root, self._ns_map, action=RequestData._Action.convert, walker=convert_walker(action_io))
+        rd = self._request_data(action=RequestData._Action.convert, walker=convert_walker(action_io))
         current = rd.process_path(path)
 
         if src_fmt == "pysros":
             current.set(payload)
         elif src_fmt == "xml":
             if not isinstance(payload, str):
                 raise make_exception(pysros_err_convert_wrong_payload_type)
@@ -630,15 +636,14 @@
         return "report-all" if defaults else None
 
     def _check_empty_string(self, model_walker):
         for k in model_walker.keys:
             if '' in k.values():
                 raise make_exception(pysros_err_filter_empty_string)
 
-
     def _prepare_root_ele(self, subtree, path):
         root = etree.Element("filter")
         root.extend(subtree)
         if self.debug:
             print("GET request for path ", path)
             print(etree.dump(root))
         return root
@@ -661,15 +666,15 @@
         model_walker = custom_walker if custom_walker else FilteredDataModelWalker.user_path_parse(self.connection.root, path)
 
         if config_only and model_walker.is_state:
             raise make_exception(pysros_err_no_data_found)
 
         self._check_empty_string(model_walker)
 
-        rd = RequestData(self.connection.root, self.connection._ns_map)
+        rd = self.connection._request_data()
         current = rd.process_path(model_walker)
         if filter is not None:
             model_walker.validate_get_filter(filter)
             current.set_filter(filter)
         config = rd.to_xml()
 
         if self.target == "running":
@@ -685,15 +690,15 @@
             response = self._operation_get_config(config, defaults, path)
 
         if self.debug:
             print("GET response")
             print(response)
         del rd, current
 
-        rd = RequestData(self.connection.root, self.connection._ns_map)
+        rd = self.connection._request_data()
         rd.set_as_xml(response)
         try:
             current = rd.process_path(model_walker, strict=True)
         except LookupError as e:
             #two possible scenarions - entry does not exists or is empty
             #if has presence and LookupError is raised, it does not exists
             if model_walker.has_explicit_presence() and not filter:
@@ -720,26 +725,26 @@
         if self.target == 'running':
             raise make_exception(pysros_err_cannot_modify_config)
         if method != 'merge' and method != 'replace':
             raise make_exception(pysros_err_unsupported_set_method)
         model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
         if model_walker.current.config == False:
             raise make_exception(pysros_err_cannot_modify_state)
-        rd = RequestData(self.connection.root, self.connection._ns_map)
+        rd = self.connection._request_data()
         if action == Datastore._SetAction.delete:
             default_operation="none"
             rd.process_path(path).delete()
         else:
             default_operation="merge"
             current = rd.process_path(path)
             current.set(value)
             if method == "replace":
                 current.replace()
         children = rd.to_xml()
-        config = new_ele_nsmap("config", rd._extra_namespaces)
+        config = new_ele_nsmap("config", rd._extra_ns)
 
         config.extend(children)
         if self.debug:
             print("SET request")
             print(f"path: '{path}', value: '{value}'")
             print(etree.dump(config))
         self.nc.edit_config(target=self.target, default_operation=default_operation, config=config)
@@ -774,15 +779,15 @@
                 return False
             return True
 
     def _get_list_keys(self, path, defaults):
         model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
         self._check_empty_string(model_walker)
 
-        rd = RequestData(self.connection.root, self.connection._ns_map)
+        rd = self.connection._request_data()
         current = rd.process_path(model_walker)
 
         #get possible errors related to the getting candidate from state before
         #errors related to the incorrect path while calling entry_get_keys
         if self.target == "candidate" and model_walker.current.config == False:
             raise make_exception(pysros_err_can_get_state_from_running_only)
 
@@ -795,15 +800,15 @@
             response = self._operation_get_config(config, defaults, path)
 
         if self.debug:
             print("GET response")
             print(response)
         del rd, current
 
-        rd = RequestData(self.connection.root, self.connection._ns_map)
+        rd = self.connection._request_data()
         rd.set_as_xml(response)
         try:
             current = rd.process_path(model_walker, strict=True)
         except LookupError as e:
             #two possible scenarios - list has no entries or path does not exist
             #doing exists to check whether really exists or not
             model_walker_copy = model_walker.copy()
@@ -827,15 +832,15 @@
 
         path = user_path if user_path != "/" else ""
 
         if path:
             model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
             if model_walker.current.config == False:
                 raise make_exception(pysros_err_unsupported_compare_endpoint)
-            rd = RequestData(self.connection.root, self.connection._ns_map)
+            rd = self.connection._request_data()
             current = rd.process_path(model_walker)
             if not current.is_compare_supported_endpoint():
                 raise make_exception(pysros_err_unsupported_compare_endpoint)
             path = rd.to_xml()
 
         op_ns = COMMON_NAMESPACES["nokiaoper"]
         xml_action = etree.Element(f"""{{{COMMON_NAMESPACES["yang_1_0"]}}}action""")
```

### Comparing `pysros-23.3.3/pysros/model.py` & `pysros-23.7.1/pysros/model.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/model_builder.py` & `pysros-23.7.1/pysros/model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,14 +411,17 @@
         self.resolve_identities()
         self.resolve_leafrefs()
         self.resolve_config()
         self.resolve_namespaces()
         self.delete_blueprints()
         self.convert_model()
 
+    def walk_models(self, cb):
+        self.root.recursive_walk(cb)
+
     def perform_parse(self, yang_name, yang_handler=None):
         if yang_name in self.parsed_yangs:
             return
         self.parsed_yangs.add(yang_name)
 
         yang_parser(self.get_module_content(yang_name), yang_handler or YangHandler(self, self.root))
 
@@ -457,15 +460,15 @@
             assert not key in self.resolved_types
             self.resolved_types[key] = resolve_typedefs_deep(value, self.types_to_resolve)
             if key in IP_TYPES:
                 assert isinstance(self.resolved_types[key].yang_type, YangUnion)
                 self.resolved_types[key].yang_type.deduplicate()
                 assert len(self.resolved_types[key].yang_type) == 1 and self.resolved_types[key].yang_type._types[0].identifier.name == "string"
                 self.resolved_types[key].yang_type = self.resolved_types[key].yang_type._types[0]
-        self.root.recursive_walk(self.set_correct_types)
+        self.walk_models(self.set_correct_types)
 
     def set_correct_range(self, yt:YangTypeBase):
         assert yt.json_name() != "decimal64" or yt.fraction_digits
         if isinstance(yt, YangUnion):
             for t in yt:
                 self.set_correct_range(t)
 
@@ -519,28 +522,28 @@
         else:
             yt.yang_range   = work_range
 
     def resolve_type_ranges(self):
         def setter(m:BuildingModel):
             if isinstance(m.yang_type, YangTypeBase):
                 self.set_correct_range(m.yang_type)
-        self.root.recursive_walk(setter)
+        self.walk_models(setter)
 
     def resolve_identities(self):
         # first step creates dict, where we find for each identity
         # its all identities, that are directly derived from it.
         directly_derived: DefaultDict[Identifier, Set[Identifier]] = defaultdict(set)
         def find_derived(m:BuildingModel):
             if m.data_def_stm != BuildingModel.StatementType.identity_:
                 return
             for b in m.identity_bases:
                 if m.status != 'obsolete':
                     directly_derived[b].add(m.name)
 
-        self.root.recursive_walk(find_derived)
+        self.walk_models(find_derived)
         # second step adds all direct and indirect derived identities together
         def add_derived_recursive(result_set, id):
             got = directly_derived.get(id, set())
             toUpdate = got - result_set
             result_set.update(got)
             for c in toUpdate:
                 add_derived_recursive(result_set, c)
@@ -557,15 +560,15 @@
             if type(m.yang_type) is IdentityRef:
                 m.yang_type.set_values(derived, self._ns_map)
             elif type(m.yang_type) is YangUnion:
                 for st in m.yang_type:
                     if type(st) is IdentityRef:
                         st.set_values(derived, self._ns_map)
 
-        self.root.recursive_walk(identityref_set_value)
+        self.walk_models(identityref_set_value)
 
     def resolve_leafrefs(self):
         def replace_leafrefs(m: BuildingModel):
             if not isinstance(m.yang_type, LeafRef):
                 return
 
             w = DataModelWalker(m)
@@ -576,15 +579,15 @@
                 module_name = w.current.name.prefix
                 if path._path and path._path[0].name != '..':
                     # absolute path - go to root
                     while not w.is_root:
                         w.go_to_parent()
                 w.go_to(path, module_name)
             m.yang_type = w.current.yang_type
-        self.root.recursive_walk(replace_leafrefs)
+        self.walk_models(replace_leafrefs)
 
     def resolve_groupings(self):
         def inner(m:BuildingModel):
             if m.data_def_stm == BuildingModel.StatementType.uses_:
                 if m.has_children:
                     return False
                 for child in self.groupings[m.name].children:
@@ -665,25 +668,25 @@
     def build_blueprints(self):
         handler = YangHandler(self, self.root)
         handler.construct()
 
     def delete_blueprints(self):
         def deleter(m: BuildingModel):
             del m.blueprint
-        self.root.recursive_walk(deleter)
+        self.walk_models(deleter)
 
     def resolve_config(self):
         def false_setter(m: BuildingModel):
             m.config = False
         def resolver(m: BuildingModel):
             if not m.config:
                 m.recursive_walk(false_setter)
                 return False
 
-        self.root.recursive_walk(resolver)
+        self.walk_models(resolver)
 
     def convert_model(self):
         new_root = StorageConstructionModel("root", BuildingModel.StatementType["container_"], None)
         w = DataModelWalker(self.root)
 
         stack = [new_root]
```

### Comparing `pysros-23.3.3/pysros/model_path.py` & `pysros-23.7.1/pysros/model_path.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/model_walker.py` & `pysros-23.7.1/pysros/model_walker.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/pprint.py` & `pysros-23.7.1/pysros/pprint.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/request_data.py` & `pysros-23.7.1/pysros/request_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from contextlib import ExitStack
 from enum import Enum, auto
 from lxml import etree
 from ncclient.xml_ import to_ele
-from typing import Union
+from typing import Union, List, Dict
 
 from .errors import *
 from .identifier import NoModule, Identifier
 from .model import Model
 from .model_walker import FilteredDataModelWalker, ModelWalker
 from .singleton import _Singleton, Empty
 from .wrappers import Wrapper, Action, Container, Leaf, LeafList
@@ -29,18 +29,44 @@
     "attrs"    : "urn:nokia.com:sros:ns:yang:sr:attributes",
 }
 
 MO_STATEMENT_TYPES = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.action_)
 FIELD_STATEMENT_TYPES = (Model.StatementType.leaf_, Model.StatementType.leaf_list_)
 
 _get_tag_name = lambda x: etree.QName(x).localname
+_get_tag_ns = lambda x: etree.QName(x).namespace
 _text_in_tag_tail = lambda x: x.tail and x.tail.strip()
 _text_in_tag_text = lambda x: x.text and x.text.strip()
 _create_root_ele = lambda : etree.Element("dummy-root", nsmap={"nokia-attr": COMMON_NAMESPACES["attrs"]})
 
+def subelement(parent, tag, nsmap, text=None, attrib=None, add_ns=None):
+    """Wrapper around etree.Subelement, that raises SrosMgmtError instead of ValueError."""
+    local_nsmap = {}
+    if add_ns:
+        local_nsmap[add_ns] = nsmap[add_ns]
+    try:
+        if tag.is_builtin():
+            result = etree.SubElement(parent, tag.name, attrib, nsmap=local_nsmap)
+        else:
+            module = tag.prefix
+            uri = nsmap[module]
+            local_nsmap[module] = uri
+            result = etree.SubElement(
+                parent,
+                etree.QName(uri, tag.name),
+                attrib,
+                nsmap=local_nsmap
+            )
+
+        if text is not None:
+            result.text = text
+        return result
+    except ValueError as err:
+        raise SrosMgmtError(err.args) from None
+
 def _raise_invalid_text_exception(tag, check_parent_tag=True):
     tag_to_check = tag.getparent() if check_parent_tag else tag
     if tag_to_check.tag == "dummy-root":
         raise make_exception(pysros_err_invalid_xml_root)
     else:
         raise make_exception(pysros_err_invalid_xml_element, element=_get_tag_name(tag_to_check))
 
@@ -58,31 +84,32 @@
     .. Reviewed by TechComms 20210712
     """
 
     class _Action(Enum):
         basic   = auto()
         convert = auto()
 
-    def __init__(self, root:Model, ns_map:dict, action:_Action=_Action.basic, walker=FilteredDataModelWalker):
-        self._root = root
-        self._data = _ListStorage(root, self)
-        self._ns_map = ns_map
-        self._action = action
-        self._Walker = walker
-        self._extra_namespaces = {}
+    def __init__(self, root:Model, ns_map:dict, ns_map_rev:dict, *, action:_Action=_Action.basic, walker=FilteredDataModelWalker):
+        self._root             = root
+        self._data             = _ListStorage(root, self)
+        self._ns_map           = ns_map
+        self._ns_map_rev       = ns_map_rev
+        self._action           = action
+        self._Walker           = walker
+        self._extra_ns         = {}
 
     def process_path(self, path:Union[str, FilteredDataModelWalker], *, strict=False):
         """Create all entries in given path and return setter for last section of the path.
 
         .. Reviewed by TechComms 20210712
         """
         walker = path if isinstance(path, ModelWalker) else self._Walker.user_path_parse(self._root, path, accept_root=(self._action == self._Action.convert))
         current = _ASetter.create_setter(self._data, self)
         for elem, keys in zip(walker.path, walker.keys):
-            if not isinstance(current, _MoDataSetter):
+            if not isinstance(current, _MoSetter):
                 raise make_exception(pysros_err_missing_keys, element=current._walker.get_name())
             if elem.data_def_stm not in FIELD_STATEMENT_TYPES:
                 if strict and not current.child_mos.is_created(elem.name.name):
                     raise make_exception(pysros_err_no_data_found)
                 current = current.child_mos.get_or_create(elem.name.name)
                 if keys:
                     if strict and not current.entry_exists_nocheck(keys):
@@ -153,17 +180,18 @@
         .. Reviewed by TechComms 20210712
         """
         self._data.debug_dump()
 
     def _unwrap(self, value):
         return value.data if isinstance(value, Wrapper) else value
 
+
     def _add_xml_namespace(self, identity):
         assert self._ns_map[identity.module] == identity.namespace
-        self._extra_namespaces[identity.module] = identity.namespace
+        self._extra_ns[identity.module] = identity.namespace
 
 
 class _AStorage(ABC):
     """Abstract representation of data storage.
 
     .. Reviewed by TechComms 20210712
     """
@@ -200,97 +228,78 @@
         if model.name.prefix in ns_map:
             return etree.QName(ns_map[model.name.prefix], model.name.name)
         elif model.name.prefix is NoModule():
             return model.name.name
         else:
             raise make_exception(pysros_err_prefix_does_not_have_ns, prefix=model.name.prefix, name=model.name.name)
 
-def subelement(parent, tag, nsmap, text=None, attrib=None, add_ns=None):
-    """Wrapper around etree.Subelement, that raises SrosMgmtError instead of ValueError."""
-    local_nsmap = {}
-    if add_ns:
-        local_nsmap[add_ns] = nsmap[add_ns]
-    try:
-        if tag.is_builtin():
-            result = etree.SubElement(parent, tag.name, attrib, nsmap=local_nsmap)
+class _FieldStorage(_AStorage):
+    """Data storage for leaves.
+    """
+
+    def __init__(self, model:Model, rd:RequestData):
+        super().__init__(rd)
+        self._model = model
+        self._value = None
+        self._operation = ""
+
+    def _to_xml(self, ns_map, root):
+        if self._operation == "delete":
+            subelement(root, self._walker.current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
+        elif self._value is FieldValuePlaceholder():
+            pass
+        elif self._value is GetValuePlaceholder():
+            subelement(root, self._walker.current.name, ns_map)
         else:
-            module = tag.prefix
-            uri = nsmap[module]
-            local_nsmap[module] = uri
-            result = etree.SubElement(
-                parent,
-                etree.QName(uri, tag.name),
-                attrib,
-                nsmap=local_nsmap
-            )
+            _leaf_to_xml(self._value, root, self._walker, ns_map, self._operation=="replace")
+
+    def to_model(self, *, key_filter={}):
+        assert self.rd._action == RequestData._Action.convert or self._value is not GetValuePlaceholder()
+        assert self._value is not FieldValuePlaceholder()
+        if self._walker.get_dds() == Model.StatementType.leaf_:
+            return Leaf._with_model(self._value, self._model)
+        return LeafList._with_model(self._value, self._model)
+
+    def debug_dump(self, indent=0):
+        print(f"{' '*(indent+1)}{self._model.name} = {self._value}")
 
-        if text is not None:
-            result.text = text
-        return result
-    except ValueError as err:
-        raise SrosMgmtError(err.args) from None
 
 class _MoStorage(_AStorage):
     """Data storage for containers and list entries (list+local keys).
 
     .. Reviewed by TechComms 20210712
     """
 
     def __init__(self, model:Model, local_keys, rd:RequestData):
         super().__init__(rd)
         self._model = model
         self._local_keys = copy.deepcopy(local_keys)
         self._child = {}
         self._operation = ""
-        self._replace_field = "" # Could be field storage
 
     def _to_xml(self, ns_map, root):
-        root_attr = None if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
+        root_attr = {} if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
         root = subelement(root, self._model.name, ns_map, None, root_attr)
         for k, v in self._local_keys.items():
             if v is FieldValuePlaceholder():
                 pass
             elif v is GetValuePlaceholder():
                 self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
             else:
                txt, add_ns = self._walker.get_child(k).get_type().to_string(v)
                subelement(root, self._walker.get_child(k).current.name, ns_map, txt, {}, add_ns)
 
         for k, v in self._child.items():
-            if isinstance(v, (_MoStorage, _ListStorage)):
-                v._to_xml(ns_map, root)
-            else:
-                if v is Delete():
-                    subelement(root, self._walker.get_child(k).current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
-                elif v is FieldValuePlaceholder():
-                    pass
-                elif v is GetValuePlaceholder():
-                    self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
-                elif self._replace_field and self._replace_field == k:
-                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map, replace_field=True)
-                else:
-                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map)
+            v._to_xml(ns_map,root)
 
     def to_xml(self, ns_map, root):
-        root_attr = None if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
+        root_attr = {} if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
 
         for k, v in self._child.items():
-            if isinstance(v, (_MoStorage, _ListStorage)):
-                v._to_xml(ns_map, root)
-            else:
-                if v is Delete():
-                    subelement(root, self._walker.get_child(k).current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
-                elif v is FieldValuePlaceholder():
-                    pass
-                elif v is GetValuePlaceholder():
-                    self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
-                elif self._replace_field and self._replace_field == k:
-                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map, replace_field=True)
-                else:
-                    _leaf_to_xml(v, root, self._walker.get_child(k), ns_map)
+            v._to_xml(ns_map, root)
 
     def _leaf_placeholder_to_xml(self, value, root, walker, ns_map):
         subelement(root, walker.current.name, ns_map)
 
     def to_model(self, *, key_filter={}):
         data = {}
         is_selection_filter = {} in key_filter.values()
@@ -298,20 +307,17 @@
             if is_selection_filter and k not in key_filter:
                 continue
             data[k] = self._leaf_to_model(k, v)
         for k, v in self._child.items():
             key_proxy = DictionaryKeysProxy(self.rd._unwrap(key_filter))
             if is_selection_filter and self._walker.get_child(k).current.name not in key_proxy:
                 continue
-            if not isinstance(v, (_MoStorage, _ListStorage)):
-                data[k] = self._leaf_to_model(k, v)
-            else:
-                data[k] = v.to_model(key_filter=(key_filter.get(k, {})))
-                if not data[k] and not self._walker.get_child(k).has_explicit_presence():
-                    del data[k]
+            data[k] = v.to_model(key_filter=(key_filter.get(k, {})))
+            if not data[k] and not self._walker.get_child(k).has_explicit_presence():
+                del data[k]
         if self._walker.is_root:
             return data
         if self._model.data_def_stm == Model.StatementType.action_:
             return Action._with_model(data, self._model)
         return Container._with_model(data, self._model)
 
     def _leaf_to_model(self, name, value):
@@ -458,34 +464,47 @@
 
     def _unwrap(self, val):
         return val.data if isinstance(val, Wrapper) else val
 
 class RdJsonEncoder(json.JSONEncoder):
     def add_ns(self, o, d, walker:ModelWalker):
         if o is self.root:
-            return {walker.get_child(k).get_name().model_string: v for k, v in d.items()}
-        return {walker.get_child(k).get_name().model_string if walker.get_name().prefix != walker.get_child(k).get_name().prefix else k: v for k, v in d.items()}
+            return {walker.get_child(k).get_name().model_string: (v if not isinstance(v, _FieldStorage) else v._value) for k, v in d.items()}
+        return {walker.get_child(k).get_name().model_string if walker.get_name().prefix != walker.get_child(k).get_name().prefix else k: (v if not isinstance(v, _FieldStorage) else v._value) for k, v in d.items()}
+
+    def stringify(self, x, dds):
+        return [str(v) for v in x] if dds == Model.StatementType.leaf_list_ else str(x)
+
+    def convert(self, o:_FieldStorage):
+        return self.stringify(o._value, o._walker.get_dds()) if o._walker.get_type().json_name() in ("int64", "uint64") else o._value
+
+    def convert_child(self, o, k, v):
+        return self.stringify(v, o._walker.get_child_dds(k)) if o._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES and o._walker.get_child_type(k).json_name() in ("int64", "uint64") else v
 
     def default(self, o):
         is_root = o is self.root
+        if isinstance(o, _FieldStorage) and is_root:
+            res = {}
+            res[o._walker.get_name().model_string] = self.convert(o)
+            return res
         if isinstance(o, _MoStorage):
             res = {}
             if not is_root:
                 res.update(self.add_ns(o, o._local_keys, o._walker))
             elif is_root and self.force_key:
                 res[o._walker.get_child(self.force_key).get_name().model_string] = o._local_keys[self.force_key]
             res.update(self.add_ns(o, o._child, o._walker))
-            stringify = lambda x, dds: [str(v) for v in x] if dds == Model.StatementType.leaf_list_ else str(x)
-            cvt = lambda k, v: stringify(v, o._walker.get_child_dds(k)) if o._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES and o._walker.get_child_type(k).json_name() in ("int64", "uint64") else v
-            res = {k: cvt(k, v) for k, v in res.items()}
+            res = {k: self.convert_child(o, k, v) for k, v in res.items()}
             return res
         elif isinstance(o, _ListStorage):
             res = list(o._entries.values())
             return {o._walker.get_name().model_string: res} if is_root else res
-        elif isinstance(o, (str, list, dict, bool)):
+        if isinstance(o, _FieldStorage):
+            o = o._value
+        if isinstance(o, (str, list, dict, bool, int)):
             return o
         elif o is Empty:
             return [None]
         else:
             return str(o)
 
 class _ASetter(ABC):
@@ -500,15 +519,15 @@
     @property
     def _walker(self):
         return self.rd._Walker(self._storage._model)
 
     @staticmethod
     def create_setter(storage:"_AStorage", rd:RequestData):
         if isinstance(storage, _MoStorage):
-            return _MoDataSetter(storage, rd)
+            return _MoSetter(storage, rd)
         else:
             return _ListSetter(storage, rd)
 
     @abstractmethod
     def set(self, value):
         """Set data in model format.
 
@@ -624,40 +643,40 @@
 
 class _LeafSetter(_ASetter):
     """Interface for managing leafs. Because leafs do not have dedicated storage, the
        class has its own implementation of to_model method.
 
     .. Reviewed by TechComms 20210713
     """
-    def __init__(self, storage:"_ListStorage", leaf_name:str, rd:RequestData):
+    def __init__(self, storage:"_FieldStorage", leaf_name:str, rd:RequestData):
         super().__init__(storage, rd)
         self._leaf_name = leaf_name
 
     def set(self, value):
         value = self.rd._unwrap(value)
         if not self._walker.check_field_value(value):
             raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._leaf_name)
         else:
             val = self._as_storage_type(value)
             self._set_nocheck(val)
 
     def _set_nocheck(self, value):
-        self._storage._child[self._leaf_name] = value
+        self._storage._value = value
 
     def set_getValue(self):
-        self._storage._child[self._leaf_name] = GetValuePlaceholder()
+        self._storage._value = GetValuePlaceholder()
 
     def set_as_xml(self, value):
         if not len(value):
             raise make_exception(pysros_err_malformed_xml)
         for v in value:
             self.set_or_append_as_xml(v)
 
     def _set_as_json(self, value, is_root = False):
-        if not isinstance(value, dict):
+        if not isinstance(value, dict) or not all(isinstance(k, str) for k in value):
             raise make_exception(pysros_err_invalid_json_structure)
         value = {k:v for k, v in value.items() if not k.startswith("@")}
         if len(value) != 1:
             raise make_exception(pysros_err_invalid_json_structure)
 
         val = next(iter(value.items()))
         if self._walker.get_name() != val[0]:
@@ -673,51 +692,48 @@
             try:
                 value = [int(self.rd._unwrap(v)) for v in val]
             except:
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name) from None
         self.set(self._walker.as_model_type(val))
 
     def set_or_append_as_xml(self, value_element):
-        if _text_in_tag_tail(value_element) or (self._walker.get_dds() == Model.StatementType.leaf_list_ and _text_in_tag_text(value_element.getparent())):
+        is_leaflist = self._walker.get_dds() == Model.StatementType.leaf_list_
+        if _text_in_tag_tail(value_element) or (is_leaflist and _text_in_tag_text(value_element.getparent())):
             _raise_invalid_text_exception(value_element)
         value = self._walker.as_model_type(value_element.text or "")
 
         if isinstance(self._walker.get_type(), IdentityRef):
             is_leaf_list = isinstance(value, list)
             assert not is_leaf_list or len(value) == 1
             identity = self._walker.get_type()._find_identity(value[0] if is_leaf_list else value)
             if not identity:
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
             value_ns = value_element.nsmap.get(identity.module, None)
             if value_ns is not None and value_ns!=identity.namespace:
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
 
-        if self._walker.get_dds() == Model.StatementType.leaf_list_ and isinstance(self._storage._child.get(self._leaf_name), list):
-            value = self._storage._child[self._leaf_name] + value
+        if is_leaflist and isinstance(self._storage._value, list):
+            value = self._storage._value + value
         self.set(value)
 
     def to_model(self, *, key_filter={}):
-        return self._storage._leaf_to_model(self._leaf_name, self._storage._child[self._leaf_name])
+        return self._storage.to_model(key_filter=key_filter)
 
     def to_xml(self):
         root = _create_root_ele()
-        _leaf_to_xml(self._storage._child[self._leaf_name], root, self._walker, self.rd._ns_map)
+        self._storage._to_xml(self.rd._ns_map, root)
         return root
 
     def delete(self):
         if self._walker.get_dds() == Model.StatementType.leaf_list_:
             raise make_exception(pysros_err_invalid_operation_on_leaflist)
-        self._storage._child[self._leaf_name] = Delete()
+        self._storage._operation = "delete"
 
     def replace(self):
-        self._storage._replace_field = self._leaf_name
-
-    @property
-    def _walker(self):
-        return super()._walker.get_child(self._leaf_name)
+        self._storage._operation = "replace"
 
 class _KeySetter(_ASetter):
     """Interface for keys. Most of this class are stub methods to provide
        setter interface to keys."""
     def __init__(self, storage:"_ListStorage", key_name:str, rd:RequestData):
         super().__init__(storage, rd)
         self._key_name = key_name
@@ -848,33 +864,33 @@
 
         .. Reviewed by TechComms 20210712
         """
         if json:
             value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
         self._check_and_unwrap_keys(value, json=json)
-        return _MoDataSetter(self._storage.get_or_create_entry(self._extract_keys(value)), self.rd)
+        return _MoSetter(self._storage.get_or_create_entry(self._extract_keys(value)), self.rd)
 
     def add_entry(self, value, *, json=False):
         if json:
             value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
         self._check_and_unwrap_keys(value, json=json)
         keys = self._extract_keys(value)
         if self._storage.has_entry(keys):
             raise make_exception(pysros_err_multiple_occurences_of_entry)
-        return _MoDataSetter(self._storage.get_or_create_entry(keys), self.rd)
+        return _MoSetter(self._storage.get_or_create_entry(keys), self.rd)
 
     def entry_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields).
 
         .. Reviewed by PLM 20211018
         """
-        return _MoDataSetter(self._storage.get_or_create_entry(self._convert_keys_to_model(self._extract_keys(value))), self.rd)
+        return _MoSetter(self._storage.get_or_create_entry(self._convert_keys_to_model(self._extract_keys(value))), self.rd)
 
     def entry_exists_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields)
         Returns true if entry exists, otherwise false.
         """
         return self._storage.has_entry(self._convert_keys_to_model(self._extract_keys(value)))
@@ -918,25 +934,25 @@
 
     def replace(self):
         for k, v in self._storage._entries.items():
             v._operation = "replace"
 
     def entry_get_keys(self):
         keys = {key:GetValuePlaceholder() for key in self._walker.get_local_key_names()}
-        setter = _MoDataSetter(self._storage.get_or_create_entry(keys), self.rd)
+        setter = _MoSetter(self._storage.get_or_create_entry(keys), self.rd)
         setter.set({})
         return setter
 
-class _MoDataSetter(_ASetter):
+class _MoSetter(_ASetter):
     """Interface managing specific list entry or container.
 
     .. Reviewed by TechComms 20210712
     """
     class _AChild:
-        def __init__(self, setter:"_MoDataSetter"):
+        def __init__(self, setter:"_MoSetter"):
             self._setter = setter
 
         @property
         def _walker(self):
             return self._setter.rd._Walker(self._setter._storage._model)
 
     class _Keys(_AChild):
@@ -979,28 +995,36 @@
             name = Identifier.from_model_string(name).name
             self.get(name).set(value)
 
         def set_as_json(self, name, value):
             name = Identifier.from_model_string(name).name
             self.get(name)._set_as_json({name: value})
 
+        def get_as_json(self, name):
+            name = Identifier.from_model_string(name).name
+            return self.get(name)
+
         def set_getValue(self, name):
             self.get(name).set_getValue()
 
         def get(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
-            return _LeafSetter(self._setter._storage, name, self._setter.rd)
+            if not self.contains(name):
+                self._setter._storage._child[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd)
+            return _LeafSetter(self._setter._storage._child[name], name, self._setter.rd)
 
         def get_nonexisting(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
             if self.contains(name) and self._walker.get_child_dds(name) != Model.StatementType.leaf_list_:
-                raise make_exception(pysros_err_multiple_occurences_of_node)
-            return _LeafSetter(self._setter._storage, name, self._setter.rd)
+                raise make_exception(pysros_err_multiple_occurences_of_node) #rewrite these two conditions
+            if not self.contains(name):
+                self._setter._storage._child[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd)
+            return _LeafSetter(self._setter._storage._child[name], name, self._setter.rd)
 
         def contains(self, name):
             return name in self._setter._storage._child
 
         def can_contains(self, name):
             return self._walker.has_field_named(name)
 
@@ -1124,31 +1148,47 @@
                     self.child_mos.get(_get_tag_name(e)).entry_xml(e).set_as_xml(e)
 
     def _set_as_json(self, value, is_root = False):
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_json_structure)
 
         children_to_set = set()
+        already_set = set()
+        def check_duplicates(name):
+            if name in children_to_set:
+                raise make_exception(pysros_err_duplicate_found, duplicate=name)
+            children_to_set.add(name)
+
         for k, v in value.items():
             if k.startswith("@"):
+                k = k[1:]
+                self._walker.get_child(k) #module name check?
+                name = Identifier.from_model_string(k).name
+                if not self.fields.can_contains(name):
+                    raise make_exception(pysros_err_unknown_field, field_name=name, path=self._walker._get_path())
+                if k not in value:
+                    raise make_exception(pysros_err_annotation_without_value, child_name=name, path=self._walker._get_path())
+                if not self.fields.contains(name):
+                    self.fields.set_as_json(name, value[k])
+                    check_duplicates(name)
+                    already_set.add(name)
                 continue
             self._walker.get_child(k) #module name check?
             k = Identifier.from_model_string(k).name
+            if k in already_set:
+                continue
             if k in self._walker.get_local_key_names():
                 self.keys.set_as_json(k, v)
             elif self._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
                 self.fields.set_as_json(k, v)
             elif self._walker.get_child_dds(k) in MO_STATEMENT_TYPES:
                 self.child_mos.set_as_json(k, v)
             else:
                 raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
-            name = Identifier.from_model_string(k).name
-            if name in children_to_set:
-                raise make_exception(pysros_err_duplicate_found, duplicate=name)
-            children_to_set.add(name)
+            check_duplicates(k)
 
     def delete(self):
         self._storage._operation = "delete"
 
     def replace(self):
         self._storage._operation = "replace"
 
@@ -1157,9 +1197,7 @@
 
 class GetValuePlaceholder(metaclass=_Singleton):
     pass
 
 class FieldValuePlaceholder(metaclass=_Singleton):
     pass
 
-class Delete(metaclass=_Singleton):
-    pass
```

### Comparing `pysros-23.3.3/pysros/singleton.py` & `pysros-23.7.1/pysros/singleton.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/tokenizer.py` & `pysros-23.7.1/pysros/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pysros-23.3.3/pysros/wrappers.py` & `pysros-23.7.1/pysros/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2021-2023 Nokia
 
 import operator
 
 from abc import ABC, abstractmethod
+from io import StringIO
 
 from .errors import *
 from .singleton import _Empty
 from .yang_type import YangUnion, DECIMAL_LEAF_TYPE, INTEGRAL_LEAF_TYPE
 
 __all__ = ("Action", "Container", "Leaf", "LeafList")
 
-__doc__ = """This module contains wrappers describing the YANG 
+__doc__ = """This module contains wrappers describing the YANG
 structure and metadata obtained from SR OS.
 
 .. Reviewed by PLM 20211201
 .. Reviewed by TechComms 20211202
 """
 
 class Schema:
@@ -108,15 +109,15 @@
                 self._model.StatementType.leaf_,
                 self._model.StatementType.leaf_list_,
                 self._model.StatementType.choice_,
                 self._model.StatementType.anydata_,
                 self._model.StatementType.anyxml_,
             ):
                 return True if self._model.mandatory else False
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attr}'")
+        raise make_exception(pysros_err_attr_object_has_no_attribute, obj=self.__class__.__name__, attribute=attr)
 
     def __eq__(self, other):
         attrs_eq = lambda self, other, attr: getattr(self, attr, None) == getattr(other, attr, None)
         return (
             self.__class__ is other.__class__
             and all(attrs_eq(self, other, attr) for attr in self._attributes)
         )
@@ -160,15 +161,15 @@
     def __getattr__(self, attr):
         if attr == "range":
             if self._yang_type.json_name() in DECIMAL_LEAF_TYPE:
                 return self._yang_type.yang_range
         if attr == "union_members":
             if isinstance(self._yang_type, YangUnion):
                 return tuple(SchemaType(yt) for yt in self._yang_type)
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attr}'")
+        raise make_exception(pysros_err_attr_object_has_no_attribute, obj=self.__class__.__name__, attribute=attr)
 
     def __str__(self):
         return self._yang_type.json_name()
 
     def __repr__(self):
         return self._yang_type.json_name()
 
@@ -206,15 +207,15 @@
         if attr == '_data' and not hasattr(self, '_data'):
             self._check_data_type(value)
             object.__setattr__(self, attr, value)
             return
         elif attr == '_model' and getattr(self, '_model', None) is None:
             object.__setattr__(self, attr, value)
             return
-        raise AttributeError(f"'{self.__class__.__name__}' object attribute '{attr}' is read-only")
+        raise make_exception(pysros_err_attr_is_read_only, obj=self.__class__.__name__, attribute=attr)
 
     def __delattr__(self, attr):
         raise make_exception(pysros_err_attr_cannot_be_deleted, obj=self.__class__.__name__, attribute=attr)
 
     def __eq__(self, other):
         return self.__class__ is other.__class__ and self._data == other._data
 
@@ -402,8 +403,11 @@
     '__rtruediv__',
     '__rxor__',
     '__sub__',
     '__truediv__',
     '__trunc__',
     '__xor__',
 )
-del forward_methods
+del forward_methods
+
+_sentinel = object()
+
```

### Comparing `pysros-23.3.3/pysros/yang_type.py` & `pysros-23.7.1/pysros/yang_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 Nokia
 
 import base64
 
 from abc import ABC, abstractmethod
 from collections import OrderedDict, namedtuple
 from enum import Enum
-from typing import Any, Dict, List, Mapping, Optional, Set, Type, Tuple, Union, NamedTuple, Iterable
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, Type, Tuple, Union, NamedTuple, Iterable
 
 from lxml.etree import SubElement
 
 from .errors import *
 from .identifier import Identifier, NoModule
 from .model_path import ModelPath
 from .singleton import Empty
@@ -337,14 +337,18 @@
     def __hash__(self):
         return hash(tuple(self))
 
     def add_enum(self, name: str):
         val = 1+max(self.values()) if self else 0
         self[name] = val
 
+    def add_enums(self, *names: Iterable[str]):
+        for name in names:
+            self.add_enum(name)
+
     def set_last_enum_value(self, val: int):
         assert self
         last_used_key = next(reversed(self))
         self[last_used_key] = val
 
     def to_value(self, val: str) -> Any:
         return str(val)
```

### Comparing `pysros-23.3.3/pysros.egg-info/PKG-INFO` & `pysros-23.7.1/pysros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.3.3
+Version: 23.7.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Python 3 for Nokia Service Router Operating System (pySROS) #
 
 ## Overview ##
 
@@ -38,15 +38,15 @@
 In order to use the pySROS library the following pre-requisites must be met:
 
 - One or more SR OS node
     - Running in model-driven mode
     - Running SR OS 21.7.R1 or greater (to execute applications on the SR OS device)
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
-- A Python 3 interpreter of version 3.6 or newer when using the pySROS library to
+- A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
 Copyright 2021-2023 Nokia.
 
 The license is located [here](LICENSE.md).
```

### Comparing `pysros-23.3.3/setup.py` & `pysros-23.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='23.3.3',
+    version='23.7.1',
     packages=['pysros'],
     url='https://www.nokia.com',
     license='Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
@@ -25,12 +25,12 @@
         "Topic :: Internet",
         "Development Status :: 5 - Production/Stable",
     ],
     install_requires=[
         "ncclient~=0.6.12",
         "lxml~=4.9.2",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

