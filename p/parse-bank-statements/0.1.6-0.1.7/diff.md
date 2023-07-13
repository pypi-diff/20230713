# Comparing `tmp/parse_bank_statements-0.1.6.tar.gz` & `tmp/parse_bank_statements-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_bank_statements-0.1.6.tar", last modified: Thu Mar  2 20:26:14 2023, max compression
+gzip compressed data, was "parse_bank_statements-0.1.7.tar", last modified: Thu Jul 13 14:45:19 2023, max compression
```

## Comparing `parse_bank_statements-0.1.6.tar` & `parse_bank_statements-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/
--rw-r--r--   0 git      (13229) t3tok     (2400)     1080 2021-09-21 19:19:04.000000 parse_bank_statements-0.1.6/LICENSE
--rw-r--r--   0 git      (13229) t3tok     (2400)       13 2021-10-12 10:17:43.000000 parse_bank_statements-0.1.6/MANIFEST.in
--rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/PKG-INFO
--rw-r--r--   0 git      (13229) t3tok     (2400)     1109 2023-01-18 17:34:48.000000 parse_bank_statements-0.1.6/README.md
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements/
--rw-r--r--   0 git      (13229) t3tok     (2400)      657 2023-03-02 20:23:24.000000 parse_bank_statements-0.1.6/parse_bank_statements/__init__.py
--rw-r--r--   0 git      (13229) t3tok     (2400)     9799 2023-03-02 20:25:13.000000 parse_bank_statements-0.1.6/parse_bank_statements/banks.py
--rw-r--r--   0 git      (13229) t3tok     (2400)      973 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.6/parse_bank_statements/dates.py
--rw-r--r--   0 git      (13229) t3tok     (2400)    10846 2023-01-19 10:07:01.000000 parse_bank_statements-0.1.6/parse_bank_statements/pbs_gui.py
--rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.6/parse_bank_statements/pbs_style.py
--rwxr-xr-x   0 git      (13229) t3tok     (2400)      622 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.6/parse_bank_statements/pdf2csv.py
-drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/
--rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/PKG-INFO
--rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/SOURCES.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)        1 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/dependency_links.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)       10 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/requires.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)       22 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/parse_bank_statements.egg-info/top_level.txt
--rw-r--r--   0 git      (13229) t3tok     (2400)      104 2021-09-21 19:23:22.000000 parse_bank_statements-0.1.6/pyproject.toml
--rw-r--r--   0 git      (13229) t3tok     (2400)      646 2023-03-02 20:26:14.000000 parse_bank_statements-0.1.6/setup.cfg
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1080 2021-09-21 19:19:04.000000 parse_bank_statements-0.1.7/LICENSE
+-rw-r--r--   0 git      (13229) t3tok     (2400)       13 2021-10-12 10:17:43.000000 parse_bank_statements-0.1.7/MANIFEST.in
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/PKG-INFO
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1109 2023-01-18 17:34:48.000000 parse_bank_statements-0.1.7/README.md
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements/
+-rw-r--r--   0 git      (13229) t3tok     (2400)      657 2023-07-13 14:41:57.000000 parse_bank_statements-0.1.7/parse_bank_statements/__init__.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)     9799 2023-03-02 20:25:13.000000 parse_bank_statements-0.1.7/parse_bank_statements/banks.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)      973 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/dates.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)    10927 2023-07-13 14:44:49.000000 parse_bank_statements-0.1.7/parse_bank_statements/pbs_gui.py
+-rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/pbs_style.py
+-rwxr-xr-x   0 git      (13229) t3tok     (2400)      622 2023-01-19 09:37:51.000000 parse_bank_statements-0.1.7/parse_bank_statements/pdf2csv.py
+drwxr-xr-x   0 git      (13229) t3tok     (2400)        0 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/
+-rw-r--r--   0 git      (13229) t3tok     (2400)     1576 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/PKG-INFO
+-rw-r--r--   0 git      (13229) t3tok     (2400)      487 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/SOURCES.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)        1 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/dependency_links.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)       10 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/requires.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)       22 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/parse_bank_statements.egg-info/top_level.txt
+-rw-r--r--   0 git      (13229) t3tok     (2400)      104 2021-09-21 19:23:22.000000 parse_bank_statements-0.1.7/pyproject.toml
+-rw-r--r--   0 git      (13229) t3tok     (2400)      646 2023-07-13 14:45:19.000000 parse_bank_statements-0.1.7/setup.cfg
```

### Comparing `parse_bank_statements-0.1.6/LICENSE` & `parse_bank_statements-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.6/PKG-INFO` & `parse_bank_statements-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse_bank_statements
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package to parse bank statements
 Home-page: https://github.com/tardini/parse_bank_statements.git
 Author: Giovanni Tardini
 Author-email: giovannitardini@yahoo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parse_bank_statements-0.1.6/README.md` & `parse_bank_statements-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements/__init__.py` & `parse_bank_statements-0.1.7/parse_bank_statements/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 """Parse bank statements
 """
 
 import os, logging
 
 __author__  = 'Giovanni Tardini'
-__version__ = '0.1.6'
-__date__    = '02.03.2023'
+__version__ = '0.1.7'
+__date__    = '13.07.2023'
 
 
 fmt = logging.Formatter('%(asctime)s | %(name)s | %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
 hnd = logging.StreamHandler()
 hnd.setFormatter(fmt)
 hnd.setLevel(level=logging.INFO)
 logger = logging.getLogger('PBS')
```

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements/banks.py` & `parse_bank_statements-0.1.7/parse_bank_statements/banks.py`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements/dates.py` & `parse_bank_statements-0.1.7/parse_bank_statements/dates.py`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements/pbs_gui.py` & `parse_bank_statements-0.1.7/parse_bank_statements/pbs_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,35 +171,36 @@
         bank2 = ttk.Radiobutton(bankframe, text='DiBa', variable=self.bank_wid, value='diba', command=self.sel)
         bank3 = ttk.Radiobutton(bankframe, text='Visa', variable=self.bank_wid, value='visa', command=self.sel)
         bank4 = ttk.Radiobutton(bankframe, text='KSKMSE', variable=self.bank_wid, value='kskmse', command=self.sel)
         for rb in bank1, bank2, bank3, bank4:
             rb.pack(side=tk.LEFT)
 
         ttk.Label(wordframe, text='Keyword').pack(side=tk.LEFT)
-        self.word_wid = tk.Entry(wordframe, width=40)
-        self.word_wid.insert(0, 'plasma')
-        self.word_wid.pack(side=tk.LEFT)
+        self.word_wid = tk.StringVar()
+        word_wid = ttk.Entry(wordframe, width=406, textvariable=self.word_wid)
+        word_wid.insert(0, 'plasma')
+        word_wid.pack(side=tk.LEFT)
 
         ttk.Label(dirframe, text='Start dir', width=12).pack(side=tk.LEFT)
         self.dir_wid = tk.Entry(dirframe, width=40)
         self.dir_wid.pack(side=tk.LEFT)
         self.sel()
 
         ttk.Label(year1frame, text='Year start', width=12).pack(side=tk.LEFT)
         self.year_beg = tk.IntVar()
-        self.year_beg = tk.Entry(year1frame, width=6)
-        self.year_beg.insert(0, 2015)
-        self.year_beg.pack(side=tk.LEFT)
+        year_beg = ttk.Entry(year1frame, width=6, textvariable=self.year_beg)
+        year_beg.insert(0, 2015)
+        year_beg.pack(side=tk.LEFT)
 
         now = datetime.datetime.now()
         ttk.Label(year2frame, text='Year end', width=12).pack(side=tk.LEFT)
         self.year_end = tk.IntVar()
-        self.year_end = tk.Entry(year2frame, width=6)
-        self.year_end.insert(0, now.year)
-        self.year_end.pack(side=tk.LEFT)
+        year_end = tk.Entry(year2frame, width=6, textvariable=self.year_end)
+        year_end.insert(0, now.year)
+        year_end.pack(side=tk.LEFT)
 
         ttk.Label(amountframe, text='Total').pack(side=tk.LEFT)
         self.amount_wid = tk.StringVar()
         amnt = ttk.Entry(amountframe, width=12, textvariable=self.amount_wid)
         amnt.insert(0, '')
         amnt.pack(side=tk.LEFT)
```

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements/pdf2csv.py` & `parse_bank_statements-0.1.7/parse_bank_statements/pdf2csv.py`

 * *Files identical despite different names*

### Comparing `parse_bank_statements-0.1.6/parse_bank_statements.egg-info/PKG-INFO` & `parse_bank_statements-0.1.7/parse_bank_statements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parse-bank-statements
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package to parse bank statements
 Home-page: https://github.com/tardini/parse_bank_statements.git
 Author: Giovanni Tardini
 Author-email: giovannitardini@yahoo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parse_bank_statements-0.1.6/setup.cfg` & `parse_bank_statements-0.1.7/setup.cfg`

 * *Files identical despite different names*

