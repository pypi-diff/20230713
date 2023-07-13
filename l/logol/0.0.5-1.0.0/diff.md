# Comparing `tmp/logol-0.0.5.tar.gz` & `tmp/logol-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logol-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "logol-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `logol-0.0.5.tar` & `logol-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     3161 2022-02-11 11:53:48.259908 logol-0.0.5/.gitignore
--rw-r--r--   0        0        0     1105 2022-12-26 16:09:44.368041 logol-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2022-12-26 12:31:09.358622 logol-0.0.5/README.md
--rw-r--r--   0        0        0     4374 2023-05-19 17:51:14.960008 logol-0.0.5/logol.py
--rw-r--r--   0        0        0      417 2023-05-19 18:18:36.913952 logol-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      555 2023-05-19 17:11:02.794317 logol-0.0.5/test.py
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 logol-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 16:39:49.609857 logol-1.0.0/LICENSE
+-rw-r--r--   0        0        0       55 2023-07-13 16:39:49.609857 logol-1.0.0/README.md
+-rw-r--r--   0        0        0     4250 2023-07-13 16:39:49.609857 logol-1.0.0/logol.py
+-rw-r--r--   0        0        0      403 2023-07-13 16:39:49.609857 logol-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      349 1970-01-01 00:00:00.000000 logol-1.0.0/PKG-INFO
```

### Comparing `logol-0.0.5/LICENSE` & `logol-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2022 Joseíto Oliveira
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2022 Joseíto Oliveira
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `logol-0.0.5/logol.py` & `logol-1.0.0/logol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""Pre-configured logs"""
-__version__ = '0.0.5'
-
-import logging
-from logging.handlers import RotatingFileHandler
-from logging import Logger
-from typing import Dict, Optional
-from time import time_ns
-from pathlib import Path
-
-
-FORMAT_LOGGER = '%(asctime)s [%(filename)s@%(threadName)s] %(levelname)-8s -> %(message)s'
-FORMAT_PRINTER = '%(asctime)s @%(threadName)s -> %(message)s'
-BASE_PATH = str(Path().home() / 'Logs')
-
-__loggers: Dict[str, Logger] = {}
-__printers: Dict[str, Logger] = {}
-
-
-def __configure_logger(logger, logpath, filesize_mb):
-    logger.setLevel(logging.DEBUG)
-
-    formatter = logging.Formatter(fmt=FORMAT_LOGGER, datefmt='%d/%b/%y %H:%M:%S')
-    if logpath:
-        if filesize_mb:
-            logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024)
-        else:
-            logfile = logging.FileHandler(logpath)
-        logfile.setLevel(logging.DEBUG)
-        logfile.setFormatter(formatter)
-        logger.addHandler(logfile)
-    
-    console = logging.StreamHandler()
-    console.setLevel(logging.INFO)
-    console.setFormatter(formatter)
-
-    logger.addHandler(console)
-
-    return logger
-
-def __default_printer(filename, filesize_mb=5):
-    logger = logging.getLogger(str(time_ns()))
-    logger.setLevel(logging.DEBUG)
-    
-    filename = Path(filename)
-    logpath = Path(BASE_PATH) / filename.relative_to(filename.anchor)
-    logpath.parent.mkdir(parents=True, exist_ok=True)
-
-    logpath = logpath.with_suffix('.log')
-    
-    formatter = logging.Formatter(fmt=FORMAT_PRINTER, datefmt='%d/%b/%y %H:%M:%S')
-    logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024)
-
-    logfile.setLevel(logging.DEBUG)
-    logfile.setFormatter(formatter)
-    logger.addHandler(logfile)
-    
-    console = logging.StreamHandler()
-    console.setLevel(logging.INFO)
-    console.setFormatter(formatter)
-
-    logger.addHandler(console)
-
-    return logger
-
-def remove_handlers(logger):
-    while len(logger.handlers) != 0:
-        logger.removeHandler(logger.handlers[0])
-    
-    return logger
-
-def get_logger(name, logpath=None, filesize_mb:Optional[int]=None, force:bool=False):
-    """Get a Logger object from the logging module partly configured.
-
-    Args:
-        name (str): Name of log.
-        logpath (str, optional): Path to log file. Defaults to None.
-        filesize_mb (Optional[int], optional): Maximum size of log file. Defaults to None.
-
-    Returns:
-        Logger: A Logger object from the logging module.
-    """
-
-    if name not in __loggers:
-        logger = logging.getLogger(name)
-        logger = __configure_logger(logger, logpath, filesize_mb)
-        __loggers[name] = logger
-        return logger
-    elif force:
-        logger = __loggers[name]
-        logger.warning(f'Reconfiguring the log called {name} to {logpath=}, {filesize_mb=}')
-        logger = remove_handlers(logger)
-        logger = __configure_logger(logger, logpath, filesize_mb)
-        return logger
-    else:   
-        logger = __loggers[name]
-        logger.warn(f'Trying to create a log with {logpath=} and {filesize_mb=}  but a log '
-                    f'with name {name} already exists. To force this operatin use force=True')
-        return logger
-
-
-def get_print_debug(logpath, filesize_mb:int=5):
-    """Get print and debug functions with logfile
-
-    Args:
-        logpath (str): path to log file
-        filesize_mb (int, optional): max size to log file. Defaults to 5.
-
-    Raises:
-        ValueError: raised when exists a printer with same path.
-
-    Returns:
-        (print, debug): Tuple with functions for print and debug.
-    """
-    if logpath in __printers:
-        raise ValueError
-
-    printer = __default_printer(logpath, filesize_mb)
-    __printers[logpath] = printer
-    return printer.info, printer.debug
-
-if __name__ == '__main__':
-    BASE_PATH = '.'
-
-    print, debug = get_print_debug(__file__)
-    print('Olá mundo!')
-    debug('Olá arquivo!')
-
-    log = get_logger('test', 'test.log', 1)
-    log.debug('Debung')
-    log.info('Information')
-    log.warning('Warning')
-    try:
-        1/0
-    except ZeroDivisionError:
-        log.exception('Exception')
-    log.error('Error')
-    log.critical('Critical')
-
+"""Pre-configured logs"""
+__version__ = '1.0.0'
+
+import logging
+from logging.handlers import RotatingFileHandler
+from logging import Logger
+from typing import Dict, Optional
+from time import time_ns
+from pathlib import Path
+
+
+FORMAT_LOGGER = '%(asctime)s [%(filename)s@%(threadName)s] %(levelname)-8s -> %(message)s'
+FORMAT_PRINTER = '%(asctime)s @%(threadName)s -> %(message)s'
+BASE_PATH = str(Path().home() / 'Logs')
+
+__loggers: Dict[str, Logger] = {}
+__printers: Dict[str, Logger] = {}
+
+
+def __configure_logger(logger, logpath, filesize_mb):
+    logger.setLevel(logging.DEBUG)
+
+    formatter = logging.Formatter(fmt=FORMAT_LOGGER, datefmt='%d/%b/%y %H:%M:%S')
+    if logpath:
+        if filesize_mb:
+            logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024)
+        else:
+            logfile = logging.FileHandler(logpath)
+        logfile.setLevel(logging.DEBUG)
+        logfile.setFormatter(formatter)
+        logger.addHandler(logfile)
+    
+    console = logging.StreamHandler()
+    console.setLevel(logging.INFO)
+    console.setFormatter(formatter)
+
+    logger.addHandler(console)
+
+    return logger
+
+def __default_printer(filename, filesize_mb=5):
+    logger = logging.getLogger(str(time_ns()))
+    logger.setLevel(logging.DEBUG)
+    
+    filename = Path(filename)
+    logpath = Path(BASE_PATH) / filename.relative_to(filename.anchor)
+    logpath.parent.mkdir(parents=True, exist_ok=True)
+
+    logpath = logpath.with_suffix('.log')
+    
+    formatter = logging.Formatter(fmt=FORMAT_PRINTER, datefmt='%d/%b/%y %H:%M:%S')
+    logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024, backupCount=1)
+
+    logfile.setLevel(logging.DEBUG)
+    logfile.setFormatter(formatter)
+    logger.addHandler(logfile)
+    
+    console = logging.StreamHandler()
+    console.setLevel(logging.INFO)
+    console.setFormatter(formatter)
+
+    logger.addHandler(console)
+
+    return logger
+
+def remove_handlers(logger):
+    while len(logger.handlers) != 0:
+        logger.removeHandler(logger.handlers[0])
+    
+    return logger
+
+def get_logger(name, logpath=None, filesize_mb:Optional[int]=None, force:bool=False):
+    """Get a Logger object from the logging module partly configured.
+
+    Args:
+        name (str): Name of log.
+        logpath (str, optional): Path to log file. Defaults to None.
+        filesize_mb (Optional[int], optional): Maximum size of log file. Defaults to None.
+
+    Returns:
+        Logger: A Logger object from the logging module.
+    """
+
+    if name not in __loggers:
+        logger = logging.getLogger(name)
+        logger = __configure_logger(logger, logpath, filesize_mb)
+        __loggers[name] = logger
+        return logger
+    elif force:
+        logger = __loggers[name]
+        logger.warning(f'Reconfiguring the log called {name} to {logpath=}, {filesize_mb=}')
+        logger = remove_handlers(logger)
+        logger = __configure_logger(logger, logpath, filesize_mb)
+        return logger
+    else:   
+        logger = __loggers[name]
+        logger.warn(f'Trying to create a log with {logpath=} and {filesize_mb=}  but a log '
+                    f'with name {name} already exists. To force this operatin use force=True')
+        return logger
+
+
+def get_print_debug(logpath, filesize_mb:int=5):
+    """Get print and debug functions with logfile
+
+    Args:
+        logpath (str): path to log file
+        filesize_mb (int, optional): max size to log file. Defaults to 5.
+
+    Raises:
+        ValueError: raised when exists a printer with same path.
+
+    Returns:
+        (print, debug): Tuple with functions for print and debug.
+    """
+    if logpath in __printers:
+        raise ValueError
+
+    printer = __default_printer(logpath, filesize_mb)
+    __printers[logpath] = printer
+    return printer.info, printer.debug
+
+if __name__ == '__main__':
+    BASE_PATH = '.'
+
+    print, debug = get_print_debug(__file__)
+    print('Olá mundo!')
+    debug('Olá arquivo!')
+
+    log = get_logger('test', 'test.log', 1)
+    log.debug('Debung')
+    log.info('Information')
+    log.warning('Warning')
+    try:
+        1/0
+    except ZeroDivisionError:
+        log.exception('Exception')
+    log.error('Error')
+    log.critical('Critical')
+
```

