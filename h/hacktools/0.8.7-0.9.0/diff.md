# Comparing `tmp/hacktools-0.8.7.tar.gz` & `tmp/hacktools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hacktools-0.8.7.tar", last modified: Mon Apr 20 18:39:04 2020, max compression
+gzip compressed data, was "dist\hacktools-0.9.0.tar", last modified: Thu Apr 23 14:21:03 2020, max compression
```

## Comparing `hacktools-0.8.7.tar` & `hacktools-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-04-20 18:39:04.165597 hacktools-0.8.7/
--rw-rw-rw-   0        0        0      555 2020-04-20 18:39:04.165597 hacktools-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0       75 2020-04-16 05:58:25.000000 hacktools-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2020-04-20 18:39:04.159599 hacktools-0.8.7/hacktools/
--rw-rw-rw-   0        0        0        0 2019-09-05 21:28:33.000000 hacktools-0.8.7/hacktools/__init__.py
--rw-rw-rw-   0        0        0     4802 2020-04-10 07:42:23.000000 hacktools-0.8.7/hacktools/arch.py
--rw-rw-rw-   0        0        0    16650 2020-04-20 10:21:34.000000 hacktools-0.8.7/hacktools/common.py
--rw-rw-rw-   0        0        0    13289 2020-04-20 06:49:13.000000 hacktools-0.8.7/hacktools/compression.py
--rw-rw-rw-   0        0        0     8555 2020-04-20 11:07:04.000000 hacktools-0.8.7/hacktools/nds.py
--rw-rw-rw-   0        0        0    57006 2020-04-20 18:33:24.000000 hacktools-0.8.7/hacktools/nitro.py
--rw-rw-rw-   0        0        0    16620 2020-04-11 07:06:51.000000 hacktools-0.8.7/hacktools/psp.py
--rw-rw-rw-   0        0        0     6915 2020-04-20 08:31:03.000000 hacktools-0.8.7/hacktools/wii.py
-drwxrwxrwx   0        0        0        0 2020-04-20 18:39:04.164598 hacktools-0.8.7/hacktools.egg-info/
--rw-rw-rw-   0        0        0      555 2020-04-20 18:39:03.000000 hacktools-0.8.7/hacktools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2020-04-20 18:39:04.000000 hacktools-0.8.7/hacktools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-04-20 18:39:03.000000 hacktools-0.8.7/hacktools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2020-04-20 18:39:04.000000 hacktools-0.8.7/hacktools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2020-04-20 18:39:04.000000 hacktools-0.8.7/hacktools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-04-20 18:39:04.165597 hacktools-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      814 2020-04-20 18:38:27.000000 hacktools-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2020-04-23 14:21:03.827847 hacktools-0.9.0/
+-rw-rw-rw-   0        0        0      555 2020-04-23 14:21:03.827847 hacktools-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2020-04-16 05:58:25.000000 hacktools-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2020-04-23 14:21:03.821846 hacktools-0.9.0/hacktools/
+-rw-rw-rw-   0        0        0        0 2019-09-05 21:28:33.000000 hacktools-0.9.0/hacktools/__init__.py
+-rw-rw-rw-   0        0        0     4802 2020-04-10 07:42:23.000000 hacktools-0.9.0/hacktools/arch.py
+-rw-rw-rw-   0        0        0    16674 2020-04-23 08:50:39.000000 hacktools-0.9.0/hacktools/common.py
+-rw-rw-rw-   0        0        0    13289 2020-04-20 06:49:13.000000 hacktools-0.9.0/hacktools/compression.py
+-rw-rw-rw-   0        0        0     8555 2020-04-20 11:07:04.000000 hacktools-0.9.0/hacktools/nds.py
+-rw-rw-rw-   0        0        0    59445 2020-04-23 11:28:02.000000 hacktools-0.9.0/hacktools/nitro.py
+-rw-rw-rw-   0        0        0    16620 2020-04-11 07:06:51.000000 hacktools-0.9.0/hacktools/psp.py
+-rw-rw-rw-   0        0        0     6915 2020-04-20 08:31:03.000000 hacktools-0.9.0/hacktools/wii.py
+drwxrwxrwx   0        0        0        0 2020-04-23 14:21:03.826846 hacktools-0.9.0/hacktools.egg-info/
+-rw-rw-rw-   0        0        0      555 2020-04-23 14:21:03.000000 hacktools-0.9.0/hacktools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2020-04-23 14:21:03.000000 hacktools-0.9.0/hacktools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-04-23 14:21:03.000000 hacktools-0.9.0/hacktools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2020-04-23 14:21:03.000000 hacktools-0.9.0/hacktools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2020-04-23 14:21:03.000000 hacktools-0.9.0/hacktools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-04-23 14:21:03.827847 hacktools-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2020-04-23 08:32:49.000000 hacktools-0.9.0/setup.py
```

### Comparing `hacktools-0.8.7/PKG-INFO` & `hacktools-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hacktools
-Version: 0.8.7
+Version: 0.9.0
 Summary: A set of utilities and tools for rom hacking and translations.
 Home-page: https://github.com/Illidanz/hacktools
 Author: Illidan
 License: UNKNOWN
 Description: # hacktools
         A set of utilities and tools for rom hacking and translations.
```

### Comparing `hacktools-0.8.7/hacktools/arch.py` & `hacktools-0.9.0/hacktools/arch.py`

 * *Files identical despite different names*

### Comparing `hacktools-0.8.7/hacktools/common.py` & `hacktools-0.9.0/hacktools/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     if text.count(sectionsep) > 0:
         lines = text.split(sectionsep)
         for i in range(len(lines)):
             lines[i] = wordwrap(lines[i], glyphs, width, codefunc, default, linebreak, sectionsep)
         return sectionsep.join(lines)
     text = text.replace(linebreak, "\n")
     pattern = re.compile(r"(\s+)")
-    lookup = dict((c, glyphs[c][2] if c in glyphs else default) for c in set(text))
+    lookup = dict((c, glyphs[c].length if c in glyphs else default) for c in set(text))
     for line in text.splitlines():
         tokens = pattern.split(line)
         tokens.append("")
         widths = []
         for token in tokens:
             tokenwidth = 0
             i = 0
@@ -342,15 +342,15 @@
     sjis = 0
     while True:
         b1 = f.readByte()
         if b1 == 0x0A:
             ret += "|"
         elif b1 == 0x00:
             break
-        elif b1 >= 28 and b1 <= 126 and sjis > 0:
+        elif b1 >= 28 and b1 <= 126 and (len(ret) > 0 or b1 == 0x25):
             ret += chr(b1)
         else:
             b2 = f.readByte()
             if checkShiftJIS(b1, b2):
                 f.seek(-2, 1)
                 try:
                     ret += f.read(2).decode(encoding).replace("〜", "～")
```

### Comparing `hacktools-0.8.7/hacktools/compression.py` & `hacktools-0.9.0/hacktools/compression.py`

 * *Files identical despite different names*

### Comparing `hacktools-0.8.7/hacktools/nds.py` & `hacktools-0.9.0/hacktools/nds.py`

 * *Files identical despite different names*

### Comparing `hacktools-0.8.7/hacktools/nitro.py` & `hacktools-0.9.0/hacktools/nitro.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,78 +119,174 @@
             else:
                 common.copyFile(infolder + cellfile, outfolder + cellfile)
             writeNCER(outfolder + file, outfolder + cellfile, image, cell, workfolder + pngfile, palettes, width, height)
     common.logMessage("Done!")
 
 
 # Font
-def getFontGlyphs(file):
+class FontNFTR:
+    height = 0
+    width = 0
+    plgcoffset = 0
+    hdwcoffset = 0
+    pamcoffset = 0
+    plgcsize = 0
+    glyphwidth = 0
+    glyphheight = 0
+    glyphbytes = 0
+    pixelbits = 0
+    tilenum = 0
+    firstcode = 0
+    lastcode = 0
+    plgc = []
+    colors = []
+    hdwc = []
+    pamc = []
     glyphs = {}
+
+
+class FontHDWC:
+    start = 0
+    width = 0
+    length = 0
+
+
+class FontPAMC:
+    firstchar = 0
+    lastchar = 0
+    type = 0
+    nextoffset = 0
+
+
+class FontGlyph:
+    start = 0
+    width = 0
+    length = 0
+    char = ""
+    code = 0
+    index = 0
+
+    def __init__(self, hdwc, char, code, index):
+        self.start = hdwc.start
+        self.width = hdwc.width
+        self.length = hdwc.length
+        self.char = char
+        self.code = code
+        self.index = index
+
+
+def readNFTR(file):
+    nftr = FontNFTR()
     with common.Stream(file, "rb") as f:
         # Header
         f.seek(25)
-        fontheight = f.readByte()
+        nftr.height = f.readByte()
         f.seek(3, 1)
-        fontwidth = f.readByte()
+        nftr.width = f.readByte()
         f.seek(2, 1)
-        plgcoffset = f.readUInt()
-        hdwcoffset = f.readUInt()
-        pamcoffset = f.readUInt()
-        common.logDebug("fontwidth:", fontwidth, "fontheight:", fontheight, "plgcoffset:", plgcoffset, "hdwcoffset:", hdwcoffset, "pamcoffset:", pamcoffset)
+        nftr.plgcoffset = f.readUInt()
+        nftr.hdwcoffset = f.readUInt()
+        nftr.pamcoffset = f.readUInt()
         # PLGC
-        f.seek(plgcoffset - 4)
-        plgcsize = f.readUInt()
+        f.seek(nftr.plgcoffset - 4)
+        nftr.plgcsize = f.readUInt()
+        nftr.glyphwidth = f.readByte()
+        nftr.glyphheight = f.readByte()
+        nftr.glyphbytes = f.readUShort()
         f.seek(2, 1)
-        tilelength = f.readUShort()
-        tilenum = (plgcsize - 0x10) // tilelength
-        common.logDebug("plgcsize:", plgcsize, "tilelength:", tilelength, "tilenum:", tilenum)
+        nftr.pixelbits = f.readUShort()
+        nftr.tilenum = (nftr.plgcsize - 0x10) // nftr.glyphbytes
+        common.logDebug(vars(nftr))
+        # Generate colors
+        nftr.colors = []
+        numcolors = pow(2, nftr.pixelbits)
+        for i in range(numcolors):
+            nftr.colors.append((0, 0, 0, int(255 * i / (numcolors - 1))))
+        # Read the glyphs graphics
+        nftr.plgc = []
+        data = f.readByte()
+        for i in range(nftr.tilenum):
+            glyph = Image.new("RGBA", (nftr.glyphwidth, nftr.glyphheight), nftr.colors[0])
+            pixels = glyph.load()
+            x = 0
+            y = 0
+            byteindex = 0
+            bitmask = 0x80
+            while byteindex < nftr.glyphbytes and y < nftr.glyphheight:
+                intensitymask = pow(2, nftr.pixelbits - 1)
+                intensity = 0
+                while intensitymask > 0:
+                    if data & bitmask > 0:
+                        intensity += intensitymask
+                    bitmask >>= 1
+                    if bitmask == 0:
+                        bitmask = 0x80
+                        byteindex += 1
+                        data = f.readByte()
+                    intensitymask >>= 1
+                if intensity > 0:
+                    pixels[x, y] = nftr.colors[intensity]
+                x += 1
+                if x >= nftr.glyphwidth:
+                    x = 0
+                    y += 1
+            while byteindex < nftr.glyphbytes:
+                data = f.readByte()
+                byteindex += 1
+            nftr.plgc.append(glyph)
         # HDWC
-        f.seek(hdwcoffset)
-        firstcode = f.readUShort()
-        lastcode = f.readUShort()
+        f.seek(nftr.hdwcoffset)
+        nftr.firstcode = f.readUShort()
+        nftr.lastcode = f.readUShort()
         f.seek(4, 1)
-        common.logDebug("firstcode:", firstcode, "lastcode:", lastcode)
-        hdwc = []
-        for i in range(tilenum):
-            hdwcstart = f.readSByte()
-            hdwcwidth = f.readByte()
-            hdwclength = f.readByte()
-            hdwc.append((hdwcstart, hdwcwidth, hdwclength))
+        nftr.hdwc = []
+        for i in range(nftr.tilenum):
+            hdwc = FontHDWC()
+            hdwc.start = f.readSByte()
+            hdwc.width = f.readByte()
+            hdwc.length = f.readByte()
+            common.logDebug(" ", vars(hdwc))
+            nftr.hdwc.append(hdwc)
         # PAMC
-        nextoffset = pamcoffset
+        nftr.pamc = []
+        nftr.glyphs = {}
+        nextoffset = nftr.pamcoffset
         while nextoffset != 0x00:
             f.seek(nextoffset)
-            firstchar = f.readUShort()
-            lastchar = f.readUShort()
-            sectiontype = f.readUInt()
-            nextoffset = f.readUInt()
-            common.logDebug("firstchar:", common.toHex(firstchar), "lastchar:", common.toHex(lastchar), "sectiontype:", sectiontype, "nextoffset:", nextoffset)
-            if sectiontype == 0:
+            pamc = FontPAMC()
+            pamc.firstchar = f.readUShort()
+            pamc.lastchar = f.readUShort()
+            pamc.type = f.readUInt()
+            nextoffset = pamc.nextoffset = f.readUInt()
+            common.logDebug(" ", vars(pamc))
+            if pamc.type == 0:
                 firstcode = f.readUShort()
-                for i in range(lastchar - firstchar + 1):
-                    c = common.codeToChar(firstchar + i)
-                    glyphs[c] = hdwc[firstcode + i] + (firstchar + i,)
-            elif sectiontype == 1:
-                for i in range(lastchar - firstchar + 1):
+                for i in range(pamc.lastchar - pamc.firstchar + 1):
+                    c = common.codeToChar(pamc.firstchar + i)
+                    nftr.glyphs[c] = FontGlyph(nftr.hdwc[firstcode + i], c, pamc.firstchar + i, firstcode + i)
+            elif pamc.type == 1:
+                for i in range(pamc.lastchar - pamc.firstchar + 1):
                     charcode = f.readUShort()
-                    if charcode == 0xFFFF or charcode >= len(hdwc):
+                    if charcode == 0xFFFF or charcode >= len(nftr.hdwc):
                         continue
-                    c = common.codeToChar(firstchar + i)
-                    glyphs[c] = hdwc[charcode] + (firstchar + i,)
+                    c = common.codeToChar(pamc.firstchar + i)
+                    nftr.glyphs[c] = FontGlyph(nftr.hdwc[charcode], c, pamc.firstchar + i, charcode)
             else:
-                common.logError("Unknown section type", sectiontype)
-    return glyphs
+                common.logError("Unknown section type", pamc.type)
+    return nftr
 
 
 def extractFontData(fontfiles, out):
+    if isinstance(fontfiles, str):
+        fontfiles = [fontfiles]
     with common.Stream(out, "wb") as f:
         for fontfile in fontfiles:
-            glyphs = getFontGlyphs(fontfile)
+            nftr = readNFTR(fontfile)
             for i in range(0x20, 0x7e):
-                f.writeByte(glyphs[chr(i)][2])
+                f.writeByte(nftr.glyphs[chr(i)][2])
 
 
 # Graphics
 class NCGR:
     width = 0
     height = 0
     bpp = 4
```

### Comparing `hacktools-0.8.7/hacktools/psp.py` & `hacktools-0.9.0/hacktools/psp.py`

 * *Files identical despite different names*

### Comparing `hacktools-0.8.7/hacktools/wii.py` & `hacktools-0.9.0/hacktools/wii.py`

 * *Files identical despite different names*

### Comparing `hacktools-0.8.7/hacktools.egg-info/PKG-INFO` & `hacktools-0.9.0/hacktools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hacktools
-Version: 0.8.7
+Version: 0.9.0
 Summary: A set of utilities and tools for rom hacking and translations.
 Home-page: https://github.com/Illidanz/hacktools
 Author: Illidan
 License: UNKNOWN
 Description: # hacktools
         A set of utilities and tools for rom hacking and translations.
```

### Comparing `hacktools-0.8.7/setup.py` & `hacktools-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hacktools",
-    version="0.8.7",
+    version="0.9.0",
     author="Illidan",
     description="A set of utilities and tools for rom hacking and translations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Illidanz/hacktools",
     packages=["hacktools"],
     classifiers=[
```

