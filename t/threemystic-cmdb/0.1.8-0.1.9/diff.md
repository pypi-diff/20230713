# Comparing `tmp/threemystic_cmdb-0.1.8.tar.gz` & `tmp/threemystic_cmdb-0.1.9.tar.gz`

## Comparing `threemystic_cmdb-0.1.8.tar` & `threemystic_cmdb-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18763 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/README.md
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     6484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/README.md
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.9/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,22 +186,26 @@
     print(f"Group NOT Updated")
     print()
     print("-----------------------------")
 
   
 
   
-  def get_drive_item_index(self, drive_item_ids, drive_item_id_options, position, cloud_share):
+  def get_drive_item_index(self, drive_item_ids, existing_drive_item_ids, drive_item_id_options, position, cloud_share):
     try:
       index = 0
       drive_id = None
       drive_item_ids_position = position + 1
-      if len(drive_item_ids) > drive_item_ids_position:
-        if self.get_common().helper_type().general().is_type(obj= drive_item_ids[drive_item_ids_position], type_check= dict):
-          drive_id = drive_item_ids[drive_item_ids_position]
+      if drive_item_ids[-1]["id"] != existing_drive_item_ids[position]["id"]:
+        return None
+      
+      
+      if len(existing_drive_item_ids) > drive_item_ids_position:
+        if self.get_common().helper_type().general().is_type(obj= existing_drive_item_ids[drive_item_ids_position], type_check= dict):
+          drive_id = existing_drive_item_ids[drive_item_ids_position]
       
       if drive_id is None:
         return None
       
       if drive_id.get("id") is None:
         return None
       
@@ -271,33 +275,34 @@
   def get_drive_item_location_options(self, ms_graph,ms_graph_resource, ms_graph_resource_id, drive_item_id, cloud_share):
     location_options_base = [
       {
       "id": "refresh",
       "display": "Refresh List"
     }
     ]
-    remove_entry = {
-      "id": "remove_entry",
-      "display": "Remove Entry (does not remove it from ms365)"
+    parent_folder = {
+      "id": "parent_folder",
+      "display": "Parent Folder"
     }
       
     new_folder = {
       "id": "new_folder",
       "display": "New Folder"
     }
       
     select = {
       "id": "select_folder",
       "display": "Select"
     }
 
     if self.get_cloud_share_config_value(config_key= cloud_share).get('group') == "me" or drive_item_id != "root":
       location_options_base.append(select)
+      location_options_base.append(parent_folder)
       location_options_base.append(new_folder)
-      location_options_base.append(remove_entry)
+      
     
 
     base_path = f"{drive_item_id}" if self.get_cloud_share_config_value(config_key= cloud_share).get('group') == "me" else f"items/{drive_item_id}"
     
     local_drive_options = ms_graph.send_request(
       url = ms_graph.generate_graph_url(resource= ms_graph_resource, resource_id= ms_graph_resource_id, base_path= f"drive/{base_path}/children")
     )
@@ -307,36 +312,40 @@
     ]
   
   def _step_ms365_tenant_path(self, cloud_share, data_client, ms_graph, *args, **kwargs):
 
     print("-----------------------------")
     print()
     print("What folder will the CMDB be stored in")
-    print("If you have moved the folder where teh cmdb is stored you could break the hierarchy used to validate the path, but the upload should be fine.")
+    print("If you have moved the folder where the cmdb is stored you could break the hierarchy used to validate the path, but the upload should be fine.")
     print("This is because the upload does not look at the pat, IE. /3mystic/data/cmdb, it looks at the last drive ID and uses that which shouldn't change as you move folders.")
     print()
     print("-----------------------------")
     
     
     index = 1
     print("loading folders")
 
     
-    drive_item_ids = self.get_cloud_share_config_value(config_key= cloud_share).get('drive_id')
+    existing_drive_item_ids = self.get_cloud_share_config_value(config_key= cloud_share).get('drive_id')
+    drive_item_ids = [
+      {"id": "root", "display": "root"}
+    ]
+    
     if not self.get_common().helper_type().general().is_type(obj= drive_item_ids, type_check= list):
-      drive_item_ids = [
+      existing_drive_item_ids = [
         {"id": "root", "display": "root"}
       ]
     try:
-      if len(drive_item_ids) < 1:
-        drive_item_ids.append({"id": "root", "display": "root"})
+      if len(existing_drive_item_ids) < 1:
+        existing_drive_item_ids.append({"id": "root", "display": "root"})
       if not self.get_common().helper_type().general().is_type(obj= drive_item_ids[0], type_check= dict):
-        drive_item_ids[0] = ({"id": "root", "display": "root"})
+        existing_drive_item_ids[0] = ({"id": "root", "display": "root"})
     except:
-      drive_item_ids = [
+      existing_drive_item_ids = [
         {"id": "root", "display": "root"}
       ]
 
     drive_item_position = 0
     drive_item_id_options = []
     drive_id_selected = False
     main_graph_resource = "me" if self.get_cloud_share_config_value(config_key= cloud_share).get('group') == "me" else f"groups"
@@ -354,22 +363,22 @@
           time.sleep(3)
         return
 
       print("-----------------------------")
       print(f"Folders in {drive_item_ids[drive_item_position].get('display')}")
       print("-----------------------------")
       
-      drive_item_index = self.get_drive_item_index(drive_item_ids= drive_item_ids, drive_item_id_options= drive_item_id_options, position= drive_item_position, cloud_share= cloud_share,)
-
+      drive_item_index = self.get_drive_item_index(drive_item_ids= drive_item_ids, existing_drive_item_ids= existing_drive_item_ids, drive_item_id_options= drive_item_id_options, position= drive_item_position, cloud_share= cloud_share,)
+      
       index = 0
       for option in drive_item_id_options[drive_item_position]:
         print(f'{index}: {option.get("display")}')
-        if drive_item_index is None and option.get("id") == "select_folder":
+        if drive_item_position > 0 and drive_item_index is None and option.get("id") == "select_folder":
           drive_item_index = index
-        index += 1   
+        index += 1 
 
       response = self.get_common().generate_data().generate(
         generate_data_config = {
           "drive_id": {
             "validation": lambda item: not self.get_common().helper_type().string().is_null_or_whitespace(string_value= item) and self.get_common().helper_type().general().is_integer(item) and self.get_common().helper_type().int().get(item) >= 0 and self.get_common().helper_type().int().get(item) <= (len(drive_item_id_options[drive_item_position]) - 1),
             "messages":{
               "validation": f"Valid options are: 0 - {len(drive_item_id_options[drive_item_position]) - 1}",
@@ -411,29 +420,29 @@
         if new_folder_info is None:
           continue
 
         drive_item_ids.append(new_folder_info)
         drive_item_position = drive_item_position + 1
         continue
       
-      if drive_id_option["id"] == "remove_entry":
+      if drive_id_option["id"] == "parent_folder":
         if len(drive_item_id_options) > 1:
           drive_item_ids.pop()
           drive_item_id_options.pop()
           drive_item_id_options.pop()
           drive_item_position = drive_item_position - 1
           continue
         print("already at the root")
         continue
       
+      
       drive_item_ids.append(drive_id_option)
       drive_item_position = drive_item_position + 1
       
       
-      
     self.get_cloud_share_config_value(
       config_key= cloud_share
     )["drive_id"] = drive_item_ids
     self._save_config_cloud_share()
     
     print("-----------------------------")
     print()
```

### Comparing `threemystic_cmdb-0.1.8/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.9/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/.gitignore` & `threemystic_cmdb-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/LICENSE` & `threemystic_cmdb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/README.md` & `threemystic_cmdb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.8/pyproject.toml` & `threemystic_cmdb-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.5",
-  "threemystic-cloud-data-client >= 0.1.8",
+  "threemystic-common >= 0.1.8",
+  "threemystic-cloud-data-client >= 0.1.9",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
   "lxml >= 4.9.2",
   "msgraph-sdk >= 1.0.0a12",  
   "polling2 >= 0.5.0",
```

### Comparing `threemystic_cmdb-0.1.8/PKG-INFO` & `threemystic_cmdb-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.8
+Version: 0.1.9
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,16 @@
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-cloud-data-client>=0.1.8
-Requires-Dist: threemystic-common>=0.1.5
+Requires-Dist: threemystic-cloud-data-client>=0.1.9
+Requires-Dist: threemystic-common>=0.1.8
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
 Currently supports AWS/Azure
```

