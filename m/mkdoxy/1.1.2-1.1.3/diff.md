# Comparing `tmp/mkdoxy-1.1.2.tar.gz` & `tmp/mkdoxy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.2.tar", last modified: Fri Jun 30 13:15:30 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.3.tar", last modified: Thu Jul 13 15:16:30 2023, max compression
```

## Comparing `mkdoxy-1.1.2.tar` & `mkdoxy-1.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.227069 mkdoxy-1.1.2/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.2/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5072 2023-06-30 13:15:30.226925 mkdoxy-1.1.2/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4344 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.223655 mkdoxy-1.1.2/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.2/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.2/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2841 2023-04-07 16:49:36.000000 mkdoxy-1.1.2/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     4326 2023-06-30 13:10:28.000000 mkdoxy-1.1.2/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    12065 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.2/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    20935 2023-06-30 12:40:39.000000 mkdoxy-1.1.2/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     7661 2023-06-30 13:09:49.000000 mkdoxy-1.1.2/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.226701 mkdoxy-1.1.2/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      351 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4480 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      444 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-06-30 11:43:03.000000 mkdoxy-1.1.2/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-06-30 13:15:30.224305 mkdoxy-1.1.2/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     5072 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      107 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-06-30 13:15:30.000000 mkdoxy-1.1.2/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-06-30 13:15:30.227110 mkdoxy-1.1.2/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1293 2023-06-30 13:12:18.000000 mkdoxy-1.1.2/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.307375 mkdoxy-1.1.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.3/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-13 15:16:30.307116 mkdoxy-1.1.3/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.3/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.294628 mkdoxy-1.1.3/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.3/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.3/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.3/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-07-13 14:02:59.000000 mkdoxy-1.1.3/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4326 2023-06-30 13:10:28.000000 mkdoxy-1.1.3/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-13 14:03:01.000000 mkdoxy-1.1.3/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.3/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.3/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    21270 2023-07-13 14:03:05.000000 mkdoxy-1.1.3/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7660 2023-07-13 13:39:26.000000 mkdoxy-1.1.3/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-13 14:03:06.000000 mkdoxy-1.1.3/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.306417 mkdoxy-1.1.3/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.3/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4572 2023-07-13 13:55:16.000000 mkdoxy-1.1.3/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.3/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-13 14:03:08.000000 mkdoxy-1.1.3/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.296345 mkdoxy-1.1.3/mkdoxy.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      131 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-13 15:16:30.308850 mkdoxy-1.1.3/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1838 2023-07-13 14:53:59.000000 mkdoxy-1.1.3/setup.py
```

### Comparing `mkdoxy-1.1.2/LICENSE` & `mkdoxy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/PKG-INFO` & `mkdoxy-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.2
+Version: 1.1.3
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
+Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
+Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
+Project-URL: Tracker, https://github.com/JakubAndrysek/MkDoxy/issues
+Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-source,documentation,mkdocs,doxygen,multilanguage,code-snippets,code,snippets,documentation-generator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
 
 <p align="center">
@@ -48,29 +53,34 @@
 - **[Code snippets](./snippets/index.md)**: Generate code snippets in place of your standard Markdown documentation.
 - **[Multiple projects](./usage/index.md#multiple-projects)**: Support for multiple projects in one documentation (e.g. C++ and Python).
 - **[Multiple source directories](./usage/index.md#multiple-source-directories)**: Configure multiple source directories in one project.
 - **[Custom Jinja templates](./usage/index.md#custom-jinja-templates)**: Define custom Jinja templates for rendering Doxygen documentation.
 - **[Custom Doxygen configuration](./usage/index.md#custom-doxygen-configuration)**: Specify custom Doxygen configuration for each project.
 
 ## Installation
-With [pip](https://pypi.org/project/mkdoxy/):
+Install the plugin using pip from [PyPI](https://pypi.org/project/mkdoxy/):
+
 ```bash
 pip install mkdoxy
 ```
+Development version with all dependencies:
+```bash
+python -m pip install mkdoxy ".[dev]"
+```
 
-Install from source - development version:
+Install from source:
 ```bash
 pip install git+https://github.com/JakubAndrysek/MkDoxy.git
 ```
 
 ## Quick start
 
 `mkdocs.yml`:
 ```yaml
-site_name: "My documentation"
+site_name: "My MkDoxy documentation"
 
 theme:
   name: material
 
 plugins:
   - search
   - mkdoxy:
@@ -79,14 +89,17 @@
           src-dirs: path/to/src/project1 # path to source code (support multiple paths separated by space) => INPUT
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -1,21 +1,25 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.2 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.3 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
-email@kubaandrysek.cz License: MIT Keywords: mkdoxy,python,open-
+email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
+JakubAndrysek/MkDoxy Project-URL: Documentation, https://
+mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
+MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
+Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **
-[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **
-[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in
-your markdown files.
+Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/
+)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API
+documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **
+[code snippets](/intro)** in your markdown files.
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
 [https://img.shields.io/github/license/JakubAndrysek/MkDoxy?style=flat-square]
    [https://img.shields.io/github/v/release/JakubAndrysek/MkDoxy?style=flat-
  square] [https://img.shields.io/github/stars/JakubAndrysek/MkDoxy?style=flat-
  square] [https://img.shields.io/github/forks/JakubAndrysek/MkDoxy?style=flat-
 square] [https://img.shields.io/github/issues/JakubAndrysek/MkDoxy?style=flat-
@@ -36,23 +40,27 @@
 index.md#multiple-projects)**: Support for multiple projects in one
 documentation (e.g. C++ and Python). - **[Multiple source directories](./usage/
 index.md#multiple-source-directories)**: Configure multiple source directories
 in one project. - **[Custom Jinja templates](./usage/index.md#custom-jinja-
 templates)**: Define custom Jinja templates for rendering Doxygen
 documentation. - **[Custom Doxygen configuration](./usage/index.md#custom-
 doxygen-configuration)**: Specify custom Doxygen configuration for each
-project. ## Installation With [pip](https://pypi.org/project/mkdoxy/): ```bash
-pip install mkdoxy ``` Install from source - development version: ```bash pip
-install git+https://github.com/JakubAndrysek/MkDoxy.git ``` ## Quick start
-`mkdocs.yml`: ```yaml site_name: "My documentation" theme: name: material
-plugins: - search - mkdoxy: projects: myProjectCpp: # name of project must be
-alphanumeric + numbers (without spaces) src-dirs: path/to/src/project1 # path
-to source code (support multiple paths separated by space) => INPUT full-doc:
-True # if you want to generate full documentation doxy-cfg: # standard doxygen
-configuration (key: value) FILE_PATTERNS: "*.cpp *.h*" # specify file patterns
-to filter out RECURSIVE: True # recursive search in source directories ``` ##
-Do You Enjoy MkDoxy or Does It Save You Time? Then definitely consider: -
-supporting me on GitHub Sponsors: [![](https://img.shields.io/static/
+project. ## Installation Install the plugin using pip from [PyPI](https://
+pypi.org/project/mkdoxy/): ```bash pip install mkdoxy ``` Development version
+with all dependencies: ```bash python -m pip install mkdoxy ".[dev]" ```
+Install from source: ```bash pip install git+https://github.com/JakubAndrysek/
+MkDoxy.git ``` ## Quick start `mkdocs.yml`: ```yaml site_name: "My MkDoxy
+documentation" theme: name: material plugins: - search - mkdoxy: projects:
+myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
+src-dirs: path/to/src/project1 # path to source code (support multiple paths
+separated by space) => INPUT full-doc: True # if you want to generate full
+documentation doxy-cfg: # standard doxygen configuration (key: value)
+FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
+True # recursive search in source directories ``` ## Contributing Pull requests
+are welcome. For major changes, please open an issue first to discuss what you
+would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+definitely consider: - supporting me on GitHub Sponsors: [![](https://
+img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.1.2/README.md` & `mkdoxy-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,29 +30,34 @@
 - **[Code snippets](./snippets/index.md)**: Generate code snippets in place of your standard Markdown documentation.
 - **[Multiple projects](./usage/index.md#multiple-projects)**: Support for multiple projects in one documentation (e.g. C++ and Python).
 - **[Multiple source directories](./usage/index.md#multiple-source-directories)**: Configure multiple source directories in one project.
 - **[Custom Jinja templates](./usage/index.md#custom-jinja-templates)**: Define custom Jinja templates for rendering Doxygen documentation.
 - **[Custom Doxygen configuration](./usage/index.md#custom-doxygen-configuration)**: Specify custom Doxygen configuration for each project.
 
 ## Installation
-With [pip](https://pypi.org/project/mkdoxy/):
+Install the plugin using pip from [PyPI](https://pypi.org/project/mkdoxy/):
+
 ```bash
 pip install mkdoxy
 ```
+Development version with all dependencies:
+```bash
+python -m pip install mkdoxy ".[dev]"
+```
 
-Install from source - development version:
+Install from source:
 ```bash
 pip install git+https://github.com/JakubAndrysek/MkDoxy.git
 ```
 
 ## Quick start
 
 `mkdocs.yml`:
 ```yaml
-site_name: "My documentation"
+site_name: "My MkDoxy documentation"
 
 theme:
   name: material
 
 plugins:
   - search
   - mkdoxy:
@@ -61,14 +66,17 @@
           src-dirs: path/to/src/project1 # path to source code (support multiple paths separated by space) => INPUT
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -26,23 +26,27 @@
 index.md#multiple-projects)**: Support for multiple projects in one
 documentation (e.g. C++ and Python). - **[Multiple source directories](./usage/
 index.md#multiple-source-directories)**: Configure multiple source directories
 in one project. - **[Custom Jinja templates](./usage/index.md#custom-jinja-
 templates)**: Define custom Jinja templates for rendering Doxygen
 documentation. - **[Custom Doxygen configuration](./usage/index.md#custom-
 doxygen-configuration)**: Specify custom Doxygen configuration for each
-project. ## Installation With [pip](https://pypi.org/project/mkdoxy/): ```bash
-pip install mkdoxy ``` Install from source - development version: ```bash pip
-install git+https://github.com/JakubAndrysek/MkDoxy.git ``` ## Quick start
-`mkdocs.yml`: ```yaml site_name: "My documentation" theme: name: material
-plugins: - search - mkdoxy: projects: myProjectCpp: # name of project must be
-alphanumeric + numbers (without spaces) src-dirs: path/to/src/project1 # path
-to source code (support multiple paths separated by space) => INPUT full-doc:
-True # if you want to generate full documentation doxy-cfg: # standard doxygen
-configuration (key: value) FILE_PATTERNS: "*.cpp *.h*" # specify file patterns
-to filter out RECURSIVE: True # recursive search in source directories ``` ##
-Do You Enjoy MkDoxy or Does It Save You Time? Then definitely consider: -
-supporting me on GitHub Sponsors: [![](https://img.shields.io/static/
+project. ## Installation Install the plugin using pip from [PyPI](https://
+pypi.org/project/mkdoxy/): ```bash pip install mkdoxy ``` Development version
+with all dependencies: ```bash python -m pip install mkdoxy ".[dev]" ```
+Install from source: ```bash pip install git+https://github.com/JakubAndrysek/
+MkDoxy.git ``` ## Quick start `mkdocs.yml`: ```yaml site_name: "My MkDoxy
+documentation" theme: name: material plugins: - search - mkdoxy: projects:
+myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
+src-dirs: path/to/src/project1 # path to source code (support multiple paths
+separated by space) => INPUT full-doc: True # if you want to generate full
+documentation doxy-cfg: # standard doxygen configuration (key: value)
+FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
+True # recursive search in source directories ``` ## Contributing Pull requests
+are welcome. For major changes, please open an issue first to discuss what you
+would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+definitely consider: - supporting me on GitHub Sponsors: [![](https://
+img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.1.2/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.1.3/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/constants.py` & `mkdoxy-1.1.3/mkdoxy/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 	FRIEND = 'friend'
 	FILE = 'file'
 	DIR = 'dir'
 	PAGE = 'page'
 	EXAMPLE = 'example'
 	GROUP = 'group'
 	INTERFACE = 'interface'
+	SIGNAL = 'signal'
+	SLOT = 'slot'
+	PROPERTY = 'property'
 
 	def is_function(self) -> bool:
 		return self == Kind.FUNCTION
 
 	def is_variable(self) -> bool:
 		return self == Kind.VARIABLE
 
@@ -128,15 +131,18 @@
 			Kind.CLASS,
 			Kind.STRUCT,
 			Kind.TYPEDEF,
 			Kind.ENUM,
 			Kind.ENUMVALUE,
 			Kind.UNION,
 			Kind.INTERFACE,
-			Kind.FRIEND
+			Kind.FRIEND,
+			Kind.SIGNAL,
+			Kind.SLOT,
+			Kind.PROPERTY,
 		]
 
 		return self in LANGUAGE
 
 	def is_parent(self) -> bool:
 		return self in [
 			Kind.NAMESPACE,
```

### Comparing `mkdoxy-1.1.2/mkdoxy/doxygen.py` & `mkdoxy-1.1.3/mkdoxy/doxygen.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/doxyrun.py` & `mkdoxy-1.1.3/mkdoxy/doxyrun.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/finder.py` & `mkdoxy-1.1.3/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.3/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/generatorBase.py` & `mkdoxy-1.1.3/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/generatorSnippets.py` & `mkdoxy-1.1.3/mkdoxy/generatorSnippets.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,20 +68,19 @@
 
 			snippet_config = self.config.copy()
 			snippet_config.update(self.try_load_yaml(match.group('yaml'), project_name, snippet, self.config))
 
 			if self.is_doxy_inactive(snippet_config):
 				continue
 
-			if not self.is_project_exist(project_name):
-				replacement = self.incorrect_project(project_name, snippet_config, snippet)
-			else:
-				replacement = self.incorrect_argument(project_name, "", snippet_config, snippet)
-
-
+			replacement = (
+				self.incorrect_argument(project_name, "", snippet_config, snippet)
+				if self.is_project_exist(project_name)
+				else self.incorrect_project(project_name, snippet_config, snippet)
+			)
 			self.replace_markdown(match.start(), match.end(), replacement)
 
 
 		matches = re.finditer(regexShort, self.markdown, re.MULTILINE)
 		for match in reversed(list(matches)):
 			snippet = match.group()
 			argument = match.group('argument').lower()
```

### Comparing `mkdoxy-1.1.2/mkdoxy/markdown.py` & `mkdoxy-1.1.3/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/node.py` & `mkdoxy-1.1.3/mkdoxy/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 		self._templateparams = Property.TemplateParams(self._xml, parser, self._kind)
 		self._specifiers = Property.Specifiers(self._xml, parser, self._kind)
 		self._values = Property.Values(self._xml, parser, self._kind)
 		self._initializer = Property.Initializer(self._xml, parser, self._kind)
 		self._definition = Property.Definition(self._xml, parser, self._kind)
 		self._programlisting = Property.Programlisting(self._xml, parser, self._kind)
 
+	def __repr__(self):
+		return f"Node: {self.name} refid: {self._refid}"
+
 	def setLinkPrefix(self, linkPrefix: str):
 		self.linkPrefix = linkPrefix
 
 	def add_child(self, child: 'Node'):
 		self._children.append(child)
 
 	def sort_children(self):
@@ -204,15 +207,15 @@
 				if kind.is_language():
 					if self._kind in [Kind.GROUP, Kind.DIR, Kind.FILE]:
 						refid = memberdef.get('id')
 						try:
 							child = self._cache.get(refid)
 							self.add_child(child)
 							continue
-						except:
+						except Exception:
 							pass
 					child = Node(None, memberdef, self._cache, self._parser, self)
 					self.add_child(child)
 
 		# for detaileddescription in self._xml.findall('detaileddescription'):
 		# 	for para in detaileddescription.findall('para'):
 		# 		for programlisting in para.findall('programlisting'):
@@ -243,15 +246,24 @@
 		inline = self._xml.get('inline')
 		self._inline = inline == 'yes'
 
 		const = self._xml.get('inline')
 		self._const = const == 'yes'
 
 		name = self._xml.find('name')
-		self._name = name.text if name is not None else ''
+		if name is not None and name.text:
+			self._name = name.text
+		else:
+			# Doxygen doesn't give anonymous unions any name
+			qualifiedname = self._xml.find('qualifiedname')
+			if qualifiedname is not None and qualifiedname.text:
+				self._name = qualifiedname.text
+			else:
+				self._name = self._refid
+
 		virt = self._xml.get('virt')
 		if virt:
 			self._virtual = virt in ['virtual', 'pure-virtual']
 			self._pure = virt == 'pure-virtual'
 		else:
 			self._virtual = False
 			self._pure = False
```

### Comparing `mkdoxy-1.1.2/mkdoxy/plugin.py` & `mkdoxy-1.1.3/mkdoxy/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,18 +106,18 @@
 			checkConfig(self.config_project, project_data, config['strict'])
 
 			if self.config.get("save-api"):
 				tempDirApi = tempDir("", self.config.get("save-api"), project_name)
 			else:
 				tempDirApi = tempDir(config['site_dir'], "assets/.doxy/", project_name)
 
-			# Check scr changes -> run Doxygen
+			# Check src changes -> run Doxygen
 			doxygenRun = DoxygenRun(self.config['doxygen-bin-path'], project_data.get('src-dirs'), tempDirApi, project_data.get('doxy-cfg', {}))
 			if doxygenRun.checkAndRun():
-				log.info("  -> generating Doxygen filese")
+				log.info("  -> generating Doxygen files")
 			else:
 				log.info("  -> skip generating Doxygen files (nothing changes)")
 
 			# Parse XML to basic structure
 			cache = Cache()
 			parser = XmlParser(cache=cache, debug=self.debug)
```

### Comparing `mkdoxy-1.1.2/mkdoxy/property.py` & `mkdoxy-1.1.3/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/code.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/error.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.3/mkdoxy/templates/member.jinja2`

 * *Files 15% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Files', 'visibility': 'public', 'kinds': ['file'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Directories', 'visibility': 'public', 'kinds': ['dir'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Modules', 'visibility': 'public', 'kinds': ['group'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Namespaces', 'visibility': 'public', 'kinds': ['namespace'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Classes', 'visibility': 'public', 'kinds': ['class', 'struct', 'interface'], 'static': False}) }}
 
 {%- for visibility in ['public', 'protected'] -%}
-{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['functions', ['function']]] -%}
+{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {%- for child in node.base_classes recursive -%}{%- if child is not string %}
 {{ templateMemTab.render({'config': {}, 'node': child, 'parent': node, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {{- loop(child.base_classes)}}
 {%- endif -%}{%- endfor -%}
 {%- endfor -%}
@@ -70,15 +70,15 @@
 {%- if node.has_details %}
 # Detailed Description
 
 {{node.details}}
 {%- endif %}
 
 {%- for visibility in ['public', 'protected'] -%}
-{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['functions', ['function']]] -%}
+{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {%- if node.has(visibility, query[1], static[1]) %}
 ## {{visibility|title}} {{static[0]|title}}{{query[0]|title}} Documentation
 {% for member in node.query(visibility, query[1], static[1]) -%}
 {{ templateMemDef.render({'config': {}, 'node': member, 'configMemDef': configMemDef}) }}
 {%- endfor %}
 {%- endif -%}
```

### Comparing `mkdoxy-1.1.2/mkdoxy/utils.py` & `mkdoxy-1.1.3/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy/xml_parser.py` & `mkdoxy-1.1.3/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.1.3/mkdoxy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.2
+Version: 1.1.3
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
+Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
+Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
+Project-URL: Tracker, https://github.com/JakubAndrysek/MkDoxy/issues
+Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-source,documentation,mkdocs,doxygen,multilanguage,code-snippets,code,snippets,documentation-generator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # MkDoxy
 
 **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in your markdown files.
 
 <p align="center">
@@ -48,29 +53,34 @@
 - **[Code snippets](./snippets/index.md)**: Generate code snippets in place of your standard Markdown documentation.
 - **[Multiple projects](./usage/index.md#multiple-projects)**: Support for multiple projects in one documentation (e.g. C++ and Python).
 - **[Multiple source directories](./usage/index.md#multiple-source-directories)**: Configure multiple source directories in one project.
 - **[Custom Jinja templates](./usage/index.md#custom-jinja-templates)**: Define custom Jinja templates for rendering Doxygen documentation.
 - **[Custom Doxygen configuration](./usage/index.md#custom-doxygen-configuration)**: Specify custom Doxygen configuration for each project.
 
 ## Installation
-With [pip](https://pypi.org/project/mkdoxy/):
+Install the plugin using pip from [PyPI](https://pypi.org/project/mkdoxy/):
+
 ```bash
 pip install mkdoxy
 ```
+Development version with all dependencies:
+```bash
+python -m pip install mkdoxy ".[dev]"
+```
 
-Install from source - development version:
+Install from source:
 ```bash
 pip install git+https://github.com/JakubAndrysek/MkDoxy.git
 ```
 
 ## Quick start
 
 `mkdocs.yml`:
 ```yaml
-site_name: "My documentation"
+site_name: "My MkDoxy documentation"
 
 theme:
   name: material
 
 plugins:
   - search
   - mkdoxy:
@@ -79,14 +89,17 @@
           src-dirs: path/to/src/project1 # path to source code (support multiple paths separated by space) => INPUT
           full-doc: True # if you want to generate full documentation
           doxy-cfg: # standard doxygen configuration (key: value)
             FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out
             RECURSIVE: True # recursive search in source directories
 ```
 
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
 ## Do You Enjoy MkDoxy or Does It Save You Time?
 Then definitely consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
```

#### html2text {}

```diff
@@ -1,21 +1,25 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.2 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.3 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
-email@kubaandrysek.cz License: MIT Keywords: mkdoxy,python,open-
+email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
+JakubAndrysek/MkDoxy Project-URL: Documentation, https://
+mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
+MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
+Keywords: mkdoxy,python,open-
 source,documentation,mkdocs,doxygen,multilanguage,code-
 snippets,code,snippets,documentation-generator Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/)** plugin for **
-[MkDocs](https://www.mkdocs.org/)** generates API documentation based on **
-[Doxygen](https://www.doxygen.nl)** comments and **[code snippets](/intro)** in
-your markdown files.
+Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # MkDoxy **[MkDoxy](https://mkdoxy.kubaandrysek.cz/
+)** plugin for **[MkDocs](https://www.mkdocs.org/)** generates API
+documentation based on **[Doxygen](https://www.doxygen.nl)** comments and **
+[code snippets](/intro)** in your markdown files.
                  [https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FJakubAndrysek%2FMkDoxy&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
 [https://img.shields.io/github/license/JakubAndrysek/MkDoxy?style=flat-square]
    [https://img.shields.io/github/v/release/JakubAndrysek/MkDoxy?style=flat-
  square] [https://img.shields.io/github/stars/JakubAndrysek/MkDoxy?style=flat-
  square] [https://img.shields.io/github/forks/JakubAndrysek/MkDoxy?style=flat-
 square] [https://img.shields.io/github/issues/JakubAndrysek/MkDoxy?style=flat-
@@ -36,23 +40,27 @@
 index.md#multiple-projects)**: Support for multiple projects in one
 documentation (e.g. C++ and Python). - **[Multiple source directories](./usage/
 index.md#multiple-source-directories)**: Configure multiple source directories
 in one project. - **[Custom Jinja templates](./usage/index.md#custom-jinja-
 templates)**: Define custom Jinja templates for rendering Doxygen
 documentation. - **[Custom Doxygen configuration](./usage/index.md#custom-
 doxygen-configuration)**: Specify custom Doxygen configuration for each
-project. ## Installation With [pip](https://pypi.org/project/mkdoxy/): ```bash
-pip install mkdoxy ``` Install from source - development version: ```bash pip
-install git+https://github.com/JakubAndrysek/MkDoxy.git ``` ## Quick start
-`mkdocs.yml`: ```yaml site_name: "My documentation" theme: name: material
-plugins: - search - mkdoxy: projects: myProjectCpp: # name of project must be
-alphanumeric + numbers (without spaces) src-dirs: path/to/src/project1 # path
-to source code (support multiple paths separated by space) => INPUT full-doc:
-True # if you want to generate full documentation doxy-cfg: # standard doxygen
-configuration (key: value) FILE_PATTERNS: "*.cpp *.h*" # specify file patterns
-to filter out RECURSIVE: True # recursive search in source directories ``` ##
-Do You Enjoy MkDoxy or Does It Save You Time? Then definitely consider: -
-supporting me on GitHub Sponsors: [![](https://img.shields.io/static/
+project. ## Installation Install the plugin using pip from [PyPI](https://
+pypi.org/project/mkdoxy/): ```bash pip install mkdoxy ``` Development version
+with all dependencies: ```bash python -m pip install mkdoxy ".[dev]" ```
+Install from source: ```bash pip install git+https://github.com/JakubAndrysek/
+MkDoxy.git ``` ## Quick start `mkdocs.yml`: ```yaml site_name: "My MkDoxy
+documentation" theme: name: material plugins: - search - mkdoxy: projects:
+myProjectCpp: # name of project must be alphanumeric + numbers (without spaces)
+src-dirs: path/to/src/project1 # path to source code (support multiple paths
+separated by space) => INPUT full-doc: True # if you want to generate full
+documentation doxy-cfg: # standard doxygen configuration (key: value)
+FILE_PATTERNS: "*.cpp *.h*" # specify file patterns to filter out RECURSIVE:
+True # recursive search in source directories ``` ## Contributing Pull requests
+are welcome. For major changes, please open an issue first to discuss what you
+would like to change. ## Do You Enjoy MkDoxy or Does It Save You Time? Then
+definitely consider: - supporting me on GitHub Sponsors: [![](https://
+img.shields.io/static/
 v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
 github.com/sponsors/jakubandrysek) ## License This project is licensed under
 the terms of the [MIT license](https://github.com/JakubAndrysek/MkDoxy/blob/
 main/LICENSE)
```

### Comparing `mkdoxy-1.1.2/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.3/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.2/setup.py` & `mkdoxy-1.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,25 +7,43 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.1.2',
+    version='1.1.3',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
     license='MIT',
     python_requires='>=3.9',
-    install_requires=requirements(),
+
+    project_urls={
+        'Source': 'https://github.com/JakubAndrysek/MkDoxy',
+        'Documentation': 'https://mkdoxy.kubaandrysek.cz/',
+        'Tracker': 'https://github.com/JakubAndrysek/MkDoxy/issues',
+        'Funding': 'https://github.com/sponsors/jakubandrysek',
+    },
+
+    install_requires=['mkdocs'],
+    extras_require={
+        "dev": [
+            "mkdocs-material==9.1.18",
+            "Jinja2~=3.1.2",
+            "ruamel.yaml~=0.17.32",
+            "mkdocs-open-in-new-tab~=1.0.2",
+            "pathlib~=1.0.1",
+            "path~=16.7.1",
+            ],
+    },
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
```

