# Comparing `tmp/dynatrace_opentelemetry_azure_functions-1.267.3-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_azure_functions-1.269.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15108 bytes, number of entries: 11
+Zip file size: 15110 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      687 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/__init__.py
 -rw-r--r--  2.0 unx     3948 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_bindings.py
 -rw-r--r--  2.0 unx     3563 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_resource.py
 -rw-r--r--  2.0 unx     6768 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_triggers.py
 -rw-r--r--  2.0 unx     8183 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/azure/functions/version.py
-?rw-r--r--  2.0 unx     1222 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/RECORD
-11 files, 37013 bytes uncompressed, 13004 bytes compressed:  64.9%
+?rw-r--r--  2.0 unx     1222 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD
+11 files, 37013 bytes uncompressed, 13006 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: dynatrace/opentelemetry/azure/functions/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/azure/functions/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/METADATA
+Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/RECORD
+Filename: dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/azure/functions/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.267.3"
+__version__ = "1.269.3"
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/METADATA` & `dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-azure-functions
-Version: 1.267.3
+Version: 1.269.3
 Summary: Dynatrace OpenTelemetry package for Azure Functions
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: azure-functions>=1.0
-Requires-Dist: dynatrace-opentelemetry-core==1.267.3
+Requires-Dist: dynatrace-opentelemetry-core==1.269.3
 Requires-Dist: opentelemetry-api~=1.3
 Requires-Dist: wrapt<2,>=1.10
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Azure Functions
```

## Comparing `dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/RECORD` & `dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dynatrace/opentelemetry/azure/functions/__init__.py,sha256=3f-XclR-IZfJbXNL2pVkCgRw1PvpaqbgfEobCXWwQqk,687
 dynatrace/opentelemetry/azure/functions/_bindings.py,sha256=xaFgbMd95sRQ-OiFolghoB7uXnU9MAgSi4vg_yYMwQM,3948
 dynatrace/opentelemetry/azure/functions/_resource.py,sha256=uwNmPP-5dqQwzM_ZXxfpFmyy5-Y2Jo3A_hASmoqKLcg,3563
 dynatrace/opentelemetry/azure/functions/_triggers.py,sha256=es8rn0I9NbSfNRANyDk3pmeWwvhpnWrYi8RZ-lUo-ic,6768
 dynatrace/opentelemetry/azure/functions/_wrapper.py,sha256=JPAG7BuCUzQayQebaSYJiodr9GLWck_OMhmHrPMZRWU,8183
 dynatrace/opentelemetry/azure/functions/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/azure/functions/version.py,sha256=jL63eMWfnt6SPFXgzY587Lcb6BNRe4ajs1r87q1v8UE,24
-dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/METADATA,sha256=tXN46tYGzrqMBjYugx3cgtUfbWnoXYmqWeGlFh07WDU,1222
-dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
-dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_azure_functions-1.267.3.dist-info/RECORD,,
+dynatrace/opentelemetry/azure/functions/version.py,sha256=Iv8aaQDjoT0tZwDpNHehTNAt5kMZ3ZmEP8YNNJg71fA,24
+dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/METADATA,sha256=x0MkrmHFmBDelTBrSMk-zpCCnACXr-iYmn7WyVqKuBA,1222
+dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
+dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_azure_functions-1.269.3.dist-info/RECORD,,
```

