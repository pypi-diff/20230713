# Comparing `tmp/uiweb-0.7.0.tar.gz` & `tmp/uiweb-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiweb-0.7.0.tar", last modified: Wed Feb 15 07:12:06 2023, max compression
+gzip compressed data, was "uiweb-0.7.5.tar", last modified: Thu Jul 13 08:37:57 2023, max compression
```

## Comparing `uiweb-0.7.0.tar` & `uiweb-0.7.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 07:12:06.550907 uiweb-0.7.0/
--rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 uiweb-0.7.0/LICENSE
--rw-rw-rw-   0        0        0      715 2023-02-15 07:12:06.549911 uiweb-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-12-05 10:28:28.000000 uiweb-0.7.0/README.MD
--rw-rw-rw-   0        0        0      701 2023-02-15 07:07:27.000000 uiweb-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-15 07:12:06.550907 uiweb-0.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-15 07:12:06.517814 uiweb-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-15 07:12:06.531777 uiweb-0.7.0/src/uiweb/
--rw-rw-rw-   0        0        0       87 2022-12-05 16:31:22.000000 uiweb-0.7.0/src/uiweb/__init__.py
--rw-rw-rw-   0        0        0   122837 2022-12-30 09:40:59.000000 uiweb-0.7.0/src/uiweb/uiweb.py
--rw-rw-rw-   0        0        0   101836 2022-12-19 13:55:10.000000 uiweb-0.7.0/src/uiweb/uiweb_.py
-drwxrwxrwx   0        0        0        0 2023-02-15 07:12:06.548941 uiweb-0.7.0/src/uiweb.egg-info/
--rw-rw-rw-   0        0        0      715 2023-02-15 07:12:06.000000 uiweb-0.7.0/src/uiweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-02-15 07:12:06.000000 uiweb-0.7.0/src/uiweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 07:12:06.000000 uiweb-0.7.0/src/uiweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-02-15 07:12:06.000000 uiweb-0.7.0/src/uiweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-15 07:12:06.000000 uiweb-0.7.0/src/uiweb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 08:37:57.794412 uiweb-0.7.5/
+-rw-rw-rw-   0        0        0    35162 2022-12-05 10:38:56.000000 uiweb-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0      715 2023-07-13 08:37:57.794412 uiweb-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2022-12-05 10:28:28.000000 uiweb-0.7.5/README.MD
+-rw-rw-rw-   0        0        0      701 2023-07-13 08:37:37.000000 uiweb-0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 08:37:57.794412 uiweb-0.7.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 08:37:57.772471 uiweb-0.7.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 08:37:57.782444 uiweb-0.7.5/src/uiweb/
+-rw-rw-rw-   0        0        0       87 2023-07-13 08:34:35.000000 uiweb-0.7.5/src/uiweb/__init__.py
+-rw-rw-rw-   0        0        0   122837 2022-12-30 09:40:59.000000 uiweb-0.7.5/src/uiweb/uiweb.py
+-rw-rw-rw-   0        0        0   102572 2023-07-13 07:58:52.000000 uiweb-0.7.5/src/uiweb/uiweb_.py
+drwxrwxrwx   0        0        0        0 2023-07-13 08:37:57.793415 uiweb-0.7.5/src/uiweb.egg-info/
+-rw-rw-rw-   0        0        0      715 2023-07-13 08:37:57.000000 uiweb-0.7.5/src/uiweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-07-13 08:37:57.000000 uiweb-0.7.5/src/uiweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 08:37:57.000000 uiweb-0.7.5/src/uiweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-13 08:37:57.000000 uiweb-0.7.5/src/uiweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 08:37:57.000000 uiweb-0.7.5/src/uiweb.egg-info/top_level.txt
```

### Comparing `uiweb-0.7.0/LICENSE` & `uiweb-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uiweb-0.7.0/PKG-INFO` & `uiweb-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiweb
-Version: 0.7.0
+Version: 0.7.5
 Summary: Simple-based web-app library
 Author-email: Dmitry Vorontsov <dv1555@hotmail.com>
 Project-URL: Homepage, http://simpleui.ru/
 Project-URL: Bug Tracker, https://forum.infostart.ru/forum104/topic211360/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `uiweb-0.7.0/pyproject.toml` & `uiweb-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uiweb"
-version = "0.7.00"
+version = "0.7.05"
 authors = [
   { name="Dmitry Vorontsov", email="dv1555@hotmail.com" },
 ]
 description = "Simple-based web-app library"
 readme = "README.MD"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `uiweb-0.7.0/src/uiweb/uiweb.py` & `uiweb-0.7.5/src/uiweb/uiweb.py`

 * *Files identical despite different names*

### Comparing `uiweb-0.7.0/src/uiweb/uiweb_.py` & `uiweb-0.7.5/src/uiweb/uiweb_.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,15 +602,14 @@
           else:    
               return "Variable has not been initialized :"+var
 
     else:
         return val 
 
 
-
   def get_layouts(self,soup,root,level,var_prefix='',localData=None):
     
     
     currentcontainer = bs4.BeautifulSoup(features="lxml")
     
 
     for elem in root['Elements']:
@@ -663,16 +662,16 @@
 
                 if "width" in elem:
                       if str(elem.get("width","")).isnumeric():
                         styles.append("flex:"+str(elem.get("width"))+"px;")
                       elif  elem.get("width","")=="match_parent":
                         if str(elem.get("weight",""))=="0":
                           styles.append("flex:1;") 
-                        elif len(elem.get("weight",""))>0:  
-                          styles.append("flex:"+elem.get("weight","")+";")
+                        elif len(str(elem.get("weight","")))>0:  
+                          styles.append("flex:"+str(elem.get("weight",""))+";")
                         
                 if "height" in elem:
                     if str(elem.get("height","")).isnumeric():
                       styles.append("height:"+str(elem.get("height"))+"px;")
                     elif  elem.get("height","")=="match_parent":
                       styles.append("height:100%;")        
               else:
@@ -695,16 +694,16 @@
 
                 if "height" in elem:
                       if str(elem.get("height","")).isnumeric():
                         styles.append("flex:"+str(elem.get("height"))+"px;")
                       elif  elem.get("height","")=="match_parent":
                         if str(elem.get("weight",""))=="0":
                           styles.append("flex:1;") 
-                        elif len(elem.get("weight",""))>0:  
-                          styles.append("flex:"+elem.get("weight","")+";") 
+                        elif len(str(elem.get("weight","")))>0:  
+                          styles.append("flex:"+str(elem.get("weight",""))+";") 
                 if "width" in elem:
                     if str(elem.get("width","")).isnumeric():
                       styles.append("width:"+str(elem.get("width"))+"px;")
                     elif  elem.get("width","")=="match_parent":
                       styles.append("width:100%;")        
 
             if elem.get('type')=='Tab':        
@@ -800,28 +799,28 @@
             if elem.get('type')=='EditTextText':
 
                 
                 #new_form = soup.new_tag("form", method="post", action="/oninput/")  
                 
                 new_element = soup.new_tag("input", id=tvkey,type="text",style=get_decor(elem))
                 if len(elem.get("Value",''))>0:
-                  new_element = soup.new_tag("input", id=tvkey,type="text",value = self.calculateField(elem.get("Value"),localData))
+                  new_element = soup.new_tag("input", id=tvkey,type="text",value = self.calculateField(elem.get("Value"),localData),style=get_decor(elem))
                   
                 
                 #new_form.append(new_element)
                 currentcontainer.append(new_element)
 
             if elem.get('type')=='EditTextAuto':
 
                 
                 #new_form = soup.new_tag("form", method="post", action="/oninput/")  
                 
                 new_element = soup.new_tag("input", id=tvkey,type="text",style=get_decor(elem), **{'class':'autotext'})
                 if len(elem.get("Value",''))>0:
-                  new_element = soup.new_tag("input", id=tvkey,type="text",value = self.calculateField(elem.get("Value"),localData), **{'class':'autotext'})
+                  new_element = soup.new_tag("input", id=tvkey,type="text",value = self.calculateField(elem.get("Value"),localData), **{'class':'autotext'},style=get_decor(elem))
                   
                 if 'style_class' in elem:
                     new_element['class'] = new_element.get('class', []) + [elem.get('style_class')]
                     
                   
                 #new_form.append(new_element)
                 currentcontainer.append(new_element)
@@ -843,15 +842,15 @@
 
                     step+="1"  
                     placeholder+="0"
 
                 
                 new_element = soup.new_tag("input", id=tvkey,type="number",style=get_decor(elem), onkeypress="return isNumberKey(event)",step=step,placeholder=placeholder)
                 if len(elem.get("Value",''))>0:
-                  new_element = soup.new_tag("input", id=tvkey,type="number",value = self.calculateField(elem.get("Value"),localData),step=step,placeholder=placeholder)
+                  new_element = soup.new_tag("input", id=tvkey,type="number",value = self.calculateField(elem.get("Value"),localData),step=step,placeholder=placeholder,style=get_decor(elem))
                   
                 if 'style_class' in elem:
                     new_element['class'] = new_element.get('class', []) + [elem.get('style_class')]
                     
                   
                 
                 currentcontainer.append(new_element)    
@@ -859,15 +858,15 @@
             if elem.get('type')=='EditTextPass':
 
                 
                 #new_form = soup.new_tag("form", method="post", action="/oninput/")  
                 
                 new_element = soup.new_tag("input", id=tvkey,type="password",style=get_decor(elem))
                 if len(elem.get("Value",''))>0:
-                  new_element = soup.new_tag("input", id=tvkey,type="password",value = self.calculateField(elem.get("Value"),localData))
+                  new_element = soup.new_tag("input", id=tvkey,type="password",value = self.calculateField(elem.get("Value"),localData),style=get_decor(elem))
                   
                 if 'style_class' in elem:
                     new_element['class'] = new_element.get('class', []) + [elem.get('style_class')]
                     
                  
                 
                 #new_form.append(new_element)
@@ -886,23 +885,35 @@
                     new_element['class'] = new_element.get('class', []) + [elem.get('style_class')]
                     
                
 
                 #new_form.append(new_element)
                 currentcontainer.append(new_element)
             
+            if elem.get('type')=='file':
+
+                
+                #new_form = soup.new_tag("form", method="post", action="/oninput/")  
+                
+                new_element = soup.new_tag("input", id=tvkey,type="file",style=get_decor(elem))
+                if len(elem.get("Value",''))>0:
+                  new_element = soup.new_tag("input", id=tvkey,type="file",value = self.calculateField(elem.get("Value"),localData),style=get_decor(elem))
+                  
+                
+                #new_form.append(new_element)
+                currentcontainer.append(new_element)
 
             if elem.get('type')=='DateField':
 
                 
                 #new_form = soup.new_tag("form", method="post", action="/oninput/")  
                 
                 new_element = soup.new_tag("input", id=tvkey,type="date",style=get_decor(elem))
                 if len(elem.get("Value",''))>0:
-                  new_element = soup.new_tag("input", id=tvkey,type="date",value = self.calculateField(elem.get("Value"),localData))
+                  new_element = soup.new_tag("input", id=tvkey,type="date",value = self.calculateField(elem.get("Value"),localData),style=get_decor(elem))
                   
                 if 'style_class' in elem:
                     new_element['class'] = new_element.get('class', []) + [elem.get('style_class')]
                     
                   
                 
                 #new_form.append(new_element)
```

### Comparing `uiweb-0.7.0/src/uiweb.egg-info/PKG-INFO` & `uiweb-0.7.5/src/uiweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiweb
-Version: 0.7.0
+Version: 0.7.5
 Summary: Simple-based web-app library
 Author-email: Dmitry Vorontsov <dv1555@hotmail.com>
 Project-URL: Homepage, http://simpleui.ru/
 Project-URL: Bug Tracker, https://forum.infostart.ru/forum104/topic211360/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

