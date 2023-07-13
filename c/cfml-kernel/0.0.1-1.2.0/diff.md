# Comparing `tmp/cfml_kernel-0.0.1.tar.gz` & `tmp/cfml_kernel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfml_kernel-0.0.1.tar", last modified: Tue Jul 11 19:19:15 2023, max compression
+gzip compressed data, was "cfml_kernel-1.2.0.tar", last modified: Thu Jul 13 19:24:13 2023, max compression
```

## Comparing `cfml_kernel-0.0.1.tar` & `cfml_kernel-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:15.105395 cfml_kernel-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-01-26 02:54:33.000000 cfml_kernel-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3620 2023-07-11 19:19:15.104394 cfml_kernel-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3193 2023-04-10 02:08:23.000000 cfml_kernel-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:15.084828 cfml_kernel-0.0.1/cfml_kernel/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/__init__.py
--rw-rw-rw-   0        0        0     5545 2023-05-03 21:33:44.000000 cfml_kernel-0.0.1/cfml_kernel/box_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:15.096819 cfml_kernel-0.0.1/cfml_kernel/cfml/
--rw-rw-rw-   0        0        0       34 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfml/__init__.py
--rw-rw-rw-   0        0        0      127 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfml/__main__.py
--rw-rw-rw-   0        0        0     2025 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfml/install.py
--rw-rw-rw-   0        0        0     1489 2023-05-03 20:57:27.000000 cfml_kernel-0.0.1/cfml_kernel/cfml/kernel.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:15.102383 cfml_kernel-0.0.1/cfml_kernel/cfscript/
--rw-rw-rw-   0        0        0       38 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfscript/__init__.py
--rw-rw-rw-   0        0        0      135 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfscript/__main__.py
--rw-rw-rw-   0        0        0     2040 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/cfml_kernel/cfscript/install.py
--rw-rw-rw-   0        0        0     1523 2023-05-03 20:56:48.000000 cfml_kernel-0.0.1/cfml_kernel/cfscript/kernel.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:15.090819 cfml_kernel-0.0.1/cfml_kernel.egg-info/
--rw-rw-rw-   0        0        0     3620 2023-07-11 19:19:15.000000 cfml_kernel-0.0.1/cfml_kernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-11 19:19:15.000000 cfml_kernel-0.0.1/cfml_kernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:19:15.000000 cfml_kernel-0.0.1/cfml_kernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-11 19:19:15.000000 cfml_kernel-0.0.1/cfml_kernel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      616 2023-04-06 01:41:17.000000 cfml_kernel-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 19:19:15.106396 cfml_kernel-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 19:24:13.285300 cfml_kernel-1.2.0/
+-rw-rw-rw-   0        0        0     1095 2023-01-26 02:54:33.000000 cfml_kernel-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3620 2023-07-13 19:24:13.285300 cfml_kernel-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3193 2023-04-10 02:08:23.000000 cfml_kernel-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 19:24:13.259719 cfml_kernel-1.2.0/cfml_kernel/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/__init__.py
+-rw-rw-rw-   0        0        0     4819 2023-07-11 19:42:23.000000 cfml_kernel-1.2.0/cfml_kernel/box_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:24:13.276033 cfml_kernel-1.2.0/cfml_kernel/cfml/
+-rw-rw-rw-   0        0        0       34 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfml/__init__.py
+-rw-rw-rw-   0        0        0      127 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfml/__main__.py
+-rw-rw-rw-   0        0        0     2025 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfml/install.py
+-rw-rw-rw-   0        0        0     1274 2023-07-11 19:42:23.000000 cfml_kernel-1.2.0/cfml_kernel/cfml/kernel.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:24:13.283032 cfml_kernel-1.2.0/cfml_kernel/cfscript/
+-rw-rw-rw-   0        0        0       38 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfscript/__init__.py
+-rw-rw-rw-   0        0        0      135 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfscript/__main__.py
+-rw-rw-rw-   0        0        0     2040 2023-04-06 01:41:17.000000 cfml_kernel-1.2.0/cfml_kernel/cfscript/install.py
+-rw-rw-rw-   0        0        0     1308 2023-07-11 19:42:23.000000 cfml_kernel-1.2.0/cfml_kernel/cfscript/kernel.py
+drwxrwxrwx   0        0        0        0 2023-07-13 19:24:13.269840 cfml_kernel-1.2.0/cfml_kernel.egg-info/
+-rw-rw-rw-   0        0        0     3620 2023-07-13 19:24:13.000000 cfml_kernel-1.2.0/cfml_kernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-07-13 19:24:13.000000 cfml_kernel-1.2.0/cfml_kernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 19:24:13.000000 cfml_kernel-1.2.0/cfml_kernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 19:24:13.000000 cfml_kernel-1.2.0/cfml_kernel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-13 19:24:13.000000 cfml_kernel-1.2.0/cfml_kernel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-13 19:23:41.000000 cfml_kernel-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 19:24:13.286428 cfml_kernel-1.2.0/setup.cfg
```

### Comparing `cfml_kernel-0.0.1/LICENSE` & `cfml_kernel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfml_kernel-0.0.1/PKG-INFO` & `cfml_kernel-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfml_kernel
-Version: 0.0.1
+Version: 1.2.0
 Summary: A Jupyter notebook kernel for CFML powered by Commandbox
 Author-email: Jason steinshouer <jason.steinshouer@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cfml_kernel-0.0.1/README.md` & `cfml_kernel-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cfml_kernel-0.0.1/cfml_kernel/box_wrapper.py` & `cfml_kernel-1.2.0/cfml_kernel/box_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-import subprocess, os, logging, re
+import subprocess, os, logging
+
 class CommandBoxWrapper():
 
     PROMPT_STRINGS = ["CFSCRIPT-REPL: ",".............: ","CFML-REPL: ","CommandBox> ",u"\u276F "]
-    CONTINUATION_PROMPT = ".............: "
     CF_REPL_TYPE = "cfscript"
-    CF_REPL_PROMPT = "CFSCRIPT-REPL: "
-    HTML_REGEX = re.compile(r"(?:</[^<]+>)|(?:<[^<]+/>)")
 
     def __init__(self,repl_type = "cfscript", **kwargs):
         # logging.basicConfig(filename='box_wrapper_debug.log',
         #                     encoding='utf-8', level=LOG_LEVEL)
         self.CF_REPL_TYPE = repl_type
-        # New version of commandbox (5.9.0) uses a prompt with the current working directory in it
-        self.PROMPT_STRINGS.append("CommandBox:" + os.getcwd().split(os.sep)[-1] + ">");
-        if (repl_type != "cfscript"):
-            self.CF_REPL_PROMPT = "CFML-REPL: "
         self.box_shell = self._create_process()
         self._search_for_output()
         self._start_repl()
 
     def do_execute(self, code):
 
         if (code[:8] == "$install" or code[:8] == "%install"):
@@ -27,56 +21,44 @@
 
             #Run the install command
             output = self._box_install(code)
 
             #start the repl
             self._start_repl()
 
-            return [output]
-        elif (code[:8] == "$loadjar" or code[:8] == "%loadjar"):    
+            return output
+        elif (code[:8] == "$loadjar" or code[:8] == "%loadjar"):
             #Load jar
             output = self._load_jar(code)
 
-            return [output]
+            return output
         else:
             code_lines = code.splitlines()
 
-            responses = []
-            output_buffer = ""
+            response = [];
             for line in code_lines:  
                 self.box_shell.stdin.write( bytes( f"{line.strip()}\n".encode("utf-8") ) )
                 self.box_shell.stdin.flush()
-                raw_output = self._search_for_output()
-
-                if raw_output.__contains__(self.CF_REPL_PROMPT):
-                    content = self._parse_response( raw_output.replace(self.CF_REPL_PROMPT,"") )
-                    responses.append( content )
+                output = self._search_for_output()
+                
+                for string in self.PROMPT_STRINGS:
+                    output = output.replace(string,"")
+
+                if (output.__contains__("[EMPTY STRING]") == False):
+                    response.append(output.strip())
+                    # response.append("\n")
 
-            return responses
+            return "\n".join(response).strip()
     
-    def _parse_response(self,raw_output):
-            # Lame check for JSON
-            if raw_output.split()[0] in "[,{":
-                return raw_output
-            # Parse for html
-            elif bool( self.HTML_REGEX.search( raw_output ) ):
-                return {
-                    'data': {
-                        'text/html': raw_output,
-                    },
-                    'metadata': {}
-                }
-            else:
-                return raw_output
-
     def _box_install(self,code):
         self.box_shell.stdin.write(bytes(f"install {code.replace('$install','').replace('%install','')}\n".encode("utf-8")))
         self.box_shell.stdin.flush()
         output = self._search_for_output()
-        output = re.sub("CommandBox:.*>","",output).strip()
+        for string in self.PROMPT_STRINGS:
+            output = output.replace(string,"")
         return output
     
     def _load_jar(self,code):
 
         loadjar_expression = "loadJar = (path) => { \
             filePath = getDirectoryFromPath( getCurrentTemplatePath() ) & path; \
             new commandbox.system.util.FileSystem().classLoad( filePath ); \
@@ -101,14 +83,16 @@
         self.box_shell.stdin.write(bytes(cmd.encode("utf-8")))
         self.box_shell.stdin.flush()
         self._search_for_output()
 
     def _stop_repl(self):
         self.box_shell.stdin.write(bytes("q\n".encode("utf-8")))
         self.box_shell.stdin.flush()
+        self.box_shell.stdin.write(bytes("reload\n".encode("utf-8")))
+        self.box_shell.stdin.flush()
         self._search_for_output()
 
     def _create_process(self):
         my_env = os.environ.copy()
         my_env["box_config_nonInteractiveMode"] = "false"
         my_env["box_config_colorInDumbTerminal"] = "true"
         # The bullet train module prompt uses this character
```

### Comparing `cfml_kernel-0.0.1/cfml_kernel/cfml/install.py` & `cfml_kernel-1.2.0/cfml_kernel/cfml/install.py`

 * *Files identical despite different names*

### Comparing `cfml_kernel-0.0.1/cfml_kernel/cfml/kernel.py` & `cfml_kernel-1.2.0/cfml_kernel/cfml/kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,22 +17,17 @@
         Kernel.__init__(self, **kwargs)
         self.box_wrapper = CommandBoxWrapper(repl_type="cfml")
 
     def do_execute(self, code, silent, store_history=True, user_expressions=None,
                    allow_stdin=False):
         if not silent:
 
-            responses = self.box_wrapper.do_execute(code)
-
-            for content in responses:
-                if isinstance( content, str ):
-                    stream_content = {'name': 'stdout', 'text': content}
-                    self.send_response(self.iopub_socket, 'stream', stream_content)
-                else:
-                    self.send_response(self.iopub_socket, 'display_data', content)
+            output = self.box_wrapper.do_execute(code);
+            stream_content = {'name': 'stdout', 'text': output}
+            self.send_response(self.iopub_socket, 'stream', stream_content)
 
         return {'status': 'ok',
                 # The base class increments the execution count
                 'execution_count': self.execution_count,
                 'payload': [],
                 'user_expressions': {},
                }
```

### Comparing `cfml_kernel-0.0.1/cfml_kernel/cfscript/install.py` & `cfml_kernel-1.2.0/cfml_kernel/cfscript/install.py`

 * *Files identical despite different names*

### Comparing `cfml_kernel-0.0.1/cfml_kernel/cfscript/kernel.py` & `cfml_kernel-1.2.0/cfml_kernel/cfscript/kernel.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,22 +17,17 @@
         Kernel.__init__(self, **kwargs)
         self.box_wrapper = CommandBoxWrapper(repl_type="cfscript")
 
     def do_execute(self, code, silent, store_history=True, user_expressions=None,
                    allow_stdin=False):
         if not silent:
 
-            responses = self.box_wrapper.do_execute(code)
-
-            for content in responses:
-                if isinstance( content, str ):
-                    stream_content = {'name': 'stdout', 'text': content}
-                    self.send_response(self.iopub_socket, 'stream', stream_content)
-                else:
-                    self.send_response(self.iopub_socket, 'display_data', content)
+            output = self.box_wrapper.do_execute(code);
+            stream_content = {'name': 'stdout', 'text': output}
+            self.send_response(self.iopub_socket, 'stream', stream_content)
 
         return {'status': 'ok',
                 # The base class increments the execution count
                 'execution_count': self.execution_count,
                 'payload': [],
                 'user_expressions': {},
                }
```

### Comparing `cfml_kernel-0.0.1/cfml_kernel.egg-info/PKG-INFO` & `cfml_kernel-1.2.0/cfml_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfml-kernel
-Version: 0.0.1
+Version: 1.2.0
 Summary: A Jupyter notebook kernel for CFML powered by Commandbox
 Author-email: Jason steinshouer <jason.steinshouer@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `cfml_kernel-0.0.1/pyproject.toml` & `cfml_kernel-1.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,25 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfml_kernel"
-version = "0.0.1"
+version = "1.2.0"
 authors = [
   { name="Jason steinshouer", email="jason.steinshouer@gmail.com" },
 ]
 description = "A Jupyter notebook kernel for CFML powered by Commandbox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "ipykernel"
+]
 
 [tool.setuptools]
 packages = ['cfml_kernel','cfml_kernel.cfml','cfml_kernel.cfscript']
```

