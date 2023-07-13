# Comparing `tmp/voila-vuetify-template-tuwien-0.6.3.tar.gz` & `tmp/voila-vuetify-template-tuwien-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-template-tuwien-0.6.3.tar", last modified: Wed Jul 12 09:00:04 2023, max compression
+gzip compressed data, was "voila-vuetify-template-tuwien-0.6.4.tar", last modified: Thu Jul 13 09:36:12 2023, max compression
```

## Comparing `voila-vuetify-template-tuwien-0.6.3.tar` & `voila-vuetify-template-tuwien-0.6.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/LICENSE
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/MANIFEST.in
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      720 2023-07-12 07:59:22.000000 voila-vuetify-template-tuwien-0.6.3/README.md
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      135 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/setup.cfg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3311 2023-07-12 08:59:48.000000 voila-vuetify-template-tuwien-0.6.3/setup.py
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.532693 voila-vuetify-template-tuwien-0.6.3/share/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.532693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.528693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.528693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     5881 2023-07-12 08:58:38.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)    15256 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   174112 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   141851 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   181109 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.532693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.532693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3141 2023-07-11 11:40:37.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/base.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1766 2023-07-12 07:33:53.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1473 2023-07-11 11:40:00.000000 voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/tree.html
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-12 09:00:04.536693 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-12 09:00:04.000000 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1300 2023-07-12 09:00:04.000000 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-12 09:00:04.000000 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-12 09:00:04.000000 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/requires.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        8 2023-07-12 09:00:04.000000 voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.775907 voila-vuetify-template-tuwien-0.6.4/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/LICENSE
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/MANIFEST.in
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-13 09:36:12.775907 voila-vuetify-template-tuwien-0.6.4/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      720 2023-07-12 07:59:22.000000 voila-vuetify-template-tuwien-0.6.4/README.md
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      135 2023-07-13 09:36:12.775907 voila-vuetify-template-tuwien-0.6.4/setup.cfg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3311 2023-07-13 09:36:03.000000 voila-vuetify-template-tuwien-0.6.4/setup.py
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.759907 voila-vuetify-template-tuwien-0.6.4/share/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.759907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.755907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.759907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.767907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3179 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.771907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     5874 2023-07-13 09:35:11.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-07-11 09:54:42.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.771907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)    15256 2023-07-13 09:32:12.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   174112 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   141851 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)   181109 2023-07-11 11:41:15.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.759907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.759907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.771907 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3141 2023-07-11 11:40:37.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/base.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1766 2023-07-12 07:33:53.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1473 2023-07-11 11:40:00.000000 voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/tree.html
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-07-13 09:36:12.775907 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      298 2023-07-13 09:36:12.000000 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1300 2023-07-13 09:36:12.000000 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-07-13 09:36:12.000000 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       18 2023-07-13 09:36:12.000000 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        8 2023-07-13 09:36:12.000000 voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/top_level.txt
```

### Comparing `voila-vuetify-template-tuwien-0.6.3/LICENSE` & `voila-vuetify-template-tuwien-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/README.md` & `voila-vuetify-template-tuwien-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/setup.py` & `voila-vuetify-template-tuwien-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-template-tuwien',
-    version="0.6.3",
+    version="0.6.4",
     description="A TU Wien vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.0,<0.5'],
     include_package_data=True,
     url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-vuetify-tu-wien-template',
     keywords=[
         'ipython',
```

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             <v-layout v-show="!loading">
                 <v-navigation-drawer v-model="showNavBar" app>
                     <v-toolbar flat>
                         <v-list>
                             <v-list-item>
                                <v-list-item-title class="title">
                                     <jupyter-widget-mount-point mount-id="content-title" style="color: #006699;">
-                                        TU Wien VoilàVuetify
+                                        TU Wien Voilà
                                     </jupyter-widget-mount-point>
                                </v-list-item-title>
                             </v-list-item>
                         </v-list>
                     </v-toolbar>
 
                     <v-divider></v-divider>
```

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/TU_logo.svg`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/icons_font.ttf`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.css`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/nbconvert/templates/vuetify-default-tuwien/static/materialize.min.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/base.html` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/base.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/jupyter/voila/templates/vuetify-base-tuwien/tree.html` & `voila-vuetify-template-tuwien-0.6.4/share/jupyter/voila/templates/vuetify-base-tuwien/tree.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-template-tuwien-0.6.3/share/voila_vuetify_template_tuwien.egg-info/SOURCES.txt` & `voila-vuetify-template-tuwien-0.6.4/share/voila_vuetify_template_tuwien.egg-info/SOURCES.txt`

 * *Files identical despite different names*

