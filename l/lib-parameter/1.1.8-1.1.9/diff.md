# Comparing `tmp/lib_parameter-1.1.8.tar.gz` & `tmp/lib_parameter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lib_parameter-1.1.8.tar", last modified: Fri Oct  9 10:43:21 2020, max compression
+gzip compressed data, was "dist/lib_parameter-1.1.9.tar", last modified: Sun Nov 21 11:14:51 2021, max compression
```

## Comparing `lib_parameter-1.1.8.tar` & `lib_parameter-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4225 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 10:43:20.000000 lib_parameter-1.1.8/lib_parameter.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10632 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter.egg-info/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/lib_parameter/
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/lib_parameter/lib_parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/lib_parameter/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/lib_parameter/lib_parameter_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/lib_parameter/__init__conf__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/lib_parameter/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7762 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    10632 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2020-10-09 10:43:21.000000 lib_parameter-1.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      637 2020-10-09 10:42:40.000000 lib_parameter-1.1.8/CHANGES.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8723 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8010 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/lib_parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      545 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/lib_parameter/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/lib_parameter/lib_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/lib_parameter/lib_parameter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/lib_parameter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8723 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-21 11:14:50.000000 lib_parameter-1.1.9/lib_parameter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/lib_parameter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-11-21 11:14:51.000000 lib_parameter-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4191 2021-11-21 11:13:42.000000 lib_parameter-1.1.9/setup.py
```

### Comparing `lib_parameter-1.1.8/setup.py` & `lib_parameter-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,15 @@
 
 def get_requirements_from_file(requirements_filename: str) -> List[str]:
     """
     >>> assert len(get_requirements_from_file('requirements.txt')) > 0
     """
     l_requirements = list()
     try:
-        with open(
-            str(pathlib.Path(__file__).parent / requirements_filename), mode="r"
-        ) as requirements_file:
+        with open(str(pathlib.Path(__file__).parent / requirements_filename), mode="r") as requirements_file:
             for line in requirements_file:
                 line_data = get_line_data(line)
                 if line_data:
                     l_requirements.append(line_data)
     except FileNotFoundError:
         pass
     return l_requirements
@@ -82,37 +80,33 @@
 if is_travis_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
 setup_kwargs["name"] = "lib_parameter"
-setup_kwargs["version"] = "v1.1.8"
+setup_kwargs["version"] = "v1.1.9"
 setup_kwargs["url"] = "https://github.com/bitranox/lib_parameter"
 setup_kwargs["packages"] = find_packages()
 setup_kwargs["package_data"] = {"lib_parameter": ["py.typed", "*.pyi", "__init__.pyi"]}
-setup_kwargs[
-    "description"
-] = "small gist,to return a default value if the parameter is None"
+setup_kwargs["description"] = "small gist,to return a default value if the parameter is None"
 setup_kwargs["long_description"] = long_description
 setup_kwargs["long_description_content_type"] = "text/x-rst"
 setup_kwargs["author"] = "Robert Nowotny"
 setup_kwargs["author_email"] = "bitranox@gmail.com"
 setup_kwargs["classifiers"] = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-setup_kwargs["entry_points"] = {
-    "console_scripts": ["lib_parameter = lib_parameter.lib_parameter_cli:cli_main"]
-}
+setup_kwargs["entry_points"] = {"console_scripts": ["lib_parameter = lib_parameter.lib_parameter_cli:cli_main"]}
 # minimally needs to run tests - no project requirements here
 setup_kwargs["tests_require"] = tests_require
 # specify what a project minimally needs to run correctly
 setup_kwargs["install_requires"] = install_requires
 # minimally needs to run the setup script, dependencies needs also to put here for "setup.py install test"
 # dependencies must not be put here for pip install
 setup_kwargs["setup_requires"] = setup_requires
```

### Comparing `lib_parameter-1.1.8/lib_parameter/lib_parameter.py` & `lib_parameter-1.1.9/lib_parameter/lib_parameter.py`

 * *Files identical despite different names*

### Comparing `lib_parameter-1.1.8/lib_parameter/lib_parameter_cli.py` & `lib_parameter-1.1.9/lib_parameter/lib_parameter_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     """
     __init__conf__.print_info()
 
 
 @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
 @click.version_option(version=__init__conf__.version,
                       prog_name=__init__conf__.shell_command,
-                      message='{} version %(version)s'.format(__init__conf__.shell_command))
+                      message=f'{__init__conf__.shell_command} version {__init__conf__.version}')
 @click.option('--traceback/--no-traceback', is_flag=True, type=bool, default=None, help='return traceback information on cli')
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
 
 
 @cli_main.command('info', context_settings=CLICK_CONTEXT_SETTINGS)
```

### Comparing `lib_parameter-1.1.8/lib_parameter/__init__conf__.py` & `lib_parameter-1.1.9/lib_parameter/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+# CONF
+
 name = 'lib_parameter'
 title = 'small gist,to return a default value if the parameter is None'
-version = 'v1.1.8'
+version = 'v1.1.9'
 url = 'https://github.com/bitranox/lib_parameter'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_parameter'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_parameter:
 
     small gist,to return a default value if the parameter is None
 
-    Version : v1.1.8
+    Version : v1.1.9
     Url     : https://github.com/bitranox/lib_parameter
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_parameter-1.1.8/README.rst` & `lib_parameter-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,42 @@
+Metadata-Version: 2.1
+Name: lib_parameter
+Version: 1.1.9
+Summary: small gist,to return a default value if the parameter is None
+Home-page: https://github.com/bitranox/lib_parameter
+Author: Robert Nowotny
+Author-email: bitranox@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6.0
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 lib_parameter
 =============
 
 
-Version v1.1.8 as of 2020-10-09 see `Changelog`_
+Version v1.1.9 as of 2021-11-21 see `Changelog`_
 
-|travis_build| |license| |jupyter| |pypi|
+|build_badge| |license| |jupyter| |pypi|
 
 |codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
-.. |travis_build| image:: https://img.shields.io/travis/bitranox/lib_parameter/master.svg
-   :target: https://travis-ci.org/bitranox/lib_parameter
+
+.. |build_badge| image:: https://github.com/bitranox/lib_parameter/actions/workflows/python-tests.yml/badge.svg
+   :target: https://github.com/bitranox/lib_parameter/actions/workflows/python-tests.yml
+
 
 .. |license| image:: https://img.shields.io/github/license/webcomics/pywine.svg
    :target: http://en.wikipedia.org/wiki/MIT_License
 
 .. |jupyter| image:: https://mybinder.org/badge_logo.svg
  :target: https://mybinder.org/v2/gh/bitranox/lib_parameter/master?filepath=lib_parameter.ipynb
 
@@ -81,17 +103,17 @@
 ----
 
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.6.0 or newer
 
-tested on linux "bionic" with python 3.6, 3.7, 3.8, 3.9-dev, pypy3 - architectures: amd64, ppc64le, s390x, arm64
+tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10.0, pypy-3.8 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_parameter>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://travis-ci.org/bitranox/lib_parameter>`_, automatic daily builds and monitoring
+`100% code coverage <https://codecov.io/gh/bitranox/lib_parameter>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_parameter/actions/workflows/python-tests.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -119,15 +141,15 @@
 
     import the module and check the code - its easy and documented there, including doctest examples.
     in case of any questions the usage section might be expanded at a later time
 
 Usage from Commandline
 ------------------------
 
-.. code-block:: bash
+.. code-block::
 
    Usage: lib_parameter [OPTIONS] COMMAND [ARGS]...
 
      small gist,to return a default value if the parameter is None
 
    Options:
      --version                     Show the version and exit.
@@ -139,51 +161,51 @@
 
 Installation and Upgrade
 ------------------------
 
 - Before You start, its highly recommended to update pip and setup tools:
 
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip --upgrade pip
     python -m pip --upgrade setuptools
 
 - to install the latest release from PyPi via pip (recommended):
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip install --upgrade lib_parameter
 
 - to install the latest version from github via pip:
 
 
-.. code-block:: bash
+.. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_parameter.git
 
 
 - include it into Your requirements.txt:
 
-.. code-block:: bash
+.. code-block::
 
     # Insert following line in Your requirements.txt:
     # for the latest Release on pypi:
     lib_parameter
 
     # for the latest development version :
     lib_parameter @ git+https://github.com/bitranox/lib_parameter.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
 - to install the latest development version from source code:
 
-.. code-block:: bash
+.. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_parameter.git
     $ cd lib_parameter
     python setup.py install
 
 - via makefile:
@@ -213,14 +235,15 @@
 following modules will be automatically installed :
 
 .. code-block:: bash
 
     ## Project Requirements
     click
     cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
+    lib_detect_testenv @ git+https://github.com/bitranox/lib_detect_testenv.git
 
 Acknowledgements
 ----------------
 
 - special thanks to "uncle bob" Robert C. Martin, especially for his books on "clean code" and "clean architecture"
 
 Contribute
@@ -239,14 +262,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+------
+2021-11-21: service release
+    - implement github actions
+    - implement check for test environment on __init__
+
 v1.1.8
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 v1.1.7
@@ -265,7 +294,9 @@
 ---------
 2020-08-01: fix pypi deploy
 
 v1.1.4
 -------
 2020-07-31: initial PyPi release
 
+
+
```

### Comparing `lib_parameter-1.1.8/setup.cfg` & `lib_parameter-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `lib_parameter-1.1.8/CHANGES.rst` & `lib_parameter-1.1.9/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.1.9
+------
+2021-11-21: service release
+    - implement github actions
+    - implement check for test environment on __init__
+
 v1.1.8
 --------
 2020-10-09: service release
     - update travis build matrix for linux 3.9-dev
     - update travis build matrix (paths) for windows 3.9 / 3.10
 
 v1.1.7
```

