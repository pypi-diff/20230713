# Comparing `tmp/limberer-0.3.4.tar.gz` & `tmp/limberer-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.3.4.tar", last modified: Thu Jul  6 07:46:23 2023, max compression
+gzip compressed data, was "limberer-0.4.tar", last modified: Thu Jul 13 01:40:16 2023, max compression
```

## Comparing `limberer-0.3.4.tar` & `limberer-0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.3.4/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.3.4/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.3.4/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10029 2023-07-06 07:46:23.220873 limberer-0.3.4/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     7967 2023-07-06 07:44:52.000000 limberer-0.3.4/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-06 07:45:02.000000 limberer-0.3.4/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-06 07:46:23.220873 limberer-0.3.4/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    12757 2023-07-06 07:40:34.000000 limberer-0.3.4/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6752 2023-07-04 03:01:36.000000 limberer-0.3.4/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-06 07:09:08.000000 limberer-0.3.4/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.3.4/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.3.4/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.3.4/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.3.4/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      324 2023-07-06 07:42:27.000000 limberer-0.3.4/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     3887 2023-07-04 03:17:45.000000 limberer-0.3.4/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.3.4/src/limberer/static/sections/example2.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.3.4/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.3.4/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.3.4/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.3.4/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-06 07:46:23.220873 limberer-0.3.4/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    10029 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-06 07:46:23.000000 limberer-0.3.4/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.4/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.4/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.4/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11169 2023-07-13 01:40:16.902598 limberer-0.4/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     9109 2023-07-13 01:39:36.000000 limberer-0.4/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1092 2023-07-13 00:51:20.000000 limberer-0.4/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-13 01:40:16.902598 limberer-0.4/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    13537 2023-07-13 01:34:44.000000 limberer-0.4/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6970 2023-07-13 01:06:50.000000 limberer-0.4/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-06 07:09:08.000000 limberer-0.4/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.4/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.4/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.4/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.4/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      324 2023-07-06 07:42:27.000000 limberer-0.4/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     4162 2023-07-13 01:19:44.000000 limberer-0.4/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.4/src/limberer/static/sections/example2.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.4/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.4/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.4/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.4/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 01:40:16.902598 limberer-0.4/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11169 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      775 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-13 01:40:16.000000 limberer-0.4/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.3.4/LICENSE` & `limberer-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/PKG-INFO` & `limberer-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.4
+Version: 0.4
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -115,15 +115,15 @@
 `section` template will be used to write document content. For such
 `type = "section"` sections, the content will be sourced from a (currently)
 Markdown file based on the section `name` value (`sections/<name>.md`). By
 default, sections will be rendered against the `template/section.html`
 template, but the template used can be changed via an `alt = "othertemplate"`
 section list setting.
 
-### Project TOML
+### Project TOML Example
 
 ```toml
 title = "Example Document"
 subheading = "..."
 #globaloption=value
 #...
 
@@ -137,14 +137,22 @@
   { type = "toc" },
   { name = "example", type = "section" },
   { name = "example2", type = "section", sectionoption = "value" },
   ...
 ]
 ```
 
+Additional or overriding settings or Mustache template variables can be
+configured by passing additional TOML file paths into the `limberer build`
+command:
+
+```
+$ limberer build report.toml stats.toml
+```
+
 ### Section Templates
 
 Out of the box, `limberer` comes with some initial section templates:
 
 * `cover`: A title page section.
 * `toc`: A table of contents section.
 * `section`: The underlying template for custom sections.
@@ -154,16 +162,17 @@
 * `appendix_start`: Subsequent sections will be treated as appendices.
 * `appendix_end`: Disables the above setting; subsequent sections are not
   treated as appendices. The appendix counter will not be cleared.
 
 ### Custom Sections
 
 Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
-where most document content is written. A section can begin with a block of
-Markdown metadata:
+with support for Mustache expressions (using the TOML configuration), where
+most document content is written. A section can begin with a block of Markdown
+metadata:
 
 ```markdown
 ---
 toc_header_level: 2
 columns: true
 title: Example3
 classes: foo bar baz
@@ -304,14 +313,45 @@
 * `.xrefpg`: This will add a " on page XX".
 
   ```
   * <a class="xrefn xrefpg" href="#example2-aaah2"></a>
   * [](#example2-aaah2){.xrefn .xrefpg}
   ```
 
+#### Code Blocks
+
+
+````markdown
+```js
+let j = await fetch("https://wat.wat", {
+  "headers": {
+    "x-test": "foo"
+  }
+}).then((res)=>res.json());
+```
+<center>Example Snippet of Code</center>
+
+```js
+let j = await fetch("https://wat.wat", {
+  "headers": {
+    "x-test": "foo"
+  }
+}).then((res)=>res.json());
+```
+<figure><figcaption>Example Snippet of Code with a figure prefix</figcaption></figure>
+````
+
+The following settings can be configured in the project TOML:
+
+* `highlight` (defaults to `"molokai"`)
+* `highlight_plaintext` (defaults to `"solarized-dark"`)
+* `highlight_font` (defaults to `"'DejaVu Sans Mono', monospace"`)
+* `highlight_style` (defaults to `"padding: 1rem; border-radius: 2px; overflow-x: auto;"`
+* `highlight_line_length` (defaults to `"74"`)
+
 #### Breaks
 
 The following can be added to force a break.
 
 ```html
 <div class="pagebreak"></div>
 ```
@@ -342,14 +382,17 @@
 convenience, the CSS is organized as `core`, `style`, and `custom`. The intent
 is for the `assets/core.css` to cover the main layout and functioning of the
 document, the `assets/style.css` to cover group theming for consistency, and
 `custom/custom.css` to be for any per-document/project styling.
 
 ## Todo List
 
+* Support for custom Mustache-generated CSS
+* Redo contiguous sections
+* Better footnotes
 * Draft builds
 * Partial builds of individual sections
 * Support for non-Markdown sections
 
 ## FAQ
 
 > Why?
```

### Comparing `limberer-0.3.4/README.md` & `limberer-0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -124,375 +124,447 @@
 000007b0: 6174 652c 2062 7574 2074 6865 2074 656d  ate, but the tem
 000007c0: 706c 6174 6520 7573 6564 2063 616e 2062  plate used can b
 000007d0: 6520 6368 616e 6765 6420 7669 6120 616e  e changed via an
 000007e0: 2060 616c 7420 3d20 226f 7468 6572 7465   `alt = "otherte
 000007f0: 6d70 6c61 7465 2260 0a73 6563 7469 6f6e  mplate"`.section
 00000800: 206c 6973 7420 7365 7474 696e 672e 0a0a   list setting...
 00000810: 2323 2320 5072 6f6a 6563 7420 544f 4d4c  ### Project TOML
-00000820: 0a0a 6060 6074 6f6d 6c0a 7469 746c 6520  ..```toml.title 
-00000830: 3d20 2245 7861 6d70 6c65 2044 6f63 756d  = "Example Docum
-00000840: 656e 7422 0a73 7562 6865 6164 696e 6720  ent".subheading 
-00000850: 3d20 222e 2e2e 220a 2367 6c6f 6261 6c6f  = "...".#globalo
-00000860: 7074 696f 6e3d 7661 6c75 650a 232e 2e2e  ption=value.#...
-00000870: 0a0a 6175 7468 6f72 7320 3d20 5b0a 2020  ..authors = [.  
-00000880: 7b20 6e61 6d65 203d 2022 4578 616d 706c  { name = "Exampl
-00000890: 6520 5065 7273 6f6e 222c 2065 6d61 696c  e Person", email
-000008a0: 203d 2022 6578 616d 706c 6540 6578 616d   = "example@exam
-000008b0: 706c 652e 636f 6d22 207d 2c0a 2020 2e2e  ple.com" },.  ..
-000008c0: 2e0a 5d0a 0a73 6563 7469 6f6e 7320 3d20  ..]..sections = 
-000008d0: 5b0a 2020 7b20 7479 7065 203d 2022 636f  [.  { type = "co
-000008e0: 7665 7222 207d 2c0a 2020 7b20 7479 7065  ver" },.  { type
-000008f0: 203d 2022 746f 6322 207d 2c0a 2020 7b20   = "toc" },.  { 
-00000900: 6e61 6d65 203d 2022 6578 616d 706c 6522  name = "example"
-00000910: 2c20 7479 7065 203d 2022 7365 6374 696f  , type = "sectio
-00000920: 6e22 207d 2c0a 2020 7b20 6e61 6d65 203d  n" },.  { name =
-00000930: 2022 6578 616d 706c 6532 222c 2074 7970   "example2", typ
-00000940: 6520 3d20 2273 6563 7469 6f6e 222c 2073  e = "section", s
-00000950: 6563 7469 6f6e 6f70 7469 6f6e 203d 2022  ectionoption = "
-00000960: 7661 6c75 6522 207d 2c0a 2020 2e2e 2e0a  value" },.  ....
-00000970: 5d0a 6060 600a 0a23 2323 2053 6563 7469  ].```..### Secti
-00000980: 6f6e 2054 656d 706c 6174 6573 0a0a 4f75  on Templates..Ou
-00000990: 7420 6f66 2074 6865 2062 6f78 2c20 606c  t of the box, `l
-000009a0: 696d 6265 7265 7260 2063 6f6d 6573 2077  imberer` comes w
-000009b0: 6974 6820 736f 6d65 2069 6e69 7469 616c  ith some initial
-000009c0: 2073 6563 7469 6f6e 2074 656d 706c 6174   section templat
-000009d0: 6573 3a0a 0a2a 2060 636f 7665 7260 3a20  es:..* `cover`: 
-000009e0: 4120 7469 746c 6520 7061 6765 2073 6563  A title page sec
-000009f0: 7469 6f6e 2e0a 2a20 6074 6f63 603a 2041  tion..* `toc`: A
-00000a00: 2074 6162 6c65 206f 6620 636f 6e74 656e   table of conten
-00000a10: 7473 2073 6563 7469 6f6e 2e0a 2a20 6073  ts section..* `s
-00000a20: 6563 7469 6f6e 603a 2054 6865 2075 6e64  ection`: The und
-00000a30: 6572 6c79 696e 6720 7465 6d70 6c61 7465  erlying template
-00000a40: 2066 6f72 2063 7573 746f 6d20 7365 6374   for custom sect
-00000a50: 696f 6e73 2e0a 0a41 6464 6974 696f 6e61  ions...Additiona
-00000a60: 6c6c 792c 2060 6c69 6d62 6572 6572 6020  lly, `limberer` 
-00000a70: 7375 7070 6f72 7473 2074 6865 2066 6f6c  supports the fol
-00000a80: 6c6f 7769 6e67 2074 656d 706c 6174 652d  lowing template-
-00000a90: 6c69 6b65 2070 7365 7564 6f2d 7365 6374  like pseudo-sect
-00000aa0: 696f 6e73 3a0a 0a2a 2060 6170 7065 6e64  ions:..* `append
-00000ab0: 6978 5f73 7461 7274 603a 2053 7562 7365  ix_start`: Subse
-00000ac0: 7175 656e 7420 7365 6374 696f 6e73 2077  quent sections w
-00000ad0: 696c 6c20 6265 2074 7265 6174 6564 2061  ill be treated a
-00000ae0: 7320 6170 7065 6e64 6963 6573 2e0a 2a20  s appendices..* 
-00000af0: 6061 7070 656e 6469 785f 656e 6460 3a20  `appendix_end`: 
-00000b00: 4469 7361 626c 6573 2074 6865 2061 626f  Disables the abo
-00000b10: 7665 2073 6574 7469 6e67 3b20 7375 6273  ve setting; subs
-00000b20: 6571 7565 6e74 2073 6563 7469 6f6e 7320  equent sections 
-00000b30: 6172 6520 6e6f 740a 2020 7472 6561 7465  are not.  treate
-00000b40: 6420 6173 2061 7070 656e 6469 6365 732e  d as appendices.
-00000b50: 2054 6865 2061 7070 656e 6469 7820 636f   The appendix co
-00000b60: 756e 7465 7220 7769 6c6c 206e 6f74 2062  unter will not b
-00000b70: 6520 636c 6561 7265 642e 0a0a 2323 2320  e cleared...### 
-00000b80: 4375 7374 6f6d 2053 6563 7469 6f6e 730a  Custom Sections.
-00000b90: 0a43 7573 746f 6d20 7365 6374 696f 6e73  .Custom sections
-00000ba0: 2028 2273 6563 7469 6f6e 7322 2920 6172   ("sections") ar
-00000bb0: 6520 6120 6d69 7820 6f66 204d 6172 6b64  e a mix of Markd
-00000bc0: 6f77 6e20 2861 6e64 2c20 696e 2073 6f6d  own (and, in som
-00000bd0: 6520 6361 7365 732c 2048 544d 4c29 2c0a  e cases, HTML),.
-00000be0: 7768 6572 6520 6d6f 7374 2064 6f63 756d  where most docum
-00000bf0: 656e 7420 636f 6e74 656e 7420 6973 2077  ent content is w
-00000c00: 7269 7474 656e 2e20 4120 7365 6374 696f  ritten. A sectio
-00000c10: 6e20 6361 6e20 6265 6769 6e20 7769 7468  n can begin with
-00000c20: 2061 2062 6c6f 636b 206f 660a 4d61 726b   a block of.Mark
-00000c30: 646f 776e 206d 6574 6164 6174 613a 0a0a  down metadata:..
-00000c40: 6060 606d 6172 6b64 6f77 6e0a 2d2d 2d0a  ```markdown.---.
-00000c50: 746f 635f 6865 6164 6572 5f6c 6576 656c  toc_header_level
-00000c60: 3a20 320a 636f 6c75 6d6e 733a 2074 7275  : 2.columns: tru
-00000c70: 650a 7469 746c 653a 2045 7861 6d70 6c65  e.title: Example
-00000c80: 330a 636c 6173 7365 733a 2066 6f6f 2062  3.classes: foo b
-00000c90: 6172 2062 617a 0a2d 2d2d 0a60 6060 0a0a  ar baz.---.```..
-00000ca0: 5468 6520 6d65 7461 6461 7461 206f 7074  The metadata opt
-00000cb0: 696f 6e73 2061 7265 206d 6572 6765 6420  ions are merged 
-00000cc0: 7769 7468 2074 6865 2073 6563 7469 6f6e  with the section
-00000cd0: 2065 6e74 7279 206f 7074 696f 6e73 2e20   entry options. 
-00000ce0: 4375 7272 656e 746c 790a 7375 7070 6f72  Currently.suppor
-00000cf0: 7465 6420 6f70 7469 6f6e 7320 6172 6520  ted options are 
-00000d00: 7468 6520 666f 6c6c 6f77 696e 673a 0a0a  the following:..
-00000d10: 2a20 6074 6f63 5f68 6561 6465 725f 6c65  * `toc_header_le
-00000d20: 7665 6c60 3a20 4865 6164 6572 206c 6576  vel`: Header lev
-00000d30: 656c 206c 696d 6974 2074 6f20 7573 6520  el limit to use 
-00000d40: 666f 7220 7461 626c 6520 6f66 2063 6f6e  for table of con
-00000d50: 7465 6e74 7320 656e 7472 790a 2020 6765  tents entry.  ge
-00000d60: 6e65 7261 7469 6f6e 2e0a 2a20 6063 6f6c  neration..* `col
-00000d70: 756d 6e73 603a 2057 6865 7468 6572 206f  umns`: Whether o
-00000d80: 7220 6e6f 7420 746f 2075 7365 2074 6865  r not to use the
-00000d90: 2032 2d63 6f6c 756d 6e20 666f 726d 6174   2-column format
-00000da0: 2066 6f72 2074 6865 2073 6563 7469 6f6e   for the section
-00000db0: 2e0a 2a20 6074 6974 6c65 603a 2053 6563  ..* `title`: Sec
-00000dc0: 7469 6f6e 2074 6974 6c65 2066 6f72 2032  tion title for 2
-00000dd0: 2d63 6f6c 756d 6e20 666f 726d 6174 2e0a  -column format..
-00000de0: 2a20 6063 6c61 7373 6573 603a 204c 6973  * `classes`: Lis
-00000df0: 7420 6f66 2048 544d 4c20 636c 6173 7320  t of HTML class 
-00000e00: 6e61 6d65 7320 746f 2061 7070 6c79 2074  names to apply t
-00000e10: 6f20 7468 6520 7365 6374 696f 6e20 2860  o the section (`
-00000e20: 3c61 7274 6963 6c65 3e60 290a 0a23 2323  <article>`)..###
-00000e30: 2320 5461 626c 6573 0a0a 5461 626c 6573  # Tables..Tables
-00000e40: 2063 616e 2062 6520 7772 6974 7465 6e20   can be written 
-00000e50: 7573 696e 6720 7468 6520 7069 7065 2d64  using the pipe-d
-00000e60: 656c 696d 6974 6564 2047 6974 4875 622d  elimited GitHub-
-00000e70: 666c 6176 6f72 6564 204d 6172 6b64 6f77  flavored Markdow
-00000e80: 6e0a 636f 6e76 656e 7469 6f6e 2c20 6f72  n.convention, or
-00000e90: 2077 6974 6820 4854 4d4c 2074 6162 6c65   with HTML table
-00000ea0: 732e 0a0a 6060 606d 6172 6b64 6f77 6e0a  s...```markdown.
-00000eb0: 7c20 4669 7273 7420 4865 6164 6572 2020  | First Header  
-00000ec0: 7c20 5365 636f 6e64 2048 6561 6465 7220  | Second Header 
-00000ed0: 7c0a 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.| ------------
-00000ee0: 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  - | ------------
-00000ef0: 2d20 7c0a 7c20 436f 6e74 656e 7420 4365  - |.| Content Ce
-00000f00: 6c6c 2020 7c20 436f 6e74 656e 7420 4365  ll  | Content Ce
-00000f10: 6c6c 2020 7c0a 7c20 436f 6e74 656e 7420  ll  |.| Content 
-00000f20: 4365 6c6c 2020 7c20 436f 6e74 656e 7420  Cell  | Content 
-00000f30: 4365 6c6c 2020 7c0a 6060 600a 0a60 6060  Cell  |.```..```
-00000f40: 6048 544d 4c0a 3c74 6162 6c65 3e0a 2020  `HTML.<table>.  
-00000f50: 3c74 6865 6164 3e0a 2020 2020 3c74 723e  <thead>.    <tr>
-00000f60: 0a20 2020 2020 203c 7468 2073 7479 6c65  .      <th style
-00000f70: 3d22 7769 6474 683a 2032 3025 223e 613c  ="width: 20%">a<
-00000f80: 2f74 683e 0a20 2020 2020 203c 7468 2073  /th>.      <th s
-00000f90: 7479 6c65 3d22 7769 6474 683a 2034 3025  tyle="width: 40%
-00000fa0: 223e 623c 2f74 683e 0a20 2020 2020 203c  ">b</th>.      <
-00000fb0: 7468 3e63 3c2f 7468 3e0a 2020 2020 2020  th>c</th>.      
-00000fc0: 3c74 683e 643c 2f74 683e 0a20 2020 203c  <th>d</th>.    <
-00000fd0: 2f74 723e 0a20 203c 2f74 6865 6164 3e0a  /tr>.  </thead>.
-00000fe0: 2020 3c74 626f 6479 3e0a 2020 2020 3c74    <tbody>.    <t
-00000ff0: 723e 3c74 643e 2a2a 426f 6c64 2a2a 3c2f  r><td>**Bold**</
-00001000: 7464 3e3c 7464 3e5f 6974 616c 6963 5f3c  td><td>_italic_<
-00001010: 2f74 643e 0a3c 7464 3e0a 6060 600a 636f  /td>.<td>.```.co
-00001020: 6465 2062 6c6f 636b 0a60 6060 0a3c 2f74  de block.```.</t
-00001030: 643e 0a3c 7464 3e0a 2a20 6c69 7374 0a2a  d>.<td>.* list.*
-00001040: 206f 660a 2a20 7468 696e 6773 0a3c 2f74   of.* things.</t
-00001050: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-00001060: 203c 7472 3e3c 7464 3e3c 2f74 643e 3c74   <tr><td></td><t
-00001070: 643e 3c2f 7464 3e3c 7464 3e3c 2f74 643e  d></td><td></td>
-00001080: 3c74 643e 3c2f 7464 3e3c 2f74 723e 0a20  <td></td></tr>. 
-00001090: 2020 203c 7472 3e3c 7464 3e3c 2f74 643e     <tr><td></td>
-000010a0: 3c74 643e 3c2f 7464 3e3c 7464 3e3c 2f74  <td></td><td></t
-000010b0: 643e 3c74 643e 3c2f 7464 3e3c 2f74 723e  d><td></td></tr>
-000010c0: 0a20 2020 203c 7472 3e3c 7464 3e3c 2f74  .    <tr><td></t
-000010d0: 643e 3c74 643e 3c2f 7464 3e3c 7464 3e3c  d><td></td><td><
-000010e0: 2f74 643e 3c74 643e 3c2f 7464 3e3c 2f74  /td><td></td></t
-000010f0: 723e 0a20 203c 2f74 626f 6479 3e0a 3c2f  r>.  </tbody>.</
-00001100: 7461 626c 653e 0a60 6060 600a 0a23 2323  table>.````..###
-00001110: 2320 496d 6167 6573 0a0a 4120 7369 6d70  # Images..A simp
-00001120: 6c65 2069 6d61 6765 2063 616e 2062 6520  le image can be 
-00001130: 656d 6265 6464 6564 2077 6974 6820 6375  embedded with cu
-00001140: 7374 6f6d 2043 5353 2074 6f20 706c 6163  stom CSS to plac
-00001150: 652f 7374 796c 6520 6974 3a0a 0a60 6060  e/style it:..```
-00001160: 6d61 726b 646f 776e 0a21 5b5d 282e 2f69  markdown.![](./i
-00001170: 6d61 6765 732f 7465 7374 312e 6a70 6729  mages/test1.jpg)
-00001180: 7b73 7479 6c65 3d22 7769 6474 683a 2033  {style="width: 3
-00001190: 3025 3b20 6d61 7267 696e 3a20 6175 746f  0%; margin: auto
-000011a0: 3b20 6469 7370 6c61 793a 2062 6c6f 636b  ; display: block
-000011b0: 3b22 7d0a 6060 600a 0a48 6f77 6576 6572  ;"}.```..However
-000011c0: 2c20 666f 7220 7468 6520 6d6f 7374 2070  , for the most p
-000011d0: 6172 742c 2066 6967 7572 6573 2061 7265  art, figures are
-000011e0: 2061 2062 6574 7465 7220 7761 7920 746f   a better way to
-000011f0: 2065 6d62 6564 2069 6d61 6765 733a 0a0a   embed images:..
-00001200: 6060 606d 6172 6b64 6f77 6e0a 215b 416e  ```markdown.![An
-00001210: 2065 7861 6d70 6c65 2069 6d61 6765 5d28   example image](
-00001220: 2e2f 696d 6167 6573 2f74 6573 7431 2e6a  ./images/test1.j
-00001230: 7067 297b 7374 796c 653d 2277 6964 7468  pg){style="width
-00001240: 3a20 3330 253b 2062 6f72 6465 723a 2031  : 30%; border: 1
-00001250: 7078 2073 6f6c 6964 2072 6564 3b22 7d0a  px solid red;"}.
-00001260: 6060 600a 0a54 6865 2066 6967 7572 6573  ```..The figures
-00001270: 2074 6865 6d73 656c 7665 7320 6361 6e20   themselves can 
-00001280: 6265 2073 7479 6c65 6420 7769 7468 2074  be styled with t
-00001290: 6865 2060 6669 6773 7479 6c65 6020 616e  he `figstyle` an
-000012a0: 6420 6066 6967 636c 6173 7360 206f 7074  d `figclass` opt
-000012b0: 696f 6e73 3a0a 0a60 6060 6d61 726b 646f  ions:..```markdo
-000012c0: 776e 0a21 5b41 6e6f 7468 6572 2065 7861  wn.![Another exa
-000012d0: 6d70 6c65 2069 6d61 6765 5d28 2e2f 696d  mple image](./im
-000012e0: 6167 6573 2f74 6573 7431 2e6a 7067 297b  ages/test1.jpg){
-000012f0: 7374 796c 653d 2277 6964 7468 3a20 312e  style="width: 1.
-00001300: 3569 6e22 2066 6967 7374 796c 653d 2263  5in" figstyle="c
-00001310: 6f6c 6f72 3a20 7265 643b 2077 6964 7468  olor: red; width
-00001320: 3a20 3335 253b 2220 6669 6763 6c61 7373  : 35%;" figclass
-00001330: 3d22 6161 6120 6262 6222 7d0a 6060 600a  ="aaa bbb"}.```.
-00001340: 0a41 6464 6974 696f 6e61 6c6c 792c 2074  .Additionally, t
-00001350: 6865 7265 2069 7320 7375 7070 6f72 7420  here is support 
-00001360: 666f 7220 6120 7369 6465 2d62 792d 7369  for a side-by-si
-00001370: 6465 2069 6d61 6765 2d61 6e64 2d74 6578  de image-and-tex
-00001380: 7420 696e 2074 6865 2064 6566 6175 6c74  t in the default
-00001390: 0a6c 6179 6f75 742f 7468 656d 6520 7573  .layout/theme us
-000013a0: 696e 6720 6120 6c69 7474 6c65 2048 544d  ing a little HTM
-000013b0: 4c3a 0a0a 6060 606d 6172 6b64 6f77 6e0a  L:..```markdown.
-000013c0: 3c64 6976 2063 6c61 7373 3d22 7477 6f2d  <div class="two-
-000013d0: 636f 6c2d 6669 6722 3e0a 215b 5468 6973  col-fig">.![This
-000013e0: 2069 7320 6f6e 2074 6865 206c 6566 745d   is on the left]
-000013f0: 282e 2f69 6d61 6765 732f 7465 7374 312e  (./images/test1.
-00001400: 6a70 6729 0a3c 6469 7620 7374 796c 653d  jpg).<div style=
-00001410: 2277 6964 7468 3a20 3430 2522 3e0a 2323  "width: 40%">.##
-00001420: 2041 2048 6561 6465 720a 0a4c 6f72 656d   A Header..Lorem
-00001430: 2069 7073 756d 2064 6f6c 6f72 2073 6974   ipsum dolor sit
-00001440: 2061 6d65 742e 2e2e 0a3c 2f64 6976 3e0a   amet....</div>.
-00001450: 3c2f 6469 763e 0a60 6060 0a0a 5468 6520  </div>.```..The 
-00001460: 6f72 6465 7220 6f66 2074 6865 7365 2063  order of these c
-00001470: 616e 2061 6c73 6f20 6265 2073 7761 7070  an also be swapp
-00001480: 6564 3a0a 0a60 6060 6d61 726b 646f 776e  ed:..```markdown
-00001490: 0a3c 6469 7620 636c 6173 733d 2274 776f  .<div class="two
-000014a0: 2d63 6f6c 2d66 6967 223e 0a3c 6469 7620  -col-fig">.<div 
-000014b0: 7374 796c 653d 2277 6964 7468 3a20 3430  style="width: 40
-000014c0: 2522 3e0a 2323 2041 2048 6561 6465 720a  %">.## A Header.
-000014d0: 0a4c 6f72 656d 2069 7073 756d 2064 6f6c  .Lorem ipsum dol
-000014e0: 6f72 2073 6974 2061 6d65 742e 2e2e 0a3c  or sit amet....<
-000014f0: 2f64 6976 3e0a 215b 5468 6973 2069 7320  /div>.![This is 
-00001500: 6f6e 2074 6865 2072 6967 6874 5d28 2e2f  on the right](./
-00001510: 696d 6167 6573 2f74 6573 7431 2e6a 7067  images/test1.jpg
-00001520: 297b 7374 796c 653d 2277 6964 7468 3a20  ){style="width: 
-00001530: 312e 3569 6e22 7d0a 3c2f 6469 763e 0a60  1.5in"}.</div>.`
-00001540: 6060 0a0a 2323 2323 2043 726f 7373 2d52  ``..#### Cross-R
-00001550: 6566 6572 656e 6365 730a 0a58 7265 6673  eferences..Xrefs
-00001560: 2063 616e 2062 6520 6d61 6465 2074 6872   can be made thr
-00001570: 6f75 6768 206c 696e 6b73 2074 6f20 616e  ough links to an
-00001580: 2065 6c65 6d65 6e74 2773 2060 6964 602e   element's `id`.
-00001590: 2042 7920 6465 6661 756c 742c 2068 6561   By default, hea
-000015a0: 6469 6e67 7320 6861 7665 0a61 7574 6f67  dings have.autog
-000015b0: 656e 6572 6174 6564 2049 4473 2062 6173  enerated IDs bas
-000015c0: 6564 206f 6e20 7468 6520 6865 6164 696e  ed on the headin
-000015d0: 6720 7465 7874 2028 652e 672e 2060 2320  g text (e.g. `# 
-000015e0: 4578 616d 706c 656c 7920 4578 616d 706c  Examplely Exampl
-000015f0: 6560 2077 696c 6c0a 6861 7665 2061 6e20  e` will.have an 
-00001600: 6069 6460 206f 6620 607b 7365 6374 696f  `id` of `{sectio
-00001610: 6e7d 2d65 7861 6d70 6c65 6c79 2d65 7861  n}-examplely-exa
-00001620: 6d70 6c65 602e 2048 6f77 6576 6572 2c20  mple`. However, 
-00001630: 7468 6973 2063 616e 2062 6520 6f76 6572  this can be over
-00001640: 7269 6464 656e 0a61 7320 666f 6c6c 6f77  ridden.as follow
-00001650: 733a 0a0a 6060 606d 6172 6b64 6f77 6e0a  s:..```markdown.
-00001660: 2323 2041 4141 7b23 6161 6168 327d 0a60  ## AAA{#aaah2}.`
-00001670: 6060 0a0a 2a2a 2a4e 6f74 653a 2a2a 2a20  ``..***Note:*** 
-00001680: 5468 6520 607b 7365 6374 696f 6e7d 2d60  The `{section}-`
-00001690: 2070 7265 6669 7820 7769 6c6c 2062 6520   prefix will be 
-000016a0: 6170 706c 6965 6420 746f 2061 6c6c 2060  applied to all `
-000016b0: 6964 6020 7661 6c75 6573 206f 7468 6572  id` values other
-000016c0: 0a74 6861 6e20 6f66 2074 6865 2073 6563  .than of the sec
-000016d0: 7469 6f6e 7320 7468 656d 7365 6c76 6573  tions themselves
-000016e0: 2e0a 0a54 6f20 7872 6566 2c20 616e 7920  ...To xref, any 
-000016f0: 6c69 6e6b 2074 6f20 6023 3c69 643e 6020  link to `#<id>` 
-00001700: 7769 6c6c 2073 7566 6669 6365 2c20 6275  will suffice, bu
-00001710: 7420 746f 2073 7479 6c65 2078 7265 6673  t to style xrefs
-00001720: 2c20 6120 6665 7720 6f70 7469 6f6e 730a  , a few options.
-00001730: 6172 6520 6176 6169 6c61 626c 6520 696e  are available in
-00001740: 2074 6865 2064 6566 6175 6c74 2073 7479   the default sty
-00001750: 6c65 2f6c 6179 6f75 742e 0a0a 2a20 602e  le/layout...* `.
-00001760: 7872 6566 603a 2041 2073 696d 706c 6520  xref`: A simple 
-00001770: 756e 7374 796c 6564 2073 6567 6d65 6e74  unstyled segment
-00001780: 206f 6620 7465 7874 2e0a 0a20 2060 6060   of text...  ```
-00001790: 0a20 202a 205b 7872 6566 2074 6f20 4578  .  * [xref to Ex
-000017a0: 616d 706c 6532 2e41 4141 5d28 2365 7861  ample2.AAA](#exa
-000017b0: 6d70 6c65 322d 6161 6168 3229 7b2e 7872  mple2-aaah2){.xr
-000017c0: 6566 7d0a 2020 2a20 3c61 2063 6c61 7373  ef}.  * <a class
-000017d0: 3d22 7872 6566 2220 6872 6566 3d22 2365  ="xref" href="#e
-000017e0: 7861 6d70 6c65 322d 6161 6168 3222 3e78  xample2-aaah2">x
-000017f0: 7265 6620 746f 2045 7861 6d70 6c65 322e  ref to Example2.
-00001800: 4141 413c 2f61 3e0a 2020 6060 600a 0a2a  AAA</a>.  ```..*
-00001810: 2060 2e78 7265 666e 603a 2054 6869 7320   `.xrefn`: This 
-00001820: 7769 6c6c 2061 7574 6f70 6f70 756c 6174  will autopopulat
-00001830: 6520 7468 6520 7461 7267 6574 2773 2074  e the target's t
-00001840: 6578 7420 636f 6e74 656e 742e 2020 0a20  ext content.  . 
-00001850: 202a 2a2a 4e6f 7465 3a2a 2a2a 2042 6520   ***Note:*** Be 
-00001860: 6361 7265 6675 6c20 6e6f 7420 746f 2075  careful not to u
-00001870: 7365 2074 6869 7320 6f6e 2065 6c65 6d65  se this on eleme
-00001880: 6e74 7320 636f 6e74 6169 6e69 6e67 206c  nts containing l
-00001890: 6172 6765 0a20 2071 7561 6e74 6974 6965  arge.  quantitie
-000018a0: 7320 6f66 2074 6578 7420 7669 6120 6368  s of text via ch
-000018b0: 696c 6420 6e6f 6465 732e 0a0a 2020 6060  ild nodes...  ``
-000018c0: 600a 2020 2a20 3c61 2063 6c61 7373 3d22  `.  * <a class="
-000018d0: 7872 6566 6e22 2068 7265 663d 2223 6578  xrefn" href="#ex
-000018e0: 616d 706c 6532 2d61 6161 6832 223e 3c2f  ample2-aaah2"></
-000018f0: 613e 0a20 202a 205b 5d28 2365 7861 6d70  a>.  * [](#examp
-00001900: 6c65 322d 6161 6168 3229 7b2e 7872 6566  le2-aaah2){.xref
-00001910: 6e7d 0a20 2060 6060 0a0a 2a20 602e 7872  n}.  ```..* `.xr
-00001920: 6566 7067 603a 2054 6869 7320 7769 6c6c  efpg`: This will
-00001930: 2061 6464 2061 2022 206f 6e20 7061 6765   add a " on page
-00001940: 2058 5822 2e0a 0a20 2060 6060 0a20 202a   XX"...  ```.  *
-00001950: 203c 6120 636c 6173 733d 2278 7265 666e   <a class="xrefn
-00001960: 2078 7265 6670 6722 2068 7265 663d 2223   xrefpg" href="#
-00001970: 6578 616d 706c 6532 2d61 6161 6832 223e  example2-aaah2">
-00001980: 3c2f 613e 0a20 202a 205b 5d28 2365 7861  </a>.  * [](#exa
-00001990: 6d70 6c65 322d 6161 6168 3229 7b2e 7872  mple2-aaah2){.xr
-000019a0: 6566 6e20 2e78 7265 6670 677d 0a20 2060  efn .xrefpg}.  `
-000019b0: 6060 0a0a 2323 2323 2042 7265 616b 730a  ``..#### Breaks.
-000019c0: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2063  .The following c
-000019d0: 616e 2062 6520 6164 6465 6420 746f 2066  an be added to f
-000019e0: 6f72 6365 2061 2062 7265 616b 2e0a 0a60  orce a break...`
-000019f0: 6060 6874 6d6c 0a3c 6469 7620 636c 6173  ``html.<div clas
-00001a00: 733d 2270 6167 6562 7265 616b 223e 3c2f  s="pagebreak"></
-00001a10: 6469 763e 0a60 6060 0a0a 6060 6068 746d  div>.```..```htm
-00001a20: 6c0a 3c64 6976 2063 6c61 7373 3d22 636f  l.<div class="co
-00001a30: 6c75 6d6e 6272 6561 6b22 3e3c 2f64 6976  lumnbreak"></div
-00001a40: 3e0a 6060 600a 0a23 2323 2320 466f 6f74  >.```..#### Foot
-00001a50: 6e6f 7465 730a 0a46 6f6f 746e 6f74 6573  notes..Footnotes
-00001a60: 2073 686f 756c 6420 6d6f 7374 6c79 2077   should mostly w
-00001a70: 6f72 6b20 6173 2065 7870 6563 7465 642c  ork as expected,
-00001a80: 2062 7574 2063 616e 2066 6974 2070 6f6f   but can fit poo
-00001a90: 726c 7920 616e 6420 6d61 7920 6265 2062  rly and may be b
-00001aa0: 6574 7465 720a 7368 6966 7465 6420 746f  etter.shifted to
-00001ab0: 2061 6e6f 7468 6572 2070 6167 652e 0a0a   another page...
-00001ac0: 6060 606d 6172 6b64 6f77 6e0a 4865 6c6c  ```markdown.Hell
-00001ad0: 6f20 776f 726c 642e 5b5e 7465 7374 5d0a  o world.[^test].
-00001ae0: 0a5b 5e74 6573 745d 3a20 3c68 7474 7073  .[^test]: <https
-00001af0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4368  ://github.com/Ch
-00001b00: 616f 7344 6174 612f 6c69 6d62 6572 6572  aosData/limberer
-00001b10: 3e0a 6060 600a 0a23 2323 2054 6865 6d69  >.```..### Themi
-00001b20: 6e67 2f53 7479 6c69 6e67 0a0a 4279 2064  ng/Styling..By d
-00001b30: 6566 6175 6c74 2c20 606c 696d 6265 7265  efault, `limbere
-00001b40: 7260 2063 6f6d 6573 2077 6974 6820 736f  r` comes with so
-00001b50: 6d65 2063 6f72 6520 7374 796c 696e 6720  me core styling 
-00001b60: 616e 6420 7365 6374 696f 6e20 7465 6d70  and section temp
-00001b70: 6c61 7465 732e 0a49 7420 6973 2065 7870  lates..It is exp
-00001b80: 6563 7465 6420 7468 6174 2075 7365 7273  ected that users
-00001b90: 2077 696c 6c20 6375 7374 6f6d 697a 6520   will customize 
-00001ba0: 7468 6569 7220 646f 6375 6d65 6e74 2074  their document t
-00001bb0: 656d 706c 6174 6573 2062 6579 6f6e 6420  emplates beyond 
-00001bc0: 7768 6174 0a69 7320 7072 6f76 6964 6564  what.is provided
-00001bd0: 2e20 4173 2073 7563 682c 2074 6865 2060  . As such, the `
-00001be0: 6c69 6d62 6572 6572 2063 7265 6174 6560  limberer create`
-00001bf0: 2063 6f6d 6d61 6e64 2073 7570 706f 7274   command support
-00001c00: 7320 6120 602d 7420 3c70 6174 683e 600a  s a `-t <path>`.
-00001c10: 6f70 7469 6f6e 2074 6f20 6765 6e65 7261  option to genera
-00001c20: 7465 2061 206e 6577 2070 726f 6a65 6374  te a new project
-00001c30: 2066 726f 6d20 6120 6769 7665 6e20 7465   from a given te
-00001c40: 6d70 6c61 7465 2070 726f 6a65 6374 2064  mplate project d
-00001c50: 6972 6563 746f 7279 2e0a 0a47 656e 6572  irectory...Gener
-00001c60: 616c 6c79 2073 7065 616b 696e 672c 2074  ally speaking, t
-00001c70: 6865 2073 7479 6c69 6e67 2079 6f75 2077  he styling you w
-00001c80: 616e 7420 746f 2075 7365 2069 7320 7570  ant to use is up
-00001c90: 2074 6f20 796f 752e 2048 6f77 6576 6572   to you. However
-00001ca0: 2c20 666f 720a 636f 6e76 656e 6965 6e63  , for.convenienc
-00001cb0: 652c 2074 6865 2043 5353 2069 7320 6f72  e, the CSS is or
-00001cc0: 6761 6e69 7a65 6420 6173 2060 636f 7265  ganized as `core
-00001cd0: 602c 2060 7374 796c 6560 2c20 616e 6420  `, `style`, and 
-00001ce0: 6063 7573 746f 6d60 2e20 5468 6520 696e  `custom`. The in
-00001cf0: 7465 6e74 0a69 7320 666f 7220 7468 6520  tent.is for the 
-00001d00: 6061 7373 6574 732f 636f 7265 2e63 7373  `assets/core.css
-00001d10: 6020 746f 2063 6f76 6572 2074 6865 206d  ` to cover the m
-00001d20: 6169 6e20 6c61 796f 7574 2061 6e64 2066  ain layout and f
-00001d30: 756e 6374 696f 6e69 6e67 206f 6620 7468  unctioning of th
-00001d40: 650a 646f 6375 6d65 6e74 2c20 7468 6520  e.document, the 
-00001d50: 6061 7373 6574 732f 7374 796c 652e 6373  `assets/style.cs
-00001d60: 7360 2074 6f20 636f 7665 7220 6772 6f75  s` to cover grou
-00001d70: 7020 7468 656d 696e 6720 666f 7220 636f  p theming for co
-00001d80: 6e73 6973 7465 6e63 792c 2061 6e64 0a60  nsistency, and.`
-00001d90: 6375 7374 6f6d 2f63 7573 746f 6d2e 6373  custom/custom.cs
-00001da0: 7360 2074 6f20 6265 2066 6f72 2061 6e79  s` to be for any
-00001db0: 2070 6572 2d64 6f63 756d 656e 742f 7072   per-document/pr
-00001dc0: 6f6a 6563 7420 7374 796c 696e 672e 0a0a  oject styling...
-00001dd0: 2323 2054 6f64 6f20 4c69 7374 0a0a 2a20  ## Todo List..* 
-00001de0: 4472 6166 7420 6275 696c 6473 0a2a 2050  Draft builds.* P
-00001df0: 6172 7469 616c 2062 7569 6c64 7320 6f66  artial builds of
-00001e00: 2069 6e64 6976 6964 7561 6c20 7365 6374   individual sect
-00001e10: 696f 6e73 0a2a 2053 7570 706f 7274 2066  ions.* Support f
-00001e20: 6f72 206e 6f6e 2d4d 6172 6b64 6f77 6e20  or non-Markdown 
-00001e30: 7365 6374 696f 6e73 0a0a 2323 2046 4151  sections..## FAQ
-00001e40: 0a0a 3e20 5768 793f 0a0a 466f 7220 6120  ..> Why?..For a 
-00001e50: 6c69 7461 6e79 206f 6620 7265 6173 6f6e  litany of reason
-00001e60: 732c 2062 7574 2069 6620 4920 6861 6420  s, but if I had 
-00001e70: 746f 2067 6f20 6f75 7420 6f6e 2061 206c  to go out on a l
-00001e80: 696d 6220 616e 6420 7069 636b 206f 6e65  imb and pick one
-00001e90: 2c20 6974 0a77 6f75 6c64 2062 6520 7468  , it.would be th
-00001ea0: 6174 204c 6154 6558 2069 7320 6120 6772  at LaTeX is a gr
-00001eb0: 6561 7420 7479 7065 7365 7474 6572 2c20  eat typesetter, 
-00001ec0: 6275 7420 6120 7465 7272 6962 6c65 2062  but a terrible b
-00001ed0: 7569 6c64 2073 7973 7465 6d2e 0a0a 3e20  uild system...> 
-00001ee0: 5768 6174 213f 0a0a 4772 6565 747a 2074  What!?..Greetz t
-00001ef0: 6f20 6173 6368 2c20 7461 6e6e 6572 2c20  o asch, tanner, 
-00001f00: 6167 7261 6e74 2c20 6a62 6c61 747a 2c20  agrant, jblatz, 
-00001f10: 616e 6420 6474 6869 656c 2e20 3c33 0a    and dthiel. <3.
+00000820: 2045 7861 6d70 6c65 0a0a 6060 6074 6f6d   Example..```tom
+00000830: 6c0a 7469 746c 6520 3d20 2245 7861 6d70  l.title = "Examp
+00000840: 6c65 2044 6f63 756d 656e 7422 0a73 7562  le Document".sub
+00000850: 6865 6164 696e 6720 3d20 222e 2e2e 220a  heading = "...".
+00000860: 2367 6c6f 6261 6c6f 7074 696f 6e3d 7661  #globaloption=va
+00000870: 6c75 650a 232e 2e2e 0a0a 6175 7468 6f72  lue.#.....author
+00000880: 7320 3d20 5b0a 2020 7b20 6e61 6d65 203d  s = [.  { name =
+00000890: 2022 4578 616d 706c 6520 5065 7273 6f6e   "Example Person
+000008a0: 222c 2065 6d61 696c 203d 2022 6578 616d  ", email = "exam
+000008b0: 706c 6540 6578 616d 706c 652e 636f 6d22  ple@example.com"
+000008c0: 207d 2c0a 2020 2e2e 2e0a 5d0a 0a73 6563   },.  ....]..sec
+000008d0: 7469 6f6e 7320 3d20 5b0a 2020 7b20 7479  tions = [.  { ty
+000008e0: 7065 203d 2022 636f 7665 7222 207d 2c0a  pe = "cover" },.
+000008f0: 2020 7b20 7479 7065 203d 2022 746f 6322    { type = "toc"
+00000900: 207d 2c0a 2020 7b20 6e61 6d65 203d 2022   },.  { name = "
+00000910: 6578 616d 706c 6522 2c20 7479 7065 203d  example", type =
+00000920: 2022 7365 6374 696f 6e22 207d 2c0a 2020   "section" },.  
+00000930: 7b20 6e61 6d65 203d 2022 6578 616d 706c  { name = "exampl
+00000940: 6532 222c 2074 7970 6520 3d20 2273 6563  e2", type = "sec
+00000950: 7469 6f6e 222c 2073 6563 7469 6f6e 6f70  tion", sectionop
+00000960: 7469 6f6e 203d 2022 7661 6c75 6522 207d  tion = "value" }
+00000970: 2c0a 2020 2e2e 2e0a 5d0a 6060 600a 0a41  ,.  ....].```..A
+00000980: 6464 6974 696f 6e61 6c20 6f72 206f 7665  dditional or ove
+00000990: 7272 6964 696e 6720 7365 7474 696e 6773  rriding settings
+000009a0: 206f 7220 4d75 7374 6163 6865 2074 656d   or Mustache tem
+000009b0: 706c 6174 6520 7661 7269 6162 6c65 7320  plate variables 
+000009c0: 6361 6e20 6265 0a63 6f6e 6669 6775 7265  can be.configure
+000009d0: 6420 6279 2070 6173 7369 6e67 2061 6464  d by passing add
+000009e0: 6974 696f 6e61 6c20 544f 4d4c 2066 696c  itional TOML fil
+000009f0: 6520 7061 7468 7320 696e 746f 2074 6865  e paths into the
+00000a00: 2060 6c69 6d62 6572 6572 2062 7569 6c64   `limberer build
+00000a10: 600a 636f 6d6d 616e 643a 0a0a 6060 600a  `.command:..```.
+00000a20: 2420 6c69 6d62 6572 6572 2062 7569 6c64  $ limberer build
+00000a30: 2072 6570 6f72 742e 746f 6d6c 2073 7461   report.toml sta
+00000a40: 7473 2e74 6f6d 6c0a 6060 600a 0a23 2323  ts.toml.```..###
+00000a50: 2053 6563 7469 6f6e 2054 656d 706c 6174   Section Templat
+00000a60: 6573 0a0a 4f75 7420 6f66 2074 6865 2062  es..Out of the b
+00000a70: 6f78 2c20 606c 696d 6265 7265 7260 2063  ox, `limberer` c
+00000a80: 6f6d 6573 2077 6974 6820 736f 6d65 2069  omes with some i
+00000a90: 6e69 7469 616c 2073 6563 7469 6f6e 2074  nitial section t
+00000aa0: 656d 706c 6174 6573 3a0a 0a2a 2060 636f  emplates:..* `co
+00000ab0: 7665 7260 3a20 4120 7469 746c 6520 7061  ver`: A title pa
+00000ac0: 6765 2073 6563 7469 6f6e 2e0a 2a20 6074  ge section..* `t
+00000ad0: 6f63 603a 2041 2074 6162 6c65 206f 6620  oc`: A table of 
+00000ae0: 636f 6e74 656e 7473 2073 6563 7469 6f6e  contents section
+00000af0: 2e0a 2a20 6073 6563 7469 6f6e 603a 2054  ..* `section`: T
+00000b00: 6865 2075 6e64 6572 6c79 696e 6720 7465  he underlying te
+00000b10: 6d70 6c61 7465 2066 6f72 2063 7573 746f  mplate for custo
+00000b20: 6d20 7365 6374 696f 6e73 2e0a 0a41 6464  m sections...Add
+00000b30: 6974 696f 6e61 6c6c 792c 2060 6c69 6d62  itionally, `limb
+00000b40: 6572 6572 6020 7375 7070 6f72 7473 2074  erer` supports t
+00000b50: 6865 2066 6f6c 6c6f 7769 6e67 2074 656d  he following tem
+00000b60: 706c 6174 652d 6c69 6b65 2070 7365 7564  plate-like pseud
+00000b70: 6f2d 7365 6374 696f 6e73 3a0a 0a2a 2060  o-sections:..* `
+00000b80: 6170 7065 6e64 6978 5f73 7461 7274 603a  appendix_start`:
+00000b90: 2053 7562 7365 7175 656e 7420 7365 6374   Subsequent sect
+00000ba0: 696f 6e73 2077 696c 6c20 6265 2074 7265  ions will be tre
+00000bb0: 6174 6564 2061 7320 6170 7065 6e64 6963  ated as appendic
+00000bc0: 6573 2e0a 2a20 6061 7070 656e 6469 785f  es..* `appendix_
+00000bd0: 656e 6460 3a20 4469 7361 626c 6573 2074  end`: Disables t
+00000be0: 6865 2061 626f 7665 2073 6574 7469 6e67  he above setting
+00000bf0: 3b20 7375 6273 6571 7565 6e74 2073 6563  ; subsequent sec
+00000c00: 7469 6f6e 7320 6172 6520 6e6f 740a 2020  tions are not.  
+00000c10: 7472 6561 7465 6420 6173 2061 7070 656e  treated as appen
+00000c20: 6469 6365 732e 2054 6865 2061 7070 656e  dices. The appen
+00000c30: 6469 7820 636f 756e 7465 7220 7769 6c6c  dix counter will
+00000c40: 206e 6f74 2062 6520 636c 6561 7265 642e   not be cleared.
+00000c50: 0a0a 2323 2320 4375 7374 6f6d 2053 6563  ..### Custom Sec
+00000c60: 7469 6f6e 730a 0a43 7573 746f 6d20 7365  tions..Custom se
+00000c70: 6374 696f 6e73 2028 2273 6563 7469 6f6e  ctions ("section
+00000c80: 7322 2920 6172 6520 6120 6d69 7820 6f66  s") are a mix of
+00000c90: 204d 6172 6b64 6f77 6e20 2861 6e64 2c20   Markdown (and, 
+00000ca0: 696e 2073 6f6d 6520 6361 7365 732c 2048  in some cases, H
+00000cb0: 544d 4c29 2c0a 7769 7468 2073 7570 706f  TML),.with suppo
+00000cc0: 7274 2066 6f72 204d 7573 7461 6368 6520  rt for Mustache 
+00000cd0: 6578 7072 6573 7369 6f6e 7320 2875 7369  expressions (usi
+00000ce0: 6e67 2074 6865 2054 4f4d 4c20 636f 6e66  ng the TOML conf
+00000cf0: 6967 7572 6174 696f 6e29 2c20 7768 6572  iguration), wher
+00000d00: 650a 6d6f 7374 2064 6f63 756d 656e 7420  e.most document 
+00000d10: 636f 6e74 656e 7420 6973 2077 7269 7474  content is writt
+00000d20: 656e 2e20 4120 7365 6374 696f 6e20 6361  en. A section ca
+00000d30: 6e20 6265 6769 6e20 7769 7468 2061 2062  n begin with a b
+00000d40: 6c6f 636b 206f 6620 4d61 726b 646f 776e  lock of Markdown
+00000d50: 0a6d 6574 6164 6174 613a 0a0a 6060 606d  .metadata:..```m
+00000d60: 6172 6b64 6f77 6e0a 2d2d 2d0a 746f 635f  arkdown.---.toc_
+00000d70: 6865 6164 6572 5f6c 6576 656c 3a20 320a  header_level: 2.
+00000d80: 636f 6c75 6d6e 733a 2074 7275 650a 7469  columns: true.ti
+00000d90: 746c 653a 2045 7861 6d70 6c65 330a 636c  tle: Example3.cl
+00000da0: 6173 7365 733a 2066 6f6f 2062 6172 2062  asses: foo bar b
+00000db0: 617a 0a2d 2d2d 0a60 6060 0a0a 5468 6520  az.---.```..The 
+00000dc0: 6d65 7461 6461 7461 206f 7074 696f 6e73  metadata options
+00000dd0: 2061 7265 206d 6572 6765 6420 7769 7468   are merged with
+00000de0: 2074 6865 2073 6563 7469 6f6e 2065 6e74   the section ent
+00000df0: 7279 206f 7074 696f 6e73 2e20 4375 7272  ry options. Curr
+00000e00: 656e 746c 790a 7375 7070 6f72 7465 6420  ently.supported 
+00000e10: 6f70 7469 6f6e 7320 6172 6520 7468 6520  options are the 
+00000e20: 666f 6c6c 6f77 696e 673a 0a0a 2a20 6074  following:..* `t
+00000e30: 6f63 5f68 6561 6465 725f 6c65 7665 6c60  oc_header_level`
+00000e40: 3a20 4865 6164 6572 206c 6576 656c 206c  : Header level l
+00000e50: 696d 6974 2074 6f20 7573 6520 666f 7220  imit to use for 
+00000e60: 7461 626c 6520 6f66 2063 6f6e 7465 6e74  table of content
+00000e70: 7320 656e 7472 790a 2020 6765 6e65 7261  s entry.  genera
+00000e80: 7469 6f6e 2e0a 2a20 6063 6f6c 756d 6e73  tion..* `columns
+00000e90: 603a 2057 6865 7468 6572 206f 7220 6e6f  `: Whether or no
+00000ea0: 7420 746f 2075 7365 2074 6865 2032 2d63  t to use the 2-c
+00000eb0: 6f6c 756d 6e20 666f 726d 6174 2066 6f72  olumn format for
+00000ec0: 2074 6865 2073 6563 7469 6f6e 2e0a 2a20   the section..* 
+00000ed0: 6074 6974 6c65 603a 2053 6563 7469 6f6e  `title`: Section
+00000ee0: 2074 6974 6c65 2066 6f72 2032 2d63 6f6c   title for 2-col
+00000ef0: 756d 6e20 666f 726d 6174 2e0a 2a20 6063  umn format..* `c
+00000f00: 6c61 7373 6573 603a 204c 6973 7420 6f66  lasses`: List of
+00000f10: 2048 544d 4c20 636c 6173 7320 6e61 6d65   HTML class name
+00000f20: 7320 746f 2061 7070 6c79 2074 6f20 7468  s to apply to th
+00000f30: 6520 7365 6374 696f 6e20 2860 3c61 7274  e section (`<art
+00000f40: 6963 6c65 3e60 290a 0a23 2323 2320 5461  icle>`)..#### Ta
+00000f50: 626c 6573 0a0a 5461 626c 6573 2063 616e  bles..Tables can
+00000f60: 2062 6520 7772 6974 7465 6e20 7573 696e   be written usin
+00000f70: 6720 7468 6520 7069 7065 2d64 656c 696d  g the pipe-delim
+00000f80: 6974 6564 2047 6974 4875 622d 666c 6176  ited GitHub-flav
+00000f90: 6f72 6564 204d 6172 6b64 6f77 6e0a 636f  ored Markdown.co
+00000fa0: 6e76 656e 7469 6f6e 2c20 6f72 2077 6974  nvention, or wit
+00000fb0: 6820 4854 4d4c 2074 6162 6c65 732e 0a0a  h HTML tables...
+00000fc0: 6060 606d 6172 6b64 6f77 6e0a 7c20 4669  ```markdown.| Fi
+00000fd0: 7273 7420 4865 6164 6572 2020 7c20 5365  rst Header  | Se
+00000fe0: 636f 6e64 2048 6561 6465 7220 7c0a 7c20  cond Header |.| 
+00000ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c20  ------------- | 
+00001000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 7c0a  ------------- |.
+00001010: 7c20 436f 6e74 656e 7420 4365 6c6c 2020  | Content Cell  
+00001020: 7c20 436f 6e74 656e 7420 4365 6c6c 2020  | Content Cell  
+00001030: 7c0a 7c20 436f 6e74 656e 7420 4365 6c6c  |.| Content Cell
+00001040: 2020 7c20 436f 6e74 656e 7420 4365 6c6c    | Content Cell
+00001050: 2020 7c0a 6060 600a 0a60 6060 6048 544d    |.```..````HTM
+00001060: 4c0a 3c74 6162 6c65 3e0a 2020 3c74 6865  L.<table>.  <the
+00001070: 6164 3e0a 2020 2020 3c74 723e 0a20 2020  ad>.    <tr>.   
+00001080: 2020 203c 7468 2073 7479 6c65 3d22 7769     <th style="wi
+00001090: 6474 683a 2032 3025 223e 613c 2f74 683e  dth: 20%">a</th>
+000010a0: 0a20 2020 2020 203c 7468 2073 7479 6c65  .      <th style
+000010b0: 3d22 7769 6474 683a 2034 3025 223e 623c  ="width: 40%">b<
+000010c0: 2f74 683e 0a20 2020 2020 203c 7468 3e63  /th>.      <th>c
+000010d0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+000010e0: 643c 2f74 683e 0a20 2020 203c 2f74 723e  d</th>.    </tr>
+000010f0: 0a20 203c 2f74 6865 6164 3e0a 2020 3c74  .  </thead>.  <t
+00001100: 626f 6479 3e0a 2020 2020 3c74 723e 3c74  body>.    <tr><t
+00001110: 643e 2a2a 426f 6c64 2a2a 3c2f 7464 3e3c  d>**Bold**</td><
+00001120: 7464 3e5f 6974 616c 6963 5f3c 2f74 643e  td>_italic_</td>
+00001130: 0a3c 7464 3e0a 6060 600a 636f 6465 2062  .<td>.```.code b
+00001140: 6c6f 636b 0a60 6060 0a3c 2f74 643e 0a3c  lock.```.</td>.<
+00001150: 7464 3e0a 2a20 6c69 7374 0a2a 206f 660a  td>.* list.* of.
+00001160: 2a20 7468 696e 6773 0a3c 2f74 643e 0a20  * things.</td>. 
+00001170: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00001180: 3e3c 7464 3e3c 2f74 643e 3c74 643e 3c2f  ><td></td><td></
+00001190: 7464 3e3c 7464 3e3c 2f74 643e 3c74 643e  td><td></td><td>
+000011a0: 3c2f 7464 3e3c 2f74 723e 0a20 2020 203c  </td></tr>.    <
+000011b0: 7472 3e3c 7464 3e3c 2f74 643e 3c74 643e  tr><td></td><td>
+000011c0: 3c2f 7464 3e3c 7464 3e3c 2f74 643e 3c74  </td><td></td><t
+000011d0: 643e 3c2f 7464 3e3c 2f74 723e 0a20 2020  d></td></tr>.   
+000011e0: 203c 7472 3e3c 7464 3e3c 2f74 643e 3c74   <tr><td></td><t
+000011f0: 643e 3c2f 7464 3e3c 7464 3e3c 2f74 643e  d></td><td></td>
+00001200: 3c74 643e 3c2f 7464 3e3c 2f74 723e 0a20  <td></td></tr>. 
+00001210: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+00001220: 653e 0a60 6060 600a 0a23 2323 2320 496d  e>.````..#### Im
+00001230: 6167 6573 0a0a 4120 7369 6d70 6c65 2069  ages..A simple i
+00001240: 6d61 6765 2063 616e 2062 6520 656d 6265  mage can be embe
+00001250: 6464 6564 2077 6974 6820 6375 7374 6f6d  dded with custom
+00001260: 2043 5353 2074 6f20 706c 6163 652f 7374   CSS to place/st
+00001270: 796c 6520 6974 3a0a 0a60 6060 6d61 726b  yle it:..```mark
+00001280: 646f 776e 0a21 5b5d 282e 2f69 6d61 6765  down.![](./image
+00001290: 732f 7465 7374 312e 6a70 6729 7b73 7479  s/test1.jpg){sty
+000012a0: 6c65 3d22 7769 6474 683a 2033 3025 3b20  le="width: 30%; 
+000012b0: 6d61 7267 696e 3a20 6175 746f 3b20 6469  margin: auto; di
+000012c0: 7370 6c61 793a 2062 6c6f 636b 3b22 7d0a  splay: block;"}.
+000012d0: 6060 600a 0a48 6f77 6576 6572 2c20 666f  ```..However, fo
+000012e0: 7220 7468 6520 6d6f 7374 2070 6172 742c  r the most part,
+000012f0: 2066 6967 7572 6573 2061 7265 2061 2062   figures are a b
+00001300: 6574 7465 7220 7761 7920 746f 2065 6d62  etter way to emb
+00001310: 6564 2069 6d61 6765 733a 0a0a 6060 606d  ed images:..```m
+00001320: 6172 6b64 6f77 6e0a 215b 416e 2065 7861  arkdown.![An exa
+00001330: 6d70 6c65 2069 6d61 6765 5d28 2e2f 696d  mple image](./im
+00001340: 6167 6573 2f74 6573 7431 2e6a 7067 297b  ages/test1.jpg){
+00001350: 7374 796c 653d 2277 6964 7468 3a20 3330  style="width: 30
+00001360: 253b 2062 6f72 6465 723a 2031 7078 2073  %; border: 1px s
+00001370: 6f6c 6964 2072 6564 3b22 7d0a 6060 600a  olid red;"}.```.
+00001380: 0a54 6865 2066 6967 7572 6573 2074 6865  .The figures the
+00001390: 6d73 656c 7665 7320 6361 6e20 6265 2073  mselves can be s
+000013a0: 7479 6c65 6420 7769 7468 2074 6865 2060  tyled with the `
+000013b0: 6669 6773 7479 6c65 6020 616e 6420 6066  figstyle` and `f
+000013c0: 6967 636c 6173 7360 206f 7074 696f 6e73  igclass` options
+000013d0: 3a0a 0a60 6060 6d61 726b 646f 776e 0a21  :..```markdown.!
+000013e0: 5b41 6e6f 7468 6572 2065 7861 6d70 6c65  [Another example
+000013f0: 2069 6d61 6765 5d28 2e2f 696d 6167 6573   image](./images
+00001400: 2f74 6573 7431 2e6a 7067 297b 7374 796c  /test1.jpg){styl
+00001410: 653d 2277 6964 7468 3a20 312e 3569 6e22  e="width: 1.5in"
+00001420: 2066 6967 7374 796c 653d 2263 6f6c 6f72   figstyle="color
+00001430: 3a20 7265 643b 2077 6964 7468 3a20 3335  : red; width: 35
+00001440: 253b 2220 6669 6763 6c61 7373 3d22 6161  %;" figclass="aa
+00001450: 6120 6262 6222 7d0a 6060 600a 0a41 6464  a bbb"}.```..Add
+00001460: 6974 696f 6e61 6c6c 792c 2074 6865 7265  itionally, there
+00001470: 2069 7320 7375 7070 6f72 7420 666f 7220   is support for 
+00001480: 6120 7369 6465 2d62 792d 7369 6465 2069  a side-by-side i
+00001490: 6d61 6765 2d61 6e64 2d74 6578 7420 696e  mage-and-text in
+000014a0: 2074 6865 2064 6566 6175 6c74 0a6c 6179   the default.lay
+000014b0: 6f75 742f 7468 656d 6520 7573 696e 6720  out/theme using 
+000014c0: 6120 6c69 7474 6c65 2048 544d 4c3a 0a0a  a little HTML:..
+000014d0: 6060 606d 6172 6b64 6f77 6e0a 3c64 6976  ```markdown.<div
+000014e0: 2063 6c61 7373 3d22 7477 6f2d 636f 6c2d   class="two-col-
+000014f0: 6669 6722 3e0a 215b 5468 6973 2069 7320  fig">.![This is 
+00001500: 6f6e 2074 6865 206c 6566 745d 282e 2f69  on the left](./i
+00001510: 6d61 6765 732f 7465 7374 312e 6a70 6729  mages/test1.jpg)
+00001520: 0a3c 6469 7620 7374 796c 653d 2277 6964  .<div style="wid
+00001530: 7468 3a20 3430 2522 3e0a 2323 2041 2048  th: 40%">.## A H
+00001540: 6561 6465 720a 0a4c 6f72 656d 2069 7073  eader..Lorem ips
+00001550: 756d 2064 6f6c 6f72 2073 6974 2061 6d65  um dolor sit ame
+00001560: 742e 2e2e 0a3c 2f64 6976 3e0a 3c2f 6469  t....</div>.</di
+00001570: 763e 0a60 6060 0a0a 5468 6520 6f72 6465  v>.```..The orde
+00001580: 7220 6f66 2074 6865 7365 2063 616e 2061  r of these can a
+00001590: 6c73 6f20 6265 2073 7761 7070 6564 3a0a  lso be swapped:.
+000015a0: 0a60 6060 6d61 726b 646f 776e 0a3c 6469  .```markdown.<di
+000015b0: 7620 636c 6173 733d 2274 776f 2d63 6f6c  v class="two-col
+000015c0: 2d66 6967 223e 0a3c 6469 7620 7374 796c  -fig">.<div styl
+000015d0: 653d 2277 6964 7468 3a20 3430 2522 3e0a  e="width: 40%">.
+000015e0: 2323 2041 2048 6561 6465 720a 0a4c 6f72  ## A Header..Lor
+000015f0: 656d 2069 7073 756d 2064 6f6c 6f72 2073  em ipsum dolor s
+00001600: 6974 2061 6d65 742e 2e2e 0a3c 2f64 6976  it amet....</div
+00001610: 3e0a 215b 5468 6973 2069 7320 6f6e 2074  >.![This is on t
+00001620: 6865 2072 6967 6874 5d28 2e2f 696d 6167  he right](./imag
+00001630: 6573 2f74 6573 7431 2e6a 7067 297b 7374  es/test1.jpg){st
+00001640: 796c 653d 2277 6964 7468 3a20 312e 3569  yle="width: 1.5i
+00001650: 6e22 7d0a 3c2f 6469 763e 0a60 6060 0a0a  n"}.</div>.```..
+00001660: 2323 2323 2043 726f 7373 2d52 6566 6572  #### Cross-Refer
+00001670: 656e 6365 730a 0a58 7265 6673 2063 616e  ences..Xrefs can
+00001680: 2062 6520 6d61 6465 2074 6872 6f75 6768   be made through
+00001690: 206c 696e 6b73 2074 6f20 616e 2065 6c65   links to an ele
+000016a0: 6d65 6e74 2773 2060 6964 602e 2042 7920  ment's `id`. By 
+000016b0: 6465 6661 756c 742c 2068 6561 6469 6e67  default, heading
+000016c0: 7320 6861 7665 0a61 7574 6f67 656e 6572  s have.autogener
+000016d0: 6174 6564 2049 4473 2062 6173 6564 206f  ated IDs based o
+000016e0: 6e20 7468 6520 6865 6164 696e 6720 7465  n the heading te
+000016f0: 7874 2028 652e 672e 2060 2320 4578 616d  xt (e.g. `# Exam
+00001700: 706c 656c 7920 4578 616d 706c 6560 2077  plely Example` w
+00001710: 696c 6c0a 6861 7665 2061 6e20 6069 6460  ill.have an `id`
+00001720: 206f 6620 607b 7365 6374 696f 6e7d 2d65   of `{section}-e
+00001730: 7861 6d70 6c65 6c79 2d65 7861 6d70 6c65  xamplely-example
+00001740: 602e 2048 6f77 6576 6572 2c20 7468 6973  `. However, this
+00001750: 2063 616e 2062 6520 6f76 6572 7269 6464   can be overridd
+00001760: 656e 0a61 7320 666f 6c6c 6f77 733a 0a0a  en.as follows:..
+00001770: 6060 606d 6172 6b64 6f77 6e0a 2323 2041  ```markdown.## A
+00001780: 4141 7b23 6161 6168 327d 0a60 6060 0a0a  AA{#aaah2}.```..
+00001790: 2a2a 2a4e 6f74 653a 2a2a 2a20 5468 6520  ***Note:*** The 
+000017a0: 607b 7365 6374 696f 6e7d 2d60 2070 7265  `{section}-` pre
+000017b0: 6669 7820 7769 6c6c 2062 6520 6170 706c  fix will be appl
+000017c0: 6965 6420 746f 2061 6c6c 2060 6964 6020  ied to all `id` 
+000017d0: 7661 6c75 6573 206f 7468 6572 0a74 6861  values other.tha
+000017e0: 6e20 6f66 2074 6865 2073 6563 7469 6f6e  n of the section
+000017f0: 7320 7468 656d 7365 6c76 6573 2e0a 0a54  s themselves...T
+00001800: 6f20 7872 6566 2c20 616e 7920 6c69 6e6b  o xref, any link
+00001810: 2074 6f20 6023 3c69 643e 6020 7769 6c6c   to `#<id>` will
+00001820: 2073 7566 6669 6365 2c20 6275 7420 746f   suffice, but to
+00001830: 2073 7479 6c65 2078 7265 6673 2c20 6120   style xrefs, a 
+00001840: 6665 7720 6f70 7469 6f6e 730a 6172 6520  few options.are 
+00001850: 6176 6169 6c61 626c 6520 696e 2074 6865  available in the
+00001860: 2064 6566 6175 6c74 2073 7479 6c65 2f6c   default style/l
+00001870: 6179 6f75 742e 0a0a 2a20 602e 7872 6566  ayout...* `.xref
+00001880: 603a 2041 2073 696d 706c 6520 756e 7374  `: A simple unst
+00001890: 796c 6564 2073 6567 6d65 6e74 206f 6620  yled segment of 
+000018a0: 7465 7874 2e0a 0a20 2060 6060 0a20 202a  text...  ```.  *
+000018b0: 205b 7872 6566 2074 6f20 4578 616d 706c   [xref to Exampl
+000018c0: 6532 2e41 4141 5d28 2365 7861 6d70 6c65  e2.AAA](#example
+000018d0: 322d 6161 6168 3229 7b2e 7872 6566 7d0a  2-aaah2){.xref}.
+000018e0: 2020 2a20 3c61 2063 6c61 7373 3d22 7872    * <a class="xr
+000018f0: 6566 2220 6872 6566 3d22 2365 7861 6d70  ef" href="#examp
+00001900: 6c65 322d 6161 6168 3222 3e78 7265 6620  le2-aaah2">xref 
+00001910: 746f 2045 7861 6d70 6c65 322e 4141 413c  to Example2.AAA<
+00001920: 2f61 3e0a 2020 6060 600a 0a2a 2060 2e78  /a>.  ```..* `.x
+00001930: 7265 666e 603a 2054 6869 7320 7769 6c6c  refn`: This will
+00001940: 2061 7574 6f70 6f70 756c 6174 6520 7468   autopopulate th
+00001950: 6520 7461 7267 6574 2773 2074 6578 7420  e target's text 
+00001960: 636f 6e74 656e 742e 2020 0a20 202a 2a2a  content.  .  ***
+00001970: 4e6f 7465 3a2a 2a2a 2042 6520 6361 7265  Note:*** Be care
+00001980: 6675 6c20 6e6f 7420 746f 2075 7365 2074  ful not to use t
+00001990: 6869 7320 6f6e 2065 6c65 6d65 6e74 7320  his on elements 
+000019a0: 636f 6e74 6169 6e69 6e67 206c 6172 6765  containing large
+000019b0: 0a20 2071 7561 6e74 6974 6965 7320 6f66  .  quantities of
+000019c0: 2074 6578 7420 7669 6120 6368 696c 6420   text via child 
+000019d0: 6e6f 6465 732e 0a0a 2020 6060 600a 2020  nodes...  ```.  
+000019e0: 2a20 3c61 2063 6c61 7373 3d22 7872 6566  * <a class="xref
+000019f0: 6e22 2068 7265 663d 2223 6578 616d 706c  n" href="#exampl
+00001a00: 6532 2d61 6161 6832 223e 3c2f 613e 0a20  e2-aaah2"></a>. 
+00001a10: 202a 205b 5d28 2365 7861 6d70 6c65 322d   * [](#example2-
+00001a20: 6161 6168 3229 7b2e 7872 6566 6e7d 0a20  aaah2){.xrefn}. 
+00001a30: 2060 6060 0a0a 2a20 602e 7872 6566 7067   ```..* `.xrefpg
+00001a40: 603a 2054 6869 7320 7769 6c6c 2061 6464  `: This will add
+00001a50: 2061 2022 206f 6e20 7061 6765 2058 5822   a " on page XX"
+00001a60: 2e0a 0a20 2060 6060 0a20 202a 203c 6120  ...  ```.  * <a 
+00001a70: 636c 6173 733d 2278 7265 666e 2078 7265  class="xrefn xre
+00001a80: 6670 6722 2068 7265 663d 2223 6578 616d  fpg" href="#exam
+00001a90: 706c 6532 2d61 6161 6832 223e 3c2f 613e  ple2-aaah2"></a>
+00001aa0: 0a20 202a 205b 5d28 2365 7861 6d70 6c65  .  * [](#example
+00001ab0: 322d 6161 6168 3229 7b2e 7872 6566 6e20  2-aaah2){.xrefn 
+00001ac0: 2e78 7265 6670 677d 0a20 2060 6060 0a0a  .xrefpg}.  ```..
+00001ad0: 2323 2323 2043 6f64 6520 426c 6f63 6b73  #### Code Blocks
+00001ae0: 0a0a 0a60 6060 606d 6172 6b64 6f77 6e0a  ...````markdown.
+00001af0: 6060 606a 730a 6c65 7420 6a20 3d20 6177  ```js.let j = aw
+00001b00: 6169 7420 6665 7463 6828 2268 7474 7073  ait fetch("https
+00001b10: 3a2f 2f77 6174 2e77 6174 222c 207b 0a20  ://wat.wat", {. 
+00001b20: 2022 6865 6164 6572 7322 3a20 7b0a 2020   "headers": {.  
+00001b30: 2020 2278 2d74 6573 7422 3a20 2266 6f6f    "x-test": "foo
+00001b40: 220a 2020 7d0a 7d29 2e74 6865 6e28 2872  ".  }.}).then((r
+00001b50: 6573 293d 3e72 6573 2e6a 736f 6e28 2929  es)=>res.json())
+00001b60: 3b0a 6060 600a 3c63 656e 7465 723e 4578  ;.```.<center>Ex
+00001b70: 616d 706c 6520 536e 6970 7065 7420 6f66  ample Snippet of
+00001b80: 2043 6f64 653c 2f63 656e 7465 723e 0a0a   Code</center>..
+00001b90: 6060 606a 730a 6c65 7420 6a20 3d20 6177  ```js.let j = aw
+00001ba0: 6169 7420 6665 7463 6828 2268 7474 7073  ait fetch("https
+00001bb0: 3a2f 2f77 6174 2e77 6174 222c 207b 0a20  ://wat.wat", {. 
+00001bc0: 2022 6865 6164 6572 7322 3a20 7b0a 2020   "headers": {.  
+00001bd0: 2020 2278 2d74 6573 7422 3a20 2266 6f6f    "x-test": "foo
+00001be0: 220a 2020 7d0a 7d29 2e74 6865 6e28 2872  ".  }.}).then((r
+00001bf0: 6573 293d 3e72 6573 2e6a 736f 6e28 2929  es)=>res.json())
+00001c00: 3b0a 6060 600a 3c66 6967 7572 653e 3c66  ;.```.<figure><f
+00001c10: 6967 6361 7074 696f 6e3e 4578 616d 706c  igcaption>Exampl
+00001c20: 6520 536e 6970 7065 7420 6f66 2043 6f64  e Snippet of Cod
+00001c30: 6520 7769 7468 2061 2066 6967 7572 6520  e with a figure 
+00001c40: 7072 6566 6978 3c2f 6669 6763 6170 7469  prefix</figcapti
+00001c50: 6f6e 3e3c 2f66 6967 7572 653e 0a60 6060  on></figure>.```
+00001c60: 600a 0a54 6865 2066 6f6c 6c6f 7769 6e67  `..The following
+00001c70: 2073 6574 7469 6e67 7320 6361 6e20 6265   settings can be
+00001c80: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
+00001c90: 6865 2070 726f 6a65 6374 2054 4f4d 4c3a  he project TOML:
+00001ca0: 0a0a 2a20 6068 6967 686c 6967 6874 6020  ..* `highlight` 
+00001cb0: 2864 6566 6175 6c74 7320 746f 2060 226d  (defaults to `"m
+00001cc0: 6f6c 6f6b 6169 2260 290a 2a20 6068 6967  olokai"`).* `hig
+00001cd0: 686c 6967 6874 5f70 6c61 696e 7465 7874  hlight_plaintext
+00001ce0: 6020 2864 6566 6175 6c74 7320 746f 2060  ` (defaults to `
+00001cf0: 2273 6f6c 6172 697a 6564 2d64 6172 6b22  "solarized-dark"
+00001d00: 6029 0a2a 2060 6869 6768 6c69 6768 745f  `).* `highlight_
+00001d10: 666f 6e74 6020 2864 6566 6175 6c74 7320  font` (defaults 
+00001d20: 746f 2060 2227 4465 6a61 5675 2053 616e  to `"'DejaVu San
+00001d30: 7320 4d6f 6e6f 272c 206d 6f6e 6f73 7061  s Mono', monospa
+00001d40: 6365 2260 290a 2a20 6068 6967 686c 6967  ce"`).* `highlig
+00001d50: 6874 5f73 7479 6c65 6020 2864 6566 6175  ht_style` (defau
+00001d60: 6c74 7320 746f 2060 2270 6164 6469 6e67  lts to `"padding
+00001d70: 3a20 3172 656d 3b20 626f 7264 6572 2d72  : 1rem; border-r
+00001d80: 6164 6975 733a 2032 7078 3b20 6f76 6572  adius: 2px; over
+00001d90: 666c 6f77 2d78 3a20 6175 746f 3b22 600a  flow-x: auto;"`.
+00001da0: 2a20 6068 6967 686c 6967 6874 5f6c 696e  * `highlight_lin
+00001db0: 655f 6c65 6e67 7468 6020 2864 6566 6175  e_length` (defau
+00001dc0: 6c74 7320 746f 2060 2237 3422 6029 0a0a  lts to `"74"`)..
+00001dd0: 2323 2323 2042 7265 616b 730a 0a54 6865  #### Breaks..The
+00001de0: 2066 6f6c 6c6f 7769 6e67 2063 616e 2062   following can b
+00001df0: 6520 6164 6465 6420 746f 2066 6f72 6365  e added to force
+00001e00: 2061 2062 7265 616b 2e0a 0a60 6060 6874   a break...```ht
+00001e10: 6d6c 0a3c 6469 7620 636c 6173 733d 2270  ml.<div class="p
+00001e20: 6167 6562 7265 616b 223e 3c2f 6469 763e  agebreak"></div>
+00001e30: 0a60 6060 0a0a 6060 6068 746d 6c0a 3c64  .```..```html.<d
+00001e40: 6976 2063 6c61 7373 3d22 636f 6c75 6d6e  iv class="column
+00001e50: 6272 6561 6b22 3e3c 2f64 6976 3e0a 6060  break"></div>.``
+00001e60: 600a 0a23 2323 2320 466f 6f74 6e6f 7465  `..#### Footnote
+00001e70: 730a 0a46 6f6f 746e 6f74 6573 2073 686f  s..Footnotes sho
+00001e80: 756c 6420 6d6f 7374 6c79 2077 6f72 6b20  uld mostly work 
+00001e90: 6173 2065 7870 6563 7465 642c 2062 7574  as expected, but
+00001ea0: 2063 616e 2066 6974 2070 6f6f 726c 7920   can fit poorly 
+00001eb0: 616e 6420 6d61 7920 6265 2062 6574 7465  and may be bette
+00001ec0: 720a 7368 6966 7465 6420 746f 2061 6e6f  r.shifted to ano
+00001ed0: 7468 6572 2070 6167 652e 0a0a 6060 606d  ther page...```m
+00001ee0: 6172 6b64 6f77 6e0a 4865 6c6c 6f20 776f  arkdown.Hello wo
+00001ef0: 726c 642e 5b5e 7465 7374 5d0a 0a5b 5e74  rld.[^test]..[^t
+00001f00: 6573 745d 3a20 3c68 7474 7073 3a2f 2f67  est]: <https://g
+00001f10: 6974 6875 622e 636f 6d2f 4368 616f 7344  ithub.com/ChaosD
+00001f20: 6174 612f 6c69 6d62 6572 6572 3e0a 6060  ata/limberer>.``
+00001f30: 600a 0a23 2323 2054 6865 6d69 6e67 2f53  `..### Theming/S
+00001f40: 7479 6c69 6e67 0a0a 4279 2064 6566 6175  tyling..By defau
+00001f50: 6c74 2c20 606c 696d 6265 7265 7260 2063  lt, `limberer` c
+00001f60: 6f6d 6573 2077 6974 6820 736f 6d65 2063  omes with some c
+00001f70: 6f72 6520 7374 796c 696e 6720 616e 6420  ore styling and 
+00001f80: 7365 6374 696f 6e20 7465 6d70 6c61 7465  section template
+00001f90: 732e 0a49 7420 6973 2065 7870 6563 7465  s..It is expecte
+00001fa0: 6420 7468 6174 2075 7365 7273 2077 696c  d that users wil
+00001fb0: 6c20 6375 7374 6f6d 697a 6520 7468 6569  l customize thei
+00001fc0: 7220 646f 6375 6d65 6e74 2074 656d 706c  r document templ
+00001fd0: 6174 6573 2062 6579 6f6e 6420 7768 6174  ates beyond what
+00001fe0: 0a69 7320 7072 6f76 6964 6564 2e20 4173  .is provided. As
+00001ff0: 2073 7563 682c 2074 6865 2060 6c69 6d62   such, the `limb
+00002000: 6572 6572 2063 7265 6174 6560 2063 6f6d  erer create` com
+00002010: 6d61 6e64 2073 7570 706f 7274 7320 6120  mand supports a 
+00002020: 602d 7420 3c70 6174 683e 600a 6f70 7469  `-t <path>`.opti
+00002030: 6f6e 2074 6f20 6765 6e65 7261 7465 2061  on to generate a
+00002040: 206e 6577 2070 726f 6a65 6374 2066 726f   new project fro
+00002050: 6d20 6120 6769 7665 6e20 7465 6d70 6c61  m a given templa
+00002060: 7465 2070 726f 6a65 6374 2064 6972 6563  te project direc
+00002070: 746f 7279 2e0a 0a47 656e 6572 616c 6c79  tory...Generally
+00002080: 2073 7065 616b 696e 672c 2074 6865 2073   speaking, the s
+00002090: 7479 6c69 6e67 2079 6f75 2077 616e 7420  tyling you want 
+000020a0: 746f 2075 7365 2069 7320 7570 2074 6f20  to use is up to 
+000020b0: 796f 752e 2048 6f77 6576 6572 2c20 666f  you. However, fo
+000020c0: 720a 636f 6e76 656e 6965 6e63 652c 2074  r.convenience, t
+000020d0: 6865 2043 5353 2069 7320 6f72 6761 6e69  he CSS is organi
+000020e0: 7a65 6420 6173 2060 636f 7265 602c 2060  zed as `core`, `
+000020f0: 7374 796c 6560 2c20 616e 6420 6063 7573  style`, and `cus
+00002100: 746f 6d60 2e20 5468 6520 696e 7465 6e74  tom`. The intent
+00002110: 0a69 7320 666f 7220 7468 6520 6061 7373  .is for the `ass
+00002120: 6574 732f 636f 7265 2e63 7373 6020 746f  ets/core.css` to
+00002130: 2063 6f76 6572 2074 6865 206d 6169 6e20   cover the main 
+00002140: 6c61 796f 7574 2061 6e64 2066 756e 6374  layout and funct
+00002150: 696f 6e69 6e67 206f 6620 7468 650a 646f  ioning of the.do
+00002160: 6375 6d65 6e74 2c20 7468 6520 6061 7373  cument, the `ass
+00002170: 6574 732f 7374 796c 652e 6373 7360 2074  ets/style.css` t
+00002180: 6f20 636f 7665 7220 6772 6f75 7020 7468  o cover group th
+00002190: 656d 696e 6720 666f 7220 636f 6e73 6973  eming for consis
+000021a0: 7465 6e63 792c 2061 6e64 0a60 6375 7374  tency, and.`cust
+000021b0: 6f6d 2f63 7573 746f 6d2e 6373 7360 2074  om/custom.css` t
+000021c0: 6f20 6265 2066 6f72 2061 6e79 2070 6572  o be for any per
+000021d0: 2d64 6f63 756d 656e 742f 7072 6f6a 6563  -document/projec
+000021e0: 7420 7374 796c 696e 672e 0a0a 2323 2054  t styling...## T
+000021f0: 6f64 6f20 4c69 7374 0a0a 2a20 5375 7070  odo List..* Supp
+00002200: 6f72 7420 666f 7220 6375 7374 6f6d 204d  ort for custom M
+00002210: 7573 7461 6368 652d 6765 6e65 7261 7465  ustache-generate
+00002220: 6420 4353 530a 2a20 5265 646f 2063 6f6e  d CSS.* Redo con
+00002230: 7469 6775 6f75 7320 7365 6374 696f 6e73  tiguous sections
+00002240: 0a2a 2042 6574 7465 7220 666f 6f74 6e6f  .* Better footno
+00002250: 7465 730a 2a20 4472 6166 7420 6275 696c  tes.* Draft buil
+00002260: 6473 0a2a 2050 6172 7469 616c 2062 7569  ds.* Partial bui
+00002270: 6c64 7320 6f66 2069 6e64 6976 6964 7561  lds of individua
+00002280: 6c20 7365 6374 696f 6e73 0a2a 2053 7570  l sections.* Sup
+00002290: 706f 7274 2066 6f72 206e 6f6e 2d4d 6172  port for non-Mar
+000022a0: 6b64 6f77 6e20 7365 6374 696f 6e73 0a0a  kdown sections..
+000022b0: 2323 2046 4151 0a0a 3e20 5768 793f 0a0a  ## FAQ..> Why?..
+000022c0: 466f 7220 6120 6c69 7461 6e79 206f 6620  For a litany of 
+000022d0: 7265 6173 6f6e 732c 2062 7574 2069 6620  reasons, but if 
+000022e0: 4920 6861 6420 746f 2067 6f20 6f75 7420  I had to go out 
+000022f0: 6f6e 2061 206c 696d 6220 616e 6420 7069  on a limb and pi
+00002300: 636b 206f 6e65 2c20 6974 0a77 6f75 6c64  ck one, it.would
+00002310: 2062 6520 7468 6174 204c 6154 6558 2069   be that LaTeX i
+00002320: 7320 6120 6772 6561 7420 7479 7065 7365  s a great typese
+00002330: 7474 6572 2c20 6275 7420 6120 7465 7272  tter, but a terr
+00002340: 6962 6c65 2062 7569 6c64 2073 7973 7465  ible build syste
+00002350: 6d2e 0a0a 3e20 5768 6174 213f 0a0a 4772  m...> What!?..Gr
+00002360: 6565 747a 2074 6f20 6173 6368 2c20 7461  eetz to asch, ta
+00002370: 6e6e 6572 2c20 6167 7261 6e74 2c20 6a62  nner, agrant, jb
+00002380: 6c61 747a 2c20 616e 6420 6474 6869 656c  latz, and dthiel
+00002390: 2e20 3c33 0a                             . <3.
```

### Comparing `limberer-0.3.4/pyproject.toml` & `limberer-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.3.4"
+version = "0.4"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.3.4/src/limberer/__init__.py` & `limberer-0.4/src/limberer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,38 +99,41 @@
     n //= 26
   r = []
   for _d in d[::-1]:
     r.append(alph[_d])
   r[-1] = chr(65+d[0])
   return ''.join(r)
 
-def convert(path, opts, toc, args):
+#def convert(path, opts, toc, args):
+def convert(content, opts, toc, args):
   global headercount
   global appendix_count
   #print("convert(" + repr(path) + ")")
-  proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
+  #proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
+  proc1 = subprocess.run(['pandoc', '-t', 'json', '-f', 'markdown'],
+                         input=content, text=True, capture_output=True)
   if proc1.returncode != 0:
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.buffer.write(proc1.stderr)
     sys.stderr.write("\n")
     sys.exit(1)
-  o1 = proc1.stdout.decode('utf-8')
+  o1 = proc1.stdout
 
   if args.debug:
     print(o1)
 
   # run the panflute filter
   sys.argv = ["html"]
   iw = io.StringIO(o1)
   ow = io.StringIO("")
 
   headers = []
   _headers = []
   _meta = []
-  r = entrypoint(iw, ow, headercount, _headers, _meta)
+  r = entrypoint(iw, ow, headercount, _headers, _meta, opts['config'])
   opts.update(_meta[0][0])
   ow.seek(0)
   o2 = ow.read()
 
   if len(_headers) == 1:
     headers = _headers[0]
     headercount += len(headers)
@@ -188,16 +191,19 @@
   build = subparsers.add_parser('build')
   parser.add_argument('-d', '--debug', action='store_true',
                       help='Debug output.')
   build.add_argument('-E', '--emit-html', metavar='<path>', type=str,
                      default="",
                      help='Emit post-processed HTML to <path>.')
 
-  build.add_argument('config', metavar='<config>', type=str,
-                      help="Path to document toml configuration file.")
+  #build.add_argument('config', metavar='<config>', type=str,
+  #                    help="Path to document toml configuration file.")
+  build.add_argument('configs', metavar='<configs...>', nargs='+', type=str,
+                      help="Paths to document toml configuration files.")
+
   args = parser.parse_args()
   return args
 
 def main():
   args = parse_args()
 
   if args.command == "build":
@@ -229,28 +235,39 @@
                 os.path.join(absprojpath, projname + ".toml"))
 
 def build(args):
   global footnotecount
   global appendix
   global appendix_count
 
-  config = args.config
+  config = args.configs[0]
   if not os.path.exists(config):
     sys.stderr.write(f"error: '{config}' not found.\n")
     sys.exit(1)
   if not os.path.isfile(config):
     sys.stderr.write(f"error: '{config}' is not a file.\n")
     sys.exit(1)
 
   dir, fname = os.path.split(config)
   wd = os.getcwd()
   if dir != "":
     os.chdir(dir)
 
-  config = toml.loads(open(fname, 'r').read())
+  config = {
+    "highlight": "molokai",
+    "highlight_plaintext": "solarized-dark",
+    "highlight_font": "'DejaVu Sans Mono', monospace",
+    "highlight_style": "padding: 1rem; border-radius: 2px; overflow-x: auto;",
+    "highlight_line_length": "74",
+  }
+
+  config = config | toml.loads(open(fname, 'r').read())
+  for path in args.configs[1:]:
+    config = config | toml.loads(open(path, 'r').read())
+
   config['config'] = config # we occasionally need top.down.variable.paths to resolve abiguity
 
   base_template = open('templates/base.html', 'r').read()
   section_template = open('templates/section.html', 'r').read()
   toc_template = open('templates/toc.html', 'r').read()
 
   body = ''
@@ -259,20 +276,25 @@
   toc = []
 
   for i in range(len(config['sections'])):
     section = config['sections'][i]
     if section['type'] == 'section':
       section_name = section['name']
       section_path = 'sections/{}.md'.format(section['name'])
-      content = open_subpath(section_path, 'rb').read()
+      raw_content = open_subpath(section_path, 'r').read()
+
       opts = {} | section
+      opts['config'] = config
       opts['section_name'] = section_name
       if appendix:
         opts['appendix'] = True
-      html = convert(section_path, opts, toc, args)
+
+      content = chevron.render(raw_content, opts)
+      html = convert(content, opts, toc, args)
+
       if appendix:
         appendix_count += 1
       footnotes = ""
       soup = BeautifulSoup(html, 'html.parser')
       _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
       for _sn in _sns:
         _snc = [c for c in _sn.children if c != "\n"]
```

### Comparing `limberer-0.3.4/src/limberer/pf.py` & `limberer-0.4/src/limberer/pf.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import base64
 from PIL import Image
 
 titlecounter = 0
 headers = []
 metadata = []
 figurecount = 1
+args = None
 
 def stringify(content):
   out = []
   for part in content:
     if isinstance(part, pf.Str):
       out.append(str(part)[4:-1])
     elif isinstance(part, pf.Space):
@@ -81,19 +82,21 @@
       if lang == 'txt':
         if platform.system() == "Darwin":
           lang = 'shellscript'
         else:
           lang = 'sh'
 
     argv = ['highlight']
-    argv += ['-s', 'solarized-dark' if lang == 'txt' or lang == 'console' else 'molokai']
+    argv += ['-s', config['highlight_plaintext'] if lang == 'txt' or lang == 'console' else config['highlight']]
     argv += ['-O' , 'html']
     argv += ['--inline-css']
     argv += ['-S' , lang]
-    argv += ['--font' , "'DejaVu Sans Mono', monospace; padding: 1rem; border-radius: 2px; overflow-x: auto"]
+    argv += ['--font' , f"{config['highlight_font']}; {config['highlight_style']}"]
+    argv += ['-V', '-J' , config['highlight_line_length']]
+    #argv += ['-l', '-j', "3"] # probably best to do line numbers in css
     argv += ['-f' , '--enclose-pre']
 
     #print(argv)
     proc = subprocess.run(argv, input=code, capture_output=True)
     if proc.returncode != 0:
       sys.stderr.write("highlight returned non-zero for {}\n".format(argv))
       sys.stderr.buffer.write(proc.stderr)
@@ -167,25 +170,28 @@
         return pf.RawInline(html, format='html')
       else:
         sys.stderr.write("image path bad: " + f + "\n")
         sys.stderr.write(os.path.realpath(f) + "\n")
         sys.stderr.write(os.path.join(os.path.realpath('.'), f) + "\n")
   return elem
 
-def entrypoint(_in=None, _out=None, _headercount=0, _headers=None, _meta=None):
+def entrypoint(_in=None, _out=None, _headercount=0, _headers=None, _meta=None, _config=None):
   global headers
   global metadata
   global headercount
+  global config
   headers = []
   if _in is None:
     pf.run_filter(header)
   else:
     if _headers != None:
       _headers.append(headers)
     if _meta != None:
       metadata = []
       _meta.append(metadata)
+    if _config != None:
+      config = _config
     headercount = _headercount
     return pf.run_filter(header, input_stream=_in, output_stream=_out)
 
 if __name__ == "__main__":
   entrypoint()
```

### Comparing `limberer-0.3.4/src/limberer/static/assets/core.css` & `limberer-0.4/src/limberer/static/assets/core.css`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/assets/logo.svg` & `limberer-0.4/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/assets/style.css` & `limberer-0.4/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/images/test1.jpg` & `limberer-0.4/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/sections/example.md` & `limberer-0.4/src/limberer/static/sections/example.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 toc_header_level: 2
 ---
 
-# Examplely Example
+# Examplely Example: {{config.title}}
 
 # Examplely Example
 
 <h2 id="wat">Hello World - not picked up by the ToC due to inline html</h2>
 
 ### Not in the ToC due to H3
 
@@ -36,14 +36,26 @@
 ```js
 let j = await fetch("https://wat.wat", {
   "headers": {
     "x-test": "foo"
   }
 }).then((res)=>res.json());
 ```
+<center>Example Snippet of Code</center>
+
+<div class="pagebreak"></div>
+
+```js
+let j = await fetch("https://wat.wat", {
+  "headers": {
+    "x-test": "foo"
+  }
+}).then((res)=>res.json());
+```
+<figure><figcaption>Example Snippet of Code</figcaption></figure>
 
 ## Table Test
 
 <table>
   <thead>
     <tr>
       <th style="width: 20%">a</th>
```

#### html2text {}

```diff
@@ -1,17 +1,21 @@
---- toc_header_level: 2 --- # Examplely Example # Examplely Example
+--- toc_header_level: 2 --- # Examplely Example: {{config.title}} # Examplely
+Example
 ***** Hello World - not picked up by the ToC due to inline html *****
 ### Not in the ToC due to H3 Hi there. * some[^aaa] * bullets[^bbb] * #Example
 [^ccc] * #Example * [^ddd] * xref_to_Example2.AAA * [xref to Example2.AAA]
 (#example2-aaah2){.xref} *  * [](#example2-aaah2){.xrefn} * xref_to
 Example2.AAA * [xref to Example2.AAA](#example2-aaah2){.xrefpg} *  * []
 (#example2-aaah2){.xrefn .xrefpg} [^aaa]:
 example.com> [^bbb]: wat [^ccc]: wat2
 foo [^ddd]: wat3 ## Code Snippet ```js let j = await fetch("https://wat.wat",
-{ "headers": { "x-test": "foo" } }).then((res)=>res.json()); ``` ## Table Test
+{ "headers": { "x-test": "foo" } }).then((res)=>res.json()); ```
+                            Example Snippet of Code
+```js let j = await fetch("https://wat.wat", { "headers": { "x-test": "foo" }
+}).then((res)=>res.json()); ``` Example Snippet of Code ## Table Test
 a                b              c            d
 table _body_     * table bullet ``` test ``` if we place the above ` `/`
 Test             Hello; world!
    1. Table list
    2. foo
    1. Table list
    2. foo
```

### Comparing `limberer-0.3.4/src/limberer/static/sections/example2.md` & `limberer-0.4/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/templates/cover.html` & `limberer-0.4/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer/static/templates/toc.html` & `limberer-0.4/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.3.4/src/limberer.egg-info/PKG-INFO` & `limberer-0.4/src/limberer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.3.4
+Version: 0.4
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -115,15 +115,15 @@
 `section` template will be used to write document content. For such
 `type = "section"` sections, the content will be sourced from a (currently)
 Markdown file based on the section `name` value (`sections/<name>.md`). By
 default, sections will be rendered against the `template/section.html`
 template, but the template used can be changed via an `alt = "othertemplate"`
 section list setting.
 
-### Project TOML
+### Project TOML Example
 
 ```toml
 title = "Example Document"
 subheading = "..."
 #globaloption=value
 #...
 
@@ -137,14 +137,22 @@
   { type = "toc" },
   { name = "example", type = "section" },
   { name = "example2", type = "section", sectionoption = "value" },
   ...
 ]
 ```
 
+Additional or overriding settings or Mustache template variables can be
+configured by passing additional TOML file paths into the `limberer build`
+command:
+
+```
+$ limberer build report.toml stats.toml
+```
+
 ### Section Templates
 
 Out of the box, `limberer` comes with some initial section templates:
 
 * `cover`: A title page section.
 * `toc`: A table of contents section.
 * `section`: The underlying template for custom sections.
@@ -154,16 +162,17 @@
 * `appendix_start`: Subsequent sections will be treated as appendices.
 * `appendix_end`: Disables the above setting; subsequent sections are not
   treated as appendices. The appendix counter will not be cleared.
 
 ### Custom Sections
 
 Custom sections ("sections") are a mix of Markdown (and, in some cases, HTML),
-where most document content is written. A section can begin with a block of
-Markdown metadata:
+with support for Mustache expressions (using the TOML configuration), where
+most document content is written. A section can begin with a block of Markdown
+metadata:
 
 ```markdown
 ---
 toc_header_level: 2
 columns: true
 title: Example3
 classes: foo bar baz
@@ -304,14 +313,45 @@
 * `.xrefpg`: This will add a " on page XX".
 
   ```
   * <a class="xrefn xrefpg" href="#example2-aaah2"></a>
   * [](#example2-aaah2){.xrefn .xrefpg}
   ```
 
+#### Code Blocks
+
+
+````markdown
+```js
+let j = await fetch("https://wat.wat", {
+  "headers": {
+    "x-test": "foo"
+  }
+}).then((res)=>res.json());
+```
+<center>Example Snippet of Code</center>
+
+```js
+let j = await fetch("https://wat.wat", {
+  "headers": {
+    "x-test": "foo"
+  }
+}).then((res)=>res.json());
+```
+<figure><figcaption>Example Snippet of Code with a figure prefix</figcaption></figure>
+````
+
+The following settings can be configured in the project TOML:
+
+* `highlight` (defaults to `"molokai"`)
+* `highlight_plaintext` (defaults to `"solarized-dark"`)
+* `highlight_font` (defaults to `"'DejaVu Sans Mono', monospace"`)
+* `highlight_style` (defaults to `"padding: 1rem; border-radius: 2px; overflow-x: auto;"`
+* `highlight_line_length` (defaults to `"74"`)
+
 #### Breaks
 
 The following can be added to force a break.
 
 ```html
 <div class="pagebreak"></div>
 ```
@@ -342,14 +382,17 @@
 convenience, the CSS is organized as `core`, `style`, and `custom`. The intent
 is for the `assets/core.css` to cover the main layout and functioning of the
 document, the `assets/style.css` to cover group theming for consistency, and
 `custom/custom.css` to be for any per-document/project styling.
 
 ## Todo List
 
+* Support for custom Mustache-generated CSS
+* Redo contiguous sections
+* Better footnotes
 * Draft builds
 * Partial builds of individual sections
 * Support for non-Markdown sections
 
 ## FAQ
 
 > Why?
```

### Comparing `limberer-0.3.4/src/limberer.egg-info/SOURCES.txt` & `limberer-0.4/src/limberer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

