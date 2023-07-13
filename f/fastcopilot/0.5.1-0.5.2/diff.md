# Comparing `tmp/fastcopilot-0.5.1.tar.gz` & `tmp/fastcopilot-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcopilot-0.5.1.tar", max compression
+gzip compressed data, was "fastcopilot-0.5.2.tar", max compression
```

## Comparing `fastcopilot-0.5.1.tar` & `fastcopilot-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.5.1/LICENSE
--rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.5.1/README.md
--rw-r--r--   0        0        0      511 2023-07-10 09:06:58.094530 fastcopilot-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.5.1/src/fastcopilot/__init__.py
--rw-r--r--   0        0        0     5537 2023-07-10 09:09:15.038301 fastcopilot-0.5.1/src/fastcopilot/copilot.py
--rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.5.1/src/fastcopilot/exceptions.py
--rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.5.1/src/fastcopilot/schemas.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 fastcopilot-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-09 22:51:06.722205 fastcopilot-0.5.2/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-09 23:12:48.281536 fastcopilot-0.5.2/README.md
+-rw-r--r--   0        0        0      511 2023-07-13 19:43:04.490726 fastcopilot-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-09 18:57:06.166013 fastcopilot-0.5.2/src/fastcopilot/__init__.py
+-rw-r--r--   0        0        0     5598 2023-07-13 19:40:02.501161 fastcopilot-0.5.2/src/fastcopilot/copilot.py
+-rw-r--r--   0        0        0      151 2023-07-06 10:19:17.568905 fastcopilot-0.5.2/src/fastcopilot/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-06 10:34:33.901722 fastcopilot-0.5.2/src/fastcopilot/schemas.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 fastcopilot-0.5.2/PKG-INFO
```

### Comparing `fastcopilot-0.5.1/LICENSE` & `fastcopilot-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcopilot-0.5.1/src/fastcopilot/copilot.py` & `fastcopilot-0.5.2/src/fastcopilot/copilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             {
                 "role": "user",
                 "content": ipt.strip()
             }
         )
         response = openai.ChatCompletion.create(**self.params)
         resp_msg = response["choices"][0]["message"]
-        if function_call := resp_msg.get("function_call"):
+        while function_call := resp_msg.get("function_call"):
             func_name = function_call["name"]
             arguments = json.loads(function_call["arguments"])
             logger.debug(f"<FunctionCall>name: {func_name}, arguments: {arguments}")
             func_spec = self._func_mapping.get(func_name)
             if asyncio.iscoroutinefunction(func_spec.handler):
                 raise AsyncFunctionNotSupported("Try `Copilot.arun()`")
             else:
@@ -100,14 +100,16 @@
                 {
                     "role": "function",
                     "name": func_name,
                     "content": json.dumps(result, ensure_ascii=False)
                 }
             )
             response = openai.ChatCompletion.create(**self.params)
+            resp_msg = response["choices"][0]["message"]
+
         self.messages.append(
             {
                 "role": "assistant",
                 "content": response["choices"][0]["message"]["content"]
             }
         )
```

### Comparing `fastcopilot-0.5.1/PKG-INFO` & `fastcopilot-0.5.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcopilot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fast Copilot framework, easy to learn, fast to code, fast to build a copilot for your applications.
 Author: Jackson
 Author-email: jackson.zhang0429@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
```

