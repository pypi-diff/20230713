# Comparing `tmp/peptacular-0.0.7.tar.gz` & `tmp/peptacular-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.0.7.tar", last modified: Wed Jul 12 22:30:39 2023, max compression
+gzip compressed data, was "peptacular-0.0.8.tar", last modified: Thu Jul 13 00:21:30 2023, max compression
```

## Comparing `peptacular-0.0.7.tar` & `peptacular-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 22:30:25.000000 peptacular-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 22:30:39.170190 peptacular-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 22:30:25.000000 peptacular-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 22:30:25.000000 peptacular-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:30:39.170190 peptacular-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-12 22:30:25.000000 peptacular-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.166190 peptacular-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.166190 peptacular-0.0.7/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/refseq.py
--rw-r--r--   0 runner    (1001) docker     (123)    25368 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_refstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 00:21:14.000000 peptacular-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 00:21:30.507984 peptacular-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 00:21:14.000000 peptacular-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-13 00:21:14.000000 peptacular-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:21:30.507984 peptacular-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 00:21:14.000000 peptacular-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/refseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_refstring.py
```

### Comparing `peptacular-0.0.7/LICENSE` & `peptacular-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/PKG-INFO` & `peptacular-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.7/README.md` & `peptacular-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/pyproject.toml` & `peptacular-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/src/peptacular/constants.py` & `peptacular-0.0.8/src/peptacular/constants.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/src/peptacular/protein.py` & `peptacular-0.0.8/src/peptacular/protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/src/peptacular/refseq.py` & `peptacular-0.0.8/src/peptacular/refseq.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/src/peptacular/sequence.py` & `peptacular-0.0.8/src/peptacular/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,16 @@
     if check_parentheses(sequence) is False:
         raise ValueError(f'Incorrect modification notation in peptide sequence : {sequence}!')
 
     unmodified_sequence = re.sub(r'\([^)]*\)', '', sequence)
     return unmodified_sequence
 
 
-def get_left_semi_sequences(sequence: str, min_len: int = None, max_len: int = None, max_semi_offset: int = None):
+def get_left_semi_sequences(sequence: str, min_len: int = None, max_len: int = None, max_semi_offset: int = None,
+                            info: bool = False):
     """
     Returns a set of left substrings of string `sequence` that have lengths between `min_len` and `max_len`.
 
     Example:
     >>> get_left_semi_sequences("abc", 1, 2)
     {'a', 'ab'}
     """
@@ -128,25 +129,31 @@
     if min_len is None:
         min_len = 1
     if max_len is None:
         max_len = len(sequence) - 1
 
     cnt = 0
     sequences = []
+    offsets = []
     for i in range(min_len, min(max_len, len(sequence) - 1) + 1)[::-1]:
         sequences.append(sequence[0:i])
+        offsets.append(i)
         cnt += 1
 
         if max_semi_offset is not None and cnt >= max_semi_offset:
             break
 
+    if info is True:
+        return sequences, offsets
+
     return sequences
 
 
-def get_right_semi_sequences(sequence: str, min_len: int = None, max_len: int = None, max_semi_offset: int = None):
+def get_right_semi_sequences(sequence: str, min_len: int = None, max_len: int = None, max_semi_offset: int = None,
+                             info: bool = False):
     """
     Returns a set of right substrings of string `sequence` that have lengths between `min_len` and `max_len`.
 
     Example:
     >>> get_right_semi_sequences("abc", 1, 2)
     {'c', 'bc'}
     """
@@ -154,21 +161,26 @@
         min_len = 1
     if max_len is None:
         max_len = len(sequence) - 1
     end = min(max_len, len(sequence) - 1)
 
     cnt = 0
     sequences = []
+    offsets = []
     for i in range(min_len, end + 1)[::-1]:
         sequences.append(sequence[-i:])
+        offsets.append(-i)
         cnt += 1
 
         if max_semi_offset is not None and cnt >= max_semi_offset:
             break
 
+    if info is True:
+        return sequences, offsets
+
     return sequences
 
 
 def get_semi_sequences(sequence: str, min_len: int = None, max_len: int = None, max_semi_offset: int = None):
     """
     Returns a set of all semi enzymatic amino acid sequences of string `sequence` that have lengths
     between `min_len` and `max_len`.
@@ -626,15 +638,15 @@
     if len(spans) != missed_cleavages + 1:
         spans.append((start_site, last_sequence_index, len(spans)))
 
     return spans
 
 
 def _digest_sequence(protein_sequence: str, enzyme_sites: List[int], missed_cleaves: int, min_len: int,
-                     max_len: int) -> List[str]:
+                     max_len: int) -> Tuple[List[str], List[Tuple[int, int, int]]]:
     """
     Digests a protein sequence according to the enzyme regex string and number of missed cleavages.
     """
 
     if len(enzyme_sites) == 0:
         return [protein_sequence], [(0, len(protein_sequence), 0)]
 
@@ -658,49 +670,38 @@
         span_len = span[1] - span[0]
         # if min_len <= span_len <= max_len:
         peptides.append(protein_sequence[span[0]:span[1]])
     return peptides, peptide_spans
 
 
 def digest_sequence(sequence: str, enzyme_regexes: Union[List[str], str], missed_cleavages: int, min_len: int,
-                    max_len: int, semi_enzymatic: bool, info: bool = False) -> List[str]:
+                    max_len: int, semi_enzymatic: bool) -> List[str]:
     """
     A function that digests a given amino acid sequence based on the provided positive and negative regular expressions and
     the number of missed cleavages. It returns a list of tuples containing the digested_sequences and the number of missed
     cleavages. The returned digested_sequences will be filtered based on the provided minimum and maximum length.
     """
 
     if isinstance(enzyme_regexes, str):
         enzyme_regexes = [enzyme_regexes]
-    digested_sequences, mc_status, semi_status, start, stop = [], [], [], [], []
+    digested_sequences = []
     for enzyme_regex in enzyme_regexes:
 
         if enzyme_regex == PROTEASES['non-specific']:
             sequences = get_non_enzymatic_sequences(sequence, min_len, max_len)
-            mc_status = [0 for _ in range(len(sequences))]
-            semi_status = [0 for _ in range(len(sequences))]
             digested_sequences.extend(sequences)
 
         else:
             cleavage_sites = identify_cleavage_sites(sequence, enzyme_regex)
             sequences, spans = _digest_sequence(sequence, cleavage_sites, missed_cleavages, min_len, max_len)
-            mc_status = [span[2] for span in spans]
             digested_sequences.extend(sequences)
-            semi_status.extend([0 for _ in range(len(sequences))])
 
             if semi_enzymatic is True:
-                for sequence, mc in zip(sequences, mc_status):
+                for sequence in sequences:
                     semi_sequences = get_semi_sequences(sequence, min_len, max_len)
                     digested_sequences.extend(semi_sequences)
-                    semi_status.extend([1 for _ in range(len(semi_sequences))])
-                    mc_status.extend([mc for _ in range(len(semi_sequences))])
 
     # filter based on min / max len
     flags = [max_len >= len(sequence) >= min_len for sequence in digested_sequences]
-    digested_sequences = [sequence for sequence, flag in zip(digested_sequences, flags) if flag is True ]
-    mc_status = [mc for mc, flag in zip(mc_status, flags) if flag is True ]
-    semi_status = [semi for semi, flag in zip(semi_status, flags) if flag is True ]
-
-    if info is True:
-        return digested_sequences, mc_status, semi_status
+    digested_sequences = [sequence for sequence, flag in zip(digested_sequences, flags) if flag is True]
 
     return digested_sequences
```

### Comparing `peptacular-0.0.7/src/peptacular/util.py` & `peptacular-0.0.8/src/peptacular/util.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.0.8/src/peptacular.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.7/tests/test_peptide.py` & `peptacular-0.0.8/tests/test_peptide.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/tests/test_protein.py` & `peptacular-0.0.8/tests/test_protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.7/tests/test_refstring.py` & `peptacular-0.0.8/tests/test_refstring.py`

 * *Files identical despite different names*

