# Comparing `tmp/botocore_stubs-1.29.99.tar.gz` & `tmp/botocore_stubs-1.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore_stubs-1.29.99.tar", max compression
+gzip compressed data, was "botocore_stubs-1.31.2.tar", max compression
```

## Comparing `botocore_stubs-1.29.99.tar` & `botocore_stubs-1.31.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     1071 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/LICENSE
--rw-r--r--   0        0        0     1465 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/README.md
--rw-r--r--   0        0        0      580 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/__init__.pyi
--rw-r--r--   0        0        0     2763 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/args.pyi
--rw-r--r--   0        0        0     4456 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/auth.pyi
--rw-r--r--   0        0        0     3668 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/awsrequest.pyi
--rw-r--r--   0        0        0     5940 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/client.pyi
--rw-r--r--   0        0        0     2334 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/compat.pyi
--rw-r--r--   0        0        0     2544 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/config.pyi
--rw-r--r--   0        0        0      274 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/configloader.pyi
--rw-r--r--   0        0        0     3528 2023-03-24 20:12:15.565131 botocore_stubs-1.29.99/botocore-stubs/configprovider.pyi
--rw-r--r--   0        0        0    11104 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/credentials.pyi
--rw-r--r--   0        0        0       74 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/crt/__init__.pyi
--rw-r--r--   0        0        0     2144 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/crt/auth.pyi
--rw-r--r--   0        0        0     2234 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/discovery.pyi
--rw-r--r--   0        0        0     2233 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/endpoint.pyi
--rw-r--r--   0        0        0     6085 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/endpoint_provider.pyi
--rw-r--r--   0        0        0      708 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/errorfactory.pyi
--rw-r--r--   0        0        0     2905 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/eventstream.pyi
--rw-r--r--   0        0        0    21599 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/exceptions.pyi
--rw-r--r--   0        0        0     6777 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/handlers.pyi
--rw-r--r--   0        0        0      570 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/history.pyi
--rw-r--r--   0        0        0     2841 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/hooks.pyi
--rw-r--r--   0        0        0     2726 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/httpchecksum.pyi
--rw-r--r--   0        0        0     2055 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/httpsession.pyi
--rw-r--r--   0        0        0     2058 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/loaders.pyi
--rw-r--r--   0        0        0     6318 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/model.pyi
--rw-r--r--   0        0        0     2358 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/monitoring.pyi
--rw-r--r--   0        0        0     1743 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/paginate.pyi
--rw-r--r--   0        0        0     2099 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/parsers.pyi
--rw-r--r--   0        0        0        0 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/py.typed
--rw-r--r--   0        0        0     3246 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/regions.pyi
--rw-r--r--   0        0        0     1081 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/response.pyi
--rw-r--r--   0        0        0        0 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/__init__.pyi
--rw-r--r--   0        0        0      854 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/adaptive.pyi
--rw-r--r--   0        0        0      185 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/base.pyi
--rw-r--r--   0        0        0      652 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/bucket.pyi
--rw-r--r--   0        0        0      348 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/quota.pyi
--rw-r--r--   0        0        0      367 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/special.pyi
--rw-r--r--   0        0        0     3756 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/standard.pyi
--rw-r--r--   0        0        0      485 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retries/throttling.pyi
--rw-r--r--   0        0        0     2522 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/retryhandler.pyi
--rw-r--r--   0        0        0     1721 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/serialize.pyi
--rw-r--r--   0        0        0     7208 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/session.pyi
--rw-r--r--   0        0        0     3544 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/signers.pyi
--rw-r--r--   0        0        0     1933 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/stub.pyi
--rw-r--r--   0        0        0     1204 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/tokens.pyi
--rw-r--r--   0        0        0      310 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/translate.pyi
--rw-r--r--   0        0        0    11812 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/utils.pyi
--rw-r--r--   0        0        0     1163 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/validate.pyi
--rw-r--r--   0        0        0     1587 2023-03-24 20:12:15.569131 botocore_stubs-1.29.99/botocore-stubs/waiter.pyi
--rw-r--r--   0        0        0     2789 2023-03-24 20:12:42.566130 botocore_stubs-1.29.99/pyproject.toml
--rw-r--r--   0        0        0     3333 1970-01-01 00:00:00.000000 botocore_stubs-1.29.99/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/LICENSE
+-rw-r--r--   0        0        0     1465 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/README.md
+-rw-r--r--   0        0        0      580 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/__init__.pyi
+-rw-r--r--   0        0        0     2899 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/args.pyi
+-rw-r--r--   0        0        0     4456 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/auth.pyi
+-rw-r--r--   0        0        0     3668 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/awsrequest.pyi
+-rw-r--r--   0        0        0     6109 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/client.pyi
+-rw-r--r--   0        0        0     2334 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/compat.pyi
+-rw-r--r--   0        0        0     2544 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/config.pyi
+-rw-r--r--   0        0        0      274 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/configloader.pyi
+-rw-r--r--   0        0        0     3851 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/configprovider.pyi
+-rw-r--r--   0        0        0    10732 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/credentials.pyi
+-rw-r--r--   0        0        0       74 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/crt/__init__.pyi
+-rw-r--r--   0        0        0     2144 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/crt/auth.pyi
+-rw-r--r--   0        0        0     2234 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/discovery.pyi
+-rw-r--r--   0        0        0     2233 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/endpoint.pyi
+-rw-r--r--   0        0        0     6085 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/endpoint_provider.pyi
+-rw-r--r--   0        0        0      708 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/errorfactory.pyi
+-rw-r--r--   0        0        0     3462 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/eventstream.pyi
+-rw-r--r--   0        0        0    21599 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     6869 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/handlers.pyi
+-rw-r--r--   0        0        0      570 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/history.pyi
+-rw-r--r--   0        0        0     2841 2023-07-13 17:32:24.872748 botocore_stubs-1.31.2/botocore-stubs/hooks.pyi
+-rw-r--r--   0        0        0     2726 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/httpchecksum.pyi
+-rw-r--r--   0        0        0     2055 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/httpsession.pyi
+-rw-r--r--   0        0        0     2058 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/loaders.pyi
+-rw-r--r--   0        0        0     6318 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/model.pyi
+-rw-r--r--   0        0        0     2358 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/monitoring.pyi
+-rw-r--r--   0        0        0     1743 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/paginate.pyi
+-rw-r--r--   0        0        0     2099 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/parsers.pyi
+-rw-r--r--   0        0        0        0 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/py.typed
+-rw-r--r--   0        0        0     3246 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/regions.pyi
+-rw-r--r--   0        0        0     1081 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/response.pyi
+-rw-r--r--   0        0        0        0 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/__init__.pyi
+-rw-r--r--   0        0        0      854 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/adaptive.pyi
+-rw-r--r--   0        0        0      185 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/base.pyi
+-rw-r--r--   0        0        0      652 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/bucket.pyi
+-rw-r--r--   0        0        0      348 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/quota.pyi
+-rw-r--r--   0        0        0      367 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/special.pyi
+-rw-r--r--   0        0        0     3756 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/standard.pyi
+-rw-r--r--   0        0        0      485 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retries/throttling.pyi
+-rw-r--r--   0        0        0     2522 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/retryhandler.pyi
+-rw-r--r--   0        0        0     1759 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/serialize.pyi
+-rw-r--r--   0        0        0     7218 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/session.pyi
+-rw-r--r--   0        0        0     3533 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/signers.pyi
+-rw-r--r--   0        0        0     1933 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/stub.pyi
+-rw-r--r--   0        0        0     1198 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/tokens.pyi
+-rw-r--r--   0        0        0      310 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/translate.pyi
+-rw-r--r--   0        0        0     1110 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/useragent.pyi
+-rw-r--r--   0        0        0    12306 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/utils.pyi
+-rw-r--r--   0        0        0     1163 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/validate.pyi
+-rw-r--r--   0        0        0     1587 2023-07-13 17:32:24.876748 botocore_stubs-1.31.2/botocore-stubs/waiter.pyi
+-rw-r--r--   0        0        0     2788 2023-07-13 17:32:50.324773 botocore_stubs-1.31.2/pyproject.toml
+-rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 botocore_stubs-1.31.2/PKG-INFO
```

### Comparing `botocore_stubs-1.29.99/LICENSE` & `botocore_stubs-1.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/README.md` & `botocore_stubs-1.31.2/README.md`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/__init__.pyi` & `botocore_stubs-1.31.2/botocore-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/args.pyi` & `botocore_stubs-1.31.2/botocore-stubs/args.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 from botocore.endpoint import EndpointCreator as EndpointCreator
 from botocore.hooks import BaseEventHooks
 from botocore.loaders import Loader
 from botocore.model import ServiceModel
 from botocore.parsers import ResponseParser, ResponseParserFactory
 from botocore.serialize import BaseRestSerializer
 from botocore.signers import RequestSigner as RequestSigner
+from botocore.useragent import UserAgentString
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 logger: Logger = ...
 
 VALID_REGIONAL_ENDPOINTS_CONFIG: List[str]
 LEGACY_GLOBAL_STS_REGIONS: List[str]
+USERAGENT_APPID_MAXLEN: int
 
 class _GetClientArgsTypeDef(TypedDict):
     serializer: BaseRestSerializer
     endpoint: Endpoint
     response_parser: ResponseParser
     event_emitter: BaseEventHooks
     request_signer: RequestSigner
@@ -41,14 +43,15 @@
         self,
         event_emitter: BaseEventHooks,
         user_agent: Any,
         response_parser_factory: ResponseParserFactory,
         loader: Loader,
         exceptions_factory: Any,
         config_store: ConfigValueStore,
+        user_agent_creator: Optional[UserAgentString] = ...,
     ) -> None: ...
     def get_client_args(
         self,
         service_model: ServiceModel,
         region_name: str,
         is_secure: bool,
         endpoint_url: Optional[str],
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/auth.pyi` & `botocore_stubs-1.31.2/botocore-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/awsrequest.pyi` & `botocore_stubs-1.31.2/botocore-stubs/awsrequest.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/client.pyi` & `botocore_stubs-1.31.2/botocore-stubs/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from botocore.model import ServiceModel as ServiceModel
 from botocore.paginate import Paginator as Paginator
 from botocore.regions import BaseEndpointResolver, EndpointRulesetResolver
 from botocore.retries import adaptive as adaptive
 from botocore.retries import standard as standard
 from botocore.serialize import Serializer
 from botocore.signers import RequestSigner
+from botocore.useragent import UserAgentString
 from botocore.utils import CachedProperty as CachedProperty
 from botocore.utils import S3ArnParamHandler as S3ArnParamHandler
 from botocore.utils import S3ControlArnParamHandler as S3ControlArnParamHandler
 from botocore.utils import S3ControlEndpointSetter as S3ControlEndpointSetter
 from botocore.utils import S3EndpointSetter as S3EndpointSetter
 from botocore.utils import S3RegionRedirector as S3RegionRedirector
 from botocore.utils import ensure_boolean as ensure_boolean
@@ -52,14 +53,15 @@
         user_agent: str,
         event_emitter: BaseEventHooks,
         retry_handler_factory: Any,
         retry_config_translator: Any,
         response_parser_factory: Optional[Any] = ...,
         exceptions_factory: Optional[Any] = ...,
         config_store: Optional[Any] = ...,
+        user_agent_creator: Optional[UserAgentString] = ...,
     ) -> None: ...
     def create_client(
         self,
         service_name: str,
         region_name: str,
         is_secure: bool = ...,
         endpoint_url: Optional[str] = ...,
@@ -109,14 +111,15 @@
         request_signer: RequestSigner,
         service_model: ServiceModel,
         loader: Loader,
         client_config: Config,
         partition: str,
         exceptions_factory: Any,
         endpoint_ruleset_resolver: Optional[EndpointRulesetResolver] = ...,
+        user_agent_creator: Optional[UserAgentString] = ...,
     ) -> None:
         self.meta: ClientMeta
     # FIXME: it hides `has no attribute` errors on Client type checking
     # def __getattr__(self, item: str) -> Any: ...
     def close(self) -> None: ...
     def get_paginator(self, operation_name: Any) -> Paginator: ...
     def can_paginate(self, operation_name: str) -> bool: ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/compat.pyi` & `botocore_stubs-1.31.2/botocore-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/config.pyi` & `botocore_stubs-1.31.2/botocore-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/configprovider.pyi` & `botocore_stubs-1.31.2/botocore-stubs/configprovider.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         default: Optional[Any] = ...,
         conversion_func: Optional[Any] = ...,
     ) -> Any: ...
 
 class ConfigValueStore:
     def __init__(self, mapping: Optional[Any] = ...) -> None: ...
     def __deepcopy__(self: _R, memo: Dict[str, Any]) -> _R: ...
+    def __copy__(self: _R) -> _R: ...
     def get_config_variable(self, logical_name: str) -> Any: ...
     def get_config_provider(self, logical_name: str) -> "BaseProvider": ...
     def set_config_variable(self, logical_name: str, value: Any) -> None: ...
     def clear_config_variable(self, logical_name: str) -> None: ...
     def set_config_provider(self, logical_name: str, provider: Any) -> None: ...
 
 class SmartDefaultsConfigStoreFactory:
@@ -84,7 +85,17 @@
     def provide(self) -> Any: ...
     def set_default_provider(self, key: str, default_provider: BaseProvider) -> None: ...
 
 class ConstantProvider(BaseProvider):
     def __init__(self, value: Any) -> None: ...
     def __deepcopy__(self: _R, memo: Dict[str, Any]) -> _R: ...
     def provide(self) -> Any: ...
+
+class ConfiguredEndpointProvider(BaseProvider):
+    def __init__(
+        self,
+        full_config: Dict[str, Any],
+        scoped_config: Dict[str, Any],
+        client_name: str,
+        environ: Optional[Dict[str, str]] = ...,
+    ) -> None: ...
+    def provide(self) -> Any: ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/credentials.pyi` & `botocore_stubs-1.31.2/botocore-stubs/credentials.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -47,22 +47,14 @@
         self, profile_name: str, disable_env_vars: bool = ...
     ) -> List[CredentialProvider]: ...
 
 def get_credentials(session: Session) -> Any: ...
 def create_assume_role_refresher(client: Any, params: Any) -> Any: ...
 def create_mfa_serial_refresher(actual_refresh: Any) -> Any: ...
 
-class JSONFileCache:
-    CACHE_DIR: Any = ...
-    def __init__(self, working_dir: Any = ..., dumps_func: Optional[Any] = ...) -> None: ...
-    def __contains__(self, cache_key: str) -> bool: ...
-    def __getitem__(self, cache_key: str) -> Any: ...
-    def __delitem__(self, cache_key: str) -> None: ...
-    def __setitem__(self, cache_key: str, value: Any) -> None: ...
-
 class Credentials:
     access_key: str = ...
     secret_key: str = ...
     token: str = ...
     method: str = ...
     def __init__(
         self,
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/crt/auth.pyi` & `botocore_stubs-1.31.2/botocore-stubs/crt/auth.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/discovery.pyi` & `botocore_stubs-1.31.2/botocore-stubs/discovery.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/endpoint.pyi` & `botocore_stubs-1.31.2/botocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/endpoint_provider.pyi` & `botocore_stubs-1.31.2/botocore-stubs/endpoint_provider.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/errorfactory.pyi` & `botocore_stubs-1.31.2/botocore-stubs/errorfactory.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/exceptions.pyi` & `botocore_stubs-1.31.2/botocore-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/handlers.pyi` & `botocore_stubs-1.31.2/botocore-stubs/handlers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,10 @@
 def remove_accid_host_prefix_from_model(
     params: Mapping[str, Any], model: Any, context: Any, **kwargs: Any
 ) -> None: ...
 def remove_arn_from_signing_path(request: Request, **kwargs: Any) -> None: ...
 def customize_endpoint_resolver_builtins(
     builtins: Mapping[str, Any], model: Any, params: Mapping[str, Any], context: Any, **kwargs: Any
 ) -> None: ...
+def remove_content_type_header_for_presigning(request: Request, **kwargs: Any) -> None: ...
 
 BUILTIN_HANDLERS: Any
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/history.pyi` & `botocore_stubs-1.31.2/botocore-stubs/history.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/hooks.pyi` & `botocore_stubs-1.31.2/botocore-stubs/hooks.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/httpchecksum.pyi` & `botocore_stubs-1.31.2/botocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/httpsession.pyi` & `botocore_stubs-1.31.2/botocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/loaders.pyi` & `botocore_stubs-1.31.2/botocore-stubs/loaders.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/model.pyi` & `botocore_stubs-1.31.2/botocore-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/monitoring.pyi` & `botocore_stubs-1.31.2/botocore-stubs/monitoring.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/paginate.pyi` & `botocore_stubs-1.31.2/botocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/parsers.pyi` & `botocore_stubs-1.31.2/botocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/regions.pyi` & `botocore_stubs-1.31.2/botocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/response.pyi` & `botocore_stubs-1.31.2/botocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/retries/adaptive.pyi` & `botocore_stubs-1.31.2/botocore-stubs/retries/adaptive.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/retries/bucket.pyi` & `botocore_stubs-1.31.2/botocore-stubs/retries/bucket.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/retries/standard.pyi` & `botocore_stubs-1.31.2/botocore-stubs/retries/standard.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/retryhandler.pyi` & `botocore_stubs-1.31.2/botocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/serialize.pyi` & `botocore_stubs-1.31.2/botocore-stubs/serialize.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, Mapping, Type
+from typing import Any, Dict, Mapping, Pattern, Type
 
 from botocore import validate as validate
 from botocore.compat import formatdate as formatdate
 from botocore.model import OperationModel
 from botocore.utils import is_json_value_header as is_json_value_header
 from botocore.utils import parse_to_aware_datetime as parse_to_aware_datetime
 from botocore.utils import percent_encode as percent_encode
 
 DEFAULT_TIMESTAMP_FORMAT: str
 ISO8601: str
 ISO8601_MICRO: str
+HOST_PREFIX_RE: Pattern[str]
 
 def create_serializer(protocol_name: str, include_validation: bool = ...) -> Any: ...
 
 class Serializer:
     DEFAULT_METHOD: str = ...
     MAP_TYPE: Type[Dict[str, Any]] = ...
     DEFAULT_ENCODING: str = ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/session.pyi` & `botocore_stubs-1.31.2/botocore-stubs/session.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     def register_component(self, name: Any, component: Any) -> None: ...
     def lazy_register_component(self, name: Any, component: Any) -> None: ...
     def create_client(
         self,
         service_name: str,
         region_name: Optional[str] = ...,
         api_version: Optional[str] = ...,
-        use_ssl: bool = ...,
+        use_ssl: Optional[bool] = ...,
         verify: Optional[Union[bool, str]] = ...,
         endpoint_url: Optional[str] = ...,
         aws_access_key_id: Optional[str] = ...,
         aws_secret_access_key: Optional[str] = ...,
         aws_session_token: Optional[str] = ...,
         config: Optional[Config] = ...,
     ) -> BaseClient: ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/signers.pyi` & `botocore_stubs-1.31.2/botocore-stubs/signers.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from botocore.awsrequest import create_request_object as create_request_object
 from botocore.awsrequest import prepare_request_dict as prepare_request_dict
 from botocore.compat import OrderedDict as OrderedDict
 from botocore.exceptions import UnknownClientMethodError as UnknownClientMethodError
 from botocore.exceptions import UnknownSignatureVersionError as UnknownSignatureVersionError
 from botocore.exceptions import UnsupportedSignatureVersionError as UnsupportedSignatureVersionError
 from botocore.hooks import BaseEventHooks
+from botocore.model import ServiceId
 from botocore.utils import datetime2timestamp as datetime2timestamp
-from botocore.utils import fix_s3_host as fix_s3_host
 
 class RequestSigner:
     def __init__(
         self,
-        service_id: str,
+        service_id: ServiceId,
         region_name: str,
         signing_name: str,
         signature_version: str,
         credentials: Any,
         event_emitter: BaseEventHooks,
         auth_token: Optional[str] = ...,
     ) -> None: ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/stub.pyi` & `botocore_stubs-1.31.2/botocore-stubs/stub.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/tokens.pyi` & `botocore_stubs-1.31.2/botocore-stubs/tokens.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import logging
 from typing import Any, Callable, Iterable, NamedTuple, Optional, Type
 
-from botocore.credentials import JSONFileCache
 from botocore.session import Session
+from botocore.utils import JSONFileCache
 
 logger: logging.Logger
 
 def create_token_resolver(session: Session) -> TokenProviderChain: ...
 
 class FrozenAuthToken(NamedTuple):
     token: str
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/utils.pyi` & `botocore_stubs-1.31.2/botocore-stubs/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from botocore.compat import get_md5 as get_md5
 from botocore.compat import get_tzinfo_options as get_tzinfo_options
 from botocore.compat import quote as quote
 from botocore.compat import urlparse as urlparse
 from botocore.compat import urlsplit as urlsplit
 from botocore.compat import urlunsplit as urlunsplit
 from botocore.compat import zip_longest as zip_longest
-from botocore.credentials import JSONFileCache as JSONFileCache
 from botocore.exceptions import ClientError as ClientError
 from botocore.exceptions import ConfigNotFound as ConfigNotFound
 from botocore.exceptions import ConnectionClosedError as ConnectionClosedError
 from botocore.exceptions import ConnectTimeoutError as ConnectTimeoutError
 from botocore.exceptions import EndpointConnectionError as EndpointConnectionError
 from botocore.exceptions import HTTPClientError as HTTPClientError
 from botocore.exceptions import InvalidDNSNameError as InvalidDNSNameError
@@ -158,14 +157,15 @@
     default_endpoint_url: Optional[str] = ...,
     **kwargs: Any,
 ) -> None: ...
 def switch_to_virtual_host_style(
     request: Any, signature_version: Any, default_endpoint_url: Optional[str] = ..., **kwargs: Any
 ) -> None: ...
 def instance_cache(func: Any) -> Any: ...
+def lru_cache_weakref(*cache_args: Any, **cache_kwargs: Any) -> Any: ...
 def switch_host_s3_accelerate(request: Any, operation_name: Any, **kwargs: Any) -> None: ...
 def switch_host_with_param(request: Any, param_name: Any) -> None: ...
 def deep_merge(base: Any, extra: Any) -> None: ...
 def hyphenize_service_id(service_id: Any) -> Any: ...
 
 class S3RegionRedirectorv2:
     def __init__(self, endpoint_bridge: Any, client: Any, cache: Optional[Any] = ...) -> None: ...
@@ -275,7 +275,18 @@
         self, params: Dict[str, Any], context: Dict[str, Any], **kwargs: Any
     ) -> None: ...
     def check_for_global_endpoint(
         self, params: Dict[str, Any], context: Dict[str, Any], **kwargs: Any
     ) -> None: ...
 
 def is_s3_accelerate_url(url: Optional[str]) -> bool: ...
+
+class JSONFileCache:
+    CACHE_DIR: Any = ...
+    def __init__(self, working_dir: Any = ..., dumps_func: Optional[Any] = ...) -> None: ...
+    def __contains__(self, cache_key: str) -> bool: ...
+    def __getitem__(self, cache_key: str) -> Any: ...
+    def __delitem__(self, cache_key: str) -> None: ...
+    def __setitem__(self, cache_key: str, value: Any) -> None: ...
+
+SERVICE_NAME_ALIASES: Dict[str, str] = ...
+CLIENT_NAME_TO_HYPHENIZED_SERVICE_ID_OVERRIDES: Dict[str, str] = ...
```

### Comparing `botocore_stubs-1.29.99/botocore-stubs/validate.pyi` & `botocore_stubs-1.31.2/botocore-stubs/validate.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/botocore-stubs/waiter.pyi` & `botocore_stubs-1.31.2/botocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `botocore_stubs-1.29.99/pyproject.toml` & `botocore_stubs-1.31.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "botocore-stubs"
-version = "1.29.99"
+version = "1.31.2"
 description = "Type annotations and code completion for botocore"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/botocore-stubs"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `botocore_stubs-1.29.99/PKG-INFO` & `botocore_stubs-1.31.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-stubs
-Version: 1.29.99
+Version: 1.31.2
 Summary: Type annotations and code completion for botocore
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: botocore,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,22 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Stubs Only
 Requires-Dist: types-awscrt
 Requires-Dist: typing-extensions (>=4.1.0) ; python_version < "3.9"
 Project-URL: Bug Tracker, https://github.com/youtype/botocore-stubs/issues
 Project-URL: Documentation, https://youtype.github.io/mypy_boto3_builder/
```

