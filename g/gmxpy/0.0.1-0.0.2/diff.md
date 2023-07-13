# Comparing `tmp/gmxpy-0.0.1.tar.gz` & `tmp/gmxpy-0.0.2.tar.gz`

## Comparing `gmxpy-0.0.1.tar` & `gmxpy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gmxpy-0.0.1/gmxpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/gmxpy/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/gmxpy/editconf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/gmxpy/grompp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/gmxpy/solvate/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.1/tests/test_gmxpy.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 gmxpy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gmxpy-0.0.1/LICENSE
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 gmxpy-0.0.1/README.md
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 gmxpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 gmxpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/analysis/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/analysis/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/editconf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/grompp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/grompp/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/solvate/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/utils/__init__,py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 gmxpy-0.0.2/gmxpy/utils/functional.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gmxpy-0.0.2/tests/test_gmxpy.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 gmxpy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gmxpy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 gmxpy-0.0.2/README.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 gmxpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 gmxpy-0.0.2/PKG-INFO
```

### Comparing `gmxpy-0.0.1/.gitignore` & `gmxpy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.1/LICENSE` & `gmxpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmxpy-0.0.1/pyproject.toml` & `gmxpy-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -61,29 +61,32 @@
 000003c0: 2050 7974 686f 6e20 3a3a 2033 2e39 222c   Python :: 3.9",
 000003d0: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
 000003e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000003f0: 7974 686f 6e20 3a3a 2033 2e31 3022 2c0d  ython :: 3.10",.
 00000400: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
 00000410: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 00000420: 7468 6f6e 203a 3a20 332e 3131 222c 0d0a  thon :: 3.11",..
-00000430: 5d0d 0a0d 0a64 796e 616d 6963 203d 205b  ]....dynamic = [
-00000440: 2276 6572 7369 6f6e 225d 0d0a 0d0a 5b70  "version"]....[p
-00000450: 726f 6a65 6374 2e75 726c 735d 0d0a 486f  roject.urls]..Ho
-00000460: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
-00000470: 2f2f 6769 7468 7562 2e63 6f6d 2f47 6f6f  //github.com/Goo
-00000480: 7361 6e67 2d59 752f 676d 7870 7922 0d0a  sang-Yu/gmxpy"..
-00000490: 5265 706f 7369 746f 7279 203d 2022 6874  Repository = "ht
-000004a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004b0: 2f47 6f6f 7361 6e67 2d59 752f 676d 7870  /Goosang-Yu/gmxp
-000004c0: 7922 0d0a 0d0a 5b74 6f6f 6c2e 6861 7463  y"....[tool.hatc
-000004d0: 682e 7665 7273 696f 6e5d 0d0a 7061 7468  h.version]..path
-000004e0: 203d 2022 676d 7870 792f 5f5f 696e 6974   = "gmxpy/__init
-000004f0: 5f5f 2e70 7922 0d0a 0d0a 5b74 6f6f 6c2e  __.py"....[tool.
-00000500: 6861 7463 682e 6275 696c 642e 7461 7267  hatch.build.targ
-00000510: 6574 732e 7364 6973 745d 0d0a 6578 636c  ets.sdist]..excl
-00000520: 7564 6520 3d20 5b0d 0a20 2022 2f2e 6769  ude = [..  "/.gi
-00000530: 7468 7562 222c 0d0a 2020 222f 646f 6373  thub",..  "/docs
-00000540: 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e68  ",..]....[tool.h
-00000550: 6174 6368 2e62 7569 6c64 2e74 6172 6765  atch.build.targe
-00000560: 7473 2e77 6865 656c 5d0d 0a70 6163 6b61  ts.wheel]..packa
-00000570: 6765 7320 3d20 5b22 676d 7870 7922 5d0d  ges = ["gmxpy"].
-00000580: 0a                                       .
+00000430: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
+00000440: 3d20 5b0d 0a20 2020 2022 6d61 7470 6c6f  = [..    "matplo
+00000450: 746c 6962 222c 0d0a 2020 2020 2270 616e  tlib",..    "pan
+00000460: 6461 7322 2c0d 0a20 2020 200d 0a20 2020  das",..    ..   
+00000470: 205d 0d0a 6479 6e61 6d69 6320 3d20 5b22   ]..dynamic = ["
+00000480: 7665 7273 696f 6e22 5d0d 0a0d 0a5b 7072  version"]....[pr
+00000490: 6f6a 6563 742e 7572 6c73 5d0d 0a48 6f6d  oject.urls]..Hom
+000004a0: 6570 6167 6520 3d20 2268 7474 7073 3a2f  epage = "https:/
+000004b0: 2f67 6974 6875 622e 636f 6d2f 476f 6f73  /github.com/Goos
+000004c0: 616e 672d 5975 2f67 6d78 7079 220d 0a52  ang-Yu/gmxpy"..R
+000004d0: 6570 6f73 6974 6f72 7920 3d20 2268 7474  epository = "htt
+000004e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004f0: 476f 6f73 616e 672d 5975 2f67 6d78 7079  Goosang-Yu/gmxpy
+00000500: 220d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  "....[tool.hatch
+00000510: 2e76 6572 7369 6f6e 5d0d 0a70 6174 6820  .version]..path 
+00000520: 3d20 2267 6d78 7079 2f5f 5f69 6e69 745f  = "gmxpy/__init_
+00000530: 5f2e 7079 220d 0a0d 0a5b 746f 6f6c 2e68  _.py"....[tool.h
+00000540: 6174 6368 2e62 7569 6c64 2e74 6172 6765  atch.build.targe
+00000550: 7473 2e73 6469 7374 5d0d 0a65 7863 6c75  ts.sdist]..exclu
+00000560: 6465 203d 205b 0d0a 2020 222f 2e67 6974  de = [..  "/.git
+00000570: 6875 6222 2c0d 0a20 2022 2f64 6f63 7322  hub",..  "/docs"
+00000580: 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 6861  ,..]....[tool.ha
+00000590: 7463 682e 6275 696c 642e 7461 7267 6574  tch.build.target
+000005a0: 732e 7768 6565 6c5d 0d0a 7061 636b 6167  s.wheel]..packag
+000005b0: 6573 203d 205b 2267 6d78 7079 225d 0d0a  es = ["gmxpy"]..
```

