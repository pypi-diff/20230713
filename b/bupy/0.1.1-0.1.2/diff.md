# Comparing `tmp/bupy-0.1.1.tar.gz` & `tmp/bupy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bupy-0.1.1.tar", max compression
+gzip compressed data, was "bupy-0.1.2.tar", max compression
```

## Comparing `bupy-0.1.1.tar` & `bupy-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0    11309 2022-08-15 19:19:34.766017 bupy-0.1.1/LICENSE
--rw-r--r--   0        0        0     4407 2022-08-16 02:26:23.902984 bupy-0.1.1/README.md
--rw-r--r--   0        0        0       44 2022-08-16 02:26:23.902984 bupy-0.1.1/bupy/__init__.py
--rw-r--r--   0        0        0      125 2022-07-20 04:51:21.622443 bupy-0.1.1/bupy/__main__.py
--rw-r--r--   0        0        0     1212 2022-08-05 06:28:40.196842 bupy-0.1.1/bupy/butane.py
--rw-r--r--   0        0        0     7976 2022-08-15 21:22:34.016530 bupy-0.1.1/bupy/cli.py
--rw-r--r--   0        0        0      763 2022-07-14 00:56:09.163006 bupy-0.1.1/bupy/config.py
--rw-r--r--   0        0        0     5021 2022-08-15 19:19:34.766017 bupy-0.1.1/bupy/fcos.py
--rw-r--r--   0        0        0     1750 2022-08-15 19:19:34.767017 bupy-0.1.1/bupy/qemu.py
--rw-r--r--   0        0        0     5337 2022-08-15 04:09:14.190479 bupy-0.1.1/bupy/template.py
--rw-r--r--   0        0        0     1100 2022-08-15 19:19:34.767017 bupy-0.1.1/bupy/util.py
--rw-r--r--   0        0        0      736 2022-08-16 02:26:23.902984 bupy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5337 2022-08-16 02:26:40.209312 bupy-0.1.1/setup.py
--rw-r--r--   0        0        0     5023 2022-08-16 02:26:40.209771 bupy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-07-13 15:52:05.423952 bupy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5332 2023-07-13 15:52:05.423952 bupy-0.1.2/README.md
+-rw-r--r--   0        0        0       44 2023-07-13 15:52:48.730657 bupy-0.1.2/bupy/__init__.py
+-rw-r--r--   0        0        0      125 2022-07-20 04:51:21.622443 bupy-0.1.2/bupy/__main__.py
+-rw-r--r--   0        0        0     1212 2022-08-05 06:28:40.196842 bupy-0.1.2/bupy/butane.py
+-rw-r--r--   0        0        0     8288 2023-07-13 15:52:05.423952 bupy-0.1.2/bupy/cli.py
+-rw-r--r--   0        0        0     5021 2022-08-15 19:19:34.766017 bupy-0.1.2/bupy/fcos.py
+-rw-r--r--   0        0        0     3357 2023-07-13 15:52:05.424952 bupy-0.1.2/bupy/qemu.py
+-rw-r--r--   0        0        0     5337 2023-04-05 03:35:15.109520 bupy-0.1.2/bupy/template.py
+-rw-r--r--   0        0        0     1100 2022-08-15 19:19:34.767017 bupy-0.1.2/bupy/util.py
+-rw-r--r--   0        0        0      776 2023-07-13 15:52:41.247535 bupy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 bupy-0.1.2/PKG-INFO
```

### Comparing `bupy-0.1.1/LICENSE` & `bupy-0.1.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Apache License
+                                 Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `bupy-0.1.1/README.md` & `bupy-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,76 +8,67 @@
 
 * [Python 3.8.10^](https://www.python.org/downloads/)
 * [butane](https://coreos.github.io/butane/)
 * [qemu](https://www.qemu.org/download/)
 * If possible, a positive attitude
 
 ### Roadmap
-- [x] Convert Support
-- [x] Jinja2 Template Support
-- [x] Launch a local QEMU FCOS VM
-- [ ] Merge Butane YAML (snippets)
-- [ ] Serve Ignition JSON via HTTP
-- [ ] Libvirt support
+
+* [x] Convert Support
+
+* [x] Jinja2 Template Support
+* [x] Launch a local QEMU FCOS VM
+* [ ] Merge Butane YAML (snippets)
+* [ ] Serve Ignition JSON via HTTP
+* [ ] Libvirt support
 
 ### Demo
 
 You can watch a quick demo of Bupy on Youtube.
 
 [![Quick demo of Bupy for Fedora CoreOS](https://img.youtube.com/vi/yBOEz827TUU/0.jpg)](https://www.youtube.com/watch?v=yBOEz827TUU)
 
 ### Development
 
 1) Clone this repo
-1) Install dependencies
-  ```
-  poetry install
-  ```
-1) Activate a poetry shell
-  ```
-  $ poetry shell
-  Spawning shell within /home/jdoss/src/quickvm/bupy/.venv
-  . /home/jdoss/src/quickvm/bupy/.venv/bin/activate
-  $ . /home/jdoss/src/quickvm/bupy/.venv/bin/activate
-  ```
-1) Make changes...
-1) See them in action
-  ```
-  (.venv) $ python -m bupy --help
+2) Install dependencies
+
+```bash
+poetry install
+```
 
-   Usage: bupy [OPTIONS] COMMAND [ARGS]...
+3) Activate a poetry shell
 
-  ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-  │ --version             -v        Show the version and exit.                                       │
-  │ --install-completion            Install completion for the current shell.                        │
-  │ --show-completion               Show completion for the current shell, to copy it or customize   │
-  │                                 the installation.                                                │
-  │ --help                          Show this message and exit.                                      │
-  ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
-  ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-  │ convert      Converts Butane YAML to Ignition JSON                                               │
-  │ merge        Merge Butane files together                                                         │
-  │ qemu         Launches a QEMU VM with the specified Ignition JSON or Butane YAML                  │
-  │ serve        Serve an ignition file via HTTP on a specified port                                 │
-  │ template     Render Butane Jinja2 templates                                                      │
-  ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
+```bash
+poetry shell
+```
+
+4) Make changes...
+5) See them in action
+
+```bash
+bupy --help
+
+ Usage: bupy [OPTIONS] COMMAND [ARGS]...
+
+ Bupy: Butane Python toolkit.
+
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --version             -v        Show the version and exit.                                                                                                                                                 │
+│ --install-completion            Install completion for the current shell.                                                                                                                                  │
+│ --show-completion               Show completion for the current shell, to copy it or customize the installation.                                                                                           │
+│ --help                          Show this message and exit.                                                                                                                                                │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ convert                      Converts Butane YAML to Ignition JSON                                                                                                                                         │
+│ template                     Renders a Jinja2 Template to Butane YAML or Ignition JSON                                                                                                                     │
+│ vm                           Launches a QEMU VM with a Butane YAML or Jinja2 Template                                                                                                                      │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+
+ Made in ✶✶✶✶ Chicago✶✶✶✶  〜 (c) 2023 QuickVM, LLC
   ```
 
 ## License
 
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-                          Copyright 2022 QuickVM, LLC
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+[Apache License Version 2.0](http://www.apache.org/licenses/LICENSE-2.0>)
+
+Copyright 2023 QuickVM, LLC
```

### Comparing `bupy-0.1.1/bupy/butane.py` & `bupy-0.1.2/bupy/butane.py`

 * *Files identical despite different names*

### Comparing `bupy-0.1.1/bupy/cli.py` & `bupy-0.1.2/bupy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import typer
 
 
 app = typer.Typer(
     help="[bold]Bupy:[/bold] [bold]Bu[/bold]tane [bold]Py[/bold]thon toolkit.",
     rich_markup_mode="rich",
     no_args_is_help=True,
-    epilog="Made in [pale_turquoise1]✶✶✶✶[/pale_turquoise1] [red1]Chicago[/red1][pale_turquoise1]✶✶✶✶[/pale_turquoise1]  〜 (c) 2022 QuickVM, LLC",
+    epilog="Made in [pale_turquoise1]✶✶✶✶[/pale_turquoise1] [red1]Chicago[/red1][pale_turquoise1]✶✶✶✶[/pale_turquoise1]  〜 (c) 2023 QuickVM, LLC",
     pretty_exceptions_show_locals=False,
 )
 
 
 @app.callback()
 def main(
     version: Optional[bool] = typer.Option(
@@ -85,15 +85,18 @@
 def vm(
     file: str = typer.Argument(
         ... if sys.stdin.isatty() else sys.stdin.read().strip(),
         help="Reads Butane from a file or stdin and converts it to Ignition JSON.",
         show_default=False,
     ),
     template: str = typer.Option(
-        "", "--template", "-t", help="Read file as a Jinja2 template and load a variables file."
+        "",
+        "--template",
+        "-t",
+        help="Read file as a Jinja2 template and load a variables file.\n(--template bupyvars.yaml template.bu.j2)",
     ),
     write: str = typer.Option("", "--write", "-w", help="Write the Ignition JSON to a file."),
     force: bool = typer.Option(False, "--force", "-f", help="Overwrite an existing Ignition file."),
     stream: str = typer.Option(
         "stable",
         "--stream",
         "-s",
@@ -102,19 +105,19 @@
     arch: str = typer.Option(
         "x86_64",
         "--arch",
         "-a",
         help="Fedora CoreOS arch: aarch64, s390x, x86_64",
     ),
     ram: int = typer.Option(1024, "--ram", "-r", help="RAM amount in MB"),
-    ports: Optional[List[int]] = typer.Option(
+    ports: Optional[List[str]] = typer.Option(
         None,
         "--port",
         "-p",
-        help="Map random host ports to VM ports. Can be used many times.",
+        help="Pass a single port number (8080) to map a random host port to the VM port. Pass 8080:80 to assign a static host port to the VM port. The --port option can be used many times. The port range allowed is 1 - 65535.",
     ),
 ):
     """
     Launches a QEMU VM with a Butane YAML or Jinja2 Template
     """
 
     butane_binary = util.find_binary("butane")
@@ -182,15 +185,15 @@
         show_default=False,
     ),
     variables: str = typer.Argument(
         ...,
         help="Reads a YAML file to use as variables for rendering a Jinja2 template.",
     ),
     show: bool = typer.Option(
-        False, "--show", "-s", help="rPrint the rendered template.", show_default=False
+        False, "--show", "-s", help="Print the rendered template.", show_default=False
     ),
     line_numbers: bool = typer.Option(
         True, "--numbers", "-n", help="Show line numbers in printed template."
     ),
     write: str = typer.Option("", "--write", "-w", help="Write the Ignition JSON to a file."),
     force: bool = typer.Option(False, "--force", "-f", help="Overwrite an existing Ignition file."),
     pretty: bool = typer.Option(
@@ -207,17 +210,20 @@
             "[bold red]Error:[/bold red] The butane binary could not be found! Please [link=https://coreos.github.io/butane/getting-started/]install[/link] it."
         )
         raise typer.Exit(code=1)
 
     with util.SilenceTemplateException():
         if show:
             bu = tpl.rendered_template(template, tpl.read_template_vars(variables)).decode("utf-8")
-            syntax = Syntax(bu, "YAML", line_numbers=line_numbers)
-            console = Console(color_system=None)
-            console.print(syntax)
+            if sys.stdout.isatty():
+                syntax = Syntax(bu, "YAML", line_numbers=line_numbers)
+                console = Console(color_system=None)
+                console.print(syntax)
+            else:
+                print(bu)
             raise typer.Exit()
 
         # TODO: Add support for finding bupyvars.yaml file in CWD, or in the directory the template resides in.
         # cwd = Path.cwd()
         template_output = tpl.rendered_template(template, tpl.read_template_vars(variables))
         ignition_json = butane.butane_to_ignition(template_output)
```

### Comparing `bupy-0.1.1/bupy/fcos.py` & `bupy-0.1.2/bupy/fcos.py`

 * *Files identical despite different names*

### Comparing `bupy-0.1.1/bupy/qemu.py` & `bupy-0.1.2/bupy/qemu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,113 @@
-from rich import print as rprint
-import socket
+import os
+import re
 import shlex
+import socket
 import subprocess
+import typer
+from rich import print as rprint
 from typing import List
 
 
 def find_port() -> int:
     """
-    Find a random open port
+    Find a random open port to use
     """
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.bind(("", 0))
     sock.listen(1)
     port = sock.getsockname()[1]
     sock.close()
     return port
 
 
-def launch(ram: int, qcow: str, ign: str, ports: List[int]) -> int:
+def check_port(port: int) -> bool:
     """
-    Launch FCOS with QEMU
+    Check to see if a port is available to use
     """
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    result = False
+    try:
+        sock.bind(("", port))
+        result = True
+    except:
+        rprint(f"[bold red]Error:[/bold red] Port {port} is already in use!")
+    sock.close()
+    return result
 
-    port_list = set([])
-    port_list.add(22)
-    if ports is not None:
-        port_list.update(ports)
+
+def validate_port_format(port: str) -> bool:
+    """
+    Validate port format. The port has to be between 1 and 65535 as a single number (8080) or a port pair (8080:80)
+    """
+    range_expression = r"(\d{1,4}|[1-5]\d{4}|6[0-4]\d{3}|65[0-4]\d{2}|655[0-2]\d|6553[0-5])"
+    pattern = rf"^{range_expression}$|^{range_expression}:{range_expression}$"
+    match = re.match(pattern, port)
+    if match:
+        return True
+    else:
+        rprint(
+            f"[bold red]Error:[/bold red] The port {port} is not between 1 - 65535 and input as a single number (8080) or a port pair (8080:80)!"
+        )
+        raise typer.Exit(code=1)
+
+
+def launch(ram: int, qcow: str, ign: str, ports: List[str]) -> int:
+    """
+    Launch FCOS with QEMU
+    """
 
     hostfwd_list = []
     port_maps = []
 
-    for port in port_list:
-        host_port = find_port()
+    if not "22" or not any(port.endswith(":22") for port in ports):
+        ports.append("22")
+
+    for port in ports:
+        validate_port_format(port)
+        if ":" not in port:
+            port = int(port)
+        if isinstance(port, int):
+            host_port = find_port()
+            vm_port = port
+        elif isinstance(port, str):
+            numbers = port.split(":")
+            host_port = int(numbers[0])
+            vm_port = int(numbers[1])
+
+        if not check_port(host_port):
+            raise typer.Exit(code=1)
 
-        if port == 22:
+        if vm_port == 22:
             ssh_port = host_port
 
-        paired_ports = f"{host_port}:{port}"
+        paired_ports = f"{host_port}:{vm_port}"
         port_maps.append(paired_ports)
 
-        hostfwd_port = f"hostfwd=tcp::{host_port}-:{port}"
+        hostfwd_port = f"hostfwd=tcp::{host_port}-:{vm_port}"
         hostfwd_list.append(hostfwd_port)
 
     joined_hostfwd = ",".join(hostfwd_list)
 
-    qemu_cmd = f"qemu-system-x86_64 -m {ram} -enable-kvm -cpu host -snapshot -daemonize \
-        -drive if=virtio,file={qcow} -name bupy-vm-{ssh_port} \
+    if not os.environ.get("DISPLAY"):
+        display = "-display none"
+    else:
+        display = ""
+
+    qemu_cmd = f"qemu-system-x86_64 \
+        -m {ram} \
+        -enable-kvm \
+        -cpu host \
+        -snapshot \
+        -daemonize \
+        -drive if=virtio,file={qcow} \
+        -name bupy-vm-{ssh_port} \
         -fw_cfg name=opt/com.coreos/config,file={ign} \
-        -nic user,model=virtio,{joined_hostfwd}"
+        -nic user,model=virtio,{joined_hostfwd} \
+        {display}"
     qemu_cmd_split = shlex.split(qemu_cmd)
 
     rprint("Launching QEMU VM...")
     process = subprocess.Popen(qemu_cmd_split, start_new_session=True)
     qemu_pid = process.pid
 
     rprint(f"The PID is: {qemu_pid}")
```

### Comparing `bupy-0.1.1/bupy/template.py` & `bupy-0.1.2/bupy/template.py`

 * *Files identical despite different names*

### Comparing `bupy-0.1.1/bupy/util.py` & `bupy-0.1.2/bupy/util.py`

 * *Files identical despite different names*

### Comparing `bupy-0.1.1/pyproject.toml` & `bupy-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-[tool.black]
-line-length = 102
-target-version = ['py38',]
-include = '\.py?$'
-exclude = '''
-/(
-    \.git
-  | \.eggs
-  | \.vscode
-  | makefiles
-  | build
-  | dist
-  | venv
-  | pycache
-)/
-'''
-
-
-
 [tool.poetry]
 name = "bupy"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python toolkit for Butane and Ignition"
 authors = ["QuickVM <hello@quickvm.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 bupy = "bupy.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.8.10"
-typer = {extras = ["all"], version = "^0.6.1"}
+typer = {extras = ["all"], version = "^0.9.0"}
 pyxdg = "^0.28"
 urllib3 = "^1.26.10"
 Jinja2 = "^3.1.2"
 "ruamel.yaml" = "^0.17.21"
-rich = "^12.5.1"
+rich = "^13.4.2"
+pip = "^23.0.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 102
+target-version = ['py38',]
+include = '\.py?$'
+exclude = '''
+/(
+    \.git
+  | \.eggs
+  | \.vscode
+  | makefiles
+  | build
+  | dist
+  | venv
+  | pycache
+)/
+'''
```

