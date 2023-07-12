# Comparing `tmp/pyGitInfo-0.0.2.tar.gz` & `tmp/pyGitInfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGitInfo-0.0.2.tar", last modified: Wed Jul 12 23:21:48 2023, max compression
+gzip compressed data, was "pyGitInfo-0.0.3.tar", last modified: Wed Jul 12 23:22:53 2023, max compression
```

## Comparing `pyGitInfo-0.0.2.tar` & `pyGitInfo-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:21:48.855403 pyGitInfo-0.0.2/
--rw-rw-rw-   0        0        0     1199 2023-07-12 19:26:07.000000 pyGitInfo-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5083 2023-07-12 23:21:48.854406 pyGitInfo-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4299 2023-07-12 19:27:46.000000 pyGitInfo-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 23:21:48.832464 pyGitInfo-0.0.2/pyGitInfo/
--rw-rw-rw-   0        0        0       26 2023-07-12 23:12:04.000000 pyGitInfo-0.0.2/pyGitInfo/__init__.py
--rw-rw-rw-   0        0        0    11119 2023-07-12 22:58:20.000000 pyGitInfo-0.0.2/pyGitInfo/pyGitInfo.py
-drwxrwxrwx   0        0        0        0 2023-07-12 23:21:48.852413 pyGitInfo-0.0.2/pyGitInfo.egg-info/
--rw-rw-rw-   0        0        0     5083 2023-07-12 23:21:48.000000 pyGitInfo-0.0.2/pyGitInfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-12 23:21:48.000000 pyGitInfo-0.0.2/pyGitInfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:21:48.000000 pyGitInfo-0.0.2/pyGitInfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-12 23:21:48.000000 pyGitInfo-0.0.2/pyGitInfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 23:21:48.000000 pyGitInfo-0.0.2/pyGitInfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:21:48.856400 pyGitInfo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      966 2023-07-12 23:21:33.000000 pyGitInfo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:22:53.026157 pyGitInfo-0.0.3/
+-rw-rw-rw-   0        0        0     1199 2023-07-12 19:26:07.000000 pyGitInfo-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5083 2023-07-12 23:22:53.025160 pyGitInfo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4299 2023-07-12 19:27:46.000000 pyGitInfo-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 23:22:53.004217 pyGitInfo-0.0.3/pyGitInfo/
+-rw-rw-rw-   0        0        0       26 2023-07-12 23:12:04.000000 pyGitInfo-0.0.3/pyGitInfo/__init__.py
+-rw-rw-rw-   0        0        0    11119 2023-07-12 22:58:20.000000 pyGitInfo-0.0.3/pyGitInfo/pyGitInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-12 23:22:53.024163 pyGitInfo-0.0.3/pyGitInfo.egg-info/
+-rw-rw-rw-   0        0        0     5083 2023-07-12 23:22:52.000000 pyGitInfo-0.0.3/pyGitInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-12 23:22:52.000000 pyGitInfo-0.0.3/pyGitInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 23:22:52.000000 pyGitInfo-0.0.3/pyGitInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-12 23:22:52.000000 pyGitInfo-0.0.3/pyGitInfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 23:22:52.000000 pyGitInfo-0.0.3/pyGitInfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 23:22:53.026157 pyGitInfo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-07-12 23:22:35.000000 pyGitInfo-0.0.3/setup.py
```

### Comparing `pyGitInfo-0.0.2/LICENSE` & `pyGitInfo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGitInfo-0.0.2/PKG-INFO` & `pyGitInfo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGitInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analisador de repositórios do github
 Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
 Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
 License: MIT License
 Keywords: gitInfo,github,git,relatorio,reports,gitReports
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyGitInfo-0.0.2/README.md` & `pyGitInfo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyGitInfo-0.0.2/pyGitInfo/pyGitInfo.py` & `pyGitInfo-0.0.3/pyGitInfo/pyGitInfo.py`

 * *Files identical despite different names*

### Comparing `pyGitInfo-0.0.2/pyGitInfo.egg-info/PKG-INFO` & `pyGitInfo-0.0.3/pyGitInfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGitInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analisador de repositórios do github
 Author: ['Catlen Cleane', 'Felipe Direito', 'Gabriel Rosa', 'Gabriel Zaranza', 'Rafael Kenji', 'Lucas Lobão', 'Vinicius de Oliveira']
 Author-email: catlen.cleane@hotmail.com, fedireito92@gmail.com, gabriel10919@outlook.com, gabrielzaranza@hotmail.com, rafak.taira@gmail.com, lucaslobao14df@gmail.com, viniciusoliveirasp22@gmail.com
 License: MIT License
 Keywords: gitInfo,github,git,relatorio,reports,gitReports
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

