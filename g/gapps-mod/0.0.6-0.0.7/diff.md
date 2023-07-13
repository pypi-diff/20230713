# Comparing `tmp/gapps-mod-0.0.6.tar.gz` & `tmp/gapps-mod-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gapps-mod-0.0.6.tar", last modified: Thu Jul 13 20:05:38 2023, max compression
+gzip compressed data, was "gapps-mod-0.0.7.tar", last modified: Thu Jul 13 21:19:11 2023, max compression
```

## Comparing `gapps-mod-0.0.6.tar` & `gapps-mod-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 20:05:38.354861 gapps-mod-0.0.6/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.6/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-13 20:05:38.354861 gapps-mod-0.0.6/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.6/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    15862 2023-07-13 20:05:02.000000 gapps-mod-0.0.6/gapps.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 20:05:38.354861 gapps-mod-0.0.6/gapps_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-13 20:05:38.000000 gapps-mod-0.0.6/gapps_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2023-07-13 20:05:38.000000 gapps-mod-0.0.6/gapps_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-13 20:05:38.000000 gapps-mod-0.0.6/gapps_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2023-07-13 20:05:38.000000 gapps-mod-0.0.6/gapps_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-07-13 20:05:38.000000 gapps-mod-0.0.6/gapps_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.6/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2023-07-13 20:05:38.354861 gapps-mod-0.0.6/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.6/setup.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 21:19:11.738800 gapps-mod-0.0.7/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2021-09-13 01:50:00.000000 gapps-mod-0.0.7/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-13 21:19:11.742800 gapps-mod-0.0.7/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       68 2022-03-13 21:47:12.000000 gapps-mod-0.0.7/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    16426 2023-07-13 21:18:21.000000 gapps-mod-0.0.7/gapps.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-07-13 21:19:11.738800 gapps-mod-0.0.7/gapps_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      601 2023-07-13 21:19:11.000000 gapps-mod-0.0.7/gapps_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      224 2023-07-13 21:19:11.000000 gapps-mod-0.0.7/gapps_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-07-13 21:19:11.000000 gapps-mod-0.0.7/gapps_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      102 2023-07-13 21:19:11.000000 gapps-mod-0.0.7/gapps_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        6 2023-07-13 21:19:11.000000 gapps-mod-0.0.7/gapps_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-13 21:42:41.000000 gapps-mod-0.0.7/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      838 2023-07-13 21:19:11.742800 gapps-mod-0.0.7/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 21:42:00.000000 gapps-mod-0.0.7/setup.py
```

### Comparing `gapps-mod-0.0.6/LICENSE` & `gapps-mod-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gapps-mod-0.0.6/PKG-INFO` & `gapps-mod-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapps-mod
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper for some Google App functionality (Sheets and email mostly)
 Home-page: https://github.com/ejohnfel/gapps
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/gapps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gapps-mod-0.0.6/gapps.py` & `gapps-mod-0.0.7/gapps.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 #
 # Variables
 #
 
 # Version Stuff
-VERSION=(0,0,6)
+VERSION=(0,0,7)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Config Location (if in Use)
 GappsConfigSection = "gapps"
 GappsCredsValue = "gappscreds"
 GappsTokenValue = "gappstoken"
 
@@ -60,15 +60,16 @@
 Config = None
 GappsConfig = None
 
 # Gapps App Scopes
 GappsAppScopes = {
 	"spreadsheets.readonly" : "https://www.googleapis.com/auth/spreadsheets.readonly",
 	"gmail.readonly" : "https://www.googleapis.com/auth/gmail.readonly",
-	"gmail" : "https://mail.google.com/"
+	"gmail" : "https://mail.google.com/",
+	"delegate" : "https://gmail.googleapis.com/gmail/v1/users/{userId}/settings/delegates/{delegateEmail}"
 }
 
 # Official Service Names Translation Table
 ServiceNames = {
 	"sheets" : "sheets",
 	"gmail" : "gmail",
 	"email" : "gmail"
@@ -666,23 +667,33 @@
 	DebugMode(True)
 	ModuleMode(True)
 
 	parser = argparse.ArgumentParser(description="Gapps Module")
 
 	parser.add_argument("-c","--creds",default="credentials.txt",required=False,help="Credentials file")
 	parser.add_argument("-t","--token",default="token.txt",required=False,help="Access token file")
+	parser.add_argument("-s","--scope",choices=GappsAppScopes.values(),default="spreadsheets.readonly",help="Scope for operations")
 	parser.add_argument("cmd",choices=["test","reauth"],help="Command to execute")
 
 	args = parser.parse_args()
 
+	Scope = CredsFile = TokenFile = None
+
 	if args.creds is not None:
 		CredsFile = args.creds
 
 	if args.token is not None:
 		TokenFile = args.token
 
+	if args.scope is noe None:
+		Scope = args.scope
+
 	if args.cmd is not None:
 		if args.cmd == "test":
 			test()
-		elif args.cmd == "reauth":
-			scopes = BuildScopes("spreadsheets.readonly")
-			creds = ReAuthToken(TokenFile,scopes)
+		elif args.cmd == "reauth" and Scope is not None and CredsFile is not None and TokenFile is not None:
+			scopes = BuildScopes(args.scope)
+			creds = ReAuthToken(CredsFile,scopes)
+			with open(TokenFile,"w") as token:
+				token.write(creds.to_json())
+		else:
+			Msg(f"Command {args.cmd} not understood or you are missing some options to complete the command")
```

### Comparing `gapps-mod-0.0.6/gapps_mod.egg-info/PKG-INFO` & `gapps-mod-0.0.7/gapps_mod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gapps-mod
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper for some Google App functionality (Sheets and email mostly)
 Home-page: https://github.com/ejohnfel/gapps
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 Project-URL: Bug Tracker, https://github.com/ejohnfel/gapps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gapps-mod-0.0.6/setup.cfg` & `gapps-mod-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = gapps-mod
-version = 0.0.6
+version = 0.0.7
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = A wrapper for some Google App functionality (Sheets and email mostly)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/gapps
 project_urls =
```

