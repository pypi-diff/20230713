# Comparing `tmp/biotext-2.4.1.3-py3.8.egg` & `tmp/biotext-3.0.0.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,15 +1,13 @@
-Zip file size: 13420 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat     7821 b- defN 22-Nov-09 01:32 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      350 b- defN 22-Nov-09 01:32 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 22-Nov-09 01:32 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 22-Nov-09 01:32 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       80 b- defN 22-Nov-09 01:32 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        8 b- defN 22-Nov-09 01:32 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      331 b- defN 22-Nov-09 01:32 biotext/__init__.pyc
--rw-rw-rw-  2.0 fat     5882 b- defN 22-Nov-09 01:32 biotext/aminocode.pyc
--rw-rw-rw-  2.0 fat     5065 b- defN 22-Nov-09 01:32 biotext/dnabits.pyc
--rw-rw-rw-  2.0 fat     7204 b- defN 22-Nov-09 01:32 biotext/fastatools.pyc
--rw-rw-rw-  2.0 fat     1853 b- defN 22-Nov-09 01:32 biotext/pubmedtools.pyc
--rw-rw-rw-  2.0 fat     1039 b- defN 22-Nov-09 01:32 biotext/treetools.pyc
--rw-rw-rw-  2.0 fat      736 b- defN 22-Nov-09 01:32 biotext/utilities.pyc
-13 files, 30372 bytes uncompressed, 11856 bytes compressed:  61.0%
+Zip file size: 18771 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat    18676 b- defN 23-Jul-13 02:54 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      308 b- defN 23-Jul-13 02:54 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-13 02:54 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-13 02:52 EGG-INFO/not-zip-safe
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-13 02:54 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-13 02:54 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      705 b- defN 23-Jul-13 02:54 biotext/__init__.pyc
+-rw-rw-rw-  2.0 fat     6336 b- defN 23-Jul-13 02:54 biotext/aminocode.pyc
+-rw-rw-rw-  2.0 fat     5455 b- defN 23-Jul-13 02:54 biotext/dnabits.pyc
+-rw-rw-rw-  2.0 fat    10562 b- defN 23-Jul-13 02:54 biotext/fastatools.pyc
+-rw-rw-rw-  2.0 fat    10995 b- defN 23-Jul-13 02:54 biotext/wordembtools.pyc
+11 files, 53098 bytes uncompressed, 17441 bytes compressed:  67.2%
```

## zipnote «TEMP»/diffoscope_ukdwcfg8_/tmpf5ojr1_j_.zip

```diff
@@ -24,17 +24,11 @@
 
 Filename: biotext/dnabits.pyc
 Comment: 
 
 Filename: biotext/fastatools.pyc
 Comment: 
 
-Filename: biotext/pubmedtools.pyc
-Comment: 
-
-Filename: biotext/treetools.pyc
-Comment: 
-
-Filename: biotext/utilities.pyc
+Filename: biotext/wordembtools.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,138 +1,692 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: biotext
-Version: 2.4.1.3
-Summary: The biotext library offers resources to support text mining strategy using bioinformatics tool
+Version: 3.0.0.0
+Summary: The biotext library offers resources for natural language processing based on bioinformatics tools
 Home-page: https://github.com/diogomachado-bioinfo/biotext
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
-License: UNKNOWN
-Description: Biotext
-        =======
-        The biotext library offers resources to support text mining strategy using bioinformatics tool.
-        
-        Installation
-        ------------
-        To install aminocode through `pip`::
-        
-              pip install biotext
-        
-        
-        Tested Platforms
-        ----------------
-        - Python:
-        
-         - 3.7.4
-        
-        - Windows (64bits):
-        
-         - 10
-        
-        - Ubuntu (64bits)
-        
-         - 18.04.1 LTS
-        
-        Required external libraries
-        ---------------------------
-        - numpy
-        - pandas
-        - scipy
-        - scikit-learn
-        - matplotlib
-        - unidecode
-        - biopython
-        - sweep
-        
-        Functions
-        ---------------
-        .. csv-table::
-           :header: "Function Name", "Description", "Input", "Output"
-           :stub-columns: 1
-        
-           "biotext.aminocode.encode_string", "Encodes a string with AMINOcode.","input_string \: string:
-            Natural language text string to be encoded.
-           detail \: string:
-            Set details in coding. 'd' for details in digits; 'p' for details on the punctuation; 'dp' or 'pd' for both.", "encoded_string \: string
-            Encoded text."
-           "biotext.aminocode.decode_string", "Decodes a string with AMINOcode reverse.", "input_string \: string:
-            Text string encoded with AMINOcode.
-           detail \: string:
-            Set details in coding. 'd' for details in digits; 'p' for details on the punctuation; 'dp' or 'pd' for both.", "decoded_string \: string
-            Decoded text."
-           "biotext.aminocode.encode_list ", "Encodes all strings in a list with AMINOcode.", "string_list \: list
-            List of string to be encoded.
-           detail \: string
-             Set details in coding. 'd' for details in digits; 'p' for details on the punctuation; 'dp' or 'pd' for both.
-           verbose \: bool
-            If True displays progress.", "encoded_list \: list
-            List with all encoded text in string format."
-           "biotext.aminocode.decode_list", "Decodes all strings in a list with reverse AMINOcode.", "string_list \: list
-            List of string encoded with aminocode.
-           detail \: string
-            Set details in coding. 'd' for details in digits; 'p' for details on the punctuation; 'dp' or 'pd' for both.
-           verbose \: bool
-            If True displays progress.", "decoded_list \: list of string
-             List with all decoded text."
-           "biotext.dnabits.encode_string", "Encodes a string with DNAbits.","input_string \: string:
-            Natural language text string to be encoded.", "encoded_string \: string
-            Encoded text."
-           "biotext.dnabits.decode_string", "Decodes a string with DNAbits reverse.", "input_string \: string:
-            Text string encoded with AMINOcode.", "decoded_string \: string
-            Decoded text."
-           "biotext.dnabits.encode_list ", "Encodes all strings in a list with DNAbits.", "string_list \: list
-            List of string to be encoded.
-           verbose \: bool
-            If True displays progress.", "encoded_list \: list
-            List with all encoded text in string format."
-           "biotext.dnabits.decode_list", "Decodes all strings in a list with reverse DNAbits.", "string_list \: list
-            List of string encoded with aminocode.
-           verbose \: bool
-            If True displays progress.", "decoded_list \: list of string
-             List with all decoded text."
-           "create_seqrecord_list", "Creates a list of SeqRecord*SeqRecord* from a string list.", "seq_list \: list of string
-            List of biological sequences in string format.
-           header \: list of string
-            List of headers in string format, if set to 'None' the headers will be automatically defined with numbers in increasing order.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord*."
-           "biotext.fastatools.import_fasta", "Uses biopython to import a FASTA file.", "input_file_name \: string (valid file name)
-            Input fasta file name.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord* imported from file."
-           "biotext.fastatools.export_fasta", "Creates a file using a SeqRecord*SeqRecord* list.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord*.
-           output_file_name \: string
-            Output fasta file name.", "A file is saved with the defined name."
-           "biotext.fastatools.get_header", "Get the header from all items in a list of SeqRecord*SeqRecord*.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord*.", "header_list \: list of string
-            List of all headers extracted from input."
-           "biotext.fastatools.get_seq", "Get the sequences from all items in a list of SeqRecord*SeqRecord*.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord*.", "seq_list \: list of string
-            List of all sequences extracted from input."
-           "biotext.fastatools.remove_pattern", "Removes patterns from a SeqRecord* range based on regular expression.", "seq_list \: list of SeqRecord*
-            List of SeqRecord*.
-           rex \: string
-            regular expression.", "seq_list \: list of SeqRecord*
-            List of SeqRecord* with removal applied."
-           "biotext.fastatools.run_clustalo", "Uses the Clustal Omega to align the strings in a FASTA file.", "input_file_name \: string (valid file name)
-            Input fasta file name.", "alignment \: MultipleSeqAlignment**
-            Alignment result."
-           "biotext.fastatools.get_consensus", "Applies clustalo and obtain alignment consensus.", "seqrecord_list \: list of SeqRecord*
-            List of SeqRecord*.", "consensus \: string
-            Alignment consensus.
-           alignment \: list of string
-            List of sequences with alignment gaps."
-           "biotext.fastatools.fasta_to_mat", "Performs a vectorization of a list of SeqRecord* using the SWeeP.", "seq_list \: list of string
-            List of strings in FASTA format.", "mat \: ndarray***
-            Matrix with the generated vectors."
-           "biotext.treetools.mat_to_tree", "Creates a dendrogram in newick format from a matrix.", "mat \: ndarray***
-            Matrix.
-           ids \: list of string
-            List with line identifiers in mat.
-           method \: string
-            Method to create the dendrogram. Available options are 'complete', scipy library implementation, and 'nj' (neighbor joining), skbio library implementation. The default is the 'complete' method.", "tree \: string
-            tree: dendrogram in newick format."
-        
-        \*Bio.SeqRecord.SeqRecord: Biopython object to store biological sequences and its information, as described in <https://biopython.org/docs/1.76/api/Bio.SeqRecord.html>.
-        
-        \*\*Bio.Align.MultipleSeqAlignment: Biopython object to store biological multiple sequence alignment, as described in <https://biopython.org/docs/1.76/api/Bio.Align.html>.
-        
-        \*\*\*numpy.ndarray: Numpy object to represent array, as described in <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>.
-Platform: UNKNOWN
+License: BSD-3-Clause
+Description-Content-Type: text/markdown
+
+# Biotext
+
+---
+
+The biotext library offers resources for natural language processing based on
+bioinformatics tools. With biotext, it is possible to use native bioinformatics
+methods to create text mining strategies. The biotext process starts by
+encoding natural language texts in a format based on biological sequences,
+which are usable in alignment and vectorization approaches.
+
+---
+
+---
+
+# Features
+
+---
+
+## AMINOcode (biotext.aminocode)
+- `biotext.aminocode.encode_string`: Encodes a string using AMINOcode.
+- `biotext.aminocode.encode_list`: Encodes all strings in a list using
+                                   AMINOcode.
+- `biotext.aminocode.decode_string`: Decodes a string encoded with AMINOcode.
+- `biotext.aminocode.decode_list`: Decodes all strings in a list encoded with
+                                   AMINOcode.
+
+## DNAbits (biotext.dnabits)
+- `biotext.dnabits.encode_string`: Encodes a string using DNAbits.
+- `biotext.dnabits.decode_string`: Decodes a string encoded with DNAbits.
+- `biotext.dnabits.encode_list`: Encodes all strings in a list using DNAbits.
+- `biotext.dnabits.decode_list`: Decodes all strings in a list encoded with
+                                 DNAbits.
+
+## FASTA Tools (biotext.fastatools)
+- `biotext.fastatools.import_fasta`: Imports a FASTA file.
+- `biotext.fastatools.export_fasta`: Creates a FASTA file from a list of
+                                     sequences.
+- `biotext.fastatools.create_seqrecord_list`: Creates a list of SeqRecord
+                                              objects from a list of sequences.
+- `biotext.fastatools.run_clustalo`: Performs multiple sequence alignment using
+                                     Clustal Omega.
+- `biotext.fastatools.get_consensus`: Retrieves the consensus sequence from a
+                                      set of sequences.
+- `biotext.fastatools.get_header`: Retrieves the headers from a list of
+                                   SeqRecord objects.
+- `biotext.fastatools.get_seq`: Retrieves the sequences from a list of
+                                SeqRecord objects.
+- `biotext.fastatools.fasta_to_mat`: Converts FASTA sequences to a vectorial
+                                     representation.
+
+## Word Embedding Tools (biotext.wordembtools)
+- `biotext.wordembtools.WordEmbedding`: A class for generating word embeddings
+                                        from a collection of texts.
+
+---
+
+---
+
+# Installation
+
+You can install BioText using pip:
+
+    pip install biotext
+---
+
+---
+
+# Functions
+
+---
+
+## AMINOcode (aminocode)
+
+---
+### `biotext.aminocode.encode_string`
+Encodes a string with AMINOcode.
+
+**Parameters**
+
+- `input_string` : str
+    - Natural language text string to be encoded.
+- `detail` : str
+    - Set details in coding.
+    - 'd' for details in digits; 'p' for details on the punctuation;
+    'dp' or 'pd' for both.
+    - Default is 'dp'.
+    
+**Returns**
+
+- `encoded_string` : string
+  - Encoded text.
+    
+**Example**
+
+Encode a string.
+```python
+import biotext as bt
+input_string = "Hello world!"
+encoded_string = bt.aminocode.encode_string(input_string,'dp')
+print(encoded_string)
+# HYELLYQYSYWYQRLDYPW
+```
+---
+### `biotext.aminocode.encode_list`
+Encodes all strings in a list with AMINOcode.
+
+**Parameters**
+
+- `string_list` : list
+    - List of string to be encoded.
+- `detail` : str
+    - Set details in coding.'d' for details in digits; 'p' for details
+    on the punctuation; 'dp' or 'pd' for both.
+    - Default is 'dp'.
+- `verbose`  : bool
+    - If True displays progress.
+
+**Returns**
+
+- `encoded_list` : list
+    - List with all encoded text in string format.
+    
+**Example**
+
+Encode the strings in a list and view the result of the first item.
+```python
+import biotext as bt
+string_list = ['Hello','world','!']
+encoded_list = bt.aminocode.encode_list(string_list,detail='dp')
+print(encoded_list)
+# ['HYELLYQ', 'YWYQRLD', 'YPW']
+```
+---
+### `biotext.aminocode.decode_string`
+Decodes a string with AMINOcode reverse.
+
+**Parameters**
+
+- `input_string` : str
+    - Text string encoded with AMINOcode.
+- `detail` : str
+    - Set details in coding. 'd' for details in digits; 'p' for details on 
+    the punctuation; 'dp' or 'pd' for both.
+    - Default is 'dp'.
+
+**Returns**
+
+- `decoded_string` : str
+    - Decoded text.
+    
+**Example**
+
+Deconde a string.
+```python
+import biotext as bt
+encoded_string = "HYELLYQYSYWYQRLDYPW"
+decoded_string = bt.aminocode.decode_string(encoded_string,'dp')
+print(decoded_string)
+# hello world!
+```
+---
+### `biotext.aminocode.decode_list`
+Decodes all strings in a list with reverse AMINOcode.	
+
+**Parameters**
+
+- `string_list` : list
+    - List of string encoded with aminocode.
+- `detail` : str
+    - Set details in coding. 'd' for details in digits; 'p' for details on 
+    the punctuation; 'dp' or 'pd' for both.
+    - Default is 'dp'.
+- `verbose`  : bool
+    - If True displays progress.
+
+**Returns**
+
+- `decoded_list` : list of string
+    - List with all decoded text.
+    
+**Example**
+
+Descode the strings in a list and view the result with a loop.
+```python
+import biotext as bt
+encoded_list = ['HYELLYQ', 'YWYQRLD', 'YPW']
+decoded_list = bt.aminocode.decode_list(encoded_list,detail='dp')
+print(decoded_list)
+# ['hello', 'world', '!']
+```
+---
+
+## DNAbits (dnabits)
+
+---
+### `biotext.dnabits.encode_string`
+Encodes a string with DNAbits.
+
+**Parameters**
+
+- `input_string` : string
+    - Natural language text string to be encoded.
+    
+**Returns**
+
+- `encoded_string` : string
+    - Encoded text.
+    
+**Example**
+
+Encode a string.
+```python
+import biotext as bt
+input_string = "Hello world!"
+encoded_string = bt.dnabits.encode_string(input_string)
+print(encoded_string)
+# AGACCCGCATGCATGCTTGCAAGATCTCTTGCGATCATGCACGCCAGA
+```
+---
+### `biotext.dnabits.decode_string`
+Decodes a string with DNAbits reverse.	
+
+**Parameters**
+
+- `input_string` : string
+    - Text string encoded with DNAbits.
+
+**Returns**
+
+- `decoded_string` : string
+    - Decoded text.
+    
+**Example**
+
+Decode a string.
+```python
+import biotext as bt
+encoded_string = "AGACCCGCATGCATGCTTGCAAGATCTCTTGCGATCATGCACGCCAGA"
+decoded_string = bt.dnabits.decode_string(encoded_string)
+print(decoded_string)
+# Hello world!
+```
+---
+### `biotext.dnabits.encode_list`
+Encodes all strings in a list with DNAbits.	
+
+**Parameters**
+
+- `string_list` : list
+    - List of string to be encoded.
+- `verbose`  : bool
+    - If True displays progress.
+
+**Returns**
+
+- `encoded_list` : list
+    - List with all encoded text in string format.
+    
+**Example**
+
+Encode the strings in a list and view the result of the first item.
+```python
+import biotext as bt
+string_list = ['Hello','world','!']
+encoded_list = bt.dnabits.encode_list(string_list)
+print(encoded_list)
+# ['AGACCCGCATGCATGCTTGC', 'TCTCTTGCGATCATGCACGC', 'CAGA']
+```
+---
+### `biotext.dnabits.decode_list`
+Decodes all strings in a list with reverse DNAbits.	
+
+**Parameters**
+
+- `string_list` : list
+    - List of string encoded with DNAbits.
+`verbose`  : bool
+    - If True displays progress.
+
+**Returns**
+
+`decoded_list` : list of string
+    - List with all decoded text.
+    
+**Example**
+
+Decode the strings in a list and view the result with a loop.
+```python
+import biotext as bt
+encoded_list = ['AGACCCGCATGCATGCTTGC', 'TCTCTTGCGATCATGCACGC', 'CAGA']
+decoded_list = bt.dnabits.decode_list(encoded_list)
+print(decoded_list)
+# ['Hello', 'world', '!']
+```
+---
+
+## FASTA Tools (fastatools)
+
+---
+### `biotext.fastatools.import_fasta`
+Uses biopython to import a FASTA file.
+
+**Parameters**
+
+- `input_file_name` : string (valid file name)
+    - Input fasta file name.
+
+**Returns**
+
+- `seqrecord_list` : list of SeqRecord
+    - List of SeqRecord imported from file.
+    
+**Example**
+
+Import a FASTA file named 'sequences.fasta'.
+```python
+import biotext as bt
+input_file = 'sequences.fasta'
+fasta = bt.fastatools.import_fasta(input_file)
+# print first sequence in input file
+print(fasta[0])
+# ID: 1
+# Name: 1
+# Description: 1
+# Number of features: 0
+# Seq('HYELLYQYSYWYQRLD')
+```
+---
+### `biotext.fastatools.export_fasta`
+Create a file using a SeqRecord (Biopython object) list.
+
+**Parameters**
+
+- `output_file_name` : string
+    - Output fasta file name.
+- `seqrecord_list` : list of SeqRecord
+    - List of SeqRecord.
+    
+**Example**
+
+Export a SeqRecord list as FASTA file named 'sequences.fasta'.
+```python
+import biotext as bt
+seq_list = ['ACTG','GTCA']
+seqrecord_list = bt.fastatools.create_seqrecord_list(seq_list)
+bt.fastatools.export_fasta(seqrecord_list,'sequences.fasta')
+```
+---
+### `biotext.fastatools.create_seqrecord_list`
+Create a list of SeqRecord (Biopython object) with a string list.
+
+**Parameters**
+
+- `seq_list` : list of string
+    - List of biological sequences in string format.
+- `header` : list of string
+    - List of headers in string format, if set to 'None' the headers will 
+    be automatically defined with numbers in increasing order.
+
+**Returns**
+
+- `seqrecord_list` : list of SeqRecord
+    - List of SeqRecord.
+    
+**Example**
+
+Decode a string.
+```python
+import biotext as bt
+seq_list = ['ACTG','GTCA']
+seqrecord_list = bt.fastatools.create_seqrecord_list(seq_list)
+for i in seqrecord_list:
+    print (i)
+# ID: 1
+# Name: <unknown name>
+# Description: 1
+# Number of features: 0
+# Seq('ACTG')
+# ID: 2
+# Name: <unknown name>
+# Description: 2
+# Number of features: 0
+# Seq('GTCA')
+```
+---
+### `biotext.fastatools.run_clustalo`
+Run Clustal Omega multiple sequence alignment on the input file.
+
+**Parameters**
+
+- `input_file_name` : str
+    - Path to the input file containing the sequences to align.
+- `args` : str, optional
+    - Additional arguments to pass to Clustal Omega. Defaults to an empty string.
+
+**Returns**
+
+- `align` : Bio.Align.MultipleSeqAlignment
+    - Aligned sequences in the Clustal format.
+
+**Example**
+
+Perform multiple sequence alignment using Clustal Omega:
+```python
+import biotext as bt
+input_file = 'sequences.fasta'
+alignment = bt.fastatools.run_clustalo(input_file)
+print(alignment)
+# Alignment with 3 rows and 16 columns
+# HYELLYQYSYWYQRLD 1
+# HYELLYQ--------- 2
+# ---------YWYQRLD 3
+```
+---
+### biotext.fastatools.get_consensus
+Get the consensus sequence from a list of sequences.
+
+**Parameters**
+
+- `seq_list` : list
+    - List of sequences in SeqRecord object format or as strings.
+- `preserve_gap` : bool, optional
+    - If True, the consensus sequence may contain gaps ("-") based
+	on the majority characters and the gaps present in the aligned sequences. 
+    - If False, the consensus sequence is determined without gaps
+	by considering only the majority characters.
+
+**Returns**
+
+- `consensus` : str
+    - Consensus sequence based on the majority characters, with or without
+	gaps ("-") depending on the `preserve_gap` parameter.
+- `align` : list
+    - List of aligned sequences.
+
+**Example**
+
+Calculate the consensus sequence from a list of sequences:
+```python
+import biotext as bt
+seq_list = ['ACTG', 'ACTC', 'ACCC', 'ACC']
+consensus, align = bt.fastatools.get_consensus(seq_list)
+print('Consensus: ', consensus)
+print('Alignment: ', align)
+# Consensus:  ACCC
+# Alignment:  ['ACTG', 'ACTC', 'ACCC', 'ACC-']
+```
+---
+### `biotext.fastatools.get_header`
+Get the header from all items in a list of SeqRecord (Biopython object).
+
+**Parameters**
+
+- `seqrecord_list` : list of SeqRecord
+    - List of SeqRecord.
+
+**Returns**
+
+- `header_list` : list of string
+    - List of all headers extracted from input.
+    
+**Example**
+
+Create seqrecord_list, extract headers and print it.
+```python
+import biotext as bt
+seq_list = ['ACTG','GTCA']
+seqrecord_list = bt.fastatools.create_seqrecord_list(seq_list)
+extracted_header_list = bt.fastatools.get_header(seqrecord_list)
+print(extracted_header_list)
+# ['1', '2']
+```
+---
+### `biotext.fastatools.get_seq`
+Get the sequences from all items in a list of SeqRecord (Biopython object).
+
+**Parameters**
+
+- `seqrecord_list` : list of SeqRecord
+    - List of SeqRecord.
+
+**Returns**
+
+- `seq_list` : list of string
+    - List of all sequences extracted from input.
+    
+**Example**
+
+Create seqrecord_list, extract sequences and print it.
+```python
+import biotext as bt
+seq_list = ['ACTG','GTCA']
+seqrecord_list = bt.fastatools.create_seqrecord_list(seq_list)
+extracted_seq_list = bt.fastatools.get_seq(seqrecord_list)
+print(extracted_seq_list)
+# ['ACTG', 'GTCA']
+```
+---
+### `biotext.fastatools.fasta_to_mat`
+Convert FASTA sequences to a matrix representation using SWeeP method.
+
+**Parameters**
+
+- `fasta` : list
+    - List of sequences in SeqRecord object format or as strings.
+- `mask` : list, optional
+    - A list specifying the mask values. Defaults to [2, 1, 2].
+- `**kwargs` : dict, optional
+    - Additional keyword arguments to pass to the `fas2sweep` function.
+
+**Returns**
+
+- `mat` : numpy.ndarray or scipy.sparse.lil_matrix
+    - Matrix representation of the sequences.
+
+**Example**
+
+Convert FASTA sequences to a matrix representation:
+```python
+import biotext as bt
+seq_list = ['HYELLYQYSYWYQRLD', 'HYELLYQ', 'YWYQRLD']
+matrix = bt.fastatools.fasta_to_mat(seq_list)
+print(matrix.shape)
+# (3, 600)
+```
+---
+
+---
+
+## Word Embedding Tools (wordembtools)
+
+---
+### `wordembtools`
+
+A class for generating word embeddings from a collection of texts.
+
+**Parameters**
+
+- `data_set` : list or pandas.Series
+    - The collection of texts to generate embeddings.
+- `word_set` : list, optional
+    - A pre-defined set of words to use for the embedding. Defaults to None.
+- `remove_stopwords` : bool, optional
+    - Whether to remove stop words from the texts. Defaults to False.
+- `stopwords_list` : list, optional
+    - Custom list of stop words to remove from the texts. Defaults to None.
+- `min_occ_to_use` : int, optional
+    - The minimum number of occurrences of a word in the collection of texts
+    to include it in the embedding. Defaults to 100.
+- `max_words` : int, optional
+    - The maximum number of words to include in the word set. Defaults to
+    10,000.
+- `word_tokenizer_fun` : function, optional
+    - Custom function for tokenizing words in each text. Defaults to None.
+- `sweep_projection_mat` : numpy.ndarray, optional
+    - The projection matrix for SWeeP vectorization. Defaults to None.
+- `sweep_mask` : list, optional
+    - The mask to apply during SWeeP vectorization. Defaults to [2, 1, 2].
+- `sweep_dtype` : dtype, optional
+    - The data type for SWeeP vectorization. Defaults to None.
+- `sweep_composition` : str, optional
+    - The composition mode for SWeeP vectorization. Defaults to 'binary'.
+- `preserve_data_set_splited` : bool, optional
+    - Whether to preserve the split data set object. Defaults to False.
+- `preserve_data_set_sweeped` : bool, optional
+    - Whether to preserve the swept data set object. Defaults to False.
+- `n_jobs` : int, optional
+    - The number of jobs to use for parallelization. Defaults to 1.
+- `chunk_size` : int, optional
+    - The size of each chunk for parallelization. Defaults to 1000.
+- `sweep_n_jobs` : int, optional
+    - The number of jobs to use for SWeeP vectorization. Defaults to None.
+    - If None, it receives the value of n_jobs.
+- `sweep_chunk_size` : int, optional
+    - The size of each chunk for SWeeP vectorization. Defaults to None.
+    - If None, it receives the value of chunk_size.
+- `verbose` : bool, optional
+    - Whether to print progress messages. Defaults to True.
+
+**Attributes**
+
+- `word_set` : list
+    - Set of unique words.
+- `word_embedding` : numpy.ndarray
+    - Word embeddings for the words in the word_set.
+- `elapsed_time` : list
+    - Elapsed time for each step of the process.
+
+**Example**
+```python
+import biotext as bt
+texts = []
+with open ('texts.txt', 'r') as file:
+    for line in file:
+        texts.append(line)
+we = bt.wordembtools.WordEmbedding(data_set = texts)
+embeddings = we.word_embedding
+```
+
+---
+
+---
+
+# Usage Examples
+
+## Encoding with AMINOcode
+```python
+import biotext as bt
+
+input_string = "Hello world!"
+encoded_string = bt.aminocode.encode_string(input_string, 'dp')
+print(encoded_string)
+# HYELLYQYSYWYQRLDYPW
+
+string_list = ['Hello', 'world', '!']
+encoded_list = bt.aminocode.encode_list(string_list, detail='dp')
+print(encoded_list)
+# ['HYELLYQ', 'YWYQRLD', 'YPW']
+```
+## Decoding with AMINOcode
+```python
+import biotext as bt
+
+encoded_string = "HYELLYQYSYWYQRLDYPW"
+decoded_string = bt.aminocode.decode_string(encoded_string, 'dp')
+print(decoded_string)
+# hello world!
+
+encoded_list = ['HYELLYQ', 'YWYQRLD', 'YPW']
+decoded_list = bt.aminocode.decode_list(encoded_list, detail='dp')
+print(decoded_list)
+# ['hello', 'world', '!']
+```
+## Importing and Exporting FASTA Files
+```python
+import biotext as bt
+
+input_file = 'sequences.fasta'
+fasta = bt.fastatools.import_fasta(input_file)
+print(fasta[0])  # Print the first sequence in the input file
+
+seq_list = ['ACTG', 'GTCA']
+seqrecord_list = bt.fastatools.create_seqrecord_list(seq_list)
+bt.fastatools.export_fasta(seqrecord_list, 'sequences.fasta')
+```
+## Generating Word Embeddings
+```python
+import biotext as bt
+
+texts = [
+    'This is the first text.',
+    'This is the second text.',
+    'And this is the third text.'
+]
+
+we = bt.wordembtools.WordEmbedding(data_set=texts)
+embeddings = we.word_embedding
+print(embeddings)
+```
+## Vectorizing FASTA Sequence
+```python
+import biotext as bt
+
+seq_list = ['HYELLYQ', 'YWYQRLD', 'YPW']
+matrix = bt.fastatools.fasta_to_mat(seq_list)
+print(matrix.shape)
+# (3, 600)
+```
+## Encoding Text with AMINOcode and Vectorizing
+```python
+import biotext as bt
+
+texts = [
+    'This is the first text.',
+    'This is the second text.',
+    'And this is the third text.'
+]
+encoded_texts = bt.aminocode.encode_list(texts, 'dp')
+matrix = bt.fastatools.fasta_to_mat([encoded_texts])
+print(matrix.shape)
+# (3, 600)
+```
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,15 +1,13 @@
-README.rst
+README.md
 setup.py
 biotext/__init__.py
 biotext/aminocode.py
 biotext/dnabits.py
 biotext/fastatools.py
-biotext/pubmedtools.py
-biotext/treetools.py
-biotext/utilities.py
+biotext/wordembtools.py
 biotext.egg-info/PKG-INFO
 biotext.egg-info/SOURCES.txt
 biotext.egg-info/dependency_links.txt
 biotext.egg-info/not-zip-safe
 biotext.egg-info/requires.txt
 biotext.egg-info/top_level.txt
```

## EGG-INFO/requires.txt

```diff
@@ -1,9 +1,7 @@
 numpy
 pandas
-unidecode
 biopython
+nltk
 sweep
 scipy
-scikit-learn
-matplotlib
-scikit-bio
+unidecode
```

## biotext/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Nov  8 02:12:00 2022 UTC, .py size: 193 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,21 +1,45 @@
-00000000: 550d 0d0a 0000 0000 f0ba 6963 c100 0000  U.........ic....
+00000000: 6f0d 0d0a 0000 0000 d885 af64 4102 0000  o..........dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
-00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c00 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c00 6d05 5a05 0100 6400 6406 6c00  d.l.m.Z...d.d.l.
-00000070: 6d06 5a06 0100 6407 5300 2908 e901 0000  m.Z...d.S.).....
-00000080: 0029 01da 0a66 6173 7461 746f 6f6c 7329  .)...fastatools)
-00000090: 01da 0974 7265 6574 6f6f 6c73 2901 da07  ...treetools)...
-000000a0: 646e 6162 6974 7329 01da 0961 6d69 6e6f  dnabits)...amino
-000000b0: 636f 6465 2901 da0b 7075 626d 6564 746f  code)...pubmedto
-000000c0: 6f6c 7329 01da 0975 7469 6c69 7469 6573  ols)...utilities
-000000d0: 4e29 07da 0072 0200 0000 7203 0000 0072  N)...r....r....r
-000000e0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-000000f0: 0000 00a9 0072 0900 0000 7209 0000 00fa  .....r....r.....
-00000100: 2d62 7569 6c64 5c62 6469 7374 2e77 696e  -build\bdist.win
-00000110: 2d61 6d64 3634 5c65 6767 5c62 696f 7465  -amd64\egg\biote
-00000120: 7874 5c5f 5f69 6e69 745f 5f2e 7079 da08  xt\__init__.py..
-00000130: 3c6d 6f64 756c 653e 0300 0000 730a 0000  <module>....s...
-00000140: 000c 010c 010c 010c 010c 01              ...........
+00000020: 0002 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c01 6d03 5a03 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
+00000050: 6d04 5a04 0100 6401 6405 6c01 6d05 5a05  m.Z...d.d.l.m.Z.
+00000060: 0100 6406 5300 2907 619f 0100 000a 5468  ..d.S.).a.....Th
+00000070: 6520 6269 6f74 6578 7420 6c69 6272 6172  e biotext librar
+00000080: 7920 6f66 6665 7273 2072 6573 6f75 7263  y offers resourc
+00000090: 6573 2066 6f72 206e 6174 7572 616c 206c  es for natural l
+000000a0: 616e 6775 6167 6520 7072 6f63 6573 7369  anguage processi
+000000b0: 6e67 2062 6173 6564 206f 6e0a 6269 6f69  ng based on.bioi
+000000c0: 6e66 6f72 6d61 7469 6373 2074 6f6f 6c73  nformatics tools
+000000d0: 2e20 5769 7468 2062 696f 7465 7874 2c20  . With biotext, 
+000000e0: 6974 2069 7320 706f 7373 6962 6c65 2074  it is possible t
+000000f0: 6f20 7573 6520 6e61 7469 7665 2062 696f  o use native bio
+00000100: 696e 666f 726d 6174 6963 730a 6d65 7468  informatics.meth
+00000110: 6f64 7320 746f 2063 7265 6174 6520 7465  ods to create te
+00000120: 7874 206d 696e 696e 6720 7374 7261 7465  xt mining strate
+00000130: 6769 6573 2e20 5468 6520 6269 6f74 6578  gies. The biotex
+00000140: 7420 7072 6f63 6573 7320 7374 6172 7473  t process starts
+00000150: 2062 790a 656e 636f 6469 6e67 206e 6174   by.encoding nat
+00000160: 7572 616c 206c 616e 6775 6167 6520 7465  ural language te
+00000170: 7874 7320 696e 2061 2066 6f72 6d61 7420  xts in a format 
+00000180: 6261 7365 6420 6f6e 2062 696f 6c6f 6769  based on biologi
+00000190: 6361 6c20 7365 7175 656e 6365 732c 0a77  cal sequences,.w
+000001a0: 6869 6368 2061 7265 2075 7361 626c 6520  hich are usable 
+000001b0: 696e 2061 6c69 676e 6d65 6e74 2061 6e64  in alignment and
+000001c0: 2076 6563 746f 7269 7a61 7469 6f6e 2061   vectorization a
+000001d0: 7070 726f 6163 6865 732e 0a0a 4175 7468  pproaches...Auth
+000001e0: 6f72 3a20 4469 6f67 6f20 6465 204a 2e20  or: Diogo de J. 
+000001f0: 532e 204d 6163 6861 646f 0a44 6174 653a  S. Machado.Date:
+00000200: 2031 332f 3037 2f32 3032 330a e901 0000   13/07/2023.....
+00000210: 0029 01da 0a66 6173 7461 746f 6f6c 7329  .)...fastatools)
+00000220: 01da 0764 6e61 6269 7473 2901 da09 616d  ...dnabits)...am
+00000230: 696e 6f63 6f64 6529 01da 0c77 6f72 6465  inocode)...worde
+00000240: 6d62 746f 6f6c 734e 2906 da07 5f5f 646f  mbtoolsN)...__do
+00000250: 635f 5fda 0072 0200 0000 7203 0000 0072  c__..r....r....r
+00000260: 0400 0000 7205 0000 00a9 0072 0800 0000  ....r......r....
+00000270: 7208 0000 00fa 2d62 7569 6c64 5c62 6469  r.....-build\bdi
+00000280: 7374 2e77 696e 2d61 6d64 3634 5c65 6767  st.win-amd64\egg
+00000290: 5c62 696f 7465 7874 5c5f 5f69 6e69 745f  \biotext\__init_
+000002a0: 5f2e 7079 da08 3c6d 6f64 756c 653e 0100  _.py..<module>..
+000002b0: 0000 730a 0000 0004 020c 0a0c 010c 0110  ..s.............
+000002c0: 01                                       .
```

## biotext/aminocode.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Nov  8 23:50:39 2022 UTC, .py size: 6594 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,368 +1,396 @@
-00000000: 550d 0d0a 0000 0000 4feb 6a63 c219 0000  U.......O.jc....
+00000000: 6f0d 0d0a 0000 0000 9d7f af64 3c1b 0000  o..........d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 001e 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6403 6404 6405 6406 6407 6408 6409  Z.d.d.d.d.d.d.d.
-00000050: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
-00000060: 6412 6413 6414 6415 6416 6417 6418 6419  d.d.d.d.d.d.d.d.
-00000070: 641a 641b 641c 641d 641e 641f 6420 9c1d  d.d.d.d.d.d.d ..
-00000080: 5a03 6421 6422 6423 6424 6425 6426 6427  Z.d!d"d#d$d%d&d'
-00000090: 6428 6429 642a 642b 9c0a 5a04 642c 642d  d(d)d*d+..Z.d,d-
-000000a0: 642e 642f 6430 6431 6432 9c06 5a05 643d  d.d/d0d1d2..Z.d=
-000000b0: 6434 6435 8401 5a06 643e 6436 6437 8401  d4d5..Z.d>d6d7..
-000000c0: 5a07 643f 6439 643a 8401 5a08 6440 643b  Z.d?d9d:..Z.d@d;
-000000d0: 643c 8401 5a09 6402 5300 2941 7a4e 0a4c  d<..Z.d.S.)AzN.L
-000000e0: 6962 7261 7279 2077 6974 6820 6675 6e63  ibrary with func
-000000f0: 7469 6f6e 7320 666f 7220 656e 636f 6469  tions for encodi
-00000100: 6e67 2061 6e64 2064 6563 6f64 696e 6720  ng and decoding 
-00000110: 7573 696e 6720 7468 6520 414d 494e 4f63  using the AMINOc
-00000120: 6f64 6520 6d65 7468 6f64 2e0a e900 0000  ode method......
-00000130: 004e 5a02 5941 da01 45da 0143 da01 445a  .NZ.YA..E..C..DZ
-00000140: 0259 45da 0146 da01 47da 0148 5a02 5949  .YE..F..G..HZ.YI
-00000150: da01 49da 014b da01 4cda 014d da01 4e5a  ..I..K..L..M..NZ
-00000160: 0259 51da 0150 da01 51da 0152 da01 53da  .YQ..P..Q..R..S.
-00000170: 0154 5a02 5956 da01 56da 0157 da01 415a  .TZ.YV..V..W..AZ
-00000180: 0259 575a 0259 595a 0259 505a 0259 445a  .YWZ.YYZ.YPZ.YDZ
-00000190: 0259 5329 1dda 0161 da01 62da 0163 da01  .YS)...a..b..c..
-000001a0: 64da 0165 da01 66da 0167 da01 68da 0169  d..e..f..g..h..i
-000001b0: da01 6ada 016b da01 6cda 016d da01 6eda  ..j..k..l..m..n.
-000001c0: 016f da01 70da 0171 da01 72da 0173 da01  .o..p..q..r..s..
-000001d0: 74da 0175 da01 76da 0178 da01 7ada 0177  t..u..v..x..z..w
-000001e0: da01 79da 012e da01 39fa 0120 5a03 5944  ..y.....9.. Z.YD
-000001f0: 415a 0359 4451 5a03 5944 545a 0359 4448  AZ.YDQZ.YDTZ.YDH
-00000200: 5a03 5944 465a 0359 4449 5a03 5944 535a  Z.YDFZ.YDIZ.YDSZ
-00000210: 0359 4445 5a03 5944 475a 0359 444e 290a  .YDEZ.YDGZ.YDN).
-00000220: da01 30da 0131 da01 32da 0133 da01 34da  ..0..1..2..3..4.
-00000230: 0135 da01 36da 0137 da01 3872 3000 0000  .5..6..7..8r0...
-00000240: 5a03 5950 455a 0359 5043 5a03 5950 535a  Z.YPEZ.YPCZ.YPSZ
-00000250: 0359 5057 5a03 5950 515a 0359 5054 2906  .YPWZ.YPQZ.YPT).
-00000260: 722f 0000 00fa 012c fa01 3bfa 0121 fa01  r/.....,..;..!..
-00000270: 3ffa 013a da02 6470 6302 0000 0000 0000  ?..:..dpc.......
-00000280: 0000 0000 0007 0000 0009 0000 0043 0000  .............C..
-00000290: 0073 ec00 0000 7a0e 7c00 a000 6401 a101  .s....z.|...d...
-000002a0: 7d00 5700 6e0c 0100 0100 0100 5900 6e02  }.W.n.......Y.n.
-000002b0: 5800 7401 a001 7c00 a101 7d00 7c00 a002  X.t...|...}.|...
-000002c0: a100 7d00 7403 a004 6402 6403 7c00 a103  ..}.t...d.d.|...
-000002d0: 7d00 7405 a006 a100 7d02 6404 7c01 6b06  }.t.....}.d.|.k.
-000002e0: 7258 7c02 a007 7408 a101 0100 6e0e 7403  rX|...t.....n.t.
-000002f0: a004 6405 6406 7c00 a103 7d00 6407 7c01  ..d.d.|...}.d.|.
-00000300: 6b06 727a 7c02 a007 7409 a101 0100 6e0e  k.rz|...t.....n.
-00000310: 7403 a004 6408 6409 7c00 a103 7d00 640a  t...d.d.|...}.d.
-00000320: a00a 740b 7c00 8301 a101 4400 5d2e 7d03  ..t.|.....D.].}.
-00000330: 7a0c 7c02 7c03 1900 0100 5700 7196 0400  z.|.|.....W.q...
-00000340: 740c 6b0a 72c2 0100 0100 0100 640b 7c02  t.k.r.......d.|.
-00000350: 7c03 3c00 5900 7196 5800 7196 7c02 a00d  |.<.Y.q.X.q.|...
-00000360: a100 4400 5d14 5c02 7d04 7d05 7c00 a00e  ..D.].\.}.}.|...
-00000370: 7c04 7c05 a102 7d00 71ce 7c00 7d06 7c06  |.|...}.q.|.}.|.
-00000380: 5300 290c 6179 0200 000a 2020 2020 456e  S.).ay....    En
-00000390: 636f 6465 7320 6120 7374 7269 6e67 2077  codes a string w
-000003a0: 6974 6820 414d 494e 4f63 6f64 652e 0a20  ith AMINOcode.. 
-000003b0: 2020 200a 2020 2020 5061 7261 6d65 7465     .    Paramete
-000003c0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-000003d0: 2d0a 2020 2020 696e 7075 745f 7374 7269  -.    input_stri
-000003e0: 6e67 203a 2073 7472 696e 670a 2020 2020  ng : string.    
-000003f0: 2020 2020 4e61 7475 7261 6c20 6c61 6e67      Natural lang
-00000400: 7561 6765 2074 6578 7420 7374 7269 6e67  uage text string
-00000410: 2074 6f20 6265 2065 6e63 6f64 6564 2e0a   to be encoded..
-00000420: 2020 2020 6465 7461 696c 203a 2073 7472      detail : str
-00000430: 696e 670a 2020 2020 2020 2020 5365 7420  ing.        Set 
-00000440: 6465 7461 696c 7320 696e 2063 6f64 696e  details in codin
-00000450: 672e 2027 6427 2066 6f72 2064 6574 6169  g. 'd' for detai
-00000460: 6c73 2069 6e20 6469 6769 7473 3b20 2770  ls in digits; 'p
-00000470: 2720 666f 7220 6465 7461 696c 7320 6f6e  ' for details on
-00000480: 200a 2020 2020 2020 2020 7468 6520 7075   .        the pu
-00000490: 6e63 7475 6174 696f 6e3b 2027 6470 2720  nctuation; 'dp' 
-000004a0: 6f72 2027 7064 2720 666f 7220 626f 7468  or 'pd' for both
-000004b0: 2e0a 2020 2020 2020 2020 0a20 2020 204f  ..        .    O
-000004c0: 7574 7075 740a 2020 2020 2d2d 2d2d 2d2d  utput.    ------
-000004d0: 2d2d 0a20 2020 2065 6e63 6f64 6564 5f73  --.    encoded_s
-000004e0: 7472 696e 6720 3a20 7374 7269 6e67 0a20  tring : string. 
-000004f0: 2020 2020 2020 2045 6e63 6f64 6564 2074         Encoded t
-00000500: 6578 742e 0a20 2020 2020 2020 200a 2020  ext..        .  
-00000510: 2020 4578 616d 706c 650a 2020 2020 2d2d    Example.    --
-00000520: 2d2d 2d2d 2d2d 0a20 2020 2045 6e63 6f6e  ------.    Encon
-00000530: 6465 2061 2073 7472 696e 672e 0a0a 2020  de a string...  
-00000540: 2020 3e3e 3e20 696d 706f 7274 2062 696f    >>> import bio
-00000550: 7465 7874 2061 7320 6274 0a20 2020 203e  text as bt.    >
-00000560: 3e3e 2069 6e70 7574 5f73 7472 696e 6720  >> input_string 
-00000570: 3d20 2248 656c 6c6f 2077 6f72 6c64 2122  = "Hello world!"
-00000580: 0a20 2020 203e 3e3e 2065 6e63 6f64 6564  .    >>> encoded
-00000590: 5f73 7472 696e 6720 3d20 6274 2e61 6d69  _string = bt.ami
-000005a0: 6e6f 636f 6465 2e65 6e63 6f64 655f 7374  nocode.encode_st
-000005b0: 7269 6e67 2869 6e70 7574 5f73 7472 696e  ring(input_strin
-000005c0: 672c 2764 7027 290a 2020 2020 3e3e 3e20  g,'dp').    >>> 
-000005d0: 7072 696e 7428 656e 636f 6465 645f 7374  print(encoded_st
-000005e0: 7269 6e67 290a 2020 2020 4859 454c 4c59  ring).    HYELLY
-000005f0: 5159 5359 5759 5152 4c44 5950 570a 2020  QYSYWYQRLDYPW.  
-00000600: 2020 7a05 7574 662d 387a 025c 7372 3100    z.utf-8z.\sr1.
-00000610: 0000 7218 0000 007a 025c 6472 3000 0000  ..r....z.\dr0...
-00000620: 7224 0000 007a 075b 2c3b 213f 3a5d 722f  r$...z.[,;!?:]r/
-00000630: 0000 00da 00da 0259 4b29 0fda 0664 6563  .......YK)...dec
-00000640: 6f64 65da 0975 6e69 6465 636f 6465 da05  ode..unidecode..
-00000650: 6c6f 7765 72da 0272 65da 0373 7562 da0f  lower..re..sub..
-00000660: 616d 696e 6f63 6f64 655f 7461 626c 65da  aminocode_table.
-00000670: 0463 6f70 79da 0675 7064 6174 65da 1161  .copy..update..a
-00000680: 6d69 6e6f 636f 6465 5f74 6162 6c65 5f64  minocode_table_d
-00000690: da11 616d 696e 6f63 6f64 655f 7461 626c  ..aminocode_tabl
-000006a0: 655f 70da 046a 6f69 6eda 0373 6574 da08  e_p..join..set..
-000006b0: 4b65 7945 7272 6f72 da05 6974 656d 73da  KeyError..items.
-000006c0: 0772 6570 6c61 6365 2907 da0c 696e 7075  .replace)...inpu
-000006d0: 745f 7374 7269 6e67 da06 6465 7461 696c  t_string..detail
-000006e0: da06 635f 6469 6374 721d 0000 0072 1f00  ..c_dictr....r..
-000006f0: 0000 722a 0000 00da 0e65 6e63 6f64 6564  ..r*.....encoded
-00000700: 5f73 7472 696e 67a9 0072 5600 0000 fa2e  _string..rV.....
-00000710: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
-00000720: 616d 6436 345c 6567 675c 6269 6f74 6578  amd64\egg\biotex
-00000730: 745c 616d 696e 6f63 6f64 652e 7079 da0d  t\aminocode.py..
-00000740: 656e 636f 6465 5f73 7472 696e 673f 0000  encode_string?..
-00000750: 0073 2e00 0000 001c 0201 0e01 0601 0602  .s..............
-00000760: 0a01 0801 0e02 0801 0801 0c02 0e01 0801  ................
-00000770: 0c02 0e02 1201 0201 0c01 0e01 1002 1001  ................
-00000780: 0e01 0401 7258 0000 0063 0200 0000 0000  ....rX...c......
-00000790: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
-000007a0: 0000 7378 0000 0074 00a0 01a1 007d 0264  ..sx...t.....}.d
-000007b0: 017c 016b 0672 1a7c 02a0 0274 03a1 0101  .|.k.r.|...t....
-000007c0: 0064 027c 016b 0672 2c7c 02a0 0274 04a1  .d.|.k.r,|...t..
-000007d0: 0101 0074 0574 067c 02a0 07a1 0064 0364  ...t.t.|.....d.d
-000007e0: 0484 0064 0564 068d 0383 017d 027c 00a0  ...d.d.....}.|..
-000007f0: 0864 0764 08a1 027d 007c 02a0 07a1 0044  .d.d...}.|.....D
-00000800: 005d 145c 027d 037d 047c 00a0 087c 047c  .].\.}.}.|...|.|
-00000810: 03a1 027d 0071 5a7c 007d 057c 0553 0029  ...}.qZ|.}.|.S.)
-00000820: 0961 7502 0000 0a20 2020 2044 6563 6f64  .au....    Decod
-00000830: 6573 2061 2073 7472 696e 6720 7769 7468  es a string with
-00000840: 2041 4d49 4e4f 636f 6465 2072 6576 6572   AMINOcode rever
-00000850: 7365 2e0a 2020 2020 0a20 2020 2050 6172  se..    .    Par
-00000860: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00000870: 2d2d 2d2d 2d2d 0a20 2020 2069 6e70 7574  ------.    input
-00000880: 5f73 7472 696e 6720 3a20 7374 7269 6e67  _string : string
-00000890: 0a20 2020 2020 2020 2054 6578 7420 7374  .        Text st
-000008a0: 7269 6e67 2065 6e63 6f64 6564 2077 6974  ring encoded wit
-000008b0: 6820 414d 494e 4f63 6f64 652e 0a20 2020  h AMINOcode..   
-000008c0: 2064 6574 6169 6c20 3a20 7374 7269 6e67   detail : string
-000008d0: 0a20 2020 2020 2020 2053 6574 2064 6574  .        Set det
-000008e0: 6169 6c73 2069 6e20 636f 6469 6e67 2e20  ails in coding. 
-000008f0: 2764 2720 666f 7220 6465 7461 696c 7320  'd' for details 
-00000900: 696e 2064 6967 6974 733b 2027 7027 2066  in digits; 'p' f
-00000910: 6f72 2064 6574 6169 6c73 206f 6e20 0a20  or details on . 
-00000920: 2020 2020 2020 2074 6865 2070 756e 6374         the punct
-00000930: 7561 7469 6f6e 3b20 2764 7027 206f 7220  uation; 'dp' or 
-00000940: 2770 6427 2066 6f72 2062 6f74 682e 0a0a  'pd' for both...
-00000950: 2020 2020 4f75 7470 7574 0a20 2020 202d      Output.    -
-00000960: 2d2d 2d2d 2d2d 2d0a 2020 2020 6465 636f  -------.    deco
-00000970: 6465 645f 7374 7269 6e67 203a 2073 7472  ded_string : str
-00000980: 696e 670a 2020 2020 2020 2020 4465 636f  ing.        Deco
-00000990: 6465 6420 7465 7874 2e0a 2020 2020 2020  ded text..      
-000009a0: 2020 0a20 2020 2045 7861 6d70 6c65 0a20    .    Example. 
-000009b0: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-000009c0: 4465 636f 6e64 6520 6120 7374 7269 6e67  Deconde a string
-000009d0: 2e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  ...    >>> impor
-000009e0: 7420 6269 6f74 6578 7420 6173 2062 740a  t biotext as bt.
-000009f0: 2020 2020 3e3e 3e20 656e 636f 6465 645f      >>> encoded_
-00000a00: 7374 7269 6e67 203d 2022 4859 454c 4c59  string = "HYELLY
-00000a10: 5159 5359 5759 5152 4c44 5950 5722 0a20  QYSYWYQRLDYPW". 
-00000a20: 2020 203e 3e3e 2064 6563 6f64 6564 5f73     >>> decoded_s
-00000a30: 7472 696e 6720 3d20 6274 2e61 6d69 6e6f  tring = bt.amino
-00000a40: 636f 6465 2e64 6563 6f64 655f 7374 7269  code.decode_stri
-00000a50: 6e67 2865 6e63 6f64 6564 5f73 7472 696e  ng(encoded_strin
-00000a60: 672c 2764 7027 290a 2020 2020 3e3e 3e20  g,'dp').    >>> 
-00000a70: 7072 696e 7428 6465 636f 6465 645f 7374  print(decoded_st
-00000a80: 7269 6e67 290a 2020 2020 6865 6c6c 6f20  ring).    hello 
-00000a90: 776f 726c 6421 0a20 2020 2072 1800 0000  world!.    r....
-00000aa0: 7224 0000 0063 0100 0000 0000 0000 0000  r$...c..........
-00000ab0: 0000 0100 0000 0300 0000 5300 0000 7314  ..........S...s.
-00000ac0: 0000 0074 007c 0064 0119 0083 017c 0064  ...t.|.d.....|.d
-00000ad0: 0219 0066 0253 0029 034e e901 0000 0072  ...f.S.).N.....r
-00000ae0: 0100 0000 2901 da03 6c65 6ea9 0172 2b00  ....)...len..r+.
-00000af0: 0000 7256 0000 0072 5600 0000 7257 0000  ..rV...rV...rW..
-00000b00: 00da 083c 6c61 6d62 6461 3e9b 0000 00f3  ...<lambda>.....
-00000b10: 0000 0000 7a1f 6465 636f 6465 5f73 7472  ....z.decode_str
-00000b20: 696e 672e 3c6c 6f63 616c 733e 2e3c 6c61  ing.<locals>.<la
-00000b30: 6d62 6461 3e54 2902 da03 6b65 79da 0772  mbda>T)...key..r
-00000b40: 6576 6572 7365 7242 0000 00fa 012d 2909  everserB.....-).
-00000b50: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
-00000b60: 4b00 0000 724c 0000 00da 0464 6963 74da  K...rL.....dict.
-00000b70: 0673 6f72 7465 6472 5000 0000 7251 0000  .sortedrP...rQ..
-00000b80: 0029 0672 5200 0000 7253 0000 0072 5400  .).rR...rS...rT.
-00000b90: 0000 721f 0000 0072 2a00 0000 da0e 6465  ..r....r*.....de
-00000ba0: 636f 6465 645f 7374 7269 6e67 7256 0000  coded_stringrV..
-00000bb0: 0072 5600 0000 7257 0000 00da 0d64 6563  .rV...rW.....dec
-00000bc0: 6f64 655f 7374 7269 6e67 7900 0000 7316  ode_stringy...s.
-00000bd0: 0000 0000 1c08 0108 010a 0108 010a 021a  ................
-00000be0: 010c 0110 010e 0104 0172 6400 0000 4663  .........rd...Fc
-00000bf0: 0300 0000 0000 0000 0000 0000 0900 0000  ................
-00000c00: 0500 0000 0300 0000 7398 0000 0074 007c  ........s....t.|
-00000c10: 0083 017d 0387 0066 0164 0164 0284 087d  ...}...f.d.d...}
-00000c20: 0467 007d 057c 0272 2474 0164 0383 0101  .g.}.|.r$t.d....
-00000c30: 0074 027c 0083 0144 005d 4a5c 027d 067d  .t.|...D.]J\.}.}
-00000c40: 077c 047c 0783 017d 087c 05a0 037c 08a1  .|.|...}.|...|..
-00000c50: 0101 007c 0272 2c7c 0664 0417 0064 0516  ...|.r,|.d...d..
-00000c60: 0064 066b 0272 2c74 0174 047c 0664 0417  .d.k.r,t.t.|.d..
-00000c70: 0083 0164 0717 0074 047c 0383 0117 0083  ...d...t.|......
-00000c80: 0101 0071 2c7c 0272 9474 0174 047c 0383  ...q,|.r.t.t.|..
-00000c90: 0164 0717 0074 047c 0383 0117 0083 0101  .d...t.|........
-00000ca0: 007c 0553 0029 0861 0003 0000 0a20 2020  .|.S.).a.....   
-00000cb0: 2045 6e63 6f64 6573 2061 6c6c 2073 7472   Encodes all str
-00000cc0: 696e 6773 2069 6e20 6120 6c69 7374 2077  ings in a list w
-00000cd0: 6974 6820 414d 494e 4f63 6f64 652e 0a20  ith AMINOcode.. 
-00000ce0: 2020 200a 2020 2020 5061 7261 6d65 7465     .    Paramete
-00000cf0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00000d00: 2d0a 2020 2020 7374 7269 6e67 5f6c 6973  -.    string_lis
-00000d10: 7420 3a20 6c69 7374 0a20 2020 2020 2020  t : list.       
-00000d20: 204c 6973 7420 6f66 2073 7472 696e 6720   List of string 
-00000d30: 746f 2062 6520 656e 636f 6465 642e 0a20  to be encoded.. 
-00000d40: 2020 2064 6574 6169 6c20 3a20 7374 7269     detail : stri
-00000d50: 6e67 0a20 2020 2020 2020 2053 6574 2064  ng.        Set d
-00000d60: 6574 6169 6c73 2069 6e20 636f 6469 6e67  etails in coding
-00000d70: 2e20 2764 2720 666f 7220 6465 7461 696c  . 'd' for detail
-00000d80: 7320 696e 2064 6967 6974 733b 2027 7027  s in digits; 'p'
-00000d90: 2066 6f72 2064 6574 6169 6c73 206f 6e20   for details on 
-00000da0: 0a20 2020 2020 2020 2074 6865 2070 756e  .        the pun
-00000db0: 6374 7561 7469 6f6e 3b20 2764 7027 206f  ctuation; 'dp' o
-00000dc0: 7220 2770 6427 2066 6f72 2062 6f74 682e  r 'pd' for both.
-00000dd0: 0a20 2020 2076 6572 626f 7365 203a 2062  .    verbose : b
-00000de0: 6f6f 6c0a 2020 2020 2020 2020 4966 2054  ool.        If T
-00000df0: 7275 6520 6469 7370 6c61 7973 2070 726f  rue displays pro
-00000e00: 6772 6573 732e 0a0a 2020 2020 4f75 7470  gress...    Outp
-00000e10: 7574 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  ut.    --------.
-00000e20: 2020 2020 656e 636f 6465 645f 6c69 7374      encoded_list
-00000e30: 203a 206c 6973 740a 2020 2020 2020 2020   : list.        
-00000e40: 4c69 7374 2077 6974 6820 616c 6c20 656e  List with all en
-00000e50: 636f 6465 6420 7465 7874 2069 6e20 7374  coded text in st
-00000e60: 7269 6e67 2066 6f72 6d61 742e 0a20 2020  ring format..   
-00000e70: 2020 2020 200a 2020 2020 4578 616d 706c       .    Exampl
-00000e80: 650a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  e.    --------. 
-00000e90: 2020 2045 6e63 6f64 6520 7468 6520 7374     Encode the st
-00000ea0: 7269 6e67 7320 696e 2061 206c 6973 7420  rings in a list 
-00000eb0: 616e 6420 7669 6577 2074 6865 2072 6573  and view the res
-00000ec0: 756c 7420 6f66 2074 6865 2066 6972 7374  ult of the first
-00000ed0: 2069 7465 6d2e 0a0a 2020 2020 3e3e 3e20   item...    >>> 
-00000ee0: 696d 706f 7274 2062 696f 7465 7874 2061  import biotext a
-00000ef0: 7320 6274 0a20 2020 203e 3e3e 2073 7472  s bt.    >>> str
-00000f00: 696e 675f 6c69 7374 203d 205b 2748 656c  ing_list = ['Hel
-00000f10: 6c6f 272c 2777 6f72 6c64 272c 2721 275d  lo','world','!']
-00000f20: 0a20 2020 203e 3e3e 2065 6e63 6f64 6564  .    >>> encoded
-00000f30: 5f6c 6973 7420 3d20 6274 2e61 6d69 6e6f  _list = bt.amino
-00000f40: 636f 6465 2e65 6e63 6f64 655f 6c69 7374  code.encode_list
-00000f50: 2873 7472 696e 675f 6c69 7374 2c64 6574  (string_list,det
-00000f60: 6169 6c3d 2764 7027 290a 2020 2020 3e3e  ail='dp').    >>
-00000f70: 3e20 7072 696e 7428 656e 636f 6465 645f  > print(encoded_
-00000f80: 6c69 7374 290a 2020 2020 5b27 4859 454c  list).    ['HYEL
-00000f90: 4c59 5127 2c20 2759 5759 5152 4c44 272c  LYQ', 'YWYQRLD',
-00000fa0: 2027 5950 5727 5d0a 2020 2020 6301 0000   'YPW'].    c...
-00000fb0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000fc0: 0013 0000 0073 0c00 0000 7400 7c00 8800  .....s....t.|...
-00000fd0: 6401 8d02 5300 a902 4ea9 0172 5300 0000  d...S...N..rS...
-00000fe0: 2901 7258 0000 0072 5b00 0000 7266 0000  ).rX...r[...rf..
-00000ff0: 0072 5600 0000 7257 0000 0072 5c00 0000  .rV...rW...r\...
-00001000: c100 0000 725d 0000 007a 1d65 6e63 6f64  ....r]...z.encod
-00001010: 655f 6c69 7374 2e3c 6c6f 6361 6c73 3e2e  e_list.<locals>.
-00001020: 3c6c 616d 6264 613e 7a10 456e 636f 6469  <lambda>z.Encodi
-00001030: 6e67 2074 6578 742e 2e2e 7259 0000 00e9  ng text...rY....
-00001040: 1027 0000 7201 0000 00fa 012f 2905 725a  .'..r....../).rZ
-00001050: 0000 00da 0570 7269 6e74 da09 656e 756d  .....print..enum
-00001060: 6572 6174 65da 0661 7070 656e 64da 0373  erate..append..s
-00001070: 7472 2909 5a0b 7374 7269 6e67 5f6c 6973  tr).Z.string_lis
-00001080: 7472 5300 0000 da07 7665 7262 6f73 65da  trS.....verbose.
-00001090: 096c 6973 745f 7369 7a65 da0f 7365 6c65  .list_size..sele
-000010a0: 6374 6564 456e 636f 6465 725a 0c65 6e63  ctedEncoderZ.enc
-000010b0: 6f64 6564 5f6c 6973 7472 1700 0000 721d  oded_listr....r.
-000010c0: 0000 00da 0373 6571 7256 0000 0072 6600  .....seqrV...rf.
-000010d0: 0000 7257 0000 00da 0b65 6e63 6f64 655f  ..rW.....encode_
-000010e0: 6c69 7374 a200 0000 731a 0000 0000 1e08  list....s.......
-000010f0: 010c 0204 0104 0108 0110 0108 010a 0114  ................
-00001100: 011e 0104 0118 0172 7100 0000 6303 0000  .......rq...c...
-00001110: 0000 0000 0000 0000 0008 0000 0006 0000  ................
-00001120: 0003 0000 0073 a000 0000 7400 7c00 8301  .....s....t.|...
-00001130: 7d03 8700 6601 6401 6402 8408 7d04 6700  }...f.d.d...}.g.
-00001140: 7d05 7c02 7224 7401 6403 8301 0100 7402  }.|.r$t.d.....t.
-00001150: 7c00 8301 4400 5d52 5c02 7d06 7d07 7c06  |...D.]R\.}.}.|.
-00001160: 6404 3700 7d06 7c02 726c 7c06 6404 1700  d.7.}.|.rl|.d...
-00001170: 6405 1600 6406 6b02 726c 7401 7403 7c06  d...d.k.rlt.t.|.
-00001180: 6404 1700 8301 6407 1700 7403 7c03 8301  d.....d...t.|...
-00001190: 1700 8301 0100 7c05 a004 7c04 7403 7c07  ......|...|.t.|.
-000011a0: 8301 8301 a101 0100 712c 7c02 729c 7401  ........q,|.r.t.
-000011b0: 7403 7c03 8301 6407 1700 7403 7c03 8301  t.|...d...t.|...
-000011c0: 1700 8301 0100 7c05 5300 2908 610a 0300  ......|.S.).a...
-000011d0: 000a 2020 2020 4465 636f 6465 7320 616c  ..    Decodes al
-000011e0: 6c20 7374 7269 6e67 7320 696e 2061 206c  l strings in a l
-000011f0: 6973 7420 7769 7468 2072 6576 6572 7365  ist with reverse
-00001200: 2041 4d49 4e4f 636f 6465 2e09 0a20 2020   AMINOcode...   
-00001210: 200a 2020 2020 5061 7261 6d65 7465 7273   .    Parameters
-00001220: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00001230: 2020 2020 7374 7269 6e67 5f6c 6973 7420      string_list 
-00001240: 3a20 6c69 7374 0a20 2020 2020 2020 204c  : list.        L
-00001250: 6973 7420 6f66 2073 7472 696e 6720 656e  ist of string en
-00001260: 636f 6465 6420 7769 7468 2061 6d69 6e6f  coded with amino
-00001270: 636f 6465 2e0a 2020 2020 6465 7461 696c  code..    detail
-00001280: 203a 2073 7472 696e 670a 2020 2020 2020   : string.      
-00001290: 2020 5365 7420 6465 7461 696c 7320 696e    Set details in
-000012a0: 2063 6f64 696e 672e 2027 6427 2066 6f72   coding. 'd' for
-000012b0: 2064 6574 6169 6c73 2069 6e20 6469 6769   details in digi
-000012c0: 7473 3b20 2770 2720 666f 7220 6465 7461  ts; 'p' for deta
-000012d0: 696c 7320 6f6e 200a 2020 2020 2020 2020  ils on .        
-000012e0: 7468 6520 7075 6e63 7475 6174 696f 6e3b  the punctuation;
-000012f0: 2027 6470 2720 6f72 2027 7064 2720 666f   'dp' or 'pd' fo
-00001300: 7220 626f 7468 2e0a 2020 2020 7665 7262  r both..    verb
-00001310: 6f73 6520 3a20 626f 6f6c 0a20 2020 2020  ose : bool.     
-00001320: 2020 2049 6620 5472 7565 2064 6973 706c     If True displ
-00001330: 6179 7320 7072 6f67 7265 7373 2e0a 0a20  ays progress... 
-00001340: 2020 204f 7574 7075 740a 2020 2020 2d2d     Output.    --
-00001350: 2d2d 2d2d 2d2d 0a20 2020 2064 6563 6f64  ------.    decod
-00001360: 6564 5f6c 6973 7420 3a20 6c69 7374 206f  ed_list : list o
-00001370: 6620 7374 7269 6e67 0a20 2020 2020 2020  f string.       
-00001380: 204c 6973 7420 7769 7468 2061 6c6c 2064   List with all d
-00001390: 6563 6f64 6564 2074 6578 742e 0a20 2020  ecoded text..   
-000013a0: 2020 2020 200a 2020 2020 4578 616d 706c       .    Exampl
-000013b0: 650a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  e.    --------. 
-000013c0: 2020 2044 6573 636f 6465 2074 6865 2073     Descode the s
-000013d0: 7472 696e 6773 2069 6e20 6120 6c69 7374  trings in a list
-000013e0: 2061 6e64 2076 6965 7720 7468 6520 7265   and view the re
-000013f0: 7375 6c74 2077 6974 6820 6120 6c6f 6f70  sult with a loop
-00001400: 2e0a 0a20 2020 203e 3e3e 2069 6d70 6f72  ...    >>> impor
-00001410: 7420 6269 6f74 6578 7420 6173 2062 740a  t biotext as bt.
-00001420: 2020 2020 3e3e 3e20 656e 636f 6465 645f      >>> encoded_
-00001430: 6c69 7374 203d 205b 2748 5945 4c4c 5951  list = ['HYELLYQ
-00001440: 272c 2027 5957 5951 524c 4427 2c20 2759  ', 'YWYQRLD', 'Y
-00001450: 5057 275d 0a20 2020 203e 3e3e 2064 6563  PW'].    >>> dec
-00001460: 6f64 6564 5f6c 6973 7420 3d20 6274 2e61  oded_list = bt.a
-00001470: 6d69 6e6f 636f 6465 2e64 6563 6f64 655f  minocode.decode_
-00001480: 6c69 7374 2865 6e63 6f64 6564 5f6c 6973  list(encoded_lis
-00001490: 742c 6465 7461 696c 3d27 6470 2729 0a20  t,detail='dp'). 
-000014a0: 2020 203e 3e3e 2070 7269 6e74 2864 6563     >>> print(dec
-000014b0: 6f64 6564 5f6c 6973 7429 0a20 2020 205b  oded_list).    [
-000014c0: 2768 656c 6c6f 272c 2027 776f 726c 6427  'hello', 'world'
-000014d0: 2c20 2721 275d 0a20 2020 2063 0100 0000  , '!'].    c....
-000014e0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-000014f0: 1300 0000 730c 0000 0074 007c 0088 0064  ....s....t.|...d
-00001500: 018d 0253 0072 6500 0000 2901 7264 0000  ...S.re...).rd..
-00001510: 0072 5b00 0000 7266 0000 0072 5600 0000  .r[...rf...rV...
-00001520: 7257 0000 0072 5c00 0000 ee00 0000 725d  rW...r\.......r]
-00001530: 0000 007a 1d64 6563 6f64 655f 6c69 7374  ...z.decode_list
-00001540: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00001550: 613e 7a10 4465 636f 6469 6e67 2074 6578  a>z.Decoding tex
-00001560: 742e 2e2e 7259 0000 0072 6700 0000 7201  t...rY...rg...r.
-00001570: 0000 0072 6800 0000 2905 725a 0000 0072  ...rh...).rZ...r
-00001580: 6900 0000 726a 0000 0072 6c00 0000 726b  i...rj...rl...rk
-00001590: 0000 0029 085a 0a69 6e70 7574 5f6c 6973  ...).Z.input_lis
-000015a0: 7472 5300 0000 726d 0000 0072 6e00 0000  trS...rm...rn...
-000015b0: 726f 0000 005a 0c64 6563 6f64 6564 5f6c  ro...Z.decoded_l
-000015c0: 6973 7472 1700 0000 721d 0000 0072 5600  istr....r....rV.
-000015d0: 0000 7266 0000 0072 5700 0000 da0b 6465  ..rf...rW.....de
-000015e0: 636f 6465 5f6c 6973 74cf 0000 0073 1a00  code_list....s..
-000015f0: 0000 001e 0801 0c02 0401 0401 0801 1001  ................
-00001600: 0801 1401 1c01 1401 0401 1802 7272 0000  ............rr..
-00001610: 0029 0172 4000 0000 2901 7240 0000 0029  .).r@...).r@...)
-00001620: 0272 4000 0000 4629 0272 4000 0000 4629  .r@...F).r@...F)
-00001630: 0ada 075f 5f64 6f63 5f5f 7246 0000 0072  ...__doc__rF...r
-00001640: 4400 0000 7248 0000 0072 4b00 0000 724c  D...rH...rK...rL
-00001650: 0000 0072 5800 0000 7264 0000 0072 7100  ...rX...rd...rq.
-00001660: 0000 7272 0000 0072 5600 0000 7256 0000  ..rr...rV...rV..
-00001670: 0072 5600 0000 7257 0000 00da 083c 6d6f  .rV...rW.....<mo
-00001680: 6475 6c65 3e03 0000 0073 6c00 0000 0403  dule>....sl.....
-00001690: 0801 0803 0201 0201 0201 0201 0201 0201  ................
-000016a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000016b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000016c0: 0201 0201 0201 0201 0201 0201 02e3 0621  ...............!
-000016d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000016e0: 0201 02f6 060e 0201 0201 0201 0201 0201  ................
-000016f0: 02fa 0609 0a3a 0a29 0a2d                 .....:.).-
+00000040: 5a02 6900 6403 6404 9301 6405 6406 9301  Z.i.d.d...d.d...
+00000050: 6407 6408 9301 6409 640a 9301 640b 640c  d.d...d.d...d.d.
+00000060: 9301 640d 640e 9301 640f 6410 9301 6411  ..d.d...d.d...d.
+00000070: 6412 9301 6413 6414 9301 6415 6416 9301  d...d.d...d.d...
+00000080: 6417 6418 9301 6419 641a 9301 641b 641c  d.d...d.d...d.d.
+00000090: 9301 641d 641e 9301 641f 6420 9301 6421  ..d.d...d.d ..d!
+000000a0: 6422 9301 6423 6424 9301 6425 6426 6427  d"..d#d$..d%d&d'
+000000b0: 6428 6429 642a 642b 642c 642d 642e 642f  d(d)d*d+d,d-d.d/
+000000c0: 6430 6431 9c0c a501 5a03 6432 6433 6434  d0d1....Z.d2d3d4
+000000d0: 6435 6436 6437 6438 6439 643a 643b 643c  d5d6d7d8d9d:d;d<
+000000e0: 9c0a 5a04 643d 643e 643f 6440 6441 6442  ..Z.d=d>d?d@dAdB
+000000f0: 6443 9c06 5a05 644e 6445 6446 8401 5a06  dC..Z.dNdEdF..Z.
+00000100: 644e 6447 6448 8401 5a07 644f 644a 644b  dNdGdH..Z.dOdJdK
+00000110: 8401 5a08 644f 644c 644d 8401 5a09 6402  ..Z.dOdLdM..Z.d.
+00000120: 5300 2950 617d 0100 000a 5468 6973 206d  S.)Pa}....This m
+00000130: 6f64 756c 6520 7072 6f76 6964 6573 2066  odule provides f
+00000140: 756e 6374 696f 6e73 2066 6f72 2065 6e63  unctions for enc
+00000150: 6f64 696e 6720 616e 6420 6465 636f 6469  oding and decodi
+00000160: 6e67 2074 6578 7420 7573 696e 6720 414d  ng text using AM
+00000170: 494e 4f63 6f64 652e 0a0a 4675 6e63 7469  INOcode...Functi
+00000180: 6f6e 733a 0a2d 2065 6e63 6f64 655f 7374  ons:.- encode_st
+00000190: 7269 6e67 3a20 456e 636f 6465 7320 6120  ring: Encodes a 
+000001a0: 7374 7269 6e67 2075 7369 6e67 2041 4d49  string using AMI
+000001b0: 4e4f 636f 6465 2e0a 2d20 6465 636f 6465  NOcode..- decode
+000001c0: 5f73 7472 696e 673a 2044 6563 6f64 6573  _string: Decodes
+000001d0: 2061 2073 7472 696e 6720 656e 636f 6465   a string encode
+000001e0: 6420 7769 7468 2041 4d49 4e4f 636f 6465  d with AMINOcode
+000001f0: 2e0a 2d20 656e 636f 6465 5f6c 6973 743a  ..- encode_list:
+00000200: 2045 6e63 6f64 6573 2061 6c6c 2073 7472   Encodes all str
+00000210: 696e 6773 2069 6e20 6120 6c69 7374 2075  ings in a list u
+00000220: 7369 6e67 2041 4d49 4e4f 636f 6465 2e0a  sing AMINOcode..
+00000230: 2d20 6465 636f 6465 5f6c 6973 743a 2044  - decode_list: D
+00000240: 6563 6f64 6573 2061 6c6c 2073 7472 696e  ecodes all strin
+00000250: 6773 2069 6e20 6120 6c69 7374 2065 6e63  gs in a list enc
+00000260: 6f64 6564 2077 6974 6820 414d 494e 4f63  oded with AMINOc
+00000270: 6f64 652e 0a0a 4175 7468 6f72 3a20 4469  ode...Author: Di
+00000280: 6f67 6f20 6465 204a 2e20 532e 204d 6163  ogo de J. S. Mac
+00000290: 6861 646f 0a44 6174 653a 2031 332f 3037  hado.Date: 13/07
+000002a0: 2f32 3032 330a e900 0000 004e da01 615a  /2023......N..aZ
+000002b0: 0259 41da 0162 da01 45da 0163 da01 43da  .YA..b..E..c..C.
+000002c0: 0164 da01 44da 0165 5a02 5945 da01 66da  .d..D..eZ.YE..f.
+000002d0: 0146 da01 67da 0147 da01 68da 0148 da01  .F..g..G..h..H..
+000002e0: 695a 0259 49da 016a da01 49da 016b da01  iZ.YI..j..I..k..
+000002f0: 4bda 016c da01 4cda 016d da01 4dda 016e  K..l..L..m..M..n
+00000300: da01 4eda 016f 5a02 5951 da01 70da 0150  ..N..oZ.YQ..p..P
+00000310: da01 71da 0151 da01 52da 0153 da01 545a  ..q..Q..R..S..TZ
+00000320: 0259 56da 0156 da01 57da 0141 5a02 5957  .YV..V..W..AZ.YW
+00000330: 5a02 5959 5a02 5950 5a02 5944 5a02 5953  Z.YYZ.YPZ.YDZ.YS
+00000340: 290c da01 72da 0173 da01 74da 0175 da01  )...r..s..t..u..
+00000350: 76da 0178 da01 7ada 0177 da01 79da 012e  v..x..z..w..y...
+00000360: da01 39fa 0120 5a03 5944 415a 0359 4451  ..9.. Z.YDAZ.YDQ
+00000370: 5a03 5944 545a 0359 4448 5a03 5944 465a  Z.YDTZ.YDHZ.YDFZ
+00000380: 0359 4449 5a03 5944 535a 0359 4445 5a03  .YDIZ.YDSZ.YDEZ.
+00000390: 5944 475a 0359 444e 290a da01 30da 0131  YDGZ.YDN)...0..1
+000003a0: da01 32da 0133 da01 34da 0135 da01 36da  ..2..3..4..5..6.
+000003b0: 0137 da01 3872 3000 0000 5a03 5950 455a  .7..8r0...Z.YPEZ
+000003c0: 0359 5043 5a03 5950 535a 0359 5057 5a03  .YPCZ.YPSZ.YPWZ.
+000003d0: 5950 515a 0359 5054 2906 722f 0000 00fa  YPQZ.YPT).r/....
+000003e0: 012c fa01 3bfa 0121 fa01 3ffa 013a da02  .,..;..!..?..:..
+000003f0: 6470 6302 0000 0000 0000 0000 0000 0007  dpc.............
+00000400: 0000 0009 0000 0043 0000 0073 e400 0000  .......C...s....
+00000410: 7a07 7c00 a000 6401 a101 7d00 5700 6e04  z.|...d...}.W.n.
+00000420: 0100 0100 0100 5900 7401 a001 7c00 a101  ......Y.t...|...
+00000430: 7d00 7c00 a002 a100 7d00 7403 a004 6402  }.|.....}.t...d.
+00000440: 6403 7c00 a103 7d00 7405 a006 a100 7d02  d.|...}.t.....}.
+00000450: 6404 7c01 7600 722a 7c02 a007 7408 a101  d.|.v.r*|...t...
+00000460: 0100 6e07 7403 a004 6405 6406 7c00 a103  ..n.t...d.d.|...
+00000470: 7d00 6407 7c01 7600 723b 7c02 a007 7409  }.d.|.v.r;|...t.
+00000480: a101 0100 6e07 7403 a004 6408 6409 7c00  ....n.t...d.d.|.
+00000490: a103 7d00 640a a00a 740b 7c00 8301 a101  ..}.d...t.|.....
+000004a0: 4400 5d15 7d03 7a06 7c02 7c03 1900 0100  D.].}.z.|.|.....
+000004b0: 5700 7149 0400 740c 795e 0100 0100 0100  W.qI..t.y^......
+000004c0: 640b 7c02 7c03 3c00 5900 7149 7700 7c02  d.|.|.<.Y.qIw.|.
+000004d0: a00d a100 4400 5d0a 5c02 7d04 7d05 7c00  ....D.].\.}.}.|.
+000004e0: a00e 7c04 7c05 a102 7d00 7163 7c00 7d06  ..|.|...}.qc|.}.
+000004f0: 7c06 5300 290c 6188 0200 000a 2020 2020  |.S.).a.....    
+00000500: 456e 636f 6465 7320 6120 7374 7269 6e67  Encodes a string
+00000510: 2077 6974 6820 414d 494e 4f63 6f64 652e   with AMINOcode.
+00000520: 0a20 2020 200a 2020 2020 5061 7261 6d65  .    .    Parame
+00000530: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000540: 2d2d 2d0a 2020 2020 696e 7075 745f 7374  ---.    input_st
+00000550: 7269 6e67 203a 2073 7472 696e 670a 2020  ring : string.  
+00000560: 2020 2020 2020 4e61 7475 7261 6c20 6c61        Natural la
+00000570: 6e67 7561 6765 2074 6578 7420 7374 7269  nguage text stri
+00000580: 6e67 2074 6f20 6265 2065 6e63 6f64 6564  ng to be encoded
+00000590: 2e0a 2020 2020 6465 7461 696c 203a 2073  ..    detail : s
+000005a0: 7472 696e 670a 2020 2020 2020 2020 5365  tring.        Se
+000005b0: 7420 6465 7461 696c 7320 696e 2063 6f64  t details in cod
+000005c0: 696e 672e 2027 6427 2066 6f72 2064 6574  ing. 'd' for det
+000005d0: 6169 6c73 2069 6e20 6469 6769 7473 3b20  ails in digits; 
+000005e0: 2770 2720 666f 7220 6465 7461 696c 7320  'p' for details 
+000005f0: 6f6e 200a 2020 2020 2020 2020 7468 6520  on .        the 
+00000600: 7075 6e63 7475 6174 696f 6e3b 2027 6470  punctuation; 'dp
+00000610: 2720 6f72 2027 7064 2720 666f 7220 626f  ' or 'pd' for bo
+00000620: 7468 2e20 4465 6661 756c 7420 6973 2027  th. Default is '
+00000630: 6470 272e 0a20 2020 2020 2020 200a 2020  dp'..        .  
+00000640: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00000650: 2d2d 2d2d 2d0a 2020 2020 656e 636f 6465  -----.    encode
+00000660: 645f 7374 7269 6e67 203a 2073 7472 696e  d_string : strin
+00000670: 670a 2020 2020 2020 2020 456e 636f 6465  g.        Encode
+00000680: 6420 7465 7874 2e0a 2020 2020 2020 2020  d text..        
+00000690: 0a20 2020 2045 7861 6d70 6c65 0a20 2020  .    Example.   
+000006a0: 202d 2d2d 2d2d 2d2d 0a20 2020 2045 6e63   -------.    Enc
+000006b0: 6f64 6520 6120 7374 7269 6e67 2e0a 0a20  ode a string... 
+000006c0: 2020 203e 3e3e 2069 6d70 6f72 7420 6269     >>> import bi
+000006d0: 6f74 6578 7420 6173 2062 740a 2020 2020  otext as bt.    
+000006e0: 3e3e 3e20 696e 7075 745f 7374 7269 6e67  >>> input_string
+000006f0: 203d 2022 4865 6c6c 6f20 776f 726c 6421   = "Hello world!
+00000700: 220a 2020 2020 3e3e 3e20 656e 636f 6465  ".    >>> encode
+00000710: 645f 7374 7269 6e67 203d 2062 742e 616d  d_string = bt.am
+00000720: 696e 6f63 6f64 652e 656e 636f 6465 5f73  inocode.encode_s
+00000730: 7472 696e 6728 696e 7075 745f 7374 7269  tring(input_stri
+00000740: 6e67 2c27 6470 2729 0a20 2020 203e 3e3e  ng,'dp').    >>>
+00000750: 2070 7269 6e74 2865 6e63 6f64 6564 5f73   print(encoded_s
+00000760: 7472 696e 6729 0a20 2020 2048 5945 4c4c  tring).    HYELL
+00000770: 5951 5953 5957 5951 524c 4459 5057 0a20  YQYSYWYQRLDYPW. 
+00000780: 2020 207a 0575 7466 2d38 7a02 5c73 7231     z.utf-8z.\sr1
+00000790: 0000 0072 0700 0000 7a02 5c64 7230 0000  ...r....z.\dr0..
+000007a0: 0072 1c00 0000 7a07 5b2c 3b21 3f3a 5d72  .r....z.[,;!?:]r
+000007b0: 2f00 0000 da00 da02 594b 290f da06 6465  /.......YK)...de
+000007c0: 636f 6465 da09 756e 6964 6563 6f64 65da  code..unidecode.
+000007d0: 056c 6f77 6572 da02 7265 da03 7375 62da  .lower..re..sub.
+000007e0: 0f61 6d69 6e6f 636f 6465 5f74 6162 6c65  .aminocode_table
+000007f0: da04 636f 7079 da06 7570 6461 7465 da11  ..copy..update..
+00000800: 616d 696e 6f63 6f64 655f 7461 626c 655f  aminocode_table_
+00000810: 64da 1161 6d69 6e6f 636f 6465 5f74 6162  d..aminocode_tab
+00000820: 6c65 5f70 da04 6a6f 696e da03 7365 74da  le_p..join..set.
+00000830: 084b 6579 4572 726f 72da 0569 7465 6d73  .KeyError..items
+00000840: da07 7265 706c 6163 6529 07da 0c69 6e70  ..replace)...inp
+00000850: 7574 5f73 7472 696e 67da 0664 6574 6169  ut_string..detai
+00000860: 6cda 0663 5f64 6963 7472 1000 0000 7213  l..c_dictr....r.
+00000870: 0000 0072 2a00 0000 da0e 656e 636f 6465  ...r*.....encode
+00000880: 645f 7374 7269 6e67 a900 7256 0000 00fa  d_string..rV....
+00000890: 2e62 7569 6c64 5c62 6469 7374 2e77 696e  .build\bdist.win
+000008a0: 2d61 6d64 3634 5c65 6767 5c62 696f 7465  -amd64\egg\biote
+000008b0: 7874 5c61 6d69 6e6f 636f 6465 2e70 79da  xt\aminocode.py.
+000008c0: 0d65 6e63 6f64 655f 7374 7269 6e67 4800  .encode_stringH.
+000008d0: 0000 7330 0000 0002 1c0e 0106 0102 010a  ..s0............
+000008e0: 0208 010e 0108 0208 010c 010e 0208 010c  ................
+000008f0: 010e 0212 0202 010c 010c 010c 0102 ff10  ................
+00000900: 030e 0104 0104 0172 5800 0000 6302 0000  .......rX...c...
+00000910: 0000 0000 0000 0000 0006 0000 0006 0000  ................
+00000920: 0043 0000 0073 7800 0000 7400 a001 a100  .C...sx...t.....
+00000930: 7d02 6401 7c01 7600 720d 7c02 a002 7403  }.d.|.v.r.|...t.
+00000940: a101 0100 6402 7c01 7600 7216 7c02 a002  ....d.|.v.r.|...
+00000950: 7404 a101 0100 7405 7406 7c02 a007 a100  t.....t.t.|.....
+00000960: 6403 6404 8400 6405 6406 8d03 8301 7d02  d.d...d.d.....}.
+00000970: 7c00 a008 6407 6408 a102 7d00 7c02 a007  |...d.d...}.|...
+00000980: a100 4400 5d0a 5c02 7d03 7d04 7c00 a008  ..D.].\.}.}.|...
+00000990: 7c04 7c03 a102 7d00 712d 7c00 7d05 7c05  |.|...}.q-|.}.|.
+000009a0: 5300 2909 6185 0200 000a 2020 2020 4465  S.).a.....    De
+000009b0: 636f 6465 7320 6120 7374 7269 6e67 2077  codes a string w
+000009c0: 6974 6820 414d 494e 4f63 6f64 6520 7265  ith AMINOcode re
+000009d0: 7665 7273 652e 0a20 2020 200a 2020 2020  verse..    .    
+000009e0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000009f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 696e  ---------.    in
+00000a00: 7075 745f 7374 7269 6e67 203a 2073 7472  put_string : str
+00000a10: 696e 670a 2020 2020 2020 2020 5465 7874  ing.        Text
+00000a20: 2073 7472 696e 6720 656e 636f 6465 6420   string encoded 
+00000a30: 7769 7468 2041 4d49 4e4f 636f 6465 2e0a  with AMINOcode..
+00000a40: 2020 2020 6465 7461 696c 203a 2073 7472      detail : str
+00000a50: 696e 670a 2020 2020 2020 2020 5365 7420  ing.        Set 
+00000a60: 6465 7461 696c 7320 696e 2063 6f64 696e  details in codin
+00000a70: 672e 2027 6427 2066 6f72 2064 6574 6169  g. 'd' for detai
+00000a80: 6c73 2069 6e20 6469 6769 7473 3b20 2770  ls in digits; 'p
+00000a90: 2720 666f 7220 6465 7461 696c 7320 6f6e  ' for details on
+00000aa0: 200a 2020 2020 2020 2020 7468 6520 7075   .        the pu
+00000ab0: 6e63 7475 6174 696f 6e3b 2027 6470 2720  nctuation; 'dp' 
+00000ac0: 6f72 2027 7064 2720 666f 7220 626f 7468  or 'pd' for both
+00000ad0: 2e20 4465 6661 756c 7420 6973 2027 6470  . Default is 'dp
+00000ae0: 272e 0a0a 2020 2020 5265 7475 726e 730a  '...    Returns.
+00000af0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000b00: 6465 636f 6465 645f 7374 7269 6e67 203a  decoded_string :
+00000b10: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00000b20: 4465 636f 6465 6420 7465 7874 2e0a 2020  Decoded text..  
+00000b30: 2020 2020 2020 0a20 2020 2045 7861 6d70        .    Examp
+00000b40: 6c65 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  le.    --------.
+00000b50: 2020 2020 4465 636f 6465 2061 2073 7472      Decode a str
+00000b60: 696e 672e 0a0a 2020 2020 3e3e 3e20 696d  ing...    >>> im
+00000b70: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
+00000b80: 6274 0a20 2020 203e 3e3e 2065 6e63 6f64  bt.    >>> encod
+00000b90: 6564 5f73 7472 696e 6720 3d20 2248 5945  ed_string = "HYE
+00000ba0: 4c4c 5951 5953 5957 5951 524c 4459 5057  LLYQYSYWYQRLDYPW
+00000bb0: 220a 2020 2020 3e3e 3e20 6465 636f 6465  ".    >>> decode
+00000bc0: 645f 7374 7269 6e67 203d 2062 742e 616d  d_string = bt.am
+00000bd0: 696e 6f63 6f64 652e 6465 636f 6465 5f73  inocode.decode_s
+00000be0: 7472 696e 6728 656e 636f 6465 645f 7374  tring(encoded_st
+00000bf0: 7269 6e67 2c27 6470 2729 0a20 2020 203e  ring,'dp').    >
+00000c00: 3e3e 2070 7269 6e74 2864 6563 6f64 6564  >> print(decoded
+00000c10: 5f73 7472 696e 6729 0a20 2020 2068 656c  _string).    hel
+00000c20: 6c6f 2077 6f72 6c64 210a 2020 2020 7207  lo world!.    r.
+00000c30: 0000 0072 1c00 0000 6301 0000 0000 0000  ...r....c.......
+00000c40: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00000c50: 0073 1400 0000 7400 7c00 6401 1900 8301  .s....t.|.d.....
+00000c60: 7c00 6402 1900 6602 5300 2903 4ee9 0100  |.d...f.S.).N...
+00000c70: 0000 7201 0000 0029 01da 036c 656e a901  ..r....)...len..
+00000c80: 722b 0000 0072 5600 0000 7256 0000 0072  r+...rV...rV...r
+00000c90: 5700 0000 da08 3c6c 616d 6264 613e a400  W.....<lambda>..
+00000ca0: 0000 7302 0000 0014 007a 1f64 6563 6f64  ..s......z.decod
+00000cb0: 655f 7374 7269 6e67 2e3c 6c6f 6361 6c73  e_string.<locals
+00000cc0: 3e2e 3c6c 616d 6264 613e 5429 02da 036b  >.<lambda>T)...k
+00000cd0: 6579 da07 7265 7665 7273 6572 4200 0000  ey..reverserB...
+00000ce0: fa01 2d29 0972 4800 0000 7249 0000 0072  ..-).rH...rI...r
+00000cf0: 4a00 0000 724b 0000 0072 4c00 0000 da04  J...rK...rL.....
+00000d00: 6469 6374 da06 736f 7274 6564 7250 0000  dict..sortedrP..
+00000d10: 0072 5100 0000 2906 7252 0000 0072 5300  .rQ...).rR...rS.
+00000d20: 0000 7254 0000 0072 1300 0000 722a 0000  ..rT...r....r*..
+00000d30: 00da 0e64 6563 6f64 6564 5f73 7472 696e  ...decoded_strin
+00000d40: 6772 5600 0000 7256 0000 0072 5700 0000  grV...rV...rW...
+00000d50: da0d 6465 636f 6465 5f73 7472 696e 6782  ..decode_string.
+00000d60: 0000 0073 1600 0000 081c 0801 0a01 0801  ...s............
+00000d70: 0a01 1a02 0c01 1001 0e01 0401 0401 7263  ..............rc
+00000d80: 0000 0046 6303 0000 0000 0000 0000 0000  ...Fc...........
+00000d90: 0009 0000 0005 0000 0003 0000 0073 9800  .............s..
+00000da0: 0000 7400 7c00 8301 7d03 8700 6601 6401  ..t.|...}...f.d.
+00000db0: 6402 8408 7d04 6700 7d05 7c02 7212 7401  d...}.g.}.|.r.t.
+00000dc0: 6403 8301 0100 7402 7c00 8301 4400 5d25  d.....t.|...D.]%
+00000dd0: 5c02 7d06 7d07 7c04 7c07 8301 7d08 7c05  \.}.}.|.|...}.|.
+00000de0: a003 7c08 a101 0100 7c02 723b 7c06 6404  ..|.....|.r;|.d.
+00000df0: 1700 6405 1600 6406 6b02 723b 7401 7404  ..d...d.k.r;t.t.
+00000e00: 7c06 6404 1700 8301 6407 1700 7404 7c03  |.d.....d...t.|.
+00000e10: 8301 1700 8301 0100 7116 7c02 724a 7401  ........q.|.rJt.
+00000e20: 7404 7c03 8301 6407 1700 7404 7c03 8301  t.|...d...t.|...
+00000e30: 1700 8301 0100 7c05 5300 2908 6111 0300  ......|.S.).a...
+00000e40: 000a 2020 2020 456e 636f 6465 7320 616c  ..    Encodes al
+00000e50: 6c20 7374 7269 6e67 7320 696e 2061 206c  l strings in a l
+00000e60: 6973 7420 7769 7468 2041 4d49 4e4f 636f  ist with AMINOco
+00000e70: 6465 2e0a 2020 2020 0a20 2020 2050 6172  de..    .    Par
+00000e80: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00000e90: 2d2d 2d2d 2d2d 0a20 2020 2073 7472 696e  ------.    strin
+00000ea0: 675f 6c69 7374 203a 206c 6973 740a 2020  g_list : list.  
+00000eb0: 2020 2020 2020 4c69 7374 206f 6620 7374        List of st
+00000ec0: 7269 6e67 2074 6f20 6265 2065 6e63 6f64  ring to be encod
+00000ed0: 6564 2e0a 2020 2020 6465 7461 696c 203a  ed..    detail :
+00000ee0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00000ef0: 5365 7420 6465 7461 696c 7320 696e 2063  Set details in c
+00000f00: 6f64 696e 672e 2027 6427 2066 6f72 2064  oding. 'd' for d
+00000f10: 6574 6169 6c73 2069 6e20 6469 6769 7473  etails in digits
+00000f20: 3b20 2770 2720 666f 7220 6465 7461 696c  ; 'p' for detail
+00000f30: 7320 6f6e 200a 2020 2020 2020 2020 7468  s on .        th
+00000f40: 6520 7075 6e63 7475 6174 696f 6e3b 2027  e punctuation; '
+00000f50: 6470 2720 6f72 2027 7064 2720 666f 7220  dp' or 'pd' for 
+00000f60: 626f 7468 2e20 4465 6661 756c 7420 6973  both. Default is
+00000f70: 2027 6470 272e 0a20 2020 2076 6572 626f   'dp'..    verbo
+00000f80: 7365 2020 3a20 626f 6f6c 0a20 2020 2020  se  : bool.     
+00000f90: 2020 2049 6620 5472 7565 2064 6973 706c     If True displ
+00000fa0: 6179 7320 7072 6f67 7265 7373 2e0a 0a20  ays progress... 
+00000fb0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00000fc0: 2d2d 2d2d 2d2d 0a20 2020 2065 6e63 6f64  ------.    encod
+00000fd0: 6564 5f6c 6973 7420 3a20 6c69 7374 0a20  ed_list : list. 
+00000fe0: 2020 2020 2020 204c 6973 7420 7769 7468         List with
+00000ff0: 2061 6c6c 2065 6e63 6f64 6564 2074 6578   all encoded tex
+00001000: 7420 696e 2073 7472 696e 6720 666f 726d  t in string form
+00001010: 6174 2e0a 2020 2020 2020 2020 0a20 2020  at..        .   
+00001020: 2045 7861 6d70 6c65 0a20 2020 202d 2d2d   Example.    ---
+00001030: 2d2d 2d2d 0a20 2020 2045 6e63 6f64 6520  ----.    Encode 
+00001040: 7468 6520 7374 7269 6e67 7320 696e 2061  the strings in a
+00001050: 206c 6973 7420 616e 6420 7669 6577 2074   list and view t
+00001060: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+00001070: 2066 6972 7374 2069 7465 6d2e 0a0a 2020   first item...  
+00001080: 2020 3e3e 3e20 696d 706f 7274 2062 696f    >>> import bio
+00001090: 7465 7874 2061 7320 6274 0a20 2020 203e  text as bt.    >
+000010a0: 3e3e 2073 7472 696e 675f 6c69 7374 203d  >> string_list =
+000010b0: 205b 2748 656c 6c6f 272c 2777 6f72 6c64   ['Hello','world
+000010c0: 272c 2721 275d 0a20 2020 203e 3e3e 2065  ','!'].    >>> e
+000010d0: 6e63 6f64 6564 5f6c 6973 7420 3d20 6274  ncoded_list = bt
+000010e0: 2e61 6d69 6e6f 636f 6465 2e65 6e63 6f64  .aminocode.encod
+000010f0: 655f 6c69 7374 2873 7472 696e 675f 6c69  e_list(string_li
+00001100: 7374 2c64 6574 6169 6c3d 2764 7027 290a  st,detail='dp').
+00001110: 2020 2020 3e3e 3e20 7072 696e 7428 656e      >>> print(en
+00001120: 636f 6465 645f 6c69 7374 290a 2020 2020  coded_list).    
+00001130: 5b27 4859 454c 4c59 5127 2c20 2759 5759  ['HYELLYQ', 'YWY
+00001140: 5152 4c44 272c 2027 5950 5727 5d0a 2020  QRLD', 'YPW'].  
+00001150: 2020 6301 0000 0000 0000 0000 0000 0001    c.............
+00001160: 0000 0004 0000 0013 0000 00f3 0c00 0000  ................
+00001170: 7400 7c00 8800 6401 8d02 5300 a902 4ea9  t.|...d...S...N.
+00001180: 0172 5300 0000 2901 7258 0000 0072 5b00  .rS...).rX...r[.
+00001190: 0000 7266 0000 0072 5600 0000 7257 0000  ..rf...rV...rW..
+000011a0: 0072 5c00 0000 ca00 0000 f302 0000 000c  .r\.............
+000011b0: 007a 1d65 6e63 6f64 655f 6c69 7374 2e3c  .z.encode_list.<
+000011c0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000011d0: 7a10 456e 636f 6469 6e67 2074 6578 742e  z.Encoding text.
+000011e0: 2e2e 7259 0000 00e9 1027 0000 7201 0000  ..rY.....'..r...
+000011f0: 00fa 012f 2905 725a 0000 00da 0570 7269  .../).rZ.....pri
+00001200: 6e74 da09 656e 756d 6572 6174 65da 0661  nt..enumerate..a
+00001210: 7070 656e 64da 0373 7472 2909 5a0b 7374  ppend..str).Z.st
+00001220: 7269 6e67 5f6c 6973 7472 5300 0000 da07  ring_listrS.....
+00001230: 7665 7262 6f73 65da 096c 6973 745f 7369  verbose..list_si
+00001240: 7a65 da0f 7365 6c65 6374 6564 456e 636f  ze..selectedEnco
+00001250: 6465 725a 0c65 6e63 6f64 6564 5f6c 6973  derZ.encoded_lis
+00001260: 7472 0500 0000 7210 0000 00da 0373 6571  tr....r......seq
+00001270: 7256 0000 0072 6600 0000 7257 0000 00da  rV...rf...rW....
+00001280: 0b65 6e63 6f64 655f 6c69 7374 ab00 0000  .encode_list....
+00001290: 731c 0000 0008 1e0c 0104 0204 0108 0110  s...............
+000012a0: 0108 010a 0114 011c 0102 8004 0118 0104  ................
+000012b0: 0172 7200 0000 6303 0000 0000 0000 0000  .rr...c.........
+000012c0: 0000 0008 0000 0006 0000 0003 0000 0073  ...............s
+000012d0: a000 0000 7400 7c00 8301 7d03 8700 6601  ....t.|...}...f.
+000012e0: 6401 6402 8408 7d04 6700 7d05 7c02 7212  d.d...}.g.}.|.r.
+000012f0: 7401 6403 8301 0100 7402 7c00 8301 4400  t.d.....t.|...D.
+00001300: 5d29 5c02 7d06 7d07 7c06 6404 3700 7d06  ])\.}.}.|.d.7.}.
+00001310: 7c02 7236 7c06 6404 1700 6405 1600 6406  |.r6|.d...d...d.
+00001320: 6b02 7236 7401 7403 7c06 6404 1700 8301  k.r6t.t.|.d.....
+00001330: 6407 1700 7403 7c03 8301 1700 8301 0100  d...t.|.........
+00001340: 7c05 a004 7c04 7403 7c07 8301 8301 a101  |...|.t.|.......
+00001350: 0100 7116 7c02 724e 7401 7403 7c03 8301  ..q.|.rNt.t.|...
+00001360: 6407 1700 7403 7c03 8301 1700 8301 0100  d...t.|.........
+00001370: 7c05 5300 2908 611b 0300 000a 2020 2020  |.S.).a.....    
+00001380: 4465 636f 6465 7320 616c 6c20 7374 7269  Decodes all stri
+00001390: 6e67 7320 696e 2061 206c 6973 7420 7769  ngs in a list wi
+000013a0: 7468 2072 6576 6572 7365 2041 4d49 4e4f  th reverse AMINO
+000013b0: 636f 6465 2e09 0a20 2020 200a 2020 2020  code...    .    
+000013c0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+000013d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+000013e0: 7269 6e67 5f6c 6973 7420 3a20 6c69 7374  ring_list : list
+000013f0: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
+00001400: 2073 7472 696e 6720 656e 636f 6465 6420   string encoded 
+00001410: 7769 7468 2061 6d69 6e6f 636f 6465 2e0a  with aminocode..
+00001420: 2020 2020 6465 7461 696c 203a 2073 7472      detail : str
+00001430: 696e 670a 2020 2020 2020 2020 5365 7420  ing.        Set 
+00001440: 6465 7461 696c 7320 696e 2063 6f64 696e  details in codin
+00001450: 672e 2027 6427 2066 6f72 2064 6574 6169  g. 'd' for detai
+00001460: 6c73 2069 6e20 6469 6769 7473 3b20 2770  ls in digits; 'p
+00001470: 2720 666f 7220 6465 7461 696c 7320 6f6e  ' for details on
+00001480: 200a 2020 2020 2020 2020 7468 6520 7075   .        the pu
+00001490: 6e63 7475 6174 696f 6e3b 2027 6470 2720  nctuation; 'dp' 
+000014a0: 6f72 2027 7064 2720 666f 7220 626f 7468  or 'pd' for both
+000014b0: 2e20 4465 6661 756c 7420 6973 2027 6470  . Default is 'dp
+000014c0: 272e 0a20 2020 2076 6572 626f 7365 2020  '..    verbose  
+000014d0: 3a20 626f 6f6c 0a20 2020 2020 2020 2049  : bool.        I
+000014e0: 6620 5472 7565 2064 6973 706c 6179 7320  f True displays 
+000014f0: 7072 6f67 7265 7373 2e0a 0a20 2020 2052  progress...    R
+00001500: 6574 7572 6e73 0a20 2020 202d 2d2d 2d2d  eturns.    -----
+00001510: 2d2d 0a20 2020 2064 6563 6f64 6564 5f6c  --.    decoded_l
+00001520: 6973 7420 3a20 6c69 7374 206f 6620 7374  ist : list of st
+00001530: 7269 6e67 0a20 2020 2020 2020 204c 6973  ring.        Lis
+00001540: 7420 7769 7468 2061 6c6c 2064 6563 6f64  t with all decod
+00001550: 6564 2074 6578 742e 0a20 2020 2020 2020  ed text..       
+00001560: 200a 2020 2020 4578 616d 706c 650a 2020   .    Example.  
+00001570: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4465    -------.    De
+00001580: 7363 6f64 6520 7468 6520 7374 7269 6e67  scode the string
+00001590: 7320 696e 2061 206c 6973 7420 616e 6420  s in a list and 
+000015a0: 7669 6577 2074 6865 2072 6573 756c 7420  view the result 
+000015b0: 7769 7468 2061 206c 6f6f 702e 0a0a 2020  with a loop...  
+000015c0: 2020 3e3e 3e20 696d 706f 7274 2062 696f    >>> import bio
+000015d0: 7465 7874 2061 7320 6274 0a20 2020 203e  text as bt.    >
+000015e0: 3e3e 2065 6e63 6f64 6564 5f6c 6973 7420  >> encoded_list 
+000015f0: 3d20 5b27 4859 454c 4c59 5127 2c20 2759  = ['HYELLYQ', 'Y
+00001600: 5759 5152 4c44 272c 2027 5950 5727 5d0a  WYQRLD', 'YPW'].
+00001610: 2020 2020 3e3e 3e20 6465 636f 6465 645f      >>> decoded_
+00001620: 6c69 7374 203d 2062 742e 616d 696e 6f63  list = bt.aminoc
+00001630: 6f64 652e 6465 636f 6465 5f6c 6973 7428  ode.decode_list(
+00001640: 656e 636f 6465 645f 6c69 7374 2c64 6574  encoded_list,det
+00001650: 6169 6c3d 2764 7027 290a 2020 2020 3e3e  ail='dp').    >>
+00001660: 3e20 7072 696e 7428 6465 636f 6465 645f  > print(decoded_
+00001670: 6c69 7374 290a 2020 2020 5b27 6865 6c6c  list).    ['hell
+00001680: 6f27 2c20 2777 6f72 6c64 272c 2027 2127  o', 'world', '!'
+00001690: 5d0a 2020 2020 6301 0000 0000 0000 0000  ].    c.........
+000016a0: 0000 0001 0000 0004 0000 0013 0000 0072  ...............r
+000016b0: 6400 0000 7265 0000 0029 0172 6300 0000  d...re...).rc...
+000016c0: 725b 0000 0072 6600 0000 7256 0000 0072  r[...rf...rV...r
+000016d0: 5700 0000 725c 0000 00f7 0000 0072 6700  W...r\.......rg.
+000016e0: 0000 7a1d 6465 636f 6465 5f6c 6973 742e  ..z.decode_list.
+000016f0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00001700: 3e7a 1044 6563 6f64 696e 6720 7465 7874  >z.Decoding text
+00001710: 2e2e 2e72 5900 0000 7268 0000 0072 0100  ...rY...rh...r..
+00001720: 0000 7269 0000 0029 0572 5a00 0000 726a  ..ri...).rZ...rj
+00001730: 0000 0072 6b00 0000 726d 0000 0072 6c00  ...rk...rm...rl.
+00001740: 0000 2908 5a0a 696e 7075 745f 6c69 7374  ..).Z.input_list
+00001750: 7253 0000 0072 6e00 0000 726f 0000 0072  rS...rn...ro...r
+00001760: 7000 0000 5a0c 6465 636f 6465 645f 6c69  p...Z.decoded_li
+00001770: 7374 7205 0000 0072 1000 0000 7256 0000  str....r....rV..
+00001780: 0072 6600 0000 7257 0000 00da 0b64 6563  .rf...rW.....dec
+00001790: 6f64 655f 6c69 7374 d800 0000 731a 0000  ode_list....s...
+000017a0: 0008 1e0c 0104 0204 0108 0110 0108 0114  ................
+000017b0: 011c 0114 0104 0118 0104 0272 7300 0000  ...........rs...
+000017c0: 2901 7240 0000 0029 0272 4000 0000 4629  ).r@...).r@...F)
+000017d0: 0ada 075f 5f64 6f63 5f5f 7246 0000 0072  ...__doc__rF...r
+000017e0: 4400 0000 7248 0000 0072 4b00 0000 724c  D...rH...rK...rL
+000017f0: 0000 0072 5800 0000 7263 0000 0072 7200  ...rX...rc...rr.
+00001800: 0000 7273 0000 0072 5600 0000 7256 0000  ..rs...rV...rV..
+00001810: 0072 5600 0000 7257 0000 00da 083c 6d6f  .rV...rW.....<mo
+00001820: 6475 6c65 3e01 0000 0073 9200 0000 0402  dule>....s......
+00001830: 080c 0801 0202 0401 02ff 0402 02fe 0403  ................
+00001840: 02fd 0404 02fc 0405 02fb 0406 02fa 0407  ................
+00001850: 02f9 0408 02f8 0409 02f7 040a 02f6 040b  ................
+00001860: 02f5 040c 02f4 040d 02f3 040e 02f2 040f  ................
+00001870: 02f1 0410 02f0 0411 02ef 0212 0201 0201  ................
+00001880: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001890: 0201 08e3 0221 0201 0201 0201 0201 0201  .....!..........
+000018a0: 0201 0201 0201 0201 06f6 020e 0201 0201  ................
+000018b0: 0201 0201 0201 06fa 0a09 0a3a 0a29 0e2d  ...........:.).-
```

## biotext/dnabits.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Nov  8 01:34:28 2022 UTC, .py size: 5016 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,317 +1,341 @@
-00000000: 550d 0d0a 0000 0000 24b2 6963 9813 0000  U.......$.ic....
+00000000: 6f0d 0d0a 0000 0000 9b7f af64 2e15 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000020: 0003 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a03 6401 6402 6c04 5a04 6403 6404 8400  Z.d.d.l.Z.d.d...
-00000050: 5a05 6405 6406 8400 5a06 6407 6408 8400  Z.d.d...Z.d.d...
-00000060: 5a07 6409 640a 8400 5a08 6410 640c 640d  Z.d.d...Z.d.d.d.
-00000070: 8401 5a09 6411 640e 640f 8401 5a0a 6402  ..Z.d.d.d...Z.d.
-00000080: 5300 2912 7a4c 0a4c 6962 7261 7279 2077  S.).zL.Library w
-00000090: 6974 6820 6675 6e63 7469 6f6e 7320 666f  ith functions fo
-000000a0: 7220 656e 636f 6469 6e67 2061 6e64 2064  r encoding and d
-000000b0: 6563 6f64 696e 6720 7573 696e 6720 7468  ecoding using th
-000000c0: 6520 444e 4162 6974 7320 6d65 7468 6f64  e DNAbits method
-000000d0: 2e0a e900 0000 004e 6301 0000 0000 0000  .......Nc.......
-000000e0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-000000f0: 0073 4800 0000 6401 7d01 7c00 4400 5d3a  .sH...d.}.|.D.]:
-00000100: 7d02 7400 7401 7c02 8301 8301 6402 6400  }.t.t.|.....d.d.
-00000110: 8502 1900 7d03 6403 7402 7c03 8301 1600  ....}.d.t.|.....
-00000120: 7d03 7c03 6400 6400 6404 8503 1900 7d03  }.|.d.d.d.....}.
-00000130: 7c01 7c03 3700 7d01 7108 7c01 5300 2905  |.|.7.}.q.|.S.).
-00000140: 4eda 00e9 0200 0000 7a04 2530 3864 e9ff  N.......z.%08d..
-00000150: ffff ff29 03da 0362 696e da03 6f72 64da  ...)...bin..ord.
-00000160: 0369 6e74 2904 da06 7374 7269 6e67 da03  .int)...string..
-00000170: 7265 73da 0463 6861 72da 0374 6d70 a900  res..char..tmp..
-00000180: 720c 0000 00fa 2c62 7569 6c64 5c62 6469  r.....,build\bdi
-00000190: 7374 2e77 696e 2d61 6d64 3634 5c65 6767  st.win-amd64\egg
-000001a0: 5c62 696f 7465 7874 5c64 6e61 6269 7473  \biotext\dnabits
-000001b0: 2e70 79da 0a73 7472 5f74 6f5f 6269 6e0a  .py..str_to_bin.
-000001c0: 0000 0073 0e00 0000 0001 0401 0801 1401  ...s............
-000001d0: 0c01 0e01 0a01 720e 0000 0063 0100 0000  ......r....c....
-000001e0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-000001f0: 4300 0000 735e 0000 0064 017d 0174 0074  C...s^...d.}.t.t
-00000200: 0174 027c 0083 0164 021b 0083 0183 0144  .t.|...d.......D
-00000210: 005d 407d 027c 007c 0264 0214 007c 0264  .]@}.|.|.d...|.d
-00000220: 0317 0064 0214 0085 0219 007d 037c 0364  ...d.......}.|.d
-00000230: 0064 0064 0485 0319 007d 0374 0374 017c  .d.d.....}.t.t.|
-00000240: 0364 0583 0283 017d 047c 017c 0437 007d  .d.....}.|.|.7.}
-00000250: 0171 187c 0153 0029 064e 7202 0000 00e9  .q.|.S.).Nr.....
-00000260: 0800 0000 e901 0000 0072 0400 0000 7203  .........r....r.
-00000270: 0000 0029 04da 0572 616e 6765 7207 0000  ...)...ranger...
-00000280: 00da 036c 656e da03 6368 7229 0572 0800  ...len..chr).r..
-00000290: 0000 7209 0000 00da 0369 6478 5a04 6373  ..r......idxZ.cs
-000002a0: 7472 720b 0000 0072 0c00 0000 720c 0000  trr....r....r...
-000002b0: 0072 0d00 0000 da0a 6269 6e5f 746f 5f73  .r......bin_to_s
-000002c0: 7472 1200 0000 730e 0000 0000 0104 0118  tr....s.........
-000002d0: 0118 010e 010e 010a 0172 1500 0000 6301  .........r....c.
-000002e0: 0000 0000 0000 0000 0000 0005 0000 0007  ................
-000002f0: 0000 0043 0000 0073 c200 0000 7400 7c00  ...C...s....t.|.
-00000300: 8301 7d00 7401 a002 6401 7c00 6402 7403  ..}.t...d.|.d.t.
-00000310: 7c00 8301 6403 1800 6404 8503 1900 a102  |...d...d.......
-00000320: 7d01 7401 a002 6401 7c00 6403 7403 7c00  }.t...d.|.d.t.|.
-00000330: 8301 6404 8503 1900 a102 7d02 7404 a005  ..d.......}.t...
-00000340: 7404 a006 7c01 7c02 6702 a101 a101 7d03  t...|.|.g.....}.
-00000350: 7c03 a007 7408 a101 7d03 7c03 6403 6404  |...t...}.|.d.d.
-00000360: 6702 1400 7d03 7404 a009 7c03 6403 a102  g...}.t...|.d...
-00000370: 7d03 7c03 a007 740a a101 7d03 6405 7c03  }.|...t...}.d.|.
-00000380: 7c03 6406 6b02 3c00 6407 7c03 7c03 6408  |.d.k.<.d.|.|.d.
-00000390: 6b02 3c00 6409 7c03 7c03 640a 6b02 3c00  k.<.d.|.|.d.k.<.
-000003a0: 640b 7c03 7c03 640c 6b02 3c00 640d a00b  d.|.|.d.k.<.d...
-000003b0: 7c03 a101 7d03 7c03 7d04 7c04 5300 290e  |...}.|.}.|.S.).
-000003c0: 61fb 0100 000a 2020 2020 456e 636f 6465  a.....    Encode
-000003d0: 7320 6120 7374 7269 6e67 2077 6974 6820  s a string with 
-000003e0: 444e 4162 6974 732e 0a20 2020 200a 2020  DNAbits..    .  
-000003f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000400: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000410: 696e 7075 745f 7374 7269 6e67 203a 2073  input_string : s
-00000420: 7472 696e 670a 2020 2020 2020 2020 4e61  tring.        Na
-00000430: 7475 7261 6c20 6c61 6e67 7561 6765 2074  tural language t
-00000440: 6578 7420 7374 7269 6e67 2074 6f20 6265  ext string to be
-00000450: 2065 6e63 6f64 6564 2e0a 2020 2020 2020   encoded..      
-00000460: 2020 0a20 2020 204f 7574 7075 740a 2020    .    Output.  
-00000470: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065    --------.    e
-00000480: 6e63 6f64 6564 5f73 7472 696e 6720 3a20  ncoded_string : 
-00000490: 7374 7269 6e67 0a20 2020 2020 2020 2045  string.        E
-000004a0: 6e63 6f64 6564 2074 6578 742e 0a20 2020  ncoded text..   
-000004b0: 2020 2020 200a 2020 2020 4578 616d 706c       .    Exampl
-000004c0: 650a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  e.    --------. 
-000004d0: 2020 2045 6e63 6f6e 6465 2061 2073 7472     Enconde a str
-000004e0: 696e 672e 0a0a 2020 2020 3e3e 3e20 696d  ing...    >>> im
-000004f0: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
-00000500: 6274 0a20 2020 203e 3e3e 2069 6e70 7574  bt.    >>> input
-00000510: 5f73 7472 696e 6720 3d20 2248 656c 6c6f  _string = "Hello
-00000520: 2077 6f72 6c64 2122 0a20 2020 203e 3e3e   world!".    >>>
-00000530: 2065 6e63 6f64 6564 5f73 7472 696e 6720   encoded_string 
-00000540: 3d20 6274 2e64 6e61 6269 7473 2e65 6e63  = bt.dnabits.enc
-00000550: 6f64 655f 7374 7269 6e67 2869 6e70 7574  ode_string(input
-00000560: 5f73 7472 696e 6729 0a20 2020 203e 3e3e  _string).    >>>
-00000570: 2070 7269 6e74 2865 6e63 6f64 6564 5f73   print(encoded_s
-00000580: 7472 696e 6729 0a20 2020 2041 4741 4343  tring).    AGACC
-00000590: 4347 4341 5447 4341 5447 4354 5447 4341  CGCATGCATGCTTGCA
-000005a0: 4147 4154 4354 4354 5447 4347 4154 4341  AGATCTCTTGCGATCA
-000005b0: 5447 4341 4347 4343 4147 410a 2020 2020  TGCACGCCAGA.    
-000005c0: da01 2e72 0100 0000 7210 0000 0072 0300  ...r....r....r..
-000005d0: 0000 da01 41da 0130 da01 43da 0131 da01  ....A..0..C..1..
-000005e0: 47da 0132 da01 54da 0133 7202 0000 0029  G..2..T..3r....)
-000005f0: 0c72 0e00 0000 da02 7265 da07 6669 6e64  .r......re..find
-00000600: 616c 6c72 1200 0000 da02 6e70 5a09 7472  allr......npZ.tr
-00000610: 616e 7370 6f73 65da 0561 7272 6179 da06  anspose..array..
-00000620: 6173 7479 7065 7207 0000 00da 0373 756d  astyper......sum
-00000630: da03 7374 72da 046a 6f69 6e29 05da 0c69  ..str..join)...i
-00000640: 6e70 7574 5f73 7472 696e 675a 0674 6578  nput_stringZ.tex
-00000650: 745f 305a 0674 6578 745f 31da 0474 6578  t_0Z.text_1..tex
-00000660: 74da 0e65 6e63 6f64 6564 5f73 7472 696e  t..encoded_strin
-00000670: 6772 0c00 0000 720c 0000 0072 0d00 0000  gr....r....r....
-00000680: da0d 656e 636f 6465 5f73 7472 696e 671b  ..encode_string.
-00000690: 0000 0073 1e00 0000 0019 0801 1e01 1a01  ...s............
-000006a0: 1401 0a01 0c01 0c01 0a01 0c01 0c01 0c01  ................
-000006b0: 0c01 0a01 0401 722a 0000 0063 0100 0000  ......r*...c....
-000006c0: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-000006d0: 4300 0000 7394 0000 0074 00a0 0174 027c  C...s....t...t.|
-000006e0: 0083 0164 0166 02a1 01a0 0374 04a1 017d  ...d.f.....t...}
-000006f0: 0174 00a0 0574 06a0 0764 027c 00a1 02a1  .t...t...d.|....
-00000700: 017d 0264 0364 0367 027c 017c 0264 046b  .}.d.d.g.|.|.d.k
-00000710: 023c 0064 0564 0367 027c 017c 0264 066b  .<.d.d.g.|.|.d.k
-00000720: 023c 0064 0364 0567 027c 017c 0264 076b  .<.d.d.g.|.|.d.k
-00000730: 023c 0064 0564 0567 027c 017c 0264 086b  .<.d.d.g.|.|.d.k
-00000740: 023c 007c 01a0 0374 08a1 017d 0164 09a0  .<.|...t...}.d..
-00000750: 0974 00a0 0a7c 01a1 01a1 017d 0174 0b7c  .t...|.....}.t.|
-00000760: 0183 017d 017c 017d 037c 0353 0029 0a61  ...}.|.}.|.S.).a
-00000770: f601 0000 0a20 2020 2044 6563 6f64 6573  .....    Decodes
-00000780: 2061 2073 7472 696e 6720 7769 7468 2044   a string with D
-00000790: 4e41 6269 7473 2072 6576 6572 7365 2e09  NAbits reverse..
-000007a0: 0a20 2020 200a 2020 2020 5061 7261 6d65  .    .    Parame
-000007b0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-000007c0: 2d2d 2d0a 2020 2020 696e 7075 745f 7374  ---.    input_st
-000007d0: 7269 6e67 203a 2073 7472 696e 670a 2020  ring : string.  
-000007e0: 2020 2020 2020 5465 7874 2073 7472 696e        Text strin
-000007f0: 6720 656e 636f 6465 6420 7769 7468 2044  g encoded with D
-00000800: 4e41 6269 7473 2e0a 0a20 2020 204f 7574  NAbits...    Out
-00000810: 7075 740a 2020 2020 2d2d 2d2d 2d2d 2d2d  put.    --------
-00000820: 0a20 2020 2064 6563 6f64 6564 5f73 7472  .    decoded_str
-00000830: 696e 6720 3a20 7374 7269 6e67 0a20 2020  ing : string.   
-00000840: 2020 2020 2044 6563 6f64 6564 2074 6578       Decoded tex
-00000850: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-00000860: 4578 616d 706c 650a 2020 2020 2d2d 2d2d  Example.    ----
-00000870: 2d2d 2d2d 0a20 2020 2044 6563 6f6e 6465  ----.    Deconde
-00000880: 2061 2073 7472 696e 672e 0a0a 2020 2020   a string...    
-00000890: 3e3e 3e20 696d 706f 7274 2062 696f 7465  >>> import biote
-000008a0: 7874 2061 7320 6274 0a20 2020 203e 3e3e  xt as bt.    >>>
-000008b0: 2065 6e63 6f64 6564 5f73 7472 696e 6720   encoded_string 
-000008c0: 3d20 2241 4741 4343 4347 4341 5447 4341  = "AGACCCGCATGCA
-000008d0: 5447 4354 5447 4341 4147 4154 4354 4354  TGCTTGCAAGATCTCT
-000008e0: 5447 4347 4154 4341 5447 4341 4347 4343  TGCGATCATGCACGCC
-000008f0: 4147 4122 0a20 2020 203e 3e3e 2064 6563  AGA".    >>> dec
-00000900: 6f64 6564 5f73 7472 696e 6720 3d20 6274  oded_string = bt
-00000910: 2e64 6e61 6269 7473 2e64 6563 6f64 655f  .dnabits.decode_
-00000920: 7374 7269 6e67 2865 6e63 6f64 6564 5f73  string(encoded_s
-00000930: 7472 696e 6729 0a20 2020 203e 3e3e 2070  tring).    >>> p
-00000940: 7269 6e74 2864 6563 6f64 6564 5f73 7472  rint(decoded_str
-00000950: 696e 6729 0a20 2020 2048 656c 6c6f 2077  ing).    Hello w
-00000960: 6f72 6c64 210a 2020 2020 7203 0000 0072  orld!.    r....r
-00000970: 1600 0000 7201 0000 0072 1700 0000 7210  ....r....r....r.
-00000980: 0000 0072 1900 0000 721b 0000 0072 1d00  ...r....r....r..
-00000990: 0000 7202 0000 0029 0c72 2100 0000 da05  ..r....).r!.....
-000009a0: 7a65 726f 7372 1200 0000 7223 0000 0072  zerosr....r#...r
-000009b0: 0700 0000 7222 0000 0072 1f00 0000 7220  ....r"...r....r 
-000009c0: 0000 0072 2500 0000 7226 0000 005a 0b63  ...r%...r&...Z.c
-000009d0: 6f6e 6361 7465 6e61 7465 7215 0000 0029  oncatenater....)
-000009e0: 0472 2700 0000 7228 0000 005a 0364 6e61  .r'...r(...Z.dna
-000009f0: da0e 6465 636f 6465 645f 7374 7269 6e67  ..decoded_string
-00000a00: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000a10: 0d64 6563 6f64 655f 7374 7269 6e67 4400  .decode_stringD.
-00000a20: 0000 7316 0000 0000 1918 0112 0110 0110  ..s.............
-00000a30: 0110 0110 010a 0110 0108 0104 0172 2d00  .............r-.
-00000a40: 0000 4663 0200 0000 0000 0000 0000 0000  ..Fc............
-00000a50: 0800 0000 0500 0000 4300 0000 7394 0000  ........C...s...
-00000a60: 0074 007c 0083 017d 0264 0164 0284 007d  .t.|...}.d.d...}
-00000a70: 0367 007d 047c 0172 2074 0164 0383 0101  .g.}.|.r t.d....
-00000a80: 0074 027c 0083 0144 005d 4a5c 027d 057d  .t.|...D.]J\.}.}
-00000a90: 067c 037c 0683 017d 077c 04a0 037c 07a1  .|.|...}.|...|..
-00000aa0: 0101 007c 0172 287c 0564 0417 0064 0516  ...|.r(|.d...d..
-00000ab0: 0064 066b 0272 2874 0174 047c 0564 0417  .d.k.r(t.t.|.d..
-00000ac0: 0083 0164 0717 0074 047c 0283 0117 0083  ...d...t.|......
-00000ad0: 0101 0071 287c 0172 9074 0174 047c 0283  ...q(|.r.t.t.|..
-00000ae0: 0164 0717 0074 047c 0283 0117 0083 0101  .d...t.|........
-00000af0: 007c 0453 0029 0861 7b02 0000 0a20 2020  .|.S.).a{....   
-00000b00: 2045 6e63 6f64 6573 2061 6c6c 2073 7472   Encodes all str
-00000b10: 696e 6773 2069 6e20 6120 6c69 7374 2077  ings in a list w
-00000b20: 6974 6820 444e 4162 6974 732e 090a 2020  ith DNAbits...  
-00000b30: 2020 0a20 2020 2050 6172 616d 6574 6572    .    Parameter
-00000b40: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00000b50: 0a20 2020 2073 7472 696e 675f 6c69 7374  .    string_list
-00000b60: 203a 206c 6973 740a 2020 2020 2020 2020   : list.        
-00000b70: 4c69 7374 206f 6620 7374 7269 6e67 2074  List of string t
-00000b80: 6f20 6265 2065 6e63 6f64 6564 2e0a 2020  o be encoded..  
-00000b90: 2020 7665 7262 6f73 6520 203a 2062 6f6f    verbose  : boo
-00000ba0: 6c0a 2020 2020 2020 2020 4966 2054 7275  l.        If Tru
-00000bb0: 6520 6469 7370 6c61 7973 2070 726f 6772  e displays progr
-00000bc0: 6573 732e 0a0a 2020 2020 4f75 7470 7574  ess...    Output
-00000bd0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00000be0: 2020 656e 636f 6465 645f 6c69 7374 203a    encoded_list :
-00000bf0: 206c 6973 740a 2020 2020 2020 2020 4c69   list.        Li
-00000c00: 7374 2077 6974 6820 616c 6c20 656e 636f  st with all enco
-00000c10: 6465 6420 7465 7874 2069 6e20 7374 7269  ded text in stri
-00000c20: 6e67 2066 6f72 6d61 742e 0a20 2020 2020  ng format..     
-00000c30: 2020 200a 2020 2020 4578 616d 706c 650a     .    Example.
-00000c40: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
-00000c50: 2045 6e63 6f64 6520 7468 6520 7374 7269   Encode the stri
-00000c60: 6e67 7320 696e 2061 206c 6973 7420 616e  ngs in a list an
-00000c70: 6420 7669 6577 2074 6865 2072 6573 756c  d view the resul
-00000c80: 7420 6f66 2074 6865 2066 6972 7374 2069  t of the first i
-00000c90: 7465 6d2e 0a0a 2020 2020 3e3e 3e20 696d  tem...    >>> im
-00000ca0: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
-00000cb0: 6274 0a20 2020 203e 3e3e 2073 7472 696e  bt.    >>> strin
-00000cc0: 675f 6c69 7374 203d 205b 2748 656c 6c6f  g_list = ['Hello
-00000cd0: 272c 2777 6f72 6c64 272c 2721 275d 0a20  ','world','!']. 
-00000ce0: 2020 203e 3e3e 2065 6e63 6f64 6564 5f6c     >>> encoded_l
-00000cf0: 6973 7420 3d20 6274 2e64 6e61 6269 7473  ist = bt.dnabits
-00000d00: 2e65 6e63 6f64 655f 6c69 7374 2873 7472  .encode_list(str
-00000d10: 696e 675f 6c69 7374 290a 2020 2020 3e3e  ing_list).    >>
-00000d20: 3e20 7072 696e 7428 656e 636f 6465 645f  > print(encoded_
-00000d30: 6c69 7374 290a 2020 2020 5b27 4147 4143  list).    ['AGAC
-00000d40: 4343 4743 4154 4743 4154 4743 5454 4743  CCGCATGCATGCTTGC
-00000d50: 272c 2027 5443 5443 5454 4743 4741 5443  ', 'TCTCTTGCGATC
-00000d60: 4154 4743 4143 4743 272c 2027 4341 4741  ATGCACGC', 'CAGA
-00000d70: 275d 0a20 2020 2063 0100 0000 0000 0000  '].    c........
-00000d80: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00000d90: 7308 0000 0074 007c 0083 0153 00a9 014e  s....t.|...S...N
-00000da0: 2901 722a 0000 00a9 01da 0178 720c 0000  ).r*.......xr...
-00000db0: 0072 0c00 0000 720d 0000 00da 083c 6c61  .r....r......<la
-00000dc0: 6d62 6461 3e85 0000 00f3 0000 0000 7a1d  mbda>.........z.
-00000dd0: 656e 636f 6465 5f6c 6973 742e 3c6c 6f63  encode_list.<loc
-00000de0: 616c 733e 2e3c 6c61 6d62 6461 3e7a 1045  als>.<lambda>z.E
-00000df0: 6e63 6f64 696e 6720 7465 7874 2e2e 2e72  ncoding text...r
-00000e00: 1000 0000 e910 2700 0072 0100 0000 fa01  ......'..r......
-00000e10: 2f29 0572 1200 0000 da05 7072 696e 74da  /).r......print.
-00000e20: 0965 6e75 6d65 7261 7465 da06 6170 7065  .enumerate..appe
-00000e30: 6e64 7225 0000 0029 085a 0b73 7472 696e  ndr%...).Z.strin
-00000e40: 675f 6c69 7374 da07 7665 7262 6f73 65da  g_list..verbose.
-00000e50: 096c 6973 745f 7369 7a65 da0f 7365 6c65  .list_size..sele
-00000e60: 6374 6564 456e 636f 6465 725a 0c65 6e63  ctedEncoderZ.enc
-00000e70: 6f64 6564 5f6c 6973 74da 0163 da01 69da  oded_list..c..i.
-00000e80: 0373 6571 720c 0000 0072 0c00 0000 720d  .seqr....r....r.
-00000e90: 0000 00da 0b65 6e63 6f64 655f 6c69 7374  .....encode_list
-00000ea0: 6900 0000 731a 0000 0000 1b08 0108 0204  i...s...........
-00000eb0: 0104 0108 0110 0108 010a 0114 011e 0104  ................
-00000ec0: 0118 0172 3e00 0000 6303 0000 0000 0000  ...r>...c.......
-00000ed0: 0000 0000 0008 0000 0006 0000 0043 0000  .............C..
-00000ee0: 0073 9c00 0000 7400 7c00 8301 7d03 6401  .s....t.|...}.d.
-00000ef0: 6402 8400 7d04 6700 7d05 7c02 7220 7401  d...}.g.}.|.r t.
-00000f00: 6403 8301 0100 7402 7c00 8301 4400 5d52  d.....t.|...D.]R
-00000f10: 5c02 7d06 7d07 7c06 6404 3700 7d06 7c02  \.}.}.|.d.7.}.|.
-00000f20: 7268 7c06 6404 1700 6405 1600 6406 6b02  rh|.d...d...d.k.
-00000f30: 7268 7401 7403 7c06 6404 1700 8301 6407  rht.t.|.d.....d.
-00000f40: 1700 7403 7c03 8301 1700 8301 0100 7c05  ..t.|.........|.
-00000f50: a004 7c04 7403 7c07 8301 8301 a101 0100  ..|.t.|.........
-00000f60: 7128 7c02 7298 7401 7403 7c03 8301 6407  q(|.r.t.t.|...d.
-00000f70: 1700 7403 7c03 8301 1700 8301 0100 7c05  ..t.|.........|.
-00000f80: 5300 2908 6182 0200 000a 2020 2020 4465  S.).a.....    De
-00000f90: 636f 6465 7320 616c 6c20 7374 7269 6e67  codes all string
-00000fa0: 7320 696e 2061 206c 6973 7420 7769 7468  s in a list with
-00000fb0: 2072 6576 6572 7365 2044 4e41 6269 7473   reverse DNAbits
-00000fc0: 2e09 0a20 2020 200a 2020 2020 5061 7261  ...    .    Para
-00000fd0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00000fe0: 2d2d 2d2d 2d0a 2020 2020 7374 7269 6e67  -----.    string
-00000ff0: 5f6c 6973 7420 3a20 6c69 7374 0a20 2020  _list : list.   
-00001000: 2020 2020 204c 6973 7420 6f66 2073 7472       List of str
-00001010: 696e 6720 656e 636f 6465 6420 7769 7468  ing encoded with
-00001020: 2044 4e41 6269 7473 2e0a 2020 2020 7665   DNAbits..    ve
-00001030: 7262 6f73 6520 203a 2062 6f6f 6c0a 2020  rbose  : bool.  
-00001040: 2020 2020 2020 4966 2054 7275 6520 6469        If True di
-00001050: 7370 6c61 7973 2070 726f 6772 6573 732e  splays progress.
-00001060: 0a0a 2020 2020 4f75 7470 7574 0a20 2020  ..    Output.   
-00001070: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 6465   --------.    de
-00001080: 636f 6465 645f 6c69 7374 203a 206c 6973  coded_list : lis
-00001090: 7420 6f66 2073 7472 696e 670a 2020 2020  t of string.    
-000010a0: 2020 2020 4c69 7374 2077 6974 6820 616c      List with al
-000010b0: 6c20 6465 636f 6465 6420 7465 7874 2e0a  l decoded text..
-000010c0: 2020 2020 2020 2020 0a20 2020 2045 7861          .    Exa
-000010d0: 6d70 6c65 0a20 2020 202d 2d2d 2d2d 2d2d  mple.    -------
-000010e0: 2d0a 2020 2020 4465 7363 6f64 6520 7468  -.    Descode th
-000010f0: 6520 7374 7269 6e67 7320 696e 2061 206c  e strings in a l
-00001100: 6973 7420 616e 6420 7669 6577 2074 6865  ist and view the
-00001110: 2072 6573 756c 7420 7769 7468 2061 206c   result with a l
-00001120: 6f6f 702e 0a0a 2020 2020 3e3e 3e20 696d  oop...    >>> im
-00001130: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
-00001140: 6274 0a20 2020 203e 3e3e 2065 6e63 6f64  bt.    >>> encod
-00001150: 6564 5f6c 6973 7420 3d20 5b27 4147 4143  ed_list = ['AGAC
-00001160: 4343 4743 4154 4743 4154 4743 5454 4743  CCGCATGCATGCTTGC
-00001170: 272c 2027 5443 5443 5454 4743 4741 5443  ', 'TCTCTTGCGATC
-00001180: 4154 4743 4143 4743 272c 2027 4341 4741  ATGCACGC', 'CAGA
-00001190: 275d 0a20 2020 203e 3e3e 2064 6563 6f64  '].    >>> decod
-000011a0: 6564 5f6c 6973 7420 3d20 6274 2e64 6e61  ed_list = bt.dna
-000011b0: 6269 7473 2e64 6563 6f64 655f 6c69 7374  bits.decode_list
-000011c0: 2865 6e63 6f64 6564 5f6c 6973 7429 0a20  (encoded_list). 
-000011d0: 2020 203e 3e3e 2070 7269 6e74 2864 6563     >>> print(dec
-000011e0: 6f64 6564 5f6c 6973 7429 0a20 2020 205b  oded_list).    [
-000011f0: 2748 656c 6c6f 272c 2027 776f 726c 6427  'Hello', 'world'
-00001200: 2c20 2721 275d 0a20 2020 2063 0100 0000  , '!'].    c....
-00001210: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001220: 5300 0000 7308 0000 0074 007c 0083 0153  S...s....t.|...S
-00001230: 0072 2e00 0000 2901 722d 0000 0072 2f00  .r....).r-...r/.
-00001240: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00001250: 0072 3100 0000 af00 0000 7232 0000 007a  .r1.......r2...z
-00001260: 1d64 6563 6f64 655f 6c69 7374 2e3c 6c6f  .decode_list.<lo
-00001270: 6361 6c73 3e2e 3c6c 616d 6264 613e 7a10  cals>.<lambda>z.
-00001280: 4465 636f 6469 6e67 2074 6578 742e 2e2e  Decoding text...
-00001290: 7210 0000 0072 3300 0000 7201 0000 0072  r....r3...r....r
-000012a0: 3400 0000 2905 7212 0000 0072 3500 0000  4...).r....r5...
-000012b0: 7236 0000 0072 2500 0000 7237 0000 0029  r6...r%...r7...)
-000012c0: 085a 0a69 6e70 7574 5f6c 6973 74da 0b6f  .Z.input_list..o
-000012d0: 7574 7075 745f 6669 6c65 7238 0000 0072  utput_filer8...r
-000012e0: 3900 0000 723a 0000 005a 0c64 6563 6f64  9...r:...Z.decod
-000012f0: 6564 5f6c 6973 7472 3b00 0000 723c 0000  ed_listr;...r<..
-00001300: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00001310: da0b 6465 636f 6465 5f6c 6973 7493 0000  ..decode_list...
-00001320: 0073 1a00 0000 001b 0801 0802 0401 0401  .s..............
-00001330: 0801 1001 0801 1401 1c01 1401 0401 1802  ................
-00001340: 7240 0000 0029 0146 2902 4e46 290b da07  r@...).F).NF)...
-00001350: 5f5f 646f 635f 5f72 1f00 0000 da05 6e75  __doc__r......nu
-00001360: 6d70 7972 2100 0000 da08 7761 726e 696e  mpyr!.....warnin
-00001370: 6773 720e 0000 0072 1500 0000 722a 0000  gsr....r....r*..
-00001380: 0072 2d00 0000 723e 0000 0072 4000 0000  .r-...r>...r@...
-00001390: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-000013a0: 0d00 0000 da08 3c6d 6f64 756c 653e 0300  ......<module>..
-000013b0: 0000 7312 0000 0004 0308 0108 0108 0208  ..s.............
-000013c0: 0808 0908 2908 250a 2a                   ....).%.*
+00000040: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
+00000050: 5a05 6410 6408 6409 8401 5a06 6411 640a  Z.d.d.d...Z.d.d.
+00000060: 640b 8401 5a07 640c 640d 8400 5a08 640e  d...Z.d.d...Z.d.
+00000070: 640f 8400 5a09 6402 5300 2912 61eb 0100  d...Z.d.S.).a...
+00000080: 000a 5468 6973 206d 6f64 756c 6520 7072  ..This module pr
+00000090: 6f76 6964 6573 2066 756e 6374 696f 6e73  ovides functions
+000000a0: 2066 6f72 2065 6e63 6f64 696e 6720 616e   for encoding an
+000000b0: 6420 6465 636f 6469 6e67 2074 6578 7420  d decoding text 
+000000c0: 7573 696e 6720 444e 4162 6974 732e 0a0a  using DNAbits...
+000000d0: 4675 6e63 7469 6f6e 733a 0a2d 2065 6e63  Functions:.- enc
+000000e0: 6f64 655f 7374 7269 6e67 3a20 456e 636f  ode_string: Enco
+000000f0: 6465 7320 6120 7374 7269 6e67 2075 7369  des a string usi
+00000100: 6e67 2044 4e41 6269 7473 2e0a 2d20 6465  ng DNAbits..- de
+00000110: 636f 6465 5f73 7472 696e 673a 2044 6563  code_string: Dec
+00000120: 6f64 6573 2061 2073 7472 696e 6720 656e  odes a string en
+00000130: 636f 6465 6420 7769 7468 2044 4e41 6269  coded with DNAbi
+00000140: 7473 2e0a 2d20 656e 636f 6465 5f6c 6973  ts..- encode_lis
+00000150: 743a 2045 6e63 6f64 6573 2061 6c6c 2073  t: Encodes all s
+00000160: 7472 696e 6773 2069 6e20 6120 6c69 7374  trings in a list
+00000170: 2075 7369 6e67 2044 4e41 6269 7473 2e0a   using DNAbits..
+00000180: 2d20 6465 636f 6465 5f6c 6973 743a 2044  - decode_list: D
+00000190: 6563 6f64 6573 2061 6c6c 2073 7472 696e  ecodes all strin
+000001a0: 6773 2069 6e20 6120 6c69 7374 2065 6e63  gs in a list enc
+000001b0: 6f64 6564 2077 6974 6820 444e 4162 6974  oded with DNAbit
+000001c0: 732e 0a2d 2073 7472 5f74 6f5f 6269 6e3a  s..- str_to_bin:
+000001d0: 2043 6f6e 7665 7274 7320 6120 7374 7269   Converts a stri
+000001e0: 6e67 2074 6f20 6120 6269 6e61 7279 2072  ng to a binary r
+000001f0: 6570 7265 7365 6e74 6174 696f 6e2e 0a2d  epresentation..-
+00000200: 2062 696e 5f74 6f5f 7374 723a 2043 6f6e   bin_to_str: Con
+00000210: 7665 7274 7320 6120 6269 6e61 7279 2072  verts a binary r
+00000220: 6570 7265 7365 6e74 6174 696f 6e20 746f  epresentation to
+00000230: 2061 2073 7472 696e 672e 0a0a 4175 7468   a string...Auth
+00000240: 6f72 3a20 4469 6f67 6f20 6465 204a 2e20  or: Diogo de J. 
+00000250: 532e 204d 6163 6861 646f 0a44 6174 653a  S. Machado.Date:
+00000260: 2031 332f 3037 2f32 3032 330a e900 0000   13/07/2023.....
+00000270: 004e 6301 0000 0000 0000 0000 0000 0005  .Nc.............
+00000280: 0000 0007 0000 0043 0000 0073 c200 0000  .......C...s....
+00000290: 7400 7c00 8301 7d00 7401 a002 6401 7c00  t.|...}.t...d.|.
+000002a0: 6402 7403 7c00 8301 6403 1800 6404 8503  d.t.|...d...d...
+000002b0: 1900 a102 7d01 7401 a002 6401 7c00 6403  ....}.t...d.|.d.
+000002c0: 7403 7c00 8301 6404 8503 1900 a102 7d02  t.|...d.......}.
+000002d0: 7404 a005 7404 a006 7c01 7c02 6702 a101  t...t...|.|.g...
+000002e0: a101 7d03 7c03 a007 7408 a101 7d03 7c03  ..}.|...t...}.|.
+000002f0: 6403 6404 6702 1400 7d03 7404 a009 7c03  d.d.g...}.t...|.
+00000300: 6403 a102 7d03 7c03 a007 740a a101 7d03  d...}.|...t...}.
+00000310: 6405 7c03 7c03 6406 6b02 3c00 6407 7c03  d.|.|.d.k.<.d.|.
+00000320: 7c03 6408 6b02 3c00 6409 7c03 7c03 640a  |.d.k.<.d.|.|.d.
+00000330: 6b02 3c00 640b 7c03 7c03 640c 6b02 3c00  k.<.d.|.|.d.k.<.
+00000340: 640d a00b 7c03 a101 7d03 7c03 7d04 7c04  d...|...}.|.}.|.
+00000350: 5300 290e 61f9 0100 000a 2020 2020 456e  S.).a.....    En
+00000360: 636f 6465 7320 6120 7374 7269 6e67 2077  codes a string w
+00000370: 6974 6820 444e 4162 6974 732e 0a20 2020  ith DNAbits..   
+00000380: 200a 2020 2020 5061 7261 6d65 7465 7273   .    Parameters
+00000390: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+000003a0: 2020 2020 696e 7075 745f 7374 7269 6e67      input_string
+000003b0: 203a 2073 7472 696e 670a 2020 2020 2020   : string.      
+000003c0: 2020 4e61 7475 7261 6c20 6c61 6e67 7561    Natural langua
+000003d0: 6765 2074 6578 7420 7374 7269 6e67 2074  ge text string t
+000003e0: 6f20 6265 2065 6e63 6f64 6564 2e0a 2020  o be encoded..  
+000003f0: 2020 2020 2020 0a20 2020 2052 6574 7572        .    Retur
+00000400: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00000410: 2020 2065 6e63 6f64 6564 5f73 7472 696e     encoded_strin
+00000420: 6720 3a20 7374 7269 6e67 0a20 2020 2020  g : string.     
+00000430: 2020 2045 6e63 6f64 6564 2074 6578 742e     Encoded text.
+00000440: 0a20 2020 2020 2020 200a 2020 2020 4578  .        .    Ex
+00000450: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
+00000460: 2d0a 2020 2020 456e 636f 6465 2061 2073  -.    Encode a s
+00000470: 7472 696e 672e 0a0a 2020 2020 3e3e 3e20  tring...    >>> 
+00000480: 696d 706f 7274 2062 696f 7465 7874 2061  import biotext a
+00000490: 7320 6274 0a20 2020 203e 3e3e 2069 6e70  s bt.    >>> inp
+000004a0: 7574 5f73 7472 696e 6720 3d20 2248 656c  ut_string = "Hel
+000004b0: 6c6f 2077 6f72 6c64 2122 0a20 2020 203e  lo world!".    >
+000004c0: 3e3e 2065 6e63 6f64 6564 5f73 7472 696e  >> encoded_strin
+000004d0: 6720 3d20 6274 2e64 6e61 6269 7473 2e65  g = bt.dnabits.e
+000004e0: 6e63 6f64 655f 7374 7269 6e67 2869 6e70  ncode_string(inp
+000004f0: 7574 5f73 7472 696e 6729 0a20 2020 203e  ut_string).    >
+00000500: 3e3e 2070 7269 6e74 2865 6e63 6f64 6564  >> print(encoded
+00000510: 5f73 7472 696e 6729 0a20 2020 2041 4741  _string).    AGA
+00000520: 4343 4347 4341 5447 4341 5447 4354 5447  CCCGCATGCATGCTTG
+00000530: 4341 4147 4154 4354 4354 5447 4347 4154  CAAGATCTCTTGCGAT
+00000540: 4341 5447 4341 4347 4343 4147 410a 2020  CATGCACGCCAGA.  
+00000550: 2020 da01 2e72 0100 0000 e901 0000 00e9    ...r..........
+00000560: 0200 0000 da01 41da 0130 da01 43da 0131  ......A..0..C..1
+00000570: da01 47da 0132 da01 54da 0133 da00 290c  ..G..2..T..3..).
+00000580: da0a 7374 725f 746f 5f62 696e da02 7265  ..str_to_bin..re
+00000590: da07 6669 6e64 616c 6cda 036c 656e da02  ..findall..len..
+000005a0: 6e70 5a09 7472 616e 7370 6f73 65da 0561  npZ.transpose..a
+000005b0: 7272 6179 da06 6173 7479 7065 da03 696e  rray..astype..in
+000005c0: 74da 0373 756d da03 7374 72da 046a 6f69  t..sum..str..joi
+000005d0: 6e29 05da 0c69 6e70 7574 5f73 7472 696e  n)...input_strin
+000005e0: 675a 0674 6578 745f 305a 0674 6578 745f  gZ.text_0Z.text_
+000005f0: 31da 0474 6578 74da 0e65 6e63 6f64 6564  1..text..encoded
+00000600: 5f73 7472 696e 67a9 0072 1c00 0000 fa2c  _string..r.....,
+00000610: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
+00000620: 616d 6436 345c 6567 675c 6269 6f74 6578  amd64\egg\biotex
+00000630: 745c 646e 6162 6974 732e 7079 da0d 656e  t\dnabits.py..en
+00000640: 636f 6465 5f73 7472 696e 6714 0000 0073  code_string....s
+00000650: 1e00 0000 0819 1e01 1a01 1401 0a01 0c01  ................
+00000660: 0c01 0a01 0c01 0c01 0c01 0c01 0a01 0401  ................
+00000670: 0401 721e 0000 0063 0100 0000 0000 0000  ..r....c........
+00000680: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00000690: 7394 0000 0074 00a0 0174 027c 0083 0164  s....t...t.|...d
+000006a0: 0166 02a1 01a0 0374 04a1 017d 0174 00a0  .f.....t...}.t..
+000006b0: 0574 06a0 0764 027c 00a1 02a1 017d 0264  .t...d.|.....}.d
+000006c0: 0364 0367 027c 017c 0264 046b 023c 0064  .d.g.|.|.d.k.<.d
+000006d0: 0564 0367 027c 017c 0264 066b 023c 0064  .d.g.|.|.d.k.<.d
+000006e0: 0364 0567 027c 017c 0264 076b 023c 0064  .d.g.|.|.d.k.<.d
+000006f0: 0564 0567 027c 017c 0264 086b 023c 007c  .d.g.|.|.d.k.<.|
+00000700: 01a0 0374 08a1 017d 0164 09a0 0974 00a0  ...t...}.d...t..
+00000710: 0a7c 01a1 01a1 017d 0174 0b7c 0183 017d  .|.....}.t.|...}
+00000720: 017c 017d 037c 0353 0029 0a61 f401 0000  .|.}.|.S.).a....
+00000730: 0a20 2020 2044 6563 6f64 6573 2061 2073  .    Decodes a s
+00000740: 7472 696e 6720 7769 7468 2044 4e41 6269  tring with DNAbi
+00000750: 7473 2072 6576 6572 7365 2e09 0a20 2020  ts reverse...   
+00000760: 200a 2020 2020 5061 7261 6d65 7465 7273   .    Parameters
+00000770: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00000780: 2020 2020 696e 7075 745f 7374 7269 6e67      input_string
+00000790: 203a 2073 7472 696e 670a 2020 2020 2020   : string.      
+000007a0: 2020 5465 7874 2073 7472 696e 6720 656e    Text string en
+000007b0: 636f 6465 6420 7769 7468 2044 4e41 6269  coded with DNAbi
+000007c0: 7473 2e0a 0a20 2020 2052 6574 7572 6e73  ts...    Returns
+000007d0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+000007e0: 2064 6563 6f64 6564 5f73 7472 696e 6720   decoded_string 
+000007f0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+00000800: 2044 6563 6f64 6564 2074 6578 742e 0a20   Decoded text.. 
+00000810: 2020 2020 2020 200a 2020 2020 4578 616d         .    Exam
+00000820: 706c 650a 2020 2020 2d2d 2d2d 2d2d 2d0a  ple.    -------.
+00000830: 2020 2020 4465 636f 6465 2061 2073 7472      Decode a str
+00000840: 696e 672e 0a0a 2020 2020 3e3e 3e20 696d  ing...    >>> im
+00000850: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
+00000860: 6274 0a20 2020 203e 3e3e 2065 6e63 6f64  bt.    >>> encod
+00000870: 6564 5f73 7472 696e 6720 3d20 2241 4741  ed_string = "AGA
+00000880: 4343 4347 4341 5447 4341 5447 4354 5447  CCCGCATGCATGCTTG
+00000890: 4341 4147 4154 4354 4354 5447 4347 4154  CAAGATCTCTTGCGAT
+000008a0: 4341 5447 4341 4347 4343 4147 4122 0a20  CATGCACGCCAGA". 
+000008b0: 2020 203e 3e3e 2064 6563 6f64 6564 5f73     >>> decoded_s
+000008c0: 7472 696e 6720 3d20 6274 2e64 6e61 6269  tring = bt.dnabi
+000008d0: 7473 2e64 6563 6f64 655f 7374 7269 6e67  ts.decode_string
+000008e0: 2865 6e63 6f64 6564 5f73 7472 696e 6729  (encoded_string)
+000008f0: 0a20 2020 203e 3e3e 2070 7269 6e74 2864  .    >>> print(d
+00000900: 6563 6f64 6564 5f73 7472 696e 6729 0a20  ecoded_string). 
+00000910: 2020 2048 656c 6c6f 2077 6f72 6c64 210a     Hello world!.
+00000920: 2020 2020 7204 0000 0072 0200 0000 7201      r....r....r.
+00000930: 0000 0072 0500 0000 7203 0000 0072 0700  ...r....r....r..
+00000940: 0000 7209 0000 0072 0b00 0000 720d 0000  ..r....r....r...
+00000950: 0029 0c72 1200 0000 5a05 7a65 726f 7372  .).r....Z.zerosr
+00000960: 1100 0000 7214 0000 0072 1500 0000 7213  ....r....r....r.
+00000970: 0000 0072 0f00 0000 7210 0000 0072 1700  ...r....r....r..
+00000980: 0000 7218 0000 005a 0b63 6f6e 6361 7465  ..r....Z.concate
+00000990: 6e61 7465 da0a 6269 6e5f 746f 5f73 7472  nate..bin_to_str
+000009a0: 2904 7219 0000 0072 1a00 0000 5a03 646e  ).r....r....Z.dn
+000009b0: 61da 0e64 6563 6f64 6564 5f73 7472 696e  a..decoded_strin
+000009c0: 6772 1c00 0000 721c 0000 0072 1d00 0000  gr....r....r....
+000009d0: da0d 6465 636f 6465 5f73 7472 696e 673d  ..decode_string=
+000009e0: 0000 0073 1600 0000 1819 1201 1001 1001  ...s............
+000009f0: 1001 1001 0a01 1001 0801 0401 0401 7221  ..............r!
+00000a00: 0000 0046 6302 0000 0000 0000 0000 0000  ...Fc...........
+00000a10: 0008 0000 0005 0000 0043 0000 0073 9400  .........C...s..
+00000a20: 0000 7400 7c00 8301 7d02 6401 6402 8400  ..t.|...}.d.d...
+00000a30: 7d03 6700 7d04 7c01 7210 7401 6403 8301  }.g.}.|.r.t.d...
+00000a40: 0100 7402 7c00 8301 4400 5d25 5c02 7d05  ..t.|...D.]%\.}.
+00000a50: 7d06 7c03 7c06 8301 7d07 7c04 a003 7c07  }.|.|...}.|...|.
+00000a60: a101 0100 7c01 7239 7c05 6404 1700 6405  ....|.r9|.d...d.
+00000a70: 1600 6406 6b02 7239 7401 7404 7c05 6404  ..d.k.r9t.t.|.d.
+00000a80: 1700 8301 6407 1700 7404 7c02 8301 1700  ....d...t.|.....
+00000a90: 8301 0100 7114 7c01 7248 7401 7404 7c02  ....q.|.rHt.t.|.
+00000aa0: 8301 6407 1700 7404 7c02 8301 1700 8301  ..d...t.|.......
+00000ab0: 0100 7c04 5300 2908 617a 0200 000a 2020  ..|.S.).az....  
+00000ac0: 2020 456e 636f 6465 7320 616c 6c20 7374    Encodes all st
+00000ad0: 7269 6e67 7320 696e 2061 206c 6973 7420  rings in a list 
+00000ae0: 7769 7468 2044 4e41 6269 7473 2e09 0a20  with DNAbits... 
+00000af0: 2020 200a 2020 2020 5061 7261 6d65 7465     .    Paramete
+00000b00: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00000b10: 2d0a 2020 2020 7374 7269 6e67 5f6c 6973  -.    string_lis
+00000b20: 7420 3a20 6c69 7374 0a20 2020 2020 2020  t : list.       
+00000b30: 204c 6973 7420 6f66 2073 7472 696e 6720   List of string 
+00000b40: 746f 2062 6520 656e 636f 6465 642e 0a20  to be encoded.. 
+00000b50: 2020 2076 6572 626f 7365 2020 3a20 626f     verbose  : bo
+00000b60: 6f6c 0a20 2020 2020 2020 2049 6620 5472  ol.        If Tr
+00000b70: 7565 2064 6973 706c 6179 7320 7072 6f67  ue displays prog
+00000b80: 7265 7373 2e0a 0a20 2020 2052 6574 7572  ress...    Retur
+00000b90: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
+00000ba0: 2020 2065 6e63 6f64 6564 5f6c 6973 7420     encoded_list 
+00000bb0: 3a20 6c69 7374 0a20 2020 2020 2020 204c  : list.        L
+00000bc0: 6973 7420 7769 7468 2061 6c6c 2065 6e63  ist with all enc
+00000bd0: 6f64 6564 2074 6578 7420 696e 2073 7472  oded text in str
+00000be0: 696e 6720 666f 726d 6174 2e0a 2020 2020  ing format..    
+00000bf0: 2020 2020 0a20 2020 2045 7861 6d70 6c65      .    Example
+00000c00: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00000c10: 2045 6e63 6f64 6520 7468 6520 7374 7269   Encode the stri
+00000c20: 6e67 7320 696e 2061 206c 6973 7420 616e  ngs in a list an
+00000c30: 6420 7669 6577 2074 6865 2072 6573 756c  d view the resul
+00000c40: 7420 6f66 2074 6865 2066 6972 7374 2069  t of the first i
+00000c50: 7465 6d2e 0a0a 2020 2020 3e3e 3e20 696d  tem...    >>> im
+00000c60: 706f 7274 2062 696f 7465 7874 2061 7320  port biotext as 
+00000c70: 6274 0a20 2020 203e 3e3e 2073 7472 696e  bt.    >>> strin
+00000c80: 675f 6c69 7374 203d 205b 2748 656c 6c6f  g_list = ['Hello
+00000c90: 272c 2777 6f72 6c64 272c 2721 275d 0a20  ','world','!']. 
+00000ca0: 2020 203e 3e3e 2065 6e63 6f64 6564 5f6c     >>> encoded_l
+00000cb0: 6973 7420 3d20 6274 2e64 6e61 6269 7473  ist = bt.dnabits
+00000cc0: 2e65 6e63 6f64 655f 6c69 7374 2873 7472  .encode_list(str
+00000cd0: 696e 675f 6c69 7374 290a 2020 2020 3e3e  ing_list).    >>
+00000ce0: 3e20 7072 696e 7428 656e 636f 6465 645f  > print(encoded_
+00000cf0: 6c69 7374 290a 2020 2020 5b27 4147 4143  list).    ['AGAC
+00000d00: 4343 4743 4154 4743 4154 4743 5454 4743  CCGCATGCATGCTTGC
+00000d10: 272c 2027 5443 5443 5454 4743 4741 5443  ', 'TCTCTTGCGATC
+00000d20: 4154 4743 4143 4743 272c 2027 4341 4741  ATGCACGC', 'CAGA
+00000d30: 275d 0a20 2020 2063 0100 0000 0000 0000  '].    c........
+00000d40: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
+00000d50: f308 0000 0074 007c 0083 0153 00a9 014e  .....t.|...S...N
+00000d60: 2901 721e 0000 00a9 01da 0178 721c 0000  ).r........xr...
+00000d70: 0072 1c00 0000 721d 0000 00da 083c 6c61  .r....r......<la
+00000d80: 6d62 6461 3e7e 0000 00f3 0200 0000 0800  mbda>~..........
+00000d90: 7a1d 656e 636f 6465 5f6c 6973 742e 3c6c  z.encode_list.<l
+00000da0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e7a  ocals>.<lambda>z
+00000db0: 1045 6e63 6f64 696e 6720 7465 7874 2e2e  .Encoding text..
+00000dc0: 2e72 0300 0000 e910 2700 0072 0100 0000  .r......'..r....
+00000dd0: fa01 2f29 0572 1100 0000 da05 7072 696e  ../).r......prin
+00000de0: 74da 0965 6e75 6d65 7261 7465 da06 6170  t..enumerate..ap
+00000df0: 7065 6e64 7217 0000 0029 085a 0b73 7472  pendr....).Z.str
+00000e00: 696e 675f 6c69 7374 da07 7665 7262 6f73  ing_list..verbos
+00000e10: 65da 096c 6973 745f 7369 7a65 da0f 7365  e..list_size..se
+00000e20: 6c65 6374 6564 456e 636f 6465 725a 0c65  lectedEncoderZ.e
+00000e30: 6e63 6f64 6564 5f6c 6973 74da 0163 da01  ncoded_list..c..
+00000e40: 69da 0373 6571 721c 0000 0072 1c00 0000  i..seqr....r....
+00000e50: 721d 0000 00da 0b65 6e63 6f64 655f 6c69  r......encode_li
+00000e60: 7374 6200 0000 731c 0000 0008 1b08 0104  stb...s.........
+00000e70: 0204 0108 0110 0108 010a 0114 011c 0102  ................
+00000e80: 8004 0118 0104 0172 3300 0000 6303 0000  .......r3...c...
+00000e90: 0000 0000 0000 0000 0008 0000 0006 0000  ................
+00000ea0: 0043 0000 0073 9c00 0000 7400 7c00 8301  .C...s....t.|...
+00000eb0: 7d03 6401 6402 8400 7d04 6700 7d05 7c02  }.d.d...}.g.}.|.
+00000ec0: 7210 7401 6403 8301 0100 7402 7c00 8301  r.t.d.....t.|...
+00000ed0: 4400 5d29 5c02 7d06 7d07 7c06 6404 3700  D.])\.}.}.|.d.7.
+00000ee0: 7d06 7c02 7234 7c06 6404 1700 6405 1600  }.|.r4|.d...d...
+00000ef0: 6406 6b02 7234 7401 7403 7c06 6404 1700  d.k.r4t.t.|.d...
+00000f00: 8301 6407 1700 7403 7c03 8301 1700 8301  ..d...t.|.......
+00000f10: 0100 7c05 a004 7c04 7403 7c07 8301 8301  ..|...|.t.|.....
+00000f20: a101 0100 7114 7c02 724c 7401 7403 7c03  ....q.|.rLt.t.|.
+00000f30: 8301 6407 1700 7403 7c03 8301 1700 8301  ..d...t.|.......
+00000f40: 0100 7c05 5300 2908 6181 0200 000a 2020  ..|.S.).a.....  
+00000f50: 2020 4465 636f 6465 7320 616c 6c20 7374    Decodes all st
+00000f60: 7269 6e67 7320 696e 2061 206c 6973 7420  rings in a list 
+00000f70: 7769 7468 2072 6576 6572 7365 2044 4e41  with reverse DNA
+00000f80: 6269 7473 2e09 0a20 2020 200a 2020 2020  bits...    .    
+00000f90: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00000fa0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+00000fb0: 7269 6e67 5f6c 6973 7420 3a20 6c69 7374  ring_list : list
+00000fc0: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
+00000fd0: 2073 7472 696e 6720 656e 636f 6465 6420   string encoded 
+00000fe0: 7769 7468 2044 4e41 6269 7473 2e0a 2020  with DNAbits..  
+00000ff0: 2020 7665 7262 6f73 6520 203a 2062 6f6f    verbose  : boo
+00001000: 6c0a 2020 2020 2020 2020 4966 2054 7275  l.        If Tru
+00001010: 6520 6469 7370 6c61 7973 2070 726f 6772  e displays progr
+00001020: 6573 732e 0a0a 2020 2020 5265 7475 726e  ess...    Return
+00001030: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00001040: 2020 6465 636f 6465 645f 6c69 7374 203a    decoded_list :
+00001050: 206c 6973 7420 6f66 2073 7472 696e 670a   list of string.
+00001060: 2020 2020 2020 2020 4c69 7374 2077 6974          List wit
+00001070: 6820 616c 6c20 6465 636f 6465 6420 7465  h all decoded te
+00001080: 7874 2e0a 2020 2020 2020 2020 0a20 2020  xt..        .   
+00001090: 2045 7861 6d70 6c65 0a20 2020 202d 2d2d   Example.    ---
+000010a0: 2d2d 2d2d 2d0a 2020 2020 4465 636f 6465  -----.    Decode
+000010b0: 2074 6865 2073 7472 696e 6773 2069 6e20   the strings in 
+000010c0: 6120 6c69 7374 2061 6e64 2076 6965 7720  a list and view 
+000010d0: 7468 6520 7265 7375 6c74 2077 6974 6820  the result with 
+000010e0: 6120 6c6f 6f70 2e0a 0a20 2020 203e 3e3e  a loop...    >>>
+000010f0: 2069 6d70 6f72 7420 6269 6f74 6578 7420   import biotext 
+00001100: 6173 2062 740a 2020 2020 3e3e 3e20 656e  as bt.    >>> en
+00001110: 636f 6465 645f 6c69 7374 203d 205b 2741  coded_list = ['A
+00001120: 4741 4343 4347 4341 5447 4341 5447 4354  GACCCGCATGCATGCT
+00001130: 5447 4327 2c20 2754 4354 4354 5447 4347  TGC', 'TCTCTTGCG
+00001140: 4154 4341 5447 4341 4347 4327 2c20 2743  ATCATGCACGC', 'C
+00001150: 4147 4127 5d0a 2020 2020 3e3e 3e20 6465  AGA'].    >>> de
+00001160: 636f 6465 645f 6c69 7374 203d 2062 742e  coded_list = bt.
+00001170: 646e 6162 6974 732e 6465 636f 6465 5f6c  dnabits.decode_l
+00001180: 6973 7428 656e 636f 6465 645f 6c69 7374  ist(encoded_list
+00001190: 290a 2020 2020 3e3e 3e20 7072 696e 7428  ).    >>> print(
+000011a0: 6465 636f 6465 645f 6c69 7374 290a 2020  decoded_list).  
+000011b0: 2020 5b27 4865 6c6c 6f27 2c20 2777 6f72    ['Hello', 'wor
+000011c0: 6c64 272c 2027 2127 5d0a 2020 2020 6301  ld', '!'].    c.
+000011d0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000011e0: 0000 0053 0000 0072 2200 0000 7223 0000  ...S...r"...r#..
+000011f0: 0029 0172 2100 0000 7224 0000 0072 1c00  .).r!...r$...r..
+00001200: 0000 721c 0000 0072 1d00 0000 7226 0000  ..r....r....r&..
+00001210: 00a8 0000 0072 2700 0000 7a1d 6465 636f  .....r'...z.deco
+00001220: 6465 5f6c 6973 742e 3c6c 6f63 616c 733e  de_list.<locals>
+00001230: 2e3c 6c61 6d62 6461 3e7a 1044 6563 6f64  .<lambda>z.Decod
+00001240: 696e 6720 7465 7874 2e2e 2e72 0300 0000  ing text...r....
+00001250: 7228 0000 0072 0100 0000 7229 0000 0029  r(...r....r)...)
+00001260: 0572 1100 0000 722a 0000 0072 2b00 0000  .r....r*...r+...
+00001270: 7217 0000 0072 2c00 0000 2908 5a0a 696e  r....r,...).Z.in
+00001280: 7075 745f 6c69 7374 da0b 6f75 7470 7574  put_list..output
+00001290: 5f66 696c 6572 2d00 0000 722e 0000 0072  _filer-...r....r
+000012a0: 2f00 0000 5a0c 6465 636f 6465 645f 6c69  /...Z.decoded_li
+000012b0: 7374 7230 0000 0072 3100 0000 721c 0000  str0...r1...r...
+000012c0: 0072 1c00 0000 721d 0000 00da 0b64 6563  .r....r......dec
+000012d0: 6f64 655f 6c69 7374 8c00 0000 731a 0000  ode_list....s...
+000012e0: 0008 1b08 0104 0204 0108 0110 0108 0114  ................
+000012f0: 011c 0114 0104 0118 0104 0272 3500 0000  ...........r5...
+00001300: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00001310: 0005 0000 0043 0000 0073 4800 0000 6401  .....C...sH...d.
+00001320: 7d01 7c00 4400 5d1d 7d02 7400 7401 7c02  }.|.D.].}.t.t.|.
+00001330: 8301 8301 6402 6400 8502 1900 7d03 6403  ....d.d.....}.d.
+00001340: 7402 7c03 8301 1600 7d03 7c03 6400 6400  t.|.....}.|.d.d.
+00001350: 6404 8503 1900 7d03 7c01 7c03 3700 7d01  d.....}.|.|.7.}.
+00001360: 7104 7c01 5300 2905 4e72 0d00 0000 7204  q.|.S.).Nr....r.
+00001370: 0000 007a 0425 3038 64e9 ffff ffff 2903  ...z.%08d.....).
+00001380: da03 6269 6eda 036f 7264 7215 0000 0029  ..bin..ordr....)
+00001390: 04da 0673 7472 696e 67da 0372 6573 da04  ...string..res..
+000013a0: 6368 6172 da03 746d 7072 1c00 0000 721c  char..tmpr....r.
+000013b0: 0000 0072 1d00 0000 720e 0000 00b7 0000  ...r....r.......
+000013c0: 0073 0e00 0000 0401 0801 1401 0c01 0e01  .s..............
+000013d0: 0a01 0401 720e 0000 0063 0100 0000 0000  ....r....c......
+000013e0: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+000013f0: 0000 735e 0000 0064 017d 0174 0074 0174  ..s^...d.}.t.t.t
+00001400: 027c 0083 0164 021b 0083 0183 0144 005d  .|...d.......D.]
+00001410: 207d 027c 007c 0264 0214 007c 0264 0317   }.|.|.d...|.d..
+00001420: 0064 0214 0085 0219 007d 037c 0364 0064  .d.......}.|.d.d
+00001430: 0064 0485 0319 007d 0374 0374 017c 0364  .d.....}.t.t.|.d
+00001440: 0583 0283 017d 047c 017c 0437 007d 0171  .....}.|.|.7.}.q
+00001450: 0c7c 0153 0029 064e 720d 0000 00e9 0800  .|.S.).Nr.......
+00001460: 0000 7203 0000 0072 3600 0000 7204 0000  ..r....r6...r...
+00001470: 0029 04da 0572 616e 6765 7215 0000 0072  .)...ranger....r
+00001480: 1100 0000 da03 6368 7229 0572 3900 0000  ......chr).r9...
+00001490: 723a 0000 00da 0369 6478 5a04 6373 7472  r:.....idxZ.cstr
+000014a0: 723c 0000 0072 1c00 0000 721c 0000 0072  r<...r....r....r
+000014b0: 1d00 0000 721f 0000 00c0 0000 0073 0e00  ....r........s..
+000014c0: 0000 0401 1801 1801 0e01 0e01 0a01 0401  ................
+000014d0: 721f 0000 0029 0146 2902 4e46 290a da07  r....).F).NF)...
+000014e0: 5f5f 646f 635f 5f72 0f00 0000 da05 6e75  __doc__r......nu
+000014f0: 6d70 7972 1200 0000 721e 0000 0072 2100  mpyr....r....r!.
+00001500: 0000 7233 0000 0072 3500 0000 720e 0000  ..r3...r5...r...
+00001510: 0072 1f00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+00001520: 721c 0000 0072 1d00 0000 da08 3c6d 6f64  r....r......<mod
+00001530: 756c 653e 0100 0000 7312 0000 0004 0208  ule>....s.......
+00001540: 0e08 0108 0208 290a 250a 2a08 2b0c 09    ......).%.*.+..
```

## biotext/fastatools.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Nov  9 03:16:42 2022 UTC, .py size: 7610 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,451 +1,661 @@
-00000000: 550d 0d0a 0000 0000 9a1b 6b63 ba1d 0000  U.........kc....
+00000000: 6f0d 0d0a 0000 0000 ca7f af64 702d 0000  o..........dp-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
-00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6400 6401 6c09 5a09 6400  m.Z...d.d.l.Z.d.
-00000070: 6401 6c0a 5a0b 6400 6405 6c0c 6d0d 5a0d  d.l.Z.d.d.l.m.Z.
-00000080: 0100 6400 6401 6c0e 5a0e 6400 6406 6c0f  ..d.d.l.Z.d.d.l.
-00000090: 6d10 5a10 0100 6400 6401 6c11 5a11 641e  m.Z...d.d.l.Z.d.
-000000a0: 6408 6409 8401 5a12 640a 640b 8400 5a13  d.d...Z.d.d...Z.
-000000b0: 640c 640d 8400 5a14 640e 640f 8400 5a15  d.d...Z.d.d...Z.
-000000c0: 641f 6410 6411 8401 5a16 6412 6413 8400  d.d.d...Z.d.d...
-000000d0: 5a17 6414 6415 8400 5a18 6420 6416 6417  Z.d.d...Z.d d.d.
-000000e0: 8401 5a19 6401 6418 6419 641a 6419 6703  ..Z.d.d.d.d.d.g.
-000000f0: 641b 641a 6605 641c 641d 8401 5a1a 6401  d.d.f.d.d...Z.d.
-00000100: 5300 2921 e900 0000 004e 2902 da07 416c  S.)!.....N)...Al
-00000110: 6967 6e49 4fda 0553 6571 494f 2901 da03  ignIO..SeqIO)...
-00000120: 5365 7129 01da 0953 6571 5265 636f 7264  Seq)...SeqRecord
-00000130: 2901 da05 7374 6174 7329 01da 0966 6173  )...stats)...fas
-00000140: 3273 7765 6570 da00 6302 0000 0000 0000  2sweep..c.......
-00000150: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00000160: 0073 6400 0000 7400 6a01 6401 6402 6403  .sd...t.j.d.d.d.
-00000170: 8d02 7d02 6404 7c00 1700 6405 1700 7c02  ..}.d.|...d...|.
-00000180: 6a02 1700 6406 1700 7d03 7c03 6407 7c01  j...d...}.|.d.|.
-00000190: 1700 3700 7d03 7403 6a04 7c03 6408 6409  ..7.}.t.j.|.d.d.
-000001a0: 8d02 0100 7405 a006 7c02 6a02 640a a102  ....t...|.j.d...
-000001b0: 7d04 7c02 a007 a100 0100 7408 a009 7c02  }.|.......t...|.
-000001c0: 6a02 a101 0100 7c04 5300 290b 4eda 0177  j.....|.S.).N..w
-000001d0: 46a9 02da 046d 6f64 65da 0664 656c 6574  F....mode..delet
-000001e0: 657a 0c63 6c75 7374 616c 6f20 2d69 207a  ez.clustalo -i z
-000001f0: 0420 2d6f 207a 1c20 2d2d 6175 746f 202d  . -o z. --auto -
-00000200: 2d6f 7574 666d 7420 636c 7520 2d2d 666f  -outfmt clu --fo
-00000210: 7263 65fa 0120 5429 01da 0573 6865 6c6c  rce.. T)...shell
-00000220: 5a07 636c 7573 7461 6c29 0ada 0874 656d  Z.clustal)...tem
-00000230: 7066 696c 65da 0d54 656d 706f 7261 7279  pfile..Temporary
-00000240: 4669 6c65 da04 6e61 6d65 da0a 7375 6270  File..name..subp
-00000250: 726f 6365 7373 da04 6361 6c6c 7202 0000  rocess..callr...
-00000260: 00da 0472 6561 64da 0563 6c6f 7365 da02  ...read..close..
-00000270: 6f73 da06 756e 6c69 6e6b 2905 da0f 696e  os..unlink)...in
-00000280: 7075 745f 6669 6c65 5f6e 616d 65da 0461  put_file_name..a
-00000290: 7267 73da 0266 705a 0a63 6d64 5f73 7472  rgs..fpZ.cmd_str
-000002a0: 696e 67da 0961 6c69 676e 6d65 6e74 a900  ing..alignment..
-000002b0: 721c 0000 00fa 2f62 7569 6c64 5c62 6469  r...../build\bdi
-000002c0: 7374 2e77 696e 2d61 6d64 3634 5c65 6767  st.win-amd64\egg
-000002d0: 5c62 696f 7465 7874 5c66 6173 7461 746f  \biotext\fastato
-000002e0: 6f6c 732e 7079 da0c 7275 6e5f 636c 7573  ols.py..run_clus
-000002f0: 7461 6c6f 0f00 0000 7310 0000 0000 010e  talo....s.......
-00000300: 0116 010c 010e 010e 0108 010c 0172 1e00  .............r..
-00000310: 0000 6301 0000 0000 0000 0000 0000 0009  ..c.............
-00000320: 0000 0007 0000 0043 0000 0073 0001 0000  .......C...s....
-00000330: 7400 7c00 8301 7d01 7401 6a02 6401 6402  t.|...}.t.j.d.d.
-00000340: 6403 8d02 7d02 7c01 4400 5d2a 7d03 7c02  d...}.|.D.]*}.|.
-00000350: a003 6404 7404 7c03 6a05 8301 1700 6405  ..d.t.|.j.....d.
-00000360: 1700 7404 7c03 6a06 8301 1700 6405 1700  ..t.|.j.....d...
-00000370: a101 0100 711a 7c02 a007 a100 0100 6700  ....q.|.......g.
-00000380: 7d04 7408 7c01 8301 6406 6b04 72d4 7409  }.t.|...d.k.r.t.
-00000390: 7c02 6a0a 8301 7d05 6700 7d06 7c05 4400  |.j...}.g.}.|.D.
-000003a0: 5d24 7d03 7c06 a00b 7400 7c03 6a06 8301  ]$}.|...t.|.j...
-000003b0: a101 0100 7c04 a00b 7404 7c03 6a06 8301  ....|...t.|.j...
-000003c0: a101 0100 7170 740c a00d 7c06 a101 7d06  ....qpt...|...}.
-000003d0: 740e a00f 7c06 a101 7d07 7c07 6407 1900  t...|...}.|.d...
-000003e0: 7c07 6406 1900 6407 6b05 1900 7d07 7410  |.d...d.k...}.t.
-000003f0: a011 6408 6409 6409 a012 7c07 a101 a103  ..d.d.d...|.....
-00000400: 7d08 6e18 7404 7c01 6407 1900 6a06 8301  }.n.t.|.d...j...
-00000410: 7d08 7c04 a00b 7c08 a101 0100 7413 a014  }.|...|.....t...
-00000420: 7c02 6a0a a101 0100 7c08 7c04 6602 5300  |.j.....|.|.f.S.
-00000430: 290a 4e72 0900 0000 4672 0a00 0000 fa01  ).Nr....Fr......
-00000440: 3eda 010a e901 0000 0072 0100 0000 7a03  >........r....z.
-00000450: 5c2d 2b72 0800 0000 2915 da04 6c69 7374  \-+r....)...list
-00000460: 720f 0000 0072 1000 0000 da05 7772 6974  r....r......writ
-00000470: 65da 0373 7472 da0b 6465 7363 7269 7074  e..str..descript
-00000480: 696f 6eda 0373 6571 7215 0000 00da 036c  ion..seqr......l
-00000490: 656e 721e 0000 0072 1100 0000 da06 6170  enr....r......ap
-000004a0: 7065 6e64 da02 6e70 da05 6172 7261 7972  pend..np..arrayr
-000004b0: 0600 0000 720b 0000 00da 0272 65da 0373  ....r......re..s
-000004c0: 7562 da04 6a6f 696e 7216 0000 0072 1700  ub..joinr....r..
-000004d0: 0000 2909 da0e 7365 7172 6563 6f72 645f  ..)...seqrecord_
-000004e0: 6c69 7374 da08 7365 715f 6c69 7374 5a09  list..seq_listZ.
-000004f0: 6661 7374 6154 6578 74da 0169 721b 0000  fastaText..ir...
-00000500: 005a 0661 6c69 676e 315a 0661 6c69 676e  .Z.align1Z.align
-00000510: 32da 016d 5a09 636f 6e73 656e 7375 7372  2..mZ.consensusr
-00000520: 1c00 0000 721c 0000 0072 1d00 0000 da0d  ....r....r......
-00000530: 6765 745f 636f 6e73 656e 7375 7319 0000  get_consensus...
-00000540: 0073 2800 0000 0001 0801 0e01 0801 2801  .s(...........(.
-00000550: 0802 0401 0c01 0a01 0401 0801 1001 1201  ................
-00000560: 0a01 0a01 1401 1602 0e01 0a02 0c01 7232  ..............r2
-00000570: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000580: 0400 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
-00000590: 0074 007c 0083 017d 0067 007d 017c 0044  .t.|...}.g.}.|.D
-000005a0: 005d 147d 027c 026a 017d 037c 01a0 027c  .].}.|.j.}.|...|
-000005b0: 03a1 0101 0071 107c 0153 0029 0161 8402  .....q.|.S.).a..
-000005c0: 0000 0a20 2020 2047 6574 2074 6865 2068  ...    Get the h
-000005d0: 6561 6465 7220 6672 6f6d 2061 6c6c 2069  eader from all i
-000005e0: 7465 6d73 2069 6e20 6120 6c69 7374 206f  tems in a list o
-000005f0: 6620 5365 7152 6563 6f72 6420 2842 696f  f SeqRecord (Bio
-00000600: 7079 7468 6f6e 206f 626a 6563 7429 2e0a  python object)..
-00000610: 2020 2020 0a20 2020 2050 6172 616d 6574      .    Paramet
-00000620: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00000630: 2d2d 0a20 2020 2073 6571 7265 636f 7264  --.    seqrecord
-00000640: 5f6c 6973 7420 3a20 6c69 7374 206f 6620  _list : list of 
-00000650: 5365 7152 6563 6f72 640a 2020 2020 2020  SeqRecord.      
-00000660: 2020 4c69 7374 206f 6620 5365 7152 6563    List of SeqRec
-00000670: 6f72 642e 0a0a 2020 2020 4f75 7470 7574  ord...    Output
-00000680: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-00000690: 2020 6865 6164 6572 5f6c 6973 7420 3a20    header_list : 
-000006a0: 6c69 7374 206f 6620 7374 7269 6e67 0a20  list of string. 
-000006b0: 2020 2020 2020 204c 6973 7420 6f66 2061         List of a
-000006c0: 6c6c 2068 6561 6465 7273 2065 7874 7261  ll headers extra
-000006d0: 6374 6564 2066 726f 6d20 696e 7075 742e  cted from input.
-000006e0: 0a20 2020 2020 2020 200a 2020 2020 4578  .        .    Ex
-000006f0: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-00000700: 2d2d 0a20 2020 2043 7265 6174 6573 2073  --.    Creates s
-00000710: 6571 7265 636f 7264 5f6c 6973 742c 2065  eqrecord_list, e
-00000720: 7874 7261 6374 2068 6561 6465 7273 2061  xtract headers a
-00000730: 6e64 2070 7269 6e74 2069 742e 0a0a 2020  nd print it...  
-00000740: 2020 3e3e 3e20 696d 706f 7274 2062 696f    >>> import bio
-00000750: 7465 7874 2061 7320 6274 0a20 2020 203e  text as bt.    >
-00000760: 3e3e 2073 6571 5f6c 6973 7420 3d20 5b27  >> seq_list = ['
-00000770: 4143 5447 272c 2747 5443 4127 5d0a 2020  ACTG','GTCA'].  
-00000780: 2020 3e3e 3e20 7365 7172 6563 6f72 645f    >>> seqrecord_
-00000790: 6c69 7374 203d 2062 742e 6661 7374 6174  list = bt.fastat
-000007a0: 6f6f 6c73 2e63 7265 6174 655f 7365 7172  ools.create_seqr
-000007b0: 6563 6f72 645f 6c69 7374 2873 6571 5f6c  ecord_list(seq_l
-000007c0: 6973 7429 0a20 2020 203e 3e3e 2065 7874  ist).    >>> ext
-000007d0: 7261 6374 6564 5f68 6561 6465 725f 6c69  racted_header_li
-000007e0: 7374 203d 2062 742e 6661 7374 6174 6f6f  st = bt.fastatoo
-000007f0: 6c73 2e67 6574 5f68 6561 6465 7228 7365  ls.get_header(se
-00000800: 7172 6563 6f72 645f 6c69 7374 290a 2020  qrecord_list).  
-00000810: 2020 3e3e 3e20 7072 696e 7428 6578 7472    >>> print(extr
-00000820: 6163 7465 645f 6865 6164 6572 5f6c 6973  acted_header_lis
-00000830: 7429 0a20 2020 205b 2730 272c 2027 3127  t).    ['0', '1'
-00000840: 5d0a 2020 2020 2903 7222 0000 0072 2500  ].    ).r"...r%.
-00000850: 0000 7228 0000 0029 0472 2e00 0000 da0b  ..r(...).r......
-00000860: 6865 6164 6572 5f6c 6973 7472 3000 0000  header_listr0...
-00000870: da06 6865 6164 6572 721c 0000 0072 1c00  ..headerr....r..
-00000880: 0000 721d 0000 00da 0a67 6574 5f68 6561  ..r......get_hea
-00000890: 6465 7232 0000 0073 0c00 0000 001a 0801  der2...s........
-000008a0: 0401 0801 0601 0c01 7235 0000 0063 0100  ........r5...c..
-000008b0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-000008c0: 0000 4300 0000 732e 0000 0074 007c 0083  ..C...s....t.|..
-000008d0: 017d 0067 007d 017c 0044 005d 187d 027c  .}.g.}.|.D.].}.|
-000008e0: 026a 017d 037c 01a0 0274 037c 0383 01a1  .j.}.|...t.|....
-000008f0: 0101 0071 107c 0153 0029 0161 8502 0000  ...q.|.S.).a....
-00000900: 0a20 2020 2047 6574 2074 6865 2073 6571  .    Get the seq
-00000910: 7565 6e63 6573 2066 726f 6d20 616c 6c20  uences from all 
-00000920: 6974 656d 7320 696e 2061 206c 6973 7420  items in a list 
-00000930: 6f66 2053 6571 5265 636f 7264 2028 4269  of SeqRecord (Bi
-00000940: 6f70 7974 686f 6e20 6f62 6a65 6374 292e  opython object).
-00000950: 0a20 2020 200a 2020 2020 5061 7261 6d65  .    .    Parame
-00000960: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00000970: 2d2d 2d0a 2020 2020 7365 7172 6563 6f72  ---.    seqrecor
-00000980: 645f 6c69 7374 203a 206c 6973 7420 6f66  d_list : list of
-00000990: 2053 6571 5265 636f 7264 0a20 2020 2020   SeqRecord.     
-000009a0: 2020 204c 6973 7420 6f66 2053 6571 5265     List of SeqRe
-000009b0: 636f 7264 2e0a 0a20 2020 204f 7574 7075  cord...    Outpu
-000009c0: 740a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  t.    --------. 
-000009d0: 2020 2073 6571 5f6c 6973 7420 3a20 6c69     seq_list : li
-000009e0: 7374 206f 6620 7374 7269 6e67 0a20 2020  st of string.   
-000009f0: 2020 2020 204c 6973 7420 6f66 2061 6c6c       List of all
-00000a00: 2073 6571 7565 6e63 6573 2065 7874 7261   sequences extra
-00000a10: 6374 6564 2066 726f 6d20 696e 7075 742e  cted from input.
-00000a20: 0a20 2020 2020 2020 200a 2020 2020 4578  .        .    Ex
-00000a30: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-00000a40: 2d2d 0a20 2020 2043 7265 6174 6573 2073  --.    Creates s
-00000a50: 6571 7265 636f 7264 5f6c 6973 742c 2065  eqrecord_list, e
-00000a60: 7874 7261 6374 2073 6571 7565 6e63 6573  xtract sequences
-00000a70: 2061 6e64 2070 7269 6e74 2069 742e 0a0a   and print it...
-00000a80: 2020 2020 3e3e 3e20 696d 706f 7274 2062      >>> import b
-00000a90: 696f 7465 7874 2061 7320 6274 0a20 2020  iotext as bt.   
-00000aa0: 203e 3e3e 2073 6571 5f6c 6973 7420 3d20   >>> seq_list = 
-00000ab0: 5b27 4143 5447 272c 2747 5443 4127 5d0a  ['ACTG','GTCA'].
-00000ac0: 2020 2020 3e3e 3e20 7365 7172 6563 6f72      >>> seqrecor
-00000ad0: 645f 6c69 7374 203d 2062 742e 6661 7374  d_list = bt.fast
-00000ae0: 6174 6f6f 6c73 2e63 7265 6174 655f 7365  atools.create_se
-00000af0: 7172 6563 6f72 645f 6c69 7374 2873 6571  qrecord_list(seq
-00000b00: 5f6c 6973 7429 0a20 2020 203e 3e3e 2065  _list).    >>> e
-00000b10: 7874 7261 6374 6564 5f73 6571 5f6c 6973  xtracted_seq_lis
-00000b20: 7420 3d20 6274 2e66 6173 7461 746f 6f6c  t = bt.fastatool
-00000b30: 732e 6765 745f 7365 7128 7365 7172 6563  s.get_seq(seqrec
-00000b40: 6f72 645f 6c69 7374 290a 2020 2020 3e3e  ord_list).    >>
-00000b50: 3e20 7072 696e 7428 6578 7472 6163 7465  > print(extracte
-00000b60: 645f 7365 715f 6c69 7374 290a 2020 2020  d_seq_list).    
-00000b70: 5b27 4143 5447 272c 2027 4754 4341 275d  ['ACTG', 'GTCA']
-00000b80: 0a20 2020 2029 0472 2200 0000 7226 0000  .    ).r"...r&..
-00000b90: 0072 2800 0000 7224 0000 0029 0472 2e00  .r(...r$...).r..
-00000ba0: 0000 722f 0000 0072 3000 0000 7226 0000  ..r/...r0...r&..
-00000bb0: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000bc0: da07 6765 745f 7365 7153 0000 0073 0c00  ..get_seqS...s..
-00000bd0: 0000 001a 0801 0401 0801 0601 1001 7236  ..............r6
-00000be0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000bf0: 0500 0000 0600 0000 4300 0000 7362 0000  ........C...sb..
-00000c00: 007c 0164 016b 0272 1a74 0074 0164 0274  .|.d.k.r.t.t.d.t
-00000c10: 027c 0083 0183 0283 017d 0167 007d 0274  .|.......}.g.}.t
-00000c20: 0164 0274 027c 0083 0183 0244 005d 307d  .d.t.|.....D.]0}
-00000c30: 0374 0374 047c 007c 0319 0083 0174 057c  .t.t.|.|.....t.|
-00000c40: 017c 0319 0083 0174 057c 0383 0164 038d  .|.....t.|...d..
-00000c50: 037d 047c 02a0 067c 04a1 0101 0071 2c7c  .}.|...|.....q,|
-00000c60: 0253 0029 0461 8103 0000 0a20 2020 2043  .S.).a.....    C
-00000c70: 7265 6174 6573 2061 206c 6973 7420 6f66  reates a list of
-00000c80: 2053 6571 5265 636f 7264 2028 4269 6f70   SeqRecord (Biop
-00000c90: 7974 686f 6e20 6f62 6a65 6374 2920 6672  ython object) fr
-00000ca0: 6f6d 2061 2073 7472 696e 6720 6c69 7374  om a string list
-00000cb0: 2e0a 2020 2020 0a20 2020 2050 6172 616d  ..    .    Param
-00000cc0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00000cd0: 2d2d 2d2d 0a20 2020 2073 6571 5f6c 6973  ----.    seq_lis
-00000ce0: 7420 3a20 6c69 7374 206f 6620 7374 7269  t : list of stri
-00000cf0: 6e67 0a20 2020 2020 2020 204c 6973 7420  ng.        List 
-00000d00: 6f66 2062 696f 6c6f 6769 6361 6c20 7365  of biological se
-00000d10: 7175 656e 6365 7320 696e 2073 7472 696e  quences in strin
-00000d20: 6720 666f 726d 6174 2e0a 2020 2020 6865  g format..    he
-00000d30: 6164 6572 203a 206c 6973 7420 6f66 2073  ader : list of s
-00000d40: 7472 696e 670a 2020 2020 2020 2020 4c69  tring.        Li
-00000d50: 7374 206f 6620 6865 6164 6572 7320 696e  st of headers in
-00000d60: 2073 7472 696e 6720 666f 726d 6174 2c20   string format, 
-00000d70: 6966 2073 6574 2074 6f20 274e 6f6e 6527  if set to 'None'
-00000d80: 2074 6865 2068 6561 6465 7273 2077 696c   the headers wil
-00000d90: 6c20 0a20 2020 2020 2020 2062 6520 6175  l .        be au
-00000da0: 746f 6d61 7469 6361 6c6c 7920 6465 6669  tomatically defi
-00000db0: 6e65 6420 7769 7468 206e 756d 6265 7273  ned with numbers
-00000dc0: 2069 6e20 696e 6372 6561 7369 6e67 206f   in increasing o
-00000dd0: 7264 6572 2e0a 0a20 2020 204f 7574 7075  rder...    Outpu
-00000de0: 740a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  t.    --------. 
-00000df0: 2020 2073 6571 7265 636f 7264 5f6c 6973     seqrecord_lis
-00000e00: 7420 3a20 6c69 7374 206f 6620 5365 7152  t : list of SeqR
-00000e10: 6563 6f72 640a 2020 2020 2020 2020 4c69  ecord.        Li
-00000e20: 7374 206f 6620 5365 7152 6563 6f72 642e  st of SeqRecord.
-00000e30: 0a20 2020 2020 2020 200a 2020 2020 4578  .        .    Ex
-00000e40: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
-00000e50: 2d2d 0a20 2020 2044 6563 6f64 6520 6120  --.    Decode a 
-00000e60: 7374 7269 6e67 2e0a 0a20 2020 203e 3e3e  string...    >>>
-00000e70: 2069 6d70 6f72 7420 6269 6f74 6578 7420   import biotext 
-00000e80: 6173 2062 740a 2020 2020 3e3e 3e20 7365  as bt.    >>> se
-00000e90: 715f 6c69 7374 203d 205b 2741 4354 4727  q_list = ['ACTG'
-00000ea0: 2c27 4754 4341 275d 0a20 2020 203e 3e3e  ,'GTCA'].    >>>
-00000eb0: 2073 6571 7265 636f 7264 5f6c 6973 7420   seqrecord_list 
-00000ec0: 3d20 6274 2e66 6173 7461 746f 6f6c 732e  = bt.fastatools.
-00000ed0: 6372 6561 7465 5f73 6571 7265 636f 7264  create_seqrecord
-00000ee0: 5f6c 6973 7428 7365 715f 6c69 7374 290a  _list(seq_list).
-00000ef0: 2020 2020 3e3e 3e20 666f 7220 6920 696e      >>> for i in
-00000f00: 2073 6571 7265 636f 7264 5f6c 6973 743a   seqrecord_list:
-00000f10: 0a20 2020 203e 3e3e 2020 2020 2070 7269  .    >>>     pri
-00000f20: 6e74 2028 6929 0a20 2020 2049 443a 2030  nt (i).    ID: 0
-00000f30: 0a20 2020 204e 616d 653a 203c 756e 6b6e  .    Name: <unkn
-00000f40: 6f77 6e20 6e61 6d65 3e0a 2020 2020 4465  own name>.    De
-00000f50: 7363 7269 7074 696f 6e3a 2030 0a20 2020  scription: 0.   
-00000f60: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
-00000f70: 7265 733a 2030 0a20 2020 2053 6571 2827  res: 0.    Seq('
-00000f80: 4143 5447 2729 0a20 2020 2049 443a 2031  ACTG').    ID: 1
-00000f90: 0a20 2020 204e 616d 653a 203c 756e 6b6e  .    Name: <unkn
-00000fa0: 6f77 6e20 6e61 6d65 3e0a 2020 2020 4465  own name>.    De
-00000fb0: 7363 7269 7074 696f 6e3a 2031 0a20 2020  scription: 1.   
-00000fc0: 204e 756d 6265 7220 6f66 2066 6561 7475   Number of featu
-00000fd0: 7265 733a 2030 0a20 2020 2053 6571 2827  res: 0.    Seq('
-00000fe0: 4754 4341 2729 0a20 2020 204e 7201 0000  GTCA').    Nr...
-00000ff0: 0029 0272 2500 0000 da02 6964 2907 7222  .).r%.....id).r"
-00001000: 0000 00da 0572 616e 6765 7227 0000 0072  .....ranger'...r
-00001010: 0500 0000 7204 0000 0072 2400 0000 7228  ....r....r$...r(
-00001020: 0000 0029 0572 2f00 0000 7233 0000 0072  ...).r/...r3...r
-00001030: 2e00 0000 7230 0000 00da 0672 6563 6f72  ....r0.....recor
-00001040: 6472 1c00 0000 721c 0000 0072 1d00 0000  dr....r....r....
-00001050: da15 6372 6561 7465 5f73 6571 7265 636f  ..create_seqreco
-00001060: 7264 5f6c 6973 7474 0000 0073 0e00 0000  rd_listt...s....
-00001070: 0025 0801 1201 0401 1201 2201 0c01 723a  .%........"...r:
-00001080: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001090: 0500 0000 0900 0000 4300 0000 7350 0000  ........C...sP..
-000010a0: 0074 007c 0083 017d 0074 0164 0174 027c  .t.|...}.t.d.t.|
-000010b0: 0083 0183 0244 005d 347d 027c 0144 005d  .....D.]4}.|.D.]
-000010c0: 2a7d 0374 03a0 047c 0364 0274 057c 007c  *}.t...|.d.t.|.|
-000010d0: 0219 006a 0683 01a1 037d 0474 077c 0483  ...j.....}.t.|..
-000010e0: 017c 007c 0219 005f 0671 1e71 167c 0053  .|.|..._.q.q.|.S
-000010f0: 0029 034e 7201 0000 0072 0800 0000 2908  .).Nr....r....).
-00001100: 7222 0000 0072 3800 0000 7227 0000 0072  r"...r8...r'...r
-00001110: 2b00 0000 722c 0000 0072 2400 0000 7226  +...r,...r$...r&
-00001120: 0000 0072 0400 0000 2905 722f 0000 005a  ...r....).r/...Z
-00001130: 0372 6578 7230 0000 00da 0269 69da 0173  .rexr0.....ii..s
-00001140: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00001150: 0e72 656d 6f76 655f 7061 7474 6572 6ea1  .remove_pattern.
-00001160: 0000 0073 0c00 0000 0001 0801 1201 0801  ...s............
-00001170: 1801 1201 723d 0000 0063 0100 0000 0000  ....r=...c......
-00001180: 0000 0000 0000 0300 0000 0900 0000 4300  ..............C.
-00001190: 0000 732e 0000 0074 00a0 017c 0064 0164  ..s....t...|.d.d
-000011a0: 02a1 038f 167d 0174 0274 03a0 047c 0164  .....}.t.t...|.d
-000011b0: 03a1 0283 017d 0257 0035 0051 0052 0058  .....}.W.5.Q.R.X
-000011c0: 007c 0253 0029 0461 9302 0000 0a20 2020  .|.S.).a.....   
-000011d0: 2055 7365 7320 6269 6f70 7974 686f 6e20   Uses biopython 
-000011e0: 746f 2069 6d70 6f72 7420 6120 4641 5354  to import a FAST
-000011f0: 4120 6669 6c65 2e0a 2020 2020 0a20 2020  A file..    .   
-00001200: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00001210: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069  ----------.    i
-00001220: 6e70 7574 5f66 696c 655f 6e61 6d65 203a  nput_file_name :
-00001230: 2073 7472 696e 6720 2876 616c 6964 2066   string (valid f
-00001240: 696c 6520 6e61 6d65 290a 2020 2020 2020  ile name).      
-00001250: 2020 496e 7075 7420 6661 7374 6120 6669    Input fasta fi
-00001260: 6c65 206e 616d 652e 0a0a 2020 2020 4f75  le name...    Ou
-00001270: 7470 7574 0a20 2020 202d 2d2d 2d2d 2d2d  tput.    -------
-00001280: 2d0a 2020 2020 7365 7172 6563 6f72 645f  -.    seqrecord_
-00001290: 6c69 7374 203a 206c 6973 7420 6f66 2053  list : list of S
-000012a0: 6571 5265 636f 7264 0a20 2020 2020 2020  eqRecord.       
-000012b0: 204c 6973 7420 6f66 2053 6571 5265 636f   List of SeqReco
-000012c0: 7264 2069 6d70 6f72 7465 6420 6672 6f6d  rd imported from
-000012d0: 2066 696c 652e 0a20 2020 2020 2020 200a   file..        .
-000012e0: 2020 2020 4578 616d 706c 650a 2020 2020      Example.    
-000012f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2043 7265  --------.    Cre
-00001300: 6174 6573 2061 2046 4153 5441 2066 696c  ates a FASTA fil
-00001310: 6520 6e61 6d65 6420 2774 6573 742e 6661  e named 'test.fa
-00001320: 7374 6127 2061 6e64 2069 6d70 6f72 7420  sta' and import 
-00001330: 6974 2061 7320 6120 5365 7152 6563 6f72  it as a SeqRecor
-00001340: 6420 6c69 7374 2e0a 0a20 2020 203e 3e3e  d list...    >>>
-00001350: 2069 6d70 6f72 7420 6269 6f74 6578 7420   import biotext 
-00001360: 6173 2062 740a 2020 2020 3e3e 3e20 7365  as bt.    >>> se
-00001370: 715f 6c69 7374 203d 205b 2741 4354 4727  q_list = ['ACTG'
-00001380: 2c27 4754 4341 275d 0a20 2020 203e 3e3e  ,'GTCA'].    >>>
-00001390: 2073 6571 7265 636f 7264 5f6c 6973 745f   seqrecord_list_
-000013a0: 3120 3d20 6274 2e66 6173 7461 746f 6f6c  1 = bt.fastatool
-000013b0: 732e 6372 6561 7465 5f73 6571 7265 636f  s.create_seqreco
-000013c0: 7264 5f6c 6973 7428 7365 715f 6c69 7374  rd_list(seq_list
-000013d0: 290a 2020 2020 3e3e 3e20 6274 2e66 6173  ).    >>> bt.fas
-000013e0: 7461 746f 6f6c 732e 6578 706f 7274 5f66  tatools.export_f
-000013f0: 6173 7461 2873 6571 7265 636f 7264 5f6c  asta(seqrecord_l
-00001400: 6973 742c 2774 6573 742e 6661 7374 6127  ist,'test.fasta'
-00001410: 290a 2020 2020 3e3e 3e20 7365 7172 6563  ).    >>> seqrec
-00001420: 6f72 645f 6c69 7374 5f32 203d 2062 742e  ord_list_2 = bt.
-00001430: 6661 7374 6174 6f6f 6c73 2e63 7265 6174  fastatools.creat
-00001440: 655f 7365 7172 6563 6f72 645f 6c69 7374  e_seqrecord_list
-00001450: 2873 6571 5f6c 6973 7429 0a20 2020 20da  (seq_list).    .
-00001460: 0172 fa05 7574 662d 385a 0566 6173 7461  .r..utf-8Z.fasta
-00001470: 2905 da06 636f 6465 6373 da04 6f70 656e  )...codecs..open
-00001480: 7222 0000 0072 0300 0000 da05 7061 7273  r"...r......pars
-00001490: 6529 0372 1800 0000 da01 6672 2e00 0000  e).r......fr....
-000014a0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-000014b0: 0c69 6d70 6f72 745f 6661 7374 61a9 0000  .import_fasta...
-000014c0: 0073 0600 0000 0019 1001 1a01 7244 0000  .s..........rD..
-000014d0: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
-000014e0: 0000 0600 0000 4300 0000 73a2 0000 0074  ......C...s....t
-000014f0: 007c 0083 017d 007c 0264 016b 0372 2674  .|...}.|.d.k.r&t
-00001500: 0164 0264 0384 007c 0044 0083 017c 0264  .d.d...|.D...|.d
-00001510: 048d 027d 0074 02a0 037c 0164 0564 06a1  ...}.t...|.d.d..
-00001520: 037d 037c 0044 005d 5c7d 0474 047c 046a  .}.|.D.]\}.t.|.j
-00001530: 0583 0164 076b 0472 387c 03a0 0664 087c  ...d.k.r8|...d.|
-00001540: 046a 0717 0064 0917 00a1 0101 0074 087c  .j...d.......t.|
-00001550: 046a 0583 017d 0574 09a0 0a64 0a74 0864  .j...}.t...d.t.d
-00001560: 0b83 0117 0064 0c17 007c 05a1 027d 0564  .....d...|...}.d
-00001570: 09a0 0b7c 05a1 017d 057c 03a0 067c 05a1  ...|...}.|...|..
-00001580: 0101 0071 387c 03a0 0ca1 0001 0064 0153  ...q8|.......d.S
-00001590: 0029 0d61 0e02 0000 0a20 2020 2043 7265  .).a.....    Cre
-000015a0: 6174 6573 2061 2066 696c 6520 7573 696e  ates a file usin
-000015b0: 6720 6120 5365 7152 6563 6f72 6420 2842  g a SeqRecord (B
-000015c0: 696f 7079 7468 6f6e 206f 626a 6563 7429  iopython object)
-000015d0: 206c 6973 742e 0a20 2020 200a 2020 2020   list..    .    
-000015e0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-000015f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7365  ---------.    se
-00001600: 7172 6563 6f72 645f 6c69 7374 203a 206c  qrecord_list : l
-00001610: 6973 7420 6f66 2053 6571 5265 636f 7264  ist of SeqRecord
-00001620: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
-00001630: 2053 6571 5265 636f 7264 2e0a 2020 2020   SeqRecord..    
-00001640: 6f75 7470 7574 5f66 696c 655f 6e61 6d65  output_file_name
-00001650: 203a 2073 7472 696e 670a 2020 2020 2020   : string.      
-00001660: 2020 4f75 7470 7574 2066 6173 7461 2066    Output fasta f
-00001670: 696c 6520 6e61 6d65 2e0a 2020 2020 2020  ile name..      
-00001680: 2020 0a20 2020 2045 7861 6d70 6c65 0a20    .    Example. 
-00001690: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-000016a0: 4578 706f 7274 2061 2053 6571 5265 636f  Export a SeqReco
-000016b0: 7264 206c 6973 7420 6173 2046 4153 5441  rd list as FASTA
-000016c0: 2066 696c 6520 6e61 6d65 6420 2774 6573   file named 'tes
-000016d0: 742e 6661 7374 6127 2e0a 0a20 2020 203e  t.fasta'...    >
-000016e0: 3e3e 2069 6d70 6f72 7420 6269 6f74 6578  >> import biotex
-000016f0: 7420 6173 2062 740a 2020 2020 3e3e 3e20  t as bt.    >>> 
-00001700: 7365 715f 6c69 7374 203d 205b 2741 4354  seq_list = ['ACT
-00001710: 4727 2c27 4754 4341 275d 0a20 2020 203e  G','GTCA'].    >
-00001720: 3e3e 2073 6571 7265 636f 7264 5f6c 6973  >> seqrecord_lis
-00001730: 7420 3d20 6274 2e66 6173 7461 746f 6f6c  t = bt.fastatool
-00001740: 732e 6372 6561 7465 5f73 6571 7265 636f  s.create_seqreco
-00001750: 7264 5f6c 6973 7428 7365 715f 6c69 7374  rd_list(seq_list
-00001760: 290a 2020 2020 3e3e 3e20 6274 2e66 6173  ).    >>> bt.fas
-00001770: 7461 746f 6f6c 732e 6578 706f 7274 5f66  tatools.export_f
-00001780: 6173 7461 2873 6571 7265 636f 7264 5f6c  asta(seqrecord_l
-00001790: 6973 742c 2774 6573 742e 6661 7374 6127  ist,'test.fasta'
-000017a0: 290a 2020 2020 4e63 0100 0000 0000 0000  ).    Nc........
-000017b0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-000017c0: 7316 0000 0067 007c 005d 0e7d 0174 007c  s....g.|.].}.t.|
-000017d0: 016a 0183 0191 0271 0453 0072 1c00 0000  .j.....q.S.r....
-000017e0: 2902 7224 0000 0072 2600 0000 2902 da02  ).r$...r&...)...
-000017f0: 2e30 7230 0000 0072 1c00 0000 721c 0000  .0r0...r....r...
-00001800: 0072 1d00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00001810: 703e de00 0000 7304 0000 0006 0002 007a  p>....s........z
-00001820: 2065 7870 6f72 745f 6661 7374 612e 3c6c   export_fasta.<l
-00001830: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00001840: 3e29 0172 3400 0000 7209 0000 0072 3f00  >).r4...r....r?.
-00001850: 0000 7201 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00001860: 007a 085b 5c77 2d5d 7b30 2ce9 6400 0000  .z.[\w-]{0,.d...
-00001870: fa01 7d29 0d72 2200 0000 723a 0000 0072  ..}).r"...r:...r
-00001880: 4000 0000 7241 0000 0072 2700 0000 7226  @...rA...r'...r&
-00001890: 0000 0072 2300 0000 7225 0000 0072 2400  ...r#...r%...r$.
-000018a0: 0000 722b 0000 00da 0766 696e 6461 6c6c  ..r+.....findall
-000018b0: 722d 0000 0072 1500 0000 2906 722e 0000  r-...r....).r...
-000018c0: 005a 106f 7574 7075 745f 6669 6c65 5f6e  .Z.output_file_n
-000018d0: 616d 6572 3400 0000 5a0a 6f75 7470 7574  amer4...Z.output
-000018e0: 4669 6c65 7230 0000 0072 2600 0000 721c  Filer0...r&...r.
-000018f0: 0000 0072 1c00 0000 721d 0000 00da 0c65  ...r....r......e
-00001900: 7870 6f72 745f 6661 7374 61c6 0000 0073  xport_fasta....s
-00001910: 1800 0000 0015 0802 0801 1602 0e01 0801  ................
-00001920: 0e01 1401 0a01 1801 0a01 0c01 724a 0000  ............rJ..
-00001930: 0067 0000 0000 0040 9f40 e902 0000 0072  .g.....@.@.....r
-00001940: 2100 0000 5a02 4141 6306 0000 0000 0000  !...Z.AAc.......
-00001950: 0000 0000 000b 0000 0008 0000 0043 0000  .............C..
-00001960: 0073 a600 0000 7a0e 7c00 6401 1900 6a00  .s....z.|.d...j.
-00001970: 0100 5700 6e1c 0400 7401 6b0a 722a 0100  ..W.n...t.k.r*..
-00001980: 0100 0100 7402 7c00 8301 7d00 5900 6e02  ....t.|...}.Y.n.
-00001990: 5800 6700 7d06 6700 7d07 7c00 4400 5d3a  X.g.}.g.}.|.D.]:
-000019a0: 7d08 7403 7404 7c08 6a00 8301 8301 7405  }.t.t.|.j.....t.
-000019b0: 7c03 8301 6b05 7268 7c06 a006 7c08 a101  |...k.rh|...|...
-000019c0: 0100 7c07 a006 6402 a101 0100 7138 7c07  ..|...d.....q8|.
-000019d0: a006 6403 a101 0100 7138 7407 a008 7403  ..d.....q8t...t.
-000019e0: 7c00 8301 6404 6602 a101 7d09 7409 7c06  |...d.f...}.t.|.
-000019f0: 7c01 7c02 7c03 7c04 7c05 6405 8d06 7d0a  |.|.|.|.|.d...}.
-00001a00: 7c0a 7c09 7c07 3c00 7c09 5300 2906 4e72  |.|.|.<.|.S.).Nr
-00001a10: 0100 0000 5446 6958 0200 0029 05da 086f  ....TFiX...)...o
-00001a20: 7274 685f 6d61 74da 0a63 6875 6e6b 5f73  rth_mat..chunk_s
-00001a30: 697a 65da 046d 6173 6bda 0a66 6173 7461  ize..mask..fasta
-00001a40: 5f74 7970 65da 066e 5f6a 6f62 7329 0a72  _type..n_jobs).r
-00001a50: 2600 0000 da0e 4174 7472 6962 7574 6545  &.....AttributeE
-00001a60: 7272 6f72 723a 0000 0072 2700 0000 7224  rrorr:...r'...r$
-00001a70: 0000 00da 0373 756d 7228 0000 0072 2900  .....sumr(...r).
-00001a80: 0000 da05 7a65 726f 7372 0700 0000 290b  ....zerosr....).
-00001a90: 722f 0000 0072 4c00 0000 724d 0000 0072  r/...rL...rM...r
-00001aa0: 4e00 0000 724f 0000 0072 5000 0000 5a09  N...rO...rP...Z.
-00001ab0: 6661 7374 615f 6175 785a 086d 696e 5f73  fasta_auxZ.min_s
-00001ac0: 697a 6572 3000 0000 da03 6d61 745a 076d  izer0.....matZ.m
-00001ad0: 6174 5f61 7578 721c 0000 0072 1c00 0000  at_auxr....r....
-00001ae0: 721d 0000 00da 0c66 6173 7461 5f74 6f5f  r......fasta_to_
-00001af0: 6d61 74ea 0000 0073 2600 0000 0002 0201  mat....s&.......
-00001b00: 0e01 0e01 0e01 0401 0401 0801 1601 0a01  ................
-00001b10: 0c02 0c02 1201 0801 0200 0200 02ff 0602  ................
-00001b20: 0802 7255 0000 0029 0172 0800 0000 2901  ..rU...).r....).
-00001b30: 4e29 014e 291b 720f 0000 0072 1600 0000  N).N).r....r....
-00001b40: 5a03 4269 6f72 0200 0000 7203 0000 005a  Z.Bior....r....Z
-00001b50: 0742 696f 2e53 6571 7204 0000 005a 0d42  .Bio.Seqr....Z.B
-00001b60: 696f 2e53 6571 5265 636f 7264 7205 0000  io.SeqRecordr...
-00001b70: 0072 2b00 0000 da05 6e75 6d70 7972 2900  .r+.....numpyr).
-00001b80: 0000 da05 7363 6970 7972 0600 0000 7240  ....scipyr....r@
-00001b90: 0000 00da 0573 7765 6570 7207 0000 0072  .....sweepr....r
-00001ba0: 1200 0000 721e 0000 0072 3200 0000 7235  ....r....r2...r5
-00001bb0: 0000 0072 3600 0000 723a 0000 0072 3d00  ...r6...r:...r=.
-00001bc0: 0000 7244 0000 0072 4a00 0000 7255 0000  ..rD...rJ...rU..
-00001bd0: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
-00001be0: 721d 0000 00da 083c 6d6f 6475 6c65 3e03  r......<module>.
-00001bf0: 0000 0073 2c00 0000 0801 0801 1001 0c01  ...s,...........
-00001c00: 0c01 0801 0801 0c01 0801 0c01 0802 0a0a  ................
-00001c10: 0819 0821 0821 0a2d 0808 081d 0a24 0c01  ...!.!.-.....$..
-00001c20: 0200 02ff                                ....
+00000020: 0003 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
+00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
+00000050: 0100 6401 6404 6c06 6d07 5a07 0100 6401  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 6401 6402 6c0a  d.l.m.Z...d.d.l.
+00000070: 5a0a 6401 6402 6c0b 5a0c 6401 6406 6c0d  Z.d.d.l.Z.d.d.l.
+00000080: 6d0e 5a0e 0100 6401 6402 6c0f 5a0f 6401  m.Z...d.d.l.Z.d.
+00000090: 6407 6c10 6d11 5a11 0100 6401 6402 6c12  d.l.m.Z...d.d.l.
+000000a0: 5a12 6401 6408 6c13 6d14 5a14 6d15 5a15  Z.d.d.l.m.Z.m.Z.
+000000b0: 0100 6409 640a 8400 5a16 641c 640b 640c  ..d.d...Z.d.d.d.
+000000c0: 8401 5a17 641c 640d 640e 8401 5a18 641d  ..Z.d.d.d...Z.d.
+000000d0: 6410 6411 8401 5a19 641e 6413 6414 8401  d.d...Z.d.d.d...
+000000e0: 5a1a 6415 6416 8400 5a1b 6417 6418 8400  Z.d.d...Z.d.d...
+000000f0: 5a1c 6700 6419 a201 6601 641a 641b 8401  Z.g.d...f.d.d...
+00000100: 5a1d 6402 5300 291f 61a4 0200 000a 5468  Z.d.S.).a.....Th
+00000110: 6973 206d 6f64 756c 6520 7072 6f76 6964  is module provid
+00000120: 6573 2066 756e 6374 696f 6e73 2066 6f72  es functions for
+00000130: 2077 6f72 6b69 6e67 2077 6974 6820 4641   working with FA
+00000140: 5354 4120 6669 6c65 7320 616e 6420 7065  STA files and pe
+00000150: 7266 6f72 6d69 6e67 0a73 6571 7565 6e63  rforming.sequenc
+00000160: 6520 616c 6967 6e6d 656e 742e 0a0a 4675  e alignment...Fu
+00000170: 6e63 7469 6f6e 733a 0a2d 2069 6d70 6f72  nctions:.- impor
+00000180: 745f 6661 7374 613a 2049 6d70 6f72 7420  t_fasta: Import 
+00000190: 6120 4641 5354 4120 6669 6c65 2075 7369  a FASTA file usi
+000001a0: 6e67 2042 696f 7079 7468 6f6e 2e0a 2d20  ng Biopython..- 
+000001b0: 6578 706f 7274 5f66 6173 7461 3a20 4578  export_fasta: Ex
+000001c0: 706f 7274 2061 2053 6571 5265 636f 7264  port a SeqRecord
+000001d0: 206c 6973 7420 6173 2061 2046 4153 5441   list as a FASTA
+000001e0: 2066 696c 652e 0a2d 2063 7265 6174 655f   file..- create_
+000001f0: 7365 7172 6563 6f72 645f 6c69 7374 3a20  seqrecord_list: 
+00000200: 4372 6561 7465 2061 2053 6571 5265 636f  Create a SeqReco
+00000210: 7264 206c 6973 7420 6672 6f6d 2061 2073  rd list from a s
+00000220: 7472 696e 6720 6c69 7374 2e0a 2d20 7275  tring list..- ru
+00000230: 6e5f 636c 7573 7461 6c6f 3a20 5275 6e20  n_clustalo: Run 
+00000240: 436c 7573 7461 6c20 4f6d 6567 6120 6d75  Clustal Omega mu
+00000250: 6c74 6970 6c65 2073 6571 7565 6e63 6520  ltiple sequence 
+00000260: 616c 6967 6e6d 656e 742e 0a2d 2067 6574  alignment..- get
+00000270: 5f63 6f6e 7365 6e73 7573 3a20 4765 7420  _consensus: Get 
+00000280: 7468 6520 636f 6e73 656e 7375 7320 7365  the consensus se
+00000290: 7175 656e 6365 2066 726f 6d20 6120 6c69  quence from a li
+000002a0: 7374 206f 6620 7365 7175 656e 6365 732e  st of sequences.
+000002b0: 0a2d 2067 6574 5f68 6561 6465 723a 2047  .- get_header: G
+000002c0: 6574 2074 6865 2068 6561 6465 7273 2066  et the headers f
+000002d0: 726f 6d20 6120 6c69 7374 206f 6620 5365  rom a list of Se
+000002e0: 7152 6563 6f72 6420 6f62 6a65 6374 732e  qRecord objects.
+000002f0: 0a2d 2067 6574 5f73 6571 3a20 4765 7420  .- get_seq: Get 
+00000300: 7468 6520 7365 7175 656e 6365 7320 6672  the sequences fr
+00000310: 6f6d 2061 206c 6973 7420 6f66 2053 6571  om a list of Seq
+00000320: 5265 636f 7264 206f 626a 6563 7473 2e0a  Record objects..
+00000330: 2d20 6661 7374 615f 746f 5f6d 6174 3a20  - fasta_to_mat: 
+00000340: 436f 6e76 6572 7420 4641 5354 4120 7365  Convert FASTA se
+00000350: 7175 656e 6365 7320 746f 2061 206d 6174  quences to a mat
+00000360: 7269 7820 7265 7072 6573 656e 7461 7469  rix representati
+00000370: 6f6e 2075 7369 6e67 2053 5765 6550 2e0a  on using SWeeP..
+00000380: 0a41 7574 686f 723a 2044 696f 676f 2064  .Author: Diogo d
+00000390: 6520 4a2e 2053 2e20 4d61 6368 6164 6f0a  e J. S. Machado.
+000003a0: 4461 7465 3a20 3133 2f30 372f 3230 3233  Date: 13/07/2023
+000003b0: 0ae9 0000 0000 4e29 02da 0741 6c69 676e  ......N)...Align
+000003c0: 494f da05 5365 7149 4f29 01da 0353 6571  IO..SeqIO)...Seq
+000003d0: 2901 da09 5365 7152 6563 6f72 6429 01da  )...SeqRecord)..
+000003e0: 0573 7461 7473 2901 da09 6661 7332 7377  .stats)...fas2sw
+000003f0: 6565 7029 02da 0a6c 696c 5f6d 6174 7269  eep)...lil_matri
+00000400: 78da 0e69 7373 706d 6174 7269 785f 6c69  x..isspmatrix_li
+00000410: 6c63 0100 0000 0000 0000 0000 0000 0300  lc..............
+00000420: 0000 0800 0000 4300 0000 7344 0000 0074  ......C...sD...t
+00000430: 00a0 017c 0064 0164 02a1 038f 117d 0174  ...|.d.d.....}.t
+00000440: 0274 03a0 047c 0164 03a1 0283 017d 0257  .t...|.d.....}.W
+00000450: 0064 0404 0004 0083 0301 007c 0253 0031  .d.........|.S.1
+00000460: 0073 1b77 0101 0001 0001 0059 0001 007c  .s.w.......Y...|
+00000470: 0253 0029 0561 7902 0000 0a20 2020 2055  .S.).ay....    U
+00000480: 7365 7320 6269 6f70 7974 686f 6e20 746f  ses biopython to
+00000490: 2069 6d70 6f72 7420 6120 4641 5354 4120   import a FASTA 
+000004a0: 6669 6c65 2e0a 2020 2020 0a20 2020 2050  file..    .    P
+000004b0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000004c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6e70  --------.    inp
+000004d0: 7574 5f66 696c 655f 6e61 6d65 203a 2073  ut_file_name : s
+000004e0: 7472 696e 6720 2876 616c 6964 2066 696c  tring (valid fil
+000004f0: 6520 6e61 6d65 290a 2020 2020 2020 2020  e name).        
+00000500: 496e 7075 7420 6661 7374 6120 6669 6c65  Input fasta file
+00000510: 206e 616d 652e 0a0a 2020 2020 5265 7475   name...    Retu
+00000520: 726e 730a 2020 2020 2d2d 2d2d 2d2d 2d0a  rns.    -------.
+00000530: 2020 2020 7365 7172 6563 6f72 645f 6c69      seqrecord_li
+00000540: 7374 203a 206c 6973 7420 6f66 2053 6571  st : list of Seq
+00000550: 5265 636f 7264 0a20 2020 2020 2020 204c  Record.        L
+00000560: 6973 7420 6f66 2053 6571 5265 636f 7264  ist of SeqRecord
+00000570: 2069 6d70 6f72 7465 6420 6672 6f6d 2066   imported from f
+00000580: 696c 652e 0a20 2020 2020 2020 200a 2020  ile..        .  
+00000590: 2020 4578 616d 706c 650a 2020 2020 2d2d    Example.    --
+000005a0: 2d2d 2d2d 2d0a 2020 2020 496d 706f 7274  -----.    Import
+000005b0: 2061 2046 4153 5441 2066 696c 6520 6e61   a FASTA file na
+000005c0: 6d65 6420 2773 6571 7565 6e63 6573 2e66  med 'sequences.f
+000005d0: 6173 7461 272e 0a0a 2020 2020 3e3e 3e20  asta'...    >>> 
+000005e0: 696d 706f 7274 2062 696f 7465 7874 2061  import biotext a
+000005f0: 7320 6274 0a20 2020 203e 3e3e 2069 6e70  s bt.    >>> inp
+00000600: 7574 5f66 696c 6520 3d20 2773 6571 7565  ut_file = 'seque
+00000610: 6e63 6573 2e66 6173 7461 270a 2020 2020  nces.fasta'.    
+00000620: 3e3e 3e20 6661 7374 6120 3d20 6274 2e66  >>> fasta = bt.f
+00000630: 6173 7461 746f 6f6c 732e 696d 706f 7274  astatools.import
+00000640: 5f66 6173 7461 2869 6e70 7574 5f66 696c  _fasta(input_fil
+00000650: 6529 0a20 2020 203e 3e3e 2070 7269 6e74  e).    >>> print
+00000660: 2866 6173 7461 5b30 5d29 2023 2070 7269  (fasta[0]) # pri
+00000670: 6e74 2066 6972 7374 2073 6571 7565 6e63  nt first sequenc
+00000680: 6520 696e 2069 6e70 7574 2066 696c 650a  e in input file.
+00000690: 2020 2020 4944 3a20 310a 2020 2020 4e61      ID: 1.    Na
+000006a0: 6d65 3a20 310a 2020 2020 4465 7363 7269  me: 1.    Descri
+000006b0: 7074 696f 6e3a 2031 0a20 2020 204e 756d  ption: 1.    Num
+000006c0: 6265 7220 6f66 2066 6561 7475 7265 733a  ber of features:
+000006d0: 2030 0a20 2020 2053 6571 2827 4859 454c   0.    Seq('HYEL
+000006e0: 4c59 5159 5359 5759 5152 4c44 2729 0a20  LYQYSYWYQRLD'). 
+000006f0: 2020 20da 0172 fa05 7574 662d 38da 0566     ..r..utf-8..f
+00000700: 6173 7461 4e29 05da 0663 6f64 6563 73da  astaN)...codecs.
+00000710: 046f 7065 6eda 046c 6973 7472 0300 0000  .open..listr....
+00000720: da05 7061 7273 6529 03da 0f69 6e70 7574  ..parse)...input
+00000730: 5f66 696c 655f 6e61 6d65 da01 66da 0e73  _file_name..f..s
+00000740: 6571 7265 636f 7264 5f6c 6973 74a9 0072  eqrecord_list..r
+00000750: 1400 0000 fa2f 6275 696c 645c 6264 6973  ...../build\bdis
+00000760: 742e 7769 6e2d 616d 6436 345c 6567 675c  t.win-amd64\egg\
+00000770: 6269 6f74 6578 745c 6661 7374 6174 6f6f  biotext\fastatoo
+00000780: 6c73 2e70 79da 0c69 6d70 6f72 745f 6661  ls.py..import_fa
+00000790: 7374 6121 0000 0073 0c00 0000 101d 1201  sta!...s........
+000007a0: 0aff 0402 10fe 0402 7216 0000 0063 0300  ........r....c..
+000007b0: 0000 0000 0000 0000 0000 0600 0000 0600  ................
+000007c0: 0000 4300 0000 73a2 0000 0074 007c 0083  ..C...s....t.|..
+000007d0: 017d 007c 0264 016b 0372 1374 0164 0264  .}.|.d.k.r.t.d.d
+000007e0: 0384 007c 0044 0083 017c 0264 048d 027d  ...|.D...|.d...}
+000007f0: 0074 02a0 037c 0164 0564 06a1 037d 037c  .t...|.d.d...}.|
+00000800: 0044 005d 2e7d 0474 047c 046a 0583 0164  .D.].}.t.|.j...d
+00000810: 076b 0472 4a7c 03a0 0664 087c 046a 0717  .k.rJ|...d.|.j..
+00000820: 0064 0917 00a1 0101 0074 087c 046a 0583  .d.......t.|.j..
+00000830: 017d 0574 09a0 0a64 0a74 0864 0b83 0117  .}.t...d.t.d....
+00000840: 0064 0c17 007c 05a1 027d 0564 09a0 0b7c  .d...|...}.d...|
+00000850: 05a1 017d 057c 03a0 067c 05a1 0101 0071  ...}.|...|.....q
+00000860: 1c7c 03a0 0ca1 0001 0064 0153 0029 0d61  .|.......d.S.).a
+00000870: 1702 0000 0a20 2020 2043 7265 6174 6520  .....    Create 
+00000880: 6120 6669 6c65 2075 7369 6e67 2061 2053  a file using a S
+00000890: 6571 5265 636f 7264 2028 4269 6f70 7974  eqRecord (Biopyt
+000008a0: 686f 6e20 6f62 6a65 6374 2920 6c69 7374  hon object) list
+000008b0: 2e0a 2020 2020 0a20 2020 2050 6172 616d  ..    .    Param
+000008c0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000008d0: 2d2d 2d2d 0a20 2020 206f 7574 7075 745f  ----.    output_
+000008e0: 6669 6c65 5f6e 616d 6520 3a20 7374 7269  file_name : stri
+000008f0: 6e67 0a20 2020 2020 2020 204f 7574 7075  ng.        Outpu
+00000900: 7420 6661 7374 6120 6669 6c65 206e 616d  t fasta file nam
+00000910: 652e 0a20 2020 2073 6571 7265 636f 7264  e..    seqrecord
+00000920: 5f6c 6973 7420 3a20 6c69 7374 206f 6620  _list : list of 
+00000930: 5365 7152 6563 6f72 640a 2020 2020 2020  SeqRecord.      
+00000940: 2020 4c69 7374 206f 6620 5365 7152 6563    List of SeqRec
+00000950: 6f72 642e 0a20 2020 2020 2020 200a 2020  ord..        .  
+00000960: 2020 4578 616d 706c 650a 2020 2020 2d2d    Example.    --
+00000970: 2d2d 2d2d 2d2d 0a20 2020 2045 7870 6f72  ------.    Expor
+00000980: 7420 6120 5365 7152 6563 6f72 6420 6c69  t a SeqRecord li
+00000990: 7374 2061 7320 4641 5354 4120 6669 6c65  st as FASTA file
+000009a0: 206e 616d 6564 2027 7365 7175 656e 6365   named 'sequence
+000009b0: 732e 6661 7374 6127 2e0a 0a20 2020 203e  s.fasta'...    >
+000009c0: 3e3e 2069 6d70 6f72 7420 6269 6f74 6578  >> import biotex
+000009d0: 7420 6173 2062 740a 2020 2020 3e3e 3e20  t as bt.    >>> 
+000009e0: 7365 715f 6c69 7374 203d 205b 2741 4354  seq_list = ['ACT
+000009f0: 4727 2c27 4754 4341 275d 0a20 2020 203e  G','GTCA'].    >
+00000a00: 3e3e 2073 6571 7265 636f 7264 5f6c 6973  >> seqrecord_lis
+00000a10: 7420 3d20 6274 2e66 6173 7461 746f 6f6c  t = bt.fastatool
+00000a20: 732e 6372 6561 7465 5f73 6571 7265 636f  s.create_seqreco
+00000a30: 7264 5f6c 6973 7428 7365 715f 6c69 7374  rd_list(seq_list
+00000a40: 290a 2020 2020 3e3e 3e20 6274 2e66 6173  ).    >>> bt.fas
+00000a50: 7461 746f 6f6c 732e 6578 706f 7274 5f66  tatools.export_f
+00000a60: 6173 7461 2873 6571 7265 636f 7264 5f6c  asta(seqrecord_l
+00000a70: 6973 742c 2773 6571 7565 6e63 6573 2e66  ist,'sequences.f
+00000a80: 6173 7461 2729 0a20 2020 204e 6301 0000  asta').    Nc...
+00000a90: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000aa0: 0053 0000 0073 1600 0000 6700 7c00 5d07  .S...s....g.|.].
+00000ab0: 7d01 7400 7c01 6a01 8301 9102 7102 5300  }.t.|.j.....q.S.
+00000ac0: 7214 0000 0029 02da 0373 7472 da03 7365  r....)...str..se
+00000ad0: 7129 02da 022e 30da 0169 7214 0000 0072  q)....0..ir....r
+00000ae0: 1400 0000 7215 0000 00da 0a3c 6c69 7374  ....r......<list
+00000af0: 636f 6d70 3e5a 0000 0073 0200 0000 1600  comp>Z...s......
+00000b00: 7a20 6578 706f 7274 5f66 6173 7461 2e3c  z export_fasta.<
+00000b10: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000b20: 703e 2901 da06 6865 6164 6572 da01 7772  p>)...header..wr
+00000b30: 0b00 0000 7201 0000 00fa 013e da01 0a7a  ....r......>...z
+00000b40: 085b 5c77 2d5d 7b30 2ce9 6400 0000 da01  .[\w-]{0,.d.....
+00000b50: 7d29 0d72 0f00 0000 da15 6372 6561 7465  }).r......create
+00000b60: 5f73 6571 7265 636f 7264 5f6c 6973 7472  _seqrecord_listr
+00000b70: 0d00 0000 720e 0000 00da 036c 656e 7218  ....r......lenr.
+00000b80: 0000 00da 0577 7269 7465 da0b 6465 7363  .....write..desc
+00000b90: 7269 7074 696f 6e72 1700 0000 da02 7265  riptionr......re
+00000ba0: da07 6669 6e64 616c 6cda 046a 6f69 6eda  ..findall..join.
+00000bb0: 0563 6c6f 7365 2906 7213 0000 005a 106f  .close).r....Z.o
+00000bc0: 7574 7075 745f 6669 6c65 5f6e 616d 6572  utput_file_namer
+00000bd0: 1c00 0000 5a0a 6f75 7470 7574 4669 6c65  ....Z.outputFile
+00000be0: 721a 0000 0072 1800 0000 7214 0000 0072  r....r....r....r
+00000bf0: 1400 0000 7215 0000 00da 0c65 7870 6f72  ....r......expor
+00000c00: 745f 6661 7374 6142 0000 0073 1a00 0000  t_fastaB...s....
+00000c10: 0815 0802 1601 0e02 0801 0e01 1401 0a01  ................
+00000c20: 1801 0a01 0a01 0280 0c01 722a 0000 0063  ..........r*...c
+00000c30: 0200 0000 0000 0000 0000 0000 0700 0000  ................
+00000c40: 0600 0000 4300 0000 7376 0000 007c 0164  ....C...sv...|.d
+00000c50: 016b 0272 0f74 0074 0164 0274 027c 0083  .k.r.t.t.d.t.|..
+00000c60: 0164 0217 0083 0283 017d 0167 007d 0274  .d.......}.g.}.t
+00000c70: 0164 0374 027c 0083 0183 0244 005d 207d  .d.t.|.....D.] }
+00000c80: 0374 037c 017c 0319 0083 017d 0474 04a0  .t.|.|.....}.t..
+00000c90: 0564 047c 04a1 0264 0319 007d 0574 0674  .d.|...d...}.t.t
+00000ca0: 077c 007c 0319 0083 017c 047c 0564 058d  .|.|.....|.|.d..
+00000cb0: 037d 067c 02a0 087c 06a1 0101 0071 187c  .}.|...|.....q.|
+00000cc0: 0253 0029 0661 7f03 0000 0a20 2020 2043  .S.).a.....    C
+00000cd0: 7265 6174 6520 6120 6c69 7374 206f 6620  reate a list of 
+00000ce0: 5365 7152 6563 6f72 6420 2842 696f 7079  SeqRecord (Biopy
+00000cf0: 7468 6f6e 206f 626a 6563 7429 2077 6974  thon object) wit
+00000d00: 6820 6120 7374 7269 6e67 206c 6973 742e  h a string list.
+00000d10: 0a20 2020 200a 2020 2020 5061 7261 6d65  .    .    Parame
+00000d20: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00000d30: 2d2d 2d0a 2020 2020 7365 715f 6c69 7374  ---.    seq_list
+00000d40: 203a 206c 6973 7420 6f66 2073 7472 696e   : list of strin
+00000d50: 670a 2020 2020 2020 2020 4c69 7374 206f  g.        List o
+00000d60: 6620 6269 6f6c 6f67 6963 616c 2073 6571  f biological seq
+00000d70: 7565 6e63 6573 2069 6e20 7374 7269 6e67  uences in string
+00000d80: 2066 6f72 6d61 742e 0a20 2020 2068 6561   format..    hea
+00000d90: 6465 7220 3a20 6c69 7374 206f 6620 7374  der : list of st
+00000da0: 7269 6e67 0a20 2020 2020 2020 204c 6973  ring.        Lis
+00000db0: 7420 6f66 2068 6561 6465 7273 2069 6e20  t of headers in 
+00000dc0: 7374 7269 6e67 2066 6f72 6d61 742c 2069  string format, i
+00000dd0: 6620 7365 7420 746f 2027 4e6f 6e65 2720  f set to 'None' 
+00000de0: 7468 6520 6865 6164 6572 7320 7769 6c6c  the headers will
+00000df0: 200a 2020 2020 2020 2020 6265 2061 7574   .        be aut
+00000e00: 6f6d 6174 6963 616c 6c79 2064 6566 696e  omatically defin
+00000e10: 6564 2077 6974 6820 6e75 6d62 6572 7320  ed with numbers 
+00000e20: 696e 2069 6e63 7265 6173 696e 6720 6f72  in increasing or
+00000e30: 6465 722e 0a0a 2020 2020 5265 7475 726e  der...    Return
+00000e40: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
+00000e50: 2020 7365 7172 6563 6f72 645f 6c69 7374    seqrecord_list
+00000e60: 203a 206c 6973 7420 6f66 2053 6571 5265   : list of SeqRe
+00000e70: 636f 7264 0a20 2020 2020 2020 204c 6973  cord.        Lis
+00000e80: 7420 6f66 2053 6571 5265 636f 7264 2e0a  t of SeqRecord..
+00000e90: 2020 2020 2020 2020 0a20 2020 2045 7861          .    Exa
+00000ea0: 6d70 6c65 0a20 2020 202d 2d2d 2d2d 2d2d  mple.    -------
+00000eb0: 0a20 2020 2044 6563 6f64 6520 6120 7374  .    Decode a st
+00000ec0: 7269 6e67 2e0a 0a20 2020 203e 3e3e 2069  ring...    >>> i
+00000ed0: 6d70 6f72 7420 6269 6f74 6578 7420 6173  mport biotext as
+00000ee0: 2062 740a 2020 2020 3e3e 3e20 7365 715f   bt.    >>> seq_
+00000ef0: 6c69 7374 203d 205b 2741 4354 4727 2c27  list = ['ACTG','
+00000f00: 4754 4341 275d 0a20 2020 203e 3e3e 2073  GTCA'].    >>> s
+00000f10: 6571 7265 636f 7264 5f6c 6973 7420 3d20  eqrecord_list = 
+00000f20: 6274 2e66 6173 7461 746f 6f6c 732e 6372  bt.fastatools.cr
+00000f30: 6561 7465 5f73 6571 7265 636f 7264 5f6c  eate_seqrecord_l
+00000f40: 6973 7428 7365 715f 6c69 7374 290a 2020  ist(seq_list).  
+00000f50: 2020 3e3e 3e20 666f 7220 6920 696e 2073    >>> for i in s
+00000f60: 6571 7265 636f 7264 5f6c 6973 743a 0a20  eqrecord_list:. 
+00000f70: 2020 203e 3e3e 2020 2020 2070 7269 6e74     >>>     print
+00000f80: 2028 6929 0a20 2020 2049 443a 2031 0a20   (i).    ID: 1. 
+00000f90: 2020 204e 616d 653a 203c 756e 6b6e 6f77     Name: <unknow
+00000fa0: 6e20 6e61 6d65 3e0a 2020 2020 4465 7363  n name>.    Desc
+00000fb0: 7269 7074 696f 6e3a 2031 0a20 2020 204e  ription: 1.    N
+00000fc0: 756d 6265 7220 6f66 2066 6561 7475 7265  umber of feature
+00000fd0: 733a 2030 0a20 2020 2053 6571 2827 4143  s: 0.    Seq('AC
+00000fe0: 5447 2729 0a20 2020 2049 443a 2032 0a20  TG').    ID: 2. 
+00000ff0: 2020 204e 616d 653a 203c 756e 6b6e 6f77     Name: <unknow
+00001000: 6e20 6e61 6d65 3e0a 2020 2020 4465 7363  n name>.    Desc
+00001010: 7269 7074 696f 6e3a 2032 0a20 2020 204e  ription: 2.    N
+00001020: 756d 6265 7220 6f66 2066 6561 7475 7265  umber of feature
+00001030: 733a 2030 0a20 2020 2053 6571 2827 4754  s: 0.    Seq('GT
+00001040: 4341 2729 0a20 2020 204e e901 0000 0072  CA').    N.....r
+00001050: 0100 0000 7a03 5c73 2b29 0272 2500 0000  ....z.\s+).r%...
+00001060: da02 6964 2909 720f 0000 00da 0572 616e  ..id).r......ran
+00001070: 6765 7223 0000 0072 1700 0000 7226 0000  ger#...r....r&..
+00001080: 00da 0573 706c 6974 7205 0000 0072 0400  ...splitr....r..
+00001090: 0000 da06 6170 7065 6e64 2907 da08 7365  ....append)...se
+000010a0: 715f 6c69 7374 da0b 6865 6164 6572 5f6c  q_list..header_l
+000010b0: 6973 7472 1300 0000 721a 0000 0072 2500  istr....r....r%.
+000010c0: 0000 da05 6964 656e 74da 0672 6563 6f72  ....ident..recor
+000010d0: 6472 1400 0000 7214 0000 0072 1500 0000  dr....r....r....
+000010e0: 7222 0000 0066 0000 0073 1600 0000 0825  r"...f...s.....%
+000010f0: 1601 0401 1201 0c01 1001 0e01 0201 06ff  ................
+00001100: 0c02 0401 7222 0000 00da 0063 0200 0000  ....r".....c....
+00001110: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+00001120: 4300 0000 7364 0000 0074 006a 0164 0164  C...sd...t.j.d.d
+00001130: 0264 038d 027d 0264 047c 0017 0064 0517  .d...}.d.|...d..
+00001140: 007c 026a 0217 0064 0617 007d 037c 0364  .|.j...d...}.|.d
+00001150: 077c 0117 0037 007d 0374 036a 047c 0364  .|...7.}.t.j.|.d
+00001160: 0864 098d 0201 0074 05a0 067c 026a 0264  .d.....t...|.j.d
+00001170: 0aa1 027d 047c 02a0 07a1 0001 0074 08a0  ...}.|.......t..
+00001180: 097c 026a 02a1 0101 007c 0453 0029 0b61  .|.j.....|.S.).a
+00001190: 0203 0000 0a20 2020 2052 756e 2043 6c75  .....    Run Clu
+000011a0: 7374 616c 204f 6d65 6761 206d 756c 7469  stal Omega multi
+000011b0: 706c 6520 7365 7175 656e 6365 2061 6c69  ple sequence ali
+000011c0: 676e 6d65 6e74 206f 6e20 7468 6520 696e  gnment on the in
+000011d0: 7075 7420 6669 6c65 2e0a 0a20 2020 2050  put file...    P
+000011e0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+000011f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6e70  --------.    inp
+00001200: 7574 5f66 696c 655f 6e61 6d65 203a 2073  ut_file_name : s
+00001210: 7472 0a20 2020 2020 2020 2050 6174 6820  tr.        Path 
+00001220: 746f 2074 6865 2069 6e70 7574 2066 696c  to the input fil
+00001230: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
+00001240: 2073 6571 7565 6e63 6573 2074 6f20 616c   sequences to al
+00001250: 6967 6e2e 0a20 2020 2061 7267 7320 3a20  ign..    args : 
+00001260: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+00001270: 2020 2020 2020 4164 6469 7469 6f6e 616c        Additional
+00001280: 2061 7267 756d 656e 7473 2074 6f20 7061   arguments to pa
+00001290: 7373 2074 6f20 436c 7573 7461 6c20 4f6d  ss to Clustal Om
+000012a0: 6567 612e 2044 6566 6175 6c74 7320 746f  ega. Defaults to
+000012b0: 2061 6e20 656d 7074 7920 7374 7269 6e67   an empty string
+000012c0: 2e0a 0a20 2020 204f 7574 7075 740a 2020  ...    Output.  
+000012d0: 2020 2d2d 2d2d 2d2d 0a20 2020 2061 6c69    ------.    ali
+000012e0: 676e 203a 2042 696f 2e41 6c69 676e 2e4d  gn : Bio.Align.M
+000012f0: 756c 7469 706c 6553 6571 416c 6967 6e6d  ultipleSeqAlignm
+00001300: 656e 740a 2020 2020 2020 2020 416c 6967  ent.        Alig
+00001310: 6e65 6420 7365 7175 656e 6365 7320 696e  ned sequences in
+00001320: 2074 6865 2043 6c75 7374 616c 2066 6f72   the Clustal for
+00001330: 6d61 742e 0a0a 2020 2020 4578 616d 706c  mat...    Exampl
+00001340: 650a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  e.    -------.  
+00001350: 2020 5065 7266 6f72 6d20 6d75 6c74 6970    Perform multip
+00001360: 6c65 2073 6571 7565 6e63 6520 616c 6967  le sequence alig
+00001370: 6e6d 656e 7420 7573 696e 6720 436c 7573  nment using Clus
+00001380: 7461 6c20 4f6d 6567 613a 0a0a 2020 2020  tal Omega:..    
+00001390: 3e3e 3e20 696d 706f 7274 2062 696f 7465  >>> import biote
+000013a0: 7874 2061 7320 6274 0a20 2020 203e 3e3e  xt as bt.    >>>
+000013b0: 2069 6e70 7574 5f66 696c 6520 3d20 2773   input_file = 's
+000013c0: 6571 7565 6e63 6573 2e66 6173 7461 270a  equences.fasta'.
+000013d0: 2020 2020 3e3e 3e20 616c 6967 6e6d 656e      >>> alignmen
+000013e0: 7420 3d20 6274 2e66 6173 7461 746f 6f6c  t = bt.fastatool
+000013f0: 732e 7275 6e5f 636c 7573 7461 6c6f 2869  s.run_clustalo(i
+00001400: 6e70 7574 5f66 696c 6529 0a20 2020 203e  nput_file).    >
+00001410: 3e3e 2070 7269 6e74 2861 6c69 676e 6d65  >> print(alignme
+00001420: 6e74 290a 2020 2020 416c 6967 6e6d 656e  nt).    Alignmen
+00001430: 7420 7769 7468 2033 2072 6f77 7320 616e  t with 3 rows an
+00001440: 6420 3136 2063 6f6c 756d 6e73 0a20 2020  d 16 columns.   
+00001450: 2048 5945 4c4c 5951 5953 5957 5951 524c   HYELLYQYSYWYQRL
+00001460: 4420 310a 2020 2020 4859 454c 4c59 512d  D 1.    HYELLYQ-
+00001470: 2d2d 2d2d 2d2d 2d2d 2032 0a20 2020 202d  -------- 2.    -
+00001480: 2d2d 2d2d 2d2d 2d2d 5957 5951 524c 4420  --------YWYQRLD 
+00001490: 330a 2020 2020 721d 0000 0046 a902 da04  3.    r....F....
+000014a0: 6d6f 6465 da06 6465 6c65 7465 7a0c 636c  mode..deletez.cl
+000014b0: 7573 7461 6c6f 202d 6920 7a04 202d 6f20  ustalo -i z. -o 
+000014c0: 7a1c 202d 2d61 7574 6f20 2d2d 6f75 7466  z. --auto --outf
+000014d0: 6d74 2063 6c75 202d 2d66 6f72 6365 fa01  mt clu --force..
+000014e0: 2054 2901 da05 7368 656c 6c5a 0763 6c75   T)...shellZ.clu
+000014f0: 7374 616c 290a da08 7465 6d70 6669 6c65  stal)...tempfile
+00001500: da0d 5465 6d70 6f72 6172 7946 696c 65da  ..TemporaryFile.
+00001510: 046e 616d 65da 0a73 7562 7072 6f63 6573  .name..subproces
+00001520: 73da 0463 616c 6c72 0200 0000 da04 7265  s..callr......re
+00001530: 6164 7229 0000 00da 026f 73da 0675 6e6c  adr).....os..unl
+00001540: 696e 6b29 0572 1100 0000 da04 6172 6773  ink).r......args
+00001550: da02 6670 5a0a 636d 645f 7374 7269 6e67  ..fpZ.cmd_string
+00001560: da05 616c 6967 6e72 1400 0000 7214 0000  ..alignr....r...
+00001570: 0072 1500 0000 da0c 7275 6e5f 636c 7573  .r......run_clus
+00001580: 7461 6c6f 9600 0000 7310 0000 000e 1e16  talo....s.......
+00001590: 030c 010e 030e 0308 030c 0104 0372 4500  .............rE.
+000015a0: 0000 4663 0200 0000 0000 0000 0000 0000  ..Fc............
+000015b0: 0900 0000 0800 0000 4300 0000 7332 0100  ........C...s2..
+000015c0: 0074 007c 0083 017d 007a 077c 0064 0119  .t.|...}.z.|.d..
+000015d0: 006a 0101 0057 006e 0d04 0074 0279 1801  .j...W.n...t.y..
+000015e0: 0001 0001 0074 037c 0083 017d 0059 006e  .....t.|...}.Y.n
+000015f0: 0177 0074 046a 0564 0264 0364 048d 027d  .w.t.j.d.d.d...}
+00001600: 027c 0044 005d 157d 037c 02a0 0664 0574  .|.D.].}.|...d.t
+00001610: 077c 036a 0183 0117 0064 0617 0074 077c  .|.j.....d...t.|
+00001620: 036a 0883 0117 0064 0617 00a1 0101 0071  .j.....d.......q
+00001630: 227c 02a0 09a1 0001 0067 007d 0474 0a7c  "|.......g.}.t.|
+00001640: 0083 0164 076b 0472 8374 0b7c 026a 0c83  ...d.k.r.t.|.j..
+00001650: 017d 0567 007d 067c 0544 005d 127d 037c  .}.g.}.|.D.].}.|
+00001660: 06a0 0d74 007c 036a 0883 01a1 0101 007c  ...t.|.j.......|
+00001670: 04a0 0d74 077c 036a 0883 01a1 0101 0071  ...t.|.j.......q
+00001680: 4d74 0ea0 0f7c 06a1 017d 0674 10a0 117c  Mt...|...}.t...|
+00001690: 06a1 017d 077c 0764 0119 007c 0764 0719  ...}.|.d...|.d..
+000016a0: 0064 016b 0519 007d 0764 08a0 127c 07a1  .d.k...}.d...|..
+000016b0: 017d 087c 0173 8274 13a0 1464 0964 087c  .}.|.s.t...d.d.|
+000016c0: 08a1 037d 086e 0c74 077c 0064 0119 006a  ...}.n.t.|.d...j
+000016d0: 0883 017d 087c 04a0 0d7c 08a1 0101 0074  ...}.|...|.....t
+000016e0: 15a0 167c 026a 0ca1 0101 007c 087c 0466  ...|.j.....|.|.f
+000016f0: 0253 0029 0a61 4b04 0000 0a20 2020 2047  .S.).aK....    G
+00001700: 6574 2074 6865 2063 6f6e 7365 6e73 7573  et the consensus
+00001710: 2073 6571 7565 6e63 6520 6672 6f6d 2061   sequence from a
+00001720: 206c 6973 7420 6f66 2073 6571 7565 6e63   list of sequenc
+00001730: 6573 2e0a 0a20 2020 2050 6172 616d 6574  es...    Paramet
+00001740: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+00001750: 2d2d 0a20 2020 2073 6571 5f6c 6973 7420  --.    seq_list 
+00001760: 3a20 6c69 7374 0a20 2020 2020 2020 204c  : list.        L
+00001770: 6973 7420 6f66 2073 6571 7565 6e63 6573  ist of sequences
+00001780: 2069 6e20 5365 7152 6563 6f72 6420 6f62   in SeqRecord ob
+00001790: 6a65 6374 2066 6f72 6d61 7420 6f72 2061  ject format or a
+000017a0: 7320 7374 7269 6e67 732e 0a20 2020 2070  s strings..    p
+000017b0: 7265 7365 7276 655f 6761 7020 3a20 626f  reserve_gap : bo
+000017c0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+000017d0: 2020 2020 2049 6620 5472 7565 2c20 7468       If True, th
+000017e0: 6520 636f 6e73 656e 7375 7320 7365 7175  e consensus sequ
+000017f0: 656e 6365 206d 6179 2063 6f6e 7461 696e  ence may contain
+00001800: 2067 6170 7320 2822 2d22 2920 6261 7365   gaps ("-") base
+00001810: 6420 6f6e 2074 6865 206d 616a 6f72 6974  d on the majorit
+00001820: 7920 6368 6172 6163 7465 7273 2061 6e64  y characters and
+00001830: 2074 6865 2067 6170 7320 7072 6573 656e   the gaps presen
+00001840: 7420 696e 2074 6865 2061 6c69 676e 6564  t in the aligned
+00001850: 2073 6571 7565 6e63 6573 2e20 0a20 2020   sequences. .   
+00001860: 2020 2020 2049 6620 4661 6c73 652c 2074       If False, t
+00001870: 6865 2063 6f6e 7365 6e73 7573 2073 6571  he consensus seq
+00001880: 7565 6e63 6520 6973 2064 6574 6572 6d69  uence is determi
+00001890: 6e65 6420 7769 7468 6f75 7420 6761 7073  ned without gaps
+000018a0: 2062 7920 636f 6e73 6964 6572 696e 6720   by considering 
+000018b0: 6f6e 6c79 2074 6865 206d 616a 6f72 6974  only the majorit
+000018c0: 7920 6368 6172 6163 7465 7273 2e0a 0a20  y characters... 
+000018d0: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+000018e0: 2d2d 2d2d 2d2d 0a20 2020 2063 6f6e 7365  ------.    conse
+000018f0: 6e73 7573 203a 2073 7472 0a20 2020 2020  nsus : str.     
+00001900: 2020 2043 6f6e 7365 6e73 7573 2073 6571     Consensus seq
+00001910: 7565 6e63 6520 6261 7365 6420 6f6e 2074  uence based on t
+00001920: 6865 206d 616a 6f72 6974 7920 6368 6172  he majority char
+00001930: 6163 7465 7273 2c20 7769 7468 206f 7220  acters, with or 
+00001940: 7769 7468 6f75 7420 6761 7073 2028 222d  without gaps ("-
+00001950: 2229 2064 6570 656e 6469 6e67 206f 6e20  ") depending on 
+00001960: 7468 6520 6070 7265 7365 7276 655f 6761  the `preserve_ga
+00001970: 7060 2070 6172 616d 6574 6572 2e0a 2020  p` parameter..  
+00001980: 2020 616c 6967 6e20 3a20 6c69 7374 0a20    align : list. 
+00001990: 2020 2020 2020 204c 6973 7420 6f66 2061         List of a
+000019a0: 6c69 676e 6564 2073 6571 7565 6e63 6573  ligned sequences
+000019b0: 2e0a 0a20 2020 2045 7861 6d70 6c65 0a20  ...    Example. 
+000019c0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2043     -------.    C
+000019d0: 616c 6375 6c61 7465 2074 6865 2063 6f6e  alculate the con
+000019e0: 7365 6e73 7573 2073 6571 7565 6e63 6520  sensus sequence 
+000019f0: 6672 6f6d 2061 206c 6973 7420 6f66 2073  from a list of s
+00001a00: 6571 7565 6e63 6573 3a0a 0a20 2020 203e  equences:..    >
+00001a10: 3e3e 2069 6d70 6f72 7420 6269 6f74 6578  >> import biotex
+00001a20: 7420 6173 2062 740a 2020 2020 3e3e 3e20  t as bt.    >>> 
+00001a30: 7365 715f 6c69 7374 203d 205b 2741 4354  seq_list = ['ACT
+00001a40: 4727 2c20 2741 4354 4327 2c20 2741 4343  G', 'ACTC', 'ACC
+00001a50: 4327 2c20 2741 4343 275d 0a20 2020 203e  C', 'ACC'].    >
+00001a60: 3e3e 2063 6f6e 7365 6e73 7573 2c20 616c  >> consensus, al
+00001a70: 6967 6e20 3d20 6274 2e66 6173 7461 746f  ign = bt.fastato
+00001a80: 6f6c 732e 6765 745f 636f 6e73 656e 7375  ols.get_consensu
+00001a90: 7328 7365 715f 6c69 7374 2c20 7072 6573  s(seq_list, pres
+00001aa0: 6572 7665 5f67 6170 3d54 7275 6529 0a20  erve_gap=True). 
+00001ab0: 2020 203e 3e3e 2070 7269 6e74 2827 436f     >>> print('Co
+00001ac0: 6e73 656e 7375 733a 2027 2c20 636f 6e73  nsensus: ', cons
+00001ad0: 656e 7375 7329 0a20 2020 203e 3e3e 2070  ensus).    >>> p
+00001ae0: 7269 6e74 2827 416c 6967 6e6d 656e 743a  rint('Alignment:
+00001af0: 2027 2c20 616c 6967 6e29 0a20 2020 2043   ', align).    C
+00001b00: 6f6e 7365 6e73 7573 3a20 2041 4343 430a  onsensus:  ACCC.
+00001b10: 2020 2020 416c 6967 6e6d 656e 743a 2020      Alignment:  
+00001b20: 5b27 4143 5447 272c 2027 4143 5443 272c  ['ACTG', 'ACTC',
+00001b30: 2027 4143 4343 272c 2027 4143 432d 275d   'ACCC', 'ACC-']
+00001b40: 0a20 2020 2072 0100 0000 721d 0000 0046  .    r....r....F
+00001b50: 7235 0000 0072 1e00 0000 721f 0000 0072  r5...r....r....r
+00001b60: 2b00 0000 7234 0000 007a 035c 2d2b 2917  +...r4...z.\-+).
+00001b70: 720f 0000 0072 2500 0000 da0e 4174 7472  r....r%.....Attr
+00001b80: 6962 7574 6545 7272 6f72 7222 0000 0072  ibuteErrorr"...r
+00001b90: 3a00 0000 723b 0000 0072 2400 0000 7217  :...r;...r$...r.
+00001ba0: 0000 0072 1800 0000 7229 0000 0072 2300  ...r....r)...r#.
+00001bb0: 0000 7245 0000 0072 3c00 0000 722f 0000  ..rE...r<...r/..
+00001bc0: 00da 026e 70da 0561 7272 6179 7206 0000  ...np..arrayr...
+00001bd0: 0072 3600 0000 7228 0000 0072 2600 0000  .r6...r(...r&...
+00001be0: da03 7375 6272 4000 0000 7241 0000 0029  ..subr@...rA...)
+00001bf0: 0972 3000 0000 5a0c 7072 6573 6572 7665  .r0...Z.preserve
+00001c00: 5f67 6170 5a09 6661 7374 6154 6578 7472  _gapZ.fastaTextr
+00001c10: 1a00 0000 7244 0000 005a 0661 6c69 676e  ....rD...Z.align
+00001c20: 315a 0661 6c69 676e 32da 016d 5a09 636f  1Z.align2..mZ.co
+00001c30: 6e73 656e 7375 7372 1400 0000 7214 0000  nsensusr....r...
+00001c40: 0072 1500 0000 da0d 6765 745f 636f 6e73  .r......get_cons
+00001c50: 656e 7375 73c7 0000 0073 3800 0000 081f  ensus....s8.....
+00001c60: 0203 0e01 0c01 0c01 02ff 0e04 0801 2801  ..............(.
+00001c70: 0801 0402 0c01 0a01 0401 0801 1001 1201  ................
+00001c80: 0a01 0a01 1401 0a01 0401 0e01 0280 0e02  ................
+00001c90: 0a01 0c02 0802 724b 0000 0063 0100 0000  ......rK...c....
+00001ca0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00001cb0: 4300 0000 732a 0000 0074 007c 0083 017d  C...s*...t.|...}
+00001cc0: 0067 007d 017c 0044 005d 0a7d 027c 026a  .g.}.|.D.].}.|.j
+00001cd0: 017d 037c 01a0 027c 03a1 0101 0071 087c  .}.|...|.....q.|
+00001ce0: 0153 0029 0161 8202 0000 0a20 2020 2047  .S.).a.....    G
+00001cf0: 6574 2074 6865 2068 6561 6465 7220 6672  et the header fr
+00001d00: 6f6d 2061 6c6c 2069 7465 6d73 2069 6e20  om all items in 
+00001d10: 6120 6c69 7374 206f 6620 5365 7152 6563  a list of SeqRec
+00001d20: 6f72 6420 2842 696f 7079 7468 6f6e 206f  ord (Biopython o
+00001d30: 626a 6563 7429 2e0a 2020 2020 0a20 2020  bject)..    .   
+00001d40: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00001d50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
+00001d60: 6571 7265 636f 7264 5f6c 6973 7420 3a20  eqrecord_list : 
+00001d70: 6c69 7374 206f 6620 5365 7152 6563 6f72  list of SeqRecor
+00001d80: 640a 2020 2020 2020 2020 4c69 7374 206f  d.        List o
+00001d90: 6620 5365 7152 6563 6f72 642e 0a0a 2020  f SeqRecord...  
+00001da0: 2020 5265 7475 726e 730a 2020 2020 2d2d    Returns.    --
+00001db0: 2d2d 2d2d 2d0a 2020 2020 6865 6164 6572  -----.    header
+00001dc0: 5f6c 6973 7420 3a20 6c69 7374 206f 6620  _list : list of 
+00001dd0: 7374 7269 6e67 0a20 2020 2020 2020 204c  string.        L
+00001de0: 6973 7420 6f66 2061 6c6c 2068 6561 6465  ist of all heade
+00001df0: 7273 2065 7874 7261 6374 6564 2066 726f  rs extracted fro
+00001e00: 6d20 696e 7075 742e 0a20 2020 2020 2020  m input..       
+00001e10: 200a 2020 2020 4578 616d 706c 650a 2020   .    Example.  
+00001e20: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 4372    -------.    Cr
+00001e30: 6561 7465 2073 6571 7265 636f 7264 5f6c  eate seqrecord_l
+00001e40: 6973 742c 2065 7874 7261 6374 2068 6561  ist, extract hea
+00001e50: 6465 7273 2061 6e64 2070 7269 6e74 2069  ders and print i
+00001e60: 742e 0a0a 2020 2020 3e3e 3e20 696d 706f  t...    >>> impo
+00001e70: 7274 2062 696f 7465 7874 2061 7320 6274  rt biotext as bt
+00001e80: 0a20 2020 203e 3e3e 2073 6571 5f6c 6973  .    >>> seq_lis
+00001e90: 7420 3d20 5b27 4143 5447 272c 2747 5443  t = ['ACTG','GTC
+00001ea0: 4127 5d0a 2020 2020 3e3e 3e20 7365 7172  A'].    >>> seqr
+00001eb0: 6563 6f72 645f 6c69 7374 203d 2062 742e  ecord_list = bt.
+00001ec0: 6661 7374 6174 6f6f 6c73 2e63 7265 6174  fastatools.creat
+00001ed0: 655f 7365 7172 6563 6f72 645f 6c69 7374  e_seqrecord_list
+00001ee0: 2873 6571 5f6c 6973 7429 0a20 2020 203e  (seq_list).    >
+00001ef0: 3e3e 2065 7874 7261 6374 6564 5f68 6561  >> extracted_hea
+00001f00: 6465 725f 6c69 7374 203d 2062 742e 6661  der_list = bt.fa
+00001f10: 7374 6174 6f6f 6c73 2e67 6574 5f68 6561  statools.get_hea
+00001f20: 6465 7228 7365 7172 6563 6f72 645f 6c69  der(seqrecord_li
+00001f30: 7374 290a 2020 2020 3e3e 3e20 7072 696e  st).    >>> prin
+00001f40: 7428 6578 7472 6163 7465 645f 6865 6164  t(extracted_head
+00001f50: 6572 5f6c 6973 7429 0a20 2020 205b 2731  er_list).    ['1
+00001f60: 272c 2027 3227 5d0a 2020 2020 2903 720f  ', '2'].    ).r.
+00001f70: 0000 0072 2500 0000 722f 0000 0029 0472  ...r%...r/...).r
+00001f80: 1300 0000 7231 0000 0072 1a00 0000 721c  ....r1...r....r.
+00001f90: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
+00001fa0: 0000 da0a 6765 745f 6865 6164 6572 0901  ....get_header..
+00001fb0: 0000 730c 0000 0008 1a04 0108 0106 010c  ..s.............
+00001fc0: 0104 0172 4c00 0000 6301 0000 0000 0000  ...rL...c.......
+00001fd0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+00001fe0: 0073 2e00 0000 7400 7c00 8301 7d00 6700  .s....t.|...}.g.
+00001ff0: 7d01 7c00 4400 5d0c 7d02 7c02 6a01 7d03  }.|.D.].}.|.j.}.
+00002000: 7c01 a002 7403 7c03 8301 a101 0100 7108  |...t.|.......q.
+00002010: 7c01 5300 2901 6183 0200 000a 2020 2020  |.S.).a.....    
+00002020: 4765 7420 7468 6520 7365 7175 656e 6365  Get the sequence
+00002030: 7320 6672 6f6d 2061 6c6c 2069 7465 6d73  s from all items
+00002040: 2069 6e20 6120 6c69 7374 206f 6620 5365   in a list of Se
+00002050: 7152 6563 6f72 6420 2842 696f 7079 7468  qRecord (Biopyth
+00002060: 6f6e 206f 626a 6563 7429 2e0a 2020 2020  on object)..    
+00002070: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00002080: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00002090: 2020 2073 6571 7265 636f 7264 5f6c 6973     seqrecord_lis
+000020a0: 7420 3a20 6c69 7374 206f 6620 5365 7152  t : list of SeqR
+000020b0: 6563 6f72 640a 2020 2020 2020 2020 4c69  ecord.        Li
+000020c0: 7374 206f 6620 5365 7152 6563 6f72 642e  st of SeqRecord.
+000020d0: 0a0a 2020 2020 5265 7475 726e 730a 2020  ..    Returns.  
+000020e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 7365    -------.    se
+000020f0: 715f 6c69 7374 203a 206c 6973 7420 6f66  q_list : list of
+00002100: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00002110: 4c69 7374 206f 6620 616c 6c20 7365 7175  List of all sequ
+00002120: 656e 6365 7320 6578 7472 6163 7465 6420  ences extracted 
+00002130: 6672 6f6d 2069 6e70 7574 2e0a 2020 2020  from input..    
+00002140: 2020 2020 0a20 2020 2045 7861 6d70 6c65      .    Example
+00002150: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+00002160: 2043 7265 6174 6520 7365 7172 6563 6f72   Create seqrecor
+00002170: 645f 6c69 7374 2c20 6578 7472 6163 7420  d_list, extract 
+00002180: 7365 7175 656e 6365 7320 616e 6420 7072  sequences and pr
+00002190: 696e 7420 6974 2e0a 0a20 2020 203e 3e3e  int it...    >>>
+000021a0: 2069 6d70 6f72 7420 6269 6f74 6578 7420   import biotext 
+000021b0: 6173 2062 740a 2020 2020 3e3e 3e20 7365  as bt.    >>> se
+000021c0: 715f 6c69 7374 203d 205b 2741 4354 4727  q_list = ['ACTG'
+000021d0: 2c27 4754 4341 275d 0a20 2020 203e 3e3e  ,'GTCA'].    >>>
+000021e0: 2073 6571 7265 636f 7264 5f6c 6973 7420   seqrecord_list 
+000021f0: 3d20 6274 2e66 6173 7461 746f 6f6c 732e  = bt.fastatools.
+00002200: 6372 6561 7465 5f73 6571 7265 636f 7264  create_seqrecord
+00002210: 5f6c 6973 7428 7365 715f 6c69 7374 290a  _list(seq_list).
+00002220: 2020 2020 3e3e 3e20 6578 7472 6163 7465      >>> extracte
+00002230: 645f 7365 715f 6c69 7374 203d 2062 742e  d_seq_list = bt.
+00002240: 6661 7374 6174 6f6f 6c73 2e67 6574 5f73  fastatools.get_s
+00002250: 6571 2873 6571 7265 636f 7264 5f6c 6973  eq(seqrecord_lis
+00002260: 7429 0a20 2020 203e 3e3e 2070 7269 6e74  t).    >>> print
+00002270: 2865 7874 7261 6374 6564 5f73 6571 5f6c  (extracted_seq_l
+00002280: 6973 7429 0a20 2020 205b 2741 4354 4727  ist).    ['ACTG'
+00002290: 2c20 2747 5443 4127 5d0a 2020 2020 2904  , 'GTCA'].    ).
+000022a0: 720f 0000 0072 1800 0000 722f 0000 0072  r....r....r/...r
+000022b0: 1700 0000 2904 7213 0000 0072 3000 0000  ....).r....r0...
+000022c0: 721a 0000 0072 1800 0000 7214 0000 0072  r....r....r....r
+000022d0: 1400 0000 7215 0000 00da 0767 6574 5f73  ....r......get_s
+000022e0: 6571 2a01 0000 730c 0000 0008 1a04 0108  eq*...s.........
+000022f0: 0106 0110 0104 0172 4d00 0000 2903 e902  .......rM...)...
+00002300: 0000 0072 2b00 0000 724e 0000 0063 0200  ...r+...rN...c..
+00002310: 0000 0000 0000 0000 0000 0900 0000 0800  ................
+00002320: 0000 4b00 0000 73de 0000 007a 077c 0064  ..K...s....z.|.d
+00002330: 0119 006a 0001 0057 006e 0d04 0074 0179  ...j...W.n...t.y
+00002340: 1401 0001 0001 0074 027c 0083 017d 0059  .......t.|...}.Y
+00002350: 006e 0177 0067 007d 0367 007d 047c 0044  .n.w.g.}.g.}.|.D
+00002360: 005d 1d7d 0574 0374 047c 056a 0083 0183  .].}.t.t.|.j....
+00002370: 0174 057c 0183 016b 0572 337c 03a0 067c  .t.|...k.r3|...|
+00002380: 05a1 0101 007c 04a0 0664 02a1 0101 0071  .....|...d.....q
+00002390: 1b7c 04a0 0664 03a1 0101 0071 1b74 077c  .|...d.....q.t.|
+000023a0: 0366 0164 047c 0169 017c 02a4 018e 017d  .f.d.|.i.|.....}
+000023b0: 0674 087c 0664 0519 0083 017d 0774 097c  .t.|.d.....}.t.|
+000023c0: 0683 0172 5b74 0a74 037c 0083 017c 066a  ...r[t.t.|...|.j
+000023d0: 0b64 0619 0066 027c 0764 078d 027d 086e  .d...f.|.d...}.n
+000023e0: 0e74 0c6a 0d74 037c 0083 017c 066a 0b64  .t.j.t.|...|.j.d
+000023f0: 0619 0066 027c 0764 078d 027d 087c 067c  ...f.|.d...}.|.|
+00002400: 087c 043c 007c 0853 0029 0861 1003 0000  .|.<.|.S.).a....
+00002410: 0a20 2020 2043 6f6e 7665 7274 2046 4153  .    Convert FAS
+00002420: 5441 2073 6571 7565 6e63 6573 2074 6f20  TA sequences to 
+00002430: 6120 6d61 7472 6978 2072 6570 7265 7365  a matrix represe
+00002440: 6e74 6174 696f 6e20 7573 696e 6720 5357  ntation using SW
+00002450: 6565 5020 6d65 7468 6f64 2e0a 0a20 2020  eeP method...   
+00002460: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00002470: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
+00002480: 6173 7461 203a 206c 6973 740a 2020 2020  asta : list.    
+00002490: 2020 2020 4c69 7374 206f 6620 7365 7175      List of sequ
+000024a0: 656e 6365 7320 696e 2053 6571 5265 636f  ences in SeqReco
+000024b0: 7264 206f 626a 6563 7420 666f 726d 6174  rd object format
+000024c0: 206f 7220 6173 2073 7472 696e 6773 2e0a   or as strings..
+000024d0: 2020 2020 6d61 736b 203a 206c 6973 742c      mask : list,
+000024e0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+000024f0: 2020 4120 6c69 7374 2073 7065 6369 6679    A list specify
+00002500: 696e 6720 7468 6520 6d61 736b 2076 616c  ing the mask val
+00002510: 7565 732e 2044 6566 6175 6c74 7320 746f  ues. Defaults to
+00002520: 205b 322c 2031 2c20 325d 2e0a 2020 2020   [2, 1, 2]..    
+00002530: 2a2a 6b77 6172 6773 203a 2064 6963 742c  **kwargs : dict,
+00002540: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00002550: 2020 4164 6469 7469 6f6e 616c 206b 6579    Additional key
+00002560: 776f 7264 2061 7267 756d 656e 7473 2074  word arguments t
+00002570: 6f20 7061 7373 2074 6f20 7468 6520 6066  o pass to the `f
+00002580: 6173 3273 7765 6570 6020 6675 6e63 7469  as2sweep` functi
+00002590: 6f6e 2e0a 0a20 2020 2052 6574 7572 6e73  on...    Returns
+000025a0: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
+000025b0: 206d 6174 203a 206e 756d 7079 2e6e 6461   mat : numpy.nda
+000025c0: 7272 6179 206f 7220 7363 6970 792e 7370  rray or scipy.sp
+000025d0: 6172 7365 2e6c 696c 5f6d 6174 7269 780a  arse.lil_matrix.
+000025e0: 2020 2020 2020 2020 4d61 7472 6978 2072          Matrix r
+000025f0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00002600: 2074 6865 2073 6571 7565 6e63 6573 2e0a   the sequences..
+00002610: 0a20 2020 2045 7861 6d70 6c65 0a20 2020  .    Example.   
+00002620: 202d 2d2d 2d2d 2d2d 0a20 2020 2043 6f6e   -------.    Con
+00002630: 7665 7274 2046 4153 5441 2073 6571 7565  vert FASTA seque
+00002640: 6e63 6573 2074 6f20 6120 6d61 7472 6978  nces to a matrix
+00002650: 2072 6570 7265 7365 6e74 6174 696f 6e3a   representation:
+00002660: 0a0a 2020 2020 3e3e 3e20 696d 706f 7274  ..    >>> import
+00002670: 2062 696f 7465 7874 2061 7320 6274 0a20   biotext as bt. 
+00002680: 2020 203e 3e3e 2073 6571 5f6c 6973 7420     >>> seq_list 
+00002690: 3d20 5b27 4859 454c 4c59 5159 5359 5759  = ['HYELLYQYSYWY
+000026a0: 5152 4c44 272c 2027 4859 454c 4c59 5127  QRLD', 'HYELLYQ'
+000026b0: 2c20 2759 5759 5152 4c44 275d 0a20 2020  , 'YWYQRLD'].   
+000026c0: 203e 3e3e 206d 6174 7269 7820 3d20 6274   >>> matrix = bt
+000026d0: 2e66 6173 7461 746f 6f6c 732e 6661 7374  .fastatools.fast
+000026e0: 615f 746f 5f6d 6174 2873 6571 5f6c 6973  a_to_mat(seq_lis
+000026f0: 7429 0a20 2020 203e 3e3e 2070 7269 6e74  t).    >>> print
+00002700: 286d 6174 7269 782e 7368 6170 6529 0a20  (matrix.shape). 
+00002710: 2020 2028 332c 2036 3030 290a 2020 2020     (3, 600).    
+00002720: 7201 0000 0054 46da 046d 6173 6b29 0272  r....TF..mask).r
+00002730: 0100 0000 7201 0000 0072 2b00 0000 2901  ....r....r+...).
+00002740: 5a05 6474 7970 6529 0e72 1800 0000 7246  Z.dtype).r....rF
+00002750: 0000 0072 2200 0000 7223 0000 0072 1700  ...r"...r#...r..
+00002760: 0000 da03 7375 6d72 2f00 0000 7207 0000  ....sumr/...r...
+00002770: 00da 0474 7970 6572 0900 0000 7208 0000  ...typer....r...
+00002780: 00da 0573 6861 7065 7247 0000 005a 057a  ...shaperG...Z.z
+00002790: 6572 6f73 2909 720c 0000 0072 4f00 0000  eros).r....rO...
+000027a0: da06 6b77 6172 6773 5a09 6661 7374 615f  ..kwargsZ.fasta_
+000027b0: 6175 785a 086d 696e 5f73 697a 6572 1a00  auxZ.min_sizer..
+000027c0: 0000 5a07 6d61 745f 6175 785a 086f 7574  ..Z.mat_auxZ.out
+000027d0: 5f74 7970 655a 036d 6174 7214 0000 0072  _typeZ.matr....r
+000027e0: 1400 0000 7215 0000 00da 0c66 6173 7461  ....r......fasta
+000027f0: 5f74 6f5f 6d61 744b 0100 0073 2600 0000  _to_matK...s&...
+00002800: 021d 0e01 0c01 0c01 02ff 0402 0401 0801  ................
+00002810: 1601 0a01 0c01 0c02 1402 0c01 0801 1c01  ................
+00002820: 1c02 0801 0402 7254 0000 0029 014e 2901  ......rT...).N).
+00002830: 7234 0000 0029 0146 291e da07 5f5f 646f  r4...).F)...__do
+00002840: 635f 5f72 3a00 0000 7240 0000 005a 0342  c__r:...r@...Z.B
+00002850: 696f 7202 0000 0072 0300 0000 5a07 4269  ior....r....Z.Bi
+00002860: 6f2e 5365 7172 0400 0000 5a0d 4269 6f2e  o.Seqr....Z.Bio.
+00002870: 5365 7152 6563 6f72 6472 0500 0000 7226  SeqRecordr....r&
+00002880: 0000 00da 056e 756d 7079 7247 0000 00da  .....numpyrG....
+00002890: 0573 6369 7079 7206 0000 0072 0d00 0000  .scipyr....r....
+000028a0: da05 7377 6565 7072 0700 0000 723d 0000  ..sweepr....r=..
+000028b0: 005a 0c73 6369 7079 2e73 7061 7273 6572  .Z.scipy.sparser
+000028c0: 0800 0000 7209 0000 0072 1600 0000 722a  ....r....r....r*
+000028d0: 0000 0072 2200 0000 7245 0000 0072 4b00  ...r"...rE...rK.
+000028e0: 0000 724c 0000 0072 4d00 0000 7254 0000  ..rL...rM...rT..
+000028f0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00002900: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00002910: 0000 0073 2a00 0000 0402 0811 0801 1001  ...s*...........
+00002920: 0c01 0c01 0801 0801 0c01 0801 0c01 0801  ................
+00002930: 1001 0802 0a21 0a24 0a30 0a31 0842 0821  .....!.$.0.1.B.!
+00002940: 1421                                     .!
```

