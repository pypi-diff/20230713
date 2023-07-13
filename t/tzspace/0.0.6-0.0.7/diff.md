# Comparing `tmp/tzspace-0.0.6.tar.gz` & `tmp/tzspace-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tzspace-0.0.6.tar", last modified: Tue Jul 11 07:29:32 2023, max compression
+gzip compressed data, was "tzspace-0.0.7.tar", last modified: Thu Jul 13 11:09:41 2023, max compression
```

## Comparing `tzspace-0.0.6.tar` & `tzspace-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.186534 tzspace-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 tzspace-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      530 2023-07-11 07:29:32.186534 tzspace-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-07-08 13:47:46.000000 tzspace-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.150696 tzspace-0.0.6/ior/
--rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.6/ior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.152691 tzspace-0.0.6/ior/config/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.6/ior/config/__init__.py
--rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.6/ior/config/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.161460 tzspace-0.0.6/ior/config/contracts/
--rw-rw-rw-   0        0        0    90537 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/Certificate.json
--rw-rw-rw-   0        0        0    29114 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/Exchange.json
--rw-rw-rw-   0        0        0    26608 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/PermissionControl.json
--rw-rw-rw-   0        0        0    29186 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/RoleControl.json
--rw-rw-rw-   0        0        0    71651 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/StoredNFT.json
--rw-rw-rw-   0        0        0    35700 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/TZContractTemplate.json
--rw-rw-rw-   0        0        0    38166 2023-03-26 16:06:07.000000 tzspace-0.0.6/ior/config/contracts/TZTemplateControl.json
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.173145 tzspace-0.0.6/ior/core/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.6/ior/core/__init__.py
--rw-rw-rw-   0        0        0     6241 2023-07-11 06:38:39.000000 tzspace-0.0.6/ior/core/certificate_service.py
--rw-rw-rw-   0        0        0     1657 2023-07-08 15:09:13.000000 tzspace-0.0.6/ior/core/exchange_service.py
--rw-rw-rw-   0        0        0     3706 2023-07-08 15:08:37.000000 tzspace-0.0.6/ior/core/permission_control_service.py
--rw-rw-rw-   0        0        0     4546 2023-07-08 15:08:23.000000 tzspace-0.0.6/ior/core/role_control_service.py
--rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.6/ior/core/stored_nft_service.py
--rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.6/ior/core/tz_contract_template_service.py
--rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.6/ior/core/tz_template_control_service.py
--rw-rw-rw-   0        0        0     1355 2023-07-08 15:14:38.000000 tzspace-0.0.6/ior/iorconfig.py
--rw-rw-rw-   0        0        0     2732 2023-07-11 07:29:11.000000 tzspace-0.0.6/ior/iorsdk.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.178351 tzspace-0.0.6/ior/util/
--rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.6/ior/util/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.6/ior/util/certificate_utils.py
--rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.6/ior/util/result_utils.py
--rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.6/ior/util/web3_utils.py
--rw-rw-rw-   0        0        0       42 2023-07-11 07:29:32.186534 tzspace-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-07-11 07:29:24.000000 tzspace-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 07:29:32.184260 tzspace-0.0.6/tzspace.egg-info/
--rw-rw-rw-   0        0        0      530 2023-07-11 07:29:31.000000 tzspace-0.0.6/tzspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-07-11 07:29:32.000000 tzspace-0.0.6/tzspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 07:29:31.000000 tzspace-0.0.6/tzspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-11 07:29:31.000000 tzspace-0.0.6/tzspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.056719 tzspace-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-07-08 13:48:47.000000 tzspace-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-07-11 07:20:58.000000 tzspace-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      466 2023-07-13 11:09:41.056719 tzspace-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13928 2023-07-13 11:08:24.000000 tzspace-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.024780 tzspace-0.0.7/ior/
+-rw-rw-rw-   0        0        0        0 2023-07-08 13:44:53.000000 tzspace-0.0.7/ior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.026769 tzspace-0.0.7/ior/config/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:55:01.000000 tzspace-0.0.7/ior/config/__init__.py
+-rw-rw-rw-   0        0        0     1051 2023-07-08 15:18:53.000000 tzspace-0.0.7/ior/config/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.036264 tzspace-0.0.7/ior/config/contracts/
+-rw-rw-rw-   0        0        0    90537 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/Certificate.json
+-rw-rw-rw-   0        0        0    29114 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/Exchange.json
+-rw-rw-rw-   0        0        0    26608 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/PermissionControl.json
+-rw-rw-rw-   0        0        0    29186 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/RoleControl.json
+-rw-rw-rw-   0        0        0    71651 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/StoredNFT.json
+-rw-rw-rw-   0        0        0    35700 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/TZContractTemplate.json
+-rw-rw-rw-   0        0        0    38166 2023-03-26 16:06:07.000000 tzspace-0.0.7/ior/config/contracts/TZTemplateControl.json
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.044922 tzspace-0.0.7/ior/core/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:42.000000 tzspace-0.0.7/ior/core/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-07-13 09:58:58.000000 tzspace-0.0.7/ior/core/certificate_service.py
+-rw-rw-rw-   0        0        0     1709 2023-07-13 09:56:40.000000 tzspace-0.0.7/ior/core/exchange_service.py
+-rw-rw-rw-   0        0        0     3750 2023-07-13 10:37:45.000000 tzspace-0.0.7/ior/core/permission_control_service.py
+-rw-rw-rw-   0        0        0     5524 2023-07-13 10:25:47.000000 tzspace-0.0.7/ior/core/role_control_service.py
+-rw-rw-rw-   0        0        0     1739 2023-07-08 15:05:36.000000 tzspace-0.0.7/ior/core/stored_nft_service.py
+-rw-rw-rw-   0        0        0     5628 2023-07-08 15:05:44.000000 tzspace-0.0.7/ior/core/tz_contract_template_service.py
+-rw-rw-rw-   0        0        0     5856 2023-07-08 15:05:49.000000 tzspace-0.0.7/ior/core/tz_template_control_service.py
+-rw-rw-rw-   0        0        0     1537 2023-07-13 08:41:23.000000 tzspace-0.0.7/ior/iorconfig.py
+-rw-rw-rw-   0        0        0     2777 2023-07-13 10:50:06.000000 tzspace-0.0.7/ior/iorsdk.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.049566 tzspace-0.0.7/ior/util/
+-rw-rw-rw-   0        0        0        0 2023-03-26 12:54:52.000000 tzspace-0.0.7/ior/util/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-02 01:59:44.000000 tzspace-0.0.7/ior/util/certificate_utils.py
+-rw-rw-rw-   0        0        0      901 2023-04-02 12:41:43.000000 tzspace-0.0.7/ior/util/result_utils.py
+-rw-rw-rw-   0        0        0     3582 2023-04-02 12:43:26.000000 tzspace-0.0.7/ior/util/web3_utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:09:41.056719 tzspace-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-07-13 11:09:36.000000 tzspace-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:09:41.054637 tzspace-0.0.7/tzspace.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      898 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-13 11:09:40.000000 tzspace-0.0.7/tzspace.egg-info/top_level.txt
```

### Comparing `tzspace-0.0.6/LICENSE` & `tzspace-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/consts.py` & `tzspace-0.0.7/ior/config/consts.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/Certificate.json` & `tzspace-0.0.7/ior/config/contracts/Certificate.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/Exchange.json` & `tzspace-0.0.7/ior/config/contracts/Exchange.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/PermissionControl.json` & `tzspace-0.0.7/ior/config/contracts/PermissionControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/RoleControl.json` & `tzspace-0.0.7/ior/config/contracts/RoleControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/StoredNFT.json` & `tzspace-0.0.7/ior/config/contracts/StoredNFT.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/TZContractTemplate.json` & `tzspace-0.0.7/ior/config/contracts/TZContractTemplate.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/config/contracts/TZTemplateControl.json` & `tzspace-0.0.7/ior/config/contracts/TZTemplateControl.json`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/core/certificate_service.py` & `tzspace-0.0.7/ior/core/certificate_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 )
 
 
 class CertificateService(object):
     def __init__(self, w3, config, address):
         self.w3 = w3
         self.config = config
+        self.address = address
         self.abi = get_abi(certificate_path)
         self.certificate_contract_instance = contract_instance(self.w3, address, self.abi)
 
     @property
     def functions(self):
         if not self.certificate_contract_instance:
             raise RuntimeError("合约获取失败【certificate_contract】")
@@ -47,15 +48,15 @@
         :return:
         """
         func = self.functions.mint(to)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
         block: HexBytes = receipt.get("blockHash")
         transaction: HexBytes = receipt.get("transactionHash")
-        return block.hex(), transaction.hex()
+        return block.hex(), transaction.hex(), receipt
 
     def bind_option(self, option, public_key, private_key):
         """
         合约方法 bindOption(address option_)
         合约返回 无
         :param option:
         :param public_key:
@@ -89,18 +90,17 @@
         合约方法 isAuthorizeApproved(uint256 tokenId, address operator)
         合约返回 bool
         :param token_id:
         :param operator:
         :return:
         """
         res = self.functions.isAuthorizeApproved(token_id, operator).call()
-        print(res)
         return res
 
-    def authorize(self, to: str, original_token_id: int, public_key: str, private_key: str) -> int:
+    def authorize(self, to: str, original_token_id: int, public_key: str, private_key: str):
         """
         合约方法 authorize(address to, uint256 originalTokenId)
         合约返回 uint256 tokenId
         :param to:
         :param original_token_id:
         :param public_key:
         :param private_key:
@@ -111,36 +111,42 @@
         print(receipt)
         return receipt
 
     def create_option(self, to, original_token_id, price, effect_date, public_key, private_key):
         func = self.functions.createOption(to, original_token_id, price, effect_date)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def authorize_option(self, to, original_token_id, option_token_id, public_key, private_key):
         func = self.functions.authorizeOption(to, original_token_id, option_token_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def recreate(self, to, ref_token_ids, public_key, private_key):
         func = self.functions.recreate(to, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def recreate_in_chain(self, to, certificates, ref_token_ids, public_key, private_key):
         func = self.functions.recreateInChain(to, certificates, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def recreate_cross_chain(self, to, chain_ids, certificates, ref_token_ids, public_key, private_key):
         func = self.functions.recreateCrossChain(to, chain_ids, certificates, ref_token_ids)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def update_token_id_mapping(self, token_id, original_token_id, public_key, private_key):
         func = self.functions.updateTokenIdMapping(token_id, original_token_id)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def token_uri(self, token_id):
         res = self.functions.tokenURI(token_id).call()
-        print(res)
+        return res
```

### Comparing `tzspace-0.0.6/ior/core/exchange_service.py` & `tzspace-0.0.7/ior/core/exchange_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 
     @property
     def functions(self):
         if not self.exchange_contract_instance:
             raise RuntimeError("合约获取失败【exchange_contract】")
         return contract_functions(self.exchange_contract_instance)
 
-    def exchange(self, nft_address: str, token_id: int, from_address: str, to_address: str, price: int, public_key: str,
+    def exchange(self, cert_address: str, token_id: int, from_address: str, to_address: str, price: int, public_key: str,
                  private_key: str):
-        func = self.functions.exchange(nft_address, token_id, from_address, to_address, price)
+        func = self.functions.exchange(cert_address, token_id, from_address, to_address, price)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         #print(receipt)
+        return receipt
 
-    def exchange_with_feed(self, nft_address: str, token_id: int, from_address: str, to_address: str, price: int,
+    def exchange_with_feed(self, cert_address: str, token_id: int, from_address: str, to_address: str, price: int,
                            fee: int, feeds: list[str], percents: list[int], public_key: str, private_key: str):
-        func = self.functions.exchangeWithFeed(nft_address, token_id, from_address, to_address, price, fee, feeds,
+        func = self.functions.exchangeWithFeed(cert_address, token_id, from_address, to_address, price, fee, feeds,
                                                percents)
         receipt = func_send_raw_transaction(self.w3, func, public_key, private_key, self.config.timeout, self.config.poll_latency)
         #print(receipt)
+        return receipt
```

### Comparing `tzspace-0.0.6/ior/core/permission_control_service.py` & `tzspace-0.0.7/ior/core/permission_control_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         """
         合约属性 mapping(bytes32=>mapping(bytes32 =>TzPermissionData)) public datas
         :param key:
         :return:
         """
         res = self.functions.datas(key).call()
         print(res)
+        return res
 
     def add_permission(self, permission_name: str, data: list[str], operations: list[int],
                        default_operations: list[int], parent: list[int], hash_values: list[str], public_key: str,
                        private_key: str):
         """
         合约方法 addPermission(bytes32 permissionName, bytes32[] calldata data, uint32[] calldata operations,
                 uint32[] calldata defaultOperations, bytes32[] calldata parent, bytes32[] calldata hash)
@@ -44,14 +45,15 @@
         permission_name_bytes = f"0x{permission_name.encode().hex()}"
         data_bytes = [f"0x{d.encode().hex()}" for d in data]
         hash_values_bytes = [f"0x{h.encode().hex()}" for h in hash_values]
         func = self.functions.addPermission(permission_name_bytes, data_bytes, operations, default_operations, parent,
                                             hash_values_bytes)
         receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
     def del_permission(self, permission_name: str, data: list[str], public_key: str, private_key: str):
         """
         合约方法 delPermission(bytes32 permissionName, bytes32[] calldata data)
         合约返回 无
         :param permission_name:
         :param data:
@@ -60,22 +62,23 @@
         :return:
         """
         permission_name_bytes = f"0x{permission_name.encode().hex()}"
         data_bytes = [f"0x{d.encode().hex()}" for d in data]
         func = self.functions.delPermission(permission_name_bytes, data_bytes)
         receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
         print(receipt)
+        return receipt
 
-    def check_permission(self, permission_name: str, data_hash: str, operations: int) -> bool:
+    def check_permission(self, permission_name: str, data: str, operations: int) -> bool:
         """
-        合约方法 checkPermission(bytes32 permissionName, bytes32 dataHash, uint32 operations)
+        合约方法 checkPermission(bytes32 permissionName, bytes32 data, uint32 operations)
         合约返回 bool
         :param permission_name:
         :param data_hash:
         :param operations:
         :return:
         """
         permission_name_bytes = f"0x{permission_name.encode().hex()}"
-        data_hash_bytes = f"0x{data_hash.encode().hex()}"
-        res = self.functions.checkPermission(permission_name_bytes, data_hash_bytes, operations).call()
+        data_bytes = f"0x{data.encode().hex()}"
+        res = self.functions.checkPermission(permission_name_bytes, data_bytes, operations).call()
         print(res)
         return res
```

### Comparing `tzspace-0.0.6/ior/core/role_control_service.py` & `tzspace-0.0.7/ior/core/role_control_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,37 @@
         """
         合约属性 mapping(bytes32 => TzRoleData) public roles
         :param key:
         :return:
         """
         res = self.functions.roles(key).call()
         print(res)
+        return res
+
+
+    def grant_role(self, role_name: str, to: str, public_key: str, private_key: str):
+
+        role_name_bytes = f"0x{role_name.encode().hex()}"
+        func = self.functions.grantRole(role_name_bytes, to)
+        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
+        print(receipt)
+
+    def revoke_role(self, role_name: str, to: str, public_key: str, private_key: str):
+
+        role_name_bytes = f"0x{role_name.encode().hex()}"
+        func = self.functions.revokeRole(role_name_bytes, to)
+        receipt = func_send_raw_transaction(func, self.w3, private_key, public_key, self.config.timeout, self.config.poll_latency)
+        print(receipt)
+
+    def has_role(self, role_name: str, to: str):
+
+        role_name_bytes = f"0x{role_name.encode().hex()}"
+        res = self.functions.hasRole(role_name_bytes,to).call()
+        print(res)
+        return res
 
     def add_role(self, role_name: str, admin_role: str, permission_role: str, permissions: list[str],
                  permission_contract_addrs: list[str], public_key: str, private_key: str):
         """
         合约方法 addRole(bytes32 roleName, bytes32 adminRole, bytes32 permissionRole,
                             bytes32[] calldata permissions, address[] calldata permissionContractAddrs)
         合约返回 无
```

### Comparing `tzspace-0.0.6/ior/core/stored_nft_service.py` & `tzspace-0.0.7/ior/core/stored_nft_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/core/tz_contract_template_service.py` & `tzspace-0.0.7/ior/core/tz_contract_template_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/core/tz_template_control_service.py` & `tzspace-0.0.7/ior/core/tz_template_control_service.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/iorconfig.py` & `tzspace-0.0.7/ior/iorconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,20 +21,30 @@
 		"TZContractTemplate": "0x59400c0ad731d23032B68E6B3f5ac0F8862eb83f"
 	}
 
 
 	# 连接地址
 	provider = "https://data-seed-prebsc-2-s3.binance.org:8545/"
 
+	is_poa = False
+
+	is_print = False
+
 	def __init__(self):
 		None
 
-	def set_contract_addresses(contract_addresses):
+	def set_contract_addresses(self, contract_addresses):
 		if contract_addresses!=None:
 			self.contract_addresses = contract_addresses
 
-	def set_default_service_contract_addresses(contract_addresses):
+	def set_default_service_contract_addresses(self, contract_addresses):
 		if contract_addresses!=None:
 			self.default_service_contract_addresses = contract_addresses
 
-	def set_provider(provider):
-		self.provider = provider
+	def set_provider(self, provider):
+		self.provider = provider
+
+	def set_is_poa(self, is_poa):
+		self.is_poa = is_poa
+
+	def set_is_print(self, is_print):
+		self.is_print = is_print
```

### Comparing `tzspace-0.0.6/ior/iorsdk.py` & `tzspace-0.0.7/ior/iorsdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 
 class IORSdk(object):
 
 	services = {}
 
 	def __init__(self, config):
 		self._config = config
-		self._w3 = get_web3(config.provider, False)
+		self._w3 = get_web3(config.provider, self._config.is_print, self._config.is_poa)
 
 		self.services['tempctrl'] = TZTemplateControlService(self._w3, self._config)
 		self.services['permission'] = PermissionControlService(self._w3, self._config)
 		self.services['role'] = RoleControlService(self._w3, self._config)
 		self.services['exchange'] = ExchangeService(self._w3, self._config)
 
 	def init_service(self):
 		self.registerService('stcc',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['STCCertificate']))
 		self.registerService('datac',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['DATACertificate']))
 		self.registerService('ctcc',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['CTCCertificate']))
 		self.registerService('mdcc',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['MDCCertificate']))
 		self.registerService('gncc',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['GNCCertificate']))
 		self.registerService('inft1',CertificateService(self._w3, self._config, self._config.default_service_contract_addresses['INFT1Certificate']))
 
-		self.registerService('contract1',CertificateService(self.w3, self._config, self._config.default_service_contract_addresses['TZContractTemplate']))
+		self.registerService('contract1',TZContractTemplateService(self._w3, self._config, self._config.default_service_contract_addresses['TZContractTemplate']))
 
 	@property
 	def w3(self):
 		return self._w3
 
 	@property
 	def tempctrl(self):
```

### Comparing `tzspace-0.0.6/ior/util/certificate_utils.py` & `tzspace-0.0.7/ior/util/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/util/result_utils.py` & `tzspace-0.0.7/ior/util/result_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/ior/util/web3_utils.py` & `tzspace-0.0.7/ior/util/web3_utils.py`

 * *Files identical despite different names*

### Comparing `tzspace-0.0.6/tzspace.egg-info/SOURCES.txt` & `tzspace-0.0.7/tzspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

