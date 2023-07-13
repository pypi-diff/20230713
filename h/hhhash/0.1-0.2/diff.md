# Comparing `tmp/hhhash-0.1.tar.gz` & `tmp/hhhash-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhhash-0.1.tar", max compression
+gzip compressed data, was "hhhash-0.2.tar", max compression
```

## Comparing `hhhash-0.1.tar` & `hhhash-0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-07-09 07:27:28.367522 hhhash-0.1/LICENSE
--rw-r--r--   0        0        0     1583 2023-07-09 08:17:49.742277 hhhash-0.1/README.md
--rw-r--r--   0        0        0       36 2023-07-09 07:47:48.981985 hhhash-0.1/hhhash/__init__.py
--rw-r--r--   0        0        0      383 2023-07-09 08:13:17.402079 hhhash-0.1/hhhash/create.py
--rw-r--r--   0        0        0      595 2023-07-09 07:42:01.592693 hhhash-0.1/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 hhhash-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-10 11:25:26.452101 hhhash-0.2/LICENSE
+-rw-r--r--   0        0        0     2524 2023-07-10 11:28:30.378592 hhhash-0.2/README.md
+-rw-r--r--   0        0        0       36 2023-07-10 11:25:26.452101 hhhash-0.2/hhhash/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-13 06:51:19.881264 hhhash-0.2/hhhash/create.py
+-rw-r--r--   0        0        0      595 2023-07-13 06:52:09.444804 hhhash-0.2/pyproject.toml
+-rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 hhhash-0.2/setup.py
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 hhhash-0.2/PKG-INFO
```

### Comparing `hhhash-0.1/LICENSE` & `hhhash-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hhhash-0.1/README.md` & `hhhash-0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # HTTP Headers Hashing (HHHash)
 
-HTTP Headers Hashing (HHHash) is a technique used to create a fingerprint of an HTTP server based on the headers it returns. HHHash employs one-way hashing to generate a hash value for the set of header keys returned by the server
+HTTP Headers Hashing (HHHash) is a technique used to create a fingerprint of an HTTP server based on the headers it returns. HHHash employs one-way hashing to generate a hash value for the set of header keys returned by the server.
+
+For more details about HHHash background, [HTTP Headers Hashing (HHHash) or improving correlation of crawled content](https://www.foo.be/2023/07/HTTP-Headers-Hashing_HHHash).
 
 ## Calculation of the HHHash
 
 To calculate the HHHash, we concatenate the list of headers returned by the HTTP server. This list is ordered according to the sequence in which the headers appear in the server's response. Each header value is separated with `:`. 
 
 The HHHash value is the SHA256 of the list.
 
@@ -23,15 +25,23 @@
 ~~~
 
 Output value
 ~~~
 hhh:1:78f7ef0651bac1a5ea42ed9d22242ed8725f07815091032a34ab4e30d3c3cefc
 ~~~
 
-### Python Library
+## Limitations 
+
+HHHash is an effective technique; however, its performance is heavily reliant on the characteristics of the HTTP client requests. Therefore, it is important to note that correlations between a set of hashes are typically established when using the same crawler or HTTP client parameters.
+
+### hhhash - Python Library
+
+The [hhhash package](https://pypi.org/project/hhhash/) can be installed via a `pip install hhhash` or build with Poetry from this repository `poetry build` and `poetry install`.
+
+#### Usage
 
 ~~~ipython
 In [1]: import hhhash
 
 In [2]: hhhash.buildhash(url="https://www.misp-lea.org", debug=False)
 Out[2]: 'hhh:1:adca8a87f2a537dbbf07ba6d8cba6db53fde257ae2da4dad6f3ee6b47080c53f'
 
@@ -39,7 +49,13 @@
 Out[3]: 'hhh:1:adca8a87f2a537dbbf07ba6d8cba6db53fde257ae2da4dad6f3ee6b47080c53f'
 
 In [4]: hhhash.buildhash(url="https://www.circl.lu", debug=False)
 Out[4]: 'hhh:1:334d8ab68f9e935f3af7c4a91220612f980f2d9168324530c03d28c9429e1299'
 
 In [5]:
 ~~~
+
+## Other libraries
+
+- [c-hhhash](https://github.com/hrbrmstr/c-hhhash) - C++ HTTP Headers Hashing CLI
+- [go-hhhash](https://github.com/hrbrmstr/go-hhhash) - golang HTTP Headers Hashing CLI
+- [R hhhash](https://github.com/hrbrmstr/hhhash) - R library HHHash
```

### Comparing `hhhash-0.1/pyproject.toml` & `hhhash-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #[build-system]
 #requires = ["setuptools>=61.0"]
 #build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "HHHash"
-version = "0.1"
+version = "0.2"
 authors = [
     "Alexandre Dulaunoy <a@foo.be>"
 ]
 description = "HHHash library is calculate HHHash from HTTP servers."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `hhhash-0.1/PKG-INFO` & `hhhash-0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: hhhash
-Version: 0.1
+Version: 0.2
 Summary: HHHash library is calculate HHHash from HTTP servers.
 Home-page: https://github.com/adulau/HHHash
 Author: Alexandre Dulaunoy
 Author-email: a@foo.be
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Project-URL: Repository, https://github.com/adulau/HHHash/issues
 Description-Content-Type: text/markdown
 
 # HTTP Headers Hashing (HHHash)
 
-HTTP Headers Hashing (HHHash) is a technique used to create a fingerprint of an HTTP server based on the headers it returns. HHHash employs one-way hashing to generate a hash value for the set of header keys returned by the server
+HTTP Headers Hashing (HHHash) is a technique used to create a fingerprint of an HTTP server based on the headers it returns. HHHash employs one-way hashing to generate a hash value for the set of header keys returned by the server.
+
+For more details about HHHash background, [HTTP Headers Hashing (HHHash) or improving correlation of crawled content](https://www.foo.be/2023/07/HTTP-Headers-Hashing_HHHash).
 
 ## Calculation of the HHHash
 
 To calculate the HHHash, we concatenate the list of headers returned by the HTTP server. This list is ordered according to the sequence in which the headers appear in the server's response. Each header value is separated with `:`. 
 
 The HHHash value is the SHA256 of the list.
 
@@ -44,15 +47,23 @@
 ~~~
 
 Output value
 ~~~
 hhh:1:78f7ef0651bac1a5ea42ed9d22242ed8725f07815091032a34ab4e30d3c3cefc
 ~~~
 
-### Python Library
+## Limitations 
+
+HHHash is an effective technique; however, its performance is heavily reliant on the characteristics of the HTTP client requests. Therefore, it is important to note that correlations between a set of hashes are typically established when using the same crawler or HTTP client parameters.
+
+### hhhash - Python Library
+
+The [hhhash package](https://pypi.org/project/hhhash/) can be installed via a `pip install hhhash` or build with Poetry from this repository `poetry build` and `poetry install`.
+
+#### Usage
 
 ~~~ipython
 In [1]: import hhhash
 
 In [2]: hhhash.buildhash(url="https://www.misp-lea.org", debug=False)
 Out[2]: 'hhh:1:adca8a87f2a537dbbf07ba6d8cba6db53fde257ae2da4dad6f3ee6b47080c53f'
 
@@ -61,7 +72,13 @@
 
 In [4]: hhhash.buildhash(url="https://www.circl.lu", debug=False)
 Out[4]: 'hhh:1:334d8ab68f9e935f3af7c4a91220612f980f2d9168324530c03d28c9429e1299'
 
 In [5]:
 ~~~
 
+## Other libraries
+
+- [c-hhhash](https://github.com/hrbrmstr/c-hhhash) - C++ HTTP Headers Hashing CLI
+- [go-hhhash](https://github.com/hrbrmstr/go-hhhash) - golang HTTP Headers Hashing CLI
+- [R hhhash](https://github.com/hrbrmstr/hhhash) - R library HHHash
+
```

