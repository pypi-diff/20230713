# Comparing `tmp/PlistParser-2023.7.16.tar.gz` & `tmp/PlistParser-2023.7.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlistParser-2023.7.16.tar", last modified: Thu Jul 13 14:45:45 2023, max compression
+gzip compressed data, was "PlistParser-2023.7.17.tar", last modified: Thu Jul 13 14:51:38 2023, max compression
```

## Comparing `PlistParser-2023.7.16.tar` & `PlistParser-2023.7.17.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/
--rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.16/LICENSE.txt
--rw-rw-rw-   0        0        0    15431 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.225238 PlistParser-2023.7.16/PlistParser/
--rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.16/PlistParser/Base64.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.234130 PlistParser-2023.7.16/PlistParser/DisplaceTemplate/
--rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.16/PlistParser/DisplaceTemplate/__init__.py
--rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.16/PlistParser/Extend.py
--rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.16/PlistParser/Info.py
--rw-rw-rw-   0        0        0     6001 2023-07-13 14:41:47.000000 PlistParser-2023.7.16/PlistParser/Plist.py
--rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.16/PlistParser/PlistParser.py
--rw-rw-rw-   0        0        0      174 2023-07-13 14:45:31.000000 PlistParser-2023.7.16/PlistParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:45:45.234130 PlistParser-2023.7.16/PlistParser.egg-info/
--rw-rw-rw-   0        0        0    15431 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-13 14:45:45.000000 PlistParser-2023.7.16/PlistParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14729 2023-07-13 13:29:30.000000 PlistParser-2023.7.16/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 14:45:45.235370 PlistParser-2023.7.16/setup.cfg
--rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/
+-rw-rw-rw-   0        0        0     1072 2023-07-11 01:29:42.000000 PlistParser-2023.7.17/LICENSE.txt
+-rw-rw-rw-   0        0        0    15688 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.282791 PlistParser-2023.7.17/PlistParser/
+-rw-rw-rw-   0        0        0      395 2023-07-11 02:07:16.000000 PlistParser-2023.7.17/PlistParser/Base64.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.292871 PlistParser-2023.7.17/PlistParser/DisplaceTemplate/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:01:26.000000 PlistParser-2023.7.17/PlistParser/DisplaceTemplate/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-07-11 15:47:49.000000 PlistParser-2023.7.17/PlistParser/Extend.py
+-rw-rw-rw-   0        0        0     4330 2023-07-12 18:22:18.000000 PlistParser-2023.7.17/PlistParser/Info.py
+-rw-rw-rw-   0        0        0     6001 2023-07-13 14:41:47.000000 PlistParser-2023.7.17/PlistParser/Plist.py
+-rw-rw-rw-   0        0        0    11195 2023-07-13 11:23:15.000000 PlistParser-2023.7.17/PlistParser/PlistParser.py
+-rw-rw-rw-   0        0        0      174 2023-07-13 14:46:51.000000 PlistParser-2023.7.17/PlistParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 14:51:38.292871 PlistParser-2023.7.17/PlistParser.egg-info/
+-rw-rw-rw-   0        0        0    15688 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 14:51:38.000000 PlistParser-2023.7.17/PlistParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14986 2023-07-13 14:51:28.000000 PlistParser-2023.7.17/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 14:51:38.293854 PlistParser-2023.7.17/setup.cfg
+-rw-rw-rw-   0        0        0     1945 2023-07-12 18:24:49.000000 PlistParser-2023.7.17/setup.py
```

### Comparing `PlistParser-2023.7.16/LICENSE.txt` & `PlistParser-2023.7.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.16/PKG-INFO` & `PlistParser-2023.7.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.16
+Version: 2023.7.17
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -20,18 +20,21 @@
 License-File: LICENSE.txt
 
 
 
 ![PlistParse Log](./logo.png)
 
 # PlistParser
+
+## 建议使用最新版
+
 ### `🏷️建议在 查看此文档`
 #### `本扩展库(包)` 还有`待完善` 如有问题 请在 `序言`-`讨论` 找到推荐的 相关问题 `讨论` 位置
 #### `谢谢`
-
+### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=hxazC_VtukLg0VcGfykpJsleBSzj-WE7&jump_from=webapi&authKey=WK2HPKG7f/2sqLYTwPo5NkicoJSrke4TNglt/dV8QAHyKvGS/XYiJFteSxSs4IpH"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
       * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
@@ -61,16 +64,16 @@
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于API
     * 相关库导入
       ```python
-        from PlistParser import PlistParser  # .plist 解析器
-        from PlistParser import Plist  # .plist 解析辅助定位器
+        from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
+        from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
         from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
         from PlistParser import Extend  # .plist 解析器 扩展函数库
         from PlistParser import Info  # .plist 解析器 相关信息
         from PlistParser import DisplaceTemplate  # .plist 解析器置换模板文件包
       ```
     * 相关库的API(接口)
```

### Comparing `PlistParser-2023.7.16/PlistParser/Info.py` & `PlistParser-2023.7.17/PlistParser/Info.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.16/PlistParser/Plist.py` & `PlistParser-2023.7.17/PlistParser/Plist.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.16/PlistParser/PlistParser.py` & `PlistParser-2023.7.17/PlistParser/PlistParser.py`

 * *Files identical despite different names*

### Comparing `PlistParser-2023.7.16/PlistParser.egg-info/PKG-INFO` & `PlistParser-2023.7.17/PlistParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlistParser
-Version: 2023.7.16
+Version: 2023.7.17
 Summary: Extension package for .plist file parsing
 Home-page: https://github.com/whiteEelsYikes/PlistParser
 Author: white-EelsYikes
 Author-email: 2172989337@qq.com
 Keywords: Plist,PlistParser
 Platform: Windows
 Platform: Linux
@@ -20,18 +20,21 @@
 License-File: LICENSE.txt
 
 
 
 ![PlistParse Log](./logo.png)
 
 # PlistParser
+
+## 建议使用最新版
+
 ### `🏷️建议在 查看此文档`
 #### `本扩展库(包)` 还有`待完善` 如有问题 请在 `序言`-`讨论` 找到推荐的 相关问题 `讨论` 位置
 #### `谢谢`
-
+### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=hxazC_VtukLg0VcGfykpJsleBSzj-WE7&jump_from=webapi&authKey=WK2HPKG7f/2sqLYTwPo5NkicoJSrke4TNglt/dV8QAHyKvGS/XYiJFteSxSs4IpH"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
       * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
@@ -61,16 +64,16 @@
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于API
     * 相关库导入
       ```python
-        from PlistParser import PlistParser  # .plist 解析器
-        from PlistParser import Plist  # .plist 解析辅助定位器
+        from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
+        from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
         from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
         from PlistParser import Extend  # .plist 解析器 扩展函数库
         from PlistParser import Info  # .plist 解析器 相关信息
         from PlistParser import DisplaceTemplate  # .plist 解析器置换模板文件包
       ```
     * 相关库的API(接口)
```

### Comparing `PlistParser-2023.7.16/README.md` & `PlistParser-2023.7.17/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 
 
 ![PlistParse Log](./logo.png)
 
 # PlistParser
+
+## 建议使用最新版
+
 ### `🏷️建议在 查看此文档`
 #### `本扩展库(包)` 还有`待完善` 如有问题 请在 `序言`-`讨论` 找到推荐的 相关问题 `讨论` 位置
 #### `谢谢`
-
+### 本库 作者实在肝不动 文档这些就随便写写了 大家把 扩展库 安装好后 主要看源代码文件就行了 见谅
 -------------------
 * 🎫 序言
   * ### `📿讨论`
     * ### [`GitHub`](https://github.com/whiteEelsYikes/PlistParser)
     * <a target="_blank" href="https://qm.qq.com/cgi-bin/qm/qr?k=hxazC_VtukLg0VcGfykpJsleBSzj-WE7&jump_from=webapi&authKey=WK2HPKG7f/2sqLYTwPo5NkicoJSrke4TNglt/dV8QAHyKvGS/XYiJFteSxSs4IpH"><img border="0" src="//pub.idqqimg.com/wpa/images/group.png" alt="PlistParser" title="PlistParser"></a>
   * ## `贡献名单`
       * `white-EelsYikes`: 邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=L1hHRltKAkpKQ1xWRkRKXG9eXgFMQEI" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a> |邮箱2:<a target="_blank" href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=TjkmJzorYysrIg4-P2AtISM" style="text-decoration:none;"><img src="http://rescdn.qqmail.com/zh_CN/htmledition/images/function/qm_open/ico_mailme_21.png"/></a>
@@ -40,16 +43,16 @@
   * 🔖 本扩展库为 扩展类型库 所以可能存在很多功能和扩展性 这里 作者提示 
   * 文档教程
     * 在[`PyPi`](https://pypi.org/project/PlistParser/)下载项目压缩包 其中可以找到`PlistParser.doc-info`与`PlistParser.test-s`他们分别保存了项目构建时保留的教程文档以及测试调试文件 可以参考 这里提供下载
     * 🔖 如果您的电脑没有解压软件 我们也推荐了解压程序[`360zip`](http://360yasuo.cn/) 您也可以在[`PyPi`](https://pypi.org/project/PlistParser/)找到该程序 我们也提供下载
   * 🧑‍💻 关于API
     * 相关库导入
       ```python
-        from PlistParser import PlistParser  # .plist 解析器
-        from PlistParser import Plist  # .plist 解析辅助定位器
+        from PlistParser import PlistParser  # .plist 解析器 引擎 提供 主要算法和解析转译支持
+        from PlistParser import Plist  # .plist 解析辅助定位器 同时支持 py基本的plist文件定义
         from PlistParser import Base64  # .plist 解析器 base64 加解密 辅助库
       
         from PlistParser import Extend  # .plist 解析器 扩展函数库
         from PlistParser import Info  # .plist 解析器 相关信息
         from PlistParser import DisplaceTemplate  # .plist 解析器置换模板文件包
       ```
     * 相关库的API(接口)
```

### Comparing `PlistParser-2023.7.16/setup.py` & `PlistParser-2023.7.17/setup.py`

 * *Files identical despite different names*

