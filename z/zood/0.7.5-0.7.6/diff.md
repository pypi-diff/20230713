# Comparing `tmp/zood-0.7.5.tar.gz` & `tmp/zood-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.7.5.tar", max compression
+gzip compressed data, was "zood-0.7.6.tar", max compression
```

## Comparing `zood-0.7.5.tar` & `zood-0.7.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      550 2023-05-24 15:15:01.902988 zood-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.5/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.5/zood/__init__.py
--rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.5/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.5/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.5/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.5/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.5/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.5/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.5/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.5/zood/config/img/sun.png
--rw-r--r--   0        0        0    18776 2023-05-24 15:13:42.054920 zood-0.7.5/zood/config/index.css
--rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.5/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.5/zood/config/js/check_box.js
--rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.5/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.5/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.5/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.5/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.5/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.5/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.5/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.5/zood/config/js/search.js
--rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.5/zood/config/template.html
--rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.5/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.5/zood/md_parser.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.5/zood/util.py
--rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.5/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.5/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-06-04 01:33:59.251613 zood-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.6/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.6/zood/__init__.py
+-rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.6/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.6/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.6/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.6/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.6/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.6/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.6/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.6/zood/config/img/sun.png
+-rw-r--r--   0        0        0    18776 2023-05-24 15:13:42.054920 zood-0.7.6/zood/config/index.css
+-rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.6/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.6/zood/config/js/check_box.js
+-rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.6/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.6/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.6/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.6/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.6/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.6/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.6/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.6/zood/config/js/search.js
+-rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.6/zood/config/template.html
+-rw-r--r--   0        0        0     4552 2023-06-04 01:33:22.050257 zood-0.7.6/zood/main.py
+-rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.6/zood/md_parser.py
+-rw-r--r--   0        0        0     4292 2023-06-04 01:12:09.286908 zood-0.7.6/zood/util.py
+-rw-r--r--   0        0        0     8743 2023-06-04 01:05:49.331724 zood-0.7.6/zood/zood.py
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.6/setup.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.6/PKG-INFO
```

### Comparing `zood-0.7.5/pyproject.toml` & `zood-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.7.5"
+version = "0.7.6"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.7.5/zood/config/_config.yml` & `zood-0.7.6/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/img/enter.png` & `zood-0.7.6/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/index.css` & `zood-0.7.6/zood/config/index.css`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/change_mode.js` & `zood-0.7.6/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/check_box.js` & `zood-0.7.6/zood/config/js/check_box.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/copy_code.js` & `zood-0.7.6/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/navigator.js` & `zood-0.7.6/zood/config/js/navigator.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/next_front.js` & `zood-0.7.6/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/picture_preview.js` & `zood-0.7.6/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/prismjs/prism.css` & `zood-0.7.6/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/prismjs/prism.js` & `zood-0.7.6/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/js/search.js` & `zood-0.7.6/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/config/template.html` & `zood-0.7.6/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/main.py` & `zood-0.7.6/zood/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,269 @@
-00000000: 0d0a 696d 706f 7274 2061 7267 7061 7273  ..import argpars
-00000010: 650d 0a69 6d70 6f72 7420 6f73 0d0a 696d  e..import os..im
-00000020: 706f 7274 2073 6875 7469 6c0d 0a0d 0a66  port shutil....f
-00000030: 726f 6d20 2e75 7469 6c20 696d 706f 7274  rom .util import
-00000040: 202a 0d0a 6672 6f6d 202e 6d64 5f70 6172   *..from .md_par
-00000050: 7365 7220 696d 706f 7274 2070 6172 7365  ser import parse
-00000060: 446f 6373 0d0a 6672 6f6d 202e 7a6f 6f64  Docs..from .zood
-00000070: 2069 6d70 6f72 7420 2a0d 0a0d 0a64 6566   import *....def
-00000080: 206d 6169 6e28 293a 0d0a 2020 2020 0d0a   main():..    ..
-00000090: 2020 2020 7061 7273 6572 203d 2061 7267      parser = arg
-000000a0: 7061 7273 652e 4172 6775 6d65 6e74 5061  parse.ArgumentPa
-000000b0: 7273 6572 280d 0a20 2020 2020 2020 2064  rser(..        d
-000000c0: 6573 6372 6970 7469 6f6e 3d27 7a6f 6f64  escription='zood
-000000d0: 3a20 7765 6220 7061 6765 2064 6f63 756d  : web page docum
-000000e0: 656e 7461 7469 6f6e 2026 2063 6f6d 6d65  entation & comme
-000000f0: 6e74 2067 656e 6572 6174 696f 6e20 646f  nt generation do
-00000100: 6375 6d65 6e74 6174 696f 6e27 0d0a 2020  cumentation'..  
-00000110: 2020 290d 0a20 2020 2070 6172 7365 722e    )..    parser.
-00000120: 6164 645f 6172 6775 6d65 6e74 2827 636d  add_argument('cm
-00000130: 6427 2c74 7970 653d 7374 722c 6e61 7267  d',type=str,narg
-00000140: 733d 272a 272c 6865 6c70 3d27 696e 6974  s='*',help='init
-00000150: 6961 6c69 7a65 2064 6f63 7320 7465 6d70  ialize docs temp
-00000160: 6c61 7465 2729 0d0a 2020 2020 7061 7273  late')..    pars
-00000170: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00000180: 272d 6727 2c27 2d2d 6765 6e65 7261 7465  '-g','--generate
-00000190: 272c 6163 7469 6f6e 3d27 7374 6f72 655f  ',action='store_
-000001a0: 7472 7565 272c 6865 6c70 3d27 6765 6e65  true',help='gene
-000001b0: 7261 7465 2068 746d 6c20 646f 6327 290d  rate html doc').
-000001c0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-000001d0: 6172 6775 6d65 6e74 2827 2d73 272c 272d  argument('-s','-
-000001e0: 2d73 6176 6527 2c61 6374 696f 6e3d 2773  -save',action='s
-000001f0: 746f 7265 5f74 7275 6527 2c68 656c 703d  tore_true',help=
-00000200: 2773 6176 6520 5f63 6f6e 6669 672e 796d  'save _config.ym
-00000210: 6c20 616e 6420 7573 6520 696e 2065 7665  l and use in eve
-00000220: 7279 2065 6e76 6972 6f6e 6d65 6e74 2729  ry environment')
-00000230: 0d0a 2020 2020 6172 6773 203d 2070 6172  ..    args = par
-00000240: 7365 722e 7061 7273 655f 6172 6773 2829  ser.parse_args()
-00000250: 0d0a 2020 2020 0d0a 2020 2020 636f 6e66  ..    ..    conf
-00000260: 6967 203d 2067 6574 5a6f 6f64 436f 6e66  ig = getZoodConf
-00000270: 6967 2829 0d0a 2020 2020 6d64 5f64 6972  ig()..    md_dir
-00000280: 5f6e 616d 6520 3d20 636f 6e66 6967 5b27  _name = config['
-00000290: 6d61 726b 646f 776e 5f66 6f6c 6465 7227  markdown_folder'
-000002a0: 5d0d 0a20 2020 200d 0a20 2020 206c 6f63  ]..    ..    loc
-000002b0: 616c 5f63 6f6e 6669 675f 7061 7468 203d  al_config_path =
-000002c0: 206f 732e 7061 7468 2e6a 6f69 6e28 6d64   os.path.join(md
-000002d0: 5f64 6972 5f6e 616d 652c 275f 636f 6e66  _dir_name,'_conf
-000002e0: 6967 2e79 6d6c 2729 0d0a 2020 2020 676c  ig.yml')..    gl
-000002f0: 6f62 616c 5f63 6f6e 6669 675f 7061 7468  obal_config_path
-00000300: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00000310: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00000320: 5f5f 6669 6c65 5f5f 292c 2763 6f6e 6669  __file__),'confi
-00000330: 6727 2c27 5f63 6f6e 6669 672e 796d 6c27  g','_config.yml'
-00000340: 290d 0a20 2020 200d 0a20 2020 2067 6c6f  )..    ..    glo
-00000350: 6261 6c20 7665 7273 696f 6e0d 0a20 2020  bal version..   
-00000360: 200d 0a20 2020 2069 6620 6172 6773 2e67   ..    if args.g
-00000370: 656e 6572 6174 653a 0d0a 2020 2020 2020  enerate:..      
-00000380: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
-00000390: 2e65 7869 7374 7328 6d64 5f64 6972 5f6e  .exists(md_dir_n
-000003a0: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
-000003b0: 2020 2070 7269 6e74 496e 666f 2822 e8af     printInfo("..
-000003c0: b7e5 8588 e4bd bfe7 94a8 207a 6f6f 6420  .......... zood 
-000003d0: 696e 6974 20e5 889d e5a7 8be5 8c96 2229  init .........")
-000003e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000003f0: 7475 726e 0d0a 2020 2020 2020 2020 7061  turn..        pa
-00000400: 7273 6544 6f63 7328 6d64 5f64 6972 5f6e  rseDocs(md_dir_n
-00000410: 616d 6529 0d0a 2020 2020 2020 2020 7265  ame)..        re
-00000420: 7475 726e 0d0a 2020 2020 0d0a 2020 2020  turn..    ..    
-00000430: 6966 2061 7267 732e 7361 7665 3a0d 0a20  if args.save:.. 
-00000440: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00000450: 682e 6578 6973 7473 286c 6f63 616c 5f63  h.exists(local_c
-00000460: 6f6e 6669 675f 7061 7468 293a 0d0a 2020  onfig_path):..  
-00000470: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
-00000480: 2e63 6f70 7928 6c6f 6361 6c5f 636f 6e66  .copy(local_conf
-00000490: 6967 5f70 6174 682c 676c 6f62 616c 5f63  ig_path,global_c
-000004a0: 6f6e 6669 675f 7061 7468 290d 0a20 2020  onfig_path)..   
-000004b0: 2020 2020 2020 2020 2070 7269 6e74 496e           printIn
-000004c0: 666f 2822 e5b7 b2e6 9bb4 e696 b0e5 85a8  fo("............
-000004d0: e5b1 80e9 858d e7bd aee6 9687 e4bb b620  ............... 
-000004e0: 5f63 6f6e 6669 672e 796d 6c22 2c63 6f6c  _config.yml",col
-000004f0: 6f72 3d27 6772 6565 6e27 290d 0a20 2020  or='green')..   
-00000500: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000510: 2020 2020 2020 2020 7072 696e 7428 27e6          print('.
-00000520: 9caa e689 bee5 88b0 272c 6c6f 6361 6c5f  ........',local_
-00000530: 636f 6e66 6967 5f70 6174 6829 0d0a 2020  config_path)..  
-00000540: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000550: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-00000560: 7328 6f73 2e70 6174 682e 6a6f 696e 286d  s(os.path.join(m
-00000570: 645f 6469 725f 6e61 6d65 2c27 7072 6973  d_dir_name,'pris
-00000580: 6d6a 7327 2929 3a0d 0a20 2020 2020 2020  mjs')):..       
-00000590: 2020 2020 2067 6c6f 6261 6c5f 7072 6973       global_pris
-000005a0: 6d5f 6373 735f 7061 7468 203d 206f 732e  m_css_path = os.
-000005b0: 7061 7468 2e6a 6f69 6e28 6f73 2e70 6174  path.join(os.pat
-000005c0: 682e 6469 726e 616d 6528 5f5f 6669 6c65  h.dirname(__file
-000005d0: 5f5f 292c 2763 6f6e 6669 6727 2c27 6a73  __),'config','js
-000005e0: 272c 2770 7269 736d 6a73 272c 2770 7269  ','prismjs','pri
-000005f0: 736d 2e63 7373 2729 0d0a 2020 2020 2020  sm.css')..      
-00000600: 2020 2020 2020 676c 6f62 616c 5f70 7269        global_pri
-00000610: 736d 5f6a 735f 7061 7468 203d 206f 732e  sm_js_path = os.
-00000620: 7061 7468 2e6a 6f69 6e28 6f73 2e70 6174  path.join(os.pat
-00000630: 682e 6469 726e 616d 6528 5f5f 6669 6c65  h.dirname(__file
-00000640: 5f5f 292c 2763 6f6e 6669 6727 2c27 6a73  __),'config','js
-00000650: 272c 2770 7269 736d 6a73 272c 2770 7269  ','prismjs','pri
-00000660: 736d 2e6a 7327 290d 0a20 2020 2020 2020  sm.js')..       
-00000670: 2020 2020 2073 6875 7469 6c2e 636f 7079       shutil.copy
-00000680: 286f 732e 7061 7468 2e6a 6f69 6e28 6d64  (os.path.join(md
-00000690: 5f64 6972 5f6e 616d 652c 2770 7269 736d  _dir_name,'prism
-000006a0: 6a73 272c 2770 7269 736d 2e63 7373 2729  js','prism.css')
-000006b0: 2c67 6c6f 6261 6c5f 7072 6973 6d5f 6373  ,global_prism_cs
-000006c0: 735f 7061 7468 290d 0a20 2020 2020 2020  s_path)..       
-000006d0: 2020 2020 2073 6875 7469 6c2e 636f 7079       shutil.copy
-000006e0: 286f 732e 7061 7468 2e6a 6f69 6e28 6d64  (os.path.join(md
-000006f0: 5f64 6972 5f6e 616d 652c 2770 7269 736d  _dir_name,'prism
-00000700: 6a73 272c 2770 7269 736d 2e6a 7327 292c  js','prism.js'),
-00000710: 676c 6f62 616c 5f70 7269 736d 5f6a 735f  global_prism_js_
-00000720: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-00000730: 2020 2070 7269 6e74 496e 666f 2822 e5b7     printInfo("..
-00000740: b2e6 9bb4 e696 b0e5 85a8 e5b1 80e9 858d  ................
-00000750: e7bd aee6 9687 e4bb b620 7072 6973 6d6a  ......... prismj
-00000760: 7322 290d 0a20 2020 2020 2020 2065 6c73  s")..        els
-00000770: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000780: 7072 696e 7428 27e6 9caa e689 bee5 88b0  print('.........
-00000790: 272c 6f73 2e70 6174 682e 6a6f 696e 286d  ',os.path.join(m
-000007a0: 645f 6469 725f 6e61 6d65 2c27 7072 6973  d_dir_name,'pris
-000007b0: 6d6a 7327 2929 0d0a 0d0a 2020 2020 2020  mjs'))....      
-000007c0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-000007d0: 6966 206c 656e 2861 7267 732e 636d 6429  if len(args.cmd)
-000007e0: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-000007f0: 7072 696e 7428 277a 6f6f 64e4 bdbf e794  print('zood.....
-00000800: a8e6 96b9 e6b3 95e8 a781 2068 7474 7073  .......... https
-00000810: 3a2f 2f6c 757a 6869 7869 6e67 3132 3334  ://luzhixing1234
-00000820: 352e 6769 7468 7562 2e69 6f2f 7a6f 6f64  5.github.io/zood
-00000830: 2f27 290d 0a20 2020 2020 2020 2072 6574  /')..        ret
-00000840: 7572 6e0d 0a20 2020 200d 0a20 2020 2069  urn..    ..    i
-00000850: 6620 6172 6773 2e63 6d64 5b30 5d20 3d3d  f args.cmd[0] ==
-00000860: 2027 696e 6974 273a 0d0a 2020 2020 2020   'init':..      
-00000870: 2020 0d0a 2020 2020 2020 2020 696e 6974    ..        init
-00000880: 5a6f 6f64 286d 645f 6469 725f 6e61 6d65  Zood(md_dir_name
-00000890: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000008a0: 2065 6c69 6620 6172 6773 2e63 6d64 5b30   elif args.cmd[0
-000008b0: 5d20 3d3d 2027 6e65 7727 3a0d 0a20 2020  ] == 'new':..   
-000008c0: 2020 2020 2069 6620 6c65 6e28 6172 6773       if len(args
-000008d0: 2e63 6d64 2920 3d3d 2032 3a0d 0a20 2020  .cmd) == 2:..   
-000008e0: 2020 2020 2020 2020 2064 6972 5f6e 616d           dir_nam
-000008f0: 6520 3d20 272e 270d 0a20 2020 2020 2020  e = '.'..       
-00000900: 2020 2020 2066 696c 655f 6e61 6d65 203d       file_name =
-00000910: 2061 7267 732e 636d 645b 315d 0d0a 2020   args.cmd[1]..  
-00000920: 2020 2020 2020 656c 6966 206c 656e 2861        elif len(a
-00000930: 7267 732e 636d 6429 203d 3d20 333a 0d0a  rgs.cmd) == 3:..
-00000940: 2020 2020 2020 2020 2020 2020 6469 725f              dir_
-00000950: 6e61 6d65 203d 2061 7267 732e 636d 645b  name = args.cmd[
-00000960: 315d 0d0a 2020 2020 2020 2020 2020 2020  1]..            
-00000970: 6669 6c65 5f6e 616d 6520 3d20 6172 6773  file_name = args
-00000980: 2e63 6d64 5b32 5d0d 0a20 2020 2020 2020  .cmd[2]..       
-00000990: 2020 2020 2069 6620 6469 725f 6e61 6d65       if dir_name
-000009a0: 203d 3d20 6d64 5f64 6972 5f6e 616d 653a   == md_dir_name:
-000009b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000009c0: 2020 7072 696e 7449 6e66 6f28 6622 e682    printInfo(f"..
-000009d0: a8e4 b88d e883 bde5 889b e5bb bae4 b880  ................
-000009e0: e4b8 aae5 928c 207b 6d64 5f64 6972 5f6e  ...... {md_dir_n
-000009f0: 616d 657d 20e5 908c e590 8de7 9a84 e5ad  ame} ...........
-00000a00: 90e6 9687 e4bb b6e5 a4b9 2229 0d0a 2020  ..........")..  
-00000a10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000a20: 7475 726e 0d0a 2020 2020 2020 2020 656c  turn..        el
-00000a30: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000a40: 2070 7269 6e74 496e 666f 2866 22e5 889b   printInfo(f"...
-00000a50: e5bb bae6 96b0 e696 87e4 bbb6 e79a 84e5  ................
-00000a60: 91bd e4bb a4e4 b8ba 207a 6f6f 6420 6e65  ........ zood ne
-00000a70: 7720 5be7 9bae e5bd 955d 205b e696 87e4  w [......] [....
-00000a80: bbb6 e590 8d5d 2229 0d0a 2020 2020 2020  .....]")..      
-00000a90: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00000aa0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000ab0: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
-00000ac0: 7869 7374 7328 6d64 5f64 6972 5f6e 616d  xists(md_dir_nam
-00000ad0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00000ae0: 2069 6e69 745a 6f6f 6428 6d64 5f64 6972   initZood(md_dir
-00000af0: 5f6e 616d 6529 0d0a 0d0a 2020 2020 2020  _name)....      
-00000b00: 2020 6372 6561 7465 4e65 7746 696c 6528    createNewFile(
-00000b10: 6d64 5f64 6972 5f6e 616d 652c 6469 725f  md_dir_name,dir_
-00000b20: 6e61 6d65 2c66 696c 655f 6e61 6d65 290d  name,file_name).
-00000b30: 0a20 2020 200d 0a20 2020 2065 6c69 6620  .    ..    elif 
-00000b40: 6172 6773 2e63 6d64 5b30 5d20 3d3d 2027  args.cmd[0] == '
-00000b50: 636c 6561 6e27 3a0d 0a20 2020 2020 2020  clean':..       
-00000b60: 2073 6875 7469 6c2e 726d 7472 6565 2827   shutil.rmtree('
-00000b70: 646f 6373 2729 0d0a 2020 2020 2020 2020  docs')..        
-00000b80: 7072 696e 7449 6e66 6f28 6622 e5b7 b2e5  printInfo(f"....
-00000b90: 88a0 e999 a420 646f 6373 2229 0d0a 2020  ..... docs")..  
-00000ba0: 2020 2020 2020 0d0a 2020 2020 656c 6966        ..    elif
-00000bb0: 2061 7267 732e 636d 645b 305d 203d 3d20   args.cmd[0] == 
-00000bc0: 2763 6f6e 6669 6727 3a0d 0a20 2020 2020  'config':..     
-00000bd0: 2020 2073 6875 7469 6c2e 636f 7079 2867     shutil.copy(g
-00000be0: 6c6f 6261 6c5f 636f 6e66 6967 5f70 6174  lobal_config_pat
-00000bf0: 682c 6c6f 6361 6c5f 636f 6e66 6967 5f70  h,local_config_p
-00000c00: 6174 6829 0d0a 2020 2020 2020 2020 7072  ath)..        pr
-00000c10: 696e 7449 6e66 6f28 6622 e794 9fe6 8890  intInfo(f"......
-00000c20: e985 8de7 bdae e696 87e4 bbb6 207b 6c6f  ............ {lo
-00000c30: 6361 6c5f 636f 6e66 6967 5f70 6174 687d  cal_config_path}
-00000c40: 222c 636f 6c6f 723d 2767 7265 656e 2729  ",color='green')
-00000c50: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-00000c60: 2020 2320 656c 6966 2061 7267 732e 636d    # elif args.cm
-00000c70: 645b 305d 203d 3d20 2775 7064 6174 6527  d[0] == 'update'
-00000c80: 3a0d 0a20 2020 2023 2020 2020 2070 7269  :..    #     pri
-00000c90: 6e74 2866 22e5 bd93 e589 8d7a 6f6f 64e7  nt(f"......zood.
-00000ca0: 8988 e69c ace4 b8ba 207b 7665 7273 696f  ........ {versio
-00000cb0: 6e7d 2c20 e6ad a3e5 9ca8 e69f a5e8 afa2  n}, ............
-00000cc0: e69c 80e6 96b0 7a6f 6f64 e789 88e6 9cac  ......zood......
-00000cd0: 2e2e 2e22 290d 0a20 2020 2023 2020 2020  ...")..    #    
-00000ce0: 206c 6174 6573 745f 7a6f 6f64 5f76 6572   latest_zood_ver
-00000cf0: 7369 6f6e 203d 2076 6572 7369 6f6e 7328  sion = versions(
-00000d00: 277a 6f6f 6427 295b 305d 0d0a 2020 2020  'zood')[0]..    
-00000d10: 2320 2020 2020 7072 696e 7428 6627 e69c  #     print(f'..
-00000d20: 80e6 96b0 7a6f 6f64 e789 88e6 9cac e4b8  ....zood........
-00000d30: ba27 2c20 6c61 7465 7374 5f7a 6f6f 645f  .', latest_zood_
-00000d40: 7665 7273 696f 6e29 0d0a 2020 2020 2320  version)..    # 
-00000d50: 2020 2020 6966 206c 6174 6573 745f 7a6f      if latest_zo
-00000d60: 6f64 5f76 6572 7369 6f6e 203d 3d20 7665  od_version == ve
-00000d70: 7273 696f 6e3a 0d0a 2020 2020 2320 2020  rsion:..    #   
-00000d80: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00000d90: 2020 2320 2020 2020 656c 7365 3a0d 0a20    #     else:.. 
-00000da0: 2020 2023 2020 2020 2020 2020 2064 6f77     #         dow
-00000db0: 6e6c 6f61 6420 3d20 696e 7075 7428 6627  nload = input(f'
-00000dc0: e698 afe5 90a6 e8a6 81e4 b88b e8bd bde6  ................
-00000dd0: 9c80 e696 b0e7 8988 207a 6f6f 643d 3d7b  ........ zood=={
-00000de0: 6c61 7465 7374 5f7a 6f6f 645f 7665 7273  latest_zood_vers
-00000df0: 696f 6e7d 2028 7965 732f 6e6f 295b 7965  ion} (yes/no)[ye
-00000e00: 735d 2027 290d 0a20 2020 2023 2020 2020  s] ')..    #    
-00000e10: 2020 2020 2069 6620 646f 776e 6c6f 6164       if download
-00000e20: 203d 3d20 2727 206f 7220 646f 776e 6c6f   == '' or downlo
-00000e30: 6164 203d 3d20 2779 6573 273a 0d0a 2020  ad == 'yes':..  
-00000e40: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-00000e50: 7072 696e 7428 27e6 ada3 e59c a8e5 8786  print('.........
-00000e60: e5a4 87e6 9bb4 e696 b02e 2e2e 2729 0d0a  ............')..
-00000e70: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00000e80: 2020 7472 793a 0d0a 2020 2020 2320 2020    try:..    #   
-00000e90: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00000ea0: 2e73 7973 7465 6d28 2770 6970 2069 6e73  .system('pip ins
-00000eb0: 7461 6c6c 202d 2d75 7067 7261 6465 207a  tall --upgrade z
-00000ec0: 6f6f 6427 290d 0a20 2020 2023 2020 2020  ood')..    #    
-00000ed0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00000ee0: 6e74 2827 e5ae 8ce6 8890 e69b b4e6 96b0  nt('............
-00000ef0: 2729 0d0a 2020 2020 2320 2020 2020 2020  ')..    #       
-00000f00: 2020 2020 2020 6578 6365 7074 3a0d 0a20        except:.. 
-00000f10: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-00000f20: 2020 2020 2070 7269 6e74 2827 e69b b4e6       print('....
-00000f30: 96b0 e5bc 82e5 b8b8 2ce8 afb7 e6a3 80e6  ........,.......
-00000f40: 9fa5 e7bd 91e7 bb9c e688 96e4 bba3 e790  ................
-00000f50: 862c e4bd bfe7 94a8 2070 6970 2069 6e73  .,...... pip ins
-00000f60: 7461 6c6c 202d 2d75 7067 7261 6465 207a  tall --upgrade z
-00000f70: 6f6f 6420 e69b b4e6 96b0 2729 0d0a 2020  ood ......')..  
-00000f80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00000f90: 2020 2020 2320 2020 2020 2020 2020 656c      #         el
-00000fa0: 7365 3a0d 0a20 2020 2023 2020 2020 2020  se:..    #      
-00000fb0: 2020 2020 2020 2070 7269 6e74 2827 e980         print('..
-00000fc0: 80e5 87ba e69b b4e6 96b0 e7a8 8be5 ba8f  ................
-00000fd0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00000fe0: 2020 2020 0d0a 2020 2020 2320 656c 6966      ..    # elif
-00000ff0: 2061 7267 732e 636d 645b 305d 203d 3d20   args.cmd[0] == 
-00001000: 2776 6572 7369 6f6e 273a 0d0a 2020 2020  'version':..    
-00001010: 2320 2020 2020 7072 696e 7428 6622 e5bd  #     print(f"..
-00001020: 93e5 898d 7a6f 6f64 e789 88e6 9cac e4b8  ....zood........
-00001030: ba20 7b76 6572 7369 6f6e 7d22 290d 0a0d  . {version}")...
-00001040: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00001050: 2020 2020 7072 696e 7428 6627 e69c aae6      print(f'....
-00001060: 89be e588 b0e6 8c87 e4bb a420 7a6f 6f64  ........... zood
-00001070: 207b 6172 6773 2e63 6d64 5b30 5d7d 2729   {args.cmd[0]}')
+00000000: 0d0a 696d 706f 7274 2079 616d 6c0d 0a69  ..import yaml..i
+00000010: 6d70 6f72 7420 6f73 0d0a 696d 706f 7274  mport os..import
+00000020: 2072 650d 0a69 6d70 6f72 7420 6a73 6f6e   re..import json
+00000030: 0d0a 0d0a 6465 6620 7265 6164 436f 6e66  ....def readConf
+00000040: 6967 4669 6c65 2866 696c 655f 7061 7468  igFile(file_path
+00000050: 3a73 7472 293a 0d0a 2020 2020 6966 206e  :str):..    if n
+00000060: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+00000070: 7328 6669 6c65 5f70 6174 6829 3a0d 0a20  s(file_path):.. 
+00000080: 2020 2020 2020 2070 7269 6e74 496e 666f         printInfo
+00000090: 2827 e689 bee4 b88d e588 b0e6 9687 e4bb  ('..............
+000000a0: b627 202b 2066 696c 655f 7061 7468 290d  .' + file_path).
+000000b0: 0a20 2020 2020 2020 2065 7869 7428 3029  .        exit(0)
+000000c0: 0d0a 2020 2020 0d0a 2020 2020 7769 7468  ..    ..    with
+000000d0: 206f 7065 6e28 6669 6c65 5f70 6174 682c   open(file_path,
+000000e0: 2027 7227 2c20 656e 636f 6469 6e67 3d22   'r', encoding="
+000000f0: 7574 662d 3822 2920 6173 2066 3a0d 0a20  utf-8") as f:.. 
+00000100: 2020 2020 2020 2066 696c 655f 6461 7461         file_data
+00000110: 203d 2066 2e72 6561 6428 290d 0a0d 0a20   = f.read().... 
+00000120: 2020 2064 6174 6120 3d20 7961 6d6c 2e6c     data = yaml.l
+00000130: 6f61 6428 6669 6c65 5f64 6174 612c 204c  oad(file_data, L
+00000140: 6f61 6465 723d 7961 6d6c 2e46 756c 6c4c  oader=yaml.FullL
+00000150: 6f61 6465 7229 0d0a 2020 2020 7265 7475  oader)..    retu
+00000160: 726e 2064 6174 610d 0a0d 0a0d 0a64 6566  rn data......def
+00000170: 2077 7269 7465 436f 6e66 6967 4669 6c65   writeConfigFile
+00000180: 2864 6174 612c 2066 696c 655f 7061 7468  (data, file_path
+00000190: 293a 0d0a 2020 2020 7769 7468 206f 7065  ):..    with ope
+000001a0: 6e28 6669 6c65 5f70 6174 682c 2027 7727  n(file_path, 'w'
+000001b0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
+000001c0: 3827 2920 6173 2066 3a0d 0a20 2020 2020  8') as f:..     
+000001d0: 2020 2079 616d 6c2e 6475 6d70 2864 6174     yaml.dump(dat
+000001e0: 612c 2066 2c61 6c6c 6f77 5f75 6e69 636f  a, f,allow_unico
+000001f0: 6465 3d54 7275 652c 736f 7274 5f6b 6579  de=True,sort_key
+00000200: 733d 4661 6c73 6529 0d0a 0d0a 6465 6620  s=False)....def 
+00000210: 736f 7274 2879 6d6c 293a 0d0a 2020 2020  sort(yml):..    
+00000220: 0d0a 2020 2020 666f 7220 5f2c 6669 6c65  ..    for _,file
+00000230: 7320 696e 2079 6d6c 2e69 7465 6d73 2829  s in yml.items()
+00000240: 3a0d 0a20 2020 2020 2020 2066 696c 6573  :..        files
+00000250: 2e73 6f72 7428 6b65 793d 6c61 6d62 6461  .sort(key=lambda
+00000260: 2069 7465 6d3a 206c 6973 7428 6974 656d   item: list(item
+00000270: 2e76 616c 7565 7328 2929 5b30 5d29 0d0a  .values())[0])..
+00000280: 0d0a 0d0a 6465 6620 7072 696e 7449 6e66  ....def printInf
+00000290: 6f28 6d73 672c 636f 6c6f 723d 2772 6564  o(msg,color='red
+000002a0: 2729 3a0d 0a20 2020 2069 6620 636f 6c6f  '):..    if colo
+000002b0: 7220 3d3d 2027 7265 6427 3a0d 0a20 2020  r == 'red':..   
+000002c0: 2020 2020 2070 7269 6e74 2866 275c 3033       print(f'\03
+000002d0: 335b 313b 3331 6d7b 6d73 677d 5c30 3333  3[1;31m{msg}\033
+000002e0: 5b30 6d27 290d 0a20 2020 2065 6c69 6620  [0m')..    elif 
+000002f0: 636f 6c6f 7220 3d3d 2027 6772 6565 6e27  color == 'green'
+00000300: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00000310: 2866 275c 3033 335b 313b 3332 6d7b 6d73  (f'\033[1;32m{ms
+00000320: 677d 5c30 3333 5b30 6d27 290d 0a20 2020  g}\033[0m')..   
+00000330: 2020 2020 200d 0a64 6566 2067 6574 5a6f       ..def getZo
+00000340: 6f64 436f 6e66 6967 2829 3a0d 0a20 2020  odConfig():..   
+00000350: 200d 0a20 2020 2067 6c6f 6261 6c5f 636f   ..    global_co
+00000360: 6e66 6967 5f70 6174 6820 3d20 6f73 2e70  nfig_path = os.p
+00000370: 6174 682e 6a6f 696e 286f 732e 7061 7468  ath.join(os.path
+00000380: 2e64 6972 6e61 6d65 285f 5f66 696c 655f  .dirname(__file_
+00000390: 5f29 2c27 636f 6e66 6967 272c 275f 636f  _),'config','_co
+000003a0: 6e66 6967 2e79 6d6c 2729 0d0a 2020 2020  nfig.yml')..    
+000003b0: 0d0a 2020 2020 676c 6f62 616c 5f7a 6f6f  ..    global_zoo
+000003c0: 645f 636f 6e66 6967 203d 2072 6561 6443  d_config = readC
+000003d0: 6f6e 6669 6746 696c 6528 676c 6f62 616c  onfigFile(global
+000003e0: 5f63 6f6e 6669 675f 7061 7468 290d 0a20  _config_path).. 
+000003f0: 2020 206d 645f 6469 725f 6e61 6d65 203d     md_dir_name =
+00000400: 2067 6c6f 6261 6c5f 7a6f 6f64 5f63 6f6e   global_zood_con
+00000410: 6669 675b 276d 6172 6b64 6f77 6e5f 666f  fig['markdown_fo
+00000420: 6c64 6572 275d 0d0a 2020 2020 0d0a 2020  lder']..    ..  
+00000430: 2020 6c6f 6361 6c5f 636f 6e66 6967 5f70    local_config_p
+00000440: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00000450: 696e 286d 645f 6469 725f 6e61 6d65 2c27  in(md_dir_name,'
+00000460: 5f63 6f6e 6669 672e 796d 6c27 290d 0a20  _config.yml').. 
+00000470: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
+00000480: 6973 7473 286c 6f63 616c 5f63 6f6e 6669  ists(local_confi
+00000490: 675f 7061 7468 293a 0d0a 2020 2020 2020  g_path):..      
+000004a0: 2020 636f 6e66 6967 5f70 6174 6820 3d20    config_path = 
+000004b0: 6c6f 6361 6c5f 636f 6e66 6967 5f70 6174  local_config_pat
+000004c0: 680d 0a20 2020 2065 6c73 653a 0d0a 2020  h..    else:..  
+000004d0: 2020 2020 2020 636f 6e66 6967 5f70 6174        config_pat
+000004e0: 6820 3d20 676c 6f62 616c 5f63 6f6e 6669  h = global_confi
+000004f0: 675f 7061 7468 0d0a 2020 2020 2020 2020  g_path..        
+00000500: 0d0a 2020 2020 7265 7475 726e 2072 6561  ..    return rea
+00000510: 6443 6f6e 6669 6746 696c 6528 636f 6e66  dConfigFile(conf
+00000520: 6967 5f70 6174 6829 0d0a 0d0a 6465 6620  ig_path)....def 
+00000530: 6361 6375 6c61 7465 4672 6f6e 744e 6578  caculateFrontNex
+00000540: 7428 666c 6174 5f70 6174 6873 3a6c 6973  t(flat_paths:lis
+00000550: 742c 7061 7468 2c6d 645f 6469 725f 6e61  t,path,md_dir_na
+00000560: 6d65 293a 0d0a 0d0a 2020 2020 6469 725f  me):....    dir_
+00000570: 6e61 6d65 203d 2070 6174 682e 7370 6c69  name = path.spli
+00000580: 7428 6f73 2e73 6570 295b 315d 0d0a 2020  t(os.sep)[1]..  
+00000590: 2020 6669 6c65 5f6e 616d 6520 3d20 7061    file_name = pa
+000005a0: 7468 2e73 706c 6974 286f 732e 7365 7029  th.split(os.sep)
+000005b0: 5b32 5d2e 7265 706c 6163 6528 272e 6d64  [2].replace('.md
+000005c0: 272c 2727 290d 0a20 2020 2069 6620 6469  ','')..    if di
+000005d0: 725f 6e61 6d65 203d 3d20 272e 273a 0d0a  r_name == '.':..
+000005e0: 2020 2020 2020 2020 6469 725f 6e61 6d65          dir_name
+000005f0: 203d 206d 645f 6469 725f 6e61 6d65 0d0a   = md_dir_name..
+00000600: 2020 2020 7061 7468 203d 206f 732e 7061      path = os.pa
+00000610: 7468 2e6a 6f69 6e28 6469 725f 6e61 6d65  th.join(dir_name
+00000620: 2c66 696c 655f 6e61 6d65 290d 0a20 2020  ,file_name)..   
+00000630: 2070 6f73 203d 2066 6c61 745f 7061 7468   pos = flat_path
+00000640: 732e 696e 6465 7828 7061 7468 290d 0a20  s.index(path).. 
+00000650: 2020 200d 0a20 2020 2066 726f 6e74 5f75     ..    front_u
+00000660: 726c 203d 2027 5c22 2e5c 2227 0d0a 2020  rl = '\".\"'..  
+00000670: 2020 6e65 7874 5f75 726c 203d 2027 5c22    next_url = '\"
+00000680: 2e5c 2227 0d0a 2020 2020 0d0a 2020 2020  .\"'..    ..    
+00000690: 6966 2070 6f73 2021 3d20 3020 3a0d 0a20  if pos != 0 :.. 
+000006a0: 2020 2020 2020 2066 726f 6e74 5f75 726c         front_url
+000006b0: 203d 2068 746d 6c52 656c 6174 6976 6555   = htmlRelativeU
+000006c0: 726c 2866 6c61 745f 7061 7468 735b 706f  rl(flat_paths[po
+000006d0: 732d 315d 290d 0a20 2020 2069 6620 706f  s-1])..    if po
+000006e0: 7320 213d 206c 656e 2866 6c61 745f 7061  s != len(flat_pa
+000006f0: 7468 7329 2d31 3a0d 0a20 2020 2020 2020  ths)-1:..       
+00000700: 206e 6578 745f 7572 6c20 3d20 6874 6d6c   next_url = html
+00000710: 5265 6c61 7469 7665 5572 6c28 666c 6174  RelativeUrl(flat
+00000720: 5f70 6174 6873 5b70 6f73 2b31 5d29 0d0a  _paths[pos+1])..
+00000730: 0d0a 2020 2020 7265 7475 726e 2066 726f  ..    return fro
+00000740: 6e74 5f75 726c 2c6e 6578 745f 7572 6c0d  nt_url,next_url.
+00000750: 0a20 2020 200d 0a64 6566 2068 746d 6c52  .    ..def htmlR
+00000760: 656c 6174 6976 6555 726c 2875 726c 3a73  elativeUrl(url:s
+00000770: 7472 293a 0d0a 2020 2020 6e65 775f 7572  tr):..    new_ur
+00000780: 6c20 3d20 7572 6c2e 7265 706c 6163 6528  l = url.replace(
+00000790: 6f73 2e73 6570 2c27 2f27 290d 0a20 2020  os.sep,'/')..   
+000007a0: 206e 6577 5f75 726c 203d 2066 275c 222e   new_url = f'\".
+000007b0: 2e2f 2e2e 2f7b 6e65 775f 7572 6c7d 5c22  ./../{new_url}\"
+000007c0: 270d 0a20 2020 2072 6574 7572 6e20 6e65  '..    return ne
+000007d0: 775f 7572 6c0d 0a20 2020 200d 0a64 6566  w_url..    ..def
+000007e0: 2067 6574 4469 7254 7265 6528 6469 7265   getDirTree(dire
+000007f0: 6374 6f72 795f 7472 6565 2c6d 645f 6469  ctory_tree,md_di
+00000800: 725f 6e61 6d65 293a 0d0a 2020 2020 7472  r_name):..    tr
+00000810: 6565 5f68 746d 6c20 3d20 2727 0d0a 2020  ee_html = ''..  
+00000820: 2020 666f 7220 6974 656d 2069 6e20 6469    for item in di
+00000830: 7265 6374 6f72 795f 7472 6565 3a0d 0a20  rectory_tree:.. 
+00000840: 2020 2020 2020 2064 6972 5f6e 616d 6520         dir_name 
+00000850: 3d20 6c69 7374 2869 7465 6d2e 6b65 7973  = list(item.keys
+00000860: 2829 295b 305d 0d0a 2020 2020 2020 2020  ())[0]..        
+00000870: 6669 6c65 7320 3d20 6974 656d 5b64 6972  files = item[dir
+00000880: 5f6e 616d 655d 0d0a 2020 2020 2020 2020  _name]..        
+00000890: 6966 2064 6972 5f6e 616d 6520 3d3d 2027  if dir_name == '
+000008a0: 2e27 3a0d 0a20 2020 2020 2020 2020 2020  .':..           
+000008b0: 2064 6972 5f6e 616d 6520 3d20 6d64 5f64   dir_name = md_d
+000008c0: 6972 5f6e 616d 650d 0a20 2020 2020 2020  ir_name..       
+000008d0: 2020 2020 2066 6f72 2066 696c 6520 696e       for file in
+000008e0: 2066 696c 6573 3a0d 0a20 2020 2020 2020   files:..       
+000008f0: 2020 2020 2020 2020 2064 6972 5f75 726c           dir_url
+00000900: 5f6c 696e 6b20 3d20 6627 2e2e 2f2e 2e2f  _link = f'../../
+00000910: 7b64 6972 5f6e 616d 657d 2f7b 6669 6c65  {dir_name}/{file
+00000920: 7d27 0d0a 2020 2020 2020 2020 2020 2020  }'..            
+00000930: 2020 2020 2320 7072 696e 7428 6469 725f      # print(dir_
+00000940: 7572 6c5f 6c69 6e6b 290d 0a20 2020 2020  url_link)..     
+00000950: 2020 2020 2020 2020 2020 2074 7265 655f             tree_
+00000960: 6874 6d6c 202b 3d20 7472 6565 4974 656d  html += treeItem
+00000970: 2866 696c 652c 6469 725f 7572 6c5f 6c69  (file,dir_url_li
+00000980: 6e6b 290d 0a20 2020 2020 2020 2065 6c73  nk)..        els
+00000990: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000009a0: 7375 625f 7472 6565 5f68 746d 6c20 3d20  sub_tree_html = 
+000009b0: 2727 0d0a 2020 2020 2020 2020 2020 2020  ''..            
+000009c0: 666f 7220 6669 6c65 2069 6e20 6669 6c65  for file in file
+000009d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000009e0: 2020 2020 6469 725f 7572 6c5f 6c69 6e6b      dir_url_link
+000009f0: 203d 2066 272e 2e2f 2e2e 2f7b 6469 725f   = f'../../{dir_
+00000a00: 6e61 6d65 7d2f 7b66 696c 657d 270d 0a20  name}/{file}'.. 
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000a20: 2070 7269 6e74 2864 6972 5f75 726c 5f6c   print(dir_url_l
+00000a30: 696e 6b29 0d0a 2020 2020 2020 2020 2020  ink)..          
+00000a40: 2020 2020 2020 7375 625f 7472 6565 5f68        sub_tree_h
+00000a50: 746d 6c20 2b3d 2074 7265 6549 7465 6d28  tml += treeItem(
+00000a60: 6669 6c65 2c64 6972 5f75 726c 5f6c 696e  file,dir_url_lin
+00000a70: 6b29 0d0a 0d0a 2020 2020 2020 2020 2020  k)....          
+00000a80: 2020 6669 7273 745f 6469 725f 7572 6c5f    first_dir_url_
+00000a90: 6c69 6e6b 203d 2066 272e 2e2f 2e2e 2f7b  link = f'../../{
+00000aa0: 6469 725f 6e61 6d65 7d2f 7b66 696c 6573  dir_name}/{files
+00000ab0: 5b30 5d7d 270d 0a20 2020 2020 2020 2020  [0]}'..         
+00000ac0: 2020 2074 7265 655f 6874 6d6c 202b 3d20     tree_html += 
+00000ad0: 7472 6565 4974 656d 2864 6972 5f6e 616d  treeItem(dir_nam
+00000ae0: 652c 6669 7273 745f 6469 725f 7572 6c5f  e,first_dir_url_
+00000af0: 6c69 6e6b 2c73 7562 5f74 7265 6520 3d20  link,sub_tree = 
+00000b00: 7375 625f 7472 6565 5f68 746d 6c29 0d0a  sub_tree_html)..
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 0d0a 2020 2020 2320 7072 696e 7428 7472  ..    # print(tr
+00000b30: 6565 5f68 746d 6c29 0d0a 2020 2020 7265  ee_html)..    re
+00000b40: 7475 726e 2066 273c 6469 7620 636c 6173  turn f'<div clas
+00000b50: 733d 5c22 6469 722d 7472 6565 5c22 3e7b  s=\"dir-tree\">{
+00000b60: 7472 6565 5f68 746d 6c7d 3c2f 6469 763e  tree_html}</div>
+00000b70: 270d 0a0d 0a64 6566 2074 7265 6549 7465  '....def treeIte
+00000b80: 6d28 6e61 6d65 2c64 6972 5f75 726c 5f6c  m(name,dir_url_l
+00000b90: 696e 6b2c 7375 625f 7472 6565 203d 2046  ink,sub_tree = F
+00000ba0: 616c 7365 293a 0d0a 2020 2020 6966 2073  alse):..    if s
+00000bb0: 7562 5f74 7265 653a 0d0a 2020 2020 2020  ub_tree:..      
+00000bc0: 2020 6c69 6e6b 203d 2066 223c 6120 6872    link = f"<a hr
+00000bd0: 6566 3d5c 227b 6469 725f 7572 6c5f 6c69  ef=\"{dir_url_li
+00000be0: 6e6b 7d5c 2220 3e7b 6e61 6d65 7d3c 2f61  nk}\" >{name}</a
+00000bf0: 3e22 0d0a 2020 2020 2020 2020 7265 7475  >"..        retu
+00000c00: 726e 2066 273c 756c 3e3c 6c69 3e7b 6c69  rn f'<ul><li>{li
+00000c10: 6e6b 7d7b 7375 625f 7472 6565 7d3c 2f6c  nk}{sub_tree}</l
+00000c20: 693e 3c2f 756c 3e27 0d0a 2020 2020 656c  i></ul>'..    el
+00000c30: 7365 3a0d 0a20 2020 2020 2020 206c 696e  se:..        lin
+00000c40: 6b20 3d20 6622 3c61 2068 7265 663d 5c22  k = f"<a href=\"
+00000c50: 7b64 6972 5f75 726c 5f6c 696e 6b7d 5c22  {dir_url_link}\"
+00000c60: 203e 7b6e 616d 657d 3c2f 613e 220d 0a20   >{name}</a>".. 
+00000c70: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
+00000c80: 3c75 6c3e 3c6c 693e 7b6c 696e 6b7d 3c2f  <ul><li>{link}</
+00000c90: 6c69 3e3c 2f75 6c3e 270d 0a0d 0a64 6566  li></ul>'....def
+00000ca0: 2075 726c 5265 706c 6163 6528 6874 6d6c   urlReplace(html
+00000cb0: 5f74 656d 706c 6174 652c 6672 6f6e 745f  _template,front_
+00000cc0: 7572 6c2c 6e65 7874 5f75 726c 2c63 6f6e  url,next_url,con
+00000cd0: 7472 6f6c 293a 0d0a 2020 2020 0d0a 2020  trol):..    ..  
+00000ce0: 2020 6874 6d6c 5f74 656d 706c 6174 6520    html_template 
+00000cf0: 3d20 6874 6d6c 5f74 656d 706c 6174 652e  = html_template.
+00000d00: 7265 706c 6163 6528 273c 2566 726f 6e74  replace('<%front
+00000d10: 5f75 726c 253e 272c 6672 6f6e 745f 7572  _url%>',front_ur
+00000d20: 6c29 2e72 6570 6c61 6365 2827 3c25 6e65  l).replace('<%ne
+00000d30: 7874 5f75 726c 253e 272c 6e65 7874 5f75  xt_url%>',next_u
+00000d40: 726c 290d 0a20 2020 2068 746d 6c5f 7465  rl)..    html_te
+00000d50: 6d70 6c61 7465 203d 2068 746d 6c5f 7465  mplate = html_te
+00000d60: 6d70 6c61 7465 2e72 6570 6c61 6365 2827  mplate.replace('
+00000d70: 3c25 636f 6e74 726f 6c25 3e27 2c66 275c  <%control%>',f'\
+00000d80: 227b 636f 6e74 726f 6c7d 5c22 2729 0d0a  "{control}\"')..
+00000d90: 2020 2020 7265 7475 726e 2068 746d 6c5f      return html_
+00000da0: 7465 6d70 6c61 7465 0d0a 0d0a 6465 6620  template....def 
+00000db0: 6765 7441 6c6c 4150 4954 6578 7428 6d61  getAllAPIText(ma
+00000dc0: 726b 646f 776e 5f68 746d 6c73 2c73 6561  rkdown_htmls,sea
+00000dd0: 7263 685f 7363 6f70 652c 6d64 5f64 6972  rch_scope,md_dir
+00000de0: 5f6e 616d 6529 3a0d 0a20 2020 2020 2020  _name):..       
+00000df0: 2020 0d0a 2020 2020 616c 6c5f 6b65 7973    ..    all_keys
+00000e00: 203d 206d 6172 6b64 6f77 6e5f 6874 6d6c   = markdown_html
+00000e10: 732e 6b65 7973 2829 0d0a 2020 2020 4150  s.keys()..    AP
+00000e20: 495f 7465 7874 203d 207b 7d0d 0a20 2020  I_text = {}..   
+00000e30: 2066 6f72 206b 6579 2069 6e20 616c 6c5f   for key in all_
+00000e40: 6b65 7973 3a0d 0a20 2020 2020 2020 2073  keys:..        s
+00000e50: 706c 6974 6564 5f6b 6579 203d 206b 6579  plited_key = key
+00000e60: 2e73 706c 6974 286f 732e 7365 7029 0d0a  .split(os.sep)..
+00000e70: 2020 2020 2020 2020 6469 725f 6e61 6d65          dir_name
+00000e80: 203d 2073 706c 6974 6564 5f6b 6579 5b31   = splited_key[1
+00000e90: 5d0d 0a20 2020 2020 2020 200d 0a20 2020  ]..        ..   
+00000ea0: 2020 2020 2069 6620 6c65 6e28 7365 6172       if len(sear
+00000eb0: 6368 5f73 636f 7065 2920 213d 2030 3a0d  ch_scope) != 0:.
+00000ec0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000ed0: 6469 725f 6e61 6d65 206e 6f74 2069 6e20  dir_name not in 
+00000ee0: 7365 6172 6368 5f73 636f 7065 3a0d 0a20  search_scope:.. 
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000f00: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+00000f10: 2069 6620 6469 725f 6e61 6d65 203d 3d20   if dir_name == 
+00000f20: 272e 273a 0d0a 2020 2020 2020 2020 2020  '.':..          
+00000f30: 2020 6469 725f 6e61 6d65 203d 206d 645f    dir_name = md_
+00000f40: 6469 725f 6e61 6d65 0d0a 2020 2020 2020  dir_name..      
+00000f50: 2020 6669 6c65 5f6e 616d 6520 3d20 7370    file_name = sp
+00000f60: 6c69 7465 645f 6b65 795b 325d 2e72 6570  lited_key[2].rep
+00000f70: 6c61 6365 2827 2e6d 6427 2c27 2729 0d0a  lace('.md','')..
+00000f80: 2020 2020 2020 2020 6d61 726b 646f 776e          markdown
+00000f90: 5f74 6578 7420 3d20 7265 2e73 7562 2872  _text = re.sub(r
+00000fa0: 273c 2e2a 3f3e 272c 2727 2c6d 6172 6b64  '<.*?>','',markd
+00000fb0: 6f77 6e5f 6874 6d6c 735b 6b65 795d 292e  own_htmls[key]).
+00000fc0: 7265 706c 6163 6528 275c 2227 2c27 2729  replace('\"','')
+00000fd0: 2e72 6570 6c61 6365 2827 5c27 272c 2727  .replace('\'',''
+00000fe0: 292e 7265 706c 6163 6528 275c 5c27 2c27  ).replace('\\','
+00000ff0: 2729 0d0a 2020 2020 2020 2020 7061 7468  ')..        path
+00001000: 203d 2066 272e 2e2f 2e2e 2f7b 6469 725f   = f'../../{dir_
+00001010: 6e61 6d65 7d2f 7b66 696c 655f 6e61 6d65  name}/{file_name
+00001020: 7d27 0d0a 2020 2020 2020 2020 4150 495f  }'..        API_
+00001030: 7465 7874 5b70 6174 685d 203d 206d 6172  text[path] = mar
+00001040: 6b64 6f77 6e5f 7465 7874 0d0a 2020 2020  kdown_text..    
+00001050: 0d0a 2020 2020 6a73 6f6e 5f41 5049 5f74  ..    json_API_t
+00001060: 6578 7420 3d20 6a73 6f6e 2e64 756d 7073  ext = json.dumps
+00001070: 2841 5049 5f74 6578 7429 2e72 6570 6c61  (API_text).repla
+00001080: 6365 2827 5c22 272c 275c 5c5c 2227 292e  ce('\"','\\\"').
+00001090: 7265 706c 6163 6528 275c 5c6e 272c 2727  replace('\\n',''
+000010a0: 290d 0a20 2020 2072 6574 7572 6e20 6627  )..    return f'
+000010b0: 5c22 7b6a 736f 6e5f 4150 495f 7465 7874  \"{json_API_text
+000010c0: 7d5c 2227                                }\"'
```

### Comparing `zood-0.7.5/zood/md_parser.py` & `zood-0.7.6/zood/md_parser.py`

 * *Files identical despite different names*

### Comparing `zood-0.7.5/zood/zood.py` & `zood-0.7.6/zood/zood.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,16 @@
     markdown_htmls = {}
     for dir_name, files in dir_yml.items():
         file_names = []
         for i in files:
             file_name = list(i.keys())[0]
             file_path = os.path.join(md_dir_name,dir_name,file_name+'.md')
             if not os.path.exists(file_path):
-                printInfo('[zood解析失败]: 请检查 dir.yml')
-                printInfo('找不到文件 ' + file_path)
+                printInfo('[zood解析失败]: 找不到文件' + file_path)
+                print("如手动删除md文件可使用 zood update 更新 dir.yml")
                 exit(0)
             else:
                 with open(file_path,'r',encoding='utf-8') as f:
                     markdown_htmls[file_path] = MarkdownParser.parse_withtag(f.read())
                 file_names.append(file_name)
         directory_tree.append({dir_name:file_names})
```

### Comparing `zood-0.7.5/setup.py` & `zood-0.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkdownParser', 'PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['zood = zood.main:main']}
 
 setup_kwargs = {
     'name': 'zood',
-    'version': '0.7.5',
+    'version': '0.7.6',
     'description': 'web page documentation & comment generation documentation',
     'long_description': '# zood\n\nzood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客\n\n## 主题预览\n\n[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)\n\n## 安装与使用\n\n```bash\npip install zood\n```\n\n参见 [用户使用文档](https://luzhixing12345.github.io/zood/)\n\n## 参考\n\n- [UI](https://remixicon.com/)',
     'author': 'kamilu',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/zood',
```

### Comparing `zood-0.7.5/PKG-INFO` & `zood-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.7.5
+Version: 0.7.6
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

