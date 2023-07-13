# Comparing `tmp/agentmemory-0.1.9.tar.gz` & `tmp/agentmemory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.1.9.tar", last modified: Mon Jul 10 23:05:34 2023, max compression
+gzip compressed data, was "agentmemory-0.2.0.tar", last modified: Thu Jul 13 02:27:52 2023, max compression
```

## Comparing `agentmemory-0.1.9.tar` & `agentmemory-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.312327 agentmemory-0.1.9/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.1.9/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     5834 2023-07-10 23:05:34.312152 agentmemory-0.1.9/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     5231 2023-07-10 22:49:00.000000 agentmemory-0.1.9/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.310574 agentmemory-0.1.9/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)      622 2023-07-10 23:05:30.000000 agentmemory-0.1.9/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    14173 2023-07-10 23:04:22.000000 agentmemory-0.1.9/agentmemory/main.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     2367 2023-07-10 23:02:02.000000 agentmemory-0.1.9/agentmemory/test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 23:05:34.311907 agentmemory-0.1.9/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     5834 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      264 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-10 23:05:34.000000 agentmemory-0.1.9/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 23:05:34.312381 agentmemory-0.1.9/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-10 23:05:30.000000 agentmemory-0.1.9/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.092797 agentmemory-0.2.0/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.0/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-13 02:27:52.092539 agentmemory-0.2.0/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-13 02:18:43.000000 agentmemory-0.2.0/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.091037 agentmemory-0.2.0/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1103 2023-07-13 02:27:48.000000 agentmemory-0.2.0/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    24183 2023-07-13 02:25:22.000000 agentmemory-0.2.0/agentmemory/main.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.092299 agentmemory-0.2.0/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-13 02:27:52.092871 agentmemory-0.2.0/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-13 02:27:48.000000 agentmemory-0.2.0/setup.py
```

### Comparing `agentmemory-0.1.9/LICENSE` & `agentmemory-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.1.9/setup.py` & `agentmemory-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.1.9',
+    version='0.2.0',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

