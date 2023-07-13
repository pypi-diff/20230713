# Comparing `tmp/mflag-1.6.8.tar.gz` & `tmp/mflag-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflag-1.6.8.tar", last modified: Fri Jul  7 11:36:22 2023, max compression
+gzip compressed data, was "mflag-1.6.9.tar", last modified: Thu Jul 13 12:04:21 2023, max compression
```

## Comparing `mflag-1.6.8.tar` & `mflag-1.6.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1071 2023-06-24 10:44:31.000000 mflag-1.6.8/LICENSE
--rw-r--r--   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-07 11:36:22.879390 mflag-1.6.8/PKG-INFO
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2026 2023-06-24 10:44:31.000000 mflag-1.6.8/README.md
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.878390 mflag-1.6.8/mflag/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      226 2023-07-05 10:21:55.000000 mflag-1.6.8/mflag/__init__.py
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     4559 2023-06-26 13:11:50.000000 mflag-1.6.8/mflag/src/flag.py
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.878390 mflag-1.6.8/mflag/src/rcmng/
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/client/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1631 2023-06-24 10:41:50.000000 mflag-1.6.8/mflag/src/rcmng/client/__init__.py
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      433 2023-06-24 09:19:59.000000 mflag-1.6.8/mflag/src/rcmng/client/run.py
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/server/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     6819 2023-07-05 10:21:40.000000 mflag-1.6.8/mflag/src/rcmng/server/__init__.py
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      255 2023-06-24 08:55:53.000000 mflag-1.6.8/mflag/src/rcmng/server/run.py
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag/src/rcmng/submit/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      844 2023-06-24 10:18:10.000000 mflag-1.6.8/mflag/src/rcmng/submit/__init__.py
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      444 2023-06-24 10:33:05.000000 mflag-1.6.8/mflag/src/rcmng/submit/run.py
-drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-07 11:36:22.879390 mflag-1.6.8/mflag.egg-info/
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/PKG-INFO
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      401 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/SOURCES.txt
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        1 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/dependency_links.txt
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)       26 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/requires.txt
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        6 2023-07-07 11:36:22.000000 mflag-1.6.8/mflag.egg-info/top_level.txt
--rw-r--r--   0 moses     (1000) sftpgroup  (1002)       38 2023-07-07 11:36:22.879390 mflag-1.6.8/setup.cfg
--rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      516 2023-06-26 13:13:56.000000 mflag-1.6.8/setup.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.245553 mflag-1.6.9/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1071 2023-06-24 10:44:31.000000 mflag-1.6.9/LICENSE
+-rw-r--r--   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-13 12:04:21.245553 mflag-1.6.9/PKG-INFO
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2026 2023-06-24 10:44:31.000000 mflag-1.6.9/README.md
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.244553 mflag-1.6.9/mflag/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      226 2023-07-13 12:03:43.000000 mflag-1.6.9/mflag/__init__.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.244553 mflag-1.6.9/mflag/src/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     4667 2023-07-13 12:03:25.000000 mflag-1.6.9/mflag/src/flag.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.244553 mflag-1.6.9/mflag/src/rcmng/
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.245553 mflag-1.6.9/mflag/src/rcmng/client/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     1631 2023-06-24 10:41:50.000000 mflag-1.6.9/mflag/src/rcmng/client/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      433 2023-06-24 09:19:59.000000 mflag-1.6.9/mflag/src/rcmng/client/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.245553 mflag-1.6.9/mflag/src/rcmng/server/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     6819 2023-07-05 10:21:40.000000 mflag-1.6.9/mflag/src/rcmng/server/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      255 2023-06-24 08:55:53.000000 mflag-1.6.9/mflag/src/rcmng/server/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.245553 mflag-1.6.9/mflag/src/rcmng/submit/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      844 2023-06-24 10:18:10.000000 mflag-1.6.9/mflag/src/rcmng/submit/__init__.py
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      444 2023-06-24 10:33:05.000000 mflag-1.6.9/mflag/src/rcmng/submit/run.py
+drwxr-xr-x   0 moses     (1000) sftpgroup  (1002)        0 2023-07-13 12:04:21.244553 mflag-1.6.9/mflag.egg-info/
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)     2209 2023-07-13 12:04:21.000000 mflag-1.6.9/mflag.egg-info/PKG-INFO
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      401 2023-07-13 12:04:21.000000 mflag-1.6.9/mflag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        1 2023-07-13 12:04:21.000000 mflag-1.6.9/mflag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)       26 2023-07-13 12:04:21.000000 mflag-1.6.9/mflag.egg-info/requires.txt
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)        6 2023-07-13 12:04:21.000000 mflag-1.6.9/mflag.egg-info/top_level.txt
+-rw-r--r--   0 moses     (1000) sftpgroup  (1002)       38 2023-07-13 12:04:21.245553 mflag-1.6.9/setup.cfg
+-rwxrwxrwx   0 moses     (1000) sftpgroup  (1002)      516 2023-06-26 13:13:56.000000 mflag-1.6.9/setup.py
```

### Comparing `mflag-1.6.8/LICENSE` & `mflag-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mflag-1.6.8/PKG-INFO` & `mflag-1.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.8
+Version: 1.6.9
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.8/README.md` & `mflag-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `mflag-1.6.8/mflag/src/flag.py` & `mflag-1.6.9/mflag/src/flag.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         
     def __initial_check(self):
         os.makedirs(self.job_dir_path, exist_ok=True)
     
     def __is_job_done(self):
         if not os.path.exists(self.job_file_path):
             job_dict = {'job_id':self.job_id, 'job_name':self.job_name, 'job_description':self.job_description, 'process_name':self.process_name, 'issue_date':str(datetime.now())}
+            dir_path = os.path.dirname(self.job_file_path)
+            os.makedirs(dir_path, exist_ok=True)
             with open(self.job_file_path, 'w') as f:
                 json.dump(job_dict, f)
             return False
         else:
             with open(self.job_file_path, 'r') as f:
                 job_dict = json.load(f)
                 if 'finish_date' in job_dict.keys():
```

### Comparing `mflag-1.6.8/mflag/src/rcmng/client/__init__.py` & `mflag-1.6.9/mflag/src/rcmng/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.8/mflag/src/rcmng/server/__init__.py` & `mflag-1.6.9/mflag/src/rcmng/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.8/mflag/src/rcmng/submit/__init__.py` & `mflag-1.6.9/mflag/src/rcmng/submit/__init__.py`

 * *Files identical despite different names*

### Comparing `mflag-1.6.8/mflag.egg-info/PKG-INFO` & `mflag-1.6.9/mflag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflag
-Version: 1.6.8
+Version: 1.6.9
 Summary: put/remove flags for files and folders
 Author: Moses Dastmard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mflag: powerful Python toolkit for mark/unmark files and directories 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pandas.svg)](https://pypi.org/project/mflag/)
```

### Comparing `mflag-1.6.8/setup.py` & `mflag-1.6.9/setup.py`

 * *Files identical despite different names*

