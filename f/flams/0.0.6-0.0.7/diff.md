# Comparing `tmp/flams-0.0.6.tar.gz` & `tmp/flams-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-0.0.6.tar", last modified: Thu May 25 08:16:28 2023, max compression
+gzip compressed data, was "flams-0.0.7.tar", last modified: Thu Jul 13 09:15:23 2023, max compression
```

## Comparing `flams-0.0.6.tar` & `flams-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-25 08:16:28.783612 flams-0.0.6/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-09 12:23:21.000000 flams-0.0.6/LICENSE
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5553 2023-05-25 08:16:28.783612 flams-0.0.6/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5293 2023-05-17 13:39:22.000000 flams-0.0.6/README.md
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-25 08:16:28.783612 flams-0.0.6/flams/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.6/flams/__init__.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-25 08:16:28.783612 flams-0.0.6/flams/databases/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.6/flams/databases/__init__.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-05-09 12:23:21.000000 flams-0.0.6/flams/databases/cplmv4.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     8914 2023-05-22 08:20:05.000000 flams-0.0.6/flams/databases/setup.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     3485 2023-05-17 13:39:22.000000 flams-0.0.6/flams/display.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2450 2023-05-17 13:39:22.000000 flams-0.0.6/flams/flams.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    13381 2023-05-17 13:39:22.000000 flams-0.0.6/flams/input.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12425 2023-05-17 13:39:22.000000 flams-0.0.6/flams/run_blast.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      960 2023-05-09 12:59:47.000000 flams-0.0.6/flams/utils.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-25 08:16:28.783612 flams-0.0.6/flams.egg-info/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5553 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/SOURCES.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/dependency_links.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/entry_points.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      131 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/requires.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-25 08:16:28.000000 flams-0.0.6/flams.egg-info/top_level.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-05-25 08:05:32.000000 flams-0.0.6/pyproject.toml
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      426 2023-05-25 07:51:05.000000 flams-0.0.6/requirements.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-25 08:16:28.783612 flams-0.0.6/setup.cfg
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     1286 2023-07-13 09:08:42.000000 flams-0.0.7/LICENSE
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-13 09:15:23.523689 flams-0.0.7/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7038 2023-07-13 09:08:42.000000 flams-0.0.7/README.md
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.7/flams/__init__.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams/databases/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.7/flams/databases/__init__.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2827 2023-07-13 09:08:42.000000 flams-0.0.7/flams/databases/cplmv4.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     8930 2023-07-13 09:08:42.000000 flams-0.0.7/flams/databases/setup.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     3485 2023-07-13 09:08:42.000000 flams-0.0.7/flams/display.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2429 2023-07-13 09:08:42.000000 flams-0.0.7/flams/flams.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    13397 2023-07-13 09:08:42.000000 flams-0.0.7/flams/input.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12443 2023-07-13 09:08:42.000000 flams-0.0.7/flams/run_blast.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      992 2023-07-13 09:08:42.000000 flams-0.0.7/flams/utils.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-07-13 09:15:23.523689 flams-0.0.7/flams.egg-info/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     7298 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/entry_points.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      131 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/requires.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-07-13 09:15:23.000000 flams-0.0.7/flams.egg-info/top_level.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      496 2023-07-13 09:15:15.000000 flams-0.0.7/pyproject.toml
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      426 2023-07-13 09:08:36.000000 flams-0.0.7/requirements.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-07-13 09:15:23.523689 flams-0.0.7/setup.cfg
```

### Comparing `flams-0.0.6/LICENSE` & `flams-0.0.7/LICENSE`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 FLAMS: Finding Lysine Acylation & other Modification Sites
 
 Authors:
   Hannelore Longin
   Nand Broeckaert
   Maarten Langen
-  
+  Roshan Hari
+  Anna Kramarska
+  Kasper Oikarinen
+
 Contributors:
   Vera van Noort
+  Rob Lavigne
 
 MIT License
 
 Copyright (c) 2023 KU Leuven
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -24,8 +28,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `flams-0.0.6/flams/databases/cplmv4.py` & `flams-0.0.7/flams/databases/cplmv4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: kasgel, hannelorelongin
+@author: hannelorelongin, kasgel
 """
 
 import csv
-import requests
 import logging
-from zipfile import ZipFile
+import requests
 from io import BytesIO, StringIO
-from Bio.SeqRecord import SeqRecord
-from Bio.Seq import Seq
+from zipfile import ZipFile
+
 from Bio import SeqIO
+from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
+
 
 """ cplmv4
 This script downloads the different contents of the CPLM database, and transforms them into a fasta format.
 Script developed to work with CPLM database version 4.
 """
 
 URL = "http://cplm.biocuckoo.cn/Download/{0}.zip"
```

### Comparing `flams-0.0.6/flams/databases/setup.py` & `flams-0.0.7/flams/databases/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: kasgel, hannelorelongin, annkamsk
+@author: annkamsk, hannelorelongin, kasgel, MaartenLangen
 """
 
-from pathlib import Path
 import subprocess
+from dataclasses import dataclass
+from pathlib import Path
 from typing import Any, List
+
 from ..databases import cplmv4
 from ..utils import get_data_dir
-from dataclasses import dataclass
 
 """ setup
 This script contains our modification database, and all associated functions to generate and maintain BLAST databases for each modification type.
 """
 
 @dataclass
 class ModificationDatabase:
```

### Comparing `flams-0.0.6/flams/display.py` & `flams-0.0.7/flams/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: Retro212, hannelorelongin, annkamsk
+@author: annkamsk, hannelorelongin, Retro212
 """
 
 import csv
 import logging
 
 """ setup
 This script deals with returning the results of FLAMS to the user in a .tsv file.
```

### Comparing `flams-0.0.6/flams/input.py` & `flams-0.0.7/flams/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: kasgel, hannelorelongin, annkamsk
+@author: annkamsk, hannelorelongin, kasgel, MaartenLangen
 """
 
 import argparse
 import logging
 import os
+import requests
 import sys
-
 from pathlib import Path
 from typing import Tuple
+
 from Bio import SeqIO
+
 from .databases import setup as db_setup
-import requests
 
 """ setup
 This script deals with parsing the input and checking the validity of all provided arguments.
 """
 
 logging.basicConfig(
         level = logging.INFO,
```

### Comparing `flams-0.0.6/flams/run_blast.py` & `flams-0.0.7/flams/run_blast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: kasgel, hannelorelongin, annkamsk
+@author: annkamsk, hannelorelongin, kasgel, MaartenLangen
 """
 
-from .databases import setup as db_setup
-import re
-import os
 import logging
-
+import os
+import re
 from dataclasses import dataclass
+from pathlib import Path
+
+from Bio.Blast import NCBIXML
 from Bio.Blast.Applications import NcbiblastpCommandline
 from Bio.Blast.Record import Blast, Alignment
-from Bio.Blast import NCBIXML
-from .utils import get_data_dir
-from pathlib import Path
 
+from .databases import setup as db_setup
+from .utils import get_data_dir
 
 """ run_blast
 This script contains all functions necessary to search through the proteins stored in the CPLM database, with BLAST,
-and retrieve those that contain conserved lysine modifications.
+and to retrieve those that contain conserved lysine modifications.
 """
 
 def run_blast(
     input,
     modifications,
     lysine_pos,
     lysine_range=0,
```

### Comparing `flams-0.0.6/flams/utils.py` & `flams-0.0.7/flams/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-@author: kasgel
+@author: hannelorelongin, kasgel, MaartenLangen
 """
 
-from pathlib import Path
 import appdirs
+from pathlib import Path
 
 """ setup
 This script deals with getting a platform-specific directory to store app data.
 E.g. on     Linux: ~/.local/share/<AppName>
             Mac: '/Users/trentm/Library/Application Support/SuperApp'
             Windows: 'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp'
 """
```

