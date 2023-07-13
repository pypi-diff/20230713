# Comparing `tmp/huhk-1.6.4.tar.gz` & `tmp/huhk-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.4.tar", last modified: Wed Jul 12 07:15:40 2023, max compression
+gzip compressed data, was "huhk-1.6.5.tar", last modified: Thu Jul 13 08:03:46 2023, max compression
```

## Comparing `huhk-1.6.4.tar` & `huhk-1.6.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.340015 huhk-1.6.4/
--rw-rw-rw-   0        0        0      223 2023-07-12 07:15:40.339018 huhk-1.6.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.300121 huhk-1.6.4/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.317110 huhk-1.6.4/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      762 2023-07-12 06:28:58.000000 huhk-1.6.4/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.318087 huhk-1.6.4/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.337023 huhk-1.6.4/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.4/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.4/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.4/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    25666 2023-07-12 07:15:19.000000 huhk-1.6.4/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.308140 huhk-1.6.4/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 07:15:40.340015 huhk-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.424088 huhk-1.6.5/
+-rw-rw-rw-   0        0        0      223 2023-07-13 08:03:46.423091 huhk-1.6.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.341335 huhk-1.6.5/huhk/
+-rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.376216 huhk-1.6.5/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.5/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-13 08:03:45.000000 huhk-1.6.5/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29281 2023-07-13 01:55:03.000000 huhk-1.6.5/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.379215 huhk-1.6.5/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.421097 huhk-1.6.5/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.5/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2648 2023-07-13 01:44:43.000000 huhk-1.6.5/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.5/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.5/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    25687 2023-07-13 08:03:20.000000 huhk-1.6.5/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.355300 huhk-1.6.5/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 08:03:46.424088 huhk-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.5/setup.py
```

### Comparing `huhk-1.6.4/huhk/__init__.py` & `huhk-1.6.5/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/__main__.py` & `huhk-1.6.5/huhk/__main__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/case_project/base_project.py` & `huhk-1.6.5/huhk/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/case_project/json_coder.py` & `huhk-1.6.5/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/case_project/main.py` & `huhk-1.6.5/huhk/case_project/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from huhk.case_project.version import version as _version
 
 
 @click.command()
-@click.option('-v', '--version', help='线索版本', nargs=0)
-@click.option('-i', '--init', help='创建项目，参数项目key', required=False)
-@click.option('-u', '--update', help='更新项目，参数项目key', required=False)
+@click.option('-v', '--version', help='线索版本', default="$None$")
+@click.option('-i', '--init', help='创建项目，参数项目key', prompt="$None$", required=False)
+@click.option('-u', '--update', help='更新项目，参数项目key', default="$None$")
 def main(version, init, update):
     """Simple program that greets NAME for a total of COUNT times."""
     if version:
         click.echo('版本：' + _version)
         click.echo(type(version))
     elif init:
         click.echo('init：' + _version)
```

### Comparing `huhk-1.6.4/huhk/case_project/setup_set.py` & `huhk-1.6.5/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/init_project.py` & `huhk-1.6.5/huhk/init_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,44 +15,43 @@
         """api_type: 0时，value是swagger的api，json的url
                      1时，value值为yapi项目token,
                      2时，value是yapi下载的json文件名，文件放在file目录下,
                      3时，value是yapi的yapi-swagger.json
            name:项目名称，空时默认当前py文件所在文件名上级目录
         """
         super().__init__(api_type, value, name, yapi_url, app_key)
-        self.get_project()
-        self.run()
 
     def get_project(self):
         if self.app_key:
             project = requests.post(self.url + '/variable/variable/',
                                     json={"app_key": self.app_key, "environment": "sit"}).json()
             if project.get('project'):
-                self.name = project.get('project')[0].get('code')
+                self.name = self.name or project.get('project')[0].get('code')
                 if project.get('api_settings'):
                     self.api_type = project.get('api_settings')[0].get('api_type')
                     if self.api_type == 2:
                         self.yapi_file_str = requests.get(self.url + "/media/" +
                                                           project.get('api_settings')[0].get('file')).text
                     elif self.api_type in (0, 3):
                         self.value = project.get('api_settings')[0].get('url')
                     elif self.api_type == 1:
                         self.yapi_url = project.get('api_settings')[0].get('url').strip()
                         if self.yapi_url[-1] == "/":
                             self.yapi_url = self.yapi_url[:-1]
                         self.value = project.get('api_settings')[0].get('token')
             else:
                 self.error = project.get('non_field_errors')[0]
-        self.name = self.name if self.name else "demo"
+        self.name = self.name or "demo"
         self.name2 = self.name.title()
 
-    def run(self):
+    def create_project(self):
         """
         创建项目
         """
+        self.get_project()
         if self.error:
             print(self.error)
             return False
         # 创建项目目录
         self.set_file_path()
         # 获取已维护api方法接口列表
         self.get_api_fun_list()
```

### Comparing `huhk-1.6.4/huhk/testcase/apache/beam_class.py` & `huhk-1.6.5/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/data.py` & `huhk-1.6.5/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/par_do.py` & `huhk-1.6.5/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.5/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_file.py` & `huhk-1.6.5/huhk/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.5/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.5/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_map.py` & `huhk-1.6.5/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.5/huhk/testcase/apache/test_par_do.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,26 +28,26 @@
             return durations.index(plant['duration']) if plant['duration'] in durations else len(durations)
 
         out = ApacheFun(data_list_dict, data_type=data_type).partition(by_duration, 4)
         # out.print("'{}: {}'.format(x['duration'], x)")
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
-        out.run()
+        out.create_project()
 
     # 使用 lambda 函数进行分区
     def test_par_do_005(self):
         durations = ['annual', 'biennial', 'perennial']
         out = ApacheFun(data_list_dict, data_type=data_type).partition(
             lambda plant, num_partitions:
             durations.index(plant['duration']) if plant['duration'] in durations else len(durations), 4)
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
-        out.run()
+        out.create_project()
 
     # 具有多个参数的分区
     def test_par_do_006(self):
 
         def split_dataset(plant, num_partitions, ratio):
             assert num_partitions == len(ratio)
             bucket = random.randint(0, sum(ratio)-1)
@@ -57,8 +57,8 @@
                 if bucket < total:
                     return i
             return len(ratio) - 1
 
         out = ApacheFun(data_list_dict*3).partition(split_dataset, 2, ratio=[10, 20])
         out.value[0].print("'1: {}'.format(x)")
         out.value[1].print("'2: {}'.format(x)")
-        out.run()
+        out.create_project()
```

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_regex.py` & `huhk-1.6.5/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_time.py` & `huhk-1.6.5/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/testcase/apache/test_to_string.py` & `huhk-1.6.5/huhk/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_apache_beam.py` & `huhk-1.6.5/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_dict.py` & `huhk-1.6.5/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_encryption.py` & `huhk-1.6.5/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_fun.py` & `huhk-1.6.5/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,15 @@
                 _data = _header.copy()
                 _data.update(v)
                 data[i] = _data
         if isdigitl:
             for i, d in enumerate(data):
                 for k, v in d.items():
                     try:
-                        if v.isdigit():
+                        if v.isdigit() and len(str(v)) < 10:
                             data[i][k] = int(v)
                     except:
                         pass
         result = DataFrame(data)
         result.to_excel(f, sheet_name=sheet_name, index=False, engine="openpyxl")
 
         try:
```

### Comparing `huhk-1.6.4/huhk/unit_logger.py` & `huhk-1.6.5/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_request.py` & `huhk-1.6.5/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/unit_tasks.py` & `huhk-1.6.5/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk/常用命令.py` & `huhk-1.6.5/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.4/huhk.egg-info/SOURCES.txt` & `huhk-1.6.5/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

