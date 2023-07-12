# Comparing `tmp/peptacular-0.0.6.tar.gz` & `tmp/peptacular-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.0.6.tar", last modified: Tue Jul 11 20:24:34 2023, max compression
+gzip compressed data, was "peptacular-0.0.7.tar", last modified: Wed Jul 12 22:30:39 2023, max compression
```

## Comparing `peptacular-0.0.6.tar` & `peptacular-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 20:24:21.000000 peptacular-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 20:24:34.846794 peptacular-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-11 20:24:21.000000 peptacular-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-11 20:24:21.000000 peptacular-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:24:34.846794 peptacular-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 20:24:21.000000 peptacular-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/refseq.py
--rw-r--r--   0 runner    (1001) docker     (123)    24396 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-11 20:24:21.000000 peptacular-0.0.6/src/peptacular/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 20:24:34.000000 peptacular-0.0.6/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:24:34.846794 peptacular-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-11 20:24:21.000000 peptacular-0.0.6/tests/test_refstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 22:30:25.000000 peptacular-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 22:30:39.170190 peptacular-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 22:30:25.000000 peptacular-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 22:30:25.000000 peptacular-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:30:39.170190 peptacular-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-12 22:30:25.000000 peptacular-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.166190 peptacular-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.166190 peptacular-0.0.7/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/refseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25368 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-12 22:30:25.000000 peptacular-0.0.7/src/peptacular/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 22:30:39.000000 peptacular-0.0.7/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:30:39.170190 peptacular-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-12 22:30:25.000000 peptacular-0.0.7/tests/test_refstring.py
```

### Comparing `peptacular-0.0.6/LICENSE` & `peptacular-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/PKG-INFO` & `peptacular-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.6/README.md` & `peptacular-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/pyproject.toml` & `peptacular-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/src/peptacular/constants.py` & `peptacular-0.0.7/src/peptacular/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "NITROGEN": 14.003074,
     "PHOSPHORUS": 30.973762,
     "SULPHUR": 31.9720707,
     "SELENIUM": 79.9165196,
 }
 
 AVERAGE_ATOMIC_MASSES = {
-    "HYDROGEN": 1.008,
+    "HYDROGEN": 1.00794,
     "PROTON": 1.007276,
     "OXYGEN": 15.999,
     "CARBON": 12.011,
     "NITROGEN": 14.007,
 }
 
 UWPR_AVERAGE_ATOMIC_MASSES = {
```

### Comparing `peptacular-0.0.6/src/peptacular/protein.py` & `peptacular-0.0.7/src/peptacular/protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/src/peptacular/refseq.py` & `peptacular-0.0.7/src/peptacular/refseq.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/src/peptacular/sequence.py` & `peptacular-0.0.7/src/peptacular/sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,17 +127,17 @@
 
     if min_len is None:
         min_len = 1
     if max_len is None:
         max_len = len(sequence) - 1
 
     cnt = 0
-    sequences = set()
+    sequences = []
     for i in range(min_len, min(max_len, len(sequence) - 1) + 1)[::-1]:
-        sequences.add(sequence[0:i])
+        sequences.append(sequence[0:i])
         cnt += 1
 
         if max_semi_offset is not None and cnt >= max_semi_offset:
             break
 
     return sequences
 
@@ -153,17 +153,17 @@
     if min_len is None:
         min_len = 1
     if max_len is None:
         max_len = len(sequence) - 1
     end = min(max_len, len(sequence) - 1)
 
     cnt = 0
-    sequences = set()
+    sequences = []
     for i in range(min_len, end + 1)[::-1]:
-        sequences.add(sequence[-i:])
+        sequences.append(sequence[-i:])
         cnt += 1
 
         if max_semi_offset is not None and cnt >= max_semi_offset:
             break
 
     return sequences
 
@@ -174,16 +174,16 @@
     between `min_len` and `max_len`.
 
     Example:
     >>> get_semi_sequences("abc", 1, 2)
     {'a', 'ab', 'c', 'bc'}
     """
 
-    return get_left_semi_sequences(sequence, min_len, max_len, max_semi_offset).union(
-        get_right_semi_sequences(sequence, min_len, max_len, max_semi_offset))
+    return get_left_semi_sequences(sequence, min_len, max_len, max_semi_offset) + \
+        get_right_semi_sequences(sequence, min_len, max_len, max_semi_offset)
 
 
 def get_non_enzymatic_sequences(sequence: str, min_len: int = None, max_len: int = None):
     """
     Returns a set of all non-enzymatic amino acid sequences of string `sequence` that have lengths
     between `min_len` and `max_len`.
 
@@ -194,19 +194,19 @@
 
     if min_len is None:
         min_len = 1
 
     if max_len is None:
         max_len = len(sequence)
 
-    substrings = set()
+    sequences = []
     for i in range(len(sequence)):
         for j in range(i + min_len, min(i + max_len + 1, len(sequence) + 1)):
-            substrings.add(sequence[i:j])
-    return substrings
+            sequences.append(sequence[i:j])
+    return sequences
 
 
 def add_static_mods(sequence: str, mod_map: Dict[str, Any]):
     """
     Add static modifications to an amino acid sequence.
 
     Args:
@@ -502,15 +502,14 @@
     # Shift mod positions, taking care to avoid negative keys
     shifted_sequence_mods = {(k - effective_shift) % seq_len if k != -1 else -1: v for k, v in mods.items()}
 
     return create_modified_sequence(shifted_stripped_sequence, shifted_sequence_mods)
 
 
 def calculate_mass_array(sequence: str, monoisotopic: bool = True):
-
     if monoisotopic is True:
         aa_masses = MONO_ISOTOPIC_AA_MASSES
     else:
         aa_masses = AVERAGE_AA_MASSES
 
     sequence_mods = parse_modified_sequence(sequence)
     stripped_sequence = strip_modifications(sequence)
@@ -528,16 +527,16 @@
         mass_arr[i] = np.float32(aa_masses[aa] + mod_mass)
 
     mass_arr = np.array(mass_arr, dtype=np.float32)
 
     return mass_arr
 
 
-def create_ion_table(sequence: str, max_len: int = 50, ion_type: str = 'y', charge: int = 0, enzyme: str = 'non-specific'):
-
+def create_ion_table(sequence: str, max_len: int = 50, ion_type: str = 'y', charge: int = 0,
+                     enzyme: str = 'non-specific'):
     if ion_type == 'y':
         sequence = sequence[::-1]
 
     sequence_cumulative_sum = np.cumsum(calculate_mass_array(sequence))
     len_sequence = len(sequence)
 
     # Add padding zeros to make our life easier when computing window sums
@@ -633,18 +632,15 @@
 def _digest_sequence(protein_sequence: str, enzyme_sites: List[int], missed_cleaves: int, min_len: int,
                      max_len: int) -> List[str]:
     """
     Digests a protein sequence according to the enzyme regex string and number of missed cleavages.
     """
 
     if len(enzyme_sites) == 0:
-        if min_len <= len(protein_sequence) <= max_len:
-            return [protein_sequence]
-        else:
-            return []
+        return [protein_sequence], [(0, len(protein_sequence), 0)]
 
     peptide_spans = []
 
     cur_site = 0
     curr_enzyme_index = -1
     while True:
         future_start_sites = enzyme_sites[curr_enzyme_index + 1:]
@@ -656,39 +652,55 @@
             break
 
         cur_site = enzyme_sites[curr_enzyme_index]
 
     peptides = []
     for span in peptide_spans:
         span_len = span[1] - span[0]
-        if min_len <= span_len <= max_len:
-            peptides.append(protein_sequence[span[0]:span[1]])
-    return peptides
+        # if min_len <= span_len <= max_len:
+        peptides.append(protein_sequence[span[0]:span[1]])
+    return peptides, peptide_spans
 
 
 def digest_sequence(sequence: str, enzyme_regexes: Union[List[str], str], missed_cleavages: int, min_len: int,
-                    max_len: int, semi_enzymatic: bool) -> List[str]:
+                    max_len: int, semi_enzymatic: bool, info: bool = False) -> List[str]:
     """
     A function that digests a given amino acid sequence based on the provided positive and negative regular expressions and
     the number of missed cleavages. It returns a list of tuples containing the digested_sequences and the number of missed
     cleavages. The returned digested_sequences will be filtered based on the provided minimum and maximum length.
     """
 
     if isinstance(enzyme_regexes, str):
         enzyme_regexes = [enzyme_regexes]
-    digested_sequences = []
+    digested_sequences, mc_status, semi_status, start, stop = [], [], [], [], []
     for enzyme_regex in enzyme_regexes:
 
         if enzyme_regex == PROTEASES['non-specific']:
-            digested_sequences.extend(
-                [peptide for peptide in get_non_enzymatic_sequences(sequence, min_len, max_len)])
+            sequences = get_non_enzymatic_sequences(sequence, min_len, max_len)
+            mc_status = [0 for _ in range(len(sequences))]
+            semi_status = [0 for _ in range(len(sequences))]
+            digested_sequences.extend(sequences)
 
         else:
             cleavage_sites = identify_cleavage_sites(sequence, enzyme_regex)
-            sequences = _digest_sequence(sequence, cleavage_sites, missed_cleavages, min_len, max_len)
+            sequences, spans = _digest_sequence(sequence, cleavage_sites, missed_cleavages, min_len, max_len)
+            mc_status = [span[2] for span in spans]
             digested_sequences.extend(sequences)
+            semi_status.extend([0 for _ in range(len(sequences))])
 
             if semi_enzymatic is True:
-                for sequence in sequences:
-                    digested_sequences.extend(get_semi_sequences(sequence, min_len, max_len))
+                for sequence, mc in zip(sequences, mc_status):
+                    semi_sequences = get_semi_sequences(sequence, min_len, max_len)
+                    digested_sequences.extend(semi_sequences)
+                    semi_status.extend([1 for _ in range(len(semi_sequences))])
+                    mc_status.extend([mc for _ in range(len(semi_sequences))])
+
+    # filter based on min / max len
+    flags = [max_len >= len(sequence) >= min_len for sequence in digested_sequences]
+    digested_sequences = [sequence for sequence, flag in zip(digested_sequences, flags) if flag is True ]
+    mc_status = [mc for mc, flag in zip(mc_status, flags) if flag is True ]
+    semi_status = [semi for semi, flag in zip(semi_status, flags) if flag is True ]
+
+    if info is True:
+        return digested_sequences, mc_status, semi_status
 
     return digested_sequences
```

### Comparing `peptacular-0.0.6/src/peptacular/util.py` & `peptacular-0.0.7/src/peptacular/util.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.0.7/src/peptacular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.6/tests/test_peptide.py` & `peptacular-0.0.7/tests/test_peptide.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,67 +108,67 @@
 
     def test_get_unmodified_peptide(self):
         self.assertEqual(strip_modifications('ACDEFG'), 'ACDEFG')
         self.assertEqual(strip_modifications('A(2)CDE(2)FG'), 'ACDEFG')
         self.assertEqual(strip_modifications('A(2)CDE(Acetyl)FG'), 'ACDEFG')
 
     def test_get_semi_sequences(self):
-        assert get_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=5) == \
+        assert set(get_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=5)) == \
                {'TIDE', 'PTIDE', 'PEPT', 'PEPTI', 'IDE', 'PEP'}
-        assert get_semi_sequences(sequence='PEPTIDE', min_len=2, max_len=5) == \
+        assert set(get_semi_sequences(sequence='PEPTIDE', min_len=2, max_len=5)) == \
                {'TIDE', 'PTIDE', 'PEPT', 'PEPTI', 'IDE', 'PEP', 'PE', 'DE'}
-        assert get_semi_sequences(sequence='PEPTIDE', min_len=2, max_len=100) == \
+        assert set(get_semi_sequences(sequence='PEPTIDE', min_len=2, max_len=100)) == \
                {'TIDE', 'PTIDE', 'PEPT', 'PEPTI', 'IDE', 'PEP', 'PE', 'DE', 'PEPTID', 'EPTIDE'}
-        assert get_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None) == \
+        assert set(get_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None)) == \
                {'P', 'E', 'TIDE', 'PTIDE', 'PEPT', 'PEPTI', 'IDE', 'PEP', 'PE', 'DE', 'PEPTID', 'EPTIDE'}
 
     def test_get_left_semi_sequences(self):
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', None, None, None),
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', None, None, None)),
                          {'P', 'PE', 'PEP', 'PEPT', 'PEPTI', 'PEPTID'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', 3, None, None), {'PEP', 'PEPT', 'PEPTI', 'PEPTID'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', None, 5, None), {'P', 'PE', 'PEP', 'PEPT', 'PEPTI'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', None, None, 1), {'PEPTID'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', None, None, 2), {'PEPTID', 'PEPTI'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', 3, 5, 1), {'PEPTI'})
-        self.assertEqual(get_left_semi_sequences('PEPTIDE', 3, 5, 2), {'PEPTI', 'PEPT'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', 3, None, None)), {'PEP', 'PEPT', 'PEPTI', 'PEPTID'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', None, 5, None)), {'P', 'PE', 'PEP', 'PEPT', 'PEPTI'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', None, None, 1)), {'PEPTID'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', None, None, 2)), {'PEPTID', 'PEPTI'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', 3, 5, 1)), {'PEPTI'})
+        self.assertEqual(set(get_left_semi_sequences('PEPTIDE', 3, 5, 2)), {'PEPTI', 'PEPT'})
 
-        assert get_left_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None) == \
+        assert set(get_left_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None)) == \
                {'P', 'PE', 'PEP', 'PEPT', 'PEPTI', 'PEPTID'}
-        assert get_left_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=None) == \
+        assert set(get_left_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=None)) == \
                {'PEP', 'PEPT', 'PEPTI', 'PEPTID'}
-        assert get_left_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=5) == \
+        assert set(get_left_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=5)) == \
                {'P', 'PE', 'PEP', 'PEPT', 'PEPTI'}
-        assert get_left_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=4) == \
+        assert set(get_left_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=4)) == \
                {'PEP', 'PEPT'}
 
     def test_get_right_semi_sequences(self):
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', None, None, None),
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', None, None, None)),
                          {'EPTIDE', 'PTIDE', 'TIDE', 'IDE', 'DE', 'E'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', 3, None, None), {'EPTIDE', 'PTIDE', 'TIDE', 'IDE'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', None, 5, None), {'PTIDE', 'TIDE', 'IDE', 'DE', 'E'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', None, None, 1), {'EPTIDE'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', None, None, 2), {'EPTIDE', 'PTIDE'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', 3, 5, 1), {'PTIDE'})
-        self.assertEqual(get_right_semi_sequences('PEPTIDE', 3, 5, 2), {'PTIDE', 'TIDE'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', 3, None, None)), {'EPTIDE', 'PTIDE', 'TIDE', 'IDE'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', None, 5, None)), {'PTIDE', 'TIDE', 'IDE', 'DE', 'E'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', None, None, 1)), {'EPTIDE'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', None, None, 2)), {'EPTIDE', 'PTIDE'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', 3, 5, 1)), {'PTIDE'})
+        self.assertEqual(set(get_right_semi_sequences('PEPTIDE', 3, 5, 2)), {'PTIDE', 'TIDE'})
 
-        assert get_right_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None) == \
+        assert set(get_right_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=None)) == \
                {'EPTIDE', 'PTIDE', 'TIDE', 'IDE', 'DE', 'E'}
-        assert get_right_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=None) == \
+        assert set(get_right_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=None)) == \
                {'EPTIDE', 'PTIDE', 'TIDE', 'IDE'}
-        assert get_right_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=5) == \
+        assert set(get_right_semi_sequences(sequence='PEPTIDE', min_len=None, max_len=5)) == \
                {'PTIDE', 'TIDE', 'IDE', 'DE', 'E'}
-        assert get_right_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=4) == \
+        assert set(get_right_semi_sequences(sequence='PEPTIDE', min_len=3, max_len=4)) == \
                {'TIDE', 'IDE'}
 
     def test_get_all_non_enzymatic_peptides(self):
-        self.assertEqual(get_non_enzymatic_sequences('PEPT'),
+        self.assertEqual(set(get_non_enzymatic_sequences('PEPT')),
                          {'P', 'E', 'P', 'T', 'PE', 'EP', 'PT', 'PEP', 'EPT', 'PEPT'})
-        self.assertEqual(get_non_enzymatic_sequences('PEPT', min_len=1, max_len=2),
+        self.assertEqual(set(get_non_enzymatic_sequences('PEPT', min_len=1, max_len=2)),
                          {'P', 'E', 'P', 'T', 'PE', 'EP', 'PT'})
-        self.assertEqual(get_non_enzymatic_sequences('PEPT', min_len=2, max_len=4),
+        self.assertEqual(set(get_non_enzymatic_sequences('PEPT', min_len=2, max_len=4)),
                          {'PE', 'EP', 'PT', 'PEP', 'EPT', 'PEPT'})
 
     def test_add_static_mod(self):
         self.assertEqual(add_static_mods('PEPCTIDE', {'C': 57.021464}), 'PEPC(57.021464)TIDE')
         self.assertEqual(add_static_mods('PEPC(57.021464)TIDE', {'C': 57.021464}), 'PEPC(57.021464)TIDE')
         self.assertEqual(add_static_mods('CPEPTIDEC', {'C': 57.021464}), 'C(57.021464)PEPTIDEC(57.021464)')
```

### Comparing `peptacular-0.0.6/tests/test_protein.py` & `peptacular-0.0.7/tests/test_protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.6/tests/test_refstring.py` & `peptacular-0.0.7/tests/test_refstring.py`

 * *Files identical despite different names*

