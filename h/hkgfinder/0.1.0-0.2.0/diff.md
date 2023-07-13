# Comparing `tmp/hkgfinder-0.1.0.tar.gz` & `tmp/hkgfinder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkgfinder-0.1.0.tar", max compression
+gzip compressed data, was "hkgfinder-0.2.0.tar", max compression
```

## Comparing `hkgfinder-0.1.0.tar` & `hkgfinder-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0     1068 2022-05-27 14:25:04.311062 hkgfinder-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     3353 2023-01-26 10:53:20.999902 hkgfinder-0.1.0/README.md
--rwxr-xr-x   0        0        0  5068650 2022-06-30 14:52:03.446320 hkgfinder-0.1.0/db/hkgfinder.hmm
--rwxr-xr-x   0        0        0       22 2022-05-26 18:35:58.113700 hkgfinder-0.1.0/hkgfinder/__init__.py
--rwxr-xr-x   0        0        0    16819 2023-04-21 21:25:56.030415 hkgfinder-0.1.0/hkgfinder/hkgfinder.py
--rwxr-xr-x   0        0        0     4398 2023-01-26 10:51:36.288556 hkgfinder-0.1.0/hkgfinder/utils.py
--rwxr-xr-x   0        0        0     1472 2023-01-26 11:25:04.882874 hkgfinder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 hkgfinder-0.1.0/setup.py
--rw-r--r--   0        0        0     4892 1970-01-01 00:00:00.000000 hkgfinder-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2022-05-27 14:25:04.311062 hkgfinder-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     2485 2023-07-13 15:05:31.210345 hkgfinder-0.2.0/README.md
+-rwxr-xr-x   0        0        0       22 2023-07-13 14:37:24.359341 hkgfinder-0.2.0/hkgfinder/__init__.py
+-rwxr-xr-x   0        0        0  5068650 2022-06-30 14:52:03.446320 hkgfinder-0.2.0/hkgfinder/hkgfinder.hmm
+-rwxr-xr-x   0        0        0    21849 2023-07-13 14:53:57.503741 hkgfinder-0.2.0/hkgfinder/hkgfinder.py
+-rwxr-xr-x   0        0        0     1509 2023-07-13 13:54:40.105271 hkgfinder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 hkgfinder-0.2.0/setup.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 hkgfinder-0.2.0/PKG-INFO
```

### Comparing `hkgfinder-0.1.0/LICENSE` & `hkgfinder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hkgfinder-0.1.0/README.md` & `hkgfinder-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -7,71 +7,48 @@
 [![Downloads](https://img.shields.io/pypi/dm/hkgfinder)](https://pypi.org/project/hkgfinder)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://www.gnu.org/licenses/MIT)
 
 
 ## Find housekeeping genes in prokaryotic (meta)genomes
 
 ### Introduction
-hkgfinder is a fast and accurate housekeeping gene finder and classifier. Hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.
+hkgfinder is a fast and accurate housekeeping gene finder and classifier. hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.
+
 
 ### How hkgfinder works
 ![](img/hkgfinder.png)
 
 ### Installation
 
-You will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.
+~~You will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.~~
 
+**hkgfinder since v0.2 is without external dependencies.**
 
-#### Install from Pip
 
 ```bash
 pip install hkgfinder
 ```
 
-
-#### Install from source
-
-```bash
-# Download hkgfinder development version
-git clone https://github.com/Ebedthan/hkgfinder.git hkgfinder
-
-# Navigate to directory
-cd hkgfinder
-
-# Install with poetry: see https://python-poetry.org
-poetry install --no-dev
-
-# Enter the Python virtual environment with
-poetry shell
-
-# Test hkgfinder is correctly installed
-hkgfinder -h
-```
-
-If you do not want to go into the virtual environment just do:
-
-```bash
-poetry run hkgfinder -h
-```
-
 ## Test
 
 * Type `hkgfinder -h` and it should output something like:
 
 ```
 usage: hkgfinder [options] [<FILE>]
 
-optional arguments:
+options:
   -o [FILE]      output result to FILE [stdout]
   -g             activate genome mode [false]
   -m             activate metagenome mode [false]
-  --faa FILE     output matched proteins sequences to FILE
-  --fna FILE     output matched DNA sequences to FILE
+  --faa FILE     output matched protein sequences to FILE [false]
+  --fna FILE     output matched DNA sequences to FILE [false]
+  -s             output sequences in file by gene [false]
   -t INT         number of threads [1]
   -q             decrease program verbosity
+  -d             enable debug mode
   -v, --version  show program's version number and exit
   -h, --help     show this help message and exit
 ```
 
 
 ## Invoking hkgfinder
 
@@ -82,27 +59,14 @@
 * hkgfinder supports gzip, lzma, bz2 and zstd compressed files.
   
 ## Bugs
 
 Submit problems or requests to the [Issue Tracker](https://github.com/Ebedthan/hkgfinder/issues).
 
 
-## Dependencies
-
-### Mandatory
-
-* [**Prodigal**](https://github.com/sib-swiss/pftools3)  
-  Used for protein-coding gene prediction.    
-  *Hyatt, D., Chen, GL., LoCascio, P.F. et al. Prodigal: prokaryotic gene recognition and translation initiation site identification. BMC Bioinformatics 11, 119 (2010). https://doi.org/10.1186/1471-2105-11-119*
-
-* [**HMMER 3**](https://hmmer.org)  
-  Used for HMM profile prediction.   
-  *Eddy SR, Accelerated Profile HMM Searches. PLOS Computational Biology 2011, 10.1371/journal.pcbi.1002195*
-
-
 ## Licence
 
 [MIT](https://github.com/Ebedthan/hkgfinder/blob/main/LICENSE).
 
 
 ## Author
```

### Comparing `hkgfinder-0.1.0/db/hkgfinder.hmm` & `hkgfinder-0.2.0/hkgfinder/hkgfinder.hmm`

 * *Files identical despite different names*

### Comparing `hkgfinder-0.1.0/pyproject.toml` & `hkgfinder-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hkgfinder"
-version = "0.1.0"
+version = "0.2.0"
 description = "find housekeeping genes in prokaryotic (meta)genomic data"
 authors = ["Anicet Ebou <anicet.ebou@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Ebedthan/hkgfinder"
 repository = "https://github.com/Ebedthan/hkgfinder"
 documentation = "https://github.com/Ebedthan/hkgfinder"
@@ -20,26 +20,28 @@
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: POSIX :: Linux",
             "Operating System :: Unix",
             "Topic :: Scientific/Engineering :: Bio-Informatics"
 ]
-include = ["db/*"]
+
+[options.package_data]
+hkgfinder = "*.hmm"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 bio = "^1.3.9"
 pyfastx = "^0.8.4"
 xphyle = "^4.4.2"
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^4.0.1"
-black = "^22.3.0"
+pyrodigal = "^2.1.0"
+pyhmmer = "^0.8.0"
 
 [tool.poetry.scripts]
 hkgfinder = "hkgfinder.hkgfinder:main"
 
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hkgfinder-0.1.0/setup.py` & `hkgfinder-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 packages = \
 ['hkgfinder']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bio>=1.3.9,<2.0.0', 'pyfastx>=0.8.4,<0.9.0', 'xphyle>=4.4.2,<5.0.0']
+['bio>=1.3.9,<2.0.0',
+ 'pyfastx>=0.8.4,<0.9.0',
+ 'pyhmmer>=0.8.0,<0.9.0',
+ 'pyrodigal>=2.1.0,<3.0.0',
+ 'xphyle>=4.4.2,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['hkgfinder = hkgfinder.hkgfinder:main']}
 
 setup_kwargs = {
     'name': 'hkgfinder',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'find housekeeping genes in prokaryotic (meta)genomic data',
-    'long_description': "# hkgfinder\n\n[![PyPI](https://img.shields.io/pypi/v/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Wheel](https://img.shields.io/pypi/wheel/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Language](https://img.shields.io/pypi/implementation/hkgfinder)](https://pypi.org/project/hkgfinder)\n[![Pyver](https://img.shields.io/pypi/pyversions/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Downloads](https://img.shields.io/pypi/dm/hkgfinder)](https://pypi.org/project/hkgfinder)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://www.gnu.org/licenses/MIT)\n\n\n## Find housekeeping genes in prokaryotic (meta)genomes\n\n### Introduction\nhkgfinder is a fast and accurate housekeeping gene finder and classifier. Hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.\n\n### How hkgfinder works\n![](img/hkgfinder.png)\n\n### Installation\n\nYou will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.\n\n\n#### Install from Pip\n\n```bash\npip install hkgfinder\n```\n\n\n#### Install from source\n\n```bash\n# Download hkgfinder development version\ngit clone https://github.com/Ebedthan/hkgfinder.git hkgfinder\n\n# Navigate to directory\ncd hkgfinder\n\n# Install with poetry: see https://python-poetry.org\npoetry install --no-dev\n\n# Enter the Python virtual environment with\npoetry shell\n\n# Test hkgfinder is correctly installed\nhkgfinder -h\n```\n\nIf you do not want to go into the virtual environment just do:\n\n```bash\npoetry run hkgfinder -h\n```\n\n## Test\n\n* Type `hkgfinder -h` and it should output something like:\n\n```\nusage: hkgfinder [options] [<FILE>]\n\noptional arguments:\n  -o [FILE]      output result to FILE [stdout]\n  -g             activate genome mode [false]\n  -m             activate metagenome mode [false]\n  --faa FILE     output matched proteins sequences to FILE\n  --fna FILE     output matched DNA sequences to FILE\n  -t INT         number of threads [1]\n  -q             decrease program verbosity\n  -v, --version  show program's version number and exit\n  -h, --help     show this help message and exit\n```\n\n\n## Invoking hkgfinder\n\n```\nhkgfinder --faa housekeeping.faa --fna housekeeping.fna file.fa.gz\n```\n\n* hkgfinder supports gzip, lzma, bz2 and zstd compressed files.\n  \n## Bugs\n\nSubmit problems or requests to the [Issue Tracker](https://github.com/Ebedthan/hkgfinder/issues).\n\n\n## Dependencies\n\n### Mandatory\n\n* [**Prodigal**](https://github.com/sib-swiss/pftools3)  \n  Used for protein-coding gene prediction.    \n  *Hyatt, D., Chen, GL., LoCascio, P.F. et al. Prodigal: prokaryotic gene recognition and translation initiation site identification. BMC Bioinformatics 11, 119 (2010). https://doi.org/10.1186/1471-2105-11-119*\n\n* [**HMMER 3**](https://hmmer.org)  \n  Used for HMM profile prediction.   \n  *Eddy SR, Accelerated Profile HMM Searches. PLOS Computational Biology 2011, 10.1371/journal.pcbi.1002195*\n\n\n## Licence\n\n[MIT](https://github.com/Ebedthan/hkgfinder/blob/main/LICENSE).\n\n\n## Author\n\n* [Anicet Ebou](https://orcid.org/0000-0003-4005-177X)\n\n",
+    'long_description': "# hkgfinder\n\n[![PyPI](https://img.shields.io/pypi/v/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Wheel](https://img.shields.io/pypi/wheel/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Language](https://img.shields.io/pypi/implementation/hkgfinder)](https://pypi.org/project/hkgfinder)\n[![Pyver](https://img.shields.io/pypi/pyversions/hkgfinder.svg)](https://pypi.org/project/hkgfinder)\n[![Downloads](https://img.shields.io/pypi/dm/hkgfinder)](https://pypi.org/project/hkgfinder)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://www.gnu.org/licenses/MIT)\n\n\n## Find housekeeping genes in prokaryotic (meta)genomes\n\n### Introduction\nhkgfinder is a fast and accurate housekeeping gene finder and classifier. hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.\n\n\n### How hkgfinder works\n![](img/hkgfinder.png)\n\n### Installation\n\n~~You will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.~~\n\n**hkgfinder since v0.2 is without external dependencies.**\n\n\n```bash\npip install hkgfinder\n```\n\n## Test\n\n* Type `hkgfinder -h` and it should output something like:\n\n```\nusage: hkgfinder [options] [<FILE>]\n\noptions:\n  -o [FILE]      output result to FILE [stdout]\n  -g             activate genome mode [false]\n  -m             activate metagenome mode [false]\n  --faa FILE     output matched protein sequences to FILE [false]\n  --fna FILE     output matched DNA sequences to FILE [false]\n  -s             output sequences in file by gene [false]\n  -t INT         number of threads [1]\n  -q             decrease program verbosity\n  -d             enable debug mode\n  -v, --version  show program's version number and exit\n  -h, --help     show this help message and exit\n```\n\n\n## Invoking hkgfinder\n\n```\nhkgfinder --faa housekeeping.faa --fna housekeeping.fna file.fa.gz\n```\n\n* hkgfinder supports gzip, lzma, bz2 and zstd compressed files.\n  \n## Bugs\n\nSubmit problems or requests to the [Issue Tracker](https://github.com/Ebedthan/hkgfinder/issues).\n\n\n## Licence\n\n[MIT](https://github.com/Ebedthan/hkgfinder/blob/main/LICENSE).\n\n\n## Author\n\n* [Anicet Ebou](https://orcid.org/0000-0003-4005-177X)\n\n",
     'author': 'Anicet Ebou',
     'author_email': 'anicet.ebou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ebedthan/hkgfinder',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `hkgfinder-0.1.0/PKG-INFO` & `hkgfinder-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkgfinder
-Version: 0.1.0
+Version: 0.2.0
 Summary: find housekeeping genes in prokaryotic (meta)genomic data
 Home-page: https://github.com/Ebedthan/hkgfinder
 License: MIT
 Keywords: bioinformatics
 Author: Anicet Ebou
 Author-email: anicet.ebou@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: bio (>=1.3.9,<2.0.0)
 Requires-Dist: pyfastx (>=0.8.4,<0.9.0)
+Requires-Dist: pyhmmer (>=0.8.0,<0.9.0)
+Requires-Dist: pyrodigal (>=2.1.0,<3.0.0)
 Requires-Dist: xphyle (>=4.4.2,<5.0.0)
 Project-URL: Documentation, https://github.com/Ebedthan/hkgfinder
 Project-URL: Repository, https://github.com/Ebedthan/hkgfinder
 Description-Content-Type: text/markdown
 
 # hkgfinder
 
@@ -43,71 +45,48 @@
 [![Downloads](https://img.shields.io/pypi/dm/hkgfinder)](https://pypi.org/project/hkgfinder)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://www.gnu.org/licenses/MIT)
 
 
 ## Find housekeeping genes in prokaryotic (meta)genomes
 
 ### Introduction
-hkgfinder is a fast and accurate housekeeping gene finder and classifier. Hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.
+hkgfinder is a fast and accurate housekeeping gene finder and classifier. hkgfinder can run on raw sequences, genomes and metagenomes. The novel value of this method lies is in its ability to directly predict and classify gene sequences into housekeeping gene families at a high specificity and sensitivity, while being also faster than genome and metagenome annotator on genome and metagenome data.
+
 
 ### How hkgfinder works
 ![](img/hkgfinder.png)
 
 ### Installation
 
-You will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.
+~~You will have first to install [Prodigal](https://github.com/hyattpd/Prodigal) and [HMMER 3](https://hmmer.org) to be able to run hkgfinder.~~
 
+**hkgfinder since v0.2 is without external dependencies.**
 
-#### Install from Pip
 
 ```bash
 pip install hkgfinder
 ```
 
-
-#### Install from source
-
-```bash
-# Download hkgfinder development version
-git clone https://github.com/Ebedthan/hkgfinder.git hkgfinder
-
-# Navigate to directory
-cd hkgfinder
-
-# Install with poetry: see https://python-poetry.org
-poetry install --no-dev
-
-# Enter the Python virtual environment with
-poetry shell
-
-# Test hkgfinder is correctly installed
-hkgfinder -h
-```
-
-If you do not want to go into the virtual environment just do:
-
-```bash
-poetry run hkgfinder -h
-```
-
 ## Test
 
 * Type `hkgfinder -h` and it should output something like:
 
 ```
 usage: hkgfinder [options] [<FILE>]
 
-optional arguments:
+options:
   -o [FILE]      output result to FILE [stdout]
   -g             activate genome mode [false]
   -m             activate metagenome mode [false]
-  --faa FILE     output matched proteins sequences to FILE
-  --fna FILE     output matched DNA sequences to FILE
+  --faa FILE     output matched protein sequences to FILE [false]
+  --fna FILE     output matched DNA sequences to FILE [false]
+  -s             output sequences in file by gene [false]
   -t INT         number of threads [1]
   -q             decrease program verbosity
+  -d             enable debug mode
   -v, --version  show program's version number and exit
   -h, --help     show this help message and exit
 ```
 
 
 ## Invoking hkgfinder
 
@@ -118,27 +97,14 @@
 * hkgfinder supports gzip, lzma, bz2 and zstd compressed files.
   
 ## Bugs
 
 Submit problems or requests to the [Issue Tracker](https://github.com/Ebedthan/hkgfinder/issues).
 
 
-## Dependencies
-
-### Mandatory
-
-* [**Prodigal**](https://github.com/sib-swiss/pftools3)  
-  Used for protein-coding gene prediction.    
-  *Hyatt, D., Chen, GL., LoCascio, P.F. et al. Prodigal: prokaryotic gene recognition and translation initiation site identification. BMC Bioinformatics 11, 119 (2010). https://doi.org/10.1186/1471-2105-11-119*
-
-* [**HMMER 3**](https://hmmer.org)  
-  Used for HMM profile prediction.   
-  *Eddy SR, Accelerated Profile HMM Searches. PLOS Computational Biology 2011, 10.1371/journal.pcbi.1002195*
-
-
 ## Licence
 
 [MIT](https://github.com/Ebedthan/hkgfinder/blob/main/LICENSE).
 
 
 ## Author
```

