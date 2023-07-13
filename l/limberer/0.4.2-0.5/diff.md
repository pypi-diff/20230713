# Comparing `tmp/limberer-0.4.2.tar.gz` & `tmp/limberer-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limberer-0.4.2.tar", last modified: Thu Jul 13 08:54:04 2023, max compression
+gzip compressed data, was "limberer-0.5.tar", last modified: Thu Jul 13 10:54:32 2023, max compression
```

## Comparing `limberer-0.4.2.tar` & `limberer-0.5.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.206291 limberer-0.4.2/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.4.2/AUTHORS
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.4.2/LICENSE
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.4.2/MANIFEST.in
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11555 2023-07-13 08:54:04.206291 limberer-0.4.2/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     9493 2023-07-13 08:49:40.000000 limberer-0.4.2/README.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1094 2023-07-13 08:53:41.000000 limberer-0.4.2/pyproject.toml
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-13 08:54:04.206291 limberer-0.4.2/setup.cfg
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    14025 2023-07-13 08:32:00.000000 limberer-0.4.2/src/limberer/__init__.py
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     6970 2023-07-13 01:06:50.000000 limberer-0.4.2/src/limberer/pf.py
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/assets/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-13 08:39:37.000000 limberer-0.4.2/src/limberer/static/assets/core.css
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.4.2/src/limberer/static/assets/logo.svg
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.4.2/src/limberer/static/assets/style.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/custom/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.4.2/src/limberer/static/custom/custom.css
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/images/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.4.2/src/limberer/static/images/test1.jpg
--rw-r--r--   0 jtd       (1000) jtd       (1000)      380 2023-07-13 08:31:33.000000 limberer-0.4.2/src/limberer/static/project.toml
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/sections/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     4168 2023-07-13 08:53:35.000000 limberer-0.4.2/src/limberer/static/sections/example.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.4.2/src/limberer/static/sections/example2.md
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       21 2023-07-13 08:31:10.000000 limberer-0.4.2/src/limberer/static/sections/example3.md
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer/static/templates/
--rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.4.2/src/limberer/static/templates/base.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.4.2/src/limberer/static/templates/cover.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      381 2023-07-06 06:48:22.000000 limberer-0.4.2/src/limberer/static/templates/section.html
--rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.4.2/src/limberer/static/templates/toc.html
-drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 08:54:04.202291 limberer-0.4.2/src/limberer.egg-info/
--rw-rw-r--   0 jtd       (1000) jtd       (1000)    11555 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/PKG-INFO
--rw-rw-r--   0 jtd       (1000) jtd       (1000)      816 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/SOURCES.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/dependency_links.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/entry_points.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/requires.txt
--rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-13 08:54:04.000000 limberer-0.4.2/src/limberer.egg-info/top_level.txt
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      104 2023-06-27 23:50:47.000000 limberer-0.5/AUTHORS
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1296 2023-06-28 11:15:36.000000 limberer-0.5/LICENSE
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       47 2023-06-28 03:48:05.000000 limberer-0.5/MANIFEST.in
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11553 2023-07-13 10:54:32.861741 limberer-0.5/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     9493 2023-07-13 08:49:40.000000 limberer-0.5/README.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1092 2023-07-13 10:49:15.000000 limberer-0.5/pyproject.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       38 2023-07-13 10:54:32.861741 limberer-0.5/setup.cfg
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    14252 2023-07-13 10:51:38.000000 limberer-0.5/src/limberer/__init__.py
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     6970 2023-07-13 01:06:50.000000 limberer-0.5/src/limberer/pf.py
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/assets/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     5711 2023-07-13 08:39:37.000000 limberer-0.5/src/limberer/static/assets/core.css
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    20981 2023-07-03 09:59:46.000000 limberer-0.5/src/limberer/static/assets/logo.svg
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      600 2023-07-04 03:25:09.000000 limberer-0.5/src/limberer/static/assets/style.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/custom/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        0 2023-06-28 04:15:05.000000 limberer-0.5/src/limberer/static/custom/custom.css
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/images/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    47100 2023-07-03 20:54:18.000000 limberer-0.5/src/limberer/static/images/test1.jpg
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      567 2023-07-13 10:52:45.000000 limberer-0.5/src/limberer/static/project.toml
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/sections/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      243 2023-07-13 10:52:22.000000 limberer-0.5/src/limberer/static/sections/configexample.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      179 2023-07-13 10:52:22.000000 limberer-0.5/src/limberer/static/sections/configexample1.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      164 2023-07-13 10:52:22.000000 limberer-0.5/src/limberer/static/sections/configexample2.toml
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     4168 2023-07-13 08:53:35.000000 limberer-0.5/src/limberer/static/sections/example.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)     1659 2023-07-06 07:43:06.000000 limberer-0.5/src/limberer/static/sections/example2.md
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       21 2023-07-13 08:31:10.000000 limberer-0.5/src/limberer/static/sections/example3.md
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer/static/templates/
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      333 2023-07-03 23:25:48.000000 limberer-0.5/src/limberer/static/templates/base.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      752 2023-06-28 13:19:57.000000 limberer-0.5/src/limberer/static/templates/cover.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      438 2023-07-13 10:52:11.000000 limberer-0.5/src/limberer/static/templates/section.html
+-rw-r--r--   0 jtd       (1000) jtd       (1000)      678 2023-07-06 06:32:49.000000 limberer-0.5/src/limberer/static/templates/toc.html
+drwxrwxr-x   0 jtd       (1000) jtd       (1000)        0 2023-07-13 10:54:32.861741 limberer-0.5/src/limberer.egg-info/
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)    11553 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/PKG-INFO
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)      960 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        1 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       43 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/entry_points.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)       55 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/requires.txt
+-rw-rw-r--   0 jtd       (1000) jtd       (1000)        9 2023-07-13 10:54:32.000000 limberer-0.5/src/limberer.egg-info/top_level.txt
```

### Comparing `limberer-0.4.2/LICENSE` & `limberer-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/PKG-INFO` & `limberer-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.4.2
+Version: 0.5
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.4.2/README.md` & `limberer-0.5/README.md`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/pyproject.toml` & `limberer-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "limberer"
-version = "0.4.2"
+version = "0.5"
 authors = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 maintainers = [
   { name = "Jeff Dileo", email = "jtdileo@gmail.com" },
 ]
 license = { file = "LICENSE" }
```

### Comparing `limberer-0.4.2/src/limberer/__init__.py` & `limberer-0.5/src/limberer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,41 @@
   cwd = os.path.abspath(".")
   target = os.path.abspath(path)
   if not target.startswith(cwd + os.sep):
     print(f"error: invalid path {repr(path)} references outside of project directory.")
     sys.exit(1)
   return open(path, mode)
 
+def parse_args():
+  parser = argparse.ArgumentParser(
+    description='A flexible document generator based on WeasyPrint, mustache templates, and Pandoc.'
+  )
+  parser.add_argument('-d', '--debug', action='store_true',
+                      help='Debug output.')
+  subparsers = parser.add_subparsers(dest='command', required=True,
+                                     title='subcommands',
+                                     description='valid subcommands',
+                                     help='additional help')
+
+  create = subparsers.add_parser('create')
+  create.add_argument('project', metavar='<project>', type=str,
+                      help="Name of project to create.")
+  create.add_argument('-t', '--template', metavar='<path>', type=str,
+                      default="",
+                      help='Create from alternative template path instead of the built-in default.')
+  build = subparsers.add_parser('build')
+  build.add_argument('-E', '--emit-html', metavar='<path>', type=str,
+                     default="",
+                     help='Emit post-processed HTML to <path>.')
+  build.add_argument('configs', metavar='<configs...>', nargs='+', type=str,
+                      help="Paths to document toml configuration files.")
+
+  args = parser.parse_args()
+  return args
+
 footnotecount = 1
 isheader = re.compile('h[1-9]')
 headercount = 0
 appendix = False
 appendix_count = 0
 
 alph = "AABCDEFGHIJKLMNOPQRSTUVWXYZ"
@@ -99,31 +126,28 @@
     n //= 26
   r = []
   for _d in d[::-1]:
     r.append(alph[_d])
   r[-1] = chr(65+d[0])
   return ''.join(r)
 
-#def convert(path, opts, toc, args):
 def convert(content, opts, toc, args):
   global headercount
   global appendix_count
-  #print("convert(" + repr(path) + ")")
-  #proc1 = subprocess.run(['pandoc', '-t', 'json', path], capture_output=True)
   proc1 = subprocess.run(['pandoc', '-t', 'json', '-f', 'markdown'],
                          input=content, text=True, capture_output=True)
   if proc1.returncode != 0:
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.buffer.write(proc1.stderr)
     sys.stderr.write("\n")
     sys.exit(1)
   o1 = proc1.stdout
 
-  if args.debug:
-    print(o1)
+  #if args.debug:
+  #  print(o1)
 
   # run the panflute filter
   sys.argv = ["html"]
   iw = io.StringIO(o1)
   ow = io.StringIO("")
 
   headers = []
@@ -168,44 +192,60 @@
     sys.stderr.write("error running initial pandoc command: \n")
     sys.stderr.write(proc2.stderr)
     sys.stderr.write("\n")
     sys.exit(1)
   content = proc2.stdout
   return content
 
+def convert_fancy(content, section_name, opts, toc, args):
+  global appendix_count
+  global footnotecount
 
-def parse_args():
-  parser = argparse.ArgumentParser(
-    description='A flexible document generator based on WeasyPrint, mustache templates, and Pandoc.'
-  )
-  subparsers = parser.add_subparsers(dest='command', required=True,
-                                     title='subcommands',
-                                     description='valid subcommands',
-                                     help='additional help')
-
-  create = subparsers.add_parser('create')
-  create.add_argument('project', metavar='<project>', type=str,
-                      help="Name of project to create.")
-  create.add_argument('-t', '--template', metavar='<path>', type=str,
-                      default="",
-                      help='Create from alternative template path instead of the built-in default.')
-  build = subparsers.add_parser('build')
-  parser.add_argument('-d', '--debug', action='store_true',
-                      help='Debug output.')
-  build.add_argument('-E', '--emit-html', metavar='<path>', type=str,
-                     default="",
-                     help='Emit post-processed HTML to <path>.')
+  if args.debug:
+    opts['debug_markdown'] = content
 
-  #build.add_argument('config', metavar='<config>', type=str,
-  #                    help="Path to document toml configuration file.")
-  build.add_argument('configs', metavar='<configs...>', nargs='+', type=str,
-                      help="Paths to document toml configuration files.")
+  html = convert(content, opts, toc, args)
 
-  args = parser.parse_args()
-  return args
+  if appendix:
+    appendix_count += 1
+  footnotes = ""
+  soup = BeautifulSoup(html, 'html.parser')
+  _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
+  for _sn in _sns:
+    _snc = [c for c in _sn.children if c != "\n"]
+    if len(_snc) > 0:
+      if re.match(isheader, _snc[0].name):
+        _snc[0]['id'] = _sn['id']
+        del _sn['id']
+  _iders = soup.find_all(lambda e: e.name != 'article' and e.attrs.get('id')!=None)
+  for _ider in _iders:
+    _ider['id'] = f"{section_name}-{_ider['id']}"
+
+  _fns = soup.find(class_="footnotes")
+  if _fns is not None:
+    _fns = _fns.extract()
+    _fns.ol['start'] = str(footnotecount)
+    _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
+    __fns = [c for c in _fns.ol.children if c != "\n"]
+    del _fns['id']
+    for _a in soup.find_all(class_="footnote-ref"):
+      _a['href'] = f"#{section_name}-{_a['href'][1:]}"
+      _a.sup.string = str(footnotecount - 1 + int(_a.sup.string))
+    for _a in _fns.find_all(class_="footnote-back"):
+      _a['href'] = f"#{section_name}-{_a['href'][1:]}"
+    _fns.name = 'div'
+    footnotecount += len(__fns)
+
+    footnotes = str(_fns)
+  html = str(soup)
+
+  opts['html'] = html
+  opts['footnotes'] = footnotes
+  opts['opts'] = opts # we occasionally need top.down.variable.paths to resolve abiguity
+  return html
 
 def main():
   args = parse_args()
 
   if args.command == "build":
     build(args)
   elif args.command == "create":
@@ -278,82 +318,48 @@
   for i in range(len(config['sections'])):
     section = config['sections'][i]
     if section['type'] == 'section':
       if section.get('cont', False) == True:
         continue
       section_name = section['name']
       section_path = 'sections/{}.md'.format(section['name'])
+
       raw_content = open_subpath(section_path, 'r').read()
+
+      opts = {} | section
+      opts['config'] = config
+      opts['section_name'] = section_name
+
+      if "conf" in section:
+        opts = opts | toml.loads(open_subpath(section['conf'], 'r').read())
+      if appendix:
+        opts['appendix'] = True
+      content = chevron.render(raw_content, opts)
+
       for j in range(i+1, len(config['sections'])):
         _section = config['sections'][j]
         if _section['type'] != 'section' or _section.get('cont', False) != True:
           break
         _section_name = _section['name']
         _section_path = 'sections/{}.md'.format(_section['name'])
         _raw_content = open_subpath(_section_path, 'r').read()
-        raw_content += "\n\n"
-        raw_content += _raw_content
 
-      opts = {} | section
-      opts['config'] = config
-      opts['section_name'] = section_name
-      if appendix:
-        opts['appendix'] = True
+        _opts = {} | _section
+        _opts['config'] = config
+        _opts['section_name'] = _section_name
+
+        if "conf" in _section:
+          _opts = _opts | toml.loads(open_subpath(_section['conf'], 'r').read())
+        _content = chevron.render(_raw_content, _opts)
 
-      content = chevron.render(raw_content, opts)
-      html = convert(content, opts, toc, args)
+        content += "\n\n"
+        content += _content
+
+      html = convert_fancy(content, section_name, opts, toc, args)
 
-      if appendix:
-        appendix_count += 1
-      footnotes = ""
-      soup = BeautifulSoup(html, 'html.parser')
-      _sns = soup.find_all(lambda e: e.name == 'section' and e.attrs.get('id')!=None)
-      for _sn in _sns:
-        _snc = [c for c in _sn.children if c != "\n"]
-        if len(_snc) > 0:
-          if re.match(isheader, _snc[0].name):
-            _snc[0]['id'] = _sn['id']
-            del _sn['id']
-      _iders = soup.find_all(lambda e: e.name != 'article' and e.attrs.get('id')!=None)
-      for _ider in _iders:
-        _ider['id'] = f"{section_name}-{_ider['id']}"
-
-      _fns = soup.find(class_="footnotes")
-      if _fns is not None:
-        _fns = _fns.extract()
-        _fns.ol['start'] = str(footnotecount)
-        _fns.ol['style'] = f"counter-reset:list-item {footnotecount}; counter-increment:list-item -1;"
-        __fns = [c for c in _fns.ol.children if c != "\n"]
-        del _fns['id']
-        # we already converted all of them above
-        #for __fn in __fns:
-        #  id = __fn['id']
-        #  print("__fn['id']: " + repr(id))
-        #  nid = f"{section_name}-{id}"
-        #  __fn['id'] = nid
-        #  __fnx = soup.find(id=id)
-        #  print("__fnx: " + repr(__fnx))
-        #  if __fnx is not None:
-        #    __fnx['id'] = nid
-        for _a in soup.find_all(class_="footnote-ref"):
-          # we already converted all of them above
-          #_a['id'] = f"{section_name}-{_a['id']}"
-          _a['href'] = f"#{section_name}-{_a['href'][1:]}"
-          _a.sup.string = str(footnotecount - 1 + int(_a.sup.string))
-        for _a in _fns.find_all(class_="footnote-back"):
-          _a['href'] = f"#{section_name}-{_a['href'][1:]}"
-        _fns.name = 'div'
-        footnotecount += len(__fns)
-
-        footnotes = str(_fns)
-      html = str(soup)
-
-      opts['html'] = html
-      opts['footnotes'] = footnotes
-      opts['opts'] = opts # we occasionally need top.down.variable.paths to resolve abiguity
       template = section_template
       if "alt" in section:
         template = open_subpath('templates/{}.html'.format(section['alt']), 'r').read()
       r = chevron.render(template, opts)
       sections.append(r)
     elif section['type'] == 'toc':
       # defer until after we get through everything else
@@ -362,16 +368,31 @@
       appendix = True
     elif section['type'] == 'appendix_end':
       appendix = False
     #elif section['type'] == 'appendix_reset':
     #  appendix_count = 0
     else:
       # assume in templates/
-      template = open_subpath('templates/{}.html'.format(section['type']), 'r').read()
-      r = chevron.render(template, config)
+      format = section.get('format', "html")
+      template = open_subpath(f"templates/{section['type']}.{format}", 'r').read()
+      _config = {} | config | section
+      if "conf" in section:
+        _config = _config | toml.loads(open_subpath(section['conf'], 'r').read())
+      if format == 'md':
+        section_name = section['name']
+        opts = _config
+        opts['config'] = _config
+        opts['section_name'] = section_name
+
+        if appendix:
+          opts['appendix'] = True
+        template = chevron.render(template, opts)
+        template = convert_fancy(template, section_name, opts, toc, args)
+
+      r = chevron.render(template, _config)
       sections.append(r)
       if section['type'] != 'cover' and "title" in section:
         name = section['type']
         ax = {}
         if appendix:
           ax['appendix_n'] = appendixify(appendix_count)
           appendix_count += 1
@@ -386,16 +407,14 @@
         r = chevron.render(toc_template, {"sections": toc})
         body += r
         body += "\n"
 
   config['body'] = body
   report_html = chevron.render(base_template, config)
 
-  if args.debug:
-    print(report_html)
   if args.emit_html != "":
     with open(args.emit_html, 'w') as fd:
       fd.write(report_html)
       fd.flush()
       fd.close()
 
   h = weasyprint.HTML(string=report_html, base_url='./', url_fetcher=fetcher)
```

### Comparing `limberer-0.4.2/src/limberer/pf.py` & `limberer-0.5/src/limberer/pf.py`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/assets/core.css` & `limberer-0.5/src/limberer/static/assets/core.css`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/assets/logo.svg` & `limberer-0.5/src/limberer/static/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/assets/style.css` & `limberer-0.5/src/limberer/static/assets/style.css`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/images/test1.jpg` & `limberer-0.5/src/limberer/static/images/test1.jpg`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/sections/example.md` & `limberer-0.5/src/limberer/static/sections/example.md`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/sections/example2.md` & `limberer-0.5/src/limberer/static/sections/example2.md`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/templates/cover.html` & `limberer-0.5/src/limberer/static/templates/cover.html`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer/static/templates/toc.html` & `limberer-0.5/src/limberer/static/templates/toc.html`

 * *Files identical despite different names*

### Comparing `limberer-0.4.2/src/limberer.egg-info/PKG-INFO` & `limberer-0.5/src/limberer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limberer
-Version: 0.4.2
+Version: 0.5
 Summary: A flexible document generator based on weasyprint, mustache templates, and pandoc.
 Author-email: Jeff Dileo <jtdileo@gmail.com>
 Maintainer-email: Jeff Dileo <jtdileo@gmail.com>
 License: Copyright (c) 2023 Jeff Dileo.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `limberer-0.4.2/src/limberer.egg-info/SOURCES.txt` & `limberer-0.5/src/limberer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 src/limberer.egg-info/top_level.txt
 src/limberer/static/project.toml
 src/limberer/static/assets/core.css
 src/limberer/static/assets/logo.svg
 src/limberer/static/assets/style.css
 src/limberer/static/custom/custom.css
 src/limberer/static/images/test1.jpg
+src/limberer/static/sections/configexample.md
+src/limberer/static/sections/configexample1.toml
+src/limberer/static/sections/configexample2.toml
 src/limberer/static/sections/example.md
 src/limberer/static/sections/example2.md
 src/limberer/static/sections/example3.md
 src/limberer/static/templates/base.html
 src/limberer/static/templates/cover.html
 src/limberer/static/templates/section.html
 src/limberer/static/templates/toc.html
```

