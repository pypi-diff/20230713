# Comparing `tmp/suitable-0.8.1.tar.gz` & `tmp/suitable-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suitable-0.8.1.tar", last modified: Thu Aug 10 11:42:46 2017, max compression
+gzip compressed data, was "dist/suitable-0.9.0.tar", last modified: Tue Sep 19 09:27:08 2017, max compression
```

## Comparing `suitable-0.8.1.tar` & `suitable-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2017-08-10 11:42:46.000000 suitable-0.8.1/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4673 2017-08-10 11:42:46.000000 suitable-0.8.1/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     1524 2017-08-10 11:42:08.000000 suitable-0.8.1/setup.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable/tests/
--rw-rw-r--   0 travis    (1000) travis    (1000)     5485 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/tests/test_api.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1074 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/errors.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     9021 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/api.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      962 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/runner_results.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      230 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/compat.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      707 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/callback.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      162 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/common.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6903 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/module_runner.py
--rw-rw-r--   0 travis    (1000) travis    (1000)       48 2017-08-10 11:42:08.000000 suitable-0.8.1/suitable/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4673 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)        9 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       33 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2017-08-10 11:42:16.000000 suitable-0.8.1/suitable.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)      434 2017-08-10 11:42:46.000000 suitable-0.8.1/suitable.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      109 2017-08-10 11:42:08.000000 suitable-0.8.1/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)    35148 2017-08-10 11:42:08.000000 suitable-0.8.1/LICENSE
--rw-rw-r--   0 travis    (1000) travis    (1000)     2956 2017-08-10 11:42:08.000000 suitable-0.8.1/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)       67 2017-08-10 11:42:46.000000 suitable-0.8.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-19 09:27:08.000000 suitable-0.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5410 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      109 2017-09-19 09:26:21.000000 suitable-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3497 2017-09-19 09:26:21.000000 suitable-0.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35148 2017-09-19 09:26:21.000000 suitable-0.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6412 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/module_runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      962 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/runner_results.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2017-09-19 09:27:08.000000 suitable-0.9.0/suitable/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5556 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/tests/test_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      707 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/callback.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9352 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2017-09-19 09:26:21.000000 suitable-0.9.0/suitable/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2017-09-19 09:27:08.000000 suitable-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1673 2017-09-19 09:26:21.000000 suitable-0.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5410 2017-09-19 09:27:08.000000 suitable-0.9.0/PKG-INFO
```

### Comparing `suitable-0.8.1/PKG-INFO` & `suitable-0.9.0/suitable.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: suitable
-Version: 0.8.1
+Version: 0.9.0
 Summary: Suitable is a thin wrapper around the Ansible API.
 Home-page: http://github.com/seantis/suitable/
 Author: Denis Krienbühl
 Author-email: denis@href.ch
 License: GPLv3
 Description: Suitable
         ========
@@ -52,14 +52,30 @@
         
         .. image:: https://badge.fury.io/py/suitable.svg
             :target: https://badge.fury.io/py/suitable
             :alt: Latest release
         
         Changelog
         ---------
+        0.9.0 (2017-09-19)
+        ~~~~~~~~~~~~~~~~~~~
+        
+        - Adds support for Ansible 2.4. Since this release introduces many changes
+          under the hood support for Ansible 2.3 has been dropped!
+        
+          You might want to assume that this will stay this way. Older Ansible
+          releases are supported if possible, but it's not a goal of this project.
+          [href]
+        
+        - Explicitly drops support for Python 3.0 - 3.4. Suitable supports the same
+          Python versions Ansible supports, which excludes these 3.x releases.
+        
+          Supported are therefore Python 2.7, 3.5 and 3.6+.
+          [href]
+        
         0.8.1 (2017-08-10)
         ~~~~~~~~~~~~~~~~~~~
         
         - Adds support for Ansible's extra_vars.
           [Liuyanglong]
         
         0.8.0 (2017-06-02)
@@ -152,7 +168,8 @@
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
```

### Comparing `suitable-0.8.1/setup.py` & `suitable-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,28 +29,30 @@
         import subprocess
         errno = subprocess.call([sys.executable, 'runtests.py'])
         raise SystemExit(errno)
 
 
 setup(
     name='suitable',
-    version='0.8.1',
+    version='0.9.0',
     url='http://github.com/seantis/suitable/',
     license='GPLv3',
     author='Denis Krienbühl',
     author_email='denis@href.ch',
     description=description,
     long_description='\n'.join(get_long_description()),
     packages=['suitable'],
     include_package_data=True,
     zip_safe=False,
     platforms='any',
     install_requires=[
-        'ansible>=2.3.0.0'
+        'ansible>=2.4.0.0'
     ],
+    # Ansible does not support Python 3.0 through 3.4, so we do not either
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
     extras_require={
         'tests': [
             'pytest',
         ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `suitable-0.8.1/suitable/tests/test_api.py` & `suitable-0.9.0/suitable/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import os.path
 import pytest
 import shutil
 import tempfile
 
-from ansible import inventory
 from suitable.api import list_ansible_modules, Api
 from suitable.errors import UnreachableError, ModuleError
 from suitable.runner_results import RunnerResults
+from suitable.compat import text_type
 
 
 def test_auto_localhost():
     host = Api('localhost')
     assert host.options.connection == 'local'
 
     host = Api('localhost', connection='smart')
@@ -22,21 +22,14 @@
     host = Api('localhost', sudo=True)
     try:
         assert host.command('whoami').stdout() == 'root'
     except ModuleError as e:
         assert 'password' in e.result['module_stderr']
 
 
-def test_no_global_state():
-    # turn the cached value into something unusable, if we don't clear it
-    # correctly, an error will arise
-    inventory.HOSTS_PATTERNS_CACHE['all'] = None
-    Api('localhost').command('whoami')
-
-
 def test_module_args():
     upgrade = (
         'apt-get upgrade -y -o Dpkg::Options::="--force-confdef" '
         '-o Dpkg::Options::="--force-confold"'
     )
 
     try:
@@ -186,15 +179,15 @@
 
 def test_error_string():
     try:
         Api('localhost').command('whoami | less')
     except ModuleError as e:
         # we don't have a msg so we mock that out, for coverage!
         e.result['msg'] = '0xdeadbeef'
-        error_string = str(e)
+        error_string = text_type(e)
 
         # we don't make many guarantees with the string messages, so
         # a basic somke test suffices here. This is not something to
         # depend on.
 
         assert '0xdeadbeef' in error_string
         assert 'command: whoami | less' in error_string
@@ -211,9 +204,22 @@
         os.mkdir(special_dir)
 
         api = Api('localhost')
         api.file(
             dest=os.path.join(special_dir, 'foo.txt'),
             state='touch'
         )
+
+    finally:
+        shutil.rmtree(tempdir)
+
+
+def test_extra_vars():
+    tempdir = tempfile.mkdtemp()
+
+    try:
+        api = Api('localhost', extra_vars={'path': tempdir})
+        api.file(dest="{{ path }}/foo.txt", state='touch')
+
+        assert os.path.exists(tempdir + '/foo.txt')
     finally:
         shutil.rmtree(tempdir)
```

### Comparing `suitable-0.8.1/suitable/errors.py` & `suitable-0.9.0/suitable/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,32 @@
         self.host = host
         self.result = result
 
     def __str__(self):
         output = []
 
         if 'msg' in self.result:
-            output.append("Message: {}".format(self.result['msg']))
+            output.append(u"Message: {}".format(self.result['msg']))
 
         if 'rc' in self.result:
-            output.append("Returncode: {}".format(self.result['rc']))
+            output.append(u"Returncode: {}".format(self.result['rc']))
 
         if 'stdout' in self.result:
-            output.append("Stdout:\n{}".format(self.result['stdout']))
+            output.append(u"Stdout:\n{}".format(self.result['stdout']))
 
         if 'stderr' in self.result:
-            output.append("Stderr:\n{}".format(self.result['stderr']))
+            output.append(u"Stderr:\n{}".format(self.result['stderr']))
 
-        return "Error running '{module}' on {host}\n{output}".format(
+        return u"Error running '{module}' on {host}\n{output}".format(
             module=self.module,
             host=self.host,
             output='\n'.join(output)
         )
 
 
 class UnreachableError(SuitableError):
     def __init__(self, module, host):
         self.module = module
         self.host = host
 
     def __str__(self):
-        return "{host} could not be reached".format(host=self.host)
+        return u"{host} could not be reached".format(host=self.host)
```

### Comparing `suitable-0.8.1/suitable/api.py` & `suitable-0.9.0/suitable/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 
 from ansible import constants as C
-from ansible.plugins import module_loader
+from ansible.plugins.loader import module_loader
 from contextlib import contextmanager
 from suitable.compat import string_types
 from suitable.errors import UnreachableError, ModuleError
 from suitable.module_runner import ModuleRunner
 
 
 VERBOSITY = {
@@ -97,14 +97,20 @@
             `<http://docs.ansible.com/ansible/developing_api.html>`_
 
             A common option would be to use the commands on the server
             as a different user using sudo::
 
                 Api('webserver', become=True, become_user='www-data')
 
+            You can also add extra variables. Note that those will be global
+            and not bound to any particular host::
+
+                api = Api('webserver', extra_vars={'home': '/home/denis'})
+                api.file(dest="{{ home }}/.zshrc", state='touch')
+
         """
         if isinstance(servers, string_types):
             self.servers = servers.split(u' ')
         else:
             self.servers = list(servers)
 
         # if the target is the local host but the transport is not set default
@@ -145,14 +151,15 @@
 
         # unfortunately, not all options seem to have accessible defaults
         options['ssh_common_args'] = options.get('ssh_common_args', None)
         options['ssh_extra_args'] = options.get('ssh_extra_args', None)
         options['sftp_extra_args'] = options.get('sftp_extra_args', None)
         options['scp_extra_args'] = options.get('scp_extra_args', None)
         options['extra_vars'] = options.get('extra_vars', {})
+        options['diff'] = options.get('diff', False)
         options['verbosity'] = VERBOSITY.get(verbosity)
         options['check'] = dry_run
 
         if 'passwords' not in options:
             options['passwords'] = {
                 'conn_pass': (
                     options.get('remote_pass') or options.get('conn_pass')
```

### Comparing `suitable-0.8.1/suitable/runner_results.py` & `suitable-0.9.0/suitable/runner_results.py`

 * *Files identical despite different names*

### Comparing `suitable-0.8.1/suitable/callback.py` & `suitable-0.9.0/suitable/callback.py`

 * *Files identical despite different names*

### Comparing `suitable-0.8.1/suitable/module_runner.py` & `suitable-0.9.0/suitable/module_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from ansible import inventory as ansible_inventory
 from ansible.executor.task_queue_manager import TaskQueueManager
 from ansible.parsing.dataloader import DataLoader
+from ansible.inventory.manager import InventoryManager
 from ansible.playbook.play import Play
-from ansible.vars import VariableManager
+from ansible.vars.manager import VariableManager
 from datetime import datetime
 from pprint import pformat
 from suitable.callback import SilentCallbackModule
 from suitable.common import log
 from suitable.runner_results import RunnerResults
 
 
-class UncachedInventory(ansible_inventory.Inventory):
-    """ Ansible uses an inventory with a global cache, which messes with our
-    execution model. We want an inventory to be bound to an api and nothing
-    else.
+class SourcelessInventoryManager(InventoryManager):
+    """ A custom inventory manager that turns the source parsing into a noop.
 
-    This Inventory makes sure that no global state is touched.
+    Without this, Ansible will warn that there are no inventory sources that
+    could be parsed. Naturally we do not have such sources, rendering this
+    warning moot.
 
     """
 
-    def get_hosts(self, *args, **kwargs):
-        if hasattr(ansible_inventory, 'HOSTS_PATTERNS_CACHE'):
-            ansible_inventory.HOSTS_PATTERNS_CACHE = {}
-
-        return super(UncachedInventory, self).get_hosts(*args, **kwargs)
+    def parse_sources(self):
+        pass
 
 
 class ModuleRunner(object):
 
     def __init__(self, module_name):
         """ Runs any ansible module given the module's name and access
         to the api instance (done through the hookup method).
@@ -77,31 +74,24 @@
         """
 
         assert self.is_hooked_up, "the module should be hooked up to the api"
 
         self.module_args = module_args = self.get_module_args(args, kwargs)
 
         loader = DataLoader()
-        variable_manager = VariableManager()
-        variable_manager.extra_vars = self.api.options.extra_vars
+        inventory_manager = SourcelessInventoryManager(loader=loader)
 
-        # Ansible has some support for host lists, but it assumes at times
-        # that these host lists are not in fact lists but a string pointing
-        # to a host list file. The easiest way to make sure that Ansible gets
-        # what we want is to pass a host list as a string which always contains
-        # at least one comma so that ansible knows it's a string of hosts.
-        host_list = ','.join(self.api.servers) + ','
+        for host in self.api.servers:
+            inventory_manager._inventory.add_host(host, group='all')
 
-        inventory = UncachedInventory(
-            loader=loader,
-            variable_manager=variable_manager,
-            host_list=host_list
-        )
+        for key, value in self.api.options.extra_vars.items():
+            inventory_manager._inventory.set_variable('all', key, value)
 
-        variable_manager.set_inventory(inventory)
+        variable_manager = VariableManager(
+            loader=loader, inventory=inventory_manager)
 
         play_source = {
             'name': "Suitable Play",
             'hosts': self.api.servers,
             'gather_facts': 'no',
             'tasks': [{
                 'action': {
@@ -124,15 +114,15 @@
 
         start = datetime.utcnow()
         task_queue_manager = None
         callback = SilentCallbackModule()
 
         try:
             task_queue_manager = TaskQueueManager(
-                inventory=inventory,
+                inventory=inventory_manager,
                 variable_manager=variable_manager,
                 loader=loader,
                 options=self.api.options,
                 passwords=getattr(self.api.options, 'passwords', {}),
                 stdout_callback=callback
             )
             task_queue_manager.run(play)
@@ -174,15 +164,15 @@
             ))
 
         for server, answer in callback.contacted.items():
 
             success = answer['success']
             result = answer['result']
 
-            if 'failed' in result:
+            if result.get('failed'):
                 success = False
 
             if 'rc' in result:
                 if self.api.is_valid_return_code(result['rc']):
                     success = True
 
             if not success:
```

### Comparing `suitable-0.8.1/suitable.egg-info/PKG-INFO` & `suitable-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: suitable
-Version: 0.8.1
+Version: 0.9.0
 Summary: Suitable is a thin wrapper around the Ansible API.
 Home-page: http://github.com/seantis/suitable/
 Author: Denis Krienbühl
 Author-email: denis@href.ch
 License: GPLv3
 Description: Suitable
         ========
@@ -52,14 +52,30 @@
         
         .. image:: https://badge.fury.io/py/suitable.svg
             :target: https://badge.fury.io/py/suitable
             :alt: Latest release
         
         Changelog
         ---------
+        0.9.0 (2017-09-19)
+        ~~~~~~~~~~~~~~~~~~~
+        
+        - Adds support for Ansible 2.4. Since this release introduces many changes
+          under the hood support for Ansible 2.3 has been dropped!
+        
+          You might want to assume that this will stay this way. Older Ansible
+          releases are supported if possible, but it's not a goal of this project.
+          [href]
+        
+        - Explicitly drops support for Python 3.0 - 3.4. Suitable supports the same
+          Python versions Ansible supports, which excludes these 3.x releases.
+        
+          Supported are therefore Python 2.7, 3.5 and 3.6+.
+          [href]
+        
         0.8.1 (2017-08-10)
         ~~~~~~~~~~~~~~~~~~~
         
         - Adds support for Ansible's extra_vars.
           [Liuyanglong]
         
         0.8.0 (2017-06-02)
@@ -152,7 +168,8 @@
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
```

### Comparing `suitable-0.8.1/LICENSE` & `suitable-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suitable-0.8.1/README.rst` & `suitable-0.9.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -44,14 +44,30 @@
 
 .. image:: https://badge.fury.io/py/suitable.svg
     :target: https://badge.fury.io/py/suitable
     :alt: Latest release
 
 Changelog
 ---------
+0.9.0 (2017-09-19)
+~~~~~~~~~~~~~~~~~~~
+
+- Adds support for Ansible 2.4. Since this release introduces many changes
+  under the hood support for Ansible 2.3 has been dropped!
+
+  You might want to assume that this will stay this way. Older Ansible
+  releases are supported if possible, but it's not a goal of this project.
+  [href]
+
+- Explicitly drops support for Python 3.0 - 3.4. Suitable supports the same
+  Python versions Ansible supports, which excludes these 3.x releases.
+
+  Supported are therefore Python 2.7, 3.5 and 3.6+.
+  [href]
+
 0.8.1 (2017-08-10)
 ~~~~~~~~~~~~~~~~~~~
 
 - Adds support for Ansible's extra_vars.
   [Liuyanglong]
 
 0.8.0 (2017-06-02)
```

