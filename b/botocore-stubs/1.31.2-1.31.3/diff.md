# Comparing `tmp/botocore_stubs-1.31.2.tar.gz` & `tmp/botocore_stubs-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore_stubs-1.31.2.tar", max compression
+gzip compressed data, was "botocore_stubs-1.31.3.tar", max compression
```

## Comparing `botocore_stubs-1.31.2.tar` & `botocore_stubs-1.31.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1071 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/LICENSE
--rw-r--r--   0        0        0     1465 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/README.md
--rw-r--r--   0        0        0      580 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/__init__.pyi
--rw-r--r--   0        0        0     2899 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/args.pyi
--rw-r--r--   0        0        0     4456 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/auth.pyi
--rw-r--r--   0        0        0     3668 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/awsrequest.pyi
--rw-r--r--   0        0        0     6109 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/client.pyi
--rw-r--r--   0        0        0     2334 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/compat.pyi
--rw-r--r--   0        0        0     2544 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/config.pyi
--rw-r--r--   0        0        0      274 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/configloader.pyi
--rw-r--r--   0        0        0     3851 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/configprovider.pyi
--rw-r--r--   0        0        0    10732 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/credentials.pyi
--rw-r--r--   0        0        0       74 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/crt/__init__.pyi
--rw-r--r--   0        0        0     2144 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/crt/auth.pyi
--rw-r--r--   0        0        0     2234 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/discovery.pyi
--rw-r--r--   0        0        0     2233 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/endpoint.pyi
--rw-r--r--   0        0        0     6085 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/endpoint_provider.pyi
--rw-r--r--   0        0        0      708 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/errorfactory.pyi
--rw-r--r--   0        0        0     3462 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/eventstream.pyi
--rw-r--r--   0        0        0    21599 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/exceptions.pyi
--rw-r--r--   0        0        0     6869 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/handlers.pyi
--rw-r--r--   0        0        0      570 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/history.pyi
--rw-r--r--   0        0        0     2841 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/hooks.pyi
--rw-r--r--   0        0        0     2726 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/httpchecksum.pyi
--rw-r--r--   0        0        0     2055 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/httpsession.pyi
--rw-r--r--   0        0        0     2058 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/loaders.pyi
--rw-r--r--   0        0        0     6318 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/model.pyi
--rw-r--r--   0        0        0     2358 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/monitoring.pyi
--rw-r--r--   0        0        0     1743 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/paginate.pyi
--rw-r--r--   0        0        0     2099 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/parsers.pyi
--rw-r--r--   0        0        0        0 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/py.typed
--rw-r--r--   0        0        0     3246 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/regions.pyi
--rw-r--r--   0        0        0     1081 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/response.pyi
--rw-r--r--   0        0        0        0 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/__init__.pyi
--rw-r--r--   0        0        0      854 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/adaptive.pyi
--rw-r--r--   0        0        0      185 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/base.pyi
--rw-r--r--   0        0        0      652 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/bucket.pyi
--rw-r--r--   0        0        0      348 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/quota.pyi
--rw-r--r--   0        0        0      367 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/special.pyi
--rw-r--r--   0        0        0     3756 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/standard.pyi
--rw-r--r--   0        0        0      485 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/throttling.pyi
--rw-r--r--   0        0        0     2522 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retryhandler.pyi
--rw-r--r--   0        0        0     1759 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/serialize.pyi
--rw-r--r--   0        0        0     7218 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/session.pyi
--rw-r--r--   0        0        0     3533 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/signers.pyi
--rw-r--r--   0        0        0     1933 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/stub.pyi
--rw-r--r--   0        0        0     1198 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/tokens.pyi
--rw-r--r--   0        0        0      310 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/translate.pyi
--rw-r--r--   0        0        0     1110 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/useragent.pyi
--rw-r--r--   0        0        0    12306 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/utils.pyi
--rw-r--r--   0        0        0     1163 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/validate.pyi
--rw-r--r--   0        0        0     1587 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/waiter.pyi
--rw-r--r--   0        0        0     2788 2023-07-13 17:32:50.324773 botocore_stubs-1.31.2/pyproject.toml
--rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 botocore_stubs-1.31.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/LICENSE
+-rw-r--r--   0        0        0     1465 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/README.md
+-rw-r--r--   0        0        0      580 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2899 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/args.pyi
+-rw-r--r--   0        0        0     4456 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/auth.pyi
+-rw-r--r--   0        0        0     3668 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/awsrequest.pyi
+-rw-r--r--   0        0        0     6109 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/client.pyi
+-rw-r--r--   0        0        0     2334 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/compat.pyi
+-rw-r--r--   0        0        0     2544 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/config.pyi
+-rw-r--r--   0        0        0      274 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/configloader.pyi
+-rw-r--r--   0        0        0     3851 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/configprovider.pyi
+-rw-r--r--   0        0        0    10732 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/credentials.pyi
+-rw-r--r--   0        0        0       74 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/crt/__init__.pyi
+-rw-r--r--   0        0        0     2144 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/crt/auth.pyi
+-rw-r--r--   0        0        0     2234 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/discovery.pyi
+-rw-r--r--   0        0        0     2233 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/endpoint.pyi
+-rw-r--r--   0        0        0     6085 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/endpoint_provider.pyi
+-rw-r--r--   0        0        0      708 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/errorfactory.pyi
+-rw-r--r--   0        0        0     3462 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/eventstream.pyi
+-rw-r--r--   0        0        0    21599 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     6869 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/handlers.pyi
+-rw-r--r--   0        0        0      570 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/history.pyi
+-rw-r--r--   0        0        0     2841 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/hooks.pyi
+-rw-r--r--   0        0        0     2726 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/httpchecksum.pyi
+-rw-r--r--   0        0        0     2055 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/httpsession.pyi
+-rw-r--r--   0        0        0     2058 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/loaders.pyi
+-rw-r--r--   0        0        0     6318 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/model.pyi
+-rw-r--r--   0        0        0     2358 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/monitoring.pyi
+-rw-r--r--   0        0        0     1743 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/paginate.pyi
+-rw-r--r--   0        0        0     2099 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/parsers.pyi
+-rw-r--r--   0        0        0        0 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/py.typed
+-rw-r--r--   0        0        0     3246 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/regions.pyi
+-rw-r--r--   0        0        0     1081 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/response.pyi
+-rw-r--r--   0        0        0        0 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/__init__.pyi
+-rw-r--r--   0        0        0      854 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/adaptive.pyi
+-rw-r--r--   0        0        0      185 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/base.pyi
+-rw-r--r--   0        0        0      652 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/bucket.pyi
+-rw-r--r--   0        0        0      348 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/quota.pyi
+-rw-r--r--   0        0        0      367 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/special.pyi
+-rw-r--r--   0        0        0     3756 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/standard.pyi
+-rw-r--r--   0        0        0      485 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retries/throttling.pyi
+-rw-r--r--   0        0        0     2522 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/retryhandler.pyi
+-rw-r--r--   0        0        0     1759 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/serialize.pyi
+-rw-r--r--   0        0        0     7218 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/session.pyi
+-rw-r--r--   0        0        0     3533 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/signers.pyi
+-rw-r--r--   0        0        0     1933 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/stub.pyi
+-rw-r--r--   0        0        0     1198 2023-07-13 20:13:54.480465 botocore_stubs-1.31.3/botocore-stubs/tokens.pyi
+-rw-r--r--   0        0        0      310 2023-07-13 20:13:54.484465 botocore_stubs-1.31.3/botocore-stubs/translate.pyi
+-rw-r--r--   0        0        0     1110 2023-07-13 20:13:54.484465 botocore_stubs-1.31.3/botocore-stubs/useragent.pyi
+-rw-r--r--   0        0        0    12306 2023-07-13 20:13:54.484465 botocore_stubs-1.31.3/botocore-stubs/utils.pyi
+-rw-r--r--   0        0        0     1163 2023-07-13 20:13:54.484465 botocore_stubs-1.31.3/botocore-stubs/validate.pyi
+-rw-r--r--   0        0        0     1587 2023-07-13 20:13:54.484465 botocore_stubs-1.31.3/botocore-stubs/waiter.pyi
+-rw-r--r--   0        0        0     2788 2023-07-13 20:14:23.552945 botocore_stubs-1.31.3/pyproject.toml
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 botocore_stubs-1.31.3/PKG-INFO
```

### Comparing `botocore_stubs-1.31.2/LICENSE` & `botocore_stubs-1.31.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/README.md` & `botocore_stubs-1.31.3/README.md`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/__init__.pyi` & `botocore_stubs-1.31.3/botocore-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/args.pyi` & `botocore_stubs-1.31.3/botocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/auth.pyi` & `botocore_stubs-1.31.3/botocore-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/awsrequest.pyi` & `botocore_stubs-1.31.3/botocore-stubs/awsrequest.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/client.pyi` & `botocore_stubs-1.31.3/botocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/compat.pyi` & `botocore_stubs-1.31.3/botocore-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/config.pyi` & `botocore_stubs-1.31.3/botocore-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/configprovider.pyi` & `botocore_stubs-1.31.3/botocore-stubs/configprovider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/credentials.pyi` & `botocore_stubs-1.31.3/botocore-stubs/credentials.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/crt/auth.pyi` & `botocore_stubs-1.31.3/botocore-stubs/crt/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/discovery.pyi` & `botocore_stubs-1.31.3/botocore-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/endpoint.pyi` & `botocore_stubs-1.31.3/botocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/endpoint_provider.pyi` & `botocore_stubs-1.31.3/botocore-stubs/endpoint_provider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/errorfactory.pyi` & `botocore_stubs-1.31.3/botocore-stubs/errorfactory.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/eventstream.pyi` & `botocore_stubs-1.31.3/botocore-stubs/eventstream.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/exceptions.pyi` & `botocore_stubs-1.31.3/botocore-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/handlers.pyi` & `botocore_stubs-1.31.3/botocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/history.pyi` & `botocore_stubs-1.31.3/botocore-stubs/history.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/hooks.pyi` & `botocore_stubs-1.31.3/botocore-stubs/hooks.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/httpchecksum.pyi` & `botocore_stubs-1.31.3/botocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/httpsession.pyi` & `botocore_stubs-1.31.3/botocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/loaders.pyi` & `botocore_stubs-1.31.3/botocore-stubs/loaders.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/model.pyi` & `botocore_stubs-1.31.3/botocore-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/monitoring.pyi` & `botocore_stubs-1.31.3/botocore-stubs/monitoring.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/paginate.pyi` & `botocore_stubs-1.31.3/botocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/parsers.pyi` & `botocore_stubs-1.31.3/botocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/regions.pyi` & `botocore_stubs-1.31.3/botocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/response.pyi` & `botocore_stubs-1.31.3/botocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/retries/adaptive.pyi` & `botocore_stubs-1.31.3/botocore-stubs/retries/adaptive.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/retries/bucket.pyi` & `botocore_stubs-1.31.3/botocore-stubs/retries/bucket.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/retries/standard.pyi` & `botocore_stubs-1.31.3/botocore-stubs/retries/standard.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/retryhandler.pyi` & `botocore_stubs-1.31.3/botocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/serialize.pyi` & `botocore_stubs-1.31.3/botocore-stubs/serialize.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/session.pyi` & `botocore_stubs-1.31.3/botocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/signers.pyi` & `botocore_stubs-1.31.3/botocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/stub.pyi` & `botocore_stubs-1.31.3/botocore-stubs/stub.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/tokens.pyi` & `botocore_stubs-1.31.3/botocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/useragent.pyi` & `botocore_stubs-1.31.3/botocore-stubs/useragent.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/utils.pyi` & `botocore_stubs-1.31.3/botocore-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/validate.pyi` & `botocore_stubs-1.31.3/botocore-stubs/validate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/botocore-stubs/waiter.pyi` & `botocore_stubs-1.31.3/botocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.31.2/pyproject.toml` & `botocore_stubs-1.31.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "botocore-stubs"
-version = "1.31.2"
+version = "1.31.3"
 description = "Type annotations and code completion for botocore"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/botocore-stubs"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `botocore_stubs-1.31.2/PKG-INFO` & `botocore_stubs-1.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-stubs
-Version: 1.31.2
+Version: 1.31.3
 Summary: Type annotations and code completion for botocore
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: botocore,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
```

