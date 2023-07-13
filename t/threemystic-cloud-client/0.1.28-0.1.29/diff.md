# Comparing `tmp/threemystic_cloud_client-0.1.28.tar.gz` & `tmp/threemystic_cloud_client-0.1.29.tar.gz`

## Comparing `threemystic_cloud_client-0.1.28.tar` & `threemystic_cloud_client-0.1.29.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/pyproject.toml
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.28/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.29/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     self._processed_arg_info = processed_info.get("processed_data")
   
     
   def step(self, *args, **kwargs):
     if not super().step( *args, **kwargs):
       return
     
-    if (self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._processed_arg_info.get("client_help"))):
+    if (self.get_common().helper_type().bool().is_true(check_value= self._processed_arg_info.get("client_help"))):
       self._arg_parser.print_help()
       return
     
     if (self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._processed_arg_info.get("token_account"))):
       self._arg_parser.print_help()
       return
```

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.29/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/.gitignore` & `threemystic_cloud_client-0.1.29/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/LICENSE` & `threemystic_cloud_client-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/README.md` & `threemystic_cloud_client-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/hatch.toml` & `threemystic_cloud_client-0.1.29/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/pyproject.toml` & `threemystic_cloud_client-0.1.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.28/PKG-INFO` & `threemystic_cloud_client-0.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.28
+Version: 0.1.29
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

