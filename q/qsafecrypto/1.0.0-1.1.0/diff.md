# Comparing `tmp/qsafecrypto-1.0.0.tar.gz` & `tmp/qsafecrypto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsafecrypto-1.0.0.tar", last modified: Mon Jul 10 13:05:46 2023, max compression
+gzip compressed data, was "qsafecrypto-1.1.0.tar", last modified: Thu Jul 13 19:01:03 2023, max compression
```

## Comparing `qsafecrypto-1.0.0.tar` & `qsafecrypto-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 13:05:46.820616 qsafecrypto-1.0.0/
--rw-rw-rw-   0        0        0     1199 2023-07-10 12:28:04.000000 qsafecrypto-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3344 2023-07-10 13:05:46.813825 qsafecrypto-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2712 2023-07-10 12:29:49.000000 qsafecrypto-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 13:05:46.786741 qsafecrypto-1.0.0/qsafecrypto/
--rw-rw-rw-   0        0        0        0 2023-07-06 15:14:09.000000 qsafecrypto-1.0.0/qsafecrypto/__init__.py
--rw-rw-rw-   0        0        0     4026 2023-07-09 15:14:33.000000 qsafecrypto-1.0.0/qsafecrypto/aes_gcm_256.py
--rw-rw-rw-   0        0        0      461 2023-07-10 11:51:14.000000 qsafecrypto-1.0.0/qsafecrypto/random.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:05:46.805478 qsafecrypto-1.0.0/qsafecrypto.egg-info/
--rw-rw-rw-   0        0        0     3344 2023-07-10 13:05:46.000000 qsafecrypto-1.0.0/qsafecrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-10 13:05:46.000000 qsafecrypto-1.0.0/qsafecrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 13:05:46.000000 qsafecrypto-1.0.0/qsafecrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-10 13:05:46.000000 qsafecrypto-1.0.0/qsafecrypto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-10 13:05:46.000000 qsafecrypto-1.0.0/qsafecrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 13:05:46.820616 qsafecrypto-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-07-10 11:37:04.000000 qsafecrypto-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 13:05:46.809805 qsafecrypto-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-06 15:08:02.000000 qsafecrypto-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1810 2023-07-10 11:53:09.000000 qsafecrypto-1.0.0/tests/test_crypto.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:01:03.883889 qsafecrypto-1.1.0/
+-rw-rw-rw-   0        0        0     1199 2023-07-10 12:28:04.000000 qsafecrypto-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    12777 2023-07-13 19:01:03.858914 qsafecrypto-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12117 2023-07-13 19:00:16.000000 qsafecrypto-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 19:01:03.748860 qsafecrypto-1.1.0/qsafecrypto/
+-rw-rw-rw-   0        0        0        0 2023-07-06 15:14:09.000000 qsafecrypto-1.1.0/qsafecrypto/__init__.py
+-rw-rw-rw-   0        0        0     3498 2023-07-13 19:00:40.000000 qsafecrypto-1.1.0/qsafecrypto/aes_gcm_256.py
+-rw-rw-rw-   0        0        0     1616 2023-07-11 14:58:54.000000 qsafecrypto-1.1.0/qsafecrypto/util.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:01:03.825646 qsafecrypto-1.1.0/qsafecrypto.egg-info/
+-rw-rw-rw-   0        0        0    12777 2023-07-13 19:01:03.000000 qsafecrypto-1.1.0/qsafecrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-13 19:01:03.000000 qsafecrypto-1.1.0/qsafecrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:01:03.000000 qsafecrypto-1.1.0/qsafecrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-13 19:01:03.000000 qsafecrypto-1.1.0/qsafecrypto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-13 19:01:03.000000 qsafecrypto-1.1.0/qsafecrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 19:01:03.886581 qsafecrypto-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-07-13 18:09:59.000000 qsafecrypto-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:01:03.839831 qsafecrypto-1.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-06 15:08:02.000000 qsafecrypto-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-07-11 14:55:11.000000 qsafecrypto-1.1.0/tests/test_crypto.py
```

### Comparing `qsafecrypto-1.0.0/LICENSE` & `qsafecrypto-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qsafecrypto-1.0.0/qsafecrypto/aes_gcm_256.py` & `qsafecrypto-1.1.0/qsafecrypto/aes_gcm_256.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from Crypto.Cipher import AES
 from Crypto.Random import get_random_bytes
 import based58
 
 # AES has never been cracked yet and it would take large amounts of computational power to crack this key.
-# https://www.appsealing.com/aes-128-encryption/#:~:text=A%20machine%20that%20can%20crack,power%20to%20crack%20this%20key.
 
 def encrypt(payload, key, verification_key, decode=True):
     """
     Encrypts the given data payload using AES-GCM-256 encryption.
 
     Args:
         payload (str | bytes): The data to be encrypted, either as a string or bytes.
@@ -30,15 +29,15 @@
         raise ValueError("Incorrect AES-GCM-256 key length ({0} bytes). Only 32-byte key length is supported for 256-bit encryption. Qsafecrypto currently supports only AES-GCM-256 as it is deemed to be quantum-safe. AES-GCM-192 & AES-GCM-128 are not supported by choice.".format(len(key)))
 
     data = payload.encode() if isinstance(payload, str) else payload
 
     nonce = get_random_bytes(12)
     
     ciphertext, verification_key = AES.new(key.encode(), AES.MODE_GCM, nonce=nonce).update(verification_key.encode()).encrypt_and_digest(data)
-
+    
     if decode:
         return based58.b58encode(nonce+ciphertext+verification_key).decode()
     else:
         return based58.b58encode(nonce+ciphertext+verification_key)
 
 
 def decrypt(payload, key, verification_key, decode=True):
@@ -68,24 +67,7 @@
     byte_convert = based58.b58decode(payload.encode() if isinstance(payload, str) else payload)
  
     if decode:
         return AES.new(key.encode(), AES.MODE_GCM, nonce=byte_convert[0:12]).update(verification_key.encode()).decrypt_and_verify(byte_convert[12:-16], byte_convert[-16:]).decode()
     else:
         return AES.new(key.encode(), AES.MODE_GCM, nonce=byte_convert[0:12]).update(verification_key.encode()).decrypt_and_verify(byte_convert[12:-16], byte_convert[-16:])
 
-
-def generate_random_key(length=32):
-    """
-    Generate a random encryption key.
-
-    Args:
-        length (int): Length of the random key desired.
-
-    Returns:
-        str: A random encryption key.
-
-    Note:
-        Generates a secure random key.
-    """
-    random_bytes = get_random_bytes(length)
-    random_key = based58.b58encode(random_bytes).decode()[:length]
-    return random_key
```

### Comparing `qsafecrypto-1.0.0/setup.py` & `qsafecrypto-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="qsafecrypto",
-    version="1.0.0",
+    version="1.1.0",
     author="Md Fazlul Karim",
     author_email="fazlulkarimrocky@gmail.com",
     description="A secure and user-friendly open-source cryptography library, offering modern cryptographic APIs that are resistant to quantum attacks. Protect your data with ease and confidence using advanced quantum-resistant algorithms",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/mindreadio/qsafecrypto",
     packages=find_packages(),
@@ -15,8 +15,9 @@
         "pycryptodome>=3.17.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    python_requires=">=3.7",
 )
```

