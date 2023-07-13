# Comparing `tmp/nvosscript-1.3.7.tar.gz` & `tmp/nvosscript-1.3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.7.tar", last modified: Wed Jun 21 02:50:00 2023, max compression
+gzip compressed data, was "nvosscript-1.3.7.2.tar", last modified: Thu Jul 13 02:51:05 2023, max compression
```

## Comparing `nvosscript-1.3.7.tar` & `nvosscript-1.3.7.2.tar`

### file list

```diff
@@ -1,30 +1,46 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.291493 nvosscript-1.3.7/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.7/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-21 02:50:00.291348 nvosscript-1.3.7/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.7/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.287919 nvosscript-1.3.7/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.7/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    13886 2023-06-20 08:38:00.000000 nvosscript-1.3.7/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     8909 2023-06-21 02:49:18.000000 nvosscript-1.3.7/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.7/nvos/run.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.288755 nvosscript-1.3.7/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-06-21 02:50:00.000000 nvosscript-1.3.7/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-06-21 02:50:00.291557 nvosscript-1.3.7/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-06-21 02:49:53.000000 nvosscript-1.3.7/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.289775 nvosscript-1.3.7/skyeye/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.7/skyeye/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.7/skyeye/handler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.7/skyeye/loghandler.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     2531 2023-06-14 01:42:31.000000 nvosscript-1.3.7/skyeye/remote.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.290808 nvosscript-1.3.7/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.7/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1803 2023-06-21 02:43:40.000000 nvosscript-1.3.7/start/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-06-21 02:49:49.000000 nvosscript-1.3.7/start/main.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.7/start/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-21 02:50:00.291036 nvosscript-1.3.7/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.7/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.925035 nvosscript-1.3.7.2/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-07-13 02:51:05.924879 nvosscript-1.3.7.2/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.917977 nvosscript-1.3.7.2/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.7.2/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    15134 2023-07-13 02:50:36.000000 nvosscript-1.3.7.2/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     8909 2023-07-04 01:26:21.000000 nvosscript-1.3.7.2/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6293 2023-06-20 02:23:27.000000 nvosscript-1.3.7.2/nvos/run.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.919036 nvosscript-1.3.7.2/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-07-13 02:51:05.000000 nvosscript-1.3.7.2/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-07-13 02:51:05.925083 nvosscript-1.3.7.2/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-07-13 01:14:55.000000 nvosscript-1.3.7.2/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.919768 nvosscript-1.3.7.2/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.7.2/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.7.2/skyeye/handler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      802 2023-06-19 10:04:39.000000 nvosscript-1.3.7.2/skyeye/loghandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     2531 2023-06-19 10:04:39.000000 nvosscript-1.3.7.2/skyeye/remote.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.920541 nvosscript-1.3.7.2/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.7.2/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1803 2023-07-04 01:26:21.000000 nvosscript-1.3.7.2/start/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4503 2023-07-13 01:15:00.000000 nvosscript-1.3.7.2/start/main.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1182 2023-06-20 02:18:44.000000 nvosscript-1.3.7.2/start/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.916097 nvosscript-1.3.7.2/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.924265 nvosscript-1.3.7.2/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.7.2/venv/bin/activate_this.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.7.2/venv/bin/jp.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.7.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-07-13 02:51:05.924501 nvosscript-1.3.7.2/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.7.2/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.7/LICENSE` & `nvosscript-1.3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/nvos/file.py` & `nvosscript-1.3.7.2/nvos/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,26 +151,26 @@
         else:
             exit_git_data.append(project_space)
     if len(not_exit_git_data) == 0:
         project_space_list.clear()
         for project_space in exit_git_data:
             # if project_space["git_branch"] != "(no branch)":
             project_space_list.append(project_space)
-        return project_space_list
+        return filter_ecus_dir(project_space_list)
     if len(exit_git_data) == 0:
         result_list = []
         for file_path in os.listdir(workspace_path):
             if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
                 continue
             if os.path.isdir(os.path.join(workspace_path, file_path)):
                 temp = {"project_space": os.path.join(workspace_path, file_path),
                         "fileDirectory": os.path.join(workspace_path, file_path),
                         "git_branch": "nvos_default", "gitBranch": "nvos_default"}
                 result_list.append(temp)
-        return result_list
+        return filter_ecus_dir(result_list)
 
     filter_exit_data = []
     for project_space in not_exit_git_data:
         max_prefix = ""
         max_public_str = ""
 
         for item in exit_git_data:
@@ -199,16 +199,41 @@
         if flag:
             filter_duplicate.append(item)
     project_space_list.clear()
     for project_space in exit_git_data:
         # if project_space["git_branch"] != "(no branch)":
         project_space_list.append(project_space)
     project_space_list.extend(filter_duplicate)
-    return project_space_list
 
+    # 再过滤一次ecus的目录
+    return filter_ecus_dir(project_space_list)
+
+def filter_ecus_dir(project_space_list):
+    final_project_space_list = []
+    for item in project_space_list:
+        # 取当前目录
+        now_dir = item["fileDirectory"]
+        # 发现是xxxx/xxx/ecus
+        if os.path.basename(now_dir) == "ecus":
+            git_branch = get_current_git_branch(now_dir)
+            for name in os.listdir(now_dir):
+                if name == ".idea" or name == ".repo" or name == ".ndtc" or name == ".DS_Store" or name == ".git" or name == ".gitignore":
+                    continue
+                sub_dir = os.path.join(now_dir, name)
+                if os.path.isdir(sub_dir):
+                    if len(git_branch) == 0:
+                        git_branch = get_current_git_branch(sub_dir)
+                        if len(git_branch) == 0:
+                            git_branch = "nvos_default"
+                    temp = {"project_space": sub_dir, "fileDirectory": sub_dir,
+                            "git_branch": git_branch, "gitBranch": git_branch}
+                    final_project_space_list.append(temp)
+        else:
+            final_project_space_list.append(item)
+    return final_project_space_list
 
 def get_current_git_branch(workspace_path):
     git_path = os.path.join(workspace_path, ".git")
     if not os.path.exists(git_path):
         return ""
 
     try:
```

### Comparing `nvosscript-1.3.7/nvos/remote.py` & `nvosscript-1.3.7.2/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/nvos/run.py` & `nvosscript-1.3.7.2/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/setup.py` & `nvosscript-1.3.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.7',
+    version='1.3.7.02',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.7/skyeye/loghandler.py` & `nvosscript-1.3.7.2/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/skyeye/remote.py` & `nvosscript-1.3.7.2/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/start/login.py` & `nvosscript-1.3.7.2/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/start/main.py` & `nvosscript-1.3.7.2/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.7")
+        print("1.3.7.02")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.7/start/utils.py` & `nvosscript-1.3.7.2/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.7/win/win_auto_script.py` & `nvosscript-1.3.7.2/win/win_auto_script.py`

 * *Files identical despite different names*

