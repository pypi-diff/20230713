# Comparing `tmp/baysalt_christmas-0.1.8.6.tar.gz` & `tmp/baysalt_christmas-0.1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.8.6.tar", last modified: Wed Jul 12 10:17:58 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.9.0.tar", last modified: Thu Jul 13 06:20:22 2023, max compression
```

## Comparing `baysalt_christmas-0.1.8.6.tar` & `baysalt_christmas-0.1.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.202878 baysalt_christmas-0.1.8.6/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.6/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.6/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-12 10:17:58.202727 baysalt_christmas-0.1.8.6/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.6/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.193847 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.197383 baysalt_christmas-0.1.8.6/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    22036 2023-07-12 10:17:28.000000 baysalt_christmas-0.1.8.6/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.197869 baysalt_christmas-0.1.8.6/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.6/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.6/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.6/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.6/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.6/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.6/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.201633 baysalt_christmas-0.1.8.6/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.202400 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.8.6/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.6/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.6/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.6/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-12 10:17:58.202929 baysalt_christmas-0.1.8.6/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-12 10:17:56.000000 baysalt_christmas-0.1.8.6/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.091675 baysalt_christmas-0.1.9.0/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-07-13 03:38:11.000000 baysalt_christmas-0.1.9.0/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.9.0/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-13 06:20:22.091546 baysalt_christmas-0.1.9.0/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.9.0/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.087493 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-13 06:20:22.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-13 06:20:21.000000 baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.089481 baysalt_christmas-0.1.9.0/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    22668 2023-07-13 06:19:54.000000 baysalt_christmas-0.1.9.0/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.089911 baysalt_christmas-0.1.9.0/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.9.0/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.9.0/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.9.0/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-13 04:50:52.000000 baysalt_christmas-0.1.9.0/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.9.0/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.9.0/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.090703 baysalt_christmas-0.1.9.0/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-13 06:20:22.091241 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.9.0/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.9.0/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.9.0/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.9.0/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.9.0/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-13 06:20:22.091728 baysalt_christmas-0.1.9.0/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-13 06:20:20.000000 baysalt_christmas-0.1.9.0/setup.py
```

### Comparing `baysalt_christmas-0.1.8.6/.DS_Store` & `baysalt_christmas-0.1.9.0/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -266,37 +266,37 @@
 00001090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000010b0: 636f 6d70 0000 0000 0000 0000 0000 001a  comp............
 000010c0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000010d0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000010e0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000010f0: 0066 006f 6c67 3153 636f 6d70 0000 0000  .f.olg1Scomp....
-00001100: 0000 1301 0000 001a 0062 0061 0079 0073  .........b.a.y.s
+00001100: 0000 133c 0000 001a 0062 0061 0079 0073  ...<.....b.a.y.s
 00001110: 0061 006c 0074 005f 0063 0068 0072 0069  .a.l.t._.c.h.r.i
 00001120: 0073 0074 006d 0061 0073 002e 0065 0067  .s.t.m.a.s...e.g
 00001130: 0067 002d 0069 006e 0066 006f 6d6f 4444  .g.-.i.n.f.omoDD
-00001140: 626c 6f62 0000 0008 2097 9c75 621b c541  blob.... ..ub..A
+00001140: 626c 6f62 0000 0008 d927 0cab 5a2f c541  blob.....'..Z/.A
 00001150: 0000 001a 0062 0061 0079 0073 0061 006c  .....b.a.y.s.a.l
 00001160: 0074 005f 0063 0068 0072 0069 0073 0074  .t._.c.h.r.i.s.t
 00001170: 006d 0061 0073 002e 0065 0067 0067 002d  .m.a.s...e.g.g.-
 00001180: 0069 006e 0066 006f 6d6f 6444 626c 6f62  .i.n.f.omodDblob
-00001190: 0000 0008 2097 9c75 621b c541 0000 001a  .... ..ub..A....
+00001190: 0000 0008 d927 0cab 5a2f c541 0000 001a  .....'..Z/.A....
 000011a0: 0062 0061 0079 0073 0061 006c 0074 005f  .b.a.y.s.a.l.t._
 000011b0: 0063 0068 0072 0069 0073 0074 006d 0061  .c.h.r.i.s.t.m.a
 000011c0: 0073 002e 0065 0067 0067 002d 0069 006e  .s...e.g.g.-.i.n
 000011d0: 0066 006f 7068 3153 636f 6d70 0000 0000  .f.oph1Scomp....
 000011e0: 0000 5000 0000 0005 0062 0075 0069 006c  ..P......b.u.i.l
 000011f0: 0064 6c67 3153 636f 6d70 0000 0000 0001  .dlg1Scomp......
-00001200: b1d7 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
-00001210: 6d6f 4444 626c 6f62 0000 0008 9aef 0785  moDDblob........
-00001220: 331c c541 0000 0005 0062 0075 0069 006c  3..A.....b.u.i.l
-00001230: 0064 6d6f 6444 626c 6f62 0000 0008 9aef  .dmodDblob......
-00001240: 0785 331c c541 0000 0005 0062 0075 0069  ..3..A.....b.u.i
+00001200: cc02 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
+00001210: 6d6f 4444 626c 6f62 0000 0008 c542 3bab  moDDblob.....B;.
+00001220: 5a2f c541 0000 0005 0062 0075 0069 006c  Z/.A.....b.u.i.l
+00001230: 0064 6d6f 6444 626c 6f62 0000 0008 c542  .dmodDblob.....B
+00001240: 3bab 5a2f c541 0000 0005 0062 0075 0069  ;.Z/.A.....b.u.i
 00001250: 006c 0064 7068 3153 636f 6d70 0000 0000  .l.dph1Scomp....
-00001260: 0002 6000 0000 0009 0063 0068 0072 0069  ..`......c.h.r.i
+00001260: 0002 9000 0000 0009 0063 0068 0072 0069  .........c.h.r.i
 00001270: 0073 0074 006d 0061 0073 6277 7370 626c  .s.t.m.a.sbwspbl
 00001280: 6f62 0000 00ba 6270 6c69 7374 3030 d601  ob....bplist00..
 00001290: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000012a0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000012b0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000012c0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000012d0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
@@ -306,15 +306,15 @@
 00001310: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8c  }}...#/;R_klmno.
 00001320: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001330: 0000 0000 0000 0000 0000 0000 0000 008d  ................
 00001340: 0000 0009 0063 0068 0072 0069 0073 0074  .....c.h.r.i.s.t
 00001350: 006d 0061 0073 6473 636c 626f 6f6c 0100  .m.a.sdsclbool..
 00001360: 0000 0900 6300 6800 7200 6900 7300 7400  ....c.h.r.i.s.t.
 00001370: 6d00 6100 736c 6731 5363 6f6d 7000 0000  m.a.slg1Scomp...
-00001380: 0000 021a 7b00 0000 0900 6300 6800 7200  ....{.....c.h.r.
+00001380: 0000 025e 0000 0000 0900 6300 6800 7200  ...^......c.h.r.
 00001390: 6900 7300 7400 6d00 6100 736c 7376 4362  i.s.t.m.a.slsvCb
 000013a0: 6c6f 6200 0003 0062 706c 6973 7430 30d8  lob....bplist00.
 000013b0: 0102 0304 0506 0708 090a 0b16 5354 550a  ............STU.
 000013c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
 000013d0: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
 000013e0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
 000013f0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
@@ -400,20 +400,20 @@
 000018f0: 0169 0172 0174 0175 0176 017f 0181 0182  .i.r.t.u.v......
 00001900: 0184 0185 018e 0190 0191 0194 0195 019e  ................
 00001910: 01a0 01a1 01a2 01a3 01ac 01b9 01c2 0000  ................
 00001920: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00001930: 0000 0000 0000 0000 0000 0000 01c3 0000  ................
 00001940: 0009 0063 0068 0072 0069 0073 0074 006d  ...c.h.r.i.s.t.m
 00001950: 0061 0073 6d6f 4444 626c 6f62 0000 0008  .a.smoDDblob....
-00001960: 5b8c 5224 621b c541 0000 0009 0063 0068  [.R$b..A.....c.h
+00001960: 16ac cb21 d42f c541 0000 0009 0063 0068  ...!./.A.....c.h
 00001970: 0072 0069 0073 0074 006d 0061 0073 6d6f  .r.i.s.t.m.a.smo
-00001980: 6444 626c 6f62 0000 0008 5b8c 5224 621b  dDblob....[.R$b.
+00001980: 6444 626c 6f62 0000 0008 16ac cb21 d42f  dDblob.......!./
 00001990: c541 0000 0009 0063 0068 0072 0069 0073  .A.....c.h.r.i.s
 000019a0: 0074 006d 0061 0073 7068 3153 636f 6d70  .t.m.a.sph1Scomp
-000019b0: 0000 0000 0003 1000 0000 0009 0063 0068  .............c.h
+000019b0: 0000 0000 0003 8000 0000 0009 0063 0068  .............c.h
 000019c0: 0072 0069 0073 0074 006d 0061 0073 7653  .r.i.s.t.m.a.svS
 000019d0: 726e 6c6f 6e67 0000 0001 0000 0004 0064  rnlong.........d
 000019e0: 0069 0073 0074 6277 7370 626c 6f62 0000  .i.s.tbwspblob..
 000019f0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 00001a00: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 00001a10: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001a20: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
@@ -422,21 +422,21 @@
 00001a50: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
 00001a60: 095f 1019 7b7b 3430 342c 2034 3738 7d2c  ._..{{404, 478},
 00001a70: 207b 3132 3338 2c20 3436 377d 7d09 0815   {1238, 467}}...
 00001a80: 232f 3b52 5f6b 6c6d 6e6f 8b00 0000 0000  #/;R_klmno......
 00001a90: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001aa0: 0000 0000 0000 0000 0000 8c00 0000 0400  ................
 00001ab0: 6400 6900 7300 746c 6731 5363 6f6d 7000  d.i.s.tlg1Scomp.
-00001ac0: 0000 0000 013b 3300 0000 0400 6400 6900  .....;3.....d.i.
-00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 0856  s.tmoDDblob....V
-00001ae0: b20e 8433 1cc5 4100 0000 0400 6400 6900  ...3..A.....d.i.
-00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 0897  s.tmodDblob.....
-00001b00: 05d1 7562 1bc5 4100 0000 0400 6400 6900  ..ub..A.....d.i.
+00001ac0: 0000 0000 0156 a500 0000 0400 6400 6900  .....V......d.i.
+00001ad0: 7300 746d 6f44 4462 6c6f 6200 0000 0890  s.tmoDDblob.....
+00001ae0: 623f ab5a 2fc5 4100 0000 0400 6400 6900  b?.Z/.A.....d.i.
+00001af0: 7300 746d 6f64 4462 6c6f 6200 0000 0890  s.tmodDblob.....
+00001b00: 623f ab5a 2fc5 4100 0000 0400 6400 6900  b?.Z/.A.....d.i.
 00001b10: 7300 7470 6831 5363 6f6d 7000 0000 0000  s.tph1Scomp.....
-00001b20: 0150 0000 0000 0400 6400 6900 7300 7476  .P......d.i.s.tv
+00001b20: 0170 0000 0000 0400 6400 6900 7300 7476  .p......d.i.s.tv
 00001b30: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
 00001b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `baysalt_christmas-0.1.8.6/PKG-INFO` & `baysalt_christmas-0.1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.8.6
+Version: 0.1.9.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.6/README.md` & `baysalt_christmas-0.1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.8.6
+Version: 0.1.9.0
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.9.0/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/Blogging.py` & `baysalt_christmas-0.1.9.0/christmas/Blogging.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,36 +49,37 @@
                  _switch_write_all_log=False,  # 是否写入日志
                  _switch_write_bug_log=False,  # 是否写入日志
                  _switch_print_log=True,  # 是否打印日志
                  _switch_write_debug_log=False,  # 是否写入单独的debug日志
                  _switch_write_info_log=False,  # 是否写入单独的info日志
                  _switch_write_warning_log=False,  # 是否写入单独的warning日志
                  _switch_write_error_log=False,  # 是否写入单独的error日志
-                 _switch_write_critical_log=False, # 是否写入单独的critical日志
-                 _manual_setBlog=False ): # 是否手动设置参数
+                 _switch_write_critical_log=False,  # 是否写入单独的critical日志
+                 _switch_bold_print=True):  # 是否打印彩色日志
         
         self.CRITICAL = logging.CRITICAL
         self.FATAL = self.CRITICAL
         self.ERROR = logging.ERROR
         self.WARNING = logging.WARNING
         self.WARN = self.WARNING
         self.INFO = logging.INFO
         self.DEBUG = logging.DEBUG
         self.NOTSET = logging.NOTSET
 
         self.loger_name = _loger_name  # 日志记录器名称
         self.logfile_name = _log_filename  # 日志文件名
         self.switch_write_all_log = _switch_write_all_log  # 是否写入全部日志
-        self.switch_write_bugs_log = _switch_write_bug_log  # 是否写入错误日志
+        self.switch_write_error_plus_log = _switch_write_bug_log  # 是否写入错误日志
         self.switch_print_log = _switch_print_log  # 是否打印日志
         self.switch_write_debug_log = _switch_write_debug_log  # 是否写入单独的debug日志
         self.switch_write_info_log = _switch_write_info_log  # 是否写入单独的info日志
         self.switch_write_warning_log = _switch_write_warning_log  # 是否写入单独的warning日志
         self.switch_write_error_log = _switch_write_error_log  # 是否写入单独的error日志
         self.switch_write_critical_log = _switch_write_critical_log  # 是否写入单独的critical日志
+        self.switch_bold_print = _switch_bold_print  # 是否打印彩色日志
         
         self.log_level = None  # 日志级别
         self.maxBytes = None  # 日志文件大小
         self.backupCount = None  # 日志文件数量
         self.write_mode = None  # 日志写入模式
         self.colors_config = None  # 控制台打印颜色配置信息
         self.log_ddt_fmt = None  # 日志文件名时间格式
@@ -88,15 +89,15 @@
         self.info_log_filename = None  # info日志文件路径
         self.warning_log_filename = None  # warning日志文件路径
         self.error_log_filename = None  # error日志文件路径
         self.critical_log_filename = None  # critical日志文件路径
         self.Rotating = None  # 日志文件处理器 time or size
         self.when = None  # 日志文件处理器 time --> S M H D W
         self.interval = None  # 日志文件处理器 time --> 间隔
-        self.logger = logging.getLogger(self.loger_name)  # 创建日志记录器
+        self._logger = logging.getLogger(self.loger_name)  # 创建日志记录器
         
         self.PARA_DEFAULT = {
             'maxBytes': 1024 * 1024 * 10,  # 日志文件大小
             'backupCount': 5,  # 日志文件数量
             'colors_config': self.__set_console_color_default(),  # 日志输出颜色
             'log_level': logging.INFO,  # 日志级别
             'log_ddt_fmt': '%Y-%m-%d',  # 日志文件名时间格式
@@ -119,17 +120,16 @@
             self.PARA_DEFAULT['debug_log_filename'] = f'{self.logfile_name}_debug.log'
             self.PARA_DEFAULT['info_log_filename'] = f'{self.logfile_name}_info.log'
             self.PARA_DEFAULT['warning_log_filename'] = f'{self.logfile_name}_warning.log'
             self.PARA_DEFAULT['error_log_filename'] = f'{self.logfile_name}_error.log'
             self.PARA_DEFAULT['critical_log_filename'] = f'{self.logfile_name}_critical.log'
         
         self.PARA = self.PARA_DEFAULT
-        if not _manual_setBlog:
-            self.setup_Blog()
-            self.console()
+        self.setup_Blog()
+        # self.console()
     
     def setup_Blog(self, **kwargs):
         
         self.PARA.update(kwargs)
         self.maxBytes = self.PARA['maxBytes']
         self.backupCount = self.PARA['backupCount']
         self.colors_config = self.PARA['colors_config']
@@ -151,18 +151,18 @@
             rmfiles(self.all_log_filename,
                     self.bug_log_filename,
                     self.debug_log_filename,
                     self.info_log_filename,
                     self.warning_log_filename,
                     self.error_log_filename,
                     self.critical_log_filename)
-        self.__rm_random_FileHandler()  # 删除日志记录器handler
+        self.__rm_single_FileHandler()  # 删除日志记录器handler
         #       实例化之后，再次调用setup_Blog()，会重复添加handler，导致日志重复打印 --> 已解决
         # TODO: 实例化之后，再次调用setup_Blog()，会重复添加handler，删除日志记录器handler时，文件已经存在，需要删除文件 --> 未解决
-        self.console()
+        # self.console()
     
     def __init_logger_handler(self, logfile_path, Rotating='time', when='H', interval=1):
         # sourcery skip: inline-immediately-returned-variable
         """
         创建日志记录器handler，用于收集日志
         :param logfile_path: 日志文件路径
         :return: 日志记录器
@@ -189,15 +189,15 @@
     def __set_log_handler(self, logger_handler, level=logging.DEBUG):
         """
         设置handler级别并添加到logger收集器
         :param logger_handler: 日志记录器
         :param level: 日志记录器级别
         """
         logger_handler.setLevel(level=level)
-        self.logger.addHandler(logger_handler)  # 添加到logger收集器
+        self._logger.addHandler(logger_handler)  # 添加到logger收集器
     
     def __set_log_Filter(self, logger_handler, _level):
         """
         设置日志过滤器
         """
         if _level == logging.DEBUG:
             ONLY_LOG = [logging.DEBUG, logging.INFO]
@@ -211,46 +211,55 @@
             ONLY_LOG = [logging.CRITICAL, float('inf')]
         else:
             raise ValueError('日志级别错误')
         log_filter = logging.Filter()
         logger_handler.setLevel(ONLY_LOG[0])
         log_filter.filter = lambda record: (record.levelno < ONLY_LOG[1])  # 设置过滤等级
         logger_handler.addFilter(log_filter)
-        self.logger.addHandler(logger_handler)  # 添加到logger收集器
+        self._logger.addHandler(logger_handler)  # 添加到logger收集器
     
     @staticmethod
     def __set_console_color_default():
         # sourcery skip: inline-immediately-returned-variable
         log_color = {
             # 颜色支持 blue蓝，green绿色，red红色，yellow黄色，cyan青色, purple紫色, white白色, black黑色, grey灰色, bold黑体
             'DEBUG': 'cyan',
             'INFO': 'blue',
             'WARNING': 'yellow',
             'ERROR': 'red',
             'CRITICAL': 'purple',
             'EXCEPTION': 'red',
         }
         return log_color
-    
-    @staticmethod
-    def __set_color_formatter(console_handle, colors_config):
+
+    def __set_color_formatter(self, console_handle, colors_config):
         """
         设置输出格式-控制台
         :param console_handle: 终端日志记录器
         :param colors_config: 控制台打印颜色配置信息
         :return:
         """
-        formatter = colorlog.ColoredFormatter(
-            # 输出那些信息，时间，文件名，函数名等等
-            fmt='%(asctime)s ---> %(log_color)s\033[1m[%(levelname)s]\033[0m %(reset)s%(log_color)s%(message)s %(reset)s',
-            # 时间格式
-            datefmt='%Y-%m-%d %H:%M:%S',
-            log_colors=colors_config,
-            force_color=True,
-        )
+        if self.switch_bold_print:
+            formatter = colorlog.ColoredFormatter(
+                # 输出那些信息，时间，文件名，函数名等等
+                fmt='%(asctime)s ---> %(log_color)s\033[1m[%(levelname)s]\033[0m %(reset)s%(log_color)s%(message)s %(reset)s',
+                # 时间格式
+                datefmt='%Y-%m-%d %H:%M:%S',
+                log_colors=colors_config,
+                force_color=True,
+            )
+        else:
+            formatter = colorlog.ColoredFormatter(
+                # 输出那些信息，时间，文件名，函数名等等
+                fmt='%(asctime)s ---> %(log_color)s%(levelname)s] %(reset)s%(log_color)s%(message)s %(reset)s',
+                # 时间格式
+                datefmt='%Y-%m-%d %H:%M:%S',
+                log_colors=colors_config,
+                force_color=True,
+            )
         console_handle.setFormatter(formatter)
     
     @staticmethod
     def __set_log_formatter(file_handler):
         """
         设置日志输出格式-日志文件
         :param file_handler: 日志记录器
@@ -267,39 +276,39 @@
         关闭日志记录器
         :param logger_handler: 日志记录器
         """
         logger_handler.close()
     
     def console(self):
         """构造日志收集器"""
-        self.logger.setLevel(self.log_level)  # 设置日志收集器级别
+        self._logger.setLevel(self.log_level)  # 设置日志收集器级别
 
-        if self.logger.hasHandlers():  # 如果已经有日志记录器，先关闭
-            self.logger.handlers.clear()
-        if self.logger.filters:  # 如果已经有日志过滤器，先关闭
-            self.logger.filters.clear()
+        if self._logger.hasHandlers():  # 如果已经有日志记录器，先关闭
+            self._logger.handlers.clear()
+        if self._logger.filters:  # 如果已经有日志过滤器，先关闭
+            self._logger.filters.clear()
         if self.switch_write_all_log:  # 是否写入全部日志
             self.__write_all_log()
-        if self.switch_write_bugs_log:  # 是否写入错误日志
+        if self.switch_write_error_plus_log:  # 是否写入错误日志
             self.__write_error_plus_log()
         if self.switch_print_log:  # 是否打印日志
             self.__print_log()
         if self.switch_write_debug_log: # 是否写入debug日志
-            self.__write_random_log(level=logging.DEBUG, _level_log_name=self.debug_log_filename)
+            self.__write_single_log(level=logging.DEBUG, _level_log_name=self.debug_log_filename)
         if self.switch_write_info_log: # 是否写入info日志
-            self.__write_random_log(level=logging.INFO, _level_log_name=self.info_log_filename)
+            self.__write_single_log(level=logging.INFO, _level_log_name=self.info_log_filename)
         if self.switch_write_warning_log: # 是否写入warning日志
-            self.__write_random_log(level=logging.WARNING, _level_log_name=self.warning_log_filename)
+            self.__write_single_log(level=logging.WARNING, _level_log_name=self.warning_log_filename)
         if self.switch_write_error_log: # 是否写入error日志
-            self.__write_random_log(level=logging.ERROR, _level_log_name=self.error_log_filename)
+            self.__write_single_log(level=logging.ERROR, _level_log_name=self.error_log_filename)
         if self.switch_write_critical_log: # 是否写入critical日志
-            self.__write_random_log(level=logging.CRITICAL, _level_log_name=self.critical_log_filename)
+            self.__write_single_log(level=logging.CRITICAL, _level_log_name=self.critical_log_filename)
             
         # 如果console被执行了一次，那么删除之前的执行结果，重新执行
-        return self.logger
+        return self._logger
     
     def __write_all_log(self):
         all_logger_handler = self.__init_logger_handler(self.all_log_filename, Rotating=self.Rotating, when=self.when,
                                                         interval=self.interval)  # 收集所有日志文件
         self.__set_log_formatter(all_logger_handler)  # 设置日志输出格式-all日志文件
         self.__set_log_handler(all_logger_handler, level=logging.DEBUG)  # 设置handler级别并添加到logger收集器
         self.__close_log_handler(all_logger_handler)  # 关闭handler
@@ -313,50 +322,55 @@
     
     def __print_log(self):
         console_handle = colorlog.StreamHandler()  # 创建终端日志记录器handler，用于输出到控制台
         self.__set_color_formatter(console_handle, self.colors_config)  # 设置输出格式-控制台
         self.__set_log_handler(console_handle, level=self.log_level)  # 设置handler级别并添加到终端logger收集器
         self.__close_log_handler(console_handle)  # 关闭handler
     
-    def __write_random_log(self, level=logging.ERROR, _level_log_name='all.log'):  # 日志单独输出
-        random_logger_handler = self.__init_logger_handler(_level_log_name, Rotating=self.Rotating, when=self.when,
+    def __write_single_log(self, level=logging.ERROR, _level_log_name='all.log'):  # 日志单独输出
+        single_logger_handler = self.__init_logger_handler(_level_log_name, Rotating=self.Rotating, when=self.when,
                                                            interval=self.interval)  # 收集随机日志信息文件
-        self.__set_log_formatter(random_logger_handler)  # 设置日志输出格式-random日志文件
-        self.__set_log_Filter(random_logger_handler, level)  # 设置过滤器
-        self.__close_log_handler(random_logger_handler)  # 关闭handler
+        self.__set_log_formatter(single_logger_handler)  # 设置日志输出格式-single日志文件
+        self.__set_log_Filter(single_logger_handler, level)  # 设置过滤器
+        self.__close_log_handler(single_logger_handler)  # 关闭handler
 
-    def __rm_random_FileHandler(self):  # 删除日志文件并关闭日志记录器
-        handlers = self.logger.handlers
+    def __rm_single_FileHandler(self):  # 删除日志文件并关闭日志记录器
+        handlers = self._logger.handlers
         for handler in handlers.copy():
             if isinstance(handler, logging.FileHandler):  # 找到文件处理器，进行删除操作
-                self.logger.removeHandler(handler)
+                self._logger.removeHandler(handler)
                 handler.close()  # 关闭文件处理器，释放资源
 
+    @property
+    def logger(self):
+        self.console()
+        return self._logger
+
     @staticmethod
     def addLevelName(level, levelName):
         logging.addLevelName(level, levelName)
     
     @staticmethod
     def getLevelName(level):
         return logging.getLevelName(level)
 
     def __getitem__(self, item):
         return getattr(self, item)
 
     def __del__(self):
-        # self.logger.handlers.clear()
-        # self.logger.filters.clear()
-        # del self.logger
+        # self._logger.handlers.clear()
+        # self._logger.filters.clear()
+        # del self._logger
         pass
 
     def __str__(self):
         return 'Blog()'
 
     def __call__(self, *args, **kwargs):
-        return self.logger
+        return self._logger
 
 
 def debug(self, *args, **kwargs):
     TF, instanced = whether_instanced(Blog)
     if TF:
         instanced[instanced.keys()[0]].logger.debug(self, *args, **kwargs)
     else:
```

### Comparing `baysalt_christmas-0.1.8.6/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.9.0/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/S_DateTime.py` & `baysalt_christmas-0.1.9.0/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/commonCode.py` & `baysalt_christmas-0.1.9.0/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/cprintf.py` & `baysalt_christmas-0.1.9.0/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.9.0/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.9.0/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.9.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/common.py` & `baysalt_christmas-0.1.9.0/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.9.0/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/processBar.py` & `baysalt_christmas-0.1.9.0/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/read_conf.py` & `baysalt_christmas-0.1.9.0/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/christmas/server_info.py` & `baysalt_christmas-0.1.9.0/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.6/setup.py` & `baysalt_christmas-0.1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.8.6",
+    version="0.1.9.0",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

