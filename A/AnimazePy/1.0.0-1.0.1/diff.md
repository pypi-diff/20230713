# Comparing `tmp/AnimazePy-1.0.0.tar.gz` & `tmp/AnimazePy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimazePy-1.0.0.tar", last modified: Thu Jul 13 18:47:10 2023, max compression
+gzip compressed data, was "AnimazePy-1.0.1.tar", last modified: Thu Jul 13 19:26:34 2023, max compression
```

## Comparing `AnimazePy-1.0.0.tar` & `AnimazePy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:10.072906 AnimazePy-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:10.072906 AnimazePy-1.0.0/AnimazePy/
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-13 18:46:59.000000 AnimazePy-1.0.0/AnimazePy/AnimazePy.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-13 18:46:59.000000 AnimazePy-1.0.0/AnimazePy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:47:10.072906 AnimazePy-1.0.0/AnimazePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-13 18:47:10.000000 AnimazePy-1.0.0/AnimazePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 18:47:10.000000 AnimazePy-1.0.0/AnimazePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:47:10.000000 AnimazePy-1.0.0/AnimazePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 18:47:10.000000 AnimazePy-1.0.0/AnimazePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 18:47:10.000000 AnimazePy-1.0.0/AnimazePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 18:46:59.000000 AnimazePy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-13 18:47:10.072906 AnimazePy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 18:46:59.000000 AnimazePy-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:47:10.072906 AnimazePy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 18:46:59.000000 AnimazePy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/AnimazePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/AnimazePy/AnimazeWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/AnimazePy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/AnimazePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 19:26:34.000000 AnimazePy-1.0.1/AnimazePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:26:34.651905 AnimazePy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-13 19:26:25.000000 AnimazePy-1.0.1/setup.py
```

### Comparing `AnimazePy-1.0.0/AnimazePy/AnimazePy.py` & `AnimazePy-1.0.1/AnimazePy/AnimazeWrapper.py`

 * *Files identical despite different names*

### Comparing `AnimazePy-1.0.0/AnimazePy/__init__.py` & `AnimazePy-1.0.1/AnimazePy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
-from . import AnimazePy
+from .AnimazeWrapper import AnimazeWrapper
```

### Comparing `AnimazePy-1.0.0/LICENSE` & `AnimazePy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimazePy-1.0.0/setup.py` & `AnimazePy-1.0.1/setup.py`

 * *Files identical despite different names*

