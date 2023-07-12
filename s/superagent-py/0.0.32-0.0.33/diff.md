# Comparing `tmp/superagent_py-0.0.32.tar.gz` & `tmp/superagent_py-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.32.tar", max compression
+gzip compressed data, was "superagent_py-0.0.33.tar", max compression
```

## Comparing `superagent_py-0.0.32.tar` & `superagent_py-0.0.33.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1073 2023-07-11 22:05:21.111118 superagent_py-0.0.32/LICENSE
--rw-r--r--   0        0        0     3169 2023-07-11 22:05:21.111118 superagent_py-0.0.32/README.md
--rw-r--r--   0        0        0      380 2023-07-11 22:05:21.111118 superagent_py-0.0.32/pyproject.toml
--rw-r--r--   0        0        0      589 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/__init__.py
--rw-r--r--   0        0        0     2963 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/py.typed
--rw-r--r--   0        0        0      343 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    13371 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     8622 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     7900 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5563 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0     9401 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10077 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0     8745 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2048 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     3990 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-11 22:05:21.111118 superagent_py-0.0.32/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 superagent_py-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-12 22:10:52.048381 superagent_py-0.0.33/LICENSE
+-rw-r--r--   0        0        0     3169 2023-07-12 22:10:52.048381 superagent_py-0.0.33/README.md
+-rw-r--r--   0        0        0      380 2023-07-12 22:10:52.048381 superagent_py-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0      589 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/__init__.py
+-rw-r--r--   0        0        0     2956 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/py.typed
+-rw-r--r--   0        0        0      343 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14309 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    10039 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0     9383 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-12 22:10:52.048381 superagent_py-0.0.33/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-12 22:10:52.052381 superagent_py-0.0.33/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 superagent_py-0.0.33/PKG-INFO
```

### Comparing `superagent_py-0.0.32/LICENSE` & `superagent_py-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/README.md` & `superagent_py-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/src/superagent/__init__.py` & `superagent_py-0.0.33/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.33/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.33/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/src/superagent/resources/agent/client.py` & `superagent_py-0.0.33/src/superagent/resources/agent/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 from ...types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AgentClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_all_agents(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -53,15 +55,17 @@
             _request["hasMemory"] = has_memory
         if prompt_id is not OMIT:
             _request["promptId"] = prompt_id
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -70,15 +74,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_agent(self, agent_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -88,15 +94,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def patch_agent(self, agent_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -105,15 +113,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_agent(self, agent_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -128,39 +138,43 @@
         _request: typing.Dict[str, typing.Any] = {"input": input}
         if has_streaming is not OMIT:
             _request["has_streaming"] = has_streaming
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}/predict"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAgentClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_all_agents(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -184,15 +198,17 @@
         if prompt_id is not OMIT:
             _request["promptId"] = prompt_id
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -202,15 +218,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_agent(self, agent_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -221,15 +239,17 @@
 
     async def patch_agent(self, agent_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -239,15 +259,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_agent(self, agent_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -263,15 +285,17 @@
         if has_streaming is not OMIT:
             _request["has_streaming"] = has_streaming
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}/predict"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.33/src/superagent/resources/agent_documents/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class AgentDocumentsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_agent_documents(self, *, expand: typing.Optional[bool] = None) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-documents"),
             params={"expand": expand},
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -38,15 +40,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent_document(self, *, agent_id: str, document_id: str) -> typing.Any:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-documents"),
             json=jsonable_encoder({"agentId": agent_id, "documentId": document_id}),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -55,15 +59,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_agent_document(self, agent_document_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-documents/{agent_document_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -72,40 +78,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_agent_document(self, agent_document_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-documents/{agent_document_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAgentDocumentsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_agent_documents(self, *, expand: typing.Optional[bool] = None) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-documents"),
                 params={"expand": expand},
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -116,15 +126,17 @@
 
     async def create_agent_document(self, *, agent_id: str, document_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-documents"),
                 json=jsonable_encoder({"agentId": agent_id, "documentId": document_id}),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -134,15 +146,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_agent_document(self, agent_document_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-documents/{agent_document_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -152,15 +166,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_agent_document(self, agent_document_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-documents/{agent_document_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.33/src/superagent/resources/agent_tools/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class AgentToolsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_agent_tools(self, *, expand: typing.Optional[bool] = None) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-tools"),
             params={"expand": expand},
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -38,15 +40,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent_tool(self, *, agent_id: str, tool_id: str) -> typing.Any:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-tools"),
             json=jsonable_encoder({"agentId": agent_id, "toolId": tool_id}),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -55,15 +59,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_agent_tool(self, agent_tool_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-tools/{agent_tool_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -72,40 +78,44 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_agent_tool(self, agent_tool_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-tools/{agent_tool_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAgentToolsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_agent_tools(self, *, expand: typing.Optional[bool] = None) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-tools"),
                 params={"expand": expand},
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -116,15 +126,17 @@
 
     async def create_agent_tool(self, *, agent_id: str, tool_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/agent-tools"),
                 json=jsonable_encoder({"agentId": agent_id, "toolId": tool_id}),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -134,15 +146,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_agent_tool(self, agent_tool_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-tools/{agent_tool_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -152,15 +166,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_agent_tool(self, agent_tool_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agent-tools/{agent_tool_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.33/src/superagent/resources/api_token/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class ApiTokenClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_api_tokens(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/api-tokens"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -35,15 +37,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_api_token(self, *, description: str) -> typing.Any:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/api-tokens"),
             json=jsonable_encoder({"description": description}),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -52,15 +56,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_api_token(self, token_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/api-tokens/{token_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -69,39 +75,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_api_token(self, token_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/api-tokens/{token_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncApiTokenClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_api_tokens(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/api-tokens"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -110,15 +120,17 @@
 
     async def create_api_token(self, *, description: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/api-tokens"),
                 json=jsonable_encoder({"description": description}),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -128,15 +140,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_api_token(self, token_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/api-tokens/{token_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -146,15 +160,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_api_token(self, token_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/api-tokens/{token_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/auth/client.py` & `superagent_py-0.0.33/src/superagent/resources/auth/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 from ...types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class AuthClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def sign_in(self, *, email: str, password: str) -> typing.Any:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/sign-in"),
             json=jsonable_encoder({"email": email, "password": password}),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -53,40 +55,44 @@
             _request["name"] = name
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/sign-up"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAuthClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def sign_in(self, *, email: str, password: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/sign-in"),
                 json=jsonable_encoder({"email": email, "password": password}),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -109,15 +115,17 @@
         if metadata is not OMIT:
             _request["metadata"] = metadata
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/sign-up"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/documents/client.py` & `superagent_py-0.0.33/src/superagent/resources/documents/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 from ...types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class DocumentsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_documents(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/documents"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -57,15 +59,17 @@
             _request["to_page"] = to_page
         if splitter is not OMIT:
             _request["splitter"] = splitter
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/documents"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -74,15 +78,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_document(self, document_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -91,39 +97,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_document(self, document_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDocumentsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_documents(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/documents"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -151,15 +161,17 @@
         if splitter is not OMIT:
             _request["splitter"] = splitter
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/documents"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -169,15 +181,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_document(self, document_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -187,15 +201,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_document(self, document_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/documents/{document_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.33/src/superagent/resources/prompts/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class PromptsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_prompts(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/prompts"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -35,15 +37,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_a_prompt(self, *, name: str, input_variables: typing.List[typing.Any], template: str) -> typing.Any:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/prompts"),
             json=jsonable_encoder({"name": name, "input_variables": input_variables, "template": template}),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -52,15 +56,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_prompt(self, prompt_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -70,15 +76,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def patch_prompt(self, prompt_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
             json=jsonable_encoder(request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -87,39 +95,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_prompt(self, prompt_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPromptsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_prompts(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/prompts"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -130,15 +142,17 @@
         self, *, name: str, input_variables: typing.List[typing.Any], template: str
     ) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/prompts"),
                 json=jsonable_encoder({"name": name, "input_variables": input_variables, "template": template}),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -148,15 +162,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_prompt(self, prompt_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -167,15 +183,17 @@
 
     async def patch_prompt(self, prompt_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
                 json=jsonable_encoder(request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -185,15 +203,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_prompt(self, prompt_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/prompts/{prompt_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/tools/client.py` & `superagent_py-0.0.33/src/superagent/resources/tools/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 from ...types.http_validation_error import HttpValidationError
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ToolsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_tools(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/tools"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -50,15 +52,17 @@
             _request["authorization"] = authorization
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/tools"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -67,15 +71,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_tool(self, tool_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -84,39 +90,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_tool(self, tool_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncToolsClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_tools(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/tools"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -137,15 +147,17 @@
         if metadata is not OMIT:
             _request["metadata"] = metadata
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/tools"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -155,15 +167,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_tool(self, tool_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
@@ -173,15 +187,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_tool(self, tool_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/traces/client.py` & `superagent_py-0.0.33/src/superagent/resources/traces/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,45 +8,49 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 
 
 class TracesClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def list_agent_traces(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/traces"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTracesClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def list_agent_traces(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/traces"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `superagent_py-0.0.32/src/superagent/resources/user/client.py` & `superagent_py-0.0.33/src/superagent/resources/user/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,62 +10,68 @@
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 
 
 class UserClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     def read_user_me(self) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/users/me"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def read_user(self, user_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/users/{user_id}"),
-            headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUserClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
-        self.api_key = api_key
+        self._token = token
 
     async def read_user_me(self) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/users/me"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -73,15 +79,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def read_user(self, user_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/users/{user_id}"),
-                headers=remove_none_from_headers({"X_SUPERAGENT_API_KEY": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
```

### Comparing `superagent_py-0.0.32/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.33/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/src/superagent/types/validation_error.py` & `superagent_py-0.0.33/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.32/PKG-INFO` & `superagent_py-0.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.32
+Version: 0.0.33
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

