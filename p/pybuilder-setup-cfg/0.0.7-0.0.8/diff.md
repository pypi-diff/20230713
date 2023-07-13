# Comparing `tmp/pybuilder-setup-cfg-0.0.7.tar.gz` & `tmp/pybuilder-setup-cfg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybuilder-setup-cfg-0.0.7.tar", last modified: Tue Mar  9 18:06:45 2021, max compression
+gzip compressed data, was "dist\pybuilder-setup-cfg-0.0.8.tar", last modified: Thu Mar 11 09:46:50 2021, max compression
```

## Comparing `pybuilder-setup-cfg-0.0.7.tar` & `pybuilder-setup-cfg-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/
--rw-rw-rw-   0        0        0      576 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg/
--rw-rw-rw-   0        0        0     6742 2021-03-09 18:02:56.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/
--rw-rw-rw-   0        0        0      576 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       13 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2021-03-09 18:06:45.000000 pybuilder-setup-cfg-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1604 2021-03-09 18:06:44.000000 pybuilder-setup-cfg-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/
+-rw-rw-rw-   0        0        0      576 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg/
+-rw-rw-rw-   0        0        0     7041 2021-03-11 09:35:58.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/
+-rw-rw-rw-   0        0        0      576 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       13 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2021-03-11 09:46:50.000000 pybuilder-setup-cfg-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1604 2021-03-11 09:46:49.000000 pybuilder-setup-cfg-0.0.8/setup.py
```

### Comparing `pybuilder-setup-cfg-0.0.7/PKG-INFO` & `pybuilder-setup-cfg-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pybuilder-setup-cfg
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyBuilder plugin for getting information from setup.cfg file or environment variables
 Home-page: https://github.com/margru/pybuilder-setup-cfg
 Author: Martin Gruber
 Author-email: martin.gruber@email.cz
 License: MIT
 Description: 
         Please, see https://github.com/margru/pybuilder-setup-cfg for more information.
```

### Comparing `pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg/__init__.py` & `pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     pass
 
 
 @init
 def init1_from_setup_cfg(project, logger):
 
     config = configparser.ConfigParser(interpolation=configparser.ExtendedInterpolation())
-    config.read("setup.cfg")
-    logger.debug("setup_cfg plugin: Loaded setup.cfg")
+    logger.debug(f"setup_cfg plugin: Project basedir: {project.basedir}")
+    setup_filename = os.path.join(project.basedir, "setup.cfg")
+    try:
+        config.read(setup_filename)
+    except Exception:
+        logger.error(f"setup_cfg plugin: setup.cfg not loaded ({setup_filename})")
+    else:
+        logger.info(f"setup_cfg plugin: Loaded configuration from {setup_filename}")
 
     name = os.environ.get("PYB_SCFG_NAME", config.get("metadata", "name", fallback=None))
     version = os.environ.get("PYB_SCFG_VERSION", config.get("metadata", "version", fallback=None))
     if version and version.startswith("file: "):
         version = read_from(version.split(maxsplit=1)[1])
     distutils_commands = list(filter(lambda item: item.strip(), map(
         lambda item: item.strip(), os.environ.get(
```

### Comparing `pybuilder-setup-cfg-0.0.7/pybuilder_setup_cfg.egg-info/PKG-INFO` & `pybuilder-setup-cfg-0.0.8/pybuilder_setup_cfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pybuilder-setup-cfg
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyBuilder plugin for getting information from setup.cfg file or environment variables
 Home-page: https://github.com/margru/pybuilder-setup-cfg
 Author: Martin Gruber
 Author-email: martin.gruber@email.cz
 License: MIT
 Description: 
         Please, see https://github.com/margru/pybuilder-setup-cfg for more information.
```

### Comparing `pybuilder-setup-cfg-0.0.7/setup.py` & `pybuilder-setup-cfg-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.post_install_script()
 
 
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-setup-cfg',
-        version = '0.0.7',
+        version = '0.0.8',
         description = 'PyBuilder plugin for getting information from setup.cfg file or environment variables',
         long_description = '\nPlease, see https://github.com/margru/pybuilder-setup-cfg for more information.\n',
         author = 'Martin Gruber',
         author_email = 'martin.gruber@email.cz',
         license = 'MIT',
         url = 'https://github.com/margru/pybuilder-setup-cfg',
         scripts = [],
```

