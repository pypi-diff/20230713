# Comparing `tmp/threemystic_cloud_client-0.1.23.tar.gz` & `tmp/threemystic_cloud_client-0.1.24.tar.gz`

## Comparing `threemystic_cloud_client-0.1.23.tar` & `threemystic_cloud_client-0.1.24.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    22417 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/hatch.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/pyproject.toml
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12138 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    22534 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    16112 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.24/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,23 @@
         {
           "--account": {
             "default": None, 
             "type": str,
             "dest": "token_account",
             "help": "The AWS Account ID to generate access token information for",
             "action": 'store'
-          }
-        },
-        {
+          },
           "--profile": {
             "default": None, 
             "type": str,
             "dest": "token_profile",
             "help": "The 3Mystic AWS Profile to use. If not provided the default will be used",
             "action": 'store'
           }
-        }
+        },
       ])
     )
 
 
     processed_info = process_options.process_opts(
       parser = self._arg_parser
     )
```

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,16 @@
       
     self._set_authenticating_session(is_authenticating_session= True)
 
     try:
       self.authenticate_session()
     finally:
       self._set_authenticating_session(is_authenticating_session= False)
+    
+    return self.ensure_session()
   
   def is_authenticating_session(self, *args, **kwargs):
     if(hasattr(self, "_is_authenticating_session")):
       return self._is_authenticating_session
     
     return False
   
@@ -405,15 +407,15 @@
 
   def __get_boto_session(self, role = None, region = None, profile = None, **kwargs):
     if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile):
       return boto_session(profile_name= profile) if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region) else boto_session(profile_name= profile, region_name= region)
 
     return botocore_session.get_session()
 
-  def get_boto_session(self, account=None, role = None, region = None, profile = None):
+  def get_boto_session(self, account=None, role = None, region = None, profile = None, *args, **kwargs):
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= role):
       role = self.get_default_rolename()
     
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= region):
       region = self.get_default_region()
 
@@ -434,15 +436,15 @@
       method="sts-assume-role",
     )
 
     session._credentials = credentials 
     session.set_config_variable("region", region)
       
     self._get_created_boto_sessions()[cache_key] = boto_session(botocore_session= session)
-    return self._get_created_boto_sessions[cache_key]
+    return self.get_boto_session(account=account, role = role, region = region, profile = profile, *args, **kwargs)
   
   def _get_accounts(self, refresh = False, include_suspended = False):
     
     if hasattr(self, "_account_list") and not refresh:
       return_list = "active" if not include_suspended else "all"
       if self._account_list is not None and len(self._account_list) > 0:
         return self._account_list[return_list]
```

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,24 +164,24 @@
           type= QueryColumnType.DIMENSION,
           name= "SubscriptionId"
         )
       ]
       )
     )
   
-  def serialize_azresource(self, resource, *args, **kwargs):
+  def serialize_resource(self, resource, *args, **kwargs):
     if resource is None:
       return None
     
     if self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
       return resource
 
     return resource.serialize(keep_readonly= True)
     
-  def deserialize_azresource(self, resource, aztype):
+  def deserialize_resource(self, resource, aztype):
     if resource is None:
       return None
 
     return aztype.deserialize(resource)
 
   def get_resource_name_from_resource(self, resource, *args, **kwargs):
     if resource is None:
@@ -249,22 +249,33 @@
         string_value= self.get_resource_id_from_resource(resource= resource), 
         case= "lower"),
       separator="/",
       regex_split= False
     )
     return resource_id_split[resource_id_split.index("resourcegroups") + 1]
   
-  def get_azresource_location(self, resource, *args, **kwargs):
+  def get_resource_name(self, resource, *args, **kwargs):
     if resource is None:
       return None
 
     if not self.get_common().helper_type().general().is_type(obj= resource, type_check= str):
       if self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
-          return self.get_azresource_location(resource= resource.get("extra_region") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value=resource.get("extra_region")) else resource.get("location"))
-      return self.get_azresource_location(resource= getattr(resource, "location"))
+          return self.get_resource_name(resource= resource.get("extra_name") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value=resource.get("extra_name")) else resource.get("name"))
+      return self.get_resource_name(resource= getattr(resource, "name"))
+
+    return resource
+  
+  def get_resource_location(self, resource, *args, **kwargs):
+    if resource is None:
+      return None
+
+    if not self.get_common().helper_type().general().is_type(obj= resource, type_check= str):
+      if self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+          return self.get_resource_location(resource= resource.get("extra_region") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value=resource.get("extra_region")) else resource.get("location"))
+      return self.get_resource_location(resource= getattr(resource, "location"))
 
     return resource
   
   def get_tenant_prefix(self, *args, **kwargs):
     return "/tenants/"
 
   def get_account_prefix(self, *args, **kwargs):
```

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -323,8 +323,38 @@
     if self.check_request_error_login(exception= error_message):
       return self._az_cli("az login", on_login_function = on_login_function)
     
     return {
       "exit_code": exit_code,
       "result": self.get_common().helper_json().loads(data= stdout_buffer.getvalue()) if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= stdout_buffer.getvalue()) else None,
       "error": error_message
-    }
+    }
+  
+  def get_resource_tags_as_dictionary(self, resource, *args, **kwargs):
+    if resource is None:
+      return None
+
+    tags = None
+    if not self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if hasattr(resource, "tags"):
+        tags = resource.tags
+    elif self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      tags = resource.get("tags")
+
+    if tags is None:
+      tags = {}
+      
+    if "name" not in tags:
+      name_options = ["display_name", "displayname", "name"]
+
+      if not self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+        for att in dir(resource):
+          if self.get_common().helper_type().string().set_case(string_value= att, case= "lower") in name_options:
+            tags["name"] = getattr(resource, att).strip()
+            return tags
+
+      for att in resource.keys():
+        if self.get_common().helper_type().string().set_case(string_value= att, case= "lower") in name_options:
+          tags["name"] = resource.get(att).strip()
+          return tags
+    return tags
+
```

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.24/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/.gitignore` & `threemystic_cloud_client-0.1.24/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/LICENSE` & `threemystic_cloud_client-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/README.md` & `threemystic_cloud_client-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/hatch.toml` & `threemystic_cloud_client-0.1.24/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.23/pyproject.toml` & `threemystic_cloud_client-0.1.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.8",
+  "threemystic-common >= 0.1.10",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "pyopenssl >= 22.1.0",
   "PyJWT >= 2.7.0",
   "cryptography >= 41.0.1",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
```

### Comparing `threemystic_cloud_client-0.1.23/PKG-INFO` & `threemystic_cloud_client-0.1.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.23
+Version: 0.1.24
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: polling2>=0.5.0
 Requires-Dist: pyjwt>=2.7.0
 Requires-Dist: pyopenssl>=22.1.0
-Requires-Dist: threemystic-common>=0.1.8
+Requires-Dist: threemystic-common>=0.1.10
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

