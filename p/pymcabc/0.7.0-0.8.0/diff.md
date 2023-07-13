# Comparing `tmp/pymcabc-0.7.0.tar.gz` & `tmp/pymcabc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.7.0.tar", last modified: Wed Jul 12 16:13:19 2023, max compression
+gzip compressed data, was "pymcabc-0.8.0.tar", last modified: Thu Jul 13 05:10:39 2023, max compression
```

## Comparing `pymcabc-0.7.0.tar` & `pymcabc-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 16:13:07.000000 pymcabc-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 16:13:07.000000 pymcabc-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-12 16:13:19.979311 pymcabc-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-12 16:13:07.000000 pymcabc-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-12 16:13:07.000000 pymcabc-0.7.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 16:13:19.000000 pymcabc-0.7.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:13:19.979311 pymcabc-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 16:13:07.000000 pymcabc-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:13:19.979311 pymcabc-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_boost.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_crosssection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_evengen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_identify.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-12 16:13:07.000000 pymcabc-0.7.0/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.023323 pymcabc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 05:10:27.000000 pymcabc-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-13 05:10:27.000000 pymcabc-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 05:10:39.019322 pymcabc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 05:10:27.000000 pymcabc-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-13 05:10:27.000000 pymcabc-0.8.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 05:10:39.000000 pymcabc-0.8.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:10:39.023323 pymcabc-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-13 05:10:27.000000 pymcabc-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:10:39.019322 pymcabc-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-13 05:10:27.000000 pymcabc-0.8.0/tests/test_plot.py
```

### Comparing `pymcabc-0.7.0/LICENSE` & `pymcabc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/PKG-INFO` & `pymcabc-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.7.0
+Version: 0.8.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.7.0/README.md` & `pymcabc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/cross_section.py` & `pymcabc-0.8.0/pymcabc/cross_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             w_i = CrossSection().dsigma_st(costh) * 2 * 2 * math.pi  
         elif self.process == "tu":
             w_i = CrossSection().dsigma_tu(costh) * 2 * 2 * math.pi 
         if w_max < w_i:
             w_max = w_i
         return w_i, w_max
 
-    def integrate_xsec(self, N=20000):
+    def integrate_xsec(self, N=40000):
         w_sum = 0
         w_max = 0
         w_square = 0
         for _i in range(N):
             w_i, w_max = CrossSection().xsection(w_max)
             w_sum += w_i
             w_square += w_i * w_i
@@ -136,15 +136,15 @@
         library["w_max"].append(w_max)
         library["w_square"].append(w_square)
         library["w_sum"].append(w_sum)
         with open("library.json", "w") as f:
             json.dump(library, f)
         return None
 
-    def calc_xsection(self, N: int = 20000):
+    def calc_xsection(self, N: int = 40000):
         self.integrate_xsec(N)
         with open("library.json", "r") as f:
             library = json.load(f)
         w_sum = library["w_sum"][0]
         w_square = library["w_square"][0]
         w_max = library["w_max"][0]
         sigma_x = w_sum * pymcabc.constants.convert/ (N * 1e12)  # result in barn unit
```

### Comparing `pymcabc-0.7.0/pymcabc/decay_particle.py` & `pymcabc-0.8.0/pymcabc/decay_particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/detector.py` & `pymcabc-0.8.0/pymcabc/detector.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/feynman_diagram.py` & `pymcabc-0.8.0/pymcabc/feynman_diagram.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/generate_event.py` & `pymcabc-0.8.0/pymcabc/generate_event.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/identify_process.py` & `pymcabc-0.8.0/pymcabc/identify_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         #self.library["E2"].append(self.E2)
         self.library["channel"].append(channel)
         self.process()
         self.channel()
         self.masses()
         self.identify_mediator()
         self.identify_decay()
-        self.ECM()
+        self._ECM()
         self.final_momenta()
         self.bw()
 
     def process(self):
         """identify the physics process"""
         self.library["process"].append(self.input_string)
         string = self.input_string.replace(" > ", " ")
@@ -143,37 +143,47 @@
         self.library["m2"].append(pmass[1])
         self.library["m3"].append(pmass[2])
         self.library["m4"].append(pmass[3])
         with open("library.json", "w") as f:
             json.dump(self.library, f)
         return None
     
-    def ECM(self):
+    def _ECM(self):
         #center of mass energy
         with open("library.json", "r") as f:
             library = json.load(f)
         m1 = library["m1"][0]
         m2 = library["m2"][0]
         E1 = math.sqrt(m1**2 + self.p_i**2)
         E2 = math.sqrt(m2**2 + self.p_i**2)
         Ecm = E1 + E2
-        if len(self.library["Ecm"]) == 0:
-            self.library["Ecm"].append(Ecm)
+        self.library["Ecm"].append(Ecm)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
+        return E1, E2, Ecm
+    
+    def ECM(self):
+        with open("library.json", "r") as f:
+            library = json.load(f)
+        m1 = library["m1"][0]
+        m2 = library["m2"][0]
+        E1 = math.sqrt(m1**2 + self.p_i**2)
+        E2 = math.sqrt(m2**2 + self.p_i**2)
+        Ecm = E1 + E2
         print(
               "\n",
             "Energy Beam 1 : ", E1,
               "\n",
             "Energy Beam 2 : ", E2,
               "\n",
             "Energy CM : ", Ecm,
               )
         return E1, E2, Ecm
-    
+
+
 
     def identify_mediator(self):
         """identify the mediator of the process"""
         process = self.library["process"][0]
         process = process.replace(" > ", " ")
         if (
             process == "A A B B"
@@ -208,16 +218,20 @@
     def final_momenta(self):
         p_f = pymcabc.constants.outgoing_p(self.library["Ecm"][0], self.library["m3"][0], self.library["m4"][0])
         self.library["outgoing_p"].append(p_f)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
 
     def bw(self):
-        deno  = 8*math.pi*(self.library["mx"][0])**2
-        self.library["bw"].append((pymcabc.constants.g**2*self.library["outgoing_p"][0])/deno)
+        if self.library["mx"][0] > 0:
+            deno  = 8*math.pi*(self.library["mx"][0])**2
+            _bw = (pymcabc.constants.g**2*self.library["outgoing_p"][0])/deno
+        else:
+            _bw = 0.0
+        self.library["bw"].append(_bw)
         with open("library.json", "w") as f:
             json.dump(self.library, f)
 
     def identify_decay(self):
         """identify the decay chain associated with the process"""
         mA = self.library["mA"][0]
         mB = self.library["mB"][0]
```

### Comparing `pymcabc-0.7.0/pymcabc/particle.py` & `pymcabc-0.8.0/pymcabc/particle.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/plotting.py` & `pymcabc-0.8.0/pymcabc/plotting.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc/save_events.py` & `pymcabc-0.8.0/pymcabc/save_events.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.8.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.7.0
+Version: 0.8.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.7.0/pymcabc.egg-info/SOURCES.txt` & `pymcabc-0.8.0/pymcabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/setup.py` & `pymcabc-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="pymcabc",
-    version="0.7.0",
+    version="0.8.0",
     description="Monte Carlo Event Generator for the ABC theory",
     author="Aman Desai",
     author_email="amanmukeshdesai@gmail.com",
     maintainer="Aman Desai",
     maintainer_email="amanmukeshdesai@gmail.com",
     url="https://github.com/amanmdesai/pymcabc",
     long_description=long_description,
```

### Comparing `pymcabc-0.7.0/tests/test_crosssection.py` & `pymcabc-0.8.0/tests/test_crosssection.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/tests/test_evengen.py` & `pymcabc-0.8.0/tests/test_evengen.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/tests/test_identify.py` & `pymcabc-0.8.0/tests/test_identify.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.7.0/tests/test_plot.py` & `pymcabc-0.8.0/tests/test_plot.py`

 * *Files identical despite different names*

