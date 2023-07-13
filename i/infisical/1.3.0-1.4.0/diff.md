# Comparing `tmp/infisical-1.3.0.tar.gz` & `tmp/infisical-1.4.0.tar.gz`

## Comparing `infisical-1.3.0.tar` & `infisical-1.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 infisical-1.3.0/.editorconfig
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 infisical-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 infisical-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/__version__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/constants.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/logger.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/create_secret.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/delete_secret.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/get_secret.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/get_secrets.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/get_service_token_data.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/models.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/api/update_secret.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/client/__init__.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/client/infisicalclient.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/helpers/__init__.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/helpers/client.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/helpers/secrets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/models/__init__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/models/api.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/models/models.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/models/secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/services/__init__.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/services/secret_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/utils/__init__.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/utils/crypto.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 infisical-1.3.0/infisical/utils/http.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 infisical-1.3.0/scripts/format.sh
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 infisical-1.3.0/scripts/lint.sh
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 infisical-1.3.0/scripts/test.sh
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 infisical-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 infisical-1.3.0/tests/test_infisical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.3.0/tests/test_client/__init__.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 infisical-1.3.0/tests/test_client/test_infisical_client.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 infisical-1.3.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 infisical-1.3.0/LICENSE
--rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 infisical-1.3.0/README.md
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 infisical-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 infisical-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 infisical-1.4.0/.editorconfig
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 infisical-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 infisical-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/__version__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/constants.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/logger.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/create_secret.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/delete_secret.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/get_secret.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/get_secrets.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/get_service_token_data.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/models.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/api/update_secret.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/client/__init__.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/client/infisicalclient.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/helpers/__init__.py
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/helpers/client.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/helpers/secrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/models/__init__.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/models/api.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/models/models.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/models/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/services/__init__.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/services/secret_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/utils/__init__.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/utils/crypto.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 infisical-1.4.0/infisical/utils/http.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 infisical-1.4.0/scripts/format.sh
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 infisical-1.4.0/scripts/lint.sh
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 infisical-1.4.0/scripts/test.sh
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 infisical-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 infisical-1.4.0/tests/test_infisical.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infisical-1.4.0/tests/test_client/__init__.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 infisical-1.4.0/tests/test_client/test_infisical_client.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 infisical-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 infisical-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 infisical-1.4.0/README.md
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 infisical-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 infisical-1.4.0/PKG-INFO
```

### Comparing `infisical-1.3.0/CHANGELOG.md` & `infisical-1.4.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 All notable changes will be documented in this file.
 
+## [1.4.0] - 2023-07-13
+
+This version adds support for folders or path-based secret storage for all secret CRUD operations.
+
 ## [1.3.0] - 2023-05-05
 
 This version adds support for generating a symmetric encryption key, symmetric encryption, and decryption; algorithm used is `aes-256-gcm` with 96-bit `iv`.
 
 - `create_symmetric_key()`: Method to create a base64-encoded, 256-bit symmetric key.
 - `encrypt_symmetric()`: Method to symmetrically encrypt plaintext using the symmetric key.
 - `decrypt_symmetric()`: Method to symmetrically decrypt ciphertext using the symmetric key.
```

### Comparing `infisical-1.3.0/infisical/api/__init__.py` & `infisical-1.4.0/infisical/api/__init__.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/create_secret.py` & `infisical-1.4.0/infisical/api/create_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/delete_secret.py` & `infisical-1.4.0/infisical/api/delete_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/get_secret.py` & `infisical-1.4.0/infisical/api/get_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/get_secrets.py` & `infisical-1.4.0/infisical/api/get_secrets.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/get_service_token_data.py` & `infisical-1.4.0/infisical/api/get_service_token_data.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/models.py` & `infisical-1.4.0/infisical/api/models.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/api/update_secret.py` & `infisical-1.4.0/infisical/api/update_secret.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/client/infisicalclient.py` & `infisical-1.4.0/infisical/client/infisicalclient.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/helpers/client.py` & `infisical-1.4.0/infisical/helpers/client.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/helpers/secrets.py` & `infisical-1.4.0/infisical/helpers/secrets.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/models/api.py` & `infisical-1.4.0/infisical/models/api.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/models/models.py` & `infisical-1.4.0/infisical/models/models.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/services/secret_service.py` & `infisical-1.4.0/infisical/services/secret_service.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/utils/crypto.py` & `infisical-1.4.0/infisical/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/infisical/utils/http.py` & `infisical-1.4.0/infisical/utils/http.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/tests/test_client/test_infisical_client.py` & `infisical-1.4.0/tests/test_client/test_infisical_client.py`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/.gitignore` & `infisical-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/LICENSE` & `infisical-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/README.md` & `infisical-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/pyproject.toml` & `infisical-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infisical-1.3.0/PKG-INFO` & `infisical-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infisical
-Version: 1.3.0
+Version: 1.4.0
 Summary: Official Infisical SDK for Python
 Project-URL: Documentation, https://github.com/Infisical/infisical-python#readme
 Project-URL: Issues, https://github.com/Infisical/infisical-python/issues
 Project-URL: Source, https://github.com/Infisical/infisical-python
 Maintainer-email: Yohann MARTIN <contact@codexus.fr>, Tony Dang <tony@infisical.com>
 License-Expression: MIT
 License-File: LICENSE
```

