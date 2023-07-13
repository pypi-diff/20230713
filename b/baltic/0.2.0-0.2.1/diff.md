# Comparing `tmp/baltic-0.2.0.tar.gz` & `tmp/baltic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baltic-0.2.0.tar", last modified: Wed Jul 12 11:06:54 2023, max compression
+gzip compressed data, was "baltic-0.2.1.tar", last modified: Wed Jul 12 12:26:30 2023, max compression
```

## Comparing `baltic-0.2.0.tar` & `baltic-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.103453 baltic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-12 11:06:45.000000 baltic-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 11:06:45.000000 baltic-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 11:06:45.000000 baltic-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 11:06:45.000000 baltic-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-12 11:06:54.103453 baltic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-12 11:06:45.000000 baltic-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.099453 baltic-0.2.0/baltic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 11:06:45.000000 baltic-0.2.0/baltic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77016 2023-07-12 11:06:45.000000 baltic-0.2.0/baltic/baltic.py
--rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-07-12 11:06:45.000000 baltic-0.2.0/baltic/samogitia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.099453 baltic-0.2.0/baltic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 11:06:54.000000 baltic-0.2.0/baltic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 11:06:45.000000 baltic-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:06:54.103453 baltic-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 11:06:45.000000 baltic-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.099453 baltic-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.103453 baltic-0.2.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:06:54.103453 baltic-0.2.0/tests/data/2020-04-13_treetime/
--rw-r--r--   0 runner    (1001) docker     (123)    73234 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/2020-04-13_treetime/divergence_tree.nexus
--rw-r--r--   0 runner    (1001) docker     (123)    72774 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/2020-04-13_treetime/timetree.nexus
--rw-r--r--   0 runner    (1001) docker     (123)   272511 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/MERS.mcc.tree
--rw-r--r--   0 runner    (1001) docker     (123)   222372 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/miniFluB.mcc.tree
--rw-r--r--   0 runner    (1001) docker     (123)  2925238 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/zika.fa
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/data/zika.nwk
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-12 11:06:45.000000 baltic-0.2.0/tests/testsuite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.930565 baltic-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-12 12:26:21.000000 baltic-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-12 12:26:21.000000 baltic-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 12:26:21.000000 baltic-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 12:26:21.000000 baltic-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-12 12:26:30.930565 baltic-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-12 12:26:21.000000 baltic-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.926565 baltic-0.2.1/baltic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 12:26:21.000000 baltic-0.2.1/baltic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77244 2023-07-12 12:26:21.000000 baltic-0.2.1/baltic/baltic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-07-12 12:26:21.000000 baltic-0.2.1/baltic/samogitia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.926565 baltic-0.2.1/baltic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:26:30.000000 baltic-0.2.1/baltic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 12:26:21.000000 baltic-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:26:30.930565 baltic-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-12 12:26:21.000000 baltic-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.926565 baltic-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.930565 baltic-0.2.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:26:30.930565 baltic-0.2.1/tests/data/2020-04-13_treetime/
+-rw-r--r--   0 runner    (1001) docker     (123)    73234 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/2020-04-13_treetime/divergence_tree.nexus
+-rw-r--r--   0 runner    (1001) docker     (123)    72774 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/2020-04-13_treetime/timetree.nexus
+-rw-r--r--   0 runner    (1001) docker     (123)   272511 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/MERS.mcc.tree
+-rw-r--r--   0 runner    (1001) docker     (123)   222372 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/miniFluB.mcc.tree
+-rw-r--r--   0 runner    (1001) docker     (123)  2925238 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/zika.fa
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/data/zika.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-12 12:26:21.000000 baltic-0.2.1/tests/testsuite.py
```

### Comparing `baltic-0.2.0/CODE_OF_CONDUCT.md` & `baltic-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/CONTRIBUTING.md` & `baltic-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/LICENSE` & `baltic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/PKG-INFO` & `baltic-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: baltic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lightweight package for analyzing, manipulating and visualizing annotated phylogenetic trees
 Home-page: https://github.com/evogytis/baltic
-Download-URL: https://github.com/evogytis/baltic/archive/v0.2.0.tar.gz
+Download-URL: https://github.com/evogytis/baltic/archive/v0.2.1.tar.gz
 Author: Gytis Dudas
 Author-email: gytisdudas@gmail.com
 License: gpl-3.0
 Keywords: phylogeny,visualization
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `baltic-0.2.0/README.md` & `baltic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/baltic/baltic.py` & `baltic-0.2.1/baltic/baltic.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,72 +788,72 @@
         if zorder==None: zorder=4
         for k in filter(target,self.Objects):
             x,y=x_attr(k),y_attr(k)
             z=zorder
             ax.text(x,y,text(k),zorder=z,**kwargs)
         return ax
 
-def addTextUnrooted(self,ax,target=None,rotation=None,x_attr=None,y_attr=None,text=None,zorder=None,**kwargs):
-    if target==None: target=lambda k: k.is_leaf()
-    if rotation==None: rotation=lambda k: 0.0
-    if x_attr==None: x_attr=lambda k: k.x
-    if y_attr==None: y_attr=lambda k: k.y
-    if text==None: text=lambda k: k.name
-    if zorder==None: zorder=4
-    
-    for k in filter(target,self.Objects):
-        local_kwargs=dict(kwargs)
-        
-        x,y=x_attr(k),y_attr(k)
-        z=zorder
-        
-        assert 'tau' in k.traits, 'Branch does not have angle tau computed by drawUnrooted().'
-        rot=np.rad2deg(k.traits['tau'])%360
-        
-        if 'horizontalalignment' not in local_kwargs: local_kwargs['horizontalalignment']='right' if 90<rot<270 else 'left'
-        if 'verticalalignment' not in local_kwargs: local_kwargs['verticalalignment']='center'
-        
-        rot=rot+180 if 90<rot<270 else rot
-        
-        ax.text(x,y,text(k),rotation=rot,rotation_mode='anchor',zorder=z,**local_kwargs)
+    def addTextUnrooted(self,ax,target=None,rotation=None,x_attr=None,y_attr=None,text=None,zorder=None,**kwargs):
+        if target==None: target=lambda k: k.is_leaf()
+        if rotation==None: rotation=lambda k: 0.0
+        if x_attr==None: x_attr=lambda k: k.x
+        if y_attr==None: y_attr=lambda k: k.y
+        if text==None: text=lambda k: k.name
+        if zorder==None: zorder=4
         
-    return ax
+        for k in filter(target,self.Objects):
+            local_kwargs=dict(kwargs)
+            
+            x,y=x_attr(k),y_attr(k)
+            z=zorder
+            
+            assert 'tau' in k.traits, 'Branch does not have angle tau computed by drawUnrooted().'
+            rot=np.rad2deg(k.traits['tau'])%360
+            
+            if 'horizontalalignment' not in local_kwargs: local_kwargs['horizontalalignment']='right' if 90<rot<270 else 'left'
+            if 'verticalalignment' not in local_kwargs: local_kwargs['verticalalignment']='center'
+            
+            rot=rot+180 if 90<rot<270 else rot
+            
+            ax.text(x,y,text(k),rotation=rot,rotation_mode='anchor',zorder=z,**local_kwargs)
+            
+        return ax
 
-def addTextCircular(self,ax,target=None,text=None,x_attr=None,y_attr=None,circStart=0.0,circFrac=1.0,inwardSpace=0.0,normaliseHeight=None,zorder=None,**kwargs):
-    if target==None: target=lambda k: k.is_leaf()
-    if x_attr==None: x_attr=lambda k:k.x
-    if y_attr==None: y_attr=lambda k:k.y
-    if text==None: text=lambda k: k.name
-    if zorder==None: zorder=4
-    
-    circ_s=circStart*math.pi*2
-    circ=circFrac*math.pi*2
-    
-    allXs=list(map(x_attr,self.Objects))
-    if normaliseHeight==None: normaliseHeight=lambda value: (value-min(allXs))/(max(allXs)-min(allXs))
-        
-    for k in filter(target,self.Objects): ## iterate over branches
-        local_kwargs=dict(kwargs) ## copy global kwargs into a local version
-        
-        x=normaliseHeight(x_attr(k)+inwardSpace) ## get branch x position
-        y=y_attr(k) ## get y position
-        
-        y=circ_s+circ*y/self.ySpan
-        X=math.sin(y)
-        Y=math.cos(y)
+    def addTextCircular(self,ax,target=None,text=None,x_attr=None,y_attr=None,circStart=0.0,circFrac=1.0,inwardSpace=0.0,normaliseHeight=None,zorder=None,**kwargs):
+        if target==None: target=lambda k: k.is_leaf()
+        if x_attr==None: x_attr=lambda k:k.x
+        if y_attr==None: y_attr=lambda k:k.y
+        if text==None: text=lambda k: k.name
+        if zorder==None: zorder=4
         
-        rot=np.rad2deg(y)%360
+        circ_s=circStart*math.pi*2
+        circ=circFrac*math.pi*2
         
-        if 'horizontalalignment' not in local_kwargs: local_kwargs['horizontalalignment']='right' if 180<rot<360 else 'left' ## rotate labels to aid readability
-        if 'verticalalignment' not in local_kwargs: local_kwargs['verticalalignment']='center'
-        rot=360-rot-90 if 180<rot<360 else 360-rot+90
+        allXs=list(map(x_attr,self.Objects))
+        if normaliseHeight==None: normaliseHeight=lambda value: (value-min(allXs))/(max(allXs)-min(allXs))
+            
+        for k in filter(target,self.Objects): ## iterate over branches
+            local_kwargs=dict(kwargs) ## copy global kwargs into a local version
+            
+            x=normaliseHeight(x_attr(k)+inwardSpace) ## get branch x position
+            y=y_attr(k) ## get y position
+            
+            y=circ_s+circ*y/self.ySpan
+            X=math.sin(y)
+            Y=math.cos(y)
+            
+            rot=np.rad2deg(y)%360
+            
+            if 'horizontalalignment' not in local_kwargs: local_kwargs['horizontalalignment']='right' if 180<rot<360 else 'left' ## rotate labels to aid readability
+            if 'verticalalignment' not in local_kwargs: local_kwargs['verticalalignment']='center'
+            rot=360-rot-90 if 180<rot<360 else 360-rot+90
+            
+            ax.text(X*x,Y*x,text(k),rotation=rot,rotation_mode='anchor',zorder=zorder,**local_kwargs)
         
-        ax.text(X*x,Y*x,text(k),rotation=rot,rotation_mode='anchor',zorder=zorder,**local_kwargs)
-    
-    return ax
+        return ax
 
     def plotPoints(self,ax,x_attr=None,y_attr=None,target=None,size=None,colour=None,
                zorder=None,outline=None,outline_size=None,outline_colour=None,**kwargs):
         if target==None: target=lambda k: k.is_leaf()
         if x_attr==None: x_attr=lambda k:k.x
         if y_attr==None: y_attr=lambda k:k.y
         if size==None: size=40
```

### Comparing `baltic-0.2.0/baltic/samogitia.py` & `baltic-0.2.1/baltic/samogitia.py`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/baltic.egg-info/PKG-INFO` & `baltic-0.2.1/baltic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: baltic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lightweight package for analyzing, manipulating and visualizing annotated phylogenetic trees
 Home-page: https://github.com/evogytis/baltic
-Download-URL: https://github.com/evogytis/baltic/archive/v0.2.0.tar.gz
+Download-URL: https://github.com/evogytis/baltic/archive/v0.2.1.tar.gz
 Author: Gytis Dudas
 Author-email: gytisdudas@gmail.com
 License: gpl-3.0
 Keywords: phylogeny,visualization
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `baltic-0.2.0/baltic.egg-info/SOURCES.txt` & `baltic-0.2.1/baltic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/setup.py` & `baltic-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     long_description = fh.read().decode()
 
 with open("requirements.txt") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="baltic",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     url="https://github.com/evogytis/baltic",
-    download_url="https://github.com/evogytis/baltic/archive/v0.2.0.tar.gz",
+    download_url="https://github.com/evogytis/baltic/archive/v0.2.1.tar.gz",
     keywords = ['phylogeny', 'visualization'],
     license="gpl-3.0",
     author="Gytis Dudas",
     author_email="gytisdudas@gmail.com",
     description="Lightweight package for analyzing, manipulating and visualizing annotated phylogenetic trees",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `baltic-0.2.0/tests/data/2020-04-13_treetime/divergence_tree.nexus` & `baltic-0.2.1/tests/data/2020-04-13_treetime/divergence_tree.nexus`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/data/2020-04-13_treetime/timetree.nexus` & `baltic-0.2.1/tests/data/2020-04-13_treetime/timetree.nexus`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/data/MERS.mcc.tree` & `baltic-0.2.1/tests/data/MERS.mcc.tree`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/data/miniFluB.mcc.tree` & `baltic-0.2.1/tests/data/miniFluB.mcc.tree`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/data/zika.fa` & `baltic-0.2.1/tests/data/zika.fa`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/data/zika.nwk` & `baltic-0.2.1/tests/data/zika.nwk`

 * *Files identical despite different names*

### Comparing `baltic-0.2.0/tests/testsuite.py` & `baltic-0.2.1/tests/testsuite.py`

 * *Files identical despite different names*

