# Comparing `tmp/nmd-0.0.5.tar.gz` & `tmp/nmd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmd-0.0.5.tar", last modified: Tue Aug  2 03:59:53 2022, max compression
+gzip compressed data, was "nmd-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nmd-0.0.5.tar` & `nmd-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     2250 2022-07-20 01:53:08.820232 nmd-0.0.5/.gitignore
--rw-r--r--   0        0        0     1098 2022-08-02 02:47:55.164963 nmd-0.0.5/LICENSE
--rw-r--r--   0        0        0     4950 2022-08-02 03:59:38.237899 nmd-0.0.5/README.md
--rw-r--r--   0        0        0    15482 2022-07-20 01:53:08.821201 nmd-0.0.5/automata.py
--rw-r--r--   0        0        0  7483238 2022-07-20 01:53:08.882038 nmd-0.0.5/british-english-insane.txt
--rw-r--r--   0        0        0     6754 2022-07-20 01:53:08.884033 nmd-0.0.5/dawg-orig.py
--rw-r--r--   0        0        0     8633 2022-07-20 01:53:08.884033 nmd-0.0.5/dawg.py
--rw-r--r--   0        0        0     9077 2022-08-02 03:52:25.826561 nmd-0.0.5/experiment.py
--rw-r--r--   0        0        0    52254 2022-07-20 01:53:08.885031 nmd-0.0.5/find_replace_trie.py
--rw-r--r--   0        0        0     6794 2022-07-20 01:53:08.886028 nmd-0.0.5/levenshtein.py
--rw-r--r--   0        0        0      242 2022-08-02 03:59:38.230894 nmd-0.0.5/nmd/__init__.py
--rw-r--r--   0        0        0    13373 2022-07-26 05:53:11.033626 nmd-0.0.5/nmd/nmd.py
--rw-r--r--   0        0        0     2178 2022-08-02 03:51:22.921810 nmd-0.0.5/nmd/nmd_bow.py
--rw-r--r--   0        0        0    16611 2022-08-02 03:51:22.931077 nmd-0.0.5/nmd/nmd_index.py
--rw-r--r--   0        0        0      409 2022-08-02 02:47:55.165961 nmd-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3821 2022-07-20 01:53:08.889020 nmd-0.0.5/schwarzenegger.txt
--rw-r--r--   0        0        0     6832 2022-07-20 01:53:08.889020 nmd-0.0.5/sizeof.py
--rw-r--r--   0        0        0    18204 2022-07-20 01:53:08.890018 nmd-0.0.5/tokenizer.py
--rw-r--r--   0        0        0   412100 2022-07-20 01:53:08.895003 nmd-0.0.5/words_en.txt
--rw-r--r--   0        0        0   491899 2022-07-20 01:53:08.899993 nmd-0.0.5/words_ms.txt
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 nmd-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2250 2023-06-19 08:15:15.660981 nmd-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1098 2023-06-19 08:15:15.660981 nmd-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5500 2023-06-19 08:15:15.661979 nmd-0.0.6/README.md
+-rw-r--r--   0        0        0    15494 2023-06-19 08:15:15.661979 nmd-0.0.6/experiments/automata.py
+-rw-r--r--   0        0        0  7483238 2023-06-19 08:15:15.720859 nmd-0.0.6/experiments/british-english-insane.txt
+-rw-r--r--   0        0        0     6754 2023-06-19 08:15:15.721821 nmd-0.0.6/experiments/dawg-orig.py
+-rw-r--r--   0        0        0     8643 2023-06-19 08:15:15.722818 nmd-0.0.6/experiments/dawg.py
+-rw-r--r--   0        0        0     6847 2023-06-19 08:15:15.722818 nmd-0.0.6/experiments/edit_distance.py
+-rw-r--r--   0        0        0     9538 2023-06-19 08:15:15.723815 nmd-0.0.6/experiments/experiment.py
+-rw-r--r--   0        0        0    52254 2023-06-19 08:15:15.723815 nmd-0.0.6/experiments/find_replace_trie.py
+-rw-r--r--   0        0        0     3821 2023-06-19 08:15:15.724820 nmd-0.0.6/experiments/schwarzenegger.txt
+-rw-r--r--   0        0        0     6832 2023-06-19 08:15:15.724820 nmd-0.0.6/experiments/sizeof.py
+-rw-r--r--   0        0        0    18211 2023-06-19 08:15:15.725817 nmd-0.0.6/experiments/tokenizer.py
+-rw-r--r--   0        0        0      825 2023-07-13 06:25:20.097027 nmd-0.0.6/experiments/wordlist-to-regex.py
+-rw-r--r--   0        0        0   412100 2023-06-19 08:15:15.729833 nmd-0.0.6/experiments/words_en.txt
+-rw-r--r--   0        0        0   491899 2023-06-19 08:15:15.734793 nmd-0.0.6/experiments/words_ms.txt
+-rw-r--r--   0        0        0      246 2023-07-13 06:23:37.449657 nmd-0.0.6/nmd/__init__.py
+-rw-r--r--   0        0        0    13547 2023-07-13 06:22:16.758243 nmd-0.0.6/nmd/nmd.py
+-rw-r--r--   0        0        0     2178 2023-06-19 08:15:15.735786 nmd-0.0.6/nmd/nmd_bow.py
+-rw-r--r--   0        0        0    16951 2023-06-19 08:15:15.736782 nmd-0.0.6/nmd/nmd_index.py
+-rw-r--r--   0        0        0      413 2023-06-19 08:15:15.736782 nmd-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 nmd-0.0.6/PKG-INFO
```

### Comparing `nmd-0.0.5/.gitignore` & `nmd-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/LICENSE` & `nmd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/README.md` & `nmd-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # N-gram Mover's Distance
 
-A string similarity measure based on Earth Mover's Distance
+* A string similarity measure based on Earth Mover's Distance
+* See [ngram-movers-distance](https://github.com/averykhoo/ngram-movers-distance) for code
 
 ## Why another string matching algorithm?
 
 * Edit distance really wasn't cutting it when I needed to look up a dictionary for a misspelled word
-  * With an edit distance of 1 or 2, the results are not very useful
-  * With a distance >=5, the results are meaningless
-  * Same goes for Damerau-Levenshtein
+    * With an edit distance of 1 or 2, the results are not useful since the target word isn't found
+    * With a distance >=5, the results are meaningless since it contains half the dictionary
+    * Same goes for Damerau-Levenshtein
 * Also, edit distance is pretty slow when looking up long words in a large dictionary
-  * Even with a decent automaton or trie implementation
-  * NMD was designed with indexing in mind
-  * A simpler index could be used for Jaccard or cosine similarity over ngrams
-    * todo: try [this paper's algo](https://www.aclweb.org/anthology/C10-1096.pdf)
-    * which referenced [this paper](https://www.cse.iitb.ac.in/~sunita/papers/sigmod04.pdf)
+    * Even after building a finite state automaton or using a trie to optimize lookup
+    * NMD was designed with indexing in mind
+        * A simpler index could be used for Jaccard or cosine similarity over ngrams
+* EMD (and hence NMD) can be optimized to run really fast with some constraints
+    * Values are 1-dimensional scalars
+    * Values are always quantized
 
 # Usage
 
 ## `ngram_movers_distance()`
 
 * string distance metric, use this to compare two strings
 
@@ -41,15 +43,15 @@
 
 * use this for dictionary lookups of words
 
 ```python
 from nmd import WordList
 
 # get words from a text file
-with open(f'words_ms.txt', encoding=f'utf8') as f:
+with open(f'dictionary.txt', encoding=f'utf8') as f:
     words = set(f.read().split())
 
 # index words
 word_list = WordList((2, 4), filter_n=0)  # combined 2- and 4-grams seem to work best
 for word in words:
     word_list.add_word(word)
 
@@ -58,36 +60,43 @@
 print(word_list.lookup(f'walaikumalasam'))  # -> 'waalaikumsalam'
 ```
 
 ## `bow_ngram_movers_distance()`
 
 * WARNING: requires `scipy.optimize`, so it's not available by default in the `nmd` namespace
 * use this to compare sequences of tokens (not necessarily unique)
+* note that this does not merge or split words, so if you're matching `["pineapple"]` and `["pine", "apple"]` the
+  similarity will be low. consider just using nmd in this case.
 
 ```python
 from nmd.nmd_bow import bow_ngram_movers_distance
-from tokenizer import unicode_tokenize
 
 text_1 = f'Clementi Sports Hub'
 text_2 = f'sport hubs clemmeti'
-print(bow_ngram_movers_distance(bag_of_words_1=unicode_tokenize(text_1.casefold(), words_only=True),
-                                bag_of_words_2=unicode_tokenize(text_2.casefold(), words_only=True),
+print(bow_ngram_movers_distance(bag_of_words_1=text_1.casefold().split(),
+                                bag_of_words_2=text_2.casefold().split(),
                                 invert=True,  # invert: return similarity instead of distance
                                 normalize=True,  # return a score between 0 and 1
                                 ))
 ```
 
 # todo
 
+* todo: try [this paper's algo](https://www.aclweb.org/anthology/C10-1096.pdf)
+    * which referenced [this paper](https://www.cse.iitb.ac.in/~sunita/papers/sigmod04.pdf)
 * use less bizarre test strings
+* note where the algorithm breaks down
+    * matching long strings with many n-grams
+    * matching strings with significantly different lengths
+    *
 * rename nmd_bow because it isn't really a bag-of-words, it's a token sequence
 * consider a `real_quick_ratio`-like optimization, or maybe calculate length bounds?
-  * needs a cutoff to actually speed up though, makes a huge difference for difflib
-  * a sufficiently low cutoff is not unreasonable, although the default of 0.6 might be a little high for nmd
-  * that said the builtin diff performs pretty badly at low similarities, so 0.6 is reasonable for them
+    * needs a cutoff to actually speed up though, makes a huge difference for difflib
+    * a sufficiently low cutoff is not unreasonable, although the default of 0.6 might be a little high for nmd
+    * that said the builtin diff performs pretty badly at low similarities, so 0.6 is reasonable for them
 
 ```python
 def real_quick_ratio(self):
     """Return an upper bound on ratio() very quickly.
 
     This isn't defined beyond that it is an upper bound on .ratio(), and
     is faster to compute than either .ratio() or .quick_ratio().
@@ -98,37 +107,34 @@
     matches, length = min(la, lb), la + lb
     if length:
         return 2.0 * matches / length
     return 1.0
 ```
 
 * create a better string container for the index, more like a `set`
-  * `add(word: str)`
-  * `remove(word: str)`
-  * `clear()`
-  * `__contains__(word: str)`
-  * `__iter__()`
+    * `add(word: str)`
+    * `remove(word: str)`
+    * `clear()`
+    * `__contains__(word: str)`
+    * `__iter__()`
 * better lookup
-  * add a min_similarity filter (float, based on normalized distance)
-    * `lookup(word: str, min_similarity: float = 0, filter: bool = True)`
-  * try `__contains__` first
-    * try levenshtein automaton (distance=1) second?
-      * sort by nmd, since most likely there will only be a few results
-    * but how to get multiple results?
-      * still need to run full search?
-      * or maybe just return top 1 result?
-  * make the 3-gram filter optional
+    * add a min_similarity filter (float, based on normalized distance)
+        * `lookup(word: str, min_similarity: float = 0, filter: bool = True)`
+    * try `__contains__` first
+        * try levenshtein automaton (distance=1) second?
+            * sort by nmd, since most likely there will only be a few results
+        * but how to get multiple results?
+            * still need to run full search?
+            * or maybe just return top 1 result?
 * prefix lookup
-  * look for all strings that are approximately prefixed
-  * like existing index but not normalized and ignoring unmatched ngrams from target
-* bag of words
-  * use WMD with NMD word distances
-  * may require proper EMD implementation?
+    * look for all strings that are approximately prefixed
+    * like existing index but not normalized and ignoring unmatched ngrams from target
 
 ## Publishing (notes for myself)
 
 * init
-  * `pip install flit`
-  * `flit init`
-  * make sure `nmd/__init__.py` contains a docstring and version
+    * `pip install flit`
+    * `flit init`
+    * make sure `nmd/__init__.py` contains a docstring and version
 * publish / update
-  * increment `__version__` in `nmd/__init__.py`
+    * increment `__version__` in `nmd/__init__.py`
+    * `flit publish`
```

### Comparing `nmd-0.0.5/automata.py` & `nmd-0.0.6/experiments/automata.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Dict
 from typing import FrozenSet
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
 # defined types
-from find_replace_trie import Trie
+from experiments.find_replace_trie import Trie
 from sizeof import deep_sizeof
 
 State = Tuple[int, int]  # tuple of (position, distance)
 DFAState = FrozenSet[State]  # a set of all NFA states reachable with the same input
 
 
 class NFA(object):
```

### Comparing `nmd-0.0.5/british-english-insane.txt` & `nmd-0.0.6/experiments/british-english-insane.txt`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/dawg-orig.py` & `nmd-0.0.6/experiments/dawg-orig.py`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/dawg.py` & `nmd-0.0.6/experiments/dawg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """
 see: https://gist.github.com/smhanov/94230b422c2100ae4218
-
 """
-import random
-import time
-
-from sizeof import deep_sizeof
 
 
 class DAWGNode(object):
     """
     This class represents a node in the directed acyclic word graph (DAWG).
     It has a list of edges to other nodes.
     It has functions for testing whether it is equivalent to another node.
@@ -226,14 +221,18 @@
 
     def get_index(self, i):
         assert i < len(self.data)
         return self.root[i]
 
 
 if __name__ == '__main__':
+    import random
+    import time
+    from sizeof import deep_sizeof
+
     words = sorted(line.split(',')[0].strip().lower() for line in open('british-english-insane.txt', encoding='utf8'))
 
     print('building...')
     start = time.time()
     dawg = DAWG()
     WordCount = 0
     for word in sorted(set(words)):
```

### Comparing `nmd-0.0.5/experiment.py` & `nmd-0.0.6/experiments/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,89 +61,89 @@
     answer_slow = emd_1d_slow(positions_x, positions_y)
     assert abs(answer_fast - answer_slow) < 0.00000001, (answer_slow, answer_fast, positions_x, positions_y)
     return answer_fast
 
 
 if __name__ == '__main__':
 
-    from levenshtein import damerau_levenshtein_distance
-    from levenshtein import edit_distance
+    from experiments.edit_distance import damerau_levenshtein_distance
+    from experiments.edit_distance import edit_distance
 
 
     def speed_test(word_1: str, word_2: str):
         edit_distance(word_1, word_2)
         damerau_levenshtein_distance(word_1, word_2)
         return ngram_movers_distance(word_1, word_2)
 
 
-    num_x = 3
-    num_y = 7
-
-    xs = [i / (num_x - 1) for i in range(num_x)]
-    ys = [i / (num_y - 1) for i in range(num_y)]
-    # print(xs)
-    # print(ys)
-    xs = xs + xs + xs
-
-    for x_len in range(len(xs) + 1):
-        for y_len in range(len(ys) + 1):
-            print(x_len, y_len)
-            for x_combi in itertools.combinations(xs, x_len):
-                for y_combi in itertools.combinations(ys, y_len):
-                    assert abs(
-                        check_correct_emd_1d(x_combi, y_combi) - check_correct_emd_1d(y_combi, x_combi)) < 0.0001, (
-                    x_combi, y_combi)
-
-    for _ in range(1000):
-        speed_test('aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa',
-                   'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
-        speed_test('aabbbbbbbbaa', 'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
-        speed_test('aaaabbbbbbbbaaaa', 'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
-        speed_test('banana', 'bababanananananananana')
-        speed_test('banana', 'bababanananananananananna')
-        speed_test('banana', 'nanananananabababa')
-        speed_test('banana', 'banana')
-        speed_test('nanananananabababa', 'banana')
-        speed_test('banana', 'bababananananananananannanananananananana')
-        speed_test('banana', 'bababananananananananannananananananananananananananannanananananananana')
-        speed_test('bananabababanana', 'bababananananananananannananananananananananananananannananabanananananana')
-
-    # test cases: https://www.watercoolertrivia.com/blog/schwarzenegger
-    with open('schwarzenegger.txt') as f:
-        for line in f:
-            print('schwarzenegger', line.strip(), speed_test(line.strip(), 'schwarzenegger'))
-
-    # real world test cases
-    with open('words_en.txt') as f1:
-        with open('words_ms.txt') as f2:
-            for en, ms in zip(f1, f2):
-                speed_test(en.strip(), ms.strip())
-                speed_test(en.strip(), en.strip())
-                speed_test(ms.strip(), ms.strip())
+    # num_x = 3
+    # num_y = 7
+    #
+    # xs = [i / (num_x - 1) for i in range(num_x)]
+    # ys = [i / (num_y - 1) for i in range(num_y)]
+    # # print(xs)
+    # # print(ys)
+    # xs = xs + xs + xs
+    #
+    # for x_len in range(len(xs) + 1):
+    #     for y_len in range(len(ys) + 1):
+    #         print(x_len, y_len)
+    #         for x_combi in itertools.combinations(xs, x_len):
+    #             for y_combi in itertools.combinations(ys, y_len):
+    #                 assert abs(
+    #                     check_correct_emd_1d(x_combi, y_combi) - check_correct_emd_1d(y_combi, x_combi)) < 0.0001, (
+    #                     x_combi, y_combi)
+    #
+    # for _ in range(1000):
+    #     speed_test('aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa',
+    #                'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
+    #     speed_test('aabbbbbbbbaa', 'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
+    #     speed_test('aaaabbbbbbbbaaaa', 'aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa')
+    #     speed_test('banana', 'bababanananananananana')
+    #     speed_test('banana', 'bababanananananananananna')
+    #     speed_test('banana', 'nanananananabababa')
+    #     speed_test('banana', 'banana')
+    #     speed_test('nanananananabababa', 'banana')
+    #     speed_test('banana', 'bababananananananananannanananananananana')
+    #     speed_test('banana', 'bababananananananananannananananananananananananananannanananananananana')
+    #     speed_test('bananabababanana', 'bababananananananananannananananananananananananananannananabanananananana')
+    #
+    # # test cases: https://www.watercoolertrivia.com/blog/schwarzenegger
+    # with open('schwarzenegger.txt') as f:
+    #     for line in f:
+    #         print('schwarzenegger', line.strip(), speed_test(line.strip(), 'schwarzenegger'))
+    #
+    # # real world test cases
+    # with open('words_en.txt') as f1:
+    #     with open('words_ms.txt') as f2:
+    #         for en, ms in zip(f1, f2):
+    #             speed_test(en.strip(), ms.strip())
+    #             speed_test(en.strip(), en.strip())
+    #             speed_test(ms.strip(), ms.strip())
 
     with open('words_ms.txt', encoding='utf8') as f:
         words_ms = set(f.read().split())
 
-    awl3_ms = ApproxWordList3((2,))
+    awl3_ms = ApproxWordListV3((1, 2, 3, 4))
     for word in words_ms:
         awl3_ms.add_word(word)
 
-    awl5_ms = WordList((2,))
+    awl5_ms = WordList((1, 2, 3, 4))
     for word in words_ms:
         awl5_ms.add_word(word)
 
     with open('words_en.txt', encoding='utf8') as f:
         # with open('british-english-insane.txt', encoding='utf8') as f:
         words = set(f.read().split())
 
-    awl3_en = ApproxWordList3((2,))
+    awl3_en = ApproxWordListV3((1, 2, 3, 4))
     for word in words:
         awl3_en.add_word(word)
 
-    awl5_en = WordList((2,))
+    awl5_en = WordList((1, 2, 3, 4))
     for word in words:
         awl5_en.add_word(word)
 
     # bananana
     # supercallousedfragilemisticexepialidocus
     # asalamalaikum
     # beewilldermant
@@ -172,14 +172,19 @@
 
         t = time.time()
         print('awl5_ms', awl5_ms.lookup(word))
         print(time.time() - t)
         print()
 
         t = time.time()
+        print('awl5_ms_denorm', awl5_ms.lookup(word, normalize=False))
+        print(time.time() - t)
+        print()
+
+        t = time.time()
         print('difflib_ms', difflib.get_close_matches(word, words_ms, n=10))
         print(time.time() - t)
         print()
 
         t = time.time()
         print('difflib_ms', difflib.get_close_matches(word, words_ms, n=10, cutoff=0.3))
         print(time.time() - t)
@@ -192,14 +197,19 @@
 
         t = time.time()
         print('awl5_en', awl5_en.lookup(word))
         print(time.time() - t)
         print()
 
         t = time.time()
+        print('awl5_en_denorm', awl5_en.lookup(word, normalize=False))
+        print(time.time() - t)
+        print()
+
+        t = time.time()
         print('difflib_en', difflib.get_close_matches(word, words, n=10))
         print(time.time() - t)
         print()
 
         t = time.time()
         print('difflib_en', difflib.get_close_matches(word, words, n=10, cutoff=0.3))
         print(time.time() - t)
@@ -216,15 +226,14 @@
         print()
 
         t = time.time()
         print('automata dist 3 en', list(find_all_matches(word, 3, m)))
         print(time.time() - t)
         print()
 
-
 if __name__ == '__main__':
 
     with open('translate-reference.txt') as f:
         ref_lines = f.readlines()
     with open('translate-google-offline.txt') as f:
         hyp_lines = f.readlines()
 
@@ -254,8 +263,7 @@
     print(tmp[1])
     print(tmp[2])
     print(tmp[3])
     print(tmp[-1])
     print(tmp[-2])
     print(tmp[-3])
     print(tmp[-4])
-
```

### Comparing `nmd-0.0.5/find_replace_trie.py` & `nmd-0.0.6/experiments/find_replace_trie.py`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/levenshtein.py` & `nmd-0.0.6/experiments/edit_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     :param hyp: hypothesis sentence
     :param ref: reference sentence
     :param deletion: deletion cost
     :param insertion: insertion cost
     :param substitution: substitution cost
     :param jump: jump cost
     :param rho: coverage cost weight
+    :param debug: print the full table of costs
     :return: EED score of hyp given ref (not symmetric)
     """
 
     # start and end with whitespace to facilitate jumps to front/end
     # works better when you use the most common whitespace (usually spaces)
     # this step is defined as part of the algorithm
     hyp = f' {hyp} '
@@ -108,15 +109,15 @@
     debug_str = []  # matched string
     debug_cost = []  # costs
     debug_idx = []  # indices of matched string
 
     # coverage: count how many times each char is visited
     visit_coverage = [0.0] * (len(hyp) + 1)
 
-    # the i-th row stores cost of cheapest path from (0,0) to (i,l) in CDER alignment grid
+    # the i-th row stores cost of the cheapest path from (0,0) to (i,l) in CDER alignment grid
     row = [0.0] + [1.0] * len(hyp)  # CDER initial row
 
     for ref_idx, ref_char in enumerate(ref):
         next_row = [float('inf')] * (len(hyp) + 1)
 
         # add 1 to the cost per row (same as edit distance)
         next_row[0] = row[0] + 1.0
```

### Comparing `nmd-0.0.5/nmd/nmd.py` & `nmd-0.0.6/nmd/nmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,30 @@
         raise TypeError(n)
     if n < 2:
         raise ValueError(n)  # technically it would work for n==1, but we'd want to drop the START and END flags
 
     # add START_TEXT and END_TEXT markers to each word
     # https://en.wikipedia.org/wiki/Control_character#Transmission_control
     # the usage of these characters in any text is almost certainly a bug
+    # it is possible to avoid using these characters by using a tuple of optional strings for each n-gram
+    # but that's slightly slower and uses more memory
     word_1 = f'\2{word_1}\3'
     word_2 = f'\2{word_2}\3'
 
     # number of n-grams per word
     num_grams_1 = len(word_1) - n + 1
     num_grams_2 = len(word_2) - n + 1
 
     # generate n_gram indices and index their locations
     n_gram_locations_1 = dict()
     for idx in range(num_grams_1):
-        n_gram_locations_1.setdefault(word_1[idx:idx + n], []).append(idx / (num_grams_1 - 1))
+        n_gram_locations_1.setdefault(word_1[idx:idx + n], []).append(idx / max(1, num_grams_1 - 1))
     n_gram_locations_2 = dict()
     for idx in range(num_grams_2):
-        n_gram_locations_2.setdefault(word_2[idx:idx + n], []).append(idx / (num_grams_2 - 1))
+        n_gram_locations_2.setdefault(word_2[idx:idx + n], []).append(idx / max(1, num_grams_2 - 1))
 
     # we want to calculate the earth mover distance for all n-grams in both words, which uses the following equation:
     # > distance = sum(emd_1d(n_gram_locations_1.get(n_gram, []), n_gram_locations_2.get(n_gram, []))
     # >                for n_gram in set(n_gram_locations_1).union(set(n_gram_locations_2)))
     # this could be optimized by only calculating emd for n-grams in common and just counting the symmetric difference
     # but calculating similarity (i.e. inverted distance) runs even faster than that
     # so instead we calculate the similarity and then find distance using the following identity:
```

### Comparing `nmd-0.0.5/nmd/nmd_bow.py` & `nmd-0.0.6/nmd/nmd_bow.py`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/nmd/nmd_index.py` & `nmd-0.0.6/nmd/nmd_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,15 +149,14 @@
             matches[other_word_index] = norm_scores
 
         # average the similarity scores
         return Counter({word_index: (sum(x ** dim for x in scores) / len(scores)) ** (1 / dim)
                         for word_index, scores in matches.items()})
 
     def lookup(self, word: str, top_k: int = 10, dim: Union[int, float] = 1):
-        # t = time.time()
         if not isinstance(word, str):
             raise TypeError(word)
         if len(word) == 0:
             raise ValueError(word)
 
         if self.__case_insensitive:
             word = word.casefold()
@@ -171,16 +170,16 @@
         # return only top_k results if specified (and non-zero), otherwise return all results
         if not top_k or top_k < 0:
             top_k = len(counter)
 
         # also return edit distances for debugging
         out = [(self.__vocabulary[word_index],
                 match_score,
-                # damerau_levenshtein_distance(word, self.__vocabulary[word_index]),
-                # edit_distance(word, self.__vocabulary[word_index]),
+                # (debugging) damerau_levenshtein_distance(word, self.__vocabulary[word_index]),
+                # (debugging) edit_distance(word, self.__vocabulary[word_index]),
                 ngram_movers_distance(word, self.__vocabulary[word_index], invert=True, normalize=True),
                 )
                for word_index, match_score in counter.most_common(top_k * 2)]
 
         # print(time.time() - t)
         return out[:top_k]
 
@@ -210,15 +209,15 @@
         # vocabulary: word <-> word_index
         self.__word_indices: Dict[str, int] = dict()  # word -> word_index
         self.__word_list: List[str] = []  # word_index -> word
         self.__word_lens: List[int] = []  # word_index -> len(word)
         self.__word_num_grams: List[Tuple[int]] = []  # word_index -> [num_grams(len(word), n) for n in self.__n_list]
 
         # n-gram filter: n_gram -> {word_index, ...}
-        self.__filter_n = filter_n
+        self.__filter_n: int = filter_n
         self.__ngram_filter: Dict[str, Set[int]] = dict()
 
         # n-gram counts: n_gram -> [(word_index, count), ...]
         self.__ngram_counts: Dict[str, List[Tuple[int, int]]] = dict()
 
         # n-gram normalized positions: n_gram -> [(word_index, (loc, loc, ...)), ...]
         self.__ngram_positions: Dict[str, List[Tuple[int, Tuple[float, ...]]]] = dict()
@@ -296,14 +295,15 @@
 
         return self
 
     def __lookup_similarity(self,
                             word: str,
                             dim: Union[int, float],
                             top_k: int,
+                            normalize: bool,
                             ) -> Counter:
         # todo: use existing indices and calculate cosine distance
         # todo: use existing indices and calculate jaccard
 
         assert isinstance(top_k, int) and top_k >= 1
         len_word = len(word)
 
@@ -316,20 +316,20 @@
         min_scores: Dict[int, List[int]] = dict()  # word_index -> [count_for_n, ...]
         for n_idx, n in enumerate(self.__n_list):
             for n_gram, count in Counter(get_n_grams(word, n)).items():
                 for other_word_index, other_count in self.__ngram_counts.get(n_gram, []):
                     if self.__filter_n and other_word_index not in possible_word_indices:
                         continue
                     if other_word_index not in min_scores:
-                        min_scores[other_word_index] = [0 for _ in range(len(self.__n_list))]
-                    denominator = num_grams(len_word, n) + self.__word_num_grams[other_word_index][n_idx]
-                    if count < other_count:
-                        min_scores[other_word_index][n_idx] += count / denominator
+                        min_scores[other_word_index] = [0] * len(self.__n_list)
+                    if normalize:
+                        denominator = num_grams(len_word, n) + self.__word_num_grams[other_word_index][n_idx]
+                        min_scores[other_word_index][n_idx] += min(count, other_count) / denominator
                     else:
-                        min_scores[other_word_index][n_idx] += other_count / denominator
+                        min_scores[other_word_index][n_idx] += min(count, other_count)
 
         # no results, return empty Counter
         if not min_scores:
             return Counter()
 
         # get min possible score per word
         _scores = [mean(scores, dim=dim) for scores in min_scores.values()]
@@ -360,23 +360,31 @@
                     word_scores[n_idx] -= emd_1d(locations, other_locations)
 
         # normalize scores
         for other_word_index, word_scores in matches.items():
             other_len = self.__word_lens[other_word_index]
 
             # should take other word into account too
-            norm_scores = [word_scores[n_idx] / (num_grams(len_word, n) + num_grams(other_len, n))
-                           for n_idx, n in enumerate(self.__n_list)]
-            matches[other_word_index] = norm_scores
+            if normalize:
+                norm_scores = [word_scores[n_idx] / (num_grams(len_word, n) + num_grams(other_len, n))
+                               for n_idx, n in enumerate(self.__n_list)]
+                matches[other_word_index] = norm_scores
+            else:
+                matches[other_word_index] = word_scores
 
         # average the similarity scores
         return Counter({word_index: mean(scores, dim) for word_index, scores in matches.items()})
 
-    def lookup(self, word: str, top_k: int = 5, dim: Union[int, float] = 1, invert=True):
-        # t = time.time()
+    def lookup(self,
+               word: str,
+               top_k: int = 5,
+               dim: Union[int, float] = 1,
+               invert: bool = True,
+               normalize: bool = False,
+               ):
         if not isinstance(word, str):
             raise TypeError(word)
         if len(word) == 0:
             raise ValueError(word)
         if not isinstance(top_k, int):
             raise TypeError(top_k)
         if top_k <= 0:
@@ -384,23 +392,23 @@
 
         if self.__case_insensitive:
             word = word.casefold()
 
         assert '\2' not in word and '\3' not in word, word
 
         # average the similarity scores
-        word_scores = self.__lookup_similarity(word, dim, top_k).most_common(top_k * 2)
+        word_scores = self.__lookup_similarity(word, dim, top_k, normalize).most_common(top_k * 2)
 
         # also return edit distances for debugging
         out = [(self.__word_list[word_index],  # word
-                match_score if invert else 1 - match_score,  # lookup result
-                # damerau_levenshtein_distance(word, self.__word_list[word_index]),
-                # edit_distance(word, self.__word_list[word_index]),
-                ngram_movers_distance(word, self.__word_list[word_index], invert=invert, normalize=True),
+                match_score if invert else normalize - match_score,  # lookup result
+                # (debugging) damerau_levenshtein_distance(word, self.__word_list[word_index]),
+                # (debugging) edit_distance(word, self.__word_list[word_index]),
+                ngram_movers_distance(word, self.__word_list[word_index], invert=invert, normalize=normalize),
                 )
                for word_index, match_score in word_scores]
 
         # print(time.time() - t)
-        return out
+        return sorted(out, key=lambda x: x[1:])
 
 
 WordList = ApproxWordListV5
```

### Comparing `nmd-0.0.5/schwarzenegger.txt` & `nmd-0.0.6/experiments/schwarzenegger.txt`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/sizeof.py` & `nmd-0.0.6/experiments/sizeof.py`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/tokenizer.py` & `nmd-0.0.6/experiments/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,38 +414,38 @@
     elif split_newline:
         assert isinstance(split_newline, str)
         paragraphs = [para.strip() for para in text.split(split_newline)]
     else:
         paragraphs = [text.strip()]
 
     for para in paragraphs:
-        buffer = []
+        _buffer = []
         closed = False
         for token in unicode_tokenize(para, as_tokens=True, merge_apostrophe_word=merge_apostrophe_word):
-            buffer.append(token)
+            _buffer.append(token)
 
             # sentence has ended iff whitespace follows the closing punctuation
             if closed and token.category is TokenCategory.WHITESPACE:
-                if buffer:
-                    yield buffer
-                buffer = []
+                if _buffer:
+                    yield _buffer
+                _buffer = []
                 closed = False
                 continue
 
             # note that this can also un-close a sentence, e.g. for "192.168.1.1"
             if token.text not in {'"', '\uFF02',
                                   ')', '\uFF09',
                                   '>', '\uFF1E',
                                   ']', '\uFF3D',
                                   '}', '\uFF5D',
                                   '\u201D'}:
                 closed = token.text in CLOSING_PUNCTUATION
 
-        if buffer:
-            yield buffer
+        if _buffer:
+            yield _buffer
 
 
 def sentence_split(text: str,
                    split_newline: Union[str, bool] = True,
                    merge_apostrophe_word: bool = False,
                    ) -> Generator[str, Any, None]:
     """
```

### Comparing `nmd-0.0.5/words_en.txt` & `nmd-0.0.6/experiments/words_en.txt`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/words_ms.txt` & `nmd-0.0.6/experiments/words_ms.txt`

 * *Files identical despite different names*

### Comparing `nmd-0.0.5/PKG-INFO` & `nmd-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: nmd
-Version: 0.0.5
+Version: 0.0.6
 Summary: A string similarity measure based on the Earth Mover's Distance
 Author-email: Avery Khoo <averykhoo@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/averykhoo/ngram-movers-distance
 
 # N-gram Mover's Distance
 
-A string similarity measure based on Earth Mover's Distance
+* A string similarity measure based on Earth Mover's Distance
+* See [ngram-movers-distance](https://github.com/averykhoo/ngram-movers-distance) for code
 
 ## Why another string matching algorithm?
 
 * Edit distance really wasn't cutting it when I needed to look up a dictionary for a misspelled word
-  * With an edit distance of 1 or 2, the results are not very useful
-  * With a distance >=5, the results are meaningless
-  * Same goes for Damerau-Levenshtein
+    * With an edit distance of 1 or 2, the results are not useful since the target word isn't found
+    * With a distance >=5, the results are meaningless since it contains half the dictionary
+    * Same goes for Damerau-Levenshtein
 * Also, edit distance is pretty slow when looking up long words in a large dictionary
-  * Even with a decent automaton or trie implementation
-  * NMD was designed with indexing in mind
-  * A simpler index could be used for Jaccard or cosine similarity over ngrams
-    * todo: try [this paper's algo](https://www.aclweb.org/anthology/C10-1096.pdf)
-    * which referenced [this paper](https://www.cse.iitb.ac.in/~sunita/papers/sigmod04.pdf)
+    * Even after building a finite state automaton or using a trie to optimize lookup
+    * NMD was designed with indexing in mind
+        * A simpler index could be used for Jaccard or cosine similarity over ngrams
+* EMD (and hence NMD) can be optimized to run really fast with some constraints
+    * Values are 1-dimensional scalars
+    * Values are always quantized
 
 # Usage
 
 ## `ngram_movers_distance()`
 
 * string distance metric, use this to compare two strings
 
@@ -50,15 +52,15 @@
 
 * use this for dictionary lookups of words
 
 ```python
 from nmd import WordList
 
 # get words from a text file
-with open(f'words_ms.txt', encoding=f'utf8') as f:
+with open(f'dictionary.txt', encoding=f'utf8') as f:
     words = set(f.read().split())
 
 # index words
 word_list = WordList((2, 4), filter_n=0)  # combined 2- and 4-grams seem to work best
 for word in words:
     word_list.add_word(word)
 
@@ -67,36 +69,43 @@
 print(word_list.lookup(f'walaikumalasam'))  # -> 'waalaikumsalam'
 ```
 
 ## `bow_ngram_movers_distance()`
 
 * WARNING: requires `scipy.optimize`, so it's not available by default in the `nmd` namespace
 * use this to compare sequences of tokens (not necessarily unique)
+* note that this does not merge or split words, so if you're matching `["pineapple"]` and `["pine", "apple"]` the
+  similarity will be low. consider just using nmd in this case.
 
 ```python
 from nmd.nmd_bow import bow_ngram_movers_distance
-from tokenizer import unicode_tokenize
 
 text_1 = f'Clementi Sports Hub'
 text_2 = f'sport hubs clemmeti'
-print(bow_ngram_movers_distance(bag_of_words_1=unicode_tokenize(text_1.casefold(), words_only=True),
-                                bag_of_words_2=unicode_tokenize(text_2.casefold(), words_only=True),
+print(bow_ngram_movers_distance(bag_of_words_1=text_1.casefold().split(),
+                                bag_of_words_2=text_2.casefold().split(),
                                 invert=True,  # invert: return similarity instead of distance
                                 normalize=True,  # return a score between 0 and 1
                                 ))
 ```
 
 # todo
 
+* todo: try [this paper's algo](https://www.aclweb.org/anthology/C10-1096.pdf)
+    * which referenced [this paper](https://www.cse.iitb.ac.in/~sunita/papers/sigmod04.pdf)
 * use less bizarre test strings
+* note where the algorithm breaks down
+    * matching long strings with many n-grams
+    * matching strings with significantly different lengths
+    *
 * rename nmd_bow because it isn't really a bag-of-words, it's a token sequence
 * consider a `real_quick_ratio`-like optimization, or maybe calculate length bounds?
-  * needs a cutoff to actually speed up though, makes a huge difference for difflib
-  * a sufficiently low cutoff is not unreasonable, although the default of 0.6 might be a little high for nmd
-  * that said the builtin diff performs pretty badly at low similarities, so 0.6 is reasonable for them
+    * needs a cutoff to actually speed up though, makes a huge difference for difflib
+    * a sufficiently low cutoff is not unreasonable, although the default of 0.6 might be a little high for nmd
+    * that said the builtin diff performs pretty badly at low similarities, so 0.6 is reasonable for them
 
 ```python
 def real_quick_ratio(self):
     """Return an upper bound on ratio() very quickly.
 
     This isn't defined beyond that it is an upper bound on .ratio(), and
     is faster to compute than either .ratio() or .quick_ratio().
@@ -107,37 +116,34 @@
     matches, length = min(la, lb), la + lb
     if length:
         return 2.0 * matches / length
     return 1.0
 ```
 
 * create a better string container for the index, more like a `set`
-  * `add(word: str)`
-  * `remove(word: str)`
-  * `clear()`
-  * `__contains__(word: str)`
-  * `__iter__()`
+    * `add(word: str)`
+    * `remove(word: str)`
+    * `clear()`
+    * `__contains__(word: str)`
+    * `__iter__()`
 * better lookup
-  * add a min_similarity filter (float, based on normalized distance)
-    * `lookup(word: str, min_similarity: float = 0, filter: bool = True)`
-  * try `__contains__` first
-    * try levenshtein automaton (distance=1) second?
-      * sort by nmd, since most likely there will only be a few results
-    * but how to get multiple results?
-      * still need to run full search?
-      * or maybe just return top 1 result?
-  * make the 3-gram filter optional
+    * add a min_similarity filter (float, based on normalized distance)
+        * `lookup(word: str, min_similarity: float = 0, filter: bool = True)`
+    * try `__contains__` first
+        * try levenshtein automaton (distance=1) second?
+            * sort by nmd, since most likely there will only be a few results
+        * but how to get multiple results?
+            * still need to run full search?
+            * or maybe just return top 1 result?
 * prefix lookup
-  * look for all strings that are approximately prefixed
-  * like existing index but not normalized and ignoring unmatched ngrams from target
-* bag of words
-  * use WMD with NMD word distances
-  * may require proper EMD implementation?
+    * look for all strings that are approximately prefixed
+    * like existing index but not normalized and ignoring unmatched ngrams from target
 
 ## Publishing (notes for myself)
 
 * init
-  * `pip install flit`
-  * `flit init`
-  * make sure `nmd/__init__.py` contains a docstring and version
+    * `pip install flit`
+    * `flit init`
+    * make sure `nmd/__init__.py` contains a docstring and version
 * publish / update
-  * increment `__version__` in `nmd/__init__.py`
+    * increment `__version__` in `nmd/__init__.py`
+    * `flit publish`
```

