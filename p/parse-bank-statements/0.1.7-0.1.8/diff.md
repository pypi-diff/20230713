# Comparing `tmp/parse_bank_statements-0.1.7.tar.gz` & `tmp/parse_bank_statements-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_bank_statements-0.1.7.tar", last modified: Thu Jul 13 14:45:19 2023, max compression
+gzip compressed data, was "parse_bank_statements-0.1.8.tar", last modified: Thu Jul 13 16:19:55 2023, max compression
```

## Comparing `parse_bank_statements-0.1.7.tar` & `parse_bank_statements-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/
--rw-r--r--   0 git      (13229) t3tok     (2400)     1080 2021-09-21 19:19:04.000000 parse_bank_statements-0.1.7/LICENSE
--rw-r--r--   0 git      (13229) t3tok     (2400)       13 2021-10-12 10:17:43.000000 parse_bank_statements-0.1.7/MANIFEST.in
--rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/PKG-INFO
--rw-r--r--   0 git      (13229) t3tok     (2400)     1109 2023-01-18 17:34:48.000000 parse_bank_statements-0.1.7/README.md
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements/
--rw-r--r--   0 git      (13229) t3tok     (2400)      657 2023-07-13 14:41:57.000000 parse_bank_statements-0.1.7/parse_bank_statements/__init__.py
--rw-r--r--   0 git      (13229) t3tok     (2400)     9799 2023-03-02 20:25:13.000000 parse_bank_statements-0.1.7/parse_bank_statements/banks.py
--rw-r--r--   0 git      (13229) t3tok     (2400)      973 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/dates.py
--rw-r--r--   0 git      (13229) t3tok     (2400)    10927 2023-07-13 14:44:49.000000 parse_bank_statements-0.1.7/parse_bank_statements/pbs_gui.py
--rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/pbs_style.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      622 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/pdf2csv.py
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/
--rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/PKG-INFO
--rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/SOURCES.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)        1 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/dependency_links.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)       10 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/requires.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)       22 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/top_level.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)      104 2021-09-21 19:23:22.000000 parse_bank_statements-0.1.7/pyproject.toml
--rw-r--r--   0 git      (13229) t3tok     (2400)      646 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/setup.cfg
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1080 2021-09-21 19:19:04.000000 parse_bank_statements-0.1.8/LICENSE
+-rw-r--r--   0 git      (13229) t3tok     (2400)       13 2021-10-12 10:17:43.000000 parse_bank_statements-0.1.8/MANIFEST.in
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/PKG-INFO
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1109 2023-01-18 17:34:48.000000 parse_bank_statements-0.1.8/README.md
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements/
+-rw-r--r--   0 git      (13229) t3tok     (2400)      657 2023-07-13 16:19:46.000000 parse_bank_statements-0.1.8/parse_bank_statements/__init__.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)     9570 2023-07-13 16:09:18.000000 parse_bank_statements-0.1.8/parse_bank_statements/banks.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)      973 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.8/parse_bank_statements/dates.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)    11016 2023-07-13 16:17:42.000000 parse_bank_statements-0.1.8/parse_bank_statements/pbs_gui.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.8/parse_bank_statements/pbs_style.py
+-rwxr-xr-x   0 git      (13229) t3tok     (2400)      622 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.8/parse_bank_statements/pdf2csv.py
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/PKG-INFO
+-rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/SOURCES.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)        1 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/dependency_links.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)       10 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/requires.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)       22 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/parse_bank_statements.egg-info/top_level.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)      104 2021-09-21 19:23:22.000000 parse_bank_statements-0.1.8/pyproject.toml
+-rw-r--r--   0 git      (13229) t3tok     (2400)      646 2023-07-13 16:19:55.000000 parse_bank_statements-0.1.8/setup.cfg
```

### Comparing `parse_bank_statements-0.1.7/LICENSE` & `parse_bank_statements-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.7/PKG-INFO` & `parse_bank_statements-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_bank_statements
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to parse bank statements
 Home-page: https://github.com/tardini/parse_bank_statements.git
 Author: Giovanni Tardini
 Author-email: giovannitardini@yahoo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parse_bank_statements-0.1.7/README.md` & `parse_bank_statements-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements/__init__.py` & `parse_bank_statements-0.1.8/parse_bank_statements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Parse bank statements
 """
 
 import os, logging
 
 __author__  = 'Giovanni Tardini'
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 __date__    = '13.07.2023'
 
 
 fmt = logging.Formatter('%(asctime)s | %(name)s | %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
 hnd = logging.StreamHandler()
 hnd.setFormatter(fmt)
 hnd.setLevel(level=logging.INFO)
```

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements/banks.py` & `parse_bank_statements-0.1.8/parse_bank_statements/banks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-import logging, traceback, csv
+import os, logging, traceback, csv
 from parse_bank_statements import dates
 
 logger = logging.getLogger('PBS.banks')
 logger.setLevel(logging.DEBUG)
 
 help = """
 AREA boundaries: (top-y, left-x, bottom-y, right-x).
 COLUMNS separators (x-positions).
 To find them out for the specific PDF column format of a given bank's statements, use e.g. gimp, mode typogr.points.
 """
 
+baseDir = '/afs/ipp-garching.mpg.de/home/g/git/attach'
+if not os.path.isdir(baseDir):
+    baseDir = '/home/gio/bank'
+
 
 def amount_sparkasse(str_in):
     '''Convert string to float (money amount)'''
 
     moneyStr = str_in.strip().replace('.', '').replace(',', '.')
 
     money = 0
@@ -75,16 +79,15 @@
 
 
 
 class sskm:
 
 
     label   = 'sskm'
-    rootDir = '/afs/ipp-garching.mpg.de/home/g/git/attach/sskm/gk'
-#    rootDir = '/home/gio/bank/sskm/gk'
+    rootDir = '%s/sskm/gk' %baseDir
     pdfArea    = (139.5, 60, 707.5, 573)
     pdfColumns = (116.4, 163.3, 360, 465.4)
     ibanStr = 'ubiger-ID:'
 
     def csv2tras(self, fcsv):
         '''Split a statement into a list of transaction dictionaries'''
 
@@ -123,16 +126,15 @@
 
         return(amount_sparkasse(str_in))
 
 
 class sskm2:
 
     label = 'sskm2'
-    rootDir = '/afs/ipp-garching.mpg.de/home/g/git/attach/sskm/gk'
-#    rootDir = '/home/gio/bank/sskm/gk'
+    rootDir = '%s/sskm/gk' %baseDir
     pdfArea    = (139.5, 60, 750, 573)
     pdfColumns = (122.1, 362.8, 470)
     ibanStr = 'ubiger-ID:'
 
     def csv2tras(self, fcsv):
 
         '''Split a statement into a list of transaction dictionaries'''
@@ -169,16 +171,15 @@
 
         return(amount_sparkasse(str_in))
 
 
 class diba:
 
     label   = 'diba'
-    rootDir = '/afs/ipp-garching.mpg.de/home/g/git/attach/lucia/diba'
-#    rootDir = '/home/gio/bank/diba'
+    rootDir = '%s/lucia/diba' %baseDir
     pdfArea    = (190, 67, 765, 568)
     pdfColumns = (131, 507)
     mandatStr   = 'Mandat:'
     referenzStr = 'Referenz:'
 
     def csv2tras(self, fcsv):
         '''Split a statement into a list of transaction dictionaries'''
@@ -216,16 +217,15 @@
             money = None
         return money
 
 
 class visa:
 
     label   = 'visa'
-    rootDir = '/afs/ipp-garching.mpg.de/home/g/git/attach/sskm/kk'
-#    rootDir = '/home/gio/bank/sskm/kk'
+    rootDir = '%s/sskm/kk' %baseDir
     pdfArea    = (300, 37, 750, 590)
     pdfColumns = (80, 120, 280, 360, 450, 530)
 
     def csv2tras(self, fcsv):
         '''Split a statement into a list of transaction dictionaries)'''
 
         logger.debug(fcsv)
@@ -245,16 +245,15 @@
 
         return(amount_sparkasse(str_in))
 
 
 class kskmse:
 
     label   = 'kskmse'
-    rootDir = '/afs/ipp-garching.mpg.de/home/g/git/attach/lucia/kskmse'
-#    rootDir = '/home/gio/bank/kskmse'
+    rootDir = '%s/lucia/kskmse' %baseDir
     pdfArea    = (139.5, 60, 707.5, 573)
     pdfColumns = (116.4, 163.3, 360, 465.4)
     ibanStr = 'ubiger-ID:'
 
     def csv2tras(self, fcsv):
         '''Split a statement into a list of transaction dictionaries'''
```

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements/dates.py` & `parse_bank_statements-0.1.8/parse_bank_statements/dates.py`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements/pbs_gui.py` & `parse_bank_statements-0.1.8/parse_bank_statements/pbs_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,23 +183,23 @@
         ttk.Label(dirframe, text='Start dir', width=12).pack(side=tk.LEFT)
         self.dir_wid = tk.Entry(dirframe, width=40)
         self.dir_wid.pack(side=tk.LEFT)
         self.sel()
 
         ttk.Label(year1frame, text='Year start', width=12).pack(side=tk.LEFT)
         self.year_beg = tk.IntVar()
+        self.year_beg.set(2015)
         year_beg = ttk.Entry(year1frame, width=6, textvariable=self.year_beg)
-        year_beg.insert(0, 2015)
         year_beg.pack(side=tk.LEFT)
 
         now = datetime.datetime.now()
         ttk.Label(year2frame, text='Year end', width=12).pack(side=tk.LEFT)
         self.year_end = tk.IntVar()
+        self.year_end.set(now.year)
         year_end = tk.Entry(year2frame, width=6, textvariable=self.year_end)
-        year_end.insert(0, now.year)
         year_end.pack(side=tk.LEFT)
 
         ttk.Label(amountframe, text='Total').pack(side=tk.LEFT)
         self.amount_wid = tk.StringVar()
         amnt = ttk.Entry(amountframe, width=12, textvariable=self.amount_wid)
         amnt.insert(0, '')
         amnt.pack(side=tk.LEFT)
@@ -240,14 +240,16 @@
 
         tot_year = 0
         out_str = ''
         logger.debug(dir_in)
         year = int(os.path.basename(dir_in))
         if self.bank.label == 'sskm' and year > 2021:
             self.bank = banks.sskm2
+        if self.bank.label == 'sskm2' and year <= 2021:
+            self.bank = banks.sskm
 
         for f_name in sorted(os.listdir(dir_in)):
             fname = '%s/%s' %(dir_in, f_name)
             pre, ext = os.path.splitext(fname)
             if (self.bank.label == 'sskm') and year == 2021:
                 month = pre.split('_')[-1]
                 if month in ('011', '012'):
```

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements/pdf2csv.py` & `parse_bank_statements-0.1.8/parse_bank_statements/pdf2csv.py`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.7/parse_bank_statements.egg-info/PKG-INFO` & `parse_bank_statements-0.1.8/parse_bank_statements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-bank-statements
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to parse bank statements
 Home-page: https://github.com/tardini/parse_bank_statements.git
 Author: Giovanni Tardini
 Author-email: giovannitardini@yahoo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parse_bank_statements-0.1.7/setup.cfg` & `parse_bank_statements-0.1.8/setup.cfg`

 * *Files identical despite different names*

