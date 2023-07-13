# Comparing `tmp/sshg-0.1.4.tar.gz` & `tmp/sshg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshg-0.1.4.tar", max compression
+gzip compressed data, was "sshg-0.1.5.tar", max compression
```

## Comparing `sshg-0.1.4.tar` & `sshg-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-05-04 07:53:20.678888 sshg-0.1.4/LICENSE
--rw-r--r--   0        0        0     2318 2023-05-04 07:53:20.678888 sshg-0.1.4/README.md
--rw-r--r--   0        0        0      629 2023-05-04 07:53:40.471302 sshg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    11223 2023-05-04 07:53:40.471302 sshg-0.1.4/sshg.py
--rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 sshg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-13 03:17:07.672388 sshg-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2366 2023-07-13 03:17:07.672388 sshg-0.1.5/README.md
+-rw-r--r--   0        0        0      677 2023-07-13 03:17:27.616754 sshg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    11332 2023-07-13 03:17:27.616754 sshg-0.1.5/sshg.py
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 sshg-0.1.5/PKG-INFO
```

### Comparing `sshg-0.1.4/LICENSE` & `sshg-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sshg-0.1.4/README.md` & `sshg-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -65,19 +65,22 @@
 
 ```bash
 # 没安装就装一下，项目依赖poetry发布
 # pip install poetry
 
 poetry self add "poetry-dynamic-versioning[plugin]"
 poetry publish --build
+
+# 进入到项目的虚拟环境
+poetry shell
 ```
 
 
 # Refs
 - https://poetry.eustace.io/docs/
 - https://pypi.org/project/poetry-dynamic-versioning/
 - https://github.com/yinheli/sshw UI风格基本都是参考这个项目
 - https://github.com/WqyJh/sshx 本来用这个名字的，发现跟它重复了
 - https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ 如何使用Github Actions发布
 
 # LICENSE
-[MIT](LICENSE)
+[MIT](LICENSE)
```

### Comparing `sshg-0.1.4/pyproject.toml` & `sshg-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "sshg"
-version = "0.1.4"
+version = "0.1.5"
 description = "ssh from config with arrow select support"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-
+homepage = "https://github.com/codeskyblue/sshg"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Jinja2 = "^3.1.2"
```

### Comparing `sshg-0.1.4/sshg.py` & `sshg-0.1.5/sshg.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.keys import Keys
 from prompt_toolkit.layout.containers import HSplit, Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.styles import Style
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 def make_field(field_name: str = None,
                mm_field=None,
                decorder: typing.Callable = None,
                default=dataclasses.MISSING,
                default_factory=dataclasses.MISSING, **kwargs) -> dataclasses.field:
     return dataclasses.field(metadata=dconfig(field_name=field_name,
@@ -230,18 +230,21 @@
         self._active_index = 0
         super().__init__(self._gen_host_windows())
 
     def _gen_host_windows(self):
         host_windows = []
         for index, config in enumerate(self._host_configs):
             prefix = "" if config.children else f" <gray>{config.user}@{config.host}</gray>"
+            name = config.name
+            if config.children:
+                name = f"+ {name}({len(config.children)})"
             if self._active_index == index:
-                html_text = "  ➤ " + f"<name>{config.name}</name>" + prefix
+                html_text = "  ➤ " + f"<name>{name}</name>" + prefix
             else:
-                html_text = "    " + f"<gray>{config.name}</gray>" + prefix
+                html_text = "    " + f"<gray>{name}</gray>" + prefix
             if config.children:
                 html_text = f"<b>{html_text}</b>"
             host_windows.append(Window(content=FormattedTextControl(HTML(html_text)), height=1))
         return host_windows
 
     def _up_hook(self, event: KeyPressEvent):
         index = self.get_active_index()
@@ -320,8 +323,8 @@
     app = Application(layout=layout, style=style, key_bindings=kb, full_screen=True)
     host_config: HostConfig = app.run()
     if host_config:
         host_config.spawn_ssh()
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `sshg-0.1.4/PKG-INFO` & `sshg-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sshg
-Version: 0.1.4
+Version: 0.1.5
 Summary: ssh from config with arrow select support
+Home-page: https://github.com/codeskyblue/sshg
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -87,19 +88,23 @@
 
 ```bash
 # 没安装就装一下，项目依赖poetry发布
 # pip install poetry
 
 poetry self add "poetry-dynamic-versioning[plugin]"
 poetry publish --build
+
+# 进入到项目的虚拟环境
+poetry shell
 ```
 
 
 # Refs
 - https://poetry.eustace.io/docs/
 - https://pypi.org/project/poetry-dynamic-versioning/
 - https://github.com/yinheli/sshw UI风格基本都是参考这个项目
 - https://github.com/WqyJh/sshx 本来用这个名字的，发现跟它重复了
 - https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/ 如何使用Github Actions发布
 
 # LICENSE
 [MIT](LICENSE)
+
```

