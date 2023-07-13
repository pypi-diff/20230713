# Comparing `tmp/puwifi-1.0.5.tar.gz` & `tmp/puwifi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puwifi-1.0.5.tar", last modified: Thu Jul 13 09:34:14 2023, max compression
+gzip compressed data, was "puwifi-1.0.6.tar", last modified: Thu Jul 13 15:56:37 2023, max compression
```

## Comparing `puwifi-1.0.5.tar` & `puwifi-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.5/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/.github/
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.5/.github/workflows/pylint.yml
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.5/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:34:14.814235 puwifi-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-10 18:08:53.000000 puwifi-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:34:14.814235 puwifi-1.0.5/puwifi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3867 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 09:34:14.000000 puwifi-1.0.5/puwifi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9136 2023-07-13 09:32:09.000000 puwifi-1.0.5/puwifi.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-13 09:34:07.000000 puwifi-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.5/renovate.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 09:34:14.814235 puwifi-1.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-10 14:39:51.000000 puwifi-1.0.6/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/.github/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-10 14:39:51.000000 puwifi-1.0.6/.github/workflows/pylint.yml
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-10 17:52:26.000000 puwifi-1.0.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-07-10 17:52:26.000000 puwifi-1.0.6/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-10 14:39:51.000000 puwifi-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-13 15:56:37.157200 puwifi-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-07-13 15:53:55.000000 puwifi-1.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-13 15:56:28.000000 puwifi-1.0.6/main.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-13 15:54:51.000000 puwifi-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-10 14:39:51.000000 puwifi-1.0.6/renovate.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 14:39:51.000000 puwifi-1.0.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 15:56:37.157200 puwifi-1.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 15:56:37.157200 puwifi-1.0.6/src/puwifi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 15:56:37.000000 puwifi-1.0.6/src/puwifi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9016 2023-07-13 15:45:57.000000 puwifi-1.0.6/src/puwifi.py
```

### Comparing `puwifi-1.0.5/.github/workflows/codeql-analysis.yml` & `puwifi-1.0.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.5/.github/workflows/pylint.yml` & `puwifi-1.0.6/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.5/.gitignore` & `puwifi-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.5/.pylintrc` & `puwifi-1.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.5/LICENSE` & `puwifi-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `puwifi-1.0.5/PKG-INFO` & `puwifi-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puwifi
-Version: 1.0.5
+Version: 1.0.6
 Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
 Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
 Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
 Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,45 +36,41 @@
 
 - make sure you installed `python` and `pip` in your OS
 
 ```bash
 pip install puwifi
 ```
 
-### Manuall Installation
-- make sure you installed python in your OS
-
-```bash
-git clone https://github.com/SaicharanKandukuri/puwifi
-cd puwifi
-pip install -r requirements.txt
-```
 ## Usage
 
 #### General
 
 ##### ♾️ Forever login mode `-k`
 this is what the aim of repo
 
 `-k` or `--keep-alive` attribute is say script to run a forever loop!
 > scripts tries to contact `google.com` if connection fails script tries to send login request to host *i.e: 10.0.0.1* with username & password provied with `-u` & `-p` arguments
-```cmd
-python3 puwifi.py -k -u YOUR_USERNAME -p YOUR_PASSWORD 
+
+
+```bash
+puwifi -k -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
 
 ##### 🪵 One-time login `-l`
 you can login with `-l` or `--login` argument
-```cmd
-python3 puwifi.py -l -u YOUR_USERNAME -p YOUR_PASSWORD
+
+```bash
+puwifi -l -u YOUR_USERNAME -p YOUR_PASSWORD
 ```
 ##### 💥 Logout from puwifi
 for logout use option `-o` or `--logout` argument
-```cmd
-python3 puwifi.py -o -u YOUR_USERNAME -p YOUR_PASSWORD 
+```bash
+puwifi -o -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
+
 <!--
 > idk why logout requires username and password too! ( vunerability ? )
 --> 
 
 <hr>
 
 ## Finally
```

### Comparing `puwifi-1.0.5/README.md` & `puwifi-1.0.6/src/puwifi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: puwifi
+Version: 1.0.6
+Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
+Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
+Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
+Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PU-wifi
 A python program that simulates [parul university](https://www.google.com/search?q=parul+university) wifi web authentication request process to keep you device connected to parul university wifi (with-a-loop)
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
@@ -22,45 +36,41 @@
 
 - make sure you installed `python` and `pip` in your OS
 
 ```bash
 pip install puwifi
 ```
 
-### Manuall Installation
-- make sure you installed python in your OS
-
-```bash
-git clone https://github.com/SaicharanKandukuri/puwifi
-cd puwifi
-pip install -r requirements.txt
-```
 ## Usage
 
 #### General
 
 ##### ♾️ Forever login mode `-k`
 this is what the aim of repo
 
 `-k` or `--keep-alive` attribute is say script to run a forever loop!
 > scripts tries to contact `google.com` if connection fails script tries to send login request to host *i.e: 10.0.0.1* with username & password provied with `-u` & `-p` arguments
-```cmd
-python3 puwifi.py -k -u YOUR_USERNAME -p YOUR_PASSWORD 
+
+
+```bash
+puwifi -k -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
 
 ##### 🪵 One-time login `-l`
 you can login with `-l` or `--login` argument
-```cmd
-python3 puwifi.py -l -u YOUR_USERNAME -p YOUR_PASSWORD
+
+```bash
+puwifi -l -u YOUR_USERNAME -p YOUR_PASSWORD
 ```
 ##### 💥 Logout from puwifi
 for logout use option `-o` or `--logout` argument
-```cmd
-python3 puwifi.py -o -u YOUR_USERNAME -p YOUR_PASSWORD 
+```bash
+puwifi -o -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
+
 <!--
 > idk why logout requires username and password too! ( vunerability ? )
 --> 
 
 <hr>
 
 ## Finally
```

### Comparing `puwifi-1.0.5/puwifi.egg-info/PKG-INFO` & `puwifi-1.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: puwifi
-Version: 1.0.5
-Summary: ⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever
-Author-email: SaicharanKandukuri <saicharankandukuri1x1@gmail.com>
-Project-URL: Homepage, https://github.com/SaicharanKandukuri/puwifi
-Project-URL: Bug Tracker, https://github.com/SaicharanKandukuri/puwifi/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PU-wifi
 A python program that simulates [parul university](https://www.google.com/search?q=parul+university) wifi web authentication request process to keep you device connected to parul university wifi (with-a-loop)
 
 ![image](https://user-images.githubusercontent.com/68287637/146675073-7e1aebcc-056d-4351-b5aa-f7e2f57b1853.png)
 
 <!--
 ![image](https://user-images.githubusercontent.com/68287637/146674599-1568723d-6c70-49e8-8d71-1275ab3b169d.png)
@@ -36,45 +22,41 @@
 
 - make sure you installed `python` and `pip` in your OS
 
 ```bash
 pip install puwifi
 ```
 
-### Manuall Installation
-- make sure you installed python in your OS
-
-```bash
-git clone https://github.com/SaicharanKandukuri/puwifi
-cd puwifi
-pip install -r requirements.txt
-```
 ## Usage
 
 #### General
 
 ##### ♾️ Forever login mode `-k`
 this is what the aim of repo
 
 `-k` or `--keep-alive` attribute is say script to run a forever loop!
 > scripts tries to contact `google.com` if connection fails script tries to send login request to host *i.e: 10.0.0.1* with username & password provied with `-u` & `-p` arguments
-```cmd
-python3 puwifi.py -k -u YOUR_USERNAME -p YOUR_PASSWORD 
+
+
+```bash
+puwifi -k -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
 
 ##### 🪵 One-time login `-l`
 you can login with `-l` or `--login` argument
-```cmd
-python3 puwifi.py -l -u YOUR_USERNAME -p YOUR_PASSWORD
+
+```bash
+puwifi -l -u YOUR_USERNAME -p YOUR_PASSWORD
 ```
 ##### 💥 Logout from puwifi
 for logout use option `-o` or `--logout` argument
-```cmd
-python3 puwifi.py -o -u YOUR_USERNAME -p YOUR_PASSWORD 
+```bash
+puwifi -o -u YOUR_USERNAME -p YOUR_PASSWORD 
 ```
+
 <!--
 > idk why logout requires username and password too! ( vunerability ? )
 --> 
 
 <hr>
 
 ## Finally
```

### Comparing `puwifi-1.0.5/puwifi.py` & `puwifi-1.0.6/src/puwifi.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,20 +43,17 @@
 logging.disable('DEBUG')
 
 log = logging.getLogger("rich")
 
 
 class WifiUtils:
     """class for wifi utils"""
-    def __init__(self, username, password, host, port):
-        self.username = username
-        self.password = password
-        self.host = host
-        self.port = port
-
+    def __init__(self):
+        pass
+    
     def pw_request(self,
                 method,
                 username,
                 password,
                 host, port,
                 timeout) -> list:
         """request method: sends request to wifi host
@@ -218,34 +215,36 @@
     parser.add_argument('-o', '--logout', action='store_true',
                       help='logout from wifi', default=False)
     parser.add_argument('-l', '--login', action='store_true',
                       help='login to wifi', default=False)
     
     args = parser.parse_args()
     
+    wu = WifiUtils()
+    
     if not sys.argv[1:]:
         print("no arguments passed")
         print(parser.print_help())
     
     if args.login:
         log.info("=> login <=")
-        log.info(WifiUtils.login(args.username,
+        log.info(wu.login(args.username,
                          args.password,
                          args.host, args.port,
                         ))
         sys.exit(0)
     
     if args.logout:
         log.info("=> logout <=")
-        log.info(WifiUtils.logout(args.username,
+        log.info(wu.logout(args.username,
                           args.password,
                           args.host, args.port,
                           ))
         sys.exit(0)
     
     if args.keep_alive:
         log.info("=> keep alive <=")
         keep_alive(args.username,
                    args.password,
                    args.host, args.port,
                    )
-    
+
```

### Comparing `puwifi-1.0.5/pyproject.toml` & `puwifi-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="puwifi"
-version="1.0.5"
+version="1.0.6"
 
 authors = [
     { name="SaicharanKandukuri", email="saicharankandukuri1x1@gmail.com"}
 ]
 
 description = "⚡ A script made to automate the wifi login process to Parul university routers. login to wifi forever"
 readme = "README.md"
```

