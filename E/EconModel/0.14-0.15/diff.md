# Comparing `tmp/EconModel-0.14.tar.gz` & `tmp/EconModel-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EconModel-0.14.tar", last modified: Mon Jul 10 07:17:17 2023, max compression
+gzip compressed data, was "EconModel-0.15.tar", last modified: Thu Jul 13 15:01:01 2023, max compression
```

## Comparing `EconModel-0.14.tar` & `EconModel-0.15.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.227231 EconModel-0.14/
-drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.201247 EconModel-0.14/EconModel/
--rw-rw-rw-   0        0        0    11921 2023-07-10 07:10:54.000000 EconModel-0.14/EconModel/EconModel.py
--rw-rw-rw-   0        0        0       59 2023-01-27 12:31:05.000000 EconModel-0.14/EconModel/__init__.py
--rw-rw-rw-   0        0        0    13724 2023-06-19 07:38:29.000000 EconModel-0.14/EconModel/cppcompile.py
--rw-rw-rw-   0        0        0     7933 2022-02-11 13:27:34.000000 EconModel-0.14/EconModel/cppstruct.py
--rw-rw-rw-   0        0        0    15038 2022-02-17 15:53:49.000000 EconModel-0.14/EconModel/cpptools.py
--rw-rw-rw-   0        0        0     1199 2022-02-16 13:47:45.000000 EconModel-0.14/EconModel/jit.py
-drwxrwxrwx   0        0        0        0 2023-07-10 07:17:17.224233 EconModel-0.14/EconModel.egg-info/
--rw-rw-rw-   0        0        0      254 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-10 07:17:17.000000 EconModel-0.14/EconModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 07:17:16.000000 EconModel-0.14/EconModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1095 2022-01-29 10:51:26.000000 EconModel-0.14/LICENSE
--rw-rw-rw-   0        0        0      254 2023-07-10 07:17:17.227231 EconModel-0.14/PKG-INFO
--rw-rw-rw-   0        0        0     3485 2023-05-11 05:52:08.000000 EconModel-0.14/README.md
--rw-rw-rw-   0        0        0       86 2023-07-10 07:17:17.230230 EconModel-0.14/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-07-10 07:14:00.000000 EconModel-0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:01:01.411916 EconModel-0.15/
+drwxrwxrwx   0        0        0        0 2023-07-13 15:01:01.356061 EconModel-0.15/EconModel/
+-rw-rw-rw-   0        0        0    12069 2023-07-13 12:39:31.000000 EconModel-0.15/EconModel/EconModel.py
+-rw-rw-rw-   0        0        0       59 2021-06-05 20:09:11.000000 EconModel-0.15/EconModel/__init__.py
+-rw-rw-rw-   0        0        0    13714 2023-07-13 12:49:46.000000 EconModel-0.15/EconModel/cppcompile.py
+-rw-rw-rw-   0        0        0     7935 2023-07-13 14:21:38.000000 EconModel-0.15/EconModel/cppstruct.py
+-rw-rw-rw-   0        0        0    15038 2023-07-13 12:53:15.000000 EconModel-0.15/EconModel/cpptools.py
+-rw-rw-rw-   0        0        0     1199 2023-07-13 12:29:06.000000 EconModel-0.15/EconModel/jit.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:01:01.408204 EconModel-0.15/EconModel.egg-info/
+-rw-rw-rw-   0        0        0      254 2023-07-13 15:01:00.000000 EconModel-0.15/EconModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-13 15:01:01.000000 EconModel-0.15/EconModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:01:00.000000 EconModel-0.15/EconModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 15:01:00.000000 EconModel-0.15/EconModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1095 2022-01-29 10:51:26.000000 EconModel-0.15/LICENSE
+-rw-rw-rw-   0        0        0      254 2023-07-13 15:01:01.412907 EconModel-0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     3485 2023-05-11 05:52:08.000000 EconModel-0.15/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-13 15:01:01.424185 EconModel-0.15/setup.cfg
+-rw-rw-rw-   0        0        0      315 2023-07-13 14:57:13.000000 EconModel-0.15/setup.py
```

### Comparing `EconModel-0.14/EconModel/EconModel.py` & `EconModel-0.15/EconModel/EconModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,31 +235,29 @@
         if not skip is None:
             for attr in skip:
                 del model_dict[attr]
                 
         # c. construct                
         self.from_dict(model_dict)
 
-    def copy(self,name=None,**kwargs):
+    def copy(self,name=None):
         """ copy the model """
         
         # a. name
         if name is None: name = f'{self.name}_copy'
         
         # b. model dict
         model_dict = self.as_dict()
 
         # c. initialize
         other = self.__class__(name=name)
 
         # d. fill
         other.from_dict(model_dict,do_copy=True)
-        other.__update(kwargs)
-        
-        if hasattr(self,'_ns_specs'): other._ns_specs = self._ns_specs
+        other._ns_specs = self._ns_specs # same jit can be used
 
         if not type(self.cpp) is SimpleNamespace:
             other.link_to_cpp(force_compile=False)
         else:
             other.cpp = SimpleNamespace()
 
         return other
@@ -283,15 +281,20 @@
                     description += f' {key} = {val} [{type(val).__name__}]\n'
                 elif type(val) is np.bool_:
                     if val:
                         description += f' {key} = True\n'
                     else:
                         description += f' {key} = False\n'
                 elif type(val) is np.ndarray:
-                    description += f' {key} = ndarray with shape = {val.shape} [dtype: {val.dtype}]\n'            
+                    if val.nbytes > 0.5*10**9:
+                        memstr = f'{val.nbytes/10**9:.1f} gb'
+                    else:
+                        memstr = f'{val.nbytes/10**6:.1f} mb'
+
+                    description += f' {key} = ndarray[{val.dtype}] with shape = {val.shape} [{memstr}]\n'            
                     nbytes += val.nbytes
                 else:                
                     description += f' {key} = ?\n'
 
             description += f' memory, gb: {nbytes/(10**9):.1f}\n' 
             return description
```

### Comparing `EconModel-0.14/EconModel/cppcompile.py` & `EconModel-0.15/EconModel/cppcompile.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,31 +174,31 @@
     """
 
     if os.path.isdir(f'{os.getcwd()}/{folder}autodiff'):
         if do_print: print('autodiff already installed')
         return
 
     # a. download
-    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}autodiff-master.zip')
+    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}autodiff-main.zip')
     if download:
-        url = 'https://github.com/autodiff/autodiff/archive/refs/heads/master.zip'
+        url = 'https://github.com/autodiff/autodiff/archive/refs/heads/main.zip'
         urllib.request.urlretrieve(url,zipfilename)
         
     # b. unzip
     if download or unzip:
         with zipfile.ZipFile(zipfilename) as file:
             file.extractall(f'{os.getcwd()}/{folder}')
         
     # c. move
-    src = f'{os.getcwd()}/{folder}/autodiff-master/autodiff'
+    src = f'{os.getcwd()}/{folder}/autodiff-main/autodiff'
     dst = f'{os.getcwd()}/{folder}/autodiff'
     shutil.move(src,dst)
 
     # d. clean
-    shutil.rmtree(f'{os.getcwd()}/{folder}/autodiff-master/')
+    shutil.rmtree(f'{os.getcwd()}/{folder}/autodiff-main/')
 
     if do_print: print('autodiff succesfully installed')
 
 def setup_Eigen(download=True,unzip=False,folder='cppfuncs/',do_print=False):
     """download and setup autodiff
 
     Args:
@@ -211,15 +211,15 @@
     """
 
     if os.path.isdir(f'{os.getcwd()}/{folder}Eigen'):
         if do_print: print('Eigen already installed')
         return
 
     # a. download
-    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}Eigen-master.zip')
+    zipfilename = os.path.abspath(f'{os.getcwd()}/{folder}Eigen-main.zip')
     if download:
         url = 'https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.zip'
         urllib.request.urlretrieve(url,zipfilename)
         
     # b. unzip
     if download or unzip:
         with zipfile.ZipFile(zipfilename) as file:
```

### Comparing `EconModel-0.14/EconModel/cppstruct.py` & `EconModel-0.15/EconModel/cppstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,27 +41,27 @@
 
     # b. main
     for key,val in pythonobj.__dict__.items():
 
         # i. scalars
         if np.isscalar(val):
 
-            if type(val) in [np.int,np.int_]:
+            if type(val) in [int,np.int_]:
         
                 ctlist.append((key,ct.c_long))
                 cttxt += f' int {key};\n'
                 ctfunctxt_update('int',key)
         
-            elif type(val) in [np.float,np.float_]:
+            elif type(val) in [float,np.float_]:
             
                 ctlist.append((key,ct.c_double))          
                 cttxt += f' double {key};\n'
                 ctfunctxt_update('double',key)
 
-            elif type(val) is np.bool:
+            elif type(val) in [bool,np.bool_]:
         
                 ctlist.append((key,ct.c_bool))
                 cttxt += f' bool {key};\n'
                 ctfunctxt_update('bool',key)
             
             elif type(val) is str:
```

### Comparing `EconModel-0.14/EconModel/cpptools.py` & `EconModel-0.15/EconModel/cpptools.py`

 * *Files identical despite different names*

### Comparing `EconModel-0.14/EconModel/jit.py` & `EconModel-0.15/EconModel/jit.py`

 * *Files identical despite different names*

### Comparing `EconModel-0.14/LICENSE` & `EconModel-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `EconModel-0.14/README.md` & `EconModel-0.15/README.md`

 * *Files identical despite different names*

