# Comparing `tmp/paybybot3-0.0.32.tar.gz` & `tmp/paybybot3-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paybybot3-0.0.32.tar", last modified: Mon Apr 10 09:47:23 2023, max compression
+gzip compressed data, was "paybybot3-0.0.33.tar", last modified: Thu Jul 13 11:18:00 2023, max compression
```

## Comparing `paybybot3-0.0.32.tar` & `paybybot3-0.0.33.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.088106 paybybot3-0.0.32/
--rw-r--r--   0 rayhan     (503) staff       (20)     1080 2023-04-08 11:47:44.000000 paybybot3-0.0.32/LICENSE
--rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-10 09:47:23.087895 paybybot3-0.0.32/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     2168 2023-04-10 09:46:12.000000 paybybot3-0.0.32/README.md
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.086604 paybybot3-0.0.32/paybybot3/
--rw-r--r--   0 rayhan     (503) staff       (20)      177 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5649 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/__main__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     8197 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/bot.py
--rw-r--r--   0 rayhan     (503) staff       (20)      614 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/config.py
--rw-r--r--   0 rayhan     (503) staff       (20)      608 2023-04-10 09:46:12.000000 paybybot3-0.0.32/paybybot3/notifs.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 09:47:23.087665 paybybot3-0.0.32/paybybot3.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     2544 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      327 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       53 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/entry_points.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       22 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       10 2023-04-10 09:47:23.000000 paybybot3-0.0.32/paybybot3.egg-info/top_level.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-04-10 09:47:23.088156 paybybot3-0.0.32/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      761 2023-04-10 09:47:12.000000 paybybot3-0.0.32/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-13 11:18:00.282180 paybybot3-0.0.33/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1080 2023-04-08 11:47:44.000000 paybybot3-0.0.33/LICENSE
+-rw-r--r--   0 rayhan     (503) staff       (20)     2823 2023-07-13 11:18:00.282033 paybybot3-0.0.33/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     2436 2023-07-13 11:17:03.000000 paybybot3-0.0.33/README.md
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-13 11:18:00.280803 paybybot3-0.0.33/paybybot3/
+-rw-r--r--   0 rayhan     (503) staff       (20)      177 2023-04-10 09:46:12.000000 paybybot3-0.0.33/paybybot3/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     6009 2023-07-13 11:17:03.000000 paybybot3-0.0.33/paybybot3/__main__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     8352 2023-07-13 11:17:03.000000 paybybot3-0.0.33/paybybot3/bot.py
+-rw-r--r--   0 rayhan     (503) staff       (20)      614 2023-04-10 09:46:12.000000 paybybot3-0.0.33/paybybot3/config.py
+-rw-r--r--   0 rayhan     (503) staff       (20)      608 2023-04-10 09:46:12.000000 paybybot3-0.0.33/paybybot3/notifs.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-13 11:18:00.281841 paybybot3-0.0.33/paybybot3.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     2823 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      327 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       53 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/entry_points.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       22 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       10 2023-07-13 11:18:00.000000 paybybot3-0.0.33/paybybot3.egg-info/top_level.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-13 11:18:00.282235 paybybot3-0.0.33/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      772 2023-07-13 11:17:42.000000 paybybot3-0.0.33/setup.py
```

### Comparing `paybybot3-0.0.32/LICENSE` & `paybybot3-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.32/PKG-INFO` & `paybybot3-0.0.33/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: paybybot3
-Version: 0.0.32
+Version: 0.0.33
 Summary: CLI interface to https://www.paybyphone.fr/
 Home-page: https://github.com/rklf/paybybot3
-Author: Louis Abraham (louisabraham) and updated by rklf
+Author: rklf but originally created by Louis Abraham (louisabraham)
 Author-email: louis.abraham@yahoo.fr
 License: MIT
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,26 +34,28 @@
 
   1. Check if there is an ongoing subscription
 
   2. Else send a notification
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### check
 
 ```
 Usage: paybybot3 check [OPTIONS] CONFIG_NAME
 
   Check if there is an ongoing subscription
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### pay
 
 ```
 Usage: paybybot3 pay [OPTIONS] CONFIG_NAME
@@ -66,24 +68,40 @@
 
   4. Notify on failure
 
 Options:
   --location TEXT  [required]
   --rate INTEGER   [required]
   --duration TEXT  [required]
+  --config TEXT
+  --help           Show this message and exit.
+```
+
+### vehicles
+
+```
+Usage: paybybot3 vehicles [OPTIONS] CONFIG_NAME
+
+  1. Show the vehicles
+
+Options:
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### payment-accounts
 
 ```
 Usage: paybybot3 payment-accounts [OPTIONS] CONFIG_NAME
 
+  Show the payment accounts
+
 Options:
-  --help  Show this message and exit.
+  --config TEXT
+  --help         Show this message and exit.
 ```
 
 ## Configuration
 
 paybybot3 allows you to store your configuration in a YAML file `~/.config/paybybot3.yml`.
 
 Here is an example:
```

### Comparing `paybybot3-0.0.32/README.md` & `paybybot3-0.0.33/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,28 @@
 
   1. Check if there is an ongoing subscription
 
   2. Else send a notification
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### check
 
 ```
 Usage: paybybot3 check [OPTIONS] CONFIG_NAME
 
   Check if there is an ongoing subscription
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### pay
 
 ```
 Usage: paybybot3 pay [OPTIONS] CONFIG_NAME
@@ -53,24 +55,40 @@
 
   4. Notify on failure
 
 Options:
   --location TEXT  [required]
   --rate INTEGER   [required]
   --duration TEXT  [required]
+  --config TEXT
+  --help           Show this message and exit.
+```
+
+### vehicles
+
+```
+Usage: paybybot3 vehicles [OPTIONS] CONFIG_NAME
+
+  1. Show the vehicles
+
+Options:
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### payment-accounts
 
 ```
 Usage: paybybot3 payment-accounts [OPTIONS] CONFIG_NAME
 
+  Show the payment accounts
+
 Options:
-  --help  Show this message and exit.
+  --config TEXT
+  --help         Show this message and exit.
 ```
 
 ## Configuration
 
 paybybot3 allows you to store your configuration in a YAML file `~/.config/paybybot3.yml`.
 
 Here is an example:
```

### Comparing `paybybot3-0.0.32/paybybot3/__main__.py` & `paybybot3-0.0.33/paybybot3/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,9 +184,25 @@
                 ),
                 to=config["notify"],
             )
 
     catch_exceptions(config)(_pay)(config, location, duration)
 
 
+@cli.command()
+@click.argument("config_name")
+@click.option("--config", required=False, type=str)
+def vehicles(config_name, config):
+    """
+    Show the vehicles
+    """
+    config = get_config(config_name, config)
+
+    def _vehicles(config):
+        bot = connect(config)
+        pprint(bot.get_vehicles())
+
+    catch_exceptions(config)(_vehicles)(config)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `paybybot3-0.0.32/paybybot3/bot.py` & `paybybot3-0.0.33/paybybot3/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,14 +213,17 @@
             locationId=locationId,
             durationQuantity=durationQuantity,
             durationTimeUnit=durationTimeUnit,
             startTime=startTime,
         )
         return post.text
 
+    def get_vehicles(self):
+        return self._get("https://consumer.paybyphoneapis.com/identity/profileservice/v1/members/vehicles/paybyphone").json()
+
     def _request(self, method, url, **kwargs):
         return requests.request(
             method,
             url,
             headers={
                 **self.base_headers,
                 "Accept": "application/json, text/plain, */*",
```

### Comparing `paybybot3-0.0.32/paybybot3/config.py` & `paybybot3-0.0.33/paybybot3/config.py`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.32/paybybot3/notifs.py` & `paybybot3-0.0.33/paybybot3/notifs.py`

 * *Files identical despite different names*

### Comparing `paybybot3-0.0.32/paybybot3.egg-info/PKG-INFO` & `paybybot3-0.0.33/paybybot3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: paybybot3
-Version: 0.0.32
+Version: 0.0.33
 Summary: CLI interface to https://www.paybyphone.fr/
 Home-page: https://github.com/rklf/paybybot3
-Author: Louis Abraham (louisabraham) and updated by rklf
+Author: rklf but originally created by Louis Abraham (louisabraham)
 Author-email: louis.abraham@yahoo.fr
 License: MIT
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,26 +34,28 @@
 
   1. Check if there is an ongoing subscription
 
   2. Else send a notification
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### check
 
 ```
 Usage: paybybot3 check [OPTIONS] CONFIG_NAME
 
   Check if there is an ongoing subscription
 
 Options:
   --location TEXT
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### pay
 
 ```
 Usage: paybybot3 pay [OPTIONS] CONFIG_NAME
@@ -66,24 +68,40 @@
 
   4. Notify on failure
 
 Options:
   --location TEXT  [required]
   --rate INTEGER   [required]
   --duration TEXT  [required]
+  --config TEXT
+  --help           Show this message and exit.
+```
+
+### vehicles
+
+```
+Usage: paybybot3 vehicles [OPTIONS] CONFIG_NAME
+
+  1. Show the vehicles
+
+Options:
+  --config TEXT
   --help           Show this message and exit.
 ```
 
 ### payment-accounts
 
 ```
 Usage: paybybot3 payment-accounts [OPTIONS] CONFIG_NAME
 
+  Show the payment accounts
+
 Options:
-  --help  Show this message and exit.
+  --config TEXT
+  --help         Show this message and exit.
 ```
 
 ## Configuration
 
 paybybot3 allows you to store your configuration in a YAML file `~/.config/paybybot3.yml`.
 
 Here is an example:
```

### Comparing `paybybot3-0.0.32/setup.py` & `paybybot3-0.0.33/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="paybybot3",
-    version="0.0.32",
-    author="Louis Abraham (louisabraham) and updated by rklf",
+    version="0.0.33",
+    author="rklf but originally created by Louis Abraham (louisabraham)",
     license="MIT",
     author_email="louis.abraham@yahoo.fr",
     description="CLI interface to https://www.paybyphone.fr/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/rklf/paybybot3",
     packages=["paybybot3"],
```

