# Comparing `tmp/rudderclient-1.9.0.tar.gz` & `tmp/rudderclient-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.9.0.tar", last modified: Thu Jun  1 14:20:02 2023, max compression
+gzip compressed data, was "rudderclient-1.9.1.tar", last modified: Wed Jun  7 09:37:21 2023, max compression
```

## Comparing `rudderclient-1.9.0.tar` & `rudderclient-1.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.818587 rudderclient-1.9.0/
--rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-06-01 14:19:28.000000 rudderclient-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 14:20:02.818587 rudderclient-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-06-01 14:19:28.000000 rudderclient-1.9.0/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-06-01 14:19:52.000000 rudderclient-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-06-01 14:20:02.818587 rudderclient-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.809586 rudderclient-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.812586 rudderclient-1.9.0/src/rudderclient/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.814586 rudderclient-1.9.0/src/rudderclient/aws/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/aws/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5006 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/aws/requests.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.816587 rudderclient-1.9.0/src/rudderclient/gcp/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/gcp/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2649 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/gcp/auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1969 2023-06-01 14:19:50.000000 rudderclient-1.9.0/src/rudderclient/gcp/http_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      869 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6353 2023-06-01 14:19:50.000000 rudderclient-1.9.0/src/rudderclient/gcp/workspace.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.817587 rudderclient-1.9.0/src/rudderclient/request/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/request/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/request/exceptions.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1260 2023-06-01 14:19:28.000000 rudderclient-1.9.0/src/rudderclient/request/helpers.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.817587 rudderclient-1.9.0/src/rudderclient/tools/
--rw-r--r--   0 runner    (1001) runner    (1001)     3816 2023-06-01 14:19:50.000000 rudderclient-1.9.0/src/rudderclient/tools/send_email.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-01 14:20:02.813586 rudderclient-1.9.0/src/rudderclient.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-01 14:20:02.000000 rudderclient-1.9.0/src/rudderclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      640 2023-06-01 14:20:02.000000 rudderclient-1.9.0/src/rudderclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-06-01 14:20:02.000000 rudderclient-1.9.0/src/rudderclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-06-01 14:20:02.000000 rudderclient-1.9.0/src/rudderclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-06-01 14:20:02.000000 rudderclient-1.9.0/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.765364 rudderclient-1.9.1/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-06-07 09:36:39.000000 rudderclient-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-07 09:37:21.764364 rudderclient-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-06-07 09:36:39.000000 rudderclient-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     1030 2023-06-07 09:37:12.000000 rudderclient-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-06-07 09:37:21.765364 rudderclient-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.759364 rudderclient-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.760364 rudderclient-1.9.1/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.762364 rudderclient-1.9.1/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5045 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.763364 rudderclient-1.9.1/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2649 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1969 2023-06-07 09:37:08.000000 rudderclient-1.9.1/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      871 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6414 2023-06-07 09:37:09.000000 rudderclient-1.9.1/src/rudderclient/gcp/workspace.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.764364 rudderclient-1.9.1/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/request/exceptions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1260 2023-06-07 09:36:39.000000 rudderclient-1.9.1/src/rudderclient/request/helpers.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.764364 rudderclient-1.9.1/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)     3816 2023-06-07 09:37:09.000000 rudderclient-1.9.1/src/rudderclient/tools/send_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-06-07 09:37:21.762364 rudderclient-1.9.1/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-06-07 09:37:21.000000 rudderclient-1.9.1/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      640 2023-06-07 09:37:21.000000 rudderclient-1.9.1/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-06-07 09:37:21.000000 rudderclient-1.9.1/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-06-07 09:37:21.000000 rudderclient-1.9.1/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       13 2023-06-07 09:37:21.000000 rudderclient-1.9.1/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.9.0/LICENSE` & `rudderclient-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.9.0/PKG-INFO` & `rudderclient-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.9.0
+Version: 1.9.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.9.0/pyproject.toml` & `rudderclient-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.9.0"
+version = "1.9.1"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3.10",]
 keywords = [ "rudder", "client", "helper",]
 dependencies = [ "google-cloud-secret-manager",]
 requires-python = ">=3.10"
 [[project.authors]]
```

### Comparing `rudderclient-1.9.0/src/rudderclient/aws/requests.py` & `rudderclient-1.9.1/src/rudderclient/aws/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         secret_access_key: The secret key to use when creating the client.
     """
     # Create IAM client
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
 
-    deleteResponse = client.delete_user(**operation_parameters)
+    delete_response = client.delete_user(**operation_parameters)
 
-    return deleteResponse
+    return delete_response
 
 
 def get_identitystore_id(region, acces_key_id, secret_access_key):
     """
     Returns the ID of your organization Identity Store in a unique region.
 
     Parameters:
@@ -57,44 +57,44 @@
         access_key_id: The access key to use when creating the client.
         secret_access_key: The secret key to use when creating the client.
     """
     client = get_boto3_client(
         "sso-admin", region, acces_key_id, secret_access_key
     )
     identitystore = client.list_instances()
-    id = identitystore["Instances"][0]["IdentityStoreId"]
-    return id
+    identitystore_id = identitystore["Instances"][0]["IdentityStoreId"]
+    return identitystore_id
 
 
-def describe_user(userId, region, acces_key_id, secret_access_key):
+def describe_user(user_id, region, acces_key_id, secret_access_key):
     """
     Returns information of a user.
 
     Parameters:
     ----------
-        userId: The ID of the user.
+        user_id: The ID of the user.
         region: The name of the region associated with the identityStore.
         access_key_id: The access key to use when creating the client.
         secret_access_key: The secret key to use when creating the client.
 
     """
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
     identitystore = get_identitystore_id(
         region, acces_key_id, secret_access_key
     )
     response = client.describe_user(
-        IdentityStoreId=identitystore, UserId=userId
+        IdentityStoreId=identitystore, UserId=user_id
     )
     return response
 
 
 def create_user(
-    userEmail, firstName, surnames, region, acces_key_id, secret_access_key
+    user_email, first_name, surnames, region, acces_key_id, secret_access_key
 ):
     """
     Creates a user in an identity Store.
 
     Parameters:
     ----------
         userEmail: the work email of the user.
@@ -106,22 +106,22 @@
     """
     client = get_boto3_client(
         "identitystore", region, acces_key_id, secret_access_key
     )
     identitystore = get_identitystore_id(
         region, acces_key_id, secret_access_key
     )
-    display_name = f"{firstName} {surnames}"
+    display_name = f"{first_name} {surnames}"
 
     response = client.create_user(
         IdentityStoreId=identitystore,
-        UserName=userEmail,
+        UserName=user_email,
         DisplayName=display_name,
-        Name={"FamilyName": firstName, "GivenName": surnames},
-        Emails=[{"Value": userEmail, "Type": "Work", "Primary": True}],
+        Name={"FamilyName": first_name, "GivenName": surnames},
+        Emails=[{"Value": user_email, "Type": "Work", "Primary": True}],
     )
     return response
 
 
 def pagination(
     action, operation_parameters, region, acces_key_id, secret_access_key
 ):
```

### Comparing `rudderclient-1.9.0/src/rudderclient/gcp/auth.py` & `rudderclient-1.9.1/src/rudderclient/gcp/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     client = secretmanager.SecretManagerServiceClient()
     secret = client.access_secret_version(request={"name": secret_id})
     value = secret.payload.data.decode("UTF-8")
     return value
 
 
-def get_OIDC_token_iap_request(client_id, **kwargs):
+def get_oidc_token_iap_request(client_id, **kwargs):
     """
     Returns a token for doing an HTTP request to an application protected by Identity-Aware Proxy.
 
     Parameters:
     ----------
         client_id: The client ID used by Identity-Aware Proxy
         **kwargs: Any of the parameters defined for the request function:
```

### Comparing `rudderclient-1.9.0/src/rudderclient/gcp/http_requests.py` & `rudderclient-1.9.1/src/rudderclient/gcp/http_requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.9.0/src/rudderclient/gcp/pubsub.py` & `rudderclient-1.9.1/src/rudderclient/gcp/pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """
 
 
 from google.cloud import pubsub_v1
 
 
-def write_message(project_id, topic_id, message_str, status, joinerId):
+def write_message(project_id, topic_id, message_str, status, joiner_id):
     """
     Publish a message in Pub Sub.
 
     Parameters:
     ----------
         project_id: The ID of the gcp project where you want to publish a message.
         topic_id: The topic name where you want to publish the message.
@@ -21,13 +21,13 @@
     publisher = pubsub_v1.PublisherClient()
     topic_path = publisher.topic_path(project_id, topic_id)
 
     # Data must be a bytestring
     message = message_str.encode("utf-8")
 
     future = publisher.publish(
-        topic_path, message, status=str(status), joinerId=str(joinerId)
+        topic_path, message, status=str(status), joinerId=str(joiner_id)
     )
 
     result = future.result()
 
     return result
```

### Comparing `rudderclient-1.9.0/src/rudderclient/gcp/workspace.py` & `rudderclient-1.9.1/src/rudderclient/gcp/workspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 """
 
 from googleapiclient.discovery import build
 from google.oauth2 import service_account
 
 
-def create_service(serviceName, version, credentials):
+def create_service(service_name, version, credentials):
     """
     Create the necessary service to interact with a specific Google Workspace service in a specific version of its API.
 
     Parameters:
     ----------
         serviceName: Name of the service.
         version: Version of the service.
         credentials: oauth2client.Credentials or google.auth.credentials.Credentials, credentials to be used for
             authentication. You can get them with 'get_workspace_impersonate_credentials_sa' method.
 
     """
-    service = build(serviceName, version, credentials=credentials)
+    service = build(service_name, version, credentials=credentials)
     return service
 
 
 def user_workspace_exist(credentials, work_email, domain):
     """
     Return true if the user email exists in the Google Workspce domain specificated, and false if not.
 
@@ -115,39 +115,43 @@
         "email": primary_email,
         "role": role,
     }
     service.members().insert(body=member_json, groupKey=group).execute()
 
 
 def update_workspace_license(
-    currentProductId, currentSkuId, userId, licenseInstance, credentials
+    current_product_id,
+    current_sku_id,
+    current_user_id,
+    license_instance,
+    credentials,
 ):
     """
     Update the Google Workspace license of a user already created.
 
     Parameters:
     ----------
-        currentProductId: The current product's unique identifier. You can check it in this link https://developers.google.com/admin-sdk/licensing/v1/how-tos/products
-        currentSkuId: The current product SKU's unique identifier. You can check it in this link https://developers.google.com/admin-sdk/licensing/v1/how-tos/products
-        userId: The user's current primary email address.
-        licenseInstance: License object instance for the updated.
+        current_product_id: The current product's unique identifier. You can check it in this link https://developers.google.com/admin-sdk/licensing/v1/how-tos/products
+        current_sku_id: The current product SKU's unique identifier. You can check it in this link https://developers.google.com/admin-sdk/licensing/v1/how-tos/products
+        current_user_id: The user's current primary email address.
+        license_instance: License object instance for the updated.
         Example: {
                     'productId': "Google-Apps",
                     'skuId': "1010020030",
                     'userId': xxxxxx
                     }
         credentials: oauth2client.Credentials or google.auth.credentials.Credentials, credentials to be used for
             authentication. You can get them with 'get_workspace_impersonate_credentials_sa' method.
     """
     service = create_service("licensing", "v1", credentials)
     service.licenseAssignments().update(
-        productId=currentProductId,
-        skuId=currentSkuId,
-        userId=userId,
-        body=licenseInstance,
+        productId=current_product_id,
+        skuId=current_sku_id,
+        userId=current_user_id,
+        body=license_instance,
     ).execute()
 
 
 def get_workspace_impersonate_credentials_sa(
     credentials_info, scopes, impersonate_mail
 ):
     """
```

### Comparing `rudderclient-1.9.0/src/rudderclient/request/exceptions.py` & `rudderclient-1.9.1/src/rudderclient/request/exceptions.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.9.0/src/rudderclient/request/helpers.py` & `rudderclient-1.9.1/src/rudderclient/request/helpers.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.9.0/src/rudderclient/tools/send_email.py` & `rudderclient-1.9.1/src/rudderclient/tools/send_email.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.9.0/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.9.1/src/rudderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.9.0
+Version: 1.9.1
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.9.0/src/rudderclient.egg-info/SOURCES.txt` & `rudderclient-1.9.1/src/rudderclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

