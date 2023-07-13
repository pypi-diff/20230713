# Comparing `tmp/pulumi_ns1-3.1.0a1687672414.tar.gz` & `tmp/pulumi_ns1-3.1.0a1689276268.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.1.0a1687672414.tar", last modified: Sun Jun 25 06:06:21 2023, max compression
+gzip compressed data, was "pulumi_ns1-3.1.0a1689276268.tar", last modified: Thu Jul 13 19:28:31 2023, max compression
```

## Comparing `pulumi_ns1-3.1.0a1687672414.tar` & `pulumi_ns1-3.1.0a1689276268.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:06:21.346459 pulumi_ns1-3.1.0a1687672414/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-25 06:06:21.346459 pulumi_ns1-3.1.0a1687672414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:06:21.342458 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    86906 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:06:21.342458 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    39137 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    81290 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    88846 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:06:21.342458 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:06:21.346459 pulumi_ns1-3.1.0a1687672414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-25 06:06:21.000000 pulumi_ns1-3.1.0a1687672414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:28:31.851206 pulumi_ns1-3.1.0a1689276268/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-13 19:28:31.851206 pulumi_ns1-3.1.0a1689276268/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:28:31.847206 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87464 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:28:31.851206 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39137 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34245 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81848 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89404 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:28:31.851206 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:28:31.851206 pulumi_ns1-3.1.0a1689276268/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 19:28:31.000000 pulumi_ns1-3.1.0a1689276268/setup.py
```

### Comparing `pulumi_ns1-3.1.0a1687672414/PKG-INFO` & `pulumi_ns1-3.1.0a1689276268/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.1.0a1687672414
+Version: 3.1.0a1689276268
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi ns1
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_ns1-3.1.0a1687672414/README.md` & `pulumi_ns1-3.1.0a1689276268/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/__init__.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/api_key.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -743,14 +746,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -1531,14 +1537,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> pulumi.Output[Optional[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @property
     @pulumi.getter(name="accountManageTeams")
     def account_manage_teams(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the apikey can modify other teams in the account.
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/application.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/data_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/data_source.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_dns_sec.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,18 +102,18 @@
     """
     __args__ = dict()
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getDNSSec:getDNSSec', __args__, opts=opts, typ=GetDNSSecResult).value
 
     return AwaitableGetDNSSecResult(
-        delegations=__ret__.delegations,
-        id=__ret__.id,
-        keys=__ret__.keys,
-        zone=__ret__.zone)
+        delegations=pulumi.get(__ret__, 'delegations'),
+        id=pulumi.get(__ret__, 'id'),
+        keys=pulumi.get(__ret__, 'keys'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_dns_sec)
 def get_dns_sec_output(zone: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSSecResult]:
     """
     Provides DNSSEC details about a NS1 Zone.
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_networks.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,9 +73,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getNetworks:getNetworks', __args__, opts=opts, typ=GetNetworksResult).value
 
     return AwaitableGetNetworksResult(
-        id=__ret__.id,
-        networks=__ret__.networks)
+        id=pulumi.get(__ret__, 'id'),
+        networks=pulumi.get(__ret__, 'networks'))
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_record.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -203,27 +203,27 @@
     __args__['domain'] = domain
     __args__['type'] = type
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getRecord:getRecord', __args__, opts=opts, typ=GetRecordResult).value
 
     return AwaitableGetRecordResult(
-        answers=__ret__.answers,
-        domain=__ret__.domain,
-        filters=__ret__.filters,
-        id=__ret__.id,
-        link=__ret__.link,
-        meta=__ret__.meta,
-        override_ttl=__ret__.override_ttl,
-        regions=__ret__.regions,
-        short_answers=__ret__.short_answers,
-        ttl=__ret__.ttl,
-        type=__ret__.type,
-        use_client_subnet=__ret__.use_client_subnet,
-        zone=__ret__.zone)
+        answers=pulumi.get(__ret__, 'answers'),
+        domain=pulumi.get(__ret__, 'domain'),
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        link=pulumi.get(__ret__, 'link'),
+        meta=pulumi.get(__ret__, 'meta'),
+        override_ttl=pulumi.get(__ret__, 'override_ttl'),
+        regions=pulumi.get(__ret__, 'regions'),
+        short_answers=pulumi.get(__ret__, 'short_answers'),
+        ttl=pulumi.get(__ret__, 'ttl'),
+        type=pulumi.get(__ret__, 'type'),
+        use_client_subnet=pulumi.get(__ret__, 'use_client_subnet'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_record)
 def get_record_output(domain: Optional[pulumi.Input[str]] = None,
                       type: Optional[pulumi.Input[str]] = None,
                       zone: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRecordResult]:
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/get_zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -260,31 +260,31 @@
     __args__['additionalPrimaries'] = additional_primaries
     __args__['primaryPort'] = primary_port
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getZone:getZone', __args__, opts=opts, typ=GetZoneResult).value
 
     return AwaitableGetZoneResult(
-        additional_ports=__ret__.additional_ports,
-        additional_primaries=__ret__.additional_primaries,
-        dns_servers=__ret__.dns_servers,
-        dnssec=__ret__.dnssec,
-        expiry=__ret__.expiry,
-        hostmaster=__ret__.hostmaster,
-        id=__ret__.id,
-        link=__ret__.link,
-        networks=__ret__.networks,
-        nx_ttl=__ret__.nx_ttl,
-        primary=__ret__.primary,
-        primary_port=__ret__.primary_port,
-        refresh=__ret__.refresh,
-        retry=__ret__.retry,
-        secondaries=__ret__.secondaries,
-        ttl=__ret__.ttl,
-        zone=__ret__.zone)
+        additional_ports=pulumi.get(__ret__, 'additional_ports'),
+        additional_primaries=pulumi.get(__ret__, 'additional_primaries'),
+        dns_servers=pulumi.get(__ret__, 'dns_servers'),
+        dnssec=pulumi.get(__ret__, 'dnssec'),
+        expiry=pulumi.get(__ret__, 'expiry'),
+        hostmaster=pulumi.get(__ret__, 'hostmaster'),
+        id=pulumi.get(__ret__, 'id'),
+        link=pulumi.get(__ret__, 'link'),
+        networks=pulumi.get(__ret__, 'networks'),
+        nx_ttl=pulumi.get(__ret__, 'nx_ttl'),
+        primary=pulumi.get(__ret__, 'primary'),
+        primary_port=pulumi.get(__ret__, 'primary_port'),
+        refresh=pulumi.get(__ret__, 'refresh'),
+        retry=pulumi.get(__ret__, 'retry'),
+        secondaries=pulumi.get(__ret__, 'secondaries'),
+        ttl=pulumi.get(__ret__, 'ttl'),
+        zone=pulumi.get(__ret__, 'zone'))
 
 
 @_utilities.lift_output_func(get_zone)
 def get_zone_output(additional_ports: Optional[pulumi.Input[Optional[Sequence[int]]]] = None,
                     additional_primaries: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                     primary_port: Optional[pulumi.Input[Optional[int]]] = None,
                     zone: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/monitoring_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/notify_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/outputs.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/provider.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/record.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,14 +185,17 @@
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RecordRegionArgs']]]]):
         pulumi.set(self, "regions", value)
 
     @property
     @pulumi.getter(name="shortAnswers")
     def short_answers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""", DeprecationWarning)
+        pulumi.log.warn("""short_answers is deprecated: short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""")
+
         return pulumi.get(self, "short_answers")
 
     @short_answers.setter
     def short_answers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "short_answers", value)
 
     @property
@@ -373,14 +376,17 @@
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['RecordRegionArgs']]]]):
         pulumi.set(self, "regions", value)
 
     @property
     @pulumi.getter(name="shortAnswers")
     def short_answers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        warnings.warn("""short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""", DeprecationWarning)
+        pulumi.log.warn("""short_answers is deprecated: short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""")
+
         return pulumi.get(self, "short_answers")
 
     @short_answers.setter
     def short_answers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "short_answers", value)
 
     @property
@@ -702,14 +708,17 @@
         documented below. Please note the ordering requirement!
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="shortAnswers")
     def short_answers(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        warnings.warn("""short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""", DeprecationWarning)
+        pulumi.log.warn("""short_answers is deprecated: short_answers will be deprecated in a future release. It is suggested to migrate to a regular \"answers\" block.""")
+
         return pulumi.get(self, "short_answers")
 
     @property
     @pulumi.getter
     def ttl(self) -> pulumi.Output[int]:
         """
         The records' time to live (in seconds).
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/subnet.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/team.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -699,14 +702,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -1443,14 +1449,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> pulumi.Output[Optional[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @property
     @pulumi.getter(name="accountManageTeams")
     def account_manage_teams(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the team can modify other teams in the account.
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/tsigkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/user.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -779,14 +782,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @account_manage_plan.setter
     def account_manage_plan(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "account_manage_plan", value)
 
     @property
@@ -1598,14 +1604,17 @@
 
     @property
     @pulumi.getter(name="accountManagePlan")
     def account_manage_plan(self) -> pulumi.Output[Optional[bool]]:
         """
         No longer in use.
         """
+        warnings.warn("""obsolete, should no longer be used""", DeprecationWarning)
+        pulumi.log.warn("""account_manage_plan is deprecated: obsolete, should no longer be used""")
+
         return pulumi.get(self, "account_manage_plan")
 
     @property
     @pulumi.getter(name="accountManageTeams")
     def account_manage_teams(self) -> pulumi.Output[Optional[bool]]:
         """
         Whether the user can modify other teams in the account.
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1/zone.py` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-ns1
-Version: 3.1.0a1687672414
+Version: 3.1.0a1689276268
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi ns1
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_ns1-3.1.0a1687672414/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.1.0a1689276268/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1687672414/setup.py` & `pulumi_ns1-3.1.0a1689276268/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.1.0a1687672414"
-PLUGIN_VERSION = "3.1.0-alpha.1687672414+21448ce4"
+VERSION = "3.1.0a1689276268"
+PLUGIN_VERSION = "3.1.0-alpha.1689276268+129a169d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'ns1', PLUGIN_VERSION])
         except OSError as error:
```

