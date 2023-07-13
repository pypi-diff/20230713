# Comparing `tmp/keeper-secrets-manager-core-16.5.4.tar.gz` & `tmp/keeper-secrets-manager-core-16.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-core-16.5.4.tar", last modified: Fri May 19 06:03:08 2023, max compression
+gzip compressed data, was "keeper-secrets-manager-core-16.6.0.tar", last modified: Thu Jul 13 17:43:32 2023, max compression
```

## Comparing `keeper-secrets-manager-core-16.5.4.tar` & `keeper-secrets-manager-core-16.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.424097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/configkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    67982 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/keeper_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:03:08.424097 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 06:03:08.000000 keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 06:03:08.428097 keeper-secrets-manager-core-16.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 06:02:53.000000 keeper-secrets-manager-core-16.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.694559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/configkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77619 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/keeper_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/setup.py
```

### Comparing `keeper-secrets-manager-core-16.5.4/PKG-INFO` & `keeper-secrets-manager-core-16.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.4
+Version: 16.6.0
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,18 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.0
+* KSM-413 - Added support for Folders
+* KSM-434 - Improved Passkey field type support
+
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
 * KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
 * KSM-416 - Fix OS detection bug
 * KSM-400 - Unpinned few dependencies
```

### Comparing `keeper-secrets-manager-core-16.5.4/README.md` & `keeper-secrets-manager-core-16.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.0
+* KSM-413 - Added support for Folders
+* KSM-434 - Improved Passkey field type support
+
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
 * KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
 * KSM-416 - Fix OS detection bug
 * KSM-400 - Unpinned few dependencies
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/configkeys.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/configkeys.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/core.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from http import HTTPStatus
 from typing import List, Tuple, Optional
 
 from keeper_secrets_manager_core import utils, helpers
 from keeper_secrets_manager_core.configkeys import ConfigKeys
 from keeper_secrets_manager_core.crypto import CryptoUtils
 from keeper_secrets_manager_core.dto.dtos import Folder, Record, RecordCreate, SecretsManagerResponse, AppData, \
-    KeeperFileUpload, KeeperFile
+    KeeperFileUpload, KeeperFile, KeeperFolder
 from keeper_secrets_manager_core.dto.payload import CompleteTransactionPayload, GetPayload, UpdatePayload, TransmissionKey, \
-    EncryptedPayload, KSMHttpResponse, CreatePayload, FileUploadPayload, DeletePayload
+    EncryptedPayload, KSMHttpResponse, CreatePayload, FileUploadPayload, DeletePayload, \
+    CreateFolderPayload, UpdateFolderPayload, DeleteFolderPayload, CreateOptions, QueryOptions
 from keeper_secrets_manager_core.exceptions import KeeperError
 from keeper_secrets_manager_core.keeper_globals import keeper_secrets_manager_sdk_client_id, keeper_public_keys, \
     logger_name, keeper_servers
 from keeper_secrets_manager_core.storage import FileKeyValueStorage, KeyValueStorage, InMemoryKeyValueStorage
 from keeper_secrets_manager_core.utils import base64_to_bytes, dict_to_json, \
     url_safe_str_to_bytes, bytes_to_base64, generate_random_bytes, now_milliseconds, string_to_bytes, json_to_dict, \
     bytes_to_string
@@ -286,15 +287,18 @@
 
         if not (
                 isinstance(payload, GetPayload) or
                 isinstance(payload, UpdatePayload) or
                 isinstance(payload, CreatePayload) or
                 isinstance(payload, FileUploadPayload) or
                 isinstance(payload, CompleteTransactionPayload) or
-                isinstance(payload, DeletePayload)):
+                isinstance(payload, DeletePayload) or
+                isinstance(payload, CreateFolderPayload) or
+                isinstance(payload, UpdateFolderPayload) or
+                isinstance(payload, DeleteFolderPayload)):
             raise Exception('Unknown payload type "%s"' % payload.__class__.__name__)
 
         payload_json_str = dict_to_json(payload.__dict__)
         payload_bytes = utils.string_to_bytes(payload_json_str)
 
         encrypted_payload = CryptoUtils.encrypt_aes(payload_bytes, transmission_key.key)
 
@@ -317,50 +321,51 @@
         payload.clientVersion = keeper_secrets_manager_sdk_client_id
         payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
         payload.recordUids = record_uids
 
         return payload
 
     @staticmethod
-    def prepare_get_payload(storage, records_filter):
-
+    def prepare_get_payload(storage, query_options:QueryOptions):
         payload = GetPayload()
 
         payload.clientVersion = keeper_secrets_manager_sdk_client_id
         payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
 
         app_key_str = storage.get(ConfigKeys.KEY_APP_KEY)
 
         if not app_key_str:
 
             public_key_bytes = CryptoUtils.extract_public_key_bytes(storage.get(ConfigKeys.KEY_PRIVATE_KEY))
             public_key_base64 = bytes_to_base64(public_key_bytes)
             # passed once when binding
             payload.publicKey = public_key_base64
 
-        if records_filter:
-            payload.requestedRecords = records_filter
+        if query_options:
+            if query_options.records_filter:
+                payload.requestedRecords = query_options.records_filter
+            if query_options.folders_filter:
+                payload.requestedFolders = query_options.folders_filter
 
         return payload
 
     @staticmethod
-    def prepare_create_payload(storage, folder_uid, record_data_json_str, folder_key):
-
+    def prepare_create_payload(storage, create_options: CreateOptions, record_data_json_str, folder_key):
         owner_public_key = storage.get(ConfigKeys.KEY_OWNER_PUBLIC_KEY)
 
         if not owner_public_key:
-            raise KeeperError('Unable to create record - owner key is missing. Looks like application was created '
-                              'using out date client (Web Vault or Commander)')
+            raise KeeperError('Unable to create record - owner key is missing.'
+                              ' Looks like application was created using'
+                              ' out of date client (Web Vault or Commander)')
 
         owner_public_key_bytes = url_safe_str_to_bytes(owner_public_key)
 
         if not folder_key:
-            raise KeeperError('Unable to create record - folder key for ' + folder_uid + ' is missing')
+            raise KeeperError('Unable to create record - folder key for ' + create_options.folder_uid + ' is missing')
 
-        record_bytes = ""
         record_key = generate_random_bytes(32)
         record_uid = generate_random_bytes(16)
 
         record_data_bytes = utils.string_to_bytes(record_data_json_str)
         record_data_encrypted = CryptoUtils.encrypt_aes(record_data_bytes, record_key)
 
         record_key_encrypted = CryptoUtils.public_encrypt(record_key, owner_public_key_bytes)
@@ -369,17 +374,18 @@
 
         payload = CreatePayload()
 
         payload.clientVersion = keeper_secrets_manager_sdk_client_id
         payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
         payload.recordUid = CryptoUtils.bytes_to_url_safe_str(record_uid)
         payload.recordKey = bytes_to_base64(record_key_encrypted)
-        payload.folderUid = folder_uid
+        payload.folderUid = create_options.folder_uid
         payload.folderKey = bytes_to_base64(folder_key_encrypted)
         payload.data = bytes_to_base64(record_data_encrypted)
+        payload.subFolderUid = create_options.subfolder_uid
 
         return payload
 
     @staticmethod
     def prepare_update_payload(storage, record, transaction_type=None):
 
         payload = UpdatePayload()
@@ -477,14 +483,66 @@
 
         payload.fileSize = len(encrypted_file_data)
         return {
             'payload': payload,
             'encryptedFileData': encrypted_file_data
         }
 
+    @staticmethod
+    def prepare_create_folder_payload(storage, create_options, folder_name, shared_folder_key):
+
+        payload = CreateFolderPayload()
+
+        payload.clientVersion = keeper_secrets_manager_sdk_client_id
+        payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
+        payload.sharedFolderUid = create_options.folder_uid
+        payload.parentUid = create_options.subfolder_uid
+
+        folder_uid = utils.generate_random_bytes(16)
+        payload.folderUid = CryptoUtils.bytes_to_url_safe_str(folder_uid)
+
+        folder_key = utils.generate_random_bytes(32)
+        encrypted_folder_key = CryptoUtils.encrypt_aes_cbc(folder_key, shared_folder_key)
+        payload.sharedFolderKey = CryptoUtils.bytes_to_url_safe_str(encrypted_folder_key)
+
+        folder_json = dict_to_json({"name": folder_name})
+        folder_data_bytes = utils.string_to_bytes(folder_json)
+        encrypted_folder_data = CryptoUtils.encrypt_aes_cbc(folder_data_bytes, folder_key)
+        payload.data = CryptoUtils.bytes_to_url_safe_str(encrypted_folder_data)
+
+        return payload
+
+    @staticmethod
+    def prepare_update_folder_payload(storage, folder_uid, folder_name, folder_key):
+
+        payload = UpdateFolderPayload()
+
+        payload.clientVersion = keeper_secrets_manager_sdk_client_id
+        payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
+        payload.folderUid = folder_uid
+
+        folder_json = dict_to_json({"name": folder_name})
+        folder_data_bytes = utils.string_to_bytes(folder_json)
+        encrypted_folder_data = CryptoUtils.encrypt_aes_cbc(folder_data_bytes, folder_key)
+        payload.data = CryptoUtils.bytes_to_url_safe_str(encrypted_folder_data)
+
+        return payload
+
+    @staticmethod
+    def prepare_delete_folder_payload(storage, folder_uids, force_deletion):
+
+        payload = DeleteFolderPayload()
+
+        payload.clientVersion = keeper_secrets_manager_sdk_client_id
+        payload.clientId = storage.get(ConfigKeys.KEY_CLIENT_ID)
+        payload.folderUids = folder_uids
+        payload.forceDeletion = force_deletion
+
+        return payload
+
     def _post_query(self, path, payload):
 
         keeper_server = helpers.get_server(self.hostname, self.config)
         url = "https://%s/api/rest/sm/v1/%s" % (keeper_server, path)
 
         while True:
 
@@ -604,17 +662,67 @@
             ))
 
         # This is a unknown error, not one of ours, just throw a HTTPError
         reason = f", Reason: {str(rs.reason)}" if rs.reason else ""
         message = f", Message: {str(rs.text)}" if rs.text else ""
         raise requests.HTTPError(f"Status Code: {rs.status_code}{reason}{message}")
 
-    def fetch_and_decrypt_secrets(self, record_filter=None):
+    @staticmethod
+    def get_shared_folder_key(folders: list, response_folders: list, parent: str):
+        folders = folders or []
+        response_folders = response_folders or []
+        while True:
+            parent_folder = next((x for x in response_folders if x.get('folderUid', None) == parent), None)
+            if parent_folder is None:
+                return None
+            if not parent_folder.get('parent', ''):
+                shared_folder = next((x for x in folders if x.folder_uid == parent_folder.get('folderUid', None)), None)
+                if shared_folder is None:
+                    return None
+                else:
+                    return shared_folder.folder_key
+            parent = parent_folder.get('parent', '')
+
+    def fetch_and_decrypt_folders(self):
+        payload = SecretsManager.prepare_get_payload(self.config, [])
+        decrypted_response_bytes = self._post_query('get_folders', payload)
+        decrypted_response_str = utils.bytes_to_string(decrypted_response_bytes)
+        decrypted_response_dict = utils.json_to_dict(decrypted_response_str) or {}
+
+        app_key = base64_to_bytes(self.config.get(ConfigKeys.KEY_APP_KEY))
+        response_folders = decrypted_response_dict.get("folders", []) or []
+        if not response_folders:
+            return []
+
+        folders = []
+        for folder in response_folders:
+            folder_key = folder.get('folderKey')
+            folder_parent = folder.get('parent', '') or ''
+            if not folder_parent:
+                folder_key = CryptoUtils.decrypt_aes(utils.base64_to_bytes(folder_key), app_key)
+            else:
+                shared_folder_key = SecretsManager.get_shared_folder_key(folders, response_folders, folder_parent)
+                folder_key = CryptoUtils.decrypt_aes_cbc(utils.base64_to_bytes(folder_key), shared_folder_key)
+
+            folder_name = ''
+            folder_data = folder.get('data', '')
+            if folder_data:
+                folder_data_json = CryptoUtils.decrypt_aes_cbc(utils.base64_to_bytes(folder_data), folder_key)
+                folder_data_dict = json.loads(folder_data_json.decode())
+                folder_name = folder_data_dict.get('name', '') or ''
+            fldr = KeeperFolder(folder_key,
+                                folder.get('folderUid', '') or '',
+                                folder_parent,
+                                folder_name)
+            folders.append(fldr)
+        return folders
 
-        payload = SecretsManager.prepare_get_payload(self.config, records_filter=record_filter)
+
+    def fetch_and_decrypt_secrets(self, query_options: QueryOptions):
+        payload = SecretsManager.prepare_get_payload(self.config, query_options=query_options)
 
         decrypted_response_bytes = self._post_query(
             'get_secret',
             payload
         )
 
         decrypted_response_str = utils.bytes_to_string(decrypted_response_bytes)
@@ -686,37 +794,51 @@
         sm_response.justBound = just_bound
 
         return sm_response
 
     def get_secrets(self, uids=None, full_response=False):
         """
         Retrieve all records associated with the given application
+        optionally filtered by record uids
         """
 
         if isinstance(uids, str):
             uids = [uids]
 
-        records_resp = self.fetch_and_decrypt_secrets(uids)
+        query_options = QueryOptions(records_filter=uids, folders_filter=None)
+        return self.get_secrets_with_options(query_options, full_response)
+
+    def get_secrets_with_options(self, query_options=None, full_response=False):
+        """
+        Retrieve records associated with the given application
+        optionally filtered by the query options
+        """
+
+        records_resp = self.fetch_and_decrypt_secrets(query_options)
 
         if records_resp.justBound:
-            records_resp = self.fetch_and_decrypt_secrets(uids)
+            records_resp = self.fetch_and_decrypt_secrets(query_options)
 
         # Log warnings we got from the server
         # Will only be displayed if logging is enabled:
         if records_resp.warnings:
             for warning in records_resp.warnings:
                 self.logger.warning(warning)
 
         if full_response:
             return records_resp
         else:
             records: list = records_resp.records or []
 
             return records
 
+    def get_folders(self):
+        # Retrieve all folders
+        return self.fetch_and_decrypt_folders()
+
     def get_secrets_by_title(self, record_title):
         """
         Retrieve all records with specified title
         """
 
         recs = self.get_secrets()
         records = [x for x in recs if x.title == record_title]
@@ -782,20 +904,98 @@
         found_folder = helpers.get_folder_key(folder_uid=folder_uid, secrets_and_folders=records_and_folders_response)
 
         if not found_folder:
             raise KeeperError('Folder uid=' + folder_uid + ' was not retrieved. If you are creating a record to a '
                               'folder folder that you know exists, make sure that at least one record is present in '
                               'the prior to adding a record to the folder.')
 
-        payload = SecretsManager.prepare_create_payload(self.config, folder_uid, record_data_json_str, found_folder.key)
+        create_options = CreateOptions(folder_uid, None)
+        payload = SecretsManager.prepare_create_payload(self.config, create_options, record_data_json_str, found_folder.key)
+        self._post_query('create_secret', payload)
 
+        return payload.recordUid
+
+    def create_secret_with_options(self, create_options: CreateOptions, record_data: RecordCreate, folders: list = []):
+        if not isinstance(record_data, RecordCreate):
+            raise KeeperError('New record data has to be a valid ' + RecordCreate.__name__ + ' object')
+        record_data_json_str = record_data.to_json()
+
+        if not folders:
+            folders = self.get_folders()
+
+        shared_folder = next((x for x in folders if x.folder_uid == create_options.folder_uid), None)
+        if shared_folder is None or not shared_folder.folder_key:
+            raise KeeperError(f'Unable to create record - folder key for {create_options.folder_uid} not found')
+
+        payload = SecretsManager.prepare_create_payload(self.config, create_options, record_data_json_str, shared_folder.folder_key)
         self._post_query('create_secret', payload)
 
         return payload.recordUid
 
+    def create_folder(self, create_options: CreateOptions, folder_name: str, folders=None):
+        """
+        Create new folder using the provided options.
+
+        If folders is None that will force downloading all folders metadata with every request.
+        Folders metadata could be retrieved from get_folders() cached and reused
+        as long as it is not modified externally or internally.
+
+        create_options.folder_uid is required and must be a parent shared folder
+
+        create_options.subfolder_uid could be many levels deep under its parent.
+        If subfolder_uid is empty - new folder is created under parent folder_uid
+        """
+
+        if not folders:
+            folders = self.get_folders()
+
+        shared_folder = next((x for x in folders if x.folder_uid == create_options.folder_uid), None)
+        if shared_folder is None or not shared_folder.folder_key:
+            raise KeeperError(f'Unable to create folder - folder key for {create_options.folder_uid} not found')
+
+        payload = SecretsManager.prepare_create_folder_payload(self.config, create_options, folder_name, shared_folder.folder_key)
+        _ = self._post_query('create_folder', payload)
+        return payload.folderUid
+
+    def update_folder(self, folder_uid: str, folder_name: str, folders=None):
+        """
+        Update folder changes the folder metadata - currently folder name only
+        """
+
+        if not folders:
+            folders = self.get_folders()
+
+        shared_folder = next((x for x in folders if x.folder_uid == folder_uid), None)
+        if shared_folder is None or not shared_folder.folder_key:
+            raise KeeperError(f'Unable to update folder - folder key for {folder_uid} not found')
+
+        payload = SecretsManager.prepare_update_folder_payload(self.config, folder_uid, folder_name, shared_folder.folder_key)
+        _ = self._post_query('update_folder', payload)
+
+    def delete_folder(self, folder_uids, force_deletion=False):
+        """
+        Delete folders with specified folder_uids
+        Use force_deletion flag to delete non-empty folders.
+        Note! When using force_deletion avoid sending parent with its children folder UIDs.
+        Depending on the delete order you may get an error ex. if parent force-deleted child first.
+        There's no guarantee that list will always be processed in FIFO order.
+        Note! Any folder_uids missing from the vault or not shared to the KSM application
+        will not result in error.
+        """
+
+        if isinstance(folder_uids, str):
+            folder_uids = [folder_uids]
+
+        payload = SecretsManager.prepare_delete_folder_payload(self.config, folder_uids, force_deletion)
+        response = self._post_query('delete_folder', payload)
+        response_str = bytes_to_string(response)
+        response_dict = json_to_dict(response_str)
+
+        return response_dict.get('folders', {}) if isinstance(response_dict, dict) else {}
+
     def upload_file(self, owner_record, file: KeeperFileUpload):
         """
         Upload file using provided file upload object
         """
 
         self.logger.info(f"Uploading file: {file.Name} to record uid {owner_record.uid}")
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/crypto.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/crypto.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,30 +11,60 @@
 
 import base64
 import os
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import ec
+from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
+from cryptography.hazmat.primitives.ciphers.algorithms import AES
+from cryptography.hazmat.primitives.ciphers.modes import CBC
+from cryptography.hazmat.primitives.padding import PKCS7
 from cryptography.hazmat.primitives.serialization import load_der_private_key
 
 from . import utils
 
+_CRYPTO_BACKEND = default_backend()
+
+
+def pad_data(data):    # type: (bytes) -> bytes
+    padder = PKCS7(16*8).padder()
+    return padder.update(data) + padder.finalize()
+
+
+def unpad_data(data):     # type: (bytes) -> bytes
+    unpadder = PKCS7(16*8).unpadder()
+    return unpadder.update(data) + unpadder.finalize()
 
 class CryptoUtils:
 
     BS = 16
 
-    pad_binary = lambda s: s + (
-                (CryptoUtils.BS - len(s) % CryptoUtils.BS) * chr(CryptoUtils.BS - len(s) % CryptoUtils.BS)).encode()
-
-    unpad_binary = lambda s: s[0:-s[-1]]
+    @staticmethod
+    def pad_binary(data: bytes, block_size: int = BS) -> bytes:
+        """ Apply standard pkcs7 padding """
+        pad_len = block_size - len(data) % block_size
+        padding = chr(pad_len).encode()*pad_len
+        return data + padding
+
+    @staticmethod
+    def unpad_binary(data: bytes, block_size: int = BS):
+        """ Remove standard pkcs7 padding """
+        data_len = len(data)
+        if data_len % block_size == 0:
+            pad_len = data[-1]
+            if pad_len > 0 and pad_len <= min(block_size, data_len):
+                # if data[-pad_len:] == chr(pad_len).encode()*pad_len:
+                return data[:-pad_len]
+        return data
 
-    unpad_char = lambda s: s[0:-ord(s[-1])]
+    @staticmethod
+    def unpad_char(data):
+        return data[0:-ord(data[-1])]
 
     @staticmethod
     def bytes_to_int(b):
         return int.from_bytes(b, byteorder='big')
 
     @staticmethod
     def url_safe_str_to_bytes(s):
@@ -111,14 +141,35 @@
     def encrypt_aes(data, key, iv=None):
         aesgcm = AESGCM(key)
         iv = iv or os.urandom(12)
         enc = aesgcm.encrypt(iv, data, None)
         return iv + enc
 
     @staticmethod
+    def decrypt_aes(data, key):
+        aesgcm = AESGCM(key)
+        return aesgcm.decrypt(data[:12], data[12:], None)
+
+    @staticmethod
+    def encrypt_aes_cbc(data, key, iv=None):
+        iv = iv or os.urandom(16)
+        cipher = Cipher(AES(key), CBC(iv), backend=_CRYPTO_BACKEND)
+        encryptor = cipher.encryptor()
+        enc = encryptor.update(pad_data(data)) + encryptor.finalize()
+        return iv + enc
+
+    @staticmethod
+    def decrypt_aes_cbc(data, key):
+        iv = data[:16]
+        cipher = Cipher(AES(key), CBC(iv), backend=_CRYPTO_BACKEND)
+        decryptor = cipher.decryptor()
+        decrypted_data = decryptor.update(data[16:]) + decryptor.finalize()
+        return unpad_data(decrypted_data)
+
+    @staticmethod
     def public_encrypt(data: bytes, server_public_raw_key_bytes: bytes, idz: bytes = None):
 
         curve = ec.SECP256R1()
 
         ephemeral_public_key = ec.EllipticCurvePublicKey.from_encoded_point(curve, server_public_raw_key_bytes)
 
         # server_public_key = load_pem_public_key(server_public_key_bytes)
@@ -165,19 +216,14 @@
 
         except Exception as e:
             raise e
 
         return result
 
     @staticmethod
-    def decrypt_aes(data, key):
-        aesgcm = AESGCM(key)
-        return aesgcm.decrypt(data[:12], data[12:], None)
-
-    @staticmethod
     def decrypt_record(data, secret_key):
         if isinstance(data, str):
             data = utils.base64_to_bytes(data)
 
         record = CryptoUtils.decrypt_aes(data, secret_key)
         record_json = utils.bytes_to_string(record)
         return record_json
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/dtos.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/dtos.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,22 @@
         print("")
         print("Custom Fields")
         print("------")
         for item in self.dict.get('custom', []):
             print("{} ({}) : {}".format(item["label"], item["type"], ", ".join(item["value"])))
 
 
+class KeeperFolder:
+    def __init__(self, folder_key, folder_uid:str, parent_uid:str, name:str):
+        self.folder_key = folder_key
+        self.folder_uid = folder_uid
+        self.parent_uid = parent_uid
+        self.name = name
+
+
 class Folder:
 
     def __init__(self, folder, secret_key):
 
         self.uid = ''
         self.records = []
 
@@ -277,16 +285,18 @@
             raise Exception("Not a folder")
 
         folder_uid = folder.get('folderUid')
         folder_key_enc = folder.get('folderKey')
         folder_key = CryptoUtils.decrypt_aes(utils.base64_to_bytes(folder_key_enc), secret_key)
         folder_records = folder.get('records')
 
-        self.uid = folder_uid
         self.key = folder_key
+        self.uid = folder_uid
+        self.parent_uid = folder.get('parentUid', '')
+        self.name = folder.get('name', '')
 
         for r in folder_records:
 
             record = Record(r, folder_key)
             self.records.append(record)
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/dto/payload.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/payload.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,35 +28,64 @@
 class GetPayload:
 
     def __init__(self):
         self.clientVersion = None
         self.clientId = None
         self.publicKey = None
         self.requestedRecords = None
+        self.requestedFolders = None
 
 
 class CreatePayload:
 
     def __init__(self):
         self.clientVersion = None
         self.clientId = None
         self.recordUid = None
         self.recordKey = None
         self.folderUid = None
         self.folderKey = None
         self.data = None
+        self.subFolderUid = None
 
 
 class DeletePayload:
     def __init__(self):
         self.clientVersion = None
         self.clientId = None
         self.recordUids = None
 
 
+class CreateFolderPayload:
+    def __init__(self):
+        self.clientVersion = None
+        self.clientId = None
+        self.folderUid = None
+        self.sharedFolderUid = None
+        self.sharedFolderKey = None
+        self.data = None
+        self.parentUid = None
+
+
+class UpdateFolderPayload:
+    def __init__(self):
+        self.clientVersion = None
+        self.clientId = None
+        self.folderUid = None
+        self.data = None
+
+
+class DeleteFolderPayload:
+    def __init__(self):
+        self.clientVersion = None
+        self.clientId = None
+        self.folderUids = None
+        self.forceDeletion = False
+
+
 class FileUploadPayload:
 
     def __init__(self):
         self.clientVersion = None
         self.clientId = None
         self.fileRecordUid = None
         self.fileRecordKey = None
@@ -95,7 +124,21 @@
 
 class KSMHttpResponse:
 
     def __init__(self, status_code, data, http_response=None):
         self.status_code = status_code
         self.data = data
         self.http_response = http_response
+
+
+class QueryOptions:
+
+    def __init__(self, records_filter, folders_filter):
+        self.records_filter = records_filter
+        self.folders_filter = folders_filter
+
+
+class CreateOptions:
+
+    def __init__(self, folder_uid, subfolder_uid):
+        self.folder_uid = folder_uid
+        self.subfolder_uid = subfolder_uid
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/exceptions.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/helpers.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/helpers.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/keeper_globals.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/keeper_globals.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/mock.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/mock.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/storage.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/storage.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core/utils.py` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/utils.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/PKG-INFO` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.5.4
+Version: 16.6.0
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,18 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.0
+* KSM-413 - Added support for Folders
+* KSM-434 - Improved Passkey field type support
+
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
 * KSM-394 - Ability to load configuration from AWS Secrets Manager using AWS AIM role in EC2 instance or AWS IAM user
 * KSM-416 - Fix OS detection bug
 * KSM-400 - Unpinned few dependencies
```

### Comparing `keeper-secrets-manager-core-16.5.4/keeper_secrets_manager_core.egg-info/SOURCES.txt` & `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.5.4/setup.py` & `keeper-secrets-manager-core-16.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'requests',
     'cryptography>=39.0.1',
     'importlib_metadata'
 ]
 
 setup(
     name="keeper-secrets-manager-core",
-    version="16.5.4",
+    version="16.6.0",
     description="Keeper Secrets Manager for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

