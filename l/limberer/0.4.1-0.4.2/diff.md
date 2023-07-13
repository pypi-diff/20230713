# Comparing `tmp/limberer-0.4.1.tar.gz` & `tmp/limberer-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.4.1.tar", last modified: Thu Jul 13 08:46:50 2023, max compression
+gzip compressed data, was "limberer-0.4.2.tar", last modified: Thu Jul 13 08:54:04 2023, max compression
```

## Comparing `limberer-0.4.1.tar` & `limberer-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.351646 limberer-0.4.1/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.4.1/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.4.1/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.4.1/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11559 2023-07-13 08:46:50.351646 limberer-0.4.1/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9497 2023-07-13 08:45:15.000000 limberer-0.4.1/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-13 08:33:51.000000 limberer-0.4.1/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-13 08:46:50.351646 limberer-0.4.1/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    14025 2023-07-13 08:32:00.000000 limberer-0.4.1/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6970 2023-07-13 01:06:50.000000 limberer-0.4.1/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-13 08:39:37.000000 limberer-0.4.1/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.4.1/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.4.1/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.4.1/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.4.1/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      380 2023-07-13 08:31:33.000000 limberer-0.4.1/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     4162 2023-07-13 01:19:44.000000 limberer-0.4.1/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.4.1/src/limberer/static/sections/example2.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       21 2023-07-13 08:31:10.000000 limberer-0.4.1/src/limberer/static/sections/example3.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.351646 limberer-0.4.1/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.4.1/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.4.1/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.4.1/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.4.1/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:46:50.347646 limberer-0.4.1/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11559 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      816 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-13 08:46:50.000000 limberer-0.4.1/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.206291 limberer-0.4.2/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.4.2/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.4.2/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.4.2/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11555 2023-07-13 08:54:04.206291 limberer-0.4.2/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     9493 2023-07-13 08:49:40.000000 limberer-0.4.2/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-13 08:53:41.000000 limberer-0.4.2/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-13 08:54:04.206291 limberer-0.4.2/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    14025 2023-07-13 08:32:00.000000 limberer-0.4.2/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6970 2023-07-13 01:06:50.000000 limberer-0.4.2/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-13 08:39:37.000000 limberer-0.4.2/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.4.2/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.4.2/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.4.2/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.4.2/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      380 2023-07-13 08:31:33.000000 limberer-0.4.2/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     4168 2023-07-13 08:53:35.000000 limberer-0.4.2/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.4.2/src/limberer/static/sections/example2.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       21 2023-07-13 08:31:10.000000 limberer-0.4.2/src/limberer/static/sections/example3.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.4.2/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.4.2/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.4.2/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.4.2/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11555 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      816 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.4.1/LICENSE` & `limberer-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/PKG-INFO` & `limberer-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.4.1
+Version: 0.4.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -184,15 +184,15 @@
 
 * `toc_header_level`: Header level limit to use for table of contents entry
   generation.
 * `columns`: Whether or not to use the 2-column format for the section.
 * `title`: Section title for 2-column format.
 * `classes`: List of HTML class names to apply to the section (`<article>`)
 
-Additionally, `"cont" = true` may be passed in a `"type" = "section"` section
+Additionally, `cont = true` may be passed in a `type = "section"` section
 entry within the project TOML to specify that the section's Markdown should be
 directly concatenated instead of being handled as a full section. This is
 occasionally useful for managing large single sections that are not intended to
 be divided across multiple `<article>` elements within the underlying HTML.
 
 #### Tables
```

### Comparing `limberer-0.4.1/README.md` & `limberer-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
 * `toc_header_level`: Header level limit to use for table of contents entry
   generation.
 * `columns`: Whether or not to use the 2-column format for the section.
 * `title`: Section title for 2-column format.
 * `classes`: List of HTML class names to apply to the section (`<article>`)
 
-Additionally, `"cont" = true` may be passed in a `"type" = "section"` section
+Additionally, `cont = true` may be passed in a `type = "section"` section
 entry within the project TOML to specify that the section's Markdown should be
 directly concatenated instead of being handled as a full section. This is
 occasionally useful for managing large single sections that are not intended to
 be divided across multiple `<article>` elements within the underlying HTML.
 
 #### Tables
```

### Comparing `limberer-0.4.1/pyproject.toml` & `limberer-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.4.1/src/limberer/__init__.py` & `limberer-0.4.2/src/limberer/__init__.py`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/pf.py` & `limberer-0.4.2/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/assets/core.css` & `limberer-0.4.2/src/limberer/static/assets/core.css`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/assets/logo.svg` & `limberer-0.4.2/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/assets/style.css` & `limberer-0.4.2/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/images/test1.jpg` & `limberer-0.4.2/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/sections/example.md` & `limberer-0.4.2/src/limberer/static/sections/example.md`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     </tr>
     <tr>
       <td><ol><li>Table list</li><li>foo</li></ol></td><td></td><td></td><td></td>
     </tr>
   </tbody>
 </table>
 
+<br>
+
 | First Header  | Second Header |
 | ------------- | ------------- |
 | Content Cell  | Content Cell  |
 | Content Cell  | Content Cell  |
 
 # Image Test
```

#### html2text {}

```diff
@@ -19,14 +19,15 @@
    2. foo
    1. Table list
    2. foo
    1. Table list
    2. foo
    1. Table list
    2. foo
+
 | First Header | Second Header | | ------------- | ------------- | | Content
 Cell | Content Cell | | Content Cell | Content Cell | # Image Test ![](./
 images/test1.jpg){style="width: 30%; margin: auto; display: block;"} Hello
 world. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
 tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
 quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
 consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
```

### Comparing `limberer-0.4.1/src/limberer/static/sections/example2.md` & `limberer-0.4.2/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/templates/cover.html` & `limberer-0.4.2/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer/static/templates/toc.html` & `limberer-0.4.2/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.4.1/src/limberer.egg-info/PKG-INFO` & `limberer-0.4.2/src/limberer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.4.1
+Version: 0.4.2
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -184,15 +184,15 @@
 
 * `toc_header_level`: Header level limit to use for table of contents entry
   generation.
 * `columns`: Whether or not to use the 2-column format for the section.
 * `title`: Section title for 2-column format.
 * `classes`: List of HTML class names to apply to the section (`<article>`)
 
-Additionally, `"cont" = true` may be passed in a `"type" = "section"` section
+Additionally, `cont = true` may be passed in a `type = "section"` section
 entry within the project TOML to specify that the section's Markdown should be
 directly concatenated instead of being handled as a full section. This is
 occasionally useful for managing large single sections that are not intended to
 be divided across multiple `<article>` elements within the underlying HTML.
 
 #### Tables
```

### Comparing `limberer-0.4.1/src/limberer.egg-info/SOURCES.txt` & `limberer-0.4.2/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

