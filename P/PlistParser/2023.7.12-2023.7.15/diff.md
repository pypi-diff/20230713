# Comparing `tmp/PlistParser-2023.7.12.tar.gz` & `tmp/PlistParser-2023.7.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.12.tar", last modified: Tue Jul 11 11:23:39 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.15.tar", last modified: Thu Jul 13 13:55:20 2023, max compression
```

## Comparing `PlistParser-2023.7.12.tar` & `PlistParser-2023.7.15.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:23:39.563444 PlistParser-2023.7.12/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.12/LICENSE.txt
--rw-rw-rw-   0        0        0      871 2023-07-11 11:23:39.563444 PlistParser-2023.7.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 11:23:39.553256 PlistParser-2023.7.12/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.12/PlistParser/Base64.py
--rw-rw-rw-   0        0        0     2694 2023-07-11 02:07:16.000000 PlistParser-2023.7.12/PlistParser/Plist.py
--rw-rw-rw-   0        0        0     9074 2023-07-11 02:08:21.000000 PlistParser-2023.7.12/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0     4255 2023-07-11 02:22:15.000000 PlistParser-2023.7.12/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:23:39.562445 PlistParser-2023.7.12/PlistParser.egg-info/
--rw-rw-rw-   0        0        0      871 2023-07-11 11:23:39.000000 PlistParser-2023.7.12/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-11 11:23:39.000000 PlistParser-2023.7.12/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:23:39.000000 PlistParser-2023.7.12/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 11:23:39.000000 PlistParser-2023.7.12/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      153 2023-07-11 01:55:00.000000 PlistParser-2023.7.12/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 11:23:39.563444 PlistParser-2023.7.12/setup.cfg
--rw-rw-rw-   0        0        0     1740 2023-07-11 10:27:17.000000 PlistParser-2023.7.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:23:39.562445 PlistParser-2023.7.12/tests/
--rw-rw-rw-   0        0        0     1879 2023-07-11 03:44:26.000000 PlistParser-2023.7.12/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.15/LICENSE.txt
+-rw-rw-rw-   0        0        0    15431 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.580562 PlistParser-2023.7.15/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.15/PlistParser/Base64.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.603667 PlistParser-2023.7.15/PlistParser/DisplaceTemplate/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.15/PlistParser/DisplaceTemplate/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.15/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.15/PlistParser/Info.py
+-rw-rw-rw-   0        0        0     5984 2023-07-13 11:36:05.000000 PlistParser-2023.7.15/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.15/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      174 2023-07-13 13:39:15.000000 PlistParser-2023.7.15/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:55:20.602670 PlistParser-2023.7.15/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0    15431 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 13:55:20.000000 PlistParser-2023.7.15/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14729 2023-07-13 13:29:30.000000 PlistParser-2023.7.15/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:55:20.604655 PlistParser-2023.7.15/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.15/setup.py
```

### Comparing `PlistParser-2023.7.12/LICENSE.txt` & `PlistParser-2023.7.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.12/PlistParser/PlistParser.py` & `PlistParser-2023.7.15/PlistParser/PlistParser.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,35 +3,43 @@
 
 import os.path
 import plistlib
 
 
 class PlistParser:
 
-    def __init__(self, parser_plist: str | None = None, auto_parser: bool = True, cust_dict: dict = None):
+    def __init__(self, parser_plist: str | dict | None = None, auto_parser: bool = True, cust_dict: dict = None):
         """
 
         :param parser_plist: 给定解析的 .plist 文件 或者 二进制 或者 文本 数据
         :param auto_parser: 是否在 plist_txt 不为空时 自动在初始化时解析 plist_txt (在 plist_txt 为空时 该参数不会有任何效果)
         :param cust_dict: 全称 customization_dict 给定自定义的 plist 字典数据
         """
+        if type(parser_plist) == dict:
+            self.__dict__ = parser_plist
+            return
         self.plist_data = parser_plist
         self.plist_dict = self.parser_dict(parser_plist) if auto_parser and parser_plist != None else None
         self.cust_dict = cust_dict
 
-    def parser_base64(self, bytes_data: bytes, mode_dict: dict) -> bytes:  # base 16 32 64 加解密支持
+    def parser_base64(self, bytes_data: bytes | str, mode_dict: dict) -> bytes | str:  # base 16 32 64 加解密支持
         """
         提供强大的 base64 基础加解密支持 可支持嵌套加解密
         :param bytes_data: 被这些操作的(加解密)数据
         :param mode_dict: 加解密操作及其参数声明字典
         :return: 执行 mode_dict 指定操作后的 加解密 数据
+                    (一开始传入的bytes_data是什么类型就返回什么类型)
         """
+        bytes_data_str_state = False
+        if type(bytes_data) == str:
+            bytes_data.encode()
+            bytes_data_str_state = True
         for base, kwargs in mode_dict.items():
             bytes_data = base(bytes_data, **kwargs)
-        return bytes_data
+        return bytes_data.decode() if bytes_data_str_state else bytes_data
 
     def parser_plist(self, parser_dict: dict | None = None, out_file: str | None = None, **kwargs) -> bytes:
         """
         将 dict 解析为 .plist
         :param parser_dict: 被解析的 dict 默认为解析 self.plist_dict
         :param out_file: 输出解析数据到指定文件 默认不输出 文件
         :param kwargs: plistlib.dumps 扩展参数
@@ -72,14 +80,16 @@
         """
         提供 基础 自定义 parser_dict 值功能
         :param value_path: 一个元组 元组中的数据从左到右顺序 表达 需要修改 或者查询数据位置
         :param cust_value: 自定义(修改)的数据 默认则不修改 仅查询
         :return: value_path 指定位置的数据 或者修改后数据
         """
         plist_dict_value = self.plist_dict
+        if plist_dict_value == None:
+            raise KeyError('parser_plist 数据为空 或者不符合执行要求 不能执行此操作')
         value_path_len = len(value_path)
         value_path_last = value_path_len - 1
         for index in range(value_path_len):
             value_path_index = value_path[index]
             if index == value_path_last and cust_value:
                 plist_dict_value[value_path_index] = cust_value
             plist_dict_value = plist_dict_value[value_path_index]
@@ -98,20 +108,20 @@
         inquire_dict = {}
         if cust_dict == None:
             raise KeyError('cust_dict 数据为空 或者不符合执行要求 不能执行此操作')
         for plist_dict_index, cust_value in cust_dict.items():
             if type(cust_value) == dict:
                 inquire_dict_item = self.customization_parser_dict_values(cust_value, plist_dict[plist_dict_index])
                 if inquire_dict_item:
-                    inquire_dict.update({plist_dict_index: inquire_dict_item})
+                    inquire_dict[plist_dict_index] = inquire_dict_item
                 continue
             elif cust_value == None:
-                inquire_dict.update({plist_dict_index: plist_dict[plist_dict_index]})
+                inquire_dict[plist_dict_index] = plist_dict[plist_dict_index]
             else:
-                plist_dict.update({plist_dict_index: cust_value})
+                plist_dict[plist_dict_index] = cust_value
         return inquire_dict
 
     def plist_dict_to_cust_dict(self, plist_dict: dict) -> dict:
         """
         将 Plist dict 数据 转换 标准 cust dict
         :param plist_dict: 需要 转换的 plist dict 数据
         :return: 完成 转换的 cust dict 数据
@@ -120,60 +130,92 @@
         for plist_key, cust_value in plist_dict.items():
             cust_dict_index = cust_dict
             plist_key_len = len(plist_key)
             plist_key_last = plist_key_len - 1
             for index in range(plist_key_len):
                 plist_key_index = plist_key[index]
                 if index == plist_key_last:
-                    cust_dict_index.update({plist_key_index: cust_value})
+                    cust_dict_index[plist_key_index] = cust_value
                     break
                 if cust_dict_index.get(plist_key_index) == None:
                     cust_dict_index[plist_key_index] = {}
                 cust_dict_index = cust_dict[plist_key_index]
         self.cust_dict = cust_dict
         return cust_dict
 
+
+class FastPlistParser(PlistParser):
+
+    def __init__(self, parser_plist: str | dict | PlistParser | None = None, auto_parser: bool = True,
+                 cust_dict: dict = None,
+                 *args, **kwargs):
+        """
+
+        :param parser_plist: 给定解析的 .plist 文件 或者 二进制 或者 文本 数据
+        :param auto_parser: 是否在 plist_txt 不为空时 自动在初始化时解析 plist_txt (在 plist_txt 为空时 该参数不会有任何效果)
+        :param cust_dict: 全称 customization_dict 给定自定义的 plist 字典数据
+        """
+        if type(parser_plist) == PlistParser:
+            super().__init__()
+            self.__dict__ = parser_plist.__dict__
+        else:
+            # super().__init__(parser_plist, auto_parser, cust_dict, *args, **kwargs)
+            super().__init__(parser_plist, auto_parser, cust_dict)
+
     def device_model(self, set_value: str | bytes | list | dict | None = None) -> str | bytes | list | dict | None:
         """
         一键 查询/设置 设备型号
         :param set_value: 自定义(修改)的数据 默认则不修改 仅查询
         :return: 设备数据 或者修改后数据
         """
-        plist_dict = self.plist_dict["CacheExtra"]
+        plist_dict = self.plist_dict
+        if plist_dict == None:
+            raise KeyError('self.plist_dict 数据为空 或者不符合执行要求 不能执行此操作')
+        plist_dict = plist_dict["CacheExtra"]
         if set_value:
             plist_dict["Z/dqyWS6OZTRy10UcmUAhw"] = set_value
         return plist_dict["Z/dqyWS6OZTRy10UcmUAhw"]
 
     def device_category(self, set_value: str | bytes | list | dict | None = None) -> str | bytes | list | dict | None:
         """
         一键 查询/设置 设备类别
         :param set_value: 自定义(修改)的数据 默认则不修改 仅查询
         :return: 设备数据 或者修改后数据
         """
-        plist_dict = self.plist_dict["CacheExtra"]
+        plist_dict = self.plist_dict
+        if plist_dict == None:
+            raise KeyError('self.plist_dict 数据为空 或者不符合执行要求 不能执行此操作')
+        plist_dict = plist_dict["CacheExtra"]
         if set_value:
             plist_dict["VuGdqp8UBpi9vPWHlPluVQ"] = set_value
         return plist_dict["VuGdqp8UBpi9vPWHlPluVQ"]
 
     def device_issuance(self, set_value: str | bytes | list | dict | None = None) -> str | bytes | list | dict | None:
         """
         一键 查询/设置 设备发行
         :param set_value: 自定义(修改)的数据 默认则不修改 仅查询
         :return: 设备数据 或者修改后数据
         """
-        plist_dict = self.plist_dict["CacheExtra"]
+        plist_dict = self.plist_dict
+        if plist_dict == None:
+            raise KeyError('self.plist_dict 数据为空 或者不符合执行要求 不能执行此操作')
+        plist_dict = plist_dict["CacheExtra"]
         if set_value:
             plist_dict["zHeENZu+wbg7PUprwNwBWg"] = set_value
         return plist_dict["zHeENZu+wbg7PUprwNwBWg"]
 
     def device_system(self, set_value: str | bytes | list | dict | None = None) -> str | bytes | list | dict | None:
         """
         一键 查询/设置 设备系统
         :param set_value: 自定义(修改)的数据 默认则不修改 仅查询
         :return: 设备数据 或者修改后数据
         """
-        plist_dict = self.plist_dict["CacheExtra"]
+        plist_dict = self.plist_dict
+        if plist_dict == None:
+            raise KeyError('self.plist_dict 数据为空 或者不符合执行要求 不能执行此操作')
+        plist_dict = plist_dict["CacheExtra"]
         if set_value:
             plist_dict["ivIu8YTDnBSrYv/SN4G8Ag"] = set_value
         return plist_dict["ivIu8YTDnBSrYv/SN4G8Ag"]
 
 
+
```

### Comparing `PlistParser-2023.7.12/PlistParser/__init__.py` & `PlistParser-2023.7.15/PlistParser/Info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-__License_body__ = \
+
+__license_body__ = \
     """
     + --------------------------------------------------------------------------------- +
     *   MIT License                                                                     *
     *                                                                                   *
     *   Copyright (c) 2023 white-EelsYikes                                              *
     *                                                                                   *
     *   Permission is hereby granted, free of charge, to any person obtaining a copy    *
@@ -24,32 +25,33 @@
     *   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER          *
     *   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,   *
     *   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE   *
     *   SOFTWARE.                                                                       *
     * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
 
 """
-__License_Head__ = \
+__license_head__ = \
     """
     \033[5;40;32m+-----------------------------------------------------------------------------------+
     \033[5;40;32m+\033[5;40;31m  ███╗   ███╗██╗████████╗    ██╗     ██╗ ██████╗███████╗███╗   ██╗███████╗███████╗ \033[5;40;32m+
     \033[5;40;32m+\033[5;40;31m  ████╗ ████║██║╚══██╔══╝    ██║     ██║██╔════╝██╔════╝████╗  ██║██╔════╝██╔════╝ \033[5;40;32m+
     \033[5;40;32m+\033[5;40;31m  ██╔████╔██║██║   ██║       ██║     ██║██║     █████╗  ██╔██╗ ██║███████╗█████╗   \033[5;40;32m+
     \033[5;40;32m+\033[5;40;31m  ██║╚██╔╝██║██║   ██║       ██║     ██║██║     ██╔══╝  ██║╚██╗██║╚════██║██╔══╝   \033[5;40;32m+
     \033[5;40;32m+\033[5;40;31m  ██║ ╚═╝ ██║██║   ██║       ███████╗██║╚██████╗███████╗██║ ╚████║███████║███████╗ \033[5;40;32m+
     \033[5;40;32m+\033[5;40;31m  ╚═╝     ╚═╝╚═╝   ╚═╝       ╚══════╝╚═╝ ╚═════╝╚══════╝╚═╝  ╚═══╝╚══════╝╚══════╝ \033[5;40;32m+\
     """
 
 
-
-__License__ = f'\033[5;40;32m{__License_Head__}\033[5;40;32m{__License_body__}\033[0m'
-__Version__ = '2023.7.11'
-__SimpleDescription__ = 'Extension package for .plist file parsing'
-__BuildPeople__ = r'white-EelsYikes'
-__Contact__ = r'2172989337@qq.com'
-__ProjectLink__ = r'https://github.com/whiteEelsYikes/PlistParser'
-__BuildPeoples__ = {
-    r'white-EelsYikes':'2172989337@qq.com',
+__build_peoples__ = {
+    r'white-EelsYikes': '2172989337@qq.com',
 }
 
+def open_project_link(project_link=r'https://github.com/whiteEelsYikes/PlistParser'):
+    """
+    使用电脑默认链接打开程序 打开指定的项目链接
+    :param project_link:
+    :return:
+    """
+    import webbrowser  # 这里 py 是有优化的 已经存在的库 再次执行导入是无效的 除非使用异步导入 重载已导入的库
+    webbrowser.open(project_link)
```

### Comparing `PlistParser-2023.7.12/setup.py` & `PlistParser-2023.7.15/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 import setuptools  # 导入setuptools打包工具
+from Cython.Build import cythonize
 import PlistParser
 
 
-with open('requires.txt', 'r', encoding='utf-8') as requires:
-    requires = requires.read().split('\n')
+# with open('requires.txt', 'w', encoding='utf-8') as requires:
+#     requires_txt = [item+'\n' for item in PlistParser.__requires_all__]
+#     requires.write(''.join(requires_txt))
+
 with open('README.md', 'r', encoding='utf-8') as README_md:
     long_description = README_md.read()
 
-
 setuptools.setup(
-    license='MIT',
     name='PlistParser',  # 项目名称
-    version='2023.7.12',  # test 使用
-    # version=PlistParser.__Version__,  # 包版本号，便于维护版本
-    url=PlistParser.__ProjectLink__,  # 自己项目地址，比如github的项目地址
-    author=PlistParser.__BuildPeople__,  # 作者，可以写自己的姓名
-    author_email=PlistParser.__Contact__,  # 作者联系方式，可写自己的邮箱地址
-    description=PlistParser.__SimpleDescription__,  # 包的简述
+    version=PlistParser.__version__,  # 包版本号，便于维护版本
+    url=r'https://github.com/whiteEelsYikes/PlistParser',  # 自己项目地址，比如github的项目地址
+    author=r'white-EelsYikes',  # 作者，可以写自己的姓名
+    author_email=r'2172989337@qq.com',  # 作者联系方式，可写自己的邮箱地址
+    description='Extension package for .plist file parsing',  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 4 - Beta',  # 3 - Alpha | 4 - Beta | 5 - Production/Stable
         'Intended Audience :: Developers',  # 开发的目标用户
         'Topic :: Software Development :: Build Tools',  # 属于什么类型
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     keywords=['Plist', 'PlistParser'],
     platforms=['Windows', 'Linux', 'MacOS'],
-    python_requires='>=3.9',  # 对python的最低版本要求
-    install_requires=requires,  # 表明当前模块依赖哪些包，若环境中没有，则会从pypi中下载安装
+    python_requires='>=3.6',  # 对python的最低版本要求
+    install_requires=[
+        # 'os',
+        # 'Base64',
+        # 'plistlib',
+    ],  # 表明当前模块依赖哪些包，若环境中没有，则会从pypi中下载安装
     packages=setuptools.find_packages(),
+    # ext_modules = cythonize(module_list=["test.py"], language_level=3)
 
 )
```

