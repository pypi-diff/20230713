# Comparing `tmp/yiddish-0.0.8.tar.gz` & `tmp/yiddish-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yiddish-0.0.8.tar", last modified: Wed Apr 19 16:48:02 2023, max compression
+gzip compressed data, was "yiddish-0.0.9.tar", last modified: Wed Jul 12 22:16:09 2023, max compression
```

## Comparing `yiddish-0.0.8.tar` & `yiddish-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.570180 yiddish-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-19 16:47:53.000000 yiddish-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-19 16:48:02.566180 yiddish-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-19 16:47:53.000000 yiddish-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 16:47:53.000000 yiddish-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:48:02.570180 yiddish-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 16:47:53.000000 yiddish-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.566180 yiddish-0.0.8/yiddish/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 16:47:53.000000 yiddish-0.0.8/yiddish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-04-19 16:47:53.000000 yiddish-0.0.8/yiddish/yiddish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:48:02.566180 yiddish-0.0.8/yiddish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 16:48:02.000000 yiddish-0.0.8/yiddish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:16:09.940023 yiddish-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-12 22:15:59.000000 yiddish-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-12 22:16:09.940023 yiddish-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-12 22:15:59.000000 yiddish-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 22:15:59.000000 yiddish-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 22:16:09.940023 yiddish-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-12 22:15:59.000000 yiddish-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:16:09.940023 yiddish-0.0.9/yiddish/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-12 22:15:59.000000 yiddish-0.0.9/yiddish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25501 2023-07-12 22:15:59.000000 yiddish-0.0.9/yiddish/yiddish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:16:09.940023 yiddish-0.0.9/yiddish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-12 22:16:09.000000 yiddish-0.0.9/yiddish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-12 22:16:09.000000 yiddish-0.0.9/yiddish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:16:09.000000 yiddish-0.0.9/yiddish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 22:16:09.000000 yiddish-0.0.9/yiddish.egg-info/top_level.txt
```

### Comparing `yiddish-0.0.8/LICENSE` & `yiddish-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yiddish-0.0.8/PKG-INFO` & `yiddish-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: yiddish
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for processing Yiddish text
 Home-page: https://github.com/ibleaman/yiddish
 Author: Isaac L. Bleaman
 Author-email: bleaman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 # yiddish
 
 A Python library for processing Yiddish text
 
 Isaac L. Bleaman (<bleaman@berkeley.edu>) and contributors (see commit history)
```

### Comparing `yiddish-0.0.8/README.md` & `yiddish-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yiddish-0.0.8/yiddish/yiddish.py` & `yiddish-0.0.9/yiddish/yiddish.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # yiddish
 # A Python library for processing Yiddish text
-# Author: Isaac L. Bleaman (bleaman@berkeley.edu)
+# https://github.com/ibleaman/yiddish/
 
 import re
-from urllib.request import urlopen
 import csv
 
 ##########
 # encoding
 ##########
 
 pairs = [
@@ -62,18 +61,17 @@
 ##########################################
 
 
 #########################################
 # import loshn-koydesh pronunciation list
 #########################################
 
-respellings_url = 'https://raw.githubusercontent.com/ibleaman/loshn-koydesh-pronunciation/master/orthographic-to-phonetic.txt'
-respellings_list = urlopen(respellings_url).read().decode('utf-8')
-respellings_list = respellings_list.split('\n')
-respellings_list = [line for line in respellings_list if line]
+with open('submodules/loshn-koydesh-pronunciation/orthographic-to-phonetic.txt', 'r') as file:
+    respellings_list = file.read().split('\n')
+    respellings_list = [line for line in respellings_list if line]
 
 lk = {} # orthographic to phonetic
 reverse_lk = {} # phonetic to orthographic
 
 for line in respellings_list:
     key = replace_with_precombined(line.split('\t')[0])
     key = replace_punctuation(key)
@@ -335,14 +333,17 @@
     (r'\barbets', 'אַרבעטס'),
     (r'\barbayts', 'אַרבײַטס'),
     (r'\bdemolts', 'דעמאָלטס'),
     (r'\bgots', 'גאָטס'),
     (r'\bguts', 'גוטס'),
     (r'\bgeshefts', 'געשעפֿטס'),
     (r'(\b|ba|far|der)haltst', r'\1האַלטסט'),
+    (r'\bnentst', 'נענטסט'),
+    (r'\bneentst', 'נעענטסט'),
+    (r'\bnoentst', 'נאָענטסט'),
     (r'\bshlekhts\b', 'שלעכטס'),
     (r'(\b|tse)shpaltst', r'\1שפּאַלטסט'),
     (r'(\b|tse|far)shpreytst', r'\1שפּרײטסט'),
     (r'shpetst', 'שפּעטסט'),
     (r'\brekhts\b', 'רעכטס'),
     (r'du shatst', 'דו שאַטסט'), # cf. ער שאַצט
     (r'\bforverts\b', 'פֿאָרװערטס'),
@@ -362,14 +363,15 @@
     'אָדער',
     'אױפֿן',
     'איבער',
     'אײן',
     'אים',
     'בױ',
     'דאַן',
+    'דינע',
     'װײס',
     'װעסט',
     'זאָל',
     'טאָמער',
     'טו',
     'לײען',
     'מאָגן',
@@ -467,14 +469,15 @@
         # skip Germanic homographs, which are usually phonetic
         if key not in germanic_semitic_homographs:
             # skip less common LK pronunciations, in favor of more common ones
             if lk[key][0] in less_common_lk_pronunciations and len(lk[key]) > 1:
                 replacement = lk[key][1]
             else:
                 replacement = lk[key][0]
+            
                 
             # replace whole words (separated by spaces & punctuation, but not
             # followed by an apostrophe);
             # also, append a Δ to the respelling so it's not accidentally overwritten
             # (e.g., to avoid סעודה to סודע to סױדע)
             text = re.sub(r'(?<![אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּתΔ])' + key + r'(?![\'אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּת])', 'Δ' + replacement, text)
     
@@ -493,49 +496,103 @@
         'יוד"שין': "יאַש",
         "יוד״שין": "יאַש",
     }
     for key in mistakes:
         text = re.sub(r'(?<![אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּת])' + key + r'(?![\'אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּת])', mistakes[key], text)
     
     return text
+
+#######################################################
+# convert phonetic spellings to loshn-koydesh spellings
+#######################################################
+
+# Note: input text WILL become precombined
+def spell_loshn_koydesh(text):
+    text = replace_with_precombined(text)
+    # loop over keys, in reverse order from longest keys to shortest
+    for key in sorted(list(reverse_lk.keys()), key=len, reverse=True):
+        # skip Germanic homophones
+        if key not in semitic_germanic_homophones:
+            replacement = reverse_lk[key]
+                
+            # replace whole words (separated by spaces & punctuation, but not
+            # followed by an apostrophe);
+            # also, append a Δ to the respelling so it's not accidentally overwritten
+            # (e.g., to avoid סעודה to סודע to סױדע)
+            text = re.sub(r'(?<![אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּתΔ])' + key + r'(?![\'אאַאָבבֿגדהװווּזחטייִײײַױכּכךלמםנןסעפּפפֿףצץקרששׂתּת])', 'Δ' + replacement, text)
     
+    # remove the added Δ
+    text = re.sub('Δ', '', text)
+
+    return text
+
 #######################################
 # convert YIVO orthography into Hasidic
 
 # note: all replacements are based on
 # looking for precombined characters
 #######################################
-hasidify_lexicon = 'https://raw.githubusercontent.com/ibleaman/hasidify_lexicon/master/'
-
-whole_word_variants = list(csv.reader(urlopen(hasidify_lexicon + 'whole_word_variants.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-whole_word_variants = dict(zip([replace_with_precombined(row[0]) for row in whole_word_variants if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in whole_word_variants if row[1] != 'Replace']))
-
-prefix_variants = list(csv.reader(urlopen(hasidify_lexicon + 'prefix_variants.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-prefix_variants = dict(zip([replace_with_precombined(row[0]) for row in prefix_variants if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in prefix_variants if row[1] != 'Replace']))
+hasidify_lexicon_path = 'submodules/hasidify_lexicon'
 
-suffix_variants = list(csv.reader(urlopen(hasidify_lexicon + 'suffix_variants.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-suffix_variants = dict(zip([replace_with_precombined(row[0]) for row in suffix_variants if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in suffix_variants if row[1] != 'Replace']))
-
-anywhere_variants = list(csv.reader(urlopen(hasidify_lexicon + 'anywhere_variants.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-anywhere_variants = dict(zip([replace_with_precombined(row[0]) for row in anywhere_variants if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in anywhere_variants if row[1] != 'Replace']))
-
-lkizmen = list(csv.reader(urlopen(hasidify_lexicon + 'lkizmen.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-lkizmen = [replace_with_precombined(row[0]) for row in lkizmen if row[0] != 'Words']
-
-word_group_variants = list(csv.reader(urlopen(hasidify_lexicon + 'word_group_variants.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-word_group_variants = dict(zip([replace_with_precombined(row[0]) for row in word_group_variants if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in word_group_variants if row[1] != 'Replace']))
-
-ik_exceptions = list(csv.reader(urlopen(hasidify_lexicon + 'ik_exceptions.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-ik_exceptions = [replace_with_precombined(row[0]) for row in ik_exceptions if row[0] != 'Words']
-
-lekh_exceptions = list(csv.reader(urlopen(hasidify_lexicon + 'lekh_exceptions.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-lekh_exceptions = [replace_with_precombined(row[0]) for row in lekh_exceptions if row[0] != 'Words']
-
-last_minute_fixes = list(csv.reader(urlopen(hasidify_lexicon + 'last_minute_fixes.csv').read().decode('utf-8').replace('\r', '').splitlines()))
-last_minute_fixes = dict(zip([replace_with_precombined(row[0]) for row in last_minute_fixes if row[0] != 'Find'], [replace_with_precombined(row[1]) for row in last_minute_fixes if row[1] != 'Replace']))
+whole_word_variants = dict()
+with open(f'{hasidify_lexicon_path}/whole_word_variants.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        whole_word_variants[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
+
+prefix_variants = dict()
+with open(f'{hasidify_lexicon_path}/prefix_variants.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        prefix_variants[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
+
+suffix_variants = dict()
+with open(f'{hasidify_lexicon_path}/suffix_variants.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        suffix_variants[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
+
+anywhere_variants = dict()
+with open(f'{hasidify_lexicon_path}/anywhere_variants.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        anywhere_variants[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
+
+lkizmen = []
+with open(f'{hasidify_lexicon_path}/lkizmen.csv', 'r') as file:
+    csv_reader = csv.reader(file)
+    header = next(csv_reader)  # Skip the header row
+    for row in csv_reader:
+        lkizmen.append(replace_with_precombined(row[0]))
+
+word_group_variants = dict()
+with open(f'{hasidify_lexicon_path}/word_group_variants.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        word_group_variants[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
+
+ik_exceptions = []
+with open(f'{hasidify_lexicon_path}/ik_exceptions.csv', 'r') as file:
+    csv_reader = csv.reader(file)
+    header = next(csv_reader)  # Skip the header row
+    for row in csv_reader:
+        ik_exceptions.append(replace_with_precombined(row[0]))
+
+lekh_exceptions = []
+with open(f'{hasidify_lexicon_path}/lekh_exceptions.csv', 'r') as file:
+    csv_reader = csv.reader(file)
+    header = next(csv_reader)  # Skip the header row
+    for row in csv_reader:
+        lekh_exceptions.append(replace_with_precombined(row[0]))
+
+last_minute_fixes = dict()
+with open(f'{hasidify_lexicon_path}/last_minute_fixes.csv', 'r') as file:
+    csv_reader = csv.DictReader(file)
+    for row in csv_reader:
+        last_minute_fixes[replace_with_precombined(row['Find'])] = replace_with_precombined(row['Replace'])
 
 reformatting = [
     ('וּװוּ', 'ואוואו'),
     ('ײיִ', 'ייאי'),
     ('ײַיִ', 'ייאי'), # frier, hebreish - no alef in HY forums AFAIK
     ('וּװ', 'ואוו'),
     ('װוּ', 'וואו'),
@@ -609,7 +666,44 @@
     for key, value in last_minute_fixes.items():
         text = re.sub(key, value, text)
     
     text = strip_diacritics(text)
     
     return text
     
+def desovietify(text):
+    text = replace_with_precombined(text)
+    text = re.split(r"([^אאַאָבבֿגדהווּװױזחטייִײײַכּכךלמםנןסעפפּפֿףצץקרששׂתּתA-Za-z'])", text)
+    
+    # add 'Γ' as a word/token boundary symbol
+    text = 'Γ'.join(text)
+    text = 'Γ' + text + 'Γ'
+
+    # replace unpointed alef with pasekh alef when not followed by vowels. 
+    # (unpointed alef, if not followed by a vov/yud-based vowel, is alway pasekh alef in Soviet orthography)
+    text = re.sub('א(?![י|יִ|ײ|ײַ|וּ|ױ|ו])', 'אַ', text)
+
+    # replace unpointed pey with fey
+    text = re.sub('פ', 'פֿ', text)
+
+    # replace final kof, mem, nun, tsadek, fey with long forms
+    text = re.sub('כ(?=Γ)', 'ך', text)
+    text = re.sub('מ(?=Γ)', 'ם', text)
+    text = re.sub('נ(?=Γ)', 'ן', text)
+    text = re.sub('צ(?=Γ)', 'ץ', text)
+    text = re.sub('פֿ(?=Γ)', 'ף', text)
+
+    # replace oyf, bay
+    text = re.sub('(?<=Γ)אַף(?=Γ)', 'אױף', text)
+    text = re.sub('(?<=Γ)אַפֿן(?=Γ)', 'אױפֿן', text)
+    text = re.sub('(?<=Γ)אוף(?=Γ)', 'אױף', text)
+    text = re.sub('(?<=Γ)אופֿ', 'אױפֿ', text)
+    text = re.sub('(?<=Γ)באַ(?=Γ)', 'בײַ', text)
+    text = re.sub('(?<=Γ)באַם(?=Γ)', 'בײַם', text)
+
+    text = spell_loshn_koydesh(text)
+
+    # remove Greek letters
+    text = text.replace('Δ', '')
+    text = text.replace('Γ', '')
+
+    return text
```

### Comparing `yiddish-0.0.8/yiddish.egg-info/PKG-INFO` & `yiddish-0.0.9/yiddish.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: yiddish
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for processing Yiddish text
 Home-page: https://github.com/ibleaman/yiddish
 Author: Isaac L. Bleaman
 Author-email: bleaman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 # yiddish
 
 A Python library for processing Yiddish text
 
 Isaac L. Bleaman (<bleaman@berkeley.edu>) and contributors (see commit history)
```

