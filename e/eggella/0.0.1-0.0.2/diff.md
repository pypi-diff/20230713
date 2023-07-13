# Comparing `tmp/eggella-0.0.1.tar.gz` & `tmp/eggella-0.0.2.tar.gz`

## Comparing `eggella-0.0.1.tar` & `eggella-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/__init__.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/app.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/exceptions.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/manager.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/abc.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/command.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/completer.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/handler.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/command/objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/events/abc.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/events/events.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.1/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.1/.gitignore
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 eggella-0.0.1/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 eggella-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/__init__.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/app.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/exceptions.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/manager.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/abc.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/command.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/completer.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/exception_handle.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/handler.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/command/objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/abc.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/events/events.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.2/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.2/.gitignore
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 eggella-0.0.2/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 eggella-0.0.2/PKG-INFO
```

### Comparing `eggella-0.0.1/eggella/app.py` & `eggella-0.0.2/eggella/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,36 +45,47 @@
         self.app_name = app_name
         self.prompt_msg = msg
         self.session: PromptSession = PromptSession(msg)
         self.cmd = CmdShortCuts()
 
         self.CTX: Dict[Hashable, Any] = {}
         self._intro: Union[HTML, PromptLikeMsg] = _DEFAULT_INTRO_MSG
-
+        self._doc: str = ""
         # managers
         self._command_manager: CommandManager = CommandManager(self)
         self._event_manager = EventManager(self)
 
         # fsm
         self.fsm = FsmController(self)
 
     @property
+    def documentation(self):
+        return self._doc
+
+    @documentation.setter
+    def documentation(self, text: str):
+        self._doc = text
+
+    @property
     def intro(self):
         return self._intro
 
     @intro.setter
     def intro(self, text: Union[HTML, PromptLikeMsg]):
         self._intro = text
 
     def on_startup(self):
         return self._event_manager.startup()
 
     def on_close(self):
         return self._event_manager.close()
 
+    def on_error(self, *errors: Type[BaseException]):
+        return self._command_manager.on_error(*errors)
+
     def on_command(
         self,
         key: Optional[str] = None,
         short_description: Optional[str] = None,
         *,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
@@ -166,14 +177,15 @@
                     continue
 
                 if (tokens := result.split(" ", 1)) and len(tokens) == 1:
                     key = tokens[0]
                     args = ""
                 else:
                     key, args = tokens[0], tokens[1]
+
                 if result := self._command_manager.exec(key, args):
                     self._event_manager.command_complete_event(result)
             except CommandNotFoundError:
                 self._event_manager.command_not_found_event(key, args)
                 self._event_manager.command_suggest_event(key, self._command_manager.commands.keys())
             except CommandParseError:
                 self._event_manager.command_error_event(key, args)
```

### Comparing `eggella-0.0.1/eggella/manager.py` & `eggella-0.0.2/eggella/manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,20 @@
+import shlex
 from functools import wraps
-from typing import TYPE_CHECKING, Callable, Dict, List, Literal, Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+)
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.completer import CommandCompleter
 from eggella.command.handler import CommandHandler
 from eggella.command.objects import Command
 from eggella.events.events import (
     OnCommandCompleteSuccess,
@@ -16,36 +27,85 @@
 from eggella.exceptions import CommandNotFoundError
 from eggella.shortcuts.help_pager import gen_help_pager
 
 if TYPE_CHECKING:
     from eggella.app import Eggella
 
 
+_ErrorEventsMapping = Dict[str, Tuple[Type[BaseException], ...]]
+
+
 class CommandManager:
     def __init__(self, app: "Eggella"):
         self._app = app
         self.commands: Dict[str, Command] = {}
+        self.error_events: Dict[str, Callable[[str, BaseException, str, str], Any]] = {}
+        self.handled_exceptions: _ErrorEventsMapping = {}
         self._register_buildin_commands()
 
+    @staticmethod
+    def _simple_parse_arguments(raw_command: str) -> Tuple[Tuple[str, ...], Dict[str, str]]:
+        tokens = shlex.split(raw_command)
+        args: List[str] = []
+        kwargs: Dict[str, str] = {}
+        for token in tokens:
+            if "=" in token:
+                key, value = token.split("=", 1)
+                kwargs[key] = value
+            else:
+                args.append(token)
+        return tuple(args), kwargs
+
     def exec(self, key: str, args: str):
-        if command := self.commands.get(key):
+        command = self.get(key)
+        try:
             return command.handle(args)
-        else:
-            raise CommandNotFoundError("Command not fouded")
+        except BaseException as e:
+            if err_handler := self.error_events.get(command.fn.__name__):
+                handle_exceptions = self.handled_exceptions.get(command.fn.__name__, None)
+                if handle_exceptions and any(e.__class__ == exc for exc in handle_exceptions):
+                    _args, _kwargs = self._simple_parse_arguments(args)
+                    return err_handler(key, e, *_args, **_kwargs)
+                else:
+                    raise e
+            raise e
 
     def get_completer(self) -> CommandCompleter:
-        return CommandCompleter(self)
+        return CommandCompleter(self)  # type: ignore
+
+    def on_error(self, *errors: Type[BaseException]):
+        def decorator(handler: Callable[[str, BaseException, str, str], Any]):
+            @wraps(handler)
+            def decorator_wrapper(func: Callable[..., Any]):
+                if not self.error_events.get(func.__name__):
+                    self.error_events[func.__name__] = handler
+                    self.handled_exceptions[func.__name__] = errors
+
+                @wraps(func)
+                def wrapper(*args, **kwargs):
+                    try:
+                        return func(*args, **kwargs)
+                    except BaseException as e:
+                        if any(e.__class__ == exc for exc in errors):
+                            return handler("", e, *args, **kwargs)
+                        raise e
+
+                return wrapper
+
+            return decorator_wrapper
+
+        return decorator
 
     @property
-    def all_completions(self):
+    def all_completions(self) -> List[Tuple[str, str]]:
         return [com.completion for com in self.commands.values()]
 
     def get(self, key: str) -> Command:
-        if comma := self.commands.get(key, None):
-            return comma
+        if command := self.commands.get(key, None):
+            return command
         raise CommandNotFoundError(f"Command {key} not founded")
 
     def command(
         self,
         key: Optional[str] = None,
         *,
         short_description: Optional[str] = None,
@@ -100,16 +160,16 @@
                 usage=usage,
             )
 
     def _help_command(self, key: Optional[str] = None):
         """show help or show pager documentation for all commands if not argument passed"""
         if not key:
             commands = self.commands.values()
-            gen_help_pager(commands)
-            return ""
+            gen_help_pager(self._app, commands)
+            return
         elif comma := self.commands.get(key):
             return f"{key} - {comma.short_desc}"
         else:
             raise CommandNotFoundError
 
     @staticmethod
     def _exit_command():
@@ -122,14 +182,15 @@
 
 
 class EventManager:
     def __init__(self, app: "Eggella"):
         self.app = app
         self.startup_events: List[Callable] = []
         self.close_events: List[Callable] = []
+        self.errors_events: Dict[str, Callable] = {}
 
         self.kb_interrupt_event: Callable[..., bool] = OnKeyboardInterrupt()
         self.eof_event: Callable[..., bool] = OnEOFError()
         self.command_error_event: Callable[..., None] = OnCommandError()
         self.command_not_found_event: Callable[..., None] = OnCommandNotFound()
         self.command_complete_event: Callable[..., None] = OnCommandCompleteSuccess()
         self.command_suggest_event: Optional[Callable[..., None]] = OnSuggest()
```

### Comparing `eggella-0.0.1/eggella/command/command.py` & `eggella-0.0.2/eggella/command/command.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/eggella/command/completer.py` & `eggella-0.0.2/eggella/command/completer.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/eggella/command/handler.py` & `eggella-0.0.2/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/eggella/command/objects.py` & `eggella-0.0.2/eggella/command/objects.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import Any, Callable, Dict, NamedTuple, Optional, Tuple
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.handler import CommandHandler
 
 
 class Command(NamedTuple):
     fn: Callable[..., Any]
@@ -13,34 +13,39 @@
     short_description: Optional[str] = None
 
     def handle(self, command_text: str) -> Tuple[Tuple[Any, ...], Dict[str, Any]]:
         args, kwargs = self.handler.handle(self.fn, command_text)
         return self.fn(*args, **kwargs)
 
     @property
-    def short_desc(self):
+    def arguments(self) -> List[str]:
         args = inspect.signature(self.fn).parameters.values()
-        arg_list = ", ".join(str(arg) for arg in args)
-        docstring = inspect.getdoc(self.fn) or ""
+        return [str(arg) for arg in args]
+
+    @property
+    def docstring(self) -> str:
+        return inspect.getdoc(self.fn) or ""
+
+    @property
+    def short_desc(self):
+        arg_list = " ".join(f"[{arg}]" for arg in self.arguments)
         if self.short_description:
             return f"({arg_list}) - {self.short_description}"
-        elif docstring:
-            short_desc = docstring.split("\n")[0]
-            return f"({arg_list}) - {short_desc}"
-        return f"({arg_list})"
+        elif self.docstring:
+            short_desc = self.docstring.split("\n")[0]
+            return f"{arg_list} - {short_desc}"
+        return f"{arg_list}"
 
     @property
-    def completion(self):
+    def completion(self) -> Tuple[str, str]:
         return self.key, self.short_desc
 
     @property
     def help(self):
-        args = inspect.signature(self.fn).parameters.values()
-        arg_list = ", ".join(str(arg) for arg in args)
-        docstring = inspect.getdoc(self.fn) or ""
-        if len(docstring.split("\n")) > 1:
+        arg_list = " ".join(f"[{arg}]" for arg in self.arguments)
+        if len(self.docstring.split("\n")) > 1:
             if self.usage:
-                return f"{self.key} ({arg_list})\n\t{docstring}\nUSAGE:\n\t{self.usage}"
-            return f"{self.key} ({arg_list})\n\t{docstring}"
+                return f"      {self.key} ({arg_list})\n            {self.docstring}\nUSAGE:\n      {self.usage}"
+            return f"      {self.key} ({arg_list})\n            {self.docstring}"
         if self.usage:
-            return f"{self.key} ({arg_list}) - {docstring}\n\tUSAGE:\n{self.usage}"
-        return f"{self.key} ({arg_list}) - {docstring}"
+            return f"      {self.key} ({arg_list}) - {self.docstring}\nUSAGE:\n      {self.usage}"
+        return f"      {self.key} ({arg_list}) - {self.docstring}"
```

### Comparing `eggella-0.0.1/eggella/events/events.py` & `eggella-0.0.2/eggella/events/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,7 +78,12 @@
 
 class OnCommandCompleteSuccess(ABCEvent):
     _STYLE = Style.from_dict({"out": "#696969 bold"})
 
     def __call__(self, result: Any):
         if result:
             print_ft(HTML(f"<out>{result}</out>"), style=self._STYLE)
+
+
+class OnCommandArgumentsException(ABCEvent):
+    def __call__(self, key: str, error: BaseException, *args, **kwargs):
+        pass
```

### Comparing `eggella-0.0.1/eggella/fsm/fsm.py` & `eggella-0.0.2/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.2/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/eggella/tools/type_caster.py` & `eggella-0.0.2/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/.gitignore` & `eggella-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/README.md` & `eggella-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 - python 3.8+ support
 - arguments auto cast from function annotations
 - cross-platform (prompt-toolkit guarantees)
 - FSM
 - customized events
 - completer
 - ctx storage (dict)
+## Install
+
+`pip install eggella`
 
 ## Examples:
 
 ### Basic
 
 ```python
 from eggella import Eggella
```

### Comparing `eggella-0.0.1/pyproject.toml` & `eggella-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.1/PKG-INFO` & `eggella-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,17 @@
 - python 3.8+ support
 - arguments auto cast from function annotations
 - cross-platform (prompt-toolkit guarantees)
 - FSM
 - customized events
 - completer
 - ctx storage (dict)
+## Install
+
+`pip install eggella`
 
 ## Examples:
 
 ### Basic
 
 ```python
 from eggella import Eggella
```

