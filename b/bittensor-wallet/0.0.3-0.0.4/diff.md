# Comparing `tmp/bittensor-wallet-0.0.3.tar.gz` & `tmp/bittensor-wallet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-wallet-0.0.3.tar", last modified: Tue Jul 11 04:52:52 2023, max compression
+gzip compressed data, was "bittensor-wallet-0.0.4.tar", last modified: Thu Jul 13 20:19:06 2023, max compression
```

## Comparing `bittensor-wallet-0.0.3.tar` & `bittensor-wallet-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.257120 bittensor-wallet-0.0.3/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.3/LICENSE
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-11 04:52:52.256959 bittensor-wallet-0.0.3/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-07-11 04:50:28.000000 bittensor-wallet-0.0.3/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.254638 bittensor-wallet-0.0.3/bittensor_wallet/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-07-11 04:46:12.000000 bittensor-wallet-0.0.3/bittensor_wallet/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.255586 bittensor-wallet-0.0.3/bittensor_wallet/_keyfile/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/_keyfile/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.3/bittensor_wallet/_keyfile/keyfile_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.3/bittensor_wallet/keypair_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.256209 bittensor-wallet-0.0.3/bittensor_wallet/mock/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1226 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3235 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/keyfile_mock.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.256467 bittensor-wallet-0.0.3/bittensor_wallet/mock/utils/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1122 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/utils/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1669 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/utils/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      658 2023-07-11 04:46:12.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3468 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/bittensor_wallet/mock/wallet_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.3/bittensor_wallet/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.3/bittensor_wallet/wallet_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.255322 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-11 04:52:52.000000 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      678 2023-07-11 04:52:52.000000 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-11 04:52:52.000000 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      165 2023-07-11 04:52:52.000000 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-11 04:52:52.000000 bittensor-wallet-0.0.3/bittensor_wallet.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-11 04:52:52.257165 bittensor-wallet-0.0.3/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.3/setup.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-11 04:52:52.256731 bittensor-wallet-0.0.3/tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11791 2023-06-26 22:03:52.000000 bittensor-wallet-0.0.3/tests/test.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9441 2023-06-26 22:03:51.000000 bittensor-wallet-0.0.3/tests/test_keypair.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.834747 bittensor-wallet-0.0.4/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.4/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-13 20:19:06.834590 bittensor-wallet-0.0.4/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-07-11 22:18:27.000000 bittensor-wallet-0.0.4/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.831829 bittensor-wallet-0.0.4/bittensor_wallet/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-07-11 22:18:41.000000 bittensor-wallet-0.0.4/bittensor_wallet/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.832842 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/keyfile_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/keypair_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.833492 bittensor-wallet-0.0.4/bittensor_wallet/mock/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1226 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3235 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/keyfile_mock.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.833923 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1211 2023-07-11 21:42:39.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1669 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      658 2023-07-11 04:46:12.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3468 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/bittensor_wallet/mock/wallet_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.4/bittensor_wallet/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.4/bittensor_wallet/wallet_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.832561 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      678 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      165 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-13 20:19:06.000000 bittensor-wallet-0.0.4/bittensor_wallet.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-13 20:19:06.834797 bittensor-wallet-0.0.4/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-07-11 04:43:57.000000 bittensor-wallet-0.0.4/setup.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 20:19:06.834319 bittensor-wallet-0.0.4/tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12379 2023-07-11 22:16:48.000000 bittensor-wallet-0.0.4/tests/test.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     9441 2023-06-26 22:03:51.000000 bittensor-wallet-0.0.4/tests/test_keypair.py
```

### Comparing `bittensor-wallet-0.0.3/LICENSE` & `bittensor-wallet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/PKG-INFO` & `bittensor-wallet-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.3
+Version: 0.0.4
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.3
+# BittensorWallet - v0.0.4
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.3
+pip install bittensor-wallet==0.0.4
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.3/README.md` & `bittensor-wallet-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# BittensorWallet - v0.0.3
+# BittensorWallet - v0.0.4
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.3
+pip install bittensor-wallet==0.0.4
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/__init__.py` & `bittensor-wallet-0.0.4/bittensor_wallet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __ss58_format__ = 42 # Bittensor ss58 format
 
 import argparse
 import copy
 import os
 from typing import Optional
```

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/_keyfile/__init__.py` & `bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/_keyfile/keyfile_impl.py` & `bittensor-wallet-0.0.4/bittensor_wallet/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/keypair_impl.py` & `bittensor-wallet-0.0.4/bittensor_wallet/keypair_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/__init__.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/keyfile_mock.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/utils/__init__.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,7 +10,9 @@
 # the Software.
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
+
+from .utils import get_mock_coldkey, get_mock_hotkey, get_mock_keypair, get_mock_wallet
```

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/utils/utils.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/utils.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/mock/wallet_mock.py` & `bittensor-wallet-0.0.4/bittensor_wallet/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/utils.py` & `bittensor-wallet-0.0.4/bittensor_wallet/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet/wallet_impl.py` & `bittensor-wallet-0.0.4/bittensor_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet.egg-info/PKG-INFO` & `bittensor-wallet-0.0.4/bittensor_wallet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.3
+Version: 0.0.4
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.3
+# BittensorWallet - v0.0.4
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.3
+pip install bittensor-wallet==0.0.4
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.3/bittensor_wallet.egg-info/SOURCES.txt` & `bittensor-wallet-0.0.4/bittensor_wallet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/setup.py` & `bittensor-wallet-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.3/tests/test.py` & `bittensor-wallet-0.0.4/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,70 +24,71 @@
 import unittest
 from unittest.mock import patch
 
 from bittensor_wallet.keypair_impl import Keypair
 from bittensor_wallet.wallet_impl import Wallet
 from bittensor_wallet._keyfile import Keyfile, keyfile
 from bittensor_wallet._keyfile.keyfile_impl import validate_password, ask_password_to_encrypt, decrypt_keyfile_data, KeyFileError
+from bittensor_wallet.mock import MockKeyfile, MockWallet
 
 class TestWallet(unittest.TestCase):
 
     def test_regen_coldkeypub_from_ss58_addr(self):
         ss58_address = "5DD26kC2kxajmwfbbZmVmxhrY9VeeyR1Gpzy9i8wxLUg6zxm"
-        mock_wallet = Wallet()
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
         with patch.object(mock_wallet, 'set_coldkeypub') as mock_set_coldkeypub:
             mock_wallet.regenerate_coldkeypub( ss58_address=ss58_address )
 
             mock_set_coldkeypub.assert_called_once()
             keypair: Keypair = mock_set_coldkeypub.call_args_list[0][0][0]
             self.assertEqual(keypair.ss58_address, ss58_address)
 
         ss58_address_bad = "5DD26kC2kxajmwfbbZmVmxhrY9VeeyR1Gpzy9i8wxLUg6zx" # 1 character short
         with pytest.raises(ValueError):
-            self.mock_wallet.regenerate_coldkeypub(ss58_address=ss58_address_bad)
+            mock_wallet.regenerate_coldkeypub(ss58_address=ss58_address_bad)
 
     def test_regen_coldkeypub_from_hex_pubkey_str(self):
         pubkey_str = "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f"
 
-        mock_wallet = Wallet()
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
         with patch.object(mock_wallet, 'set_coldkeypub') as mock_set_coldkeypub:
             mock_wallet.regenerate_coldkeypub(public_key=pubkey_str)
 
             mock_set_coldkeypub.assert_called_once()
             keypair: Keypair = mock_set_coldkeypub.call_args_list[0][0][0]
             self.assertEqual('0x' + keypair.public_key.hex(), pubkey_str)
 
         pubkey_str_bad = "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512" # 1 character short
         with pytest.raises(ValueError):
-            self.mock_wallet.regenerate_coldkeypub(ss58_address=pubkey_str_bad)
+            mock_wallet.regenerate_coldkeypub(ss58_address=pubkey_str_bad)
 
     def test_regen_coldkeypub_from_hex_pubkey_bytes(self):
         pubkey_str = "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f"
         pubkey_bytes = bytes.fromhex(pubkey_str[2:]) # Remove 0x from beginning
 
-        mock_wallet = Wallet()
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
         with patch.object(mock_wallet, 'set_coldkeypub') as mock_set_coldkeypub:
             mock_wallet.regenerate_coldkeypub(public_key=pubkey_bytes)
 
             mock_set_coldkeypub.assert_called_once()
             keypair: Keypair = mock_set_coldkeypub.call_args_list[0][0][0]
             self.assertEqual(keypair.public_key, pubkey_bytes)
 
     def test_regen_coldkeypub_no_pubkey(self):
-        mock_wallet = Wallet()
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
 
         with pytest.raises(ValueError):
             # Must provide either public_key or ss58_address
             mock_wallet.regenerate_coldkeypub(ss58_address=None, public_key=None)
 
     def test_regen_coldkey_from_hex_seed_str(self):
         ss58_addr = "5D5cwd8DX6ij7nouVcoxDuWtJfiR1BnzCkiBVTt7DU8ft5Ta"
         seed_str = "0x659c024d5be809000d0d93fe378cfde020846150b01c49a201fc2a02041f7636"
 
-        mock_wallet = Wallet()
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
         with patch.object(mock_wallet, 'set_coldkey') as mock_set_coldkey:
             mock_wallet.regenerate_coldkey(seed=seed_str)
 
             mock_set_coldkey.assert_called_once()
             keypair: Keypair = mock_set_coldkey.call_args_list[0][0][0]
             self.assertRegex(keypair.seed_hex if isinstance(keypair.seed_hex, str) else keypair.seed_hex.hex(), rf'(0x|){seed_str[2:]}')
             self.assertEqual(keypair.ss58_address, ss58_addr) # Check that the ss58 address is correct
@@ -96,16 +97,16 @@
         with pytest.raises(ValueError):
             mock_wallet.regenerate_coldkey(seed=seed_str_bad)
 
     def test_regen_hotkey_from_hex_seed_str(self):
         ss58_addr = "5D5cwd8DX6ij7nouVcoxDuWtJfiR1BnzCkiBVTt7DU8ft5Ta"
         seed_str = "0x659c024d5be809000d0d93fe378cfde020846150b01c49a201fc2a02041f7636"
 
-        mock_wallet = Wallet()
-        with patch.object(self.mock_wallet, 'set_hotkey') as mock_set_hotkey:
+        mock_wallet = MockWallet( name=f"mock", hotkey="mock_hk", path=f"/tmp/mock-wallet-{self.id()}" )
+        with patch.object(mock_wallet, 'set_hotkey') as mock_set_hotkey:
             mock_wallet.regenerate_hotkey(seed=seed_str)
 
             mock_set_hotkey.assert_called_once()
             keypair: Keypair = mock_set_hotkey.call_args_list[0][0][0]
             self.assertRegex(keypair.seed_hex if isinstance(keypair.seed_hex, str) else keypair.seed_hex.hex(), rf'(0x|){seed_str[2:]}')
             self.assertEqual(keypair.ss58_address, ss58_addr) # Check that the ss58 address is correct
 
@@ -122,68 +123,68 @@
 
         self.create_keyfile()
 
     def tearDown(self) -> None:
         shutil.rmtree(self.root_path)
 
     def create_keyfile(self):
-        keyfile = keyfile(path=os.path.join(self.root_path, "keyfile"))
+        _keyfile = keyfile(path=os.path.join(self.root_path, "keyfile"))
 
         mnemonic = Keypair.generate_mnemonic(12)
         alice = Keypair.create_from_mnemonic(mnemonic)
-        keyfile.set_keypair(alice, encrypt=True, overwrite=True, password='thisisafakepassword')
+        _keyfile.set_keypair(alice, encrypt=True, overwrite=True, password='thisisafakepassword')
 
         bob = Keypair.create_from_uri('/Bob')
-        keyfile.set_keypair(bob, encrypt=True, overwrite=True, password='thisisafakepassword')
+        _keyfile.set_keypair(bob, encrypt=True, overwrite=True, password='thisisafakepassword')
 
         return keyfile
 
     def test_create(self):
-        keyfile = keyfile(path=os.path.join(self.root_path, "keyfile"))
+        _keyfile = keyfile(path=os.path.join(self.root_path, "keyfile"))
 
         mnemonic = Keypair.generate_mnemonic( 12 )
         alice = Keypair.create_from_mnemonic(mnemonic)
-        keyfile.set_keypair(alice, encrypt=True, overwrite=True, password = 'thisisafakepassword')
-        assert keyfile.is_readable()
-        assert keyfile.is_writable()
-        assert keyfile.is_encrypted()
-        keyfile.decrypt( password = 'thisisafakepassword' )
-        assert not keyfile.is_encrypted()
-        keyfile.encrypt( password = 'thisisafakepassword' )
-        assert keyfile.is_encrypted()
+        _keyfile.set_keypair(alice, encrypt=True, overwrite=True, password = 'thisisafakepassword')
+        assert _keyfile.is_readable()
+        assert _keyfile.is_writable()
+        assert _keyfile.is_encrypted()
+        _keyfile.decrypt( password = 'thisisafakepassword' )
+        assert not _keyfile.is_encrypted()
+        _keyfile.encrypt( password = 'thisisafakepassword' )
+        assert _keyfile.is_encrypted()
         str(keyfile)
-        keyfile.decrypt( password = 'thisisafakepassword' )
-        assert not keyfile.is_encrypted()
+        _keyfile.decrypt( password = 'thisisafakepassword' )
+        assert not _keyfile.is_encrypted()
         str(keyfile)
 
-        assert keyfile.get_keypair( password = 'thisisafakepassword' ).ss58_address == alice.ss58_address
-        assert keyfile.get_keypair( password = 'thisisafakepassword' ).private_key == alice.private_key
-        assert keyfile.get_keypair( password = 'thisisafakepassword' ).public_key == alice.public_key
+        assert _keyfile.get_keypair( password = 'thisisafakepassword' ).ss58_address == alice.ss58_address
+        assert _keyfile.get_keypair( password = 'thisisafakepassword' ).private_key == alice.private_key
+        assert _keyfile.get_keypair( password = 'thisisafakepassword' ).public_key == alice.public_key
 
         bob = Keypair.create_from_uri ('/Bob')
-        keyfile.set_keypair(bob, encrypt=True, overwrite=True, password = 'thisisafakepassword')
-        assert keyfile.get_keypair( password = 'thisisafakepassword' ).ss58_address == bob.ss58_address
-        assert keyfile.get_keypair( password = 'thisisafakepassword' ).public_key == bob.public_key
+        _keyfile.set_keypair(bob, encrypt=True, overwrite=True, password = 'thisisafakepassword')
+        assert _keyfile.get_keypair( password = 'thisisafakepassword' ).ss58_address == bob.ss58_address
+        assert _keyfile.get_keypair( password = 'thisisafakepassword' ).public_key == bob.public_key
 
         repr(keyfile)
 
     def test_legacy_coldkey(self):
         legacy_filename = os.path.join(self.root_path, "coldlegacy_keyfile")
-        keyfile = keyfile (path = legacy_filename)
-        keyfile.make_dirs()
+        _keyfile = keyfile (path = legacy_filename)
+        _keyfile.make_dirs()
         keyfile_data = b'0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f'
         with open(legacy_filename, "wb") as keyfile_obj:
             keyfile_obj.write( keyfile_data )
-        assert keyfile.keyfile_data == keyfile_data
-        keyfile.encrypt( password = 'this is the fake password' )
-        keyfile.decrypt( password = 'this is the fake password' )
+        assert _keyfile.keyfile_data == keyfile_data
+        _keyfile.encrypt( password = 'this is the fake password' )
+        _keyfile.decrypt( password = 'this is the fake password' )
         keypair_bytes = b'{"accountId": "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f", "publicKey": "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f", "secretPhrase": null, "secretSeed": null, "ss58Address": "5DD26kC2kxajmwfbbZmVmxhrY9VeeyR1Gpzy9i8wxLUg6zxm"}'
-        assert keyfile.keyfile_data == keypair_bytes
-        assert keyfile.get_keypair().ss58_address == "5DD26kC2kxajmwfbbZmVmxhrY9VeeyR1Gpzy9i8wxLUg6zxm"
-        assert "0x" + keyfile.get_keypair().public_key.hex() == "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f"
+        assert _keyfile.keyfile_data == keypair_bytes
+        assert _keyfile.get_keypair().ss58_address == "5DD26kC2kxajmwfbbZmVmxhrY9VeeyR1Gpzy9i8wxLUg6zxm"
+        assert "0x" + _keyfile.get_keypair().public_key.hex() == "0x32939b6abc4d81f02dff04d2b8d1d01cc8e71c5e4c7492e4fa6a238cdca3512f"
 
     def test_validate_password(self):
         assert validate_password(None) == False
         assert validate_password('passw0rd') == False
         assert validate_password('123456789') == False
         with patch('getpass.getpass',return_value='biTTensor'):
             assert validate_password('biTTensor') == True
@@ -215,27 +216,25 @@
         assert decrypted_data == data
 
     def test_user_interface(self):
         with patch('getpass.getpass', side_effect = ['pass', 'password', 'asdury3294y', 'asdury3294y']):
             assert ask_password_to_encrypt() == 'asdury3294y'
 
     def test_overwriting(self):
-        keyfile = keyfile (path = os.path.join(self.root_path, "keyfile"))
+        _keyfile = keyfile (path = os.path.join(self.root_path, "keyfile"))
         alice = Keypair.create_from_uri ('/Alice')
-        keyfile.set_keypair(alice, encrypt=True, overwrite=True, password = 'thisisafakepassword')
+        _keyfile.set_keypair(alice, encrypt=True, overwrite=True, password = 'thisisafakepassword')
         bob = Keypair.create_from_uri ('/Bob')
 
         with pytest.raises(KeyFileError) as pytest_wrapped_e:
             with patch('builtins.input', return_value = 'n'):
-                keyfile.set_keypair(bob, encrypt=True, overwrite=False, password = 'thisisafakepassword')
+                _keyfile.set_keypair(bob, encrypt=True, overwrite=False, password = 'thisisafakepassword')
 
     def test_keyfile_mock(self):
-        file = keyfile( _mock = True )
-        assert file.exists_on_device()
-        assert not file.is_encrypted()
-        assert file.is_readable()
-        assert file.data
-        assert file.keypair
-        file.set_keypair( keypair = Keypair.create_from_mnemonic( mnemonic = Keypair.generate_mnemonic() ))
-
-    def test_keyfile_mock_func(self):
-        file = keyfile.mock()
+        with patch('bittensor_wallet._keyfile.keyfile.__new__', return_value=MockKeyfile(path='/tmp/test-wallet/keyfile')):
+            file = keyfile( )
+            assert file.exists_on_device()
+            assert not file.is_encrypted()
+            assert file.is_readable()
+            assert file.data
+            assert file.keypair
+            file.set_keypair( keypair = Keypair.create_from_mnemonic( mnemonic = Keypair.generate_mnemonic() ))
```

### Comparing `bittensor-wallet-0.0.3/tests/test_keypair.py` & `bittensor-wallet-0.0.4/tests/test_keypair.py`

 * *Files identical despite different names*

