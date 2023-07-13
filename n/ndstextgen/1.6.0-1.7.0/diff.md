# Comparing `tmp/ndstextgen-1.6.0.tar.gz` & `tmp/ndstextgen-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndstextgen-1.6.0.tar", last modified: Wed Mar  8 15:03:14 2023, max compression
+gzip compressed data, was "ndstextgen-1.7.0.tar", last modified: Thu Jul 13 10:57:52 2023, max compression
```

## Comparing `ndstextgen-1.6.0.tar` & `ndstextgen-1.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:03:14.008315 ndstextgen-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-08 15:03:14.008315 ndstextgen-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:03:14.008315 ndstextgen-1.6.0/ndstextgen/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/ndstextgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/ndstextgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/ndstextgen/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:03:14.008315 ndstextgen-1.6.0/ndstextgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-08 15:03:13.000000 ndstextgen-1.6.0/ndstextgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-08 15:03:14.000000 ndstextgen-1.6.0/ndstextgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 15:03:13.000000 ndstextgen-1.6.0/ndstextgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-08 15:03:13.000000 ndstextgen-1.6.0/ndstextgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-08 15:03:13.000000 ndstextgen-1.6.0/ndstextgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-08 15:03:13.000000 ndstextgen-1.6.0/ndstextgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 15:03:14.008315 ndstextgen-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-08 15:03:03.000000 ndstextgen-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/ndstextgen/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/ndstextgen/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/ndstextgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 10:57:52.000000 ndstextgen-1.7.0/ndstextgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:57:52.342171 ndstextgen-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 10:57:42.000000 ndstextgen-1.7.0/setup.py
```

### Comparing `ndstextgen-1.6.0/LICENSE` & `ndstextgen-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ndstextgen-1.6.0/PKG-INFO` & `ndstextgen-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndstextgen
-Version: 1.6.0
+Version: 1.7.0
 Summary: Command line tool to render text from NDS .NFTR fonts.
 Home-page: https://github.com/Illidanz/ndstextgen
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,12 +32,13 @@
 `--color <text>`: Color to apply to the font. Default: black  
 `--bg <text>`: Background color. Default: transparent  
 `--width <int>`: Set width for the generated image. Default: 256  
 `--height <int>`: Set height for the generated image. Default: 256  
 `--center`: Center each line.  
 `--wwrap`: Automatic wordwrap.  
 `--no-crop`: Don't crop the image before saving it.  
+`--encoding <str>`: Encoding the font uses. See [Python documentation](https://docs.python.org/3/library/codecs.html#standard-encodings).  
 ## Script usage
 ```python
 import ndstextgen
 image = ndstextgen.gen("font.NFTR", "Print multiline\nred text.", color="red")
 ```
```

### Comparing `ndstextgen-1.6.0/README.md` & `ndstextgen-1.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 `--color <text>`: Color to apply to the font. Default: black  
 `--bg <text>`: Background color. Default: transparent  
 `--width <int>`: Set width for the generated image. Default: 256  
 `--height <int>`: Set height for the generated image. Default: 256  
 `--center`: Center each line.  
 `--wwrap`: Automatic wordwrap.  
 `--no-crop`: Don't crop the image before saving it.  
+`--encoding <str>`: Encoding the font uses. See [Python documentation](https://docs.python.org/3/library/codecs.html#standard-encodings).  
 ## Script usage
 ```python
 import ndstextgen
 image = ndstextgen.gen("font.NFTR", "Print multiline\nred text.", color="red")
 ```
```

### Comparing `ndstextgen-1.6.0/ndstextgen/__init__.py` & `ndstextgen-1.7.0/ndstextgen/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-def gen(font, text, out="text.png", vert=2, fw=0, spacing=0, color="black", bg="transparent", width=256, height=256, center=False, wwrap=False, no_crop=False):
+def gen(font, text, out="text.png", vert=2, fw=0, spacing=0, color="black", bg="transparent", width=256, height=256, center=False, wwrap=False, no_crop=False, encoding="shift_jis"):
     from . import cli
-    args = [font, text, "--out", out, "--vert", vert, "--fw", fw, "--spacing", spacing, "--color", color, "--bg", bg, "--width", width, "--height", height]
+    args = [font, text, "--out", out, "--vert", vert, "--fw", fw, "--spacing", spacing, "--color", color, "--bg", bg, "--width", width, "--height", height, "--encoding", encoding]
     if center:
         args.append("--center")
     if wwrap:
         args.append("--wwrap")
     if no_crop:
         args.append("--no-crop")
     return cli.gen(args, standalone_mode=False)
```

### Comparing `ndstextgen-1.6.0/ndstextgen/cli.py` & `ndstextgen-1.7.0/ndstextgen/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from PIL import Image
 from hacktools import common, nitro
 
 
 @common.cli.command(context_settings=dict(show_default=True))
 @click.argument("font")
 @click.argument("text")
-@click.option("--out",     default="text.png",    help="Output file, set empty to just return the image.")
-@click.option("--vert",    default=2,             help="Vertical spacing between lines.")
-@click.option("--fw",      default=0,             help="Use a fixed width instead of the VWF values in the font.")
-@click.option("--spacing", default=0,             help="Additional horizontal spacing between characters.")
-@click.option("--color",   default="black",       help="Color to apply to the font.")
-@click.option("--bg",      default="transparent", help="Background color.")
-@click.option("--width",   default=256,           help="Set width for the generated image.")
-@click.option("--height",  default=256,           help="Set height for the generated image.")
-@click.option("--center",  is_flag=True,          help="Center each line.")
-@click.option("--wwrap",   is_flag=True,          help="Automatic wordwrap.")
-@click.option("--no-crop", is_flag=True,          help="Don't crop the image before saving it.")
-def gen(font, text, out, vert, fw, spacing, color, bg, width, height, center, wwrap, no_crop):
+@click.option("--out",      default="text.png",    help="Output file, set empty to just return the image.")
+@click.option("--vert",     default=2,             help="Vertical spacing between lines.")
+@click.option("--fw",       default=0,             help="Use a fixed width instead of the VWF values in the font.")
+@click.option("--spacing",  default=0,             help="Additional horizontal spacing between characters.")
+@click.option("--color",    default="black",       help="Color to apply to the font.")
+@click.option("--bg",       default="transparent", help="Background color.")
+@click.option("--width",    default=256,           help="Set width for the generated image.")
+@click.option("--height",   default=256,           help="Set height for the generated image.")
+@click.option("--center",   is_flag=True,          help="Center each line.")
+@click.option("--wwrap",    is_flag=True,          help="Automatic wordwrap.")
+@click.option("--no-crop",  is_flag=True,          help="Don't crop the image before saving it.")
+@click.option("--encoding", default="shift_jis",   help="Encoding the font uses.")
+def gen(font, text, out, vert, fw, spacing, color, bg, width, height, center, wwrap, no_crop, encoding):
     """FONT is the font file, .NFTR extension can be omitted.
 
     TEXT is the text to write. "\\n" can be used for a line break. Can be the name of a UTF-8 file to read the text from."""
     if not os.path.isfile(font):
         if not font.lower().endswith(".nftr"):
             font = font + ".NFTR"
         if not os.path.isfile(font):
@@ -33,15 +34,15 @@
         with codecs.open(text, "r", "utf-8") as f:
             text = f.read().replace("\r\n", "\\n").replace("\n", "\\n")
     text = text.replace("\\n", "\n")
     # Add an additional line break to center the last line
     if not text.endswith("\n"):
         text += "\n"
     # Read the font data
-    nftr = nitro.readNFTR(font, True)
+    nftr = nitro.readNFTR(font, True, encoding)
     if wwrap:
         # Extract the glyphs for wordwrapping
         glyphs = {}
         for char in nftr.glyphs:
             glyph = nftr.glyphs[char]
             glyphs[char] = common.FontGlyph(glyph.start, glyph.width, glyph.length, glyph.char, glyph.code, glyph.index)
             if fw > 0:
@@ -97,9 +98,9 @@
         final.paste(img, (0, 0), img)
     if out != "":
         final.save(out, "PNG")
     return final
 
 
 def main():
-    click.echo("ndstextgen version 1.6.0")
+    click.echo("ndstextgen version 1.7.0")
     gen()
```

### Comparing `ndstextgen-1.6.0/ndstextgen.egg-info/PKG-INFO` & `ndstextgen-1.7.0/ndstextgen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndstextgen
-Version: 1.6.0
+Version: 1.7.0
 Summary: Command line tool to render text from NDS .NFTR fonts.
 Home-page: https://github.com/Illidanz/ndstextgen
 Author: Illidan
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -32,12 +32,13 @@
 `--color <text>`: Color to apply to the font. Default: black  
 `--bg <text>`: Background color. Default: transparent  
 `--width <int>`: Set width for the generated image. Default: 256  
 `--height <int>`: Set height for the generated image. Default: 256  
 `--center`: Center each line.  
 `--wwrap`: Automatic wordwrap.  
 `--no-crop`: Don't crop the image before saving it.  
+`--encoding <str>`: Encoding the font uses. See [Python documentation](https://docs.python.org/3/library/codecs.html#standard-encodings).  
 ## Script usage
 ```python
 import ndstextgen
 image = ndstextgen.gen("font.NFTR", "Print multiline\nred text.", color="red")
 ```
```

### Comparing `ndstextgen-1.6.0/setup.py` & `ndstextgen-1.7.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ndstextgen",
-    version="1.6.0",
+    version="1.7.0",
     author="Illidan",
     description="Command line tool to render text from NDS .NFTR fonts.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Illidanz/ndstextgen",
     packages=["ndstextgen"],
     classifiers=[
@@ -17,11 +17,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["ndstextgen=ndstextgen.cli:main"],
     },
     install_requires=[
-        "hacktools>=0.13"
+        "hacktools>=0.32.7"
     ],
     python_requires=">=3.7",
 )
```

