# Comparing `tmp/pulumiverse_buildkite-2.2.0.tar.gz` & `tmp/pulumiverse_buildkite-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_buildkite-2.2.0.tar", last modified: Fri Jun 16 16:45:31 2023, max compression
+gzip compressed data, was "pulumiverse_buildkite-2.3.0.tar", last modified: Thu Jul 13 14:48:26 2023, max compression
```

## Comparing `pulumiverse_buildkite-2.2.0.tar` & `pulumiverse_buildkite-2.3.0.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.258150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/get_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59466 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.237240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.237240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/agent/agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.237240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/cluster_agent_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/cluster_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/cluster/get_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.237240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/get_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63055 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22208 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19823 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:48:26.237240 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 14:48:26.000000 pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:48:26.241240 pulumiverse_buildkite-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-13 14:48:25.000000 pulumiverse_buildkite-2.3.0/setup.py
```

### Comparing `pulumiverse_buildkite-2.2.0/PKG-INFO` & `pulumiverse_buildkite-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_buildkite
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -32,21 +32,21 @@
 This package is available in many languages in the standard packaging formats.
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/pulumi-buildkite
+npm install @pulumiverse/buildkite
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/pulumi-buildkite
+yarn add @pulumiverse/buildkite
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -79,15 +79,15 @@
 - `buildkite:rest_url` (optional, environment: `BUILDKITE_REST_URL`) - The Buildkite REST URL.
 
 ## Example
 
 Example for *Typescript* to create a resource:
 
 ```typescript
-import * as buildkite from '@pulumiverse/pulumi-buildkite';
+import * as buildkite from '@pulumiverse/buildkite';
 
 const args = {};
 const vm = new buildkite.agent.AgentToken(
   'token',
   args,
 );
 ```
```

### Comparing `pulumiverse_buildkite-2.2.0/README.md` & `pulumiverse_buildkite-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 This package is available in many languages in the standard packaging formats.
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/pulumi-buildkite
+npm install @pulumiverse/buildkite
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/pulumi-buildkite
+yarn add @pulumiverse/buildkite
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -67,15 +67,15 @@
 - `buildkite:rest_url` (optional, environment: `BUILDKITE_REST_URL`) - The Buildkite REST URL.
 
 ## Example
 
 Example for *Typescript* to create a resource:
 
 ```typescript
-import * as buildkite from '@pulumiverse/pulumi-buildkite';
+import * as buildkite from '@pulumiverse/buildkite';
 
 const args = {};
 const vm = new buildkite.agent.AgentToken(
   'token',
   args,
 );
 ```
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/__init__.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 from .get_meta import *
 from .provider import *
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import pulumiverse_buildkite.agent as __agent
     agent = __agent
+    import pulumiverse_buildkite.cluster as __cluster
+    cluster = __cluster
     import pulumiverse_buildkite.config as __config
     config = __config
     import pulumiverse_buildkite.organization as __organization
     organization = __organization
     import pulumiverse_buildkite.pipeline as __pipeline
     pipeline = __pipeline
     import pulumiverse_buildkite.team as __team
     team = __team
 else:
     agent = _utilities.lazy_import('pulumiverse_buildkite.agent')
+    cluster = _utilities.lazy_import('pulumiverse_buildkite.cluster')
     config = _utilities.lazy_import('pulumiverse_buildkite.config')
     organization = _utilities.lazy_import('pulumiverse_buildkite.organization')
     pipeline = _utilities.lazy_import('pulumiverse_buildkite.pipeline')
     team = _utilities.lazy_import('pulumiverse_buildkite.team')
 
 _utilities.register(
     resource_modules="""
@@ -36,14 +39,38 @@
   "fqn": "pulumiverse_buildkite.agent",
   "classes": {
    "buildkite:Agent/agentToken:AgentToken": "AgentToken"
   }
  },
  {
   "pkg": "buildkite",
+  "mod": "Cluster/cluster",
+  "fqn": "pulumiverse_buildkite.cluster",
+  "classes": {
+   "buildkite:Cluster/cluster:Cluster": "Cluster"
+  }
+ },
+ {
+  "pkg": "buildkite",
+  "mod": "Cluster/clusterAgentToken",
+  "fqn": "pulumiverse_buildkite.cluster",
+  "classes": {
+   "buildkite:Cluster/clusterAgentToken:ClusterAgentToken": "ClusterAgentToken"
+  }
+ },
+ {
+  "pkg": "buildkite",
+  "mod": "Cluster/clusterQueue",
+  "fqn": "pulumiverse_buildkite.cluster",
+  "classes": {
+   "buildkite:Cluster/clusterQueue:ClusterQueue": "ClusterQueue"
+  }
+ },
+ {
+  "pkg": "buildkite",
   "mod": "Organization/settings",
   "fqn": "pulumiverse_buildkite.organization",
   "classes": {
    "buildkite:Organization/settings:Settings": "Settings"
   }
  },
  {
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/_utilities.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/agent_token.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/agent/agent_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,14 +174,16 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = AgentTokenArgs.__new__(AgentTokenArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["token"] = None
             __props__.__dict__["uuid"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["token"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(AgentToken, __self__).__init__(
             'buildkite:Agent/agentToken:AgentToken',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/vars.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/get_meta.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/get_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('buildkite:index/getMeta:getMeta', __args__, opts=opts, typ=GetMetaResult).value
 
     return AwaitableGetMetaResult(
-        id=__ret__.id,
-        webhook_ips=__ret__.webhook_ips)
+        id=pulumi.get(__ret__, 'id'),
+        webhook_ips=pulumi.get(__ret__, 'webhook_ips'))
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/get_organization.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/get_organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,17 +94,17 @@
     """
     __args__ = dict()
     __args__['allowedApiIpAddresses'] = allowed_api_ip_addresses
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('buildkite:Organization/getOrganization:getOrganization', __args__, opts=opts, typ=GetOrganizationResult).value
 
     return AwaitableGetOrganizationResult(
-        allowed_api_ip_addresses=__ret__.allowed_api_ip_addresses,
-        id=__ret__.id,
-        uuid=__ret__.uuid)
+        allowed_api_ip_addresses=pulumi.get(__ret__, 'allowed_api_ip_addresses'),
+        id=pulumi.get(__ret__, 'id'),
+        uuid=pulumi.get(__ret__, 'uuid'))
 
 
 @_utilities.lift_output_func(get_organization)
 def get_organization_output(allowed_api_ip_addresses: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationResult]:
     """
     ## # Data Source: organization
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/settings.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/organization/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 
         Organization settings can be imported by passing the organization slug to the import command, along with the identifier of the resource.
 
         ```sh
          $ pulumi import buildkite:Organization/settings:Settings test_settings test_org
         ```
 
+         Your organization's slug can be found in your organisation's [settings](https://buildkite.com/organizations/~/settings) page.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_api_ip_addresses: A list of IP addresses in CIDR format that are allowed to access the Buildkite API. If not set, all IP addresses are allowed (the same as setting 0.0.0.0/0).
         """
         ...
     @overload
     def __init__(__self__,
@@ -136,14 +138,16 @@
 
         Organization settings can be imported by passing the organization slug to the import command, along with the identifier of the resource.
 
         ```sh
          $ pulumi import buildkite:Organization/settings:Settings test_settings test_org
         ```
 
+         Your organization's slug can be found in your organisation's [settings](https://buildkite.com/organizations/~/settings) page.
+
         :param str resource_name: The name of the resource.
         :param SettingsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(SettingsArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/_inputs.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/get_pipeline.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/get_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,21 +137,21 @@
     """
     __args__ = dict()
     __args__['slug'] = slug
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('buildkite:Pipeline/getPipeline:getPipeline', __args__, opts=opts, typ=GetPipelineResult).value
 
     return AwaitableGetPipelineResult(
-        default_branch=__ret__.default_branch,
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        repository=__ret__.repository,
-        slug=__ret__.slug,
-        webhook_url=__ret__.webhook_url)
+        default_branch=pulumi.get(__ret__, 'default_branch'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        repository=pulumi.get(__ret__, 'repository'),
+        slug=pulumi.get(__ret__, 'slug'),
+        webhook_url=pulumi.get(__ret__, 'webhook_url'))
 
 
 @_utilities.lift_output_func(get_pipeline)
 def get_pipeline_output(slug: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPipelineResult]:
     """
     ## # Data Source: pipeline
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/outputs.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/pipeline.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 __all__ = ['PipelineArgs', 'Pipeline']
 
 @pulumi.input_type
 class PipelineArgs:
     def __init__(__self__, *,
                  repository: pulumi.Input[str],
                  allow_rebuilds: Optional[pulumi.Input[bool]] = None,
+                 archive_on_delete: Optional[pulumi.Input[bool]] = None,
                  branch_configuration: Optional[pulumi.Input[str]] = None,
                  cancel_intermediate_builds: Optional[pulumi.Input[bool]] = None,
                  cancel_intermediate_builds_branch_filter: Optional[pulumi.Input[str]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  default_timeout_in_minutes: Optional[pulumi.Input[int]] = None,
                  deletion_protection: Optional[pulumi.Input[bool]] = None,
@@ -53,14 +54,16 @@
         :param pulumi.Input[str] skip_intermediate_builds_branch_filter: Limit which branches build skipping applies to, for example `!master` will ensure that the master branch won't have its builds automatically skipped.
         :param pulumi.Input[str] steps: The string YAML steps to run the pipeline. Defaults to `buildkite-agent pipeline upload` if not specified.
         :param pulumi.Input[Sequence[pulumi.Input['PipelineTeamArgs']]] teams: Set team access for the pipeline. Can be specified multiple times for each team. See Teams Configuration below for details.
         """
         pulumi.set(__self__, "repository", repository)
         if allow_rebuilds is not None:
             pulumi.set(__self__, "allow_rebuilds", allow_rebuilds)
+        if archive_on_delete is not None:
+            pulumi.set(__self__, "archive_on_delete", archive_on_delete)
         if branch_configuration is not None:
             pulumi.set(__self__, "branch_configuration", branch_configuration)
         if cancel_intermediate_builds is not None:
             pulumi.set(__self__, "cancel_intermediate_builds", cancel_intermediate_builds)
         if cancel_intermediate_builds_branch_filter is not None:
             pulumi.set(__self__, "cancel_intermediate_builds_branch_filter", cancel_intermediate_builds_branch_filter)
         if cluster_id is not None:
@@ -111,14 +114,23 @@
         return pulumi.get(self, "allow_rebuilds")
 
     @allow_rebuilds.setter
     def allow_rebuilds(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_rebuilds", value)
 
     @property
+    @pulumi.getter(name="archiveOnDelete")
+    def archive_on_delete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "archive_on_delete")
+
+    @archive_on_delete.setter
+    def archive_on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "archive_on_delete", value)
+
+    @property
     @pulumi.getter(name="branchConfiguration")
     def branch_configuration(self) -> Optional[pulumi.Input[str]]:
         """
         Limit which branches and tags cause new builds to be created, either via a code push or via the Builds REST API.
         """
         return pulumi.get(self, "branch_configuration")
 
@@ -304,14 +316,15 @@
         pulumi.set(self, "teams", value)
 
 
 @pulumi.input_type
 class _PipelineState:
     def __init__(__self__, *,
                  allow_rebuilds: Optional[pulumi.Input[bool]] = None,
+                 archive_on_delete: Optional[pulumi.Input[bool]] = None,
                  badge_url: Optional[pulumi.Input[str]] = None,
                  branch_configuration: Optional[pulumi.Input[str]] = None,
                  cancel_intermediate_builds: Optional[pulumi.Input[bool]] = None,
                  cancel_intermediate_builds_branch_filter: Optional[pulumi.Input[str]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  default_timeout_in_minutes: Optional[pulumi.Input[int]] = None,
@@ -349,14 +362,16 @@
         :param pulumi.Input[str] slug: The buildkite slug of the team.
         :param pulumi.Input[str] steps: The string YAML steps to run the pipeline. Defaults to `buildkite-agent pipeline upload` if not specified.
         :param pulumi.Input[Sequence[pulumi.Input['PipelineTeamArgs']]] teams: Set team access for the pipeline. Can be specified multiple times for each team. See Teams Configuration below for details.
         :param pulumi.Input[str] webhook_url: The Buildkite webhook URL to configure on the repository to trigger builds on this pipeline.
         """
         if allow_rebuilds is not None:
             pulumi.set(__self__, "allow_rebuilds", allow_rebuilds)
+        if archive_on_delete is not None:
+            pulumi.set(__self__, "archive_on_delete", archive_on_delete)
         if badge_url is not None:
             pulumi.set(__self__, "badge_url", badge_url)
         if branch_configuration is not None:
             pulumi.set(__self__, "branch_configuration", branch_configuration)
         if cancel_intermediate_builds is not None:
             pulumi.set(__self__, "cancel_intermediate_builds", cancel_intermediate_builds)
         if cancel_intermediate_builds_branch_filter is not None:
@@ -403,14 +418,23 @@
         return pulumi.get(self, "allow_rebuilds")
 
     @allow_rebuilds.setter
     def allow_rebuilds(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "allow_rebuilds", value)
 
     @property
+    @pulumi.getter(name="archiveOnDelete")
+    def archive_on_delete(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "archive_on_delete")
+
+    @archive_on_delete.setter
+    def archive_on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "archive_on_delete", value)
+
+    @property
     @pulumi.getter(name="badgeUrl")
     def badge_url(self) -> Optional[pulumi.Input[str]]:
         """
         The pipeline's last build status so you can display build status badge.
         """
         return pulumi.get(self, "badge_url")
 
@@ -646,14 +670,15 @@
 
 class Pipeline(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_rebuilds: Optional[pulumi.Input[bool]] = None,
+                 archive_on_delete: Optional[pulumi.Input[bool]] = None,
                  branch_configuration: Optional[pulumi.Input[str]] = None,
                  cancel_intermediate_builds: Optional[pulumi.Input[bool]] = None,
                  cancel_intermediate_builds_branch_filter: Optional[pulumi.Input[str]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  default_timeout_in_minutes: Optional[pulumi.Input[int]] = None,
                  deletion_protection: Optional[pulumi.Input[bool]] = None,
@@ -716,14 +741,27 @@
         test_new = buildkite.pipeline.Pipeline("testNew",
             repository="https://github.com/buildkite/terraform-provider-buildkite.git",
             steps=(lambda path: open(path).read())("./deploy-steps.yml"),
             deletion_protection=True)
         ```
 
         `deletion_protection` will block `destroy` actions on the **pipeline**. Attached resources, such as `schedules` will still be destroyed.
+        ### With Archive On Delete
+
+        ```python
+        import pulumi
+        import pulumiverse_buildkite as buildkite
+
+        test_new = buildkite.pipeline.Pipeline("testNew",
+            repository="https://github.com/buildkite/terraform-provider-buildkite.git",
+            steps=(lambda path: open(path).read())("./deploy-steps.yml"),
+            archive_on_delete=True)
+        ```
+
+        `archive_on_delete` will archive the **pipeline** when `destroy` is called. Attached resources, such as `schedules` will still be destroyed. In order to delete the pipeline, `archive_on_delete` must be set to `false` in the configuration, then `destroy` must be called again.
         ### With GitHub Provider Settings
 
         ```python
         import pulumi
         import pulumiverse_buildkite as buildkite
 
         # Pipeline that should not be triggered from a GitHub webhook
@@ -749,14 +787,22 @@
 
         Pipelines can be imported using the `GraphQL ID` (not UUID), e.g.
 
         ```sh
          $ pulumi import buildkite:Pipeline/pipeline:Pipeline fleet UGlwZWxpbmUtLS00MzVjYWQ1OC1lODFkLTQ1YWYtODYzNy1iMWNmODA3MDIzOGQ=
         ```
 
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/04e6ac1d-222e-49f9-8167-4767ab0f5362). graphql query getPipelineId {
+
+         pipeline(slug"ORGANIZATION_SLUG/PIPELINE_SLUG") {
+
+         id
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_rebuilds: A boolean on whether or not to allow rebuilds for the pipeline.
         :param pulumi.Input[str] branch_configuration: Limit which branches and tags cause new builds to be created, either via a code push or via the Builds REST API.
         :param pulumi.Input[bool] cancel_intermediate_builds: A boolean to enable automatically cancelling any running builds on the same branch when a new build is created.
         :param pulumi.Input[str] cancel_intermediate_builds_branch_filter: Limit which branches build cancelling applies to, for example !master will ensure that the master branch won't have its builds automatically cancelled.
         :param pulumi.Input[str] cluster_id: The GraphQL ID of the cluster you want to use for the pipeline.
@@ -827,14 +873,27 @@
         test_new = buildkite.pipeline.Pipeline("testNew",
             repository="https://github.com/buildkite/terraform-provider-buildkite.git",
             steps=(lambda path: open(path).read())("./deploy-steps.yml"),
             deletion_protection=True)
         ```
 
         `deletion_protection` will block `destroy` actions on the **pipeline**. Attached resources, such as `schedules` will still be destroyed.
+        ### With Archive On Delete
+
+        ```python
+        import pulumi
+        import pulumiverse_buildkite as buildkite
+
+        test_new = buildkite.pipeline.Pipeline("testNew",
+            repository="https://github.com/buildkite/terraform-provider-buildkite.git",
+            steps=(lambda path: open(path).read())("./deploy-steps.yml"),
+            archive_on_delete=True)
+        ```
+
+        `archive_on_delete` will archive the **pipeline** when `destroy` is called. Attached resources, such as `schedules` will still be destroyed. In order to delete the pipeline, `archive_on_delete` must be set to `false` in the configuration, then `destroy` must be called again.
         ### With GitHub Provider Settings
 
         ```python
         import pulumi
         import pulumiverse_buildkite as buildkite
 
         # Pipeline that should not be triggered from a GitHub webhook
@@ -860,14 +919,22 @@
 
         Pipelines can be imported using the `GraphQL ID` (not UUID), e.g.
 
         ```sh
          $ pulumi import buildkite:Pipeline/pipeline:Pipeline fleet UGlwZWxpbmUtLS00MzVjYWQ1OC1lODFkLTQ1YWYtODYzNy1iMWNmODA3MDIzOGQ=
         ```
 
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/04e6ac1d-222e-49f9-8167-4767ab0f5362). graphql query getPipelineId {
+
+         pipeline(slug"ORGANIZATION_SLUG/PIPELINE_SLUG") {
+
+         id
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param PipelineArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(PipelineArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -876,14 +943,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  allow_rebuilds: Optional[pulumi.Input[bool]] = None,
+                 archive_on_delete: Optional[pulumi.Input[bool]] = None,
                  branch_configuration: Optional[pulumi.Input[str]] = None,
                  cancel_intermediate_builds: Optional[pulumi.Input[bool]] = None,
                  cancel_intermediate_builds_branch_filter: Optional[pulumi.Input[str]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  default_timeout_in_minutes: Optional[pulumi.Input[int]] = None,
                  deletion_protection: Optional[pulumi.Input[bool]] = None,
@@ -903,14 +971,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PipelineArgs.__new__(PipelineArgs)
 
             __props__.__dict__["allow_rebuilds"] = allow_rebuilds
+            __props__.__dict__["archive_on_delete"] = archive_on_delete
             __props__.__dict__["branch_configuration"] = branch_configuration
             __props__.__dict__["cancel_intermediate_builds"] = cancel_intermediate_builds
             __props__.__dict__["cancel_intermediate_builds_branch_filter"] = cancel_intermediate_builds_branch_filter
             __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["default_branch"] = default_branch
             __props__.__dict__["default_timeout_in_minutes"] = default_timeout_in_minutes
             __props__.__dict__["deletion_protection"] = deletion_protection
@@ -936,14 +1005,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             allow_rebuilds: Optional[pulumi.Input[bool]] = None,
+            archive_on_delete: Optional[pulumi.Input[bool]] = None,
             badge_url: Optional[pulumi.Input[str]] = None,
             branch_configuration: Optional[pulumi.Input[str]] = None,
             cancel_intermediate_builds: Optional[pulumi.Input[bool]] = None,
             cancel_intermediate_builds_branch_filter: Optional[pulumi.Input[str]] = None,
             cluster_id: Optional[pulumi.Input[str]] = None,
             default_branch: Optional[pulumi.Input[str]] = None,
             default_timeout_in_minutes: Optional[pulumi.Input[int]] = None,
@@ -989,14 +1059,15 @@
         :param pulumi.Input[str] webhook_url: The Buildkite webhook URL to configure on the repository to trigger builds on this pipeline.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PipelineState.__new__(_PipelineState)
 
         __props__.__dict__["allow_rebuilds"] = allow_rebuilds
+        __props__.__dict__["archive_on_delete"] = archive_on_delete
         __props__.__dict__["badge_url"] = badge_url
         __props__.__dict__["branch_configuration"] = branch_configuration
         __props__.__dict__["cancel_intermediate_builds"] = cancel_intermediate_builds
         __props__.__dict__["cancel_intermediate_builds_branch_filter"] = cancel_intermediate_builds_branch_filter
         __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["default_branch"] = default_branch
         __props__.__dict__["default_timeout_in_minutes"] = default_timeout_in_minutes
@@ -1013,31 +1084,36 @@
         __props__.__dict__["tags"] = tags
         __props__.__dict__["teams"] = teams
         __props__.__dict__["webhook_url"] = webhook_url
         return Pipeline(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="allowRebuilds")
-    def allow_rebuilds(self) -> pulumi.Output[bool]:
+    def allow_rebuilds(self) -> pulumi.Output[Optional[bool]]:
         """
         A boolean on whether or not to allow rebuilds for the pipeline.
         """
         return pulumi.get(self, "allow_rebuilds")
 
     @property
+    @pulumi.getter(name="archiveOnDelete")
+    def archive_on_delete(self) -> pulumi.Output[Optional[bool]]:
+        return pulumi.get(self, "archive_on_delete")
+
+    @property
     @pulumi.getter(name="badgeUrl")
     def badge_url(self) -> pulumi.Output[str]:
         """
         The pipeline's last build status so you can display build status badge.
         """
         return pulumi.get(self, "badge_url")
 
     @property
     @pulumi.getter(name="branchConfiguration")
-    def branch_configuration(self) -> pulumi.Output[str]:
+    def branch_configuration(self) -> pulumi.Output[Optional[str]]:
         """
         Limit which branches and tags cause new builds to be created, either via a code push or via the Builds REST API.
         """
         return pulumi.get(self, "branch_configuration")
 
     @property
     @pulumi.getter(name="cancelIntermediateBuilds")
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/schedule.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/pipeline/schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -325,14 +325,52 @@
 
         Pipeline schedules can be imported using a slug (which consists of `$BUILDKITE_ORGANIZATION_SLUG/$BUILDKITE_PIPELINE_SLUG/$PIPELINE_SCHEDULE_UUID`), e.g.
 
         ```sh
          $ pulumi import buildkite:Pipeline/schedule:Schedule test myorg/test/1be3e7c7-1e03-4011-accf-b2d8eec90222
         ```
 
+         Your organization's slug can be found in your organisation's [settings](https://buildkite.com/organizations/~/settingss) page.
+
+        The pipeline slug and its relevant schedule UUID can be found with the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/abf9270e-eccf-4c5f-af21-4cd35164ab6c), specifying the organisation slug (when known) and the pipeline search term (PIPELINE_SEARCH_TERM). graphql query getPipelineScheduleUuid {
+
+         organization(slug"ORGANIZATION_SLUG") {
+
+         pipelines(first5, search"PIPELINE_SEARCH_TERM") {
+
+         edges{
+
+         node{
+
+         name
+
+         schedules{
+
+         edges{
+
+        node{
+
+         uuid
+
+         cronline
+
+         }
+
+         }
+
+         }
+
+         }
+
+         }
+
+         }
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] branch: The branch to use for the build.
         :param pulumi.Input[str] commit: The commit ref to use for the build.
         :param pulumi.Input[str] cronline: Schedule interval (see [docs](https://buildkite.com/docs/pipelines/scheduled-builds#schedule-intervals)).
         :param pulumi.Input[bool] enabled: Whether the schedule should run.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] env: A map of environment variables to use for the build.
@@ -369,14 +407,52 @@
 
         Pipeline schedules can be imported using a slug (which consists of `$BUILDKITE_ORGANIZATION_SLUG/$BUILDKITE_PIPELINE_SLUG/$PIPELINE_SCHEDULE_UUID`), e.g.
 
         ```sh
          $ pulumi import buildkite:Pipeline/schedule:Schedule test myorg/test/1be3e7c7-1e03-4011-accf-b2d8eec90222
         ```
 
+         Your organization's slug can be found in your organisation's [settings](https://buildkite.com/organizations/~/settingss) page.
+
+        The pipeline slug and its relevant schedule UUID can be found with the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/abf9270e-eccf-4c5f-af21-4cd35164ab6c), specifying the organisation slug (when known) and the pipeline search term (PIPELINE_SEARCH_TERM). graphql query getPipelineScheduleUuid {
+
+         organization(slug"ORGANIZATION_SLUG") {
+
+         pipelines(first5, search"PIPELINE_SEARCH_TERM") {
+
+         edges{
+
+         node{
+
+         name
+
+         schedules{
+
+         edges{
+
+        node{
+
+         uuid
+
+         cronline
+
+         }
+
+         }
+
+         }
+
+         }
+
+         }
+
+         }
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param ScheduleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ScheduleArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/provider.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,69 +10,71 @@
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
-                 api_token: pulumi.Input[str],
-                 organization: pulumi.Input[str],
+                 api_token: Optional[pulumi.Input[str]] = None,
                  graphql_url: Optional[pulumi.Input[str]] = None,
+                 organization: Optional[pulumi.Input[str]] = None,
                  rest_url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] api_token: API token with GraphQL access and `write_pipelines, read_pipelines` scopes
-        :param pulumi.Input[str] organization: The Buildkite organization slug
         :param pulumi.Input[str] graphql_url: Base URL for the GraphQL API to use
+        :param pulumi.Input[str] organization: The Buildkite organization slug
         :param pulumi.Input[str] rest_url: Base URL for the REST API to use
         """
-        pulumi.set(__self__, "api_token", api_token)
-        pulumi.set(__self__, "organization", organization)
+        if api_token is not None:
+            pulumi.set(__self__, "api_token", api_token)
         if graphql_url is not None:
             pulumi.set(__self__, "graphql_url", graphql_url)
+        if organization is not None:
+            pulumi.set(__self__, "organization", organization)
         if rest_url is not None:
             pulumi.set(__self__, "rest_url", rest_url)
 
     @property
     @pulumi.getter(name="apiToken")
-    def api_token(self) -> pulumi.Input[str]:
+    def api_token(self) -> Optional[pulumi.Input[str]]:
         """
         API token with GraphQL access and `write_pipelines, read_pipelines` scopes
         """
         return pulumi.get(self, "api_token")
 
     @api_token.setter
-    def api_token(self, value: pulumi.Input[str]):
+    def api_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_token", value)
 
     @property
-    @pulumi.getter
-    def organization(self) -> pulumi.Input[str]:
-        """
-        The Buildkite organization slug
-        """
-        return pulumi.get(self, "organization")
-
-    @organization.setter
-    def organization(self, value: pulumi.Input[str]):
-        pulumi.set(self, "organization", value)
-
-    @property
     @pulumi.getter(name="graphqlUrl")
     def graphql_url(self) -> Optional[pulumi.Input[str]]:
         """
         Base URL for the GraphQL API to use
         """
         return pulumi.get(self, "graphql_url")
 
     @graphql_url.setter
     def graphql_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "graphql_url", value)
 
     @property
+    @pulumi.getter
+    def organization(self) -> Optional[pulumi.Input[str]]:
+        """
+        The Buildkite organization slug
+        """
+        return pulumi.get(self, "organization")
+
+    @organization.setter
+    def organization(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "organization", value)
+
+    @property
     @pulumi.getter(name="restUrl")
     def rest_url(self) -> Optional[pulumi.Input[str]]:
         """
         Base URL for the REST API to use
         """
         return pulumi.get(self, "rest_url")
 
@@ -104,15 +106,15 @@
         :param pulumi.Input[str] organization: The Buildkite organization slug
         :param pulumi.Input[str] rest_url: Base URL for the REST API to use
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProviderArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The provider type for the buildkite package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
@@ -140,31 +142,29 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
-            if api_token is None and not opts.urn:
-                raise TypeError("Missing required property 'api_token'")
-            __props__.__dict__["api_token"] = api_token
+            __props__.__dict__["api_token"] = None if api_token is None else pulumi.Output.secret(api_token)
             __props__.__dict__["graphql_url"] = graphql_url
-            if organization is None and not opts.urn:
-                raise TypeError("Missing required property 'organization'")
             __props__.__dict__["organization"] = organization
             __props__.__dict__["rest_url"] = rest_url
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiToken"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'buildkite',
             resource_name,
             __props__,
             opts)
 
     @property
     @pulumi.getter(name="apiToken")
-    def api_token(self) -> pulumi.Output[str]:
+    def api_token(self) -> pulumi.Output[Optional[str]]:
         """
         API token with GraphQL access and `write_pipelines, read_pipelines` scopes
         """
         return pulumi.get(self, "api_token")
 
     @property
     @pulumi.getter(name="graphqlUrl")
@@ -172,15 +172,15 @@
         """
         Base URL for the GraphQL API to use
         """
         return pulumi.get(self, "graphql_url")
 
     @property
     @pulumi.getter
-    def organization(self) -> pulumi.Output[str]:
+    def organization(self) -> pulumi.Output[Optional[str]]:
         """
         The Buildkite organization slug
         """
         return pulumi.get(self, "organization")
 
     @property
     @pulumi.getter(name="restUrl")
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/get_team.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/get_team.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,23 +161,23 @@
     """
     __args__ = dict()
     __args__['slug'] = slug
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('buildkite:Team/getTeam:getTeam', __args__, opts=opts, typ=GetTeamResult).value
 
     return AwaitableGetTeamResult(
-        default_member_role=__ret__.default_member_role,
-        default_team=__ret__.default_team,
-        description=__ret__.description,
-        id=__ret__.id,
-        members_can_create_pipelines=__ret__.members_can_create_pipelines,
-        name=__ret__.name,
-        privacy=__ret__.privacy,
-        slug=__ret__.slug,
-        uuid=__ret__.uuid)
+        default_member_role=pulumi.get(__ret__, 'default_member_role'),
+        default_team=pulumi.get(__ret__, 'default_team'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        members_can_create_pipelines=pulumi.get(__ret__, 'members_can_create_pipelines'),
+        name=pulumi.get(__ret__, 'name'),
+        privacy=pulumi.get(__ret__, 'privacy'),
+        slug=pulumi.get(__ret__, 'slug'),
+        uuid=pulumi.get(__ret__, 'uuid'))
 
 
 @_utilities.lift_output_func(get_team)
 def get_team_output(slug: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamResult]:
     """
     ## # Data Source: team
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/member.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/member.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,25 +176,25 @@
 
         Team members can be imported using the GraphQL ID of the membership. Note this is different to the ID of the user.
 
         ```sh
          $ pulumi import buildkite:Team/member:Member a_smith VGVhbU1lbWJlci0tLTVlZDEyMmY2LTM2NjQtNDI1MS04YzMwLTc4NjRiMDdiZDQ4Zg==
         ```
 
-         To find the ID of a team member you are trying to import you can use the GraphQL snippet below. A link to this snippet can also be found at https://buildkite.com/user/graphql/console/c6a2cc65-dc59-49df-95c6-7167b68dbd5d. You will need fo fill in the organization slug and search terms for teams and members. Both search terms work on the name of the associated object. graphql query {
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/ce4540dd-4f60-4e79-8e8f-9f4c3bc8784e), where you will need fo fill in the organization slug and search terms for teams and members. Both search terms (TEAM_SEARCH_TERM and TEAM_MEMBER_SEARCH_TERM) work on the name of the associated object. graphql query getTeamMemberId {
 
-         organization(slug"") {
+         organization(slug"ORGANIZATION_SLUG") {
 
-         teams(first2, search"") {
+         teams(first2, search"TEAM_SEARCH_TERM") {
 
          edges {
 
          node {
 
-         members(first2, search"") {
+         members(first2, search"TEAM_MEMBER_SEARCH_TERM") {
 
          edges {
 
          node {
 
          id
 
@@ -255,25 +255,25 @@
 
         Team members can be imported using the GraphQL ID of the membership. Note this is different to the ID of the user.
 
         ```sh
          $ pulumi import buildkite:Team/member:Member a_smith VGVhbU1lbWJlci0tLTVlZDEyMmY2LTM2NjQtNDI1MS04YzMwLTc4NjRiMDdiZDQ4Zg==
         ```
 
-         To find the ID of a team member you are trying to import you can use the GraphQL snippet below. A link to this snippet can also be found at https://buildkite.com/user/graphql/console/c6a2cc65-dc59-49df-95c6-7167b68dbd5d. You will need fo fill in the organization slug and search terms for teams and members. Both search terms work on the name of the associated object. graphql query {
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/ce4540dd-4f60-4e79-8e8f-9f4c3bc8784e), where you will need fo fill in the organization slug and search terms for teams and members. Both search terms (TEAM_SEARCH_TERM and TEAM_MEMBER_SEARCH_TERM) work on the name of the associated object. graphql query getTeamMemberId {
 
-         organization(slug"") {
+         organization(slug"ORGANIZATION_SLUG") {
 
-         teams(first2, search"") {
+         teams(first2, search"TEAM_SEARCH_TERM") {
 
          edges {
 
          node {
 
-         members(first2, search"") {
+         members(first2, search"TEAM_MEMBER_SEARCH_TERM") {
 
          edges {
 
          node {
 
          id
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/team.py` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite/team/team.py`

 * *Files 4% similar despite different names*

```diff
@@ -277,14 +277,44 @@
 
         team = buildkite.team.Team("team",
             default_member_role="MEMBER",
             default_team=True,
             privacy="VISIBLE")
         ```
 
+        ## Import
+
+        Teams can be imported using the `GraphQL ID` (not UUID), e.g.
+
+        ```sh
+         $ pulumi import buildkite:Team/team:Team fleet UGlwZWxpbmUtLS00MzVjYWQ1OC1lODFkLTQ1YWYtODYzNy1iMWNmODA3MDIzOGQ=
+        ```
+
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/6e74c89c-4e91-4d1d-92ca-4fb19d0ea453), where you will need fo fill in the organization slug and search term (TEAM_SEARCH_TERM) for the team. graphql query getTeamId {
+
+         organization(slug"ORGANIZATION_SLUG") {
+
+         teams(first1, search"TEAM_SEARCH_TERM") {
+
+         edges {
+
+         node {
+
+         id
+
+         name
+
+         }
+
+         }
+
+         }
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_member_role: Default role to assign to a team member.
         :param pulumi.Input[bool] default_team: Whether to assign this team to a user by default.
         :param pulumi.Input[str] description: The description to assign to the team.
         :param pulumi.Input[bool] members_can_create_pipelines: Whether team members can create.
         :param pulumi.Input[str] name: The name of the team.
@@ -313,14 +343,44 @@
 
         team = buildkite.team.Team("team",
             default_member_role="MEMBER",
             default_team=True,
             privacy="VISIBLE")
         ```
 
+        ## Import
+
+        Teams can be imported using the `GraphQL ID` (not UUID), e.g.
+
+        ```sh
+         $ pulumi import buildkite:Team/team:Team fleet UGlwZWxpbmUtLS00MzVjYWQ1OC1lODFkLTQ1YWYtODYzNy1iMWNmODA3MDIzOGQ=
+        ```
+
+         To find the ID to use, you can use the GraphQL query below. Alternatively, you could use this [pre-saved query](https://buildkite.com/user/graphql/console/6e74c89c-4e91-4d1d-92ca-4fb19d0ea453), where you will need fo fill in the organization slug and search term (TEAM_SEARCH_TERM) for the team. graphql query getTeamId {
+
+         organization(slug"ORGANIZATION_SLUG") {
+
+         teams(first1, search"TEAM_SEARCH_TERM") {
+
+         edges {
+
+         node {
+
+         id
+
+         name
+
+         }
+
+         }
+
+         }
+
+         } }
+
         :param str resource_name: The name of the resource.
         :param TeamArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TeamArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/PKG-INFO` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-buildkite
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -32,21 +32,21 @@
 This package is available in many languages in the standard packaging formats.
 
 ### Node.js (JavaScript/TypeScript)
 
 To use from JavaScript or TypeScript in Node.js, install using either `npm`:
 
 ```bash
-npm install @pulumiverse/pulumi-buildkite
+npm install @pulumiverse/buildkite
 ```
 
 or `yarn`:
 
 ```bash
-yarn add @pulumiverse/pulumi-buildkite
+yarn add @pulumiverse/buildkite
 ```
 
 ### Python
 
 To use from Python, install using `pip`:
 
 ```bash
@@ -79,15 +79,15 @@
 - `buildkite:rest_url` (optional, environment: `BUILDKITE_REST_URL`) - The Buildkite REST URL.
 
 ## Example
 
 Example for *Typescript* to create a resource:
 
 ```typescript
-import * as buildkite from '@pulumiverse/pulumi-buildkite';
+import * as buildkite from '@pulumiverse/buildkite';
 
 const args = {};
 const vm = new buildkite.agent.AgentToken(
   'token',
   args,
 );
 ```
```

### Comparing `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/SOURCES.txt` & `pulumiverse_buildkite-2.3.0/pulumiverse_buildkite.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 pulumiverse_buildkite.egg-info/SOURCES.txt
 pulumiverse_buildkite.egg-info/dependency_links.txt
 pulumiverse_buildkite.egg-info/not-zip-safe
 pulumiverse_buildkite.egg-info/requires.txt
 pulumiverse_buildkite.egg-info/top_level.txt
 pulumiverse_buildkite/agent/__init__.py
 pulumiverse_buildkite/agent/agent_token.py
+pulumiverse_buildkite/cluster/__init__.py
+pulumiverse_buildkite/cluster/cluster.py
+pulumiverse_buildkite/cluster/cluster_agent_token.py
+pulumiverse_buildkite/cluster/cluster_queue.py
+pulumiverse_buildkite/cluster/get_cluster.py
 pulumiverse_buildkite/config/__init__.py
 pulumiverse_buildkite/config/vars.py
 pulumiverse_buildkite/organization/__init__.py
 pulumiverse_buildkite/organization/get_organization.py
 pulumiverse_buildkite/organization/settings.py
 pulumiverse_buildkite/pipeline/__init__.py
 pulumiverse_buildkite/pipeline/_inputs.py
```

### Comparing `pulumiverse_buildkite-2.2.0/setup.py` & `pulumiverse_buildkite-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.2.0"
-PLUGIN_VERSION = "2.2.0"
+VERSION = "2.3.0"
+PLUGIN_VERSION = "2.3.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'buildkite', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-buildkite'])
         except OSError as error:
```

