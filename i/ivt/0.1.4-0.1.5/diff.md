# Comparing `tmp/ivt-0.1.4.tar.gz` & `tmp/ivt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivt-0.1.4.tar", last modified: Mon Jul  3 17:52:28 2023, max compression
+gzip compressed data, was "ivt-0.1.5.tar", last modified: Thu Jul 13 21:30:09 2023, max compression
```

## Comparing `ivt-0.1.4.tar` & `ivt-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1123 2023-06-23 02:53:28.491095 ivt-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2174 2023-07-01 06:32:29.559569 ivt-0.1.4/.gitignore
--rw-r--r--   0        0        0     1091 2022-09-20 06:31:32.939829 ivt-0.1.4/LICENSE
--rw-r--r--   0        0        0      776 2023-06-23 02:53:28.491598 ivt-0.1.4/README.md
--rw-r--r--   0        0        0      661 2022-09-20 06:31:32.945331 ivt-0.1.4/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      493 2022-09-20 06:31:32.945832 ivt-0.1.4/docs/_templates/page.html
--rw-r--r--   0        0        0     1012 2022-09-20 06:31:32.946831 ivt-0.1.4/docs/conf.py
--rw-r--r--   0        0        0       58 2022-09-20 06:31:32.946831 ivt-0.1.4/docs/core_install.rst
--rw-r--r--   0        0        0       88 2022-09-20 06:31:32.947332 ivt-0.1.4/docs/core_intro.rst
--rw-r--r--   0        0        0       65 2022-09-20 06:31:32.947832 ivt-0.1.4/docs/forward_intro.rst
--rw-r--r--   0        0        0      605 2022-09-20 06:31:32.948332 ivt-0.1.4/docs/index.rst
--rw-r--r--   0        0        0       66 2022-09-20 06:31:32.948831 ivt-0.1.4/docs/inverse_intro.rst
--rw-r--r--   0        0        0       54 2022-09-20 06:31:32.949332 ivt-0.1.4/docs/plugin_refs.rst
--rw-r--r--   0        0        0       43 2022-09-20 06:31:32.949332 ivt-0.1.4/docs/requirements.txt
--rw-r--r--   0        0        0   268052 2022-09-20 06:31:32.950832 ivt-0.1.4/docs/teaser.png
--rw-r--r--   0        0        0      269 2023-07-03 17:50:22.568627 ivt-0.1.4/ivt/__init__.py
--rw-r--r--   0        0        0       83 2023-06-05 09:53:24.917312 ivt-0.1.4/ivt/config.py
--rw-r--r--   0        0        0      953 2023-06-05 09:53:24.917812 ivt-0.1.4/ivt/connector.py
--rw-r--r--   0        0        0       48 2023-06-05 09:53:24.918311 ivt-0.1.4/ivt/connectors/__init__.py
--rw-r--r--   0        0        0    14827 2023-07-03 02:09:02.909218 ivt-0.1.4/ivt/connectors/psdr_jit_connector.py
--rw-r--r--   0        0        0     3588 2023-07-03 02:06:06.590286 ivt-0.1.4/ivt/io.py
--rw-r--r--   0        0        0     2265 2023-03-07 09:19:51.701658 ivt-0.1.4/ivt/loss.py
--rw-r--r--   0        0        0     1554 2023-06-05 09:53:24.919812 ivt-0.1.4/ivt/model.py
--rw-r--r--   0        0        0     1908 2023-06-23 02:53:28.527105 ivt-0.1.4/ivt/parameter.py
--rw-r--r--   0        0        0     1925 2023-06-05 09:53:24.920815 ivt-0.1.4/ivt/renderer.py
--rw-r--r--   0        0        0     3217 2022-11-23 06:50:05.478582 ivt-0.1.4/ivt/sampling.py
--rw-r--r--   0        0        0     7093 2023-07-03 06:05:49.508316 ivt-0.1.4/ivt/scene.py
--rw-r--r--   0        0        0     3589 2023-07-01 06:32:29.564578 ivt-0.1.4/ivt/transform.py
--rw-r--r--   0        0        0      521 2023-07-03 00:44:02.988608 ivt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 ivt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-13 21:28:19.498054 ivt-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2030 2023-07-13 21:28:19.498054 ivt-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-13 21:28:19.498054 ivt-0.1.5/LICENSE
+-rw-r--r--   0        0        0      767 2023-07-13 21:28:19.498054 ivt-0.1.5/README.md
+-rw-r--r--   0        0        0      621 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      478 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/_templates/page.html
+-rw-r--r--   0        0        0      956 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0       54 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/core_install.rst
+-rw-r--r--   0        0        0       78 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/core_intro.rst
+-rw-r--r--   0        0        0       59 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/forward_intro.rst
+-rw-r--r--   0        0        0      571 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/index.rst
+-rw-r--r--   0        0        0       60 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/inverse_intro.rst
+-rw-r--r--   0        0        0       50 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/plugin_refs.rst
+-rw-r--r--   0        0        0       41 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/requirements.txt
+-rw-r--r--   0        0        0   268052 2023-07-13 21:28:19.498054 ivt-0.1.5/docs/teaser.png
+-rw-r--r--   0        0        0      258 2023-07-13 21:29:13.066935 ivt-0.1.5/ivt/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/config.py
+-rw-r--r--   0        0        0      916 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/connector.py
+-rw-r--r--   0        0        0       48 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/connectors/__init__.py
+-rw-r--r--   0        0        0    14436 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/connectors/psdr_jit_connector.py
+-rw-r--r--   0        0        0     3460 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/io.py
+-rw-r--r--   0        0        0     2213 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/loss.py
+-rw-r--r--   0        0        0     1530 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/model.py
+-rw-r--r--   0        0        0     1850 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/parameter.py
+-rw-r--r--   0        0        0     1874 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/renderer.py
+-rw-r--r--   0        0        0     3111 2023-07-13 21:28:19.526055 ivt-0.1.5/ivt/sampling.py
+-rw-r--r--   0        0        0     6924 2023-07-13 21:28:19.530055 ivt-0.1.5/ivt/scene.py
+-rw-r--r--   0        0        0     3450 2023-07-13 21:28:19.530055 ivt-0.1.5/ivt/transform.py
+-rw-r--r--   0        0        0      522 2023-07-13 21:28:20.006063 ivt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 ivt-0.1.5/PKG-INFO
```

### Comparing `ivt-0.1.4/.gitignore` & `ivt-0.1.5/.gitignore`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-# For project_template
-project_template/data
-project_template/results
-
-# Temp output in examples
-examples/**/*.png
-examples/**/*.exr
-examples/**/*.obj
-
-# Don't ignore files in examples/data
-!examples/data
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-result/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-pip-wheel-metadata/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-.python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# VSCode
+# For project_template
+project_template/data
+project_template/results
+
+# Temp output in examples
+examples/**/*.png
+examples/**/*.exr
+examples/**/*.obj
+
+# Don't ignore files in examples/data
+!examples/data
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+result/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+pip-wheel-metadata/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+.python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# VSCode
 .vscode
```

### Comparing `ivt-0.1.4/LICENSE` & `ivt-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 UCI Rendering
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 UCI Rendering
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ivt-0.1.4/README.md` & `ivt-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# ivt
-`ivt` stands for Inverse-Rendering Toolkit. It is a simple framework for conducting inverse rendering experiments. Since there are a lot differentiable renderers in development, mastering them all and migrating between them can be a headache. `ivt` provides a simple scene representation based on `pytorch` that can be rendered by **connectors** that connect to different differentiable renderers and get the graident of the scene parameters. Migrating between renderers is just a matter of changing the connector. 
-
-## Installation
-`ivt` depends on `pytorch`. Since it is widely used and some projects might have specific requirements to it, we leave its installation to the user. 
-
-After installing `pytorch`, you can install `ivt` via
-```
-pip install ivt
+# ivt
+`ivt` stands for Inverse-Rendering Toolkit. It is a simple framework for conducting inverse rendering experiments. Since there are a lot differentiable renderers in development, mastering them all and migrating between them can be a headache. `ivt` provides a simple scene representation based on `pytorch` that can be rendered by **connectors** that connect to different differentiable renderers and get the graident of the scene parameters. Migrating between renderers is just a matter of changing the connector. 
+
+## Installation
+`ivt` depends on `pytorch`. Since it is widely used and some projects might have specific requirements to it, we leave its installation to the user. 
+
+After installing `pytorch`, you can install `ivt` via
+```
+pip install ivt
 ```
```

### Comparing `ivt-0.1.4/docs/teaser.png` & `ivt-0.1.5/docs/teaser.png`

 * *Files identical despite different names*

### Comparing `ivt-0.1.4/ivt/connector.py` & `ivt-0.1.5/ivt/connector.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from abc import ABC, abstractmethod
-
-_connector_table = {}
-
-
-class Connector(ABC):
-
-    def __init_subclass__(cls, connector_name, **kwargs):
-        super().__init_subclass__(**kwargs)
-        _connector_table[connector_name] = cls
-        cls.extensions = {}
-
-    @abstractmethod
-    def renderC(self, scene, render_options, sensor_ids=[0], integrator_id=0):
-        pass
-
-    @abstractmethod
-    def renderD(self, image_grads, scene, render_options, sensor_ids=[0], integrator_id=0):
-        pass
-
-    @classmethod
-    def register(cls, class_name):
-        def wrapper(func):
-            cls.extensions[class_name] = func
-            return func
-        return wrapper
-
-def is_connector_available(connector_name):
-    return connector_name in _connector_table
-
-
-def get_connector_list():
-    return list(_connector_table.keys())
-
-
-def get_connector(connector_name):
-    return _connector_table[connector_name]()
+from abc import ABC, abstractmethod
+
+_connector_table = {}
+
+
+class Connector(ABC):
+
+    def __init_subclass__(cls, connector_name, **kwargs):
+        super().__init_subclass__(**kwargs)
+        _connector_table[connector_name] = cls
+        cls.extensions = {}
+
+    @abstractmethod
+    def renderC(self, scene, render_options, sensor_ids=[0], integrator_id=0):
+        pass
+
+    @abstractmethod
+    def renderD(self, image_grads, scene, render_options, sensor_ids=[0], integrator_id=0):
+        pass
+
+    @classmethod
+    def register(cls, class_name):
+        def wrapper(func):
+            cls.extensions[class_name] = func
+            return func
+        return wrapper
+
+def is_connector_available(connector_name):
+    return connector_name in _connector_table
+
+
+def get_connector_list():
+    return list(_connector_table.keys())
+
+
+def get_connector(connector_name):
+    return _connector_table[connector_name]()
```

### Comparing `ivt-0.1.4/ivt/connectors/psdr_jit_connector.py` & `ivt-0.1.5/ivt/connectors/psdr_jit_connector.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,392 +1,392 @@
-from ..connector import Connector
-from ..scene import *
-from ..config import *
-from ..io import write_mesh
-from collections import OrderedDict
-
-import drjit
-import psdr_jit
-from drjit.scalar import Array3f
-from drjit.cuda import Array3f as Vector3fC, Array3i as Vector3iC
-from drjit.cuda.ad import Array3f as Vector3fD, Float32 as FloatD, Matrix4f as Matrix4fD, Matrix3f as Matrix3fD
-from drjit.cuda.ad import Float32 as FloatD
-import torch
-
-import time
-import os
-
-class Timer:
-    def __init__(self, label):
-        self.label = label
-
-    def __enter__(self):
-        self.start_time = time.time()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        elapsed_time = time.time() - self.start_time
-        print(f"[{self.label}] Elapsed time: {elapsed_time} seconds")
-
-class PSDRJITConnector(Connector, connector_name='psdr_jit'):
-
-    backend = 'torch'
-    device = 'cuda'
-    ftype = torch.float32
-    itype = torch.long
-
-    def __init__(self):
-        super().__init__()
-
-    def update_scene_objects(self, scene, render_options):
-        if 'psdr_jit' in scene.cached:
-            cache = scene.cached['psdr_jit']
-        else:
-            cache = {}
-            scene.cached['psdr_jit'] = cache
-
-            cache['scene'] = psdr_jit.Scene()
-            cache['scene'].opts.spp = render_options['spp']
-            cache['scene'].opts.sppe = render_options['sppe']
-            cache['scene'].opts.sppse = render_options['sppse']
-            cache['scene'].opts.log_level = render_options['log_level']
-
-            cache['name_map'] = {}
-            cache['integrators'] = OrderedDict()
-            cache['configured'] = False
-
-        drjit_params = []
-        for name in scene.components:
-            component = scene[name]
-            drjit_params += self.extensions[type(component)](name, scene)
-
-        if not cache['configured']:
-            cache['scene'].configure() 
-            cache['configured'] = True
-        
-        return scene.cached['psdr_jit'], drjit_params
-
-    def renderC(self, scene, render_options, sensor_ids=[0], integrator_id=0):
-        cache, _ = self.update_scene_objects(scene, render_options)
-
-        cache['scene'].configure(sensor_ids)
-
-        npass = render_options['npass']
-        h, w, c = cache['film']['shape']
-        if type(integrator_id) == int:
-            integrator = list(cache['integrators'].values())[integrator_id]
-        elif type(integrator_id) == str:
-            integrator = cache['integrators'][integrator_id]
-        else:
-            raise RuntimeError('integrator_id is invalid: {integrator_id}')
-
-        images = []
-        for sensor_id in sensor_ids:
-            image = torch.zeros((h * w, c)).to(device).to(ftype)
-            for i in range(npass):
-                image_pass = integrator.renderC(cache['scene'], sensor_id).torch()
-                image += image_pass / npass
-            image = image.reshape(h, w, c)
-            images.append(image)
-
-        return images
-        
-    def renderD(self, image_grads, scene, render_options, sensor_ids=[0], integrator_id=0):
-        cache, drjit_params = self.update_scene_objects(scene, render_options)
-
-        cache['scene'].configure(sensor_ids)
-
-        npass = render_options['npass']
-        h, w, c = cache['film']['shape']
-        if type(integrator_id) == int:
-            integrator = list(cache['integrators'].values())[integrator_id]
-        elif type(integrator_id) == str:
-            integrator = cache['integrators'][integrator_id]
-        else:
-            raise RuntimeError('integrator_id is invalid: {integrator_id}')
-        
-        param_grads = [torch.zeros_like(scene[param_name]) for param_name in scene.requiring_grad]
-
-        for i, sensor_id in enumerate(sensor_ids):
-            image_grad = Vector3fC(image_grads[i].reshape(-1, 3) / npass)
-            for j in range(npass):
-                image = integrator.renderD(cache['scene'], sensor_id)
-                tmp = drjit.dot(image_grad, image)
-                drjit.backward(tmp)
-
-                for param_grad, drjit_param in zip(param_grads, drjit_params):
-                    grad = drjit.grad(drjit_param).torch().to(device).to(ftype)
-                    grad = torch.nan_to_num(grad).reshape(param_grad.shape)
-                    param_grad += grad
-
-        return param_grads
-
-@PSDRJITConnector.register(Integrator)
-def process_integrator(name, scene):
-    integrator = scene[name]
-    cache = scene.cached['psdr_jit']
-
-    if integrator['type'] == 'field':
-        psdr_integrator = psdr_jit.FieldExtractionIntegrator(integrator['config']['type'])
-        cache['integrators'][name] = psdr_integrator
-    elif integrator['type'] == 'collocated':
-        psdr_integrator = psdr_jit.CollocatedIntegrator(integrator['config']['intensity'])
-        cache['integrators'][name] = psdr_integrator
-    elif integrator['type'] == 'path':
-        psdr_integrator = psdr_jit.PathTracer(integrator['config']['max_depth'])
-        cache['integrators'][name] = psdr_integrator
-        if 'hide_emitters' in integrator['config']:
-            psdr_integrator.hide_emitters = integrator['config']['hide_emitters']
-    else:
-        raise RuntimeError(f"unrecognized integrator type: {integrator['type']}")
-
-    return []
-
-@PSDRJITConnector.register(HDRFilm)
-def process_hdr_film(name, scene):
-    film = scene[name]
-    cache = scene.cached['psdr_jit']
-
-    cache['film'] = {
-        'shape': (film['height'], film['width'], 3)
-    }
-    cache['scene'].opts.width = film['width']
-    cache['scene'].opts.height = film['height']
-
-    return []
-
-@PSDRJITConnector.register(PerspectiveCamera)
-def process_perspective_camera(name, scene):
-    sensor = scene[name]
-    cache = scene.cached['psdr_jit']
-    psdr_scene = cache['scene']
-
-    # Create the object if it has not been created
-    if name not in cache['name_map']:
-        psdr_sensor = psdr_jit.PerspectiveCamera(sensor['fov'], sensor['near'], sensor['far'])
-        psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
-        psdr_scene.add_Sensor(psdr_sensor)
-        cache['name_map'][name] = f"Sensor[{psdr_scene.num_sensors - 1}]"
-
-    psdr_sensor = psdr_scene.param_map[cache['name_map'][name]]
-    
-    # Update parameters
-    updated = sensor.get_updated()
-    if len(updated) > 0:
-        for param_name in updated:
-            if param_name == "to_world":
-                psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
-            sensor.params[param_name]['updated'] = False
-
-    # Enable grad for parameters requiring grad
-    drjit_params = []
-    requiring_grad = sensor.get_requiring_grad()
-    if len(requiring_grad) > 0:
-        for param_name in requiring_grad:
-            if param_name == "to_world":
-                drjit_param = psdr_sensor.to_world
-                drjit.enable_grad(drjit_param)
-                drjit_params.append(drjit_param)
-
-    return drjit_params
-
-@PSDRJITConnector.register(Mesh)
-def process_mesh(name, scene):
-    mesh = scene[name]
-    cache = scene.cached['psdr_jit']
-    psdr_scene = cache['scene']
-
-    # Create the object if it has not been created
-    if name not in cache['name_map']:
-        # Create its material first
-        mat_id = mesh['mat_id']
-        if mat_id not in scene:
-            raise RuntimeError(f"The material of the mesh {name} doesn't exist: mat_id={mat_id}")
-        brdf = scene[mat_id]
-        PSDRJITConnector.extensions[type(brdf)](mat_id, scene)
-
-        # TODO: Fix this workaround when psdr-jit updates psdr_mesh.load_raw()
-        if mesh['can_change_topology']:
-            psdr_mesh = psdr_jit.Mesh()
-            psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
-            psdr_mesh.use_face_normal = mesh['use_face_normal']
-
-            psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
-            psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
-        else:
-            write_mesh('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
-            psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
-            psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
-            os.remove('__psdr_jit_tmp__.obj')
-        
-        cache['name_map'][name] = f"Mesh[{psdr_scene.num_meshes - 1}]"
-
-    psdr_mesh = psdr_scene.param_map[cache['name_map'][name]]
-
-    # Update parameters
-    updated = mesh.get_updated()
-    if len(updated) > 0:
-        for param_name in updated:
-            if param_name == 'v':
-                if mesh['can_change_topology']:
-                    psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
-                else:
-                    psdr_mesh.vertex_positions = Vector3fC(mesh['v'])
-                    psdr_mesh.face_indices = Vector3iC(mesh['f'])
-
-            mesh.params[param_name]['updated'] = False
-
-    # Enable grad for parameters requiring grad
-    drjit_params = []
-    requiring_grad = mesh.get_requiring_grad()
-    if len(requiring_grad) > 0:
-        for param_name in requiring_grad:
-            if param_name == 'v':
-                drjit_param = psdr_mesh.vertex_positions
-                drjit.enable_grad(drjit_param)
-                drjit_params.append(drjit_param)
-
-    return drjit_params
-
-def convert_color(color, c, bitmap=True):
-    if color.shape == ():
-        color = color.tile(c)
-    if color.shape == (c,):
-        color = color.reshape(1, 1, c)
-    h, w, _ = color.shape
-    if c == 3:
-        color = Vector3fD(color.reshape(-1, c))
-        if bitmap:
-            color = psdr_jit.Bitmap3fD(w, h, color)
-    elif c == 1:
-        color = FloatD(color.reshape(-1))
-        if bitmap:
-            color = psdr_jit.Bitmap1fD(w, h, color)
-    else:
-        raise RuntimeError("Not support bitmap channel number: {c}")
-    return color
-
-@PSDRJITConnector.register(DiffuseBRDF)
-def process_diffuse_brdf(name, scene):
-    brdf = scene[name]
-    cache = scene.cached['psdr_jit']
-    psdr_scene = cache['scene']
-    
-    # Create the object if it has not been created
-    if name not in cache['name_map']:
-        d = convert_color(brdf['d'], 3)
-        psdr_bsdf = psdr_jit.DiffuseBSDF(d)
-        psdr_scene.add_BSDF(psdr_bsdf, name)
-        cache['name_map'][name] = f"BSDF[id={name}]"
-
-    psdr_brdf = psdr_scene.param_map[cache['name_map'][name]]
-
-    # Update parameters
-    updated = brdf.get_updated()
-    if len(updated) > 0:
-        for param_name in updated:
-            if param_name == 'd':
-                psdr_brdf.reflectance = convert_color(brdf['d'], 3)
-            brdf.params[param_name]['updated'] = False
-
-    # Enable grad for parameters requiring grad
-    drjit_params = []
-    requiring_grad = brdf.get_requiring_grad()
-    if len(requiring_grad) > 0:
-        for param_name in requiring_grad:
-            if param_name == 'd':
-                drjit_param = psdr_brdf.reflectance.data
-                drjit.enable_grad(drjit_param)
-                drjit_params.append(drjit_param)
-
-    return drjit_params
-
-@PSDRJITConnector.register(MicrofacetBRDF)
-def process_microfacet_brdf(name, scene):
-    brdf = scene[name]
-    cache = scene.cached['psdr_jit']
-    psdr_scene = cache['scene']
-    
-    # Create the object if it has not been created
-    if name not in cache['name_map']:
-        d = convert_color(brdf['d'], 3)
-        s = convert_color(brdf['s'], 3)
-        r = convert_color(brdf['r'], 1)
-
-        psdr_bsdf = psdr_jit.MicrofacetBSDF(s, d, r)
-        psdr_scene.add_BSDF(psdr_bsdf, name)
-        cache['name_map'][name] = f"BSDF[id={name}]"
-
-    psdr_brdf = psdr_scene.param_map[cache['name_map'][name]]
-
-    # Update parameters
-    updated = brdf.get_updated()
-    if len(updated) > 0:
-        for param_name in updated:
-            if param_name == 'd':
-                psdr_brdf.diffuseReflectance.data = convert_color(brdf['d'], 3, bitmap=False)
-            elif param_name == 's':
-                psdr_brdf.specularReflectance.data = convert_color(brdf['s'], 3, bitmap=False)
-            elif param_name == 'r':
-                psdr_brdf.roughness.data = convert_color(brdf['r'], 1, bitmap=False)
-            brdf.params[param_name]['updated'] = False
-
-    # Enable grad for parameters requiring grad
-    drjit_params = []
-    
-    def enable_grad(drjit_param):
-        drjit.enable_grad(drjit_param)
-        drjit_params.append(drjit_param)
-
-    requiring_grad = brdf.get_requiring_grad()
-    if len(requiring_grad) > 0:
-        for param_name in requiring_grad:
-            if param_name == 'd':
-                enable_grad(psdr_brdf.diffuseReflectance.data)
-            elif param_name == 's':
-                enable_grad(psdr_brdf.specularReflectance.data)
-            elif param_name == 'r':
-                enable_grad(psdr_brdf.roughness.data)
-
-    return drjit_params
-
-@PSDRJITConnector.register(EnvironmentLight)
-def process_environment_light(name, scene):
-    emitter = scene[name]
-    cache = scene.cached['psdr_jit']
-    psdr_scene = cache['scene']
-    
-    # Create the object if it has not been created
-    if name not in cache['name_map']:
-        radiance = convert_color(emitter['radiance'], 3)
-
-        psdr_emitter = psdr_jit.EnvironmentMap()
-        psdr_emitter.radiance = radiance
-        psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
-        psdr_scene.add_EnvironmentMap(psdr_emitter)
-        cache['name_map'][name] = f"Emitter[{psdr_scene.get_num_emitters() - 1}]"
-
-    psdr_emitter = psdr_scene.param_map[cache['name_map'][name]]
-
-    # Update parameters
-    updated = emitter.get_updated()
-    if len(updated) > 0:
-        for param_name in updated:
-            if param_name == 'radiance':
-                psdr_emitter.radiance = convert_color(emitter['radiance'], 3)
-            elif param_name == 'to_world':
-                psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
-            emitter.params[param_name]['updated'] = False
-
-    # Enable grad for parameters requiring grad
-    drjit_params = []
-    
-    def enable_grad(drjit_param):
-        drjit.enable_grad(drjit_param)
-        drjit_params.append(drjit_param)
-
-    requiring_grad = emitter.get_requiring_grad()
-    if len(requiring_grad) > 0:
-        for param_name in requiring_grad:
-            if param_name == 'radiance':
-                enable_grad(psdr_emitter.radiance.data)
-                
+from ..connector import Connector
+from ..scene import *
+from ..config import *
+from ..io import write_mesh
+from collections import OrderedDict
+
+import drjit
+import psdr_jit
+from drjit.scalar import Array3f
+from drjit.cuda import Array3f as Vector3fC, Array3i as Vector3iC
+from drjit.cuda.ad import Array3f as Vector3fD, Float32 as FloatD, Matrix4f as Matrix4fD, Matrix3f as Matrix3fD
+from drjit.cuda.ad import Float32 as FloatD
+import torch
+
+import time
+import os
+
+class Timer:
+    def __init__(self, label):
+        self.label = label
+
+    def __enter__(self):
+        self.start_time = time.time()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        elapsed_time = time.time() - self.start_time
+        print(f"[{self.label}] Elapsed time: {elapsed_time} seconds")
+
+class PSDRJITConnector(Connector, connector_name='psdr_jit'):
+
+    backend = 'torch'
+    device = 'cuda'
+    ftype = torch.float32
+    itype = torch.long
+
+    def __init__(self):
+        super().__init__()
+
+    def update_scene_objects(self, scene, render_options):
+        if 'psdr_jit' in scene.cached:
+            cache = scene.cached['psdr_jit']
+        else:
+            cache = {}
+            scene.cached['psdr_jit'] = cache
+
+            cache['scene'] = psdr_jit.Scene()
+            cache['scene'].opts.spp = render_options['spp']
+            cache['scene'].opts.sppe = render_options['sppe']
+            cache['scene'].opts.sppse = render_options['sppse']
+            cache['scene'].opts.log_level = render_options['log_level']
+
+            cache['name_map'] = {}
+            cache['integrators'] = OrderedDict()
+            cache['configured'] = False
+
+        drjit_params = []
+        for name in scene.components:
+            component = scene[name]
+            drjit_params += self.extensions[type(component)](name, scene)
+
+        if not cache['configured']:
+            cache['scene'].configure() 
+            cache['configured'] = True
+        
+        return scene.cached['psdr_jit'], drjit_params
+
+    def renderC(self, scene, render_options, sensor_ids=[0], integrator_id=0):
+        cache, _ = self.update_scene_objects(scene, render_options)
+
+        cache['scene'].configure(sensor_ids)
+
+        npass = render_options['npass']
+        h, w, c = cache['film']['shape']
+        if type(integrator_id) == int:
+            integrator = list(cache['integrators'].values())[integrator_id]
+        elif type(integrator_id) == str:
+            integrator = cache['integrators'][integrator_id]
+        else:
+            raise RuntimeError('integrator_id is invalid: {integrator_id}')
+
+        images = []
+        for sensor_id in sensor_ids:
+            image = torch.zeros((h * w, c)).to(device).to(ftype)
+            for i in range(npass):
+                image_pass = integrator.renderC(cache['scene'], sensor_id).torch()
+                image += image_pass / npass
+            image = image.reshape(h, w, c)
+            images.append(image)
+
+        return images
+        
+    def renderD(self, image_grads, scene, render_options, sensor_ids=[0], integrator_id=0):
+        cache, drjit_params = self.update_scene_objects(scene, render_options)
+
+        cache['scene'].configure(sensor_ids)
+
+        npass = render_options['npass']
+        h, w, c = cache['film']['shape']
+        if type(integrator_id) == int:
+            integrator = list(cache['integrators'].values())[integrator_id]
+        elif type(integrator_id) == str:
+            integrator = cache['integrators'][integrator_id]
+        else:
+            raise RuntimeError('integrator_id is invalid: {integrator_id}')
+        
+        param_grads = [torch.zeros_like(scene[param_name]) for param_name in scene.requiring_grad]
+
+        for i, sensor_id in enumerate(sensor_ids):
+            image_grad = Vector3fC(image_grads[i].reshape(-1, 3) / npass)
+            for j in range(npass):
+                image = integrator.renderD(cache['scene'], sensor_id)
+                tmp = drjit.dot(image_grad, image)
+                drjit.backward(tmp)
+
+                for param_grad, drjit_param in zip(param_grads, drjit_params):
+                    grad = drjit.grad(drjit_param).torch().to(device).to(ftype)
+                    grad = torch.nan_to_num(grad).reshape(param_grad.shape)
+                    param_grad += grad
+
+        return param_grads
+
+@PSDRJITConnector.register(Integrator)
+def process_integrator(name, scene):
+    integrator = scene[name]
+    cache = scene.cached['psdr_jit']
+
+    if integrator['type'] == 'field':
+        psdr_integrator = psdr_jit.FieldExtractionIntegrator(integrator['config']['type'])
+        cache['integrators'][name] = psdr_integrator
+    elif integrator['type'] == 'collocated':
+        psdr_integrator = psdr_jit.CollocatedIntegrator(integrator['config']['intensity'])
+        cache['integrators'][name] = psdr_integrator
+    elif integrator['type'] == 'path':
+        psdr_integrator = psdr_jit.PathTracer(integrator['config']['max_depth'])
+        cache['integrators'][name] = psdr_integrator
+        if 'hide_emitters' in integrator['config']:
+            psdr_integrator.hide_emitters = integrator['config']['hide_emitters']
+    else:
+        raise RuntimeError(f"unrecognized integrator type: {integrator['type']}")
+
+    return []
+
+@PSDRJITConnector.register(HDRFilm)
+def process_hdr_film(name, scene):
+    film = scene[name]
+    cache = scene.cached['psdr_jit']
+
+    cache['film'] = {
+        'shape': (film['height'], film['width'], 3)
+    }
+    cache['scene'].opts.width = film['width']
+    cache['scene'].opts.height = film['height']
+
+    return []
+
+@PSDRJITConnector.register(PerspectiveCamera)
+def process_perspective_camera(name, scene):
+    sensor = scene[name]
+    cache = scene.cached['psdr_jit']
+    psdr_scene = cache['scene']
+
+    # Create the object if it has not been created
+    if name not in cache['name_map']:
+        psdr_sensor = psdr_jit.PerspectiveCamera(sensor['fov'], sensor['near'], sensor['far'])
+        psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
+        psdr_scene.add_Sensor(psdr_sensor)
+        cache['name_map'][name] = f"Sensor[{psdr_scene.num_sensors - 1}]"
+
+    psdr_sensor = psdr_scene.param_map[cache['name_map'][name]]
+    
+    # Update parameters
+    updated = sensor.get_updated()
+    if len(updated) > 0:
+        for param_name in updated:
+            if param_name == "to_world":
+                psdr_sensor.to_world = Matrix4fD(sensor['to_world'].reshape(1, 4, 4))
+            sensor.params[param_name]['updated'] = False
+
+    # Enable grad for parameters requiring grad
+    drjit_params = []
+    requiring_grad = sensor.get_requiring_grad()
+    if len(requiring_grad) > 0:
+        for param_name in requiring_grad:
+            if param_name == "to_world":
+                drjit_param = psdr_sensor.to_world
+                drjit.enable_grad(drjit_param)
+                drjit_params.append(drjit_param)
+
+    return drjit_params
+
+@PSDRJITConnector.register(Mesh)
+def process_mesh(name, scene):
+    mesh = scene[name]
+    cache = scene.cached['psdr_jit']
+    psdr_scene = cache['scene']
+
+    # Create the object if it has not been created
+    if name not in cache['name_map']:
+        # Create its material first
+        mat_id = mesh['mat_id']
+        if mat_id not in scene:
+            raise RuntimeError(f"The material of the mesh {name} doesn't exist: mat_id={mat_id}")
+        brdf = scene[mat_id]
+        PSDRJITConnector.extensions[type(brdf)](mat_id, scene)
+
+        # TODO: Fix this workaround when psdr-jit updates psdr_mesh.load_raw()
+        if mesh['can_change_topology']:
+            psdr_mesh = psdr_jit.Mesh()
+            psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
+            psdr_mesh.use_face_normal = mesh['use_face_normal']
+
+            psdr_emitter = psdr_jit.AreaLight(mesh['radiance'].tolist()) if mesh['is_emitter'] else None
+            psdr_scene.add_Mesh(psdr_mesh, mat_id, psdr_emitter)
+        else:
+            write_mesh('__psdr_jit_tmp__.obj', mesh['v'], mesh['f'], mesh['uv'], mesh['fuv'])
+            psdr_emitter = psdr_jit.AreaLight(mesh['radiance']) if mesh['is_emitter'] else None
+            psdr_scene.add_Mesh('__psdr_jit_tmp__.obj', mesh['to_world'].reshape(1, 4, 4), mat_id, psdr_emitter)
+            os.remove('__psdr_jit_tmp__.obj')
+        
+        cache['name_map'][name] = f"Mesh[{psdr_scene.num_meshes - 1}]"
+
+    psdr_mesh = psdr_scene.param_map[cache['name_map'][name]]
+
+    # Update parameters
+    updated = mesh.get_updated()
+    if len(updated) > 0:
+        for param_name in updated:
+            if param_name == 'v':
+                if mesh['can_change_topology']:
+                    psdr_mesh.load_raw(Vector3fC(mesh['v']), Vector3iC(mesh['f']))
+                else:
+                    psdr_mesh.vertex_positions = Vector3fC(mesh['v'])
+                    psdr_mesh.face_indices = Vector3iC(mesh['f'])
+
+            mesh.params[param_name]['updated'] = False
+
+    # Enable grad for parameters requiring grad
+    drjit_params = []
+    requiring_grad = mesh.get_requiring_grad()
+    if len(requiring_grad) > 0:
+        for param_name in requiring_grad:
+            if param_name == 'v':
+                drjit_param = psdr_mesh.vertex_positions
+                drjit.enable_grad(drjit_param)
+                drjit_params.append(drjit_param)
+
+    return drjit_params
+
+def convert_color(color, c, bitmap=True):
+    if color.shape == ():
+        color = color.tile(c)
+    if color.shape == (c,):
+        color = color.reshape(1, 1, c)
+    h, w, _ = color.shape
+    if c == 3:
+        color = Vector3fD(color.reshape(-1, c))
+        if bitmap:
+            color = psdr_jit.Bitmap3fD(w, h, color)
+    elif c == 1:
+        color = FloatD(color.reshape(-1))
+        if bitmap:
+            color = psdr_jit.Bitmap1fD(w, h, color)
+    else:
+        raise RuntimeError("Not support bitmap channel number: {c}")
+    return color
+
+@PSDRJITConnector.register(DiffuseBRDF)
+def process_diffuse_brdf(name, scene):
+    brdf = scene[name]
+    cache = scene.cached['psdr_jit']
+    psdr_scene = cache['scene']
+    
+    # Create the object if it has not been created
+    if name not in cache['name_map']:
+        d = convert_color(brdf['d'], 3)
+        psdr_bsdf = psdr_jit.DiffuseBSDF(d)
+        psdr_scene.add_BSDF(psdr_bsdf, name)
+        cache['name_map'][name] = f"BSDF[id={name}]"
+
+    psdr_brdf = psdr_scene.param_map[cache['name_map'][name]]
+
+    # Update parameters
+    updated = brdf.get_updated()
+    if len(updated) > 0:
+        for param_name in updated:
+            if param_name == 'd':
+                psdr_brdf.reflectance = convert_color(brdf['d'], 3)
+            brdf.params[param_name]['updated'] = False
+
+    # Enable grad for parameters requiring grad
+    drjit_params = []
+    requiring_grad = brdf.get_requiring_grad()
+    if len(requiring_grad) > 0:
+        for param_name in requiring_grad:
+            if param_name == 'd':
+                drjit_param = psdr_brdf.reflectance.data
+                drjit.enable_grad(drjit_param)
+                drjit_params.append(drjit_param)
+
+    return drjit_params
+
+@PSDRJITConnector.register(MicrofacetBRDF)
+def process_microfacet_brdf(name, scene):
+    brdf = scene[name]
+    cache = scene.cached['psdr_jit']
+    psdr_scene = cache['scene']
+    
+    # Create the object if it has not been created
+    if name not in cache['name_map']:
+        d = convert_color(brdf['d'], 3)
+        s = convert_color(brdf['s'], 3)
+        r = convert_color(brdf['r'], 1)
+
+        psdr_bsdf = psdr_jit.MicrofacetBSDF(s, d, r)
+        psdr_scene.add_BSDF(psdr_bsdf, name)
+        cache['name_map'][name] = f"BSDF[id={name}]"
+
+    psdr_brdf = psdr_scene.param_map[cache['name_map'][name]]
+
+    # Update parameters
+    updated = brdf.get_updated()
+    if len(updated) > 0:
+        for param_name in updated:
+            if param_name == 'd':
+                psdr_brdf.diffuseReflectance.data = convert_color(brdf['d'], 3, bitmap=False)
+            elif param_name == 's':
+                psdr_brdf.specularReflectance.data = convert_color(brdf['s'], 3, bitmap=False)
+            elif param_name == 'r':
+                psdr_brdf.roughness.data = convert_color(brdf['r'], 1, bitmap=False)
+            brdf.params[param_name]['updated'] = False
+
+    # Enable grad for parameters requiring grad
+    drjit_params = []
+    
+    def enable_grad(drjit_param):
+        drjit.enable_grad(drjit_param)
+        drjit_params.append(drjit_param)
+
+    requiring_grad = brdf.get_requiring_grad()
+    if len(requiring_grad) > 0:
+        for param_name in requiring_grad:
+            if param_name == 'd':
+                enable_grad(psdr_brdf.diffuseReflectance.data)
+            elif param_name == 's':
+                enable_grad(psdr_brdf.specularReflectance.data)
+            elif param_name == 'r':
+                enable_grad(psdr_brdf.roughness.data)
+
+    return drjit_params
+
+@PSDRJITConnector.register(EnvironmentLight)
+def process_environment_light(name, scene):
+    emitter = scene[name]
+    cache = scene.cached['psdr_jit']
+    psdr_scene = cache['scene']
+    
+    # Create the object if it has not been created
+    if name not in cache['name_map']:
+        radiance = convert_color(emitter['radiance'], 3)
+
+        psdr_emitter = psdr_jit.EnvironmentMap()
+        psdr_emitter.radiance = radiance
+        psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
+        psdr_scene.add_EnvironmentMap(psdr_emitter)
+        cache['name_map'][name] = f"Emitter[{psdr_scene.get_num_emitters() - 1}]"
+
+    psdr_emitter = psdr_scene.param_map[cache['name_map'][name]]
+
+    # Update parameters
+    updated = emitter.get_updated()
+    if len(updated) > 0:
+        for param_name in updated:
+            if param_name == 'radiance':
+                psdr_emitter.radiance = convert_color(emitter['radiance'], 3)
+            elif param_name == 'to_world':
+                psdr_emitter.set_transform(Matrix4fD(emitter['to_world'].reshape(1, 4, 4)))
+            emitter.params[param_name]['updated'] = False
+
+    # Enable grad for parameters requiring grad
+    drjit_params = []
+    
+    def enable_grad(drjit_param):
+        drjit.enable_grad(drjit_param)
+        drjit_params.append(drjit_param)
+
+    requiring_grad = emitter.get_requiring_grad()
+    if len(requiring_grad) > 0:
+        for param_name in requiring_grad:
+            if param_name == 'radiance':
+                enable_grad(psdr_emitter.radiance.data)
+                
     return drjit_params
```

### Comparing `ivt-0.1.4/ivt/io.py` & `ivt-0.1.5/ivt/io.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from .config import *
-import imageio.v3 as iio
-import numpy as np
-import torch
-from pathlib import Path
-import gpytoolbox
-
-def read_mesh(mesh_path):
-    v, f, uv, fuv = gpytoolbox.read_mesh(mesh_path, return_UV=True)
-    if uv.size == 0:
-        uv = np.zeros((0, 2))
-        fuv = np.zeros((0, 3))
-    return v, f, uv, fuv
-
-def write_mesh(mesh_path, v, f, uv=None, fuv=None):
-    v = to_numpy(v)
-    f = to_numpy(f)
-    if uv is not None: 
-        if uv.size == 0:
-            uv = None
-        else:
-            uv = to_numpy(uv)
-    if fuv is not None: 
-        if fuv.size == 0:
-            fuv = None
-        else:
-            fuv = to_numpy(fuv)
-    gpytoolbox.write_mesh(str(mesh_path), v, f, uv, fuv)
-
-def linear_to_srgb(l):
-    s = np.zeros_like(l)
-    m = l <= 0.00313066844250063
-    s[m] = l[m] * 12.92
-    s[~m] = 1.055*(l[~m]**(1.0/2.4))-0.055
-    return s
-
-def srgb_to_linear(s):
-    l = np.zeros_like(s)
-    m = s <= 0.0404482362771082
-    l[m] = s[m] / 12.92
-    l[~m] = ((s[~m]+0.055)/1.055) ** 2.4
-    return l
-
-def to_srgb(image):
-    image = to_numpy(image)
-    if image.shape[2] == 4:
-        image_alpha = image[:, :, 3:4]
-        image = linear_to_srgb(image[:, :, 0:3])
-        image = np.concatenate([image, image_alpha], axis=2)
-    else:
-        image = linear_to_srgb(image)
-    return np.clip(image, 0, 1)
-
-def to_linear(image):
-    image = to_numpy(image)
-    if image.shape[2] == 4:
-        image_alpha = image[:, :, 3:4]
-        image = srgb_to_linear(image[:, :, 0:3])
-        image = np.concatenate([image, image_alpha], axis=2)
-    else:
-        image = srgb_to_linear(image)
-    return image
-
-def to_numpy(data):
-    if torch.is_tensor(data):
-        return data.detach().cpu().numpy()
-    else:
-        return np.array(data)
-    
-def to_torch(data, dtype):
-    if torch.is_tensor(data):
-        return data.to(dtype).to(device).contiguous()
-    elif isinstance(data, np.ndarray):
-        return torch.from_numpy(data).to(dtype).to(device).contiguous()
-    else:
-        return torch.tensor(data, dtype=dtype, device=device).contiguous()
-
-def to_torch_f(data):
-    return to_torch(data, ftype)
-
-def to_torch_i(data):
-    return to_torch(data, itype)
-
-def read_image(image_path, is_srgb=None, remove_alpha=True):
-    image_path = Path(image_path)
-    image = iio.imread(image_path)
-    image = np.atleast_3d(image)
-    if remove_alpha and image.shape[2] == 4:
-        image = image[:, :, 0:3]
-
-    if image.dtype == np.uint8 or image.dtype == np.int16:
-        image = image.astype("float32") / 255.0
-    elif image.dtype == np.uint16 or image.dtype == np.int32:
-        image = image.astype("float32") / 65535.0
-
-    if is_srgb is None:
-        if image_path.suffix in ['.exr', '.hdr', '.rgbe']:
-            is_srgb = False
-        else:
-            is_srgb = True
-
-    if is_srgb:
-        image = to_linear(image)
-
-    return image
-
-def write_image(image_path, image, is_srgb=None):
-    image_path = Path(image_path)
-    image = to_numpy(image)
-    image = np.atleast_3d(image)
-    if image.shape[2] == 1:
-        image = np.repeat(image, 3, axis=2)
-
-    if is_srgb is None:
-        if image_path.suffix in ['.exr', '.hdr', '.rgbe']:
-            is_srgb = False
-        else:
-            is_srgb = True
-
-    if is_srgb:
-        image = to_srgb(image)
-
-    if image_path.suffix == '.exr':
-        image = image.astype(np.float32)
-    else:
-        image = (image * 255).astype(np.uint8)
-
-    iio.imwrite(image_path, image)
+from .config import *
+import imageio.v3 as iio
+import numpy as np
+import torch
+from pathlib import Path
+import gpytoolbox
+
+def read_mesh(mesh_path):
+    v, f, uv, fuv = gpytoolbox.read_mesh(mesh_path, return_UV=True)
+    if uv.size == 0:
+        uv = np.zeros((0, 2))
+        fuv = np.zeros((0, 3))
+    return v, f, uv, fuv
+
+def write_mesh(mesh_path, v, f, uv=None, fuv=None):
+    v = to_numpy(v)
+    f = to_numpy(f)
+    if uv is not None: 
+        if uv.size == 0:
+            uv = None
+        else:
+            uv = to_numpy(uv)
+    if fuv is not None: 
+        if fuv.size == 0:
+            fuv = None
+        else:
+            fuv = to_numpy(fuv)
+    gpytoolbox.write_mesh(str(mesh_path), v, f, uv, fuv)
+
+def linear_to_srgb(l):
+    s = np.zeros_like(l)
+    m = l <= 0.00313066844250063
+    s[m] = l[m] * 12.92
+    s[~m] = 1.055*(l[~m]**(1.0/2.4))-0.055
+    return s
+
+def srgb_to_linear(s):
+    l = np.zeros_like(s)
+    m = s <= 0.0404482362771082
+    l[m] = s[m] / 12.92
+    l[~m] = ((s[~m]+0.055)/1.055) ** 2.4
+    return l
+
+def to_srgb(image):
+    image = to_numpy(image)
+    if image.shape[2] == 4:
+        image_alpha = image[:, :, 3:4]
+        image = linear_to_srgb(image[:, :, 0:3])
+        image = np.concatenate([image, image_alpha], axis=2)
+    else:
+        image = linear_to_srgb(image)
+    return np.clip(image, 0, 1)
+
+def to_linear(image):
+    image = to_numpy(image)
+    if image.shape[2] == 4:
+        image_alpha = image[:, :, 3:4]
+        image = srgb_to_linear(image[:, :, 0:3])
+        image = np.concatenate([image, image_alpha], axis=2)
+    else:
+        image = srgb_to_linear(image)
+    return image
+
+def to_numpy(data):
+    if torch.is_tensor(data):
+        return data.detach().cpu().numpy()
+    else:
+        return np.array(data)
+    
+def to_torch(data, dtype):
+    if torch.is_tensor(data):
+        return data.to(dtype).to(device).contiguous()
+    elif isinstance(data, np.ndarray):
+        return torch.from_numpy(data).to(dtype).to(device).contiguous()
+    else:
+        return torch.tensor(data, dtype=dtype, device=device).contiguous()
+
+def to_torch_f(data):
+    return to_torch(data, ftype)
+
+def to_torch_i(data):
+    return to_torch(data, itype)
+
+def read_image(image_path, is_srgb=None, remove_alpha=True):
+    image_path = Path(image_path)
+    image = iio.imread(image_path)
+    image = np.atleast_3d(image)
+    if remove_alpha and image.shape[2] == 4:
+        image = image[:, :, 0:3]
+
+    if image.dtype == np.uint8 or image.dtype == np.int16:
+        image = image.astype("float32") / 255.0
+    elif image.dtype == np.uint16 or image.dtype == np.int32:
+        image = image.astype("float32") / 65535.0
+
+    if is_srgb is None:
+        if image_path.suffix in ['.exr', '.hdr', '.rgbe']:
+            is_srgb = False
+        else:
+            is_srgb = True
+
+    if is_srgb:
+        image = to_linear(image)
+
+    return image
+
+def write_image(image_path, image, is_srgb=None):
+    image_path = Path(image_path)
+    image = to_numpy(image)
+    image = np.atleast_3d(image)
+    if image.shape[2] == 1:
+        image = np.repeat(image, 3, axis=2)
+
+    if is_srgb is None:
+        if image_path.suffix in ['.exr', '.hdr', '.rgbe']:
+            is_srgb = False
+        else:
+            is_srgb = True
+
+    if is_srgb:
+        image = to_srgb(image)
+
+    if image_path.suffix == '.exr':
+        image = image.astype(np.float32)
+    else:
+        image = (image * 255).astype(np.uint8)
+
+    iio.imwrite(image_path, image)
```

### Comparing `ivt-0.1.4/ivt/loss.py` & `ivt-0.1.5/ivt/loss.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import torch
-
-def l1_loss(target_image, rendered_image):
-    return (target_image - rendered_image).abs().mean() # NOTE
-
-def mesh_laplacian_smoothing(verts, faces):
-    # compute L once per mesh subdiv.
-    with torch.no_grad():
-        V, F = verts.shape[0], faces.shape[0]
-        face_verts = verts[faces]
-        v0, v1, v2 = face_verts[:, 0], face_verts[:, 1], face_verts[:, 2]
-        # Side lengths of each triangle, of shape (sum(F_n),)
-        # A is the side opposite v1, B is opposite v2, and C is opposite v3
-        A = (v1 - v2).norm(dim=1)
-        B = (v0 - v2).norm(dim=1)
-        C = (v0 - v1).norm(dim=1)
-        # Area of each triangle (with Heron's formula); shape is (sum(F_n),)
-        s = 0.5 * (A + B + C)
-        # note that the area can be negative (close to 0) causing nans after sqrt()
-        # we clip it to a small positive value
-        area = (s * (s - A) * (s - B) * (s - C)).clamp_(min=1e-6).sqrt()
-        # Compute cotangents of angles, of shape (sum(F_n), 3)
-        A2, B2, C2 = A * A, B * B, C * C
-        cota = (B2 + C2 - A2) / area
-        cotb = (A2 + C2 - B2) / area
-        cotc = (A2 + B2 - C2) / area
-        cot = torch.stack([cota, cotb, cotc], dim=1)
-        cot /= 4.0
-        # Construct a sparse matrix by basically doing:
-        # L[v1, v2] = cota
-        # L[v2, v0] = cotb
-        # L[v0, v1] = cotc
-        ii = faces[:, [1, 2, 0]]
-        jj = faces[:, [2, 0, 1]]
-        idx = torch.stack([ii, jj], dim=0).view(2, F * 3)
-        L = torch.sparse.FloatTensor(idx, cot.view(-1), (V, V))
-        # Make it symmetric; this means we are also setting
-        # L[v2, v1] = cota
-        # L[v0, v2] = cotb
-        # L[v1, v0] = cotc
-        L += L.t()
-        norm_w = torch.sparse.sum(L, dim=1).to_dense().view(-1, 1)
-        idx = norm_w > 1e-6
-        norm_w[idx] = 1.0 / norm_w[idx]
-    loss = L.mm(verts) * norm_w - verts
-    loss = loss.norm(dim=1)
-    return loss.mean()
-
-def total_variation_loss(texture, texture_mask):
-    m = (texture_mask[:-1, :-1] & texture_mask[1:, :-1] & texture_mask[:-1, 1:])
-    loss = (texture[:-1, :-1] - texture[1:, :-1])[m].abs().mean() +\
-           (texture[:-1, :-1] - texture[:-1, 1:])[m].abs().mean()
+import torch
+
+def l1_loss(target_image, rendered_image):
+    return (target_image - rendered_image).abs().mean() # NOTE
+
+def mesh_laplacian_smoothing(verts, faces):
+    # compute L once per mesh subdiv.
+    with torch.no_grad():
+        V, F = verts.shape[0], faces.shape[0]
+        face_verts = verts[faces]
+        v0, v1, v2 = face_verts[:, 0], face_verts[:, 1], face_verts[:, 2]
+        # Side lengths of each triangle, of shape (sum(F_n),)
+        # A is the side opposite v1, B is opposite v2, and C is opposite v3
+        A = (v1 - v2).norm(dim=1)
+        B = (v0 - v2).norm(dim=1)
+        C = (v0 - v1).norm(dim=1)
+        # Area of each triangle (with Heron's formula); shape is (sum(F_n),)
+        s = 0.5 * (A + B + C)
+        # note that the area can be negative (close to 0) causing nans after sqrt()
+        # we clip it to a small positive value
+        area = (s * (s - A) * (s - B) * (s - C)).clamp_(min=1e-6).sqrt()
+        # Compute cotangents of angles, of shape (sum(F_n), 3)
+        A2, B2, C2 = A * A, B * B, C * C
+        cota = (B2 + C2 - A2) / area
+        cotb = (A2 + C2 - B2) / area
+        cotc = (A2 + B2 - C2) / area
+        cot = torch.stack([cota, cotb, cotc], dim=1)
+        cot /= 4.0
+        # Construct a sparse matrix by basically doing:
+        # L[v1, v2] = cota
+        # L[v2, v0] = cotb
+        # L[v0, v1] = cotc
+        ii = faces[:, [1, 2, 0]]
+        jj = faces[:, [2, 0, 1]]
+        idx = torch.stack([ii, jj], dim=0).view(2, F * 3)
+        L = torch.sparse.FloatTensor(idx, cot.view(-1), (V, V))
+        # Make it symmetric; this means we are also setting
+        # L[v2, v1] = cota
+        # L[v0, v2] = cotb
+        # L[v1, v0] = cotc
+        L += L.t()
+        norm_w = torch.sparse.sum(L, dim=1).to_dense().view(-1, 1)
+        idx = norm_w > 1e-6
+        norm_w[idx] = 1.0 / norm_w[idx]
+    loss = L.mm(verts) * norm_w - verts
+    loss = loss.norm(dim=1)
+    return loss.mean()
+
+def total_variation_loss(texture, texture_mask):
+    m = (texture_mask[:-1, :-1] & texture_mask[1:, :-1] & texture_mask[:-1, 1:])
+    loss = (texture[:-1, :-1] - texture[1:, :-1])[m].abs().mean() +\
+           (texture[:-1, :-1] - texture[:-1, 1:])[m].abs().mean()
     return loss
```

### Comparing `ivt-0.1.4/ivt/model.py` & `ivt-0.1.5/ivt/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import torch
-from abc import ABC, abstractmethod
-from pathlib import Path
-from .config import *
-
-import gin 
-
-class Model(ABC):
-    def __init__(self, scene):
-        self.scene = scene
-
-    @abstractmethod
-    def zero_grad(self):
-        pass
-
-    @abstractmethod
-    def set_data(self):
-        pass
-
-    @abstractmethod
-    def step(self):
-        pass
-
-    @abstractmethod
-    def get_results(self):
-        pass
-
-    @abstractmethod
-    def write_results(self, result_path):
-        pass
-
-    def get_regularization(self):
-        return torch.tensor(0.0, device=device, dtype=ftype)
-
-@gin.configurable
-class MultiOpt(Model):
-
-    def __init__(self, scene, model_classes):
-        super().__init__(scene)
-
-        self._models = [model_class(scene) for model_class in model_classes]
-
-    def zero_grad(self):
-        for model in self._models:
-            model.zero_grad()
-
-    def set_data(self):
-        for model in self._models:
-            model.set_data()
-        
-    def step(self):
-        for model in self._models:
-            model.step()
-
-    def get_results(self):
-        results = []
-        for model in self._models:
-            results.append(model.get_results())
-        return results
-
-    def write_results(self, result_path):
-        for model in self._models:
-            model.write_results(result_path)
-
-    def get_regularization(self):
-        reg = 0
-        for model in self._models:
-            reg += model.get_regularization()
+import torch
+from abc import ABC, abstractmethod
+from pathlib import Path
+from .config import *
+
+import gin 
+
+class Model(ABC):
+    def __init__(self, scene):
+        self.scene = scene
+
+    @abstractmethod
+    def zero_grad(self):
+        pass
+
+    @abstractmethod
+    def set_data(self):
+        pass
+
+    @abstractmethod
+    def step(self):
+        pass
+
+    @abstractmethod
+    def get_results(self):
+        pass
+
+    @abstractmethod
+    def write_results(self, result_path):
+        pass
+
+    def get_regularization(self):
+        return torch.tensor(0.0, device=device, dtype=ftype)
+
+@gin.configurable
+class MultiOpt(Model):
+
+    def __init__(self, scene, model_classes):
+        super().__init__(scene)
+
+        self._models = [model_class(scene) for model_class in model_classes]
+
+    def zero_grad(self):
+        for model in self._models:
+            model.zero_grad()
+
+    def set_data(self):
+        for model in self._models:
+            model.set_data()
+        
+    def step(self):
+        for model in self._models:
+            model.step()
+
+    def get_results(self):
+        results = []
+        for model in self._models:
+            results.append(model.get_results())
+        return results
+
+    def write_results(self, result_path):
+        for model in self._models:
+            model.write_results(result_path)
+
+    def get_regularization(self):
+        reg = torch.tensor(0.0, device=device, dtype=ftype)
+        for model in self._models:
+            reg += model.get_regularization()
         return reg
```

### Comparing `ivt-0.1.4/ivt/renderer.py` & `ivt-0.1.5/ivt/renderer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from .connector import get_connector
-from .config import *
-import torch 
-import numpy as np
-
-import gin
-
-class RenderFunction(torch.autograd.Function):
-
-    @staticmethod
-    def forward(ctx, connector, scene, render_options, sensor_ids, integrator_id, *params):
-        images = connector.renderC(scene, render_options, sensor_ids=sensor_ids, integrator_id=integrator_id)
-        images = torch.stack(images, dim=0)
-
-        ctx.connector = connector
-        ctx.scene = scene
-        ctx.render_options = render_options
-        ctx.sensor_ids = sensor_ids
-        ctx.integrator_id = integrator_id
-        ctx.num_no_grads = 5 # number of inputs that don't require grad
-
-        ctx.params = params
-       
-        assert(images.sum().isfinite())
-        return images
-
-    @staticmethod
-    def backward(ctx, grad_out):
-        image_grads = [image_grad for image_grad in grad_out]
-        param_grads = ctx.connector.renderD(image_grads, ctx.scene, ctx.render_options, ctx.sensor_ids, ctx.integrator_id)
-        return tuple([None] * ctx.num_no_grads + param_grads)
-
-@gin.configurable
-class Renderer(torch.nn.Module):
-
-    def __init__(self, connector_name, render_options=None):
-        super().__init__()
-        self.connector = get_connector(connector_name)
-        self.render_options = render_options
-
-    def forward(self, scene, sensor_ids=[0], integrator_id=0):
-        assert self.render_options is not None, "Please set render options first."
-        if torch.is_tensor(sensor_ids):
-            sensor_ids = sensor_ids.flatten().tolist()
-
-        params = [scene[param_name] for param_name in scene.requiring_grad]
-        
-        images = RenderFunction.apply(self.connector, scene, self.render_options, sensor_ids, integrator_id, *params)
-        return images
-
-    def set_render_options(self, render_options):
+from .connector import get_connector
+from .config import *
+import torch 
+import numpy as np
+
+import gin
+
+class RenderFunction(torch.autograd.Function):
+
+    @staticmethod
+    def forward(ctx, connector, scene, render_options, sensor_ids, integrator_id, *params):
+        images = connector.renderC(scene, render_options, sensor_ids=sensor_ids, integrator_id=integrator_id)
+        images = torch.stack(images, dim=0)
+
+        ctx.connector = connector
+        ctx.scene = scene
+        ctx.render_options = render_options
+        ctx.sensor_ids = sensor_ids
+        ctx.integrator_id = integrator_id
+        ctx.num_no_grads = 5 # number of inputs that don't require grad
+
+        ctx.params = params
+       
+        assert(images.sum().isfinite())
+        return images
+
+    @staticmethod
+    def backward(ctx, grad_out):
+        image_grads = [image_grad for image_grad in grad_out]
+        param_grads = ctx.connector.renderD(image_grads, ctx.scene, ctx.render_options, ctx.sensor_ids, ctx.integrator_id)
+        return tuple([None] * ctx.num_no_grads + param_grads)
+
+@gin.configurable
+class Renderer(torch.nn.Module):
+
+    def __init__(self, connector_name, render_options=None):
+        super().__init__()
+        self.connector = get_connector(connector_name)
+        self.render_options = render_options
+
+    def forward(self, scene, sensor_ids=[0], integrator_id=0):
+        assert self.render_options is not None, "Please set render options first."
+        if torch.is_tensor(sensor_ids):
+            sensor_ids = sensor_ids.flatten().tolist()
+
+        params = [scene[param_name] for param_name in scene.requiring_grad]
+        
+        images = RenderFunction.apply(self.connector, scene, self.render_options, sensor_ids, integrator_id, *params)
+        return images
+
+    def set_render_options(self, render_options):
         self.render_options = render_options
```

### Comparing `ivt-0.1.4/ivt/sampling.py` & `ivt-0.1.5/ivt/sampling.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import torch 
-
-def sample_sphere(batch, radius, method='stratified', axis=1):
-	# assumes y-axis is up by default, otherwise we swap 
-	if method == 'uniform':
-		phi = torch.rand(batch, 1) * torch.pi 
-		theta = torch.rand(batch, 1) * 2 * torch.pi     
-		sinPhi = torch.sin(phi)  
-		cosPhi = torch.cos(phi) 
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-
-	elif method == 'stratified':
-		cosPhi = torch.linspace(1.0 - 0.01, -1.0 + 0.01, batch).unsqueeze(-1)
-		theta  = torch.linspace(0, torch.pi * 10, batch).unsqueeze(-1) \
-			+ torch.rand(batch, 1) * 0.01
-		
-		sinPhi = torch.sqrt(1 - cosPhi * cosPhi)
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-		
-	elif method == 'fibonacci':
-		# From http://extremelearning.com.au/how-to-evenly-distribute-points-on-a-sphere-more-effectively-than-the-canonical-fibonacci-lattice/
-		golden_ratio = (1 + 5**0.5) / 2
-		i = torch.arange(batch).unsqueeze(-1)
-		theta = 2 * torch.pi * i / golden_ratio
-		phi = torch.acos(1 - 2 * (i + 0.5) / batch)
-		sinPhi = torch.sin(phi)  
-		cosPhi = torch.cos(phi)
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-	
-	# Switch axis 
-	index = torch.LongTensor([0, 1, 2])
-	index[axis] = 1 
-	index[1] = axis 
-	points = samples[:, index]
-
-	return points
-
-def sample_hemisphere(batch, radius, method='stratified', axis=1):
-	# assumes y-axis is up by default, otherwise we swap 
-	if method == 'uniform':
-		phi = torch.rand(batch, 1) * torch.pi * 0.5
-		theta = torch.rand(batch, 1) * 2 * torch.pi     
-		sinPhi = torch.sin(phi)  
-		cosPhi = torch.cos(phi) 
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-
-	elif method == 'stratified':
-		cosPhi = torch.linspace(1.0 - 0.01, 0.0 + 0.01, batch).unsqueeze(-1)
-		theta  = torch.linspace(0, torch.pi * 10, batch).unsqueeze(-1) \
-			+ torch.rand(batch, 1) * 0.01
-		
-		sinPhi = torch.sqrt(1 - cosPhi * cosPhi)
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-		
-	elif method == 'fibonacci':
-		# From http://extremelearning.com.au/how-to-evenly-distribute-points-on-a-sphere-more-effectively-than-the-canonical-fibonacci-lattice/
-		golden_ratio = (1 + 5**0.5) / 2
-		i = torch.arange(batch).unsqueeze(-1)
-		theta = 2 * torch.pi * i / golden_ratio
-		phi = torch.acos(1 - (i + 0.5) / batch)
-		sinPhi = torch.sin(phi)  
-		cosPhi = torch.cos(phi)
-		sinTheta = torch.sin(theta) 
-		cosTheta = torch.cos(theta) 
-		samples = torch.cat([
-			sinPhi * cosTheta, 
-			cosPhi,
-			sinPhi * sinTheta
-		], dim=1) * radius
-	
-	# Switch axis 
-	index = torch.LongTensor([0, 1, 2])
-	index[axis] = 1 
-	index[1] = axis 
-	points = samples[:, index]
-
+import torch 
+
+def sample_sphere(batch, radius, method='stratified', axis=1):
+	# assumes y-axis is up by default, otherwise we swap 
+	if method == 'uniform':
+		phi = torch.rand(batch, 1) * torch.pi 
+		theta = torch.rand(batch, 1) * 2 * torch.pi     
+		sinPhi = torch.sin(phi)  
+		cosPhi = torch.cos(phi) 
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+
+	elif method == 'stratified':
+		cosPhi = torch.linspace(1.0 - 0.01, -1.0 + 0.01, batch).unsqueeze(-1)
+		theta  = torch.linspace(0, torch.pi * 10, batch).unsqueeze(-1) \
+			+ torch.rand(batch, 1) * 0.01
+		
+		sinPhi = torch.sqrt(1 - cosPhi * cosPhi)
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+		
+	elif method == 'fibonacci':
+		# From http://extremelearning.com.au/how-to-evenly-distribute-points-on-a-sphere-more-effectively-than-the-canonical-fibonacci-lattice/
+		golden_ratio = (1 + 5**0.5) / 2
+		i = torch.arange(batch).unsqueeze(-1)
+		theta = 2 * torch.pi * i / golden_ratio
+		phi = torch.acos(1 - 2 * (i + 0.5) / batch)
+		sinPhi = torch.sin(phi)  
+		cosPhi = torch.cos(phi)
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+	
+	# Switch axis 
+	index = torch.LongTensor([0, 1, 2])
+	index[axis] = 1 
+	index[1] = axis 
+	points = samples[:, index]
+
+	return points
+
+def sample_hemisphere(batch, radius, method='stratified', axis=1):
+	# assumes y-axis is up by default, otherwise we swap 
+	if method == 'uniform':
+		phi = torch.rand(batch, 1) * torch.pi * 0.5
+		theta = torch.rand(batch, 1) * 2 * torch.pi     
+		sinPhi = torch.sin(phi)  
+		cosPhi = torch.cos(phi) 
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+
+	elif method == 'stratified':
+		cosPhi = torch.linspace(1.0 - 0.01, 0.0 + 0.01, batch).unsqueeze(-1)
+		theta  = torch.linspace(0, torch.pi * 10, batch).unsqueeze(-1) \
+			+ torch.rand(batch, 1) * 0.01
+		
+		sinPhi = torch.sqrt(1 - cosPhi * cosPhi)
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+		
+	elif method == 'fibonacci':
+		# From http://extremelearning.com.au/how-to-evenly-distribute-points-on-a-sphere-more-effectively-than-the-canonical-fibonacci-lattice/
+		golden_ratio = (1 + 5**0.5) / 2
+		i = torch.arange(batch).unsqueeze(-1)
+		theta = 2 * torch.pi * i / golden_ratio
+		phi = torch.acos(1 - (i + 0.5) / batch)
+		sinPhi = torch.sin(phi)  
+		cosPhi = torch.cos(phi)
+		sinTheta = torch.sin(theta) 
+		cosTheta = torch.cos(theta) 
+		samples = torch.cat([
+			sinPhi * cosTheta, 
+			cosPhi,
+			sinPhi * sinTheta
+		], dim=1) * radius
+	
+	# Switch axis 
+	index = torch.LongTensor([0, 1, 2])
+	index[axis] = 1 
+	index[1] = axis 
+	points = samples[:, index]
+
 	return points
```

### Comparing `ivt-0.1.4/ivt/scene.py` & `ivt-0.1.5/ivt/scene.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-from .parameter import ParamGroup
-from .transform import lookat, perspective, batched_transform_pos, batched_transform_dir
-from .io import read_image, read_mesh, to_torch_f, to_torch_i
-
-from collections import OrderedDict
-
-import torch
-import torch.nn.functional as F
-
-class Scene:
-
-    def __init__(self) -> None:
-        self.components = OrderedDict()
-        self.requiring_grad = ()
-        self.cached = {}
-
-    def set(self, name, component):
-        self.components[name] = component
-
-    def __getitem__(self, name):
-        item = self.components
-        for c in name.split('.'):
-            item = item[c]
-        return item
-    
-    def __setitem__(self, name, param_value):
-        component_name, param_name = name.rsplit('.', 1)
-        self[component_name][param_name] = param_value
-    
-    def __contains__(self, name):
-        item = self.components
-        for c in name.split('.'):
-            if c not in item: return False
-            item = item[c]
-        return True
-
-    def configure(self):
-        requiring_grad = []
-        for cname in self.components:
-            requiring_grad += [f'{cname}.{pname}' for pname in self.components[cname].get_requiring_grad()]
-        self.requiring_grad = tuple(requiring_grad)
-
-    def __str__(self):
-        lines = []
-
-        for name in self.components:
-            lines.append(f"{name}:")
-            lines.append(str(self.components[name]))
-            lines.append("\n")
-
-        return '\n'.join(lines)
-    
-    def clear_cache(self):
-        self.cached = {}
-        # Detach the tensors requiring grad
-        for param_name in self.requiring_grad:
-            self[param_name] = self[param_name].detach()
-
-    def filter(self, component_type):
-        return [cname for cname in self.components if component_type == type(self.components[cname])]
-
-class Integrator(ParamGroup):
-
-    def __init__(self, type, config):
-        super().__init__()
-        
-        self.add_param('type', type, help_msg='integrator type')
-        self.add_param('config', config, help_msg='integrator config')
-
-class HDRFilm(ParamGroup):
-
-    def __init__(self, width, height):
-        super().__init__()
-        
-        self.add_param('width', width, help_msg='film width')
-        self.add_param('height', height, help_msg='film height')
-
-class PerspectiveCamera(ParamGroup):
-    
-    def __init__(self, fov, to_world, near=1e-6, far=1e7):
-        super().__init__()
-
-        self.add_param('fov', fov, help_msg='sensor fov')
-        self.add_param('near', near, help_msg='sensor near clip')
-        self.add_param('far', far, help_msg='sensor far clip')
-        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=True, help_msg='sensor to_world matrix')
-
-    def get_rays(self, samples, aspect_ratio):
-        samples = torch.cat([samples, torch.zeros_like(samples)[:, 0:1]], dim=1)
-        sample_to_camera = torch.inverse(perspective(self['fov'], aspect_ratio, self['near'], self['far']))
-        rays_o = batched_transform_pos(self['to_world'], to_torch_f([[0, 0, 0]]))
-        rays_d = F.normalize(batched_transform_pos(sample_to_camera, samples), dim=1)
-        rays_d = batched_transform_dir(self['to_world'], rays_d)
-        return rays_o.repeat(samples.shape[0], 1), rays_d
-
-    @classmethod
-    def from_lookat(cls, fov, origin, target, up, near=1e-6, far=1e7):
-        sensor = cls(fov, torch.eye(4), near, far)
-        origin = to_torch_f(origin)
-        target = to_torch_f(target)
-        up = to_torch_f(up)
-        sensor['to_world'] = lookat(origin, target, up)
-        return sensor
-        
-class Mesh(ParamGroup):
-
-    def __init__(self, v, f, uv, fuv, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
-        super().__init__()
-        
-        self.add_param('v', to_torch_f(v), is_tensor=True, is_diff=True, help_msg='mesh vertex positions')
-        self.add_param('f', to_torch_i(f), is_tensor=True, help_msg='mesh face indices')
-        self.add_param('uv', to_torch_f(uv), is_tensor=True, help_msg='mesh uv coordinates')
-        self.add_param('fuv', to_torch_i(fuv), is_tensor=True, help_msg='mesh uv face indices')
-        self.add_param('mat_id', mat_id, help_msg='name of the material of the mesh')
-        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, help_msg='mesh to world matrix')
-        self.add_param('use_face_normal', use_face_normal, help_msg='whether to use face normal')
-        self.add_param('can_change_topology', can_change_topology, help_msg='whether to the topology can be chagned')
-
-        radiance = to_torch_f(radiance)
-        is_emitter = radiance.sum() > 0
-        self.add_param('is_emitter', is_emitter, help_msg='whether it is used as an emitter')
-        self.add_param('radiance', radiance, is_tensor=True, is_diff=True, help_msg='radiance if it is used as an emitter')
-
-    @classmethod
-    def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
-        v, f, uv, fuv = read_mesh(filename)
-        return cls(v, f, uv, fuv, mat_id, to_world, use_face_normal, can_change_topology, radiance)
-    
-class DiffuseBRDF(ParamGroup):
-
-    def __init__(self, d):
-        super().__init__()
-        
-        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
-
-    @classmethod
-    def from_file(cls, filename, is_srgb=None):
-        texture = read_image(filename, is_srgb)
-        return cls(texture)
-    
-class MicrofacetBRDF(ParamGroup):
-
-    def __init__(self, d, s, r):
-        super().__init__()
-        
-        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
-        self.add_param('s', to_torch_f(s), is_tensor=True, is_diff=True, help_msg='specular reflectance')
-        self.add_param('r', to_torch_f(r), is_tensor=True, is_diff=True, help_msg='roughness')
-
-    @classmethod
-    def from_file(cls, d_filename, s_filename, r_filename, d_is_srgb=None, s_is_srgb=None, r_is_srgb=None):
-        d_texture = read_image(d_filename, d_is_srgb)
-        s_texture = read_image(s_filename, s_is_srgb)
-        r_texture = read_image(r_filename, r_is_srgb)[..., 0:1]
-
-        return cls(d_texture, s_texture, r_texture)
-    
-class EnvironmentLight(ParamGroup):
-
-    def __init__(self, radiance, to_world=torch.eye(4)):
-        super().__init__()
-        
-        self.add_param('radiance', to_torch_f(radiance), is_tensor=True, is_diff=True, help_msg='environment light radiance')
-        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=False, help_msg='environment to_world matrix')
-
-    @classmethod
-    def from_file(cls, radiance_filename, radiance_is_srgb=None, to_world=torch.eye(4)):
-        radiance_texture = read_image(radiance_filename, radiance_is_srgb)
-
+from .parameter import ParamGroup
+from .transform import lookat, perspective, batched_transform_pos, batched_transform_dir
+from .io import read_image, read_mesh, to_torch_f, to_torch_i
+
+from collections import OrderedDict
+
+import torch
+import torch.nn.functional as F
+
+class Scene:
+
+    def __init__(self) -> None:
+        self.components = OrderedDict()
+        self.requiring_grad = ()
+        self.cached = {}
+
+    def set(self, name, component):
+        self.components[name] = component
+
+    def __getitem__(self, name):
+        item = self.components
+        for c in name.split('.'):
+            item = item[c]
+        return item
+    
+    def __setitem__(self, name, param_value):
+        component_name, param_name = name.rsplit('.', 1)
+        self[component_name][param_name] = param_value
+    
+    def __contains__(self, name):
+        item = self.components
+        for c in name.split('.'):
+            if c not in item: return False
+            item = item[c]
+        return True
+
+    def configure(self):
+        requiring_grad = []
+        for cname in self.components:
+            requiring_grad += [f'{cname}.{pname}' for pname in self.components[cname].get_requiring_grad()]
+        self.requiring_grad = tuple(requiring_grad)
+
+    def __str__(self):
+        lines = []
+
+        for name in self.components:
+            lines.append(f"{name}:")
+            lines.append(str(self.components[name]))
+            lines.append("\n")
+
+        return '\n'.join(lines)
+    
+    def clear_cache(self):
+        self.cached = {}
+        # Detach the tensors requiring grad
+        for param_name in self.requiring_grad:
+            self[param_name] = self[param_name].detach()
+
+    def filter(self, component_type):
+        return [cname for cname in self.components if component_type == type(self.components[cname])]
+
+class Integrator(ParamGroup):
+
+    def __init__(self, type, config):
+        super().__init__()
+        
+        self.add_param('type', type, help_msg='integrator type')
+        self.add_param('config', config, help_msg='integrator config')
+
+class HDRFilm(ParamGroup):
+
+    def __init__(self, width, height):
+        super().__init__()
+        
+        self.add_param('width', width, help_msg='film width')
+        self.add_param('height', height, help_msg='film height')
+
+class PerspectiveCamera(ParamGroup):
+    
+    def __init__(self, fov, to_world, near=1e-6, far=1e7):
+        super().__init__()
+
+        self.add_param('fov', fov, help_msg='sensor fov')
+        self.add_param('near', near, help_msg='sensor near clip')
+        self.add_param('far', far, help_msg='sensor far clip')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=True, help_msg='sensor to_world matrix')
+
+    def get_rays(self, samples, aspect_ratio):
+        samples = torch.cat([samples, torch.zeros_like(samples)[:, 0:1]], dim=1)
+        sample_to_camera = torch.inverse(perspective(self['fov'], aspect_ratio, self['near'], self['far']))
+        rays_o = batched_transform_pos(self['to_world'], to_torch_f([[0, 0, 0]]))
+        rays_d = F.normalize(batched_transform_pos(sample_to_camera, samples), dim=1)
+        rays_d = batched_transform_dir(self['to_world'], rays_d)
+        return rays_o.repeat(samples.shape[0], 1), rays_d
+
+    @classmethod
+    def from_lookat(cls, fov, origin, target, up, near=1e-6, far=1e7):
+        sensor = cls(fov, torch.eye(4), near, far)
+        origin = to_torch_f(origin)
+        target = to_torch_f(target)
+        up = to_torch_f(up)
+        sensor['to_world'] = lookat(origin, target, up)
+        return sensor
+        
+class Mesh(ParamGroup):
+
+    def __init__(self, v, f, uv, fuv, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
+        super().__init__()
+        
+        self.add_param('v', to_torch_f(v), is_tensor=True, is_diff=True, help_msg='mesh vertex positions')
+        self.add_param('f', to_torch_i(f), is_tensor=True, help_msg='mesh face indices')
+        self.add_param('uv', to_torch_f(uv), is_tensor=True, help_msg='mesh uv coordinates')
+        self.add_param('fuv', to_torch_i(fuv), is_tensor=True, help_msg='mesh uv face indices')
+        self.add_param('mat_id', mat_id, help_msg='name of the material of the mesh')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, help_msg='mesh to world matrix')
+        self.add_param('use_face_normal', use_face_normal, help_msg='whether to use face normal')
+        self.add_param('can_change_topology', can_change_topology, help_msg='whether to the topology can be chagned')
+
+        radiance = to_torch_f(radiance)
+        is_emitter = radiance.sum() > 0
+        self.add_param('is_emitter', is_emitter, help_msg='whether it is used as an emitter')
+        self.add_param('radiance', radiance, is_tensor=True, is_diff=True, help_msg='radiance if it is used as an emitter')
+
+    @classmethod
+    def from_file(cls, filename, mat_id, to_world=torch.eye(4), use_face_normal=True, can_change_topology=False, radiance=torch.zeros(3)):
+        v, f, uv, fuv = read_mesh(filename)
+        return cls(v, f, uv, fuv, mat_id, to_world, use_face_normal, can_change_topology, radiance)
+    
+class DiffuseBRDF(ParamGroup):
+
+    def __init__(self, d):
+        super().__init__()
+        
+        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
+
+    @classmethod
+    def from_file(cls, filename, is_srgb=None):
+        texture = read_image(filename, is_srgb)
+        return cls(texture)
+    
+class MicrofacetBRDF(ParamGroup):
+
+    def __init__(self, d, s, r):
+        super().__init__()
+        
+        self.add_param('d', to_torch_f(d), is_tensor=True, is_diff=True, help_msg='diffuse reflectance')
+        self.add_param('s', to_torch_f(s), is_tensor=True, is_diff=True, help_msg='specular reflectance')
+        self.add_param('r', to_torch_f(r), is_tensor=True, is_diff=True, help_msg='roughness')
+
+    @classmethod
+    def from_file(cls, d_filename, s_filename, r_filename, d_is_srgb=None, s_is_srgb=None, r_is_srgb=None):
+        d_texture = read_image(d_filename, d_is_srgb)
+        s_texture = read_image(s_filename, s_is_srgb)
+        r_texture = read_image(r_filename, r_is_srgb)[..., 0:1]
+
+        return cls(d_texture, s_texture, r_texture)
+    
+class EnvironmentLight(ParamGroup):
+
+    def __init__(self, radiance, to_world=torch.eye(4)):
+        super().__init__()
+        
+        self.add_param('radiance', to_torch_f(radiance), is_tensor=True, is_diff=True, help_msg='environment light radiance')
+        self.add_param('to_world', to_torch_f(to_world), is_tensor=True, is_diff=False, help_msg='environment to_world matrix')
+
+    @classmethod
+    def from_file(cls, radiance_filename, radiance_is_srgb=None, to_world=torch.eye(4)):
+        radiance_texture = read_image(radiance_filename, radiance_is_srgb)
+
         return cls(radiance_texture, to_world)
```

### Comparing `ivt-0.1.4/ivt/transform.py` & `ivt-0.1.5/ivt/transform.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from .io import to_torch_f
-import torch 
-import torch.nn.functional as F
-
-def lookat(origin, target, up):
-    origin = to_torch_f(origin)
-    target = to_torch_f(target)
-    up = to_torch_f(up)
-
-    dir = F.normalize(target - origin, dim=0)
-    left = F.normalize(torch.cross(up, dir), dim=0)
-    new_up = F.normalize(torch.cross(dir, left), dim=0)
-
-    to_world = to_torch_f(torch.eye(4))
-    to_world[:3, 0] = left
-    to_world[:3, 1] = new_up
-    to_world[:3, 2] = dir
-    to_world[:3, 3] = origin
-
-    return to_world
-
-def perspective(fov, aspect_ratio, near=1e-6, far=1e7):
-    recip = 1 / (far - near)
-    tan = torch.tan(torch.deg2rad(to_torch_f(fov * 0.5)))
-    cot = 1 / tan
-
-    mat = torch.diag(to_torch_f([cot, cot, far * recip, 0]))
-    mat[2, 3] = -near * far * recip
-    mat[3, 2] = 1
-
-    mat = scale([-0.5, -0.5 * aspect_ratio, 1]) @ translate([-1, -1 / aspect_ratio, 0]) @ mat
-
-    return mat
-
-def batched_transform_pos(mat, vec):
-    mat = mat.view(1, 4, 4)
-    vec = vec.view(-1, 3, 1)
-    tmp = (mat @ torch.cat([vec, torch.ones_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
-    return tmp[:, 0:3] / tmp[:, 3:]
-
-def batched_transform_dir(mat, vec):
-    mat = mat.view(1, 4, 4)
-    vec = vec.view(-1, 3, 1)
-    tmp = (mat @ torch.cat([vec, torch.zeros_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
-    return tmp[:, 0:3]
-
-def translate(t_vec):
-    t_vec = to_torch_f(t_vec)
-
-    to_world = to_torch_f(torch.eye(4))
-    to_world[:3, 3] = t_vec
-
-    return to_world
-
-def rotate(axis, angle, use_degree=True):
-    axis = to_torch_f(axis)
-    angle = to_torch_f(angle)
-
-    to_world = to_torch_f(torch.eye(4))
-    axis = F.normalize(axis, dim=0).reshape(3, 1)
-
-    if use_degree:
-        angle = torch.deg2rad(angle)
-
-    sin_theta = torch.sin(angle)
-    cos_theta = torch.cos(angle)
-
-    cpm = to_torch_f(torch.zeros((3, 3)))
-    cpm[0, 1] = -axis[2]
-    cpm[0, 2] =  axis[1]
-    cpm[1, 0] =  axis[2]
-    cpm[1, 2] = -axis[0]
-    cpm[2, 0] = -axis[1]
-    cpm[2, 1] =  axis[0]
-
-    R = cos_theta * to_torch_f(torch.eye(3))
-    R += sin_theta * cpm
-    R += (1 - cos_theta) * (axis @ axis.T)
-
-    to_world[:3, :3] = R
-
-    return to_world
-
-def scale(size):
-    size = to_torch_f(size)
-
-    to_world = to_torch_f(torch.eye(4))
-
-    if size.size() == () or size.size(dim=0) == 1:
-        to_world[:3, :3] = to_torch_f(torch.eye(3)) * size
-    elif size.size(dim=0) == 3:
-        to_world[:3, :3] = torch.diag(size)
-    else:
-        print(f"unrecognized shape for size: {size.shape}")
-        exit()
-
-    return to_world
-
-# texture map transform (2d)
-def translate2D(t_vec):
-    t_vec = to_torch_f(t_vec)
-
-    to_world = to_torch_f(torch.eye(3))
-    to_world[:2, 2] = t_vec
-
-    return to_world
-
-def rotate2D(angle, use_degree=True):
-    angle = to_torch_f(angle)
-
-    to_world = to_torch_f(torch.eye(3))
-
-    if use_degree:
-        angle = torch.deg2rad(angle)
-
-    sin_theta = torch.sin(angle)
-    cos_theta = torch.cos(angle)
-
-    R = cos_theta * to_torch_f(torch.eye(2))
-
-    R[0 ,1] = -sin_theta
-    R[1 ,0] = sin_theta
-
-    to_world[:2, :2] = R
-
-    return to_world
-
-def scale2D(size):
-    size = to_torch_f(size)
-    to_world = to_torch_f(torch.eye(3))
-
-    if size.size(dim=0) == 1:
-        to_world[:2, :2] = torch.diag(size) * to_torch_f(torch.eye(2))
-    elif size.size(dim=0) == 2:
-        to_world[:2, :2] = torch.diag(size)
-    else:
-        print(f"unrecognized shape for size: {size.shape}")
-        exit()
-
+from .io import to_torch_f
+import torch 
+import torch.nn.functional as F
+
+def lookat(origin, target, up):
+    origin = to_torch_f(origin)
+    target = to_torch_f(target)
+    up = to_torch_f(up)
+
+    dir = F.normalize(target - origin, dim=0)
+    left = F.normalize(torch.cross(up, dir), dim=0)
+    new_up = F.normalize(torch.cross(dir, left), dim=0)
+
+    to_world = to_torch_f(torch.eye(4))
+    to_world[:3, 0] = left
+    to_world[:3, 1] = new_up
+    to_world[:3, 2] = dir
+    to_world[:3, 3] = origin
+
+    return to_world
+
+def perspective(fov, aspect_ratio, near=1e-6, far=1e7):
+    recip = 1 / (far - near)
+    tan = torch.tan(torch.deg2rad(to_torch_f(fov * 0.5)))
+    cot = 1 / tan
+
+    mat = torch.diag(to_torch_f([cot, cot, far * recip, 0]))
+    mat[2, 3] = -near * far * recip
+    mat[3, 2] = 1
+
+    mat = scale([-0.5, -0.5 * aspect_ratio, 1]) @ translate([-1, -1 / aspect_ratio, 0]) @ mat
+
+    return mat
+
+def batched_transform_pos(mat, vec):
+    mat = mat.view(1, 4, 4)
+    vec = vec.view(-1, 3, 1)
+    tmp = (mat @ torch.cat([vec, torch.ones_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
+    return tmp[:, 0:3] / tmp[:, 3:]
+
+def batched_transform_dir(mat, vec):
+    mat = mat.view(1, 4, 4)
+    vec = vec.view(-1, 3, 1)
+    tmp = (mat @ torch.cat([vec, torch.zeros_like(vec)[:, 0:1]], dim=1)).reshape(-1, 4)
+    return tmp[:, 0:3]
+
+def translate(t_vec):
+    t_vec = to_torch_f(t_vec)
+
+    to_world = to_torch_f(torch.eye(4))
+    to_world[:3, 3] = t_vec
+
+    return to_world
+
+def rotate(axis, angle, use_degree=True):
+    axis = to_torch_f(axis)
+    angle = to_torch_f(angle)
+
+    to_world = to_torch_f(torch.eye(4))
+    axis = F.normalize(axis, dim=0).reshape(3, 1)
+
+    if use_degree:
+        angle = torch.deg2rad(angle)
+
+    sin_theta = torch.sin(angle)
+    cos_theta = torch.cos(angle)
+
+    cpm = to_torch_f(torch.zeros((3, 3)))
+    cpm[0, 1] = -axis[2]
+    cpm[0, 2] =  axis[1]
+    cpm[1, 0] =  axis[2]
+    cpm[1, 2] = -axis[0]
+    cpm[2, 0] = -axis[1]
+    cpm[2, 1] =  axis[0]
+
+    R = cos_theta * to_torch_f(torch.eye(3))
+    R += sin_theta * cpm
+    R += (1 - cos_theta) * (axis @ axis.T)
+
+    to_world[:3, :3] = R
+
+    return to_world
+
+def scale(size):
+    size = to_torch_f(size)
+
+    to_world = to_torch_f(torch.eye(4))
+
+    if size.size() == () or size.size(dim=0) == 1:
+        to_world[:3, :3] = to_torch_f(torch.eye(3)) * size
+    elif size.size(dim=0) == 3:
+        to_world[:3, :3] = torch.diag(size)
+    else:
+        print(f"unrecognized shape for size: {size.shape}")
+        exit()
+
+    return to_world
+
+# texture map transform (2d)
+def translate2D(t_vec):
+    t_vec = to_torch_f(t_vec)
+
+    to_world = to_torch_f(torch.eye(3))
+    to_world[:2, 2] = t_vec
+
+    return to_world
+
+def rotate2D(angle, use_degree=True):
+    angle = to_torch_f(angle)
+
+    to_world = to_torch_f(torch.eye(3))
+
+    if use_degree:
+        angle = torch.deg2rad(angle)
+
+    sin_theta = torch.sin(angle)
+    cos_theta = torch.cos(angle)
+
+    R = cos_theta * to_torch_f(torch.eye(2))
+
+    R[0 ,1] = -sin_theta
+    R[1 ,0] = sin_theta
+
+    to_world[:2, :2] = R
+
+    return to_world
+
+def scale2D(size):
+    size = to_torch_f(size)
+    to_world = to_torch_f(torch.eye(3))
+
+    if size.size(dim=0) == 1:
+        to_world[:2, :2] = torch.diag(size) * to_torch_f(torch.eye(2))
+    elif size.size(dim=0) == 2:
+        to_world[:2, :2] = torch.diag(size)
+    else:
+        print(f"unrecognized shape for size: {size.shape}")
+        exit()
+
     return to_world
```

### Comparing `ivt-0.1.4/PKG-INFO` & `ivt-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ivt
-Version: 0.1.4
+Version: 0.1.5
 Summary: Inverse-Rendering Toolkit
 Author-email: Guangyan Cai <gcai3@uci.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imageio >= 2.27.0
+Requires-Dist: imageio-freeimage
 Requires-Dist: numpy
 Requires-Dist: gin-config
 Requires-Dist: gpytoolbox
 Project-URL: Home, https://github.com/uci-rendering/inv-render-toolkit
 
 # ivt
 `ivt` stands for Inverse-Rendering Toolkit. It is a simple framework for conducting inverse rendering experiments. Since there are a lot differentiable renderers in development, mastering them all and migrating between them can be a headache. `ivt` provides a simple scene representation based on `pytorch` that can be rendered by **connectors** that connect to different differentiable renderers and get the graident of the scene parameters. Migrating between renderers is just a matter of changing the connector.
```

