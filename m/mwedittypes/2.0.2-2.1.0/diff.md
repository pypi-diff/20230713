# Comparing `tmp/mwedittypes-2.0.2.tar.gz` & `tmp/mwedittypes-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/edit-types/edit-types/dist/.tmp-mquhow_r/mwedittypes-2.0.2.tar", last modified: Wed Dec  7 22:41:51 2022, max compression
+gzip compressed data, was "/home/runner/work/edit-types/edit-types/dist/.tmp-ujfntg0j/mwedittypes-2.1.0.tar", last modified: Thu Jul 13 18:59:14 2023, max compression
```

## Comparing `mwedittypes-2.0.2.tar` & `mwedittypes-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25323 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/mwedittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/node_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/simple_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32402 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/tree_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/mwedittypes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/mwedittypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 22:41:51.000000 mwedittypes-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2022-12-07 22:41:42.000000 mwedittypes-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25376 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/mwedittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/node_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/simple_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32230 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/tree_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/mwedittypes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/mwedittypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:59:14.000000 mwedittypes-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_edittypes_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_edittypes_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-13 18:59:03.000000 mwedittypes-2.1.0/tests/test_tree_differ.py
```

### Comparing `mwedittypes-2.0.2/LICENSE` & `mwedittypes-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.0.2/PKG-INFO` & `mwedittypes-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwedittypes
-Version: 2.0.2
+Version: 2.1.0
 Summary: Edit diffs and type detection for Wikipedia
 Home-page: https://github.com/geohci/edit-types
 Author: geohci & Amamgbu (Isaac Johnson & Jesse Amamgbu)
 Author-email: <amamgbujesse@yahoo.com>
 License: MIT License
 Keywords: python,wikipedia,edit types,edit diffs,wiki,edit detection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mwedittypes-2.0.2/README.md` & `mwedittypes-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.0.2/mwedittypes/constants.py` & `mwedittypes-2.1.0/mwedittypes/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # pre and nowiki are for mono-spaced text (I leave out `code` because it generally contains code not text)
 # small / big / sub / sup all affect text size
 TEXT_FORMATTING_TAGS = ('b', 'i', 's', 'u', 'del', 'ins','hr', 'br','pre', 'nowiki','small',
                          'big', 'sub', 'sup', 'font', 'blockquote', 'span', 'center')
 TABLE_ELEMENTS_TAGS = ('th', 'tr', 'td')
 LIST_TAGS = ('li', 'dt', 'dd', 'ul', 'ol', 'dl')
 
-# CJK period/question/exclamation; Bengali full-stops
-NON_ENGLISH_FULL_STOPS = '。？！।॥'
+# CJK period/question/exclamation; Bengali full-stops; Armenian verǰaket (full-stop; resembles a colon)
+NON_ENGLISH_FULL_STOPS = '。？！।॥։'
 # This regex identifies end-of-sentence punctuation and new-lines as sentence breaks
 # It avoids matching dots between two digits but takes into account ellipses and fullstops.
 # fuller explanation:
 # [!?...] - 1 or more !, ?, new-line, or non-english stops
 # | - or
 # (?<!\.) - next character must not precede a fullstop
 # \. - next character
```

### Comparing `mwedittypes-2.0.2/mwedittypes/mwedittypes.py` & `mwedittypes-2.1.0/mwedittypes/mwedittypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 class StructuredEditTypes:
 
     def __init__(self, prev_wikitext='', curr_wikitext='', lang='en', timeout=False, debug=False):
         self.prev_wikitext = prev_wikitext
         self.curr_wikitext = curr_wikitext
         self.lang = lang
         self.timeout = timeout
-        self.debug = debug
         self.tree_diff = None
         self.actions = None
 
     def get_diff(self):
         self.tree_diff = get_diff(self.prev_wikitext, self.curr_wikitext, lang=self.lang,
-                                  timeout=self.timeout, debug=self.debug)
+                                  timeout=self.timeout)
         self.actions = get_diff_count(self.tree_diff, lang=self.lang)
         return self.actions
 
 
 class SimpleEditTypes:
 
     def __init__(self, prev_wikitext='', curr_wikitext='', lang='en'):
```

### Comparing `mwedittypes-2.0.2/mwedittypes/node_differ.py` & `mwedittypes-2.1.0/mwedittypes/node_differ.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import namedtuple
 import mwparserfromhell as mw
 
 from mwedittypes.tokenizer import parse_change_text
-from mwedittypes.utils import parse_image_options
+from mwconstants.media import parse_image_options
 
 NodeEdit = namedtuple('NodeEdit', ['type', 'edittype', 'section', 'name', 'changes'])
 TextEdit = namedtuple('TextEdit', ['type', 'edittype', 'text', 'count'])
 Context = namedtuple('Context', ['type', 'edittype', 'count'])
 
 
 def get_node_diff(node_type, prev_wikitext='', curr_wikitext='', lang='en'):
@@ -27,16 +27,16 @@
     -------
     changes
         List with specific differences between previous and current nodes. Most whitespace changes are ignored.
     """
     name = None
     changes = []
     try:
-        prev_wc = mw.parse(prev_wikitext).nodes[0] if prev_wikitext else None
-        curr_wc = mw.parse(curr_wikitext).nodes[0] if curr_wikitext else None
+        prev_wc = mw.parse(prev_wikitext, skip_style_tags=True).nodes[0] if prev_wikitext else None
+        curr_wc = mw.parse(curr_wikitext, skip_style_tags=True).nodes[0] if curr_wikitext else None
 
         if node_type == 'Template':
             # separate between name changes and parameter changes
             pt_name = prev_wc.name.strip() if prev_wc else None
             ct_name = curr_wc.name.strip() if curr_wc else None
             name = pt_name if pt_name else ct_name
             pt_params = {str(p.name).strip(): str(p.value).strip() for p in prev_wc.params} if prev_wc else {}
@@ -51,29 +51,23 @@
                                     (p, ct_params[p]) if p in ct_params else None))
 
         elif node_type == 'Media':
             # Media can be in three different formats:
             # Brackets: [[File:filename.ext|formatting options|caption]]
             # Template: File:filename.ext
             # Gallery: filename.ext|formatting options|caption
-            # If template or gallery, we add the brackets and re-parse so the title/options can be consistently handled
-            if prev_wikitext and not prev_wikitext.startswith('[['):
-                prev_wc = mw.parse(f'[[{prev_wikitext}]]').nodes[0]
-            if curr_wikitext and not curr_wikitext.startswith('[['):
-                curr_wc = mw.parse(f'[[{curr_wikitext}]]').nodes[0]
-
-            pm_title = prev_wc.title.strip() if prev_wc else None
-            cm_title = curr_wc.title.strip() if curr_wc else None
+            pm_title, pm_caption, pm_options = parse_image_options(prev_wc if prev_wc else '', lang=lang)
+            cm_title, cm_caption, cm_options = parse_image_options(curr_wc if curr_wc else '', lang=lang)
+            # remove leading/trailing whitespace as we don't want it affecting perceived changes
+            pm_title = pm_title.strip() if pm_title else None
+            cm_title = cm_title.strip() if cm_title else None
             name = pm_title if pm_title else cm_title
             if pm_title != cm_title:
                 changes.append(('filename', pm_title, cm_title))
 
-            pm_options, pm_caption = parse_image_options(prev_wc.text.strip() if prev_wc else '', lang=lang)
-            cm_options, cm_caption = parse_image_options(curr_wc.text.strip() if curr_wc else '', lang=lang)
-
             if pm_caption != cm_caption:
                 changes.append(('caption', pm_caption, cm_caption))
 
             options = set(pm_options).union(set(cm_options))
             for o in options:
                 if o not in pm_options:
                     changes.append(('option', None, o))
@@ -148,26 +142,26 @@
                     changes.append(('attribute',
                                     (a, pt_attrs[a]) if a in pt_attrs else None,
                                     (a, ct_attrs[a]) if a in ct_attrs else None))
 
             pt_caption = None
             pt_cells = {}
             if prev_wc:
-                for te in mw.parse(prev_wikitext).filter_tags():
+                for te in mw.parse(prev_wikitext, skip_style_tags=True).filter_tags():
                     if te.tag == 'td' or te.tag == 'th':
                         if '+' in [a.name for a in te.attributes] or te.contents.startswith('+'):
                             pt_caption = te.contents.lstrip('+')
                         else:
                             cell = hash(te.contents.strip())
                             pt_cells[cell] = pt_cells.get(cell, 0) + 1
 
             ct_caption = None
             ct_cells = {}
             if curr_wc:
-                for te in mw.parse(curr_wikitext).filter_tags():
+                for te in mw.parse(curr_wikitext, skip_style_tags=True).filter_tags():
                     if te.tag == 'td' or te.tag == 'th':
                         if '+' in [a.name for a in te.attributes] or te.contents.startswith('+'):
                             ct_caption = te.contents.lstrip('+')
                         else:
                             cell = hash(te.contents.strip())
                             ct_cells[cell] = ct_cells.get(cell, 0) + 1
 
@@ -188,22 +182,20 @@
                 changes.append(('cells', 'remove', removed))
             if changed:
                 changes.append(('cells', 'change', changed))
 
         elif node_type == 'Text Formatting':
             # check if format type / contents changed
             # Note this will skip '''text''' -> <b>text</b> which are both `b` tags (same for italics)
-            prev_tag = str(prev_wc.tag) if prev_wc else None
-            curr_tag = str(curr_wc.tag) if curr_wc else None
-            if prev_tag != curr_tag:
-                changes.append(('format tag', prev_tag, curr_tag))
-            prev_contents = str(prev_wc.contents) if prev_wc else None
-            curr_contents = str(curr_wc.contents) if curr_wc else None
-            if prev_contents != curr_contents:
-                changes.append(('contents', prev_contents, curr_contents))
+            if prev_wikitext is not None and '>' in prev_wikitext:
+                prev_wikitext = prev_wikitext[:prev_wikitext.find('>') + 1]
+            if curr_wikitext is not None and '>' in curr_wikitext:
+                curr_wikitext = curr_wikitext[:curr_wikitext.find('>') + 1]
+            if prev_wikitext != curr_wikitext:
+                changes.append(('format tag', prev_wikitext, curr_wikitext))
 
         elif node_type == 'HTMLEntity':
             # check if display value of the HTMLEntity has changed
             # This will ignore code differences that don't affect output
             # e.g., '&Delta;' vs. '&#916;' vs. '&#x0394;' are all the equivalent of 'Δ'
             prev_ent = prev_wc.normalize() if prev_wc else None
             curr_ent = curr_wc.normalize() if curr_wc else None
@@ -243,15 +235,15 @@
         elif node_type == 'Comment':
             # check if comment contents changed
             pc_contents = prev_wc.contents.strip() if prev_wc else None
             cc_contents = curr_wc.contents.strip() if curr_wc else None
             if pc_contents != cc_contents:
                 changes.append(('comment', pc_contents, cc_contents))
 
-        elif node_type == 'External Link':
+        elif node_type == 'ExternalLink':
             # separate between url and text (display) changes
             pe_url = prev_wc.url.strip() if prev_wc else None
             ce_url = curr_wc.url.strip() if curr_wc else None
             name = pe_url if pe_url else ce_url
             if pe_url != ce_url:
                 changes.append(('url', pe_url, ce_url))
 
@@ -282,51 +274,83 @@
     text_edits = []
     context = []
     section_titles = set()
     prev_text = []
     curr_text = []
 
     # go through each type of action (insert, remove, change, move) and compute edit types
+    # for text-formatting, the starting tags -- e.g., '' -- are captured independently of the
+    # ending tags. This means that insert/removal/change of a standard block of text-formatting will
+    # trigger two text-formatting changes in the tree differ. To account for that, we essentially skip
+    # every other text-formatting result.
+    tf_removes = set()
     for r in result['remove']:
         text = r['text']  # wikitext of the node
         et = r['type']
+        if et == 'Text Formatting' and text.startswith("'"):
+            if text in tf_removes:  # already added 'start' of text-formatting -- don't duplicate
+                tf_removes.remove(text)
+                continue
+            else:
+                tf_removes.add(text)
         section_titles.add(r['section'])
         # if node is text, just check whether there's anything and retain for later
         # because all the text is processed at once at the end
         if et == 'Text' and text:
             prev_text.append(text)
         # non-text node: verify/fine-tune the edit type and add to results dictionary
         else:
             name, changes = get_node_diff(node_type=et, prev_wikitext=text, curr_wikitext='', lang=lang)
             node_edits.append(NodeEdit(et, 'remove', r['section'], name, changes))
+    tf_inserts = set()
     for i in result['insert']:
         text = i['text']
         et = i['type']
+        if et == 'Text Formatting' and text.startswith("'"):
+            if text in tf_inserts:  # already added 'start' of text-formatting -- don't duplicate
+                tf_inserts.remove(text)
+                continue
+            else:
+                tf_inserts.add(text)
         section_titles.add(i['section'])
         if et == 'Text' and text:
             curr_text.append(text)
         else:
             name, changes = get_node_diff(node_type=et, prev_wikitext='', curr_wikitext=text, lang=lang)
             node_edits.append(NodeEdit(et, 'insert', i['section'], name, changes))
+    tf_changes = set()
     for c in result['change']:
         et = c['prev']['type']
         ptext = c['prev']['text']
         ctext = c['curr']['text']
+        if et == 'Text Formatting' and ptext.startswith("'"):
+            if ptext in tf_changes:  # already added 'start' of text-formatting -- don't duplicate
+                tf_changes.remove(ptext)
+                continue
+            else:
+                tf_changes.add(ptext)
         section_titles.add(c['curr']['section'])
         section_titles.add(c['prev']['section'])
         if et == 'Text' and ptext != ctext:
             prev_text.append(ptext)
             curr_text.append(ctext)
         else:
             name, changes = get_node_diff(node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang)
             node_edits.append(NodeEdit(et, 'change', c['prev']['section'], name, changes))
+    tf_moves = set()
     for m in result['move']:
         et = m['prev']['type']
         ptext = m['prev']['text']
         ctext = m['curr']['text']
+        if et == 'Text Formatting' and ptext.startswith("'"):
+            if ptext in tf_moves:  # already added 'start' of text-formatting -- don't duplicate
+                tf_moves.remove(ptext)
+                continue
+            else:
+                tf_moves.add(ptext)
         section_titles.add(m['curr']['section'])
         section_titles.add(m['prev']['section'])
         name, changes = get_node_diff(node_type=et, prev_wikitext=ptext, curr_wikitext=ctext, lang=lang)
         node_edits.append(NodeEdit(et, 'move', m['prev']['section'], name, changes))
 
     # give raw insert/remove counts
     # changes can be assumed to be overlap between insert+remove -- e.g., 5 insert and 3 remove -> 3 change, 2 insert
```

### Comparing `mwedittypes-2.0.2/mwedittypes/simple_differ.py` & `mwedittypes-2.1.0/mwedittypes/simple_differ.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import re
+
 import mwparserfromhell as mw
 
 from mwedittypes.tokenizer import parse_change_text
-from mwedittypes.utils import extract_text, find_nested_media, node_to_name, sec_to_name, simple_node_class
+from mwedittypes.utils import find_nested_media, node_to_name, sec_to_name, simple_node_class, wikitext_to_plaintext
 
 
 # equivalent of main function
 def get_diff(prev_wikitext, curr_wikitext, lang='en'):
     """Run through full process of getting diff between two wikitext revisions."""
     prev_tree = WikitextBag(wikitext=prev_wikitext, lang=lang)
     curr_tree = WikitextBag(wikitext=curr_wikitext, lang=lang)
@@ -15,85 +17,73 @@
 
 
 class Node:
     """
     Basic object for wrapping mwparserfromhell wikitext nodes
     """
 
-    def __init__(self, name, ntype='Text', text_hash=None, text='', section=None, mwnode=None):
+    def __init__(self, name, ntype='Text', mwnode=None, section=None):
         self.name = name  # For debugging purposes
         self.ntype = ntype  # Type of node for result
-        self.text = str(text)  # Text that is needed if unnesting the node
-        # Used for quickly computing equality for most nodes.
+        self.mwnode = mwnode
+        self.text = str(mwnode)  # Text that is needed if unnesting the node
+        # Content hash is used for quickly computing equality for most nodes.
         # Generally this just a simple hash of self.text (wikitext associated with a node) but
-        # the text hash for sections and paragraphs is based on all the content within the section/paragraph
-        # so it can be used for pruning while self.text is just the text that creates the section/paragraph
+        # the text hash for sections is based on all the content within the section
+        # so it can be used for pruning while self.text is just the text that creates the section
         # e.g., "==Section==\nThis is a section." would have as text "==Section==" but hash the full.
-        # so the Differ doesn't identify a section/paragraph as changing when content within it is changed
-        if text_hash is None:
-            self.text_hash = hash(self.text)
-        else:
-            self.text_hash = hash(str(text_hash))
+        # so the Differ doesn't identify a section as changing when content within it is changed
+        self.content_hash = hash(self.text)
         self.section = section  # section that the node is a part of -- useful for formatting final diff
-        # store tag name (primarily for text formatting) as context matters and
-        # re-parsing in isolation might change the node type
-        try:
-            self.tag = str(mwnode.tag)
-        except AttributeError:
-            self.tag = None
 
     def unnest(self, lang='en'):
         """Expand a node to also include all of its subnodes.
         This approach starts with a single wikitext node -- e.g., a single Tag node with nested link nodes etc.:
         <ref>{{cite web|title=[[Gallery]]|url=http://digital.belvedere.at|publisher=Digitales Belvedere}}</ref>
         and splits it into its component parts (ref, template, wikilink, externallink) to identify fine-grained changes.
         """
         nodes = []
         # Using string mixin methods such as wt.find(x) for subnodes in the for
         # loop below means doing str(wt) everytime, which is expensive because
         # it recursively converts each node to str. Better to create a string using
         # the node's text and use built-in string methods instead.
-        node_str = self.text
         if self.ntype == 'Gallery':
             # strip leading / trailing gallery tags so parser correctly parses everything in between
             # otherwise links, formatting, etc. is treated as text
             gallery_start = self.text.find('>')
             gallery_end = self.text.rfind('<')
             try:
                 # the <br> is a hack; it'll be skipped in the ifilter loop; otherwise first image skipped
-                node_str = '<br>' + self.text[gallery_start+1:gallery_end]
-                wt = mw.parse(node_str)
+                wt = mw.parse('<br>' + self.text[gallery_start+1:gallery_end], skip_style_tags=True)
             except Exception:  # fallback
-                node_str = self.text
-                wt = mw.parse(node_str)
+                wt = mw.parse(self.mwnode)
         else:
-            wt = mw.parse(node_str)
+            wt = mw.parse(self.mwnode)
         for idx, nn in enumerate(wt.ifilter(recursive=True)):
             if idx == 0:
                 continue  # skip root node -- already set
             ntype = simple_node_class(nn, lang)
             if ntype == 'Text':
                 # media w/o bracket will be IDed as text by mwparserfromhell
                 # templates / galleries are where we find this nested media
                 if self.ntype == 'Template' or self.ntype == 'Gallery':
-                    media = find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery'))
-                    for m in media:
+                    for m in find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery')):
                         nn_node = Node(f'Media: {m[:10]}...',
                                        ntype='Media',
-                                       text=m,
+                                       mwnode=m,
                                        section=self.section)
                         nodes.append(nn_node)
             # tables are very highly-structured and produce a ton of nodes (each cell and more)
             # so we just extract links, formatting, etc. that appears in the table and skip the cells
             # because changes to those will generally be caught in the overall table changes and text changes
             # this leads to much faster parsing in exchange for not knowing how many table cells were edited
             elif ntype == 'Table Element':
                 pass
             else:
-                nn_node = Node(node_to_name(nn, lang=lang), ntype=ntype, text=nn, section=self.section, mwnode=nn)
+                nn_node = Node(node_to_name(nn, lang=lang), ntype=ntype, mwnode=nn, section=self.section)
                 nodes.append(nn_node)
         return nodes
 
 
 class WikitextBag:
     """
     Structure for extracting and holding an unordered collection of wikitext nodes based on mwparserfromhell
@@ -106,36 +96,51 @@
         self.wikitext_to_bagofnodes(wikitext)
 
     def wikitext_to_bagofnodes(self, wikitext):
         """Build bag of document nodes from Wikipedia article.
         Includes special Section nodes that will cover any changes made to that section.
         Excludes text, which will be processed later (and is captured by the Section nodes).
         """
-        wt = mw.parse(wikitext)
+        wt = mw.parse(wikitext, skip_style_tags=True)
         for sidx, s in enumerate(wt.get_sections(flat=True)):
             if s:
-                sec_hash = sec_to_name(s, sidx)
-                sec_text = ''.join([str(n) for n in s.nodes])
-                self.secname_to_text[sec_hash] = sec_text
-                s_node = Node(sec_hash, ntype="Section", text=sec_text, section=sec_hash)
-                self.nodes[s_node.text_hash] = self.nodes.get(s_node.text_hash, []) + [s_node]
+                sec_id = sec_to_name(s, sidx)
+                s_node = Node(sec_id, ntype="Section", mwnode=s, section=sec_id)
+                self.secname_to_text[sec_id] = s_node.text
+                self.nodes[s_node.content_hash] = self.nodes.get(s_node.content_hash, []) + [s_node]
                 for n in s.nodes:  # this is just top-level of nodes so e.g., table but not all the table rows etc.
                     ntype = simple_node_class(n, self.lang)
                     if ntype != 'Text':
-                        n_node = Node(node_to_name(n, self.lang), ntype=ntype, text=n, section=s_node.name, mwnode=n)
-                        self.nodes[n_node.text_hash] = self.nodes.get(n_node.text_hash, []) + [n_node]
+                        n_node = Node(node_to_name(n, self.lang), ntype=ntype, mwnode=n, section=s_node.name)
+                        self.nodes[n_node.content_hash] = self.nodes.get(n_node.content_hash, []) + [n_node]
+                if "''" in s_node.text:
+                    for line in s_node.text.split('\n'):
+                        if "''" in line:
+                            line, bt_found = re.subn("'{5}", "", line)
+                            for _ in range(bt_found // 2):
+                                tfn = Node("Bold-Italic", ntype='Text Formatting', mwnode="'''''",
+                                           section=s_node.name)
+                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
+                            line, b_found = re.subn("'{3}", "", line)
+                            for _ in range(b_found // 2):
+                                tfn = Node("Bold", ntype='Text Formatting', mwnode="'''", section=s_node.name)
+                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
+                            line, t_found = re.subn("'{2}", "", line)
+                            for _ in range(t_found // 2):
+                                tfn = Node("Italic", ntype='Text Formatting', mwnode="''", section=s_node.name)
+                                self.nodes[tfn.content_hash] = self.nodes.get(tfn.content_hash, []) + [tfn]
 
     def expand_nested(self):
         """Expand nested nodes in tree -- e.g., Ref tags with templates/links contained in them."""
         to_add = {}
         for n_hash in self.nodes:
             for n in self.nodes[n_hash]:
                 if n.ntype not in ('Section', 'Heading', 'Text'):  # leaves tag, link, etc.
                     for nn in n.unnest(self.lang):
-                        to_add[nn.text_hash] = to_add.get(nn.text_hash, []) + [nn]
+                        to_add[nn.content_hash] = to_add.get(nn.content_hash, []) + [nn]
 
         for n_hash in to_add:
             for n in to_add[n_hash]:
                 self.nodes[n_hash] = self.nodes.get(n_hash, []) + [n]
 
 
 class Differ:
@@ -210,18 +215,19 @@
             if chg > 0:
                 edit_types[n_type]['change'] = chg
             if rem > 0:
                 edit_types[n_type]['remove'] = rem
             if ins > 0:
                 edit_types[n_type]['insert'] = ins
 
+        lang = self.t1.lang
         prev_text = ''
         for s in prev_text_sections:
-            prev_text += ''.join([extract_text(n, self.t1.lang) for n in mw.parse(self.t1.secname_to_text[s]).nodes])
+            prev_text += wikitext_to_plaintext(self.t1.secname_to_text[s], lang=lang)
         curr_text = ''
         for s in curr_text_sections:
-            curr_text += ''.join([extract_text(n, self.t2.lang) for n in mw.parse(self.t2.secname_to_text[s]).nodes])
+            curr_text += wikitext_to_plaintext(self.t2.secname_to_text[s], lang=lang)
 
-        text_changes = parse_change_text(prev_text, curr_text, self.t1.lang)
+        text_changes = parse_change_text(prev_text, curr_text, lang=lang)
         edit_types.update(text_changes)
 
         return edit_types
```

### Comparing `mwedittypes-2.0.2/mwedittypes/tokenizer.py` & `mwedittypes-2.1.0/mwedittypes/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mwedittypes-2.0.2/mwedittypes/tree_differ.py` & `mwedittypes-2.1.0/mwedittypes/tree_differ.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from anytree import PostOrderIter, NodeMixin
 from anytree.util import leftsibling
 import mwparserfromhell as mw
 
-from mwedittypes.utils import find_nested_media, node_to_name, sec_to_name, simple_node_class, wikitext_to_plaintext
+from mwedittypes.utils import (find_nested_media, find_nested_textformatting, node_to_name, sec_to_name,
+                               simple_node_class, wikitext_to_plaintext)
 
 
 # equivalent of main function
-def get_diff(prev_wikitext, curr_wikitext, lang='en', timeout=False, debug=False):
+def get_diff(prev_wikitext, curr_wikitext, lang='en', timeout=False):
     """Run through full process of getting tree diff between two wikitext revisions."""
     # To provide proper structure, need all content to be nested under a section
     prev_tree = WikitextTree(wikitext=prev_wikitext, lang=lang)
     curr_tree = WikitextTree(wikitext=curr_wikitext, lang=lang)
     d = Differ(prev_tree, curr_tree, timeout=timeout)
-    diff = d.get_corresponding_nodes(debug=debug)
+    diff = d.get_corresponding_nodes()
     result = diff.post_process(prev_tree.secname_to_text, curr_tree.secname_to_text, lang=lang)
     # this helps the node differ know that the lede is also a new section
     # otherwise depends on headings to track changes to sections
     if not prev_wikitext:
         result['prev-no-content'] = True
     if not curr_wikitext:
         result['curr-no-content'] = True
@@ -24,173 +25,171 @@
 
 
 class OrderedNode(NodeMixin):
     """
     Extension of anytree library node to support tree differ.
     """
 
-    def __init__(self, name, ntype='Text', text_hash=None, idx=-1, text='', char_offset=-1, section=None,
+    def __init__(self, name, ntype='Text', idx=-1, mwnode=None, section=None,
                  parent=None, children=None):
         super(OrderedNode, self).__init__()
         self.name = name  # For debugging purposes
         self.ntype = ntype  # Different node types can be treated differently when computing equality
-        self.text = str(text)  # Text that can then be passed to a diffing library
+        self.mwnode = mwnode
+        self.text = str(mwnode) if mwnode is not None else ''  # Text that can then be passed to a diffing library
         # Used for quickly computing equality for most nodes.
-        # Generally this just a simple hash of self.text (wikitext associated with a node) but
-        # the text hash for sections and paragraphs is based on all the content within the section/paragraph
-        # so it can be used for pruning while self.text is just the text that creates the section/paragraph
+        # Generally this just a simple hash of self.mwnode (wikitext associated with a node) but
+        # the text hash for sections is based on all the content within the section
+        # so it can be used for pruning while self.text is just the text that creates the section
         # e.g., "==Section==\nThis is a section." would have as text "==Section==" but hash the full.
-        # so the Differ doesn't identify a section/paragraph as changing when content within it is changed
-        if text_hash is None:
-            self.text_hash = hash(self.text)
-        else:
-            self.text_hash = hash(str(text_hash))
+        # so the Differ doesn't identify a section as changing when content within it is changed
+        self.content_hash = hash(self.text)
         self.idx = idx  # Used by Differ -- Post order on tree from 0...# nodes - 1
-        self.char_offset = char_offset  # make it easy to find node in section text
         self.section = section  # section that the node is a part of -- useful for formatting final diff
         self.parent = parent
         if children:
             self.children = children
+        self.leftmostidx = None
 
     def leftmost(self):
-        return self.idx if self.is_leaf else self.children[0].leftmost()
+        if self.leftmostidx is None:
+            self.leftmostidx = self.idx if self.is_leaf else self.children[0].leftmost()
+        return self.leftmostidx
 
     def unnest(self, lang='en'):
         """Build tree of document nodes by recursing within a single wikitext node.
 
         This approach starts with a single wikitext node -- e.g., a single Tag node with nested link nodes etc.:
         <ref>{{cite web|title=[[Gallery]]|url=http://digital.belvedere.at|publisher=Digitales Belvedere}}</ref>
         and splits it into its component pieces to then identify what has changed between revisions.
 
         Example above would take a Reference node as input and build the following tree (in-place):
         <--rest-of-tree-- Reference <--child-of-- Template (cite web) <--child-of-- WikiLink (Gallery)
                                                                 ^--------child-of-- External Link (http://digital...)
         """
         if self.ntype == 'Gallery':
             # strip leading / trailing gallery tags so parser correctly parses everything in between
-            # otherwise links, formatting, etc. is treated as text
+            # otherwise links, templates, etc. is treated as text
             gallery_start = self.text.find('>')
             gallery_end = self.text.rfind('<')
             try:
                 # the break is a hack; it'll be skipped in the ifilter loop; otherwise first image skipped
-                wt = mw.parse('<br>' + self.text[gallery_start+1:gallery_end])
+                wt = mw.parse('<br>' + self.text[gallery_start+1:gallery_end], skip_style_tags=True)
             except Exception:  # fallback
-                wt = mw.parse(self.text)
+                wt = mw.parse(self.mwnode)  # automatically carries over skip_style_tags
         else:
-            wt = mw.parse(self.text)
-        parent_node = self
-        base_offset = self.char_offset
+            wt = mw.parse(self.mwnode)  # automatically carries over skip_style_tags
         parent_ranges = [(0, len(self.text), self)]  # (start idx of node, end idx of node, node object)
         for idx, nn in enumerate(wt.ifilter(recursive=True)):
             if idx == 0:
                 continue  # skip root node -- already set or placeholder <br> node for galleries
             ntype = simple_node_class(nn, lang)
             if ntype == 'Text':
                 # media w/o bracket will be IDed as text by mwparserfromhell
                 # templates / galleries are where we find this nested media
+                # any discovered media will just be the start and aren't guaranteed to be the whole image + caption etc.
                 if self.ntype == 'Template' or self.ntype == 'Gallery':
-                    media = find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery'))
-                    for m in media:
+                    for m in find_nested_media(str(nn), is_gallery=(self.ntype == 'Gallery')):
                         nn_node = OrderedNode(f'Media: {m[:10]}...',
                                               ntype='Media',
-                                              text=m,
-                                              char_offset=base_offset + self.text.find(str(m), parent_ranges[0][0]),
+                                              mwnode=m,
                                               section=self.section,
                                               parent=self)
+                        offset = self.text.find(str(m), parent_ranges[0][0])
+                        parent_ranges.insert(0, (offset, offset + len(m), nn_node))
             # tables are very highly-structured and produce a ton of nodes (each cell and more)
             # so we just extract links, formatting, etc. that appears in the table and skip the cells
             # because changes to those will generally be caught in the overall table changes and text changes
             # this leads to much faster parsing in exchange for not knowing how many table cells were edited
             elif ntype == 'Table Element':
                 pass
             else:
                 # start looking from the start of the latest node
                 node_start = self.text.find(str(nn), parent_ranges[0][0])
                 # identify direct parent of node
-                for parent in parent_ranges:
-                    if node_start < parent[1]:  # falls within parent range
-                        parent_node = parent[2]
+                for parent_start, parent_end, parent_node in parent_ranges:
+                    if node_start < parent_end:  # starts before end of a previous node; already know it begins after it
+                        nn_node = OrderedNode(node_to_name(nn, lang=lang), ntype=ntype, mwnode=nn,
+                                              section=self.section, parent=parent_node)
+                        parent_ranges.insert(0, (node_start, node_start + len(nn), nn_node))
+                        break
+        if "''" in self.text:
+            for tfnode, tfspan in find_nested_textformatting(self.text):
+                for parent_start, parent_end, parent_node in parent_ranges:
+                    if tfspan[0] >= parent_start and tfspan[1] <= parent_end:
+                        nn_node = OrderedNode(f'Text-Formatting: {tfnode}',
+                                              ntype='Text Formatting',
+                                              mwnode=tfnode,
+                                              section=self.section,
+                                              parent=parent_node)
                         break
-                nn_node = OrderedNode(node_to_name(nn, lang=lang), ntype=ntype, text=nn,
-                                      char_offset=base_offset + node_start,
-                                      section=self.section, parent=parent_node)
-                parent_ranges.insert(0, (node_start, node_start + len(nn), nn_node))
-
-    def dump(self, debug=False):
-        result = {'type': self.ntype,
-                  'text': self.text,
-                  'section': self.section}
-        if debug:
-            result['name'] = self.name
-            result['offset'] = self.char_offset
-        return result
 
+    def dump(self):
+        return {'type': self.ntype,
+                'text': self.text,
+                'section': self.section}
 
 class WikitextTree:
     """
     Tree structure for wikitext based on mwparserfromhell
     """
 
     def __init__(self, wikitext, lang="en"):
         self.lang = lang
         self.root = OrderedNode('root', ntype="Article")
         self.secname_to_text = {}
         self.wikitext_to_tree(wikitext)
+        self.key_roots = None
 
     def wikitext_to_tree(self, wikitext):
         """Build tree of document nodes from Wikipedia article.
 
         This approach builds a tree with an artificial 'root' node on the 1st level,
         all of the article sections nested flatly underneath (including the Lede section),
         and all of the text, link, template, etc. nodes nested under their respective sections.
         """
-        wt = mw.parse(wikitext)
+        wt = mw.parse(wikitext, skip_style_tags=True)
         for sidx, s in enumerate(wt.get_sections(flat=True)):
-            if s:
-                sec_hash = sec_to_name(s, sidx)
-                sec_text = ''.join([str(n) for n in s.nodes])
-                self.secname_to_text[sec_hash] = sec_text
-                s_node = OrderedNode(sec_hash, ntype="Section", text=s.nodes[0], text_hash=sec_text, char_offset=0,
-                                     section=sec_hash, parent=self.root)
-                char_offset = 0
-                for n in s.nodes:
-                    n_node = OrderedNode(node_to_name(n, self.lang), ntype=simple_node_class(n, self.lang), text=n,
-                                         char_offset=char_offset, section=s_node.name, parent=s_node)
-                    char_offset += len(str(n))
-            # empty lede
-            else:
-                sec_hash = sec_to_name(s, sidx)
-                sec_text = ''
-                self.secname_to_text[sec_hash] = sec_text
-                s_node = OrderedNode(sec_hash, ntype="Section", text=sec_text, text_hash=sec_text, char_offset=0,
-                                     section=sec_hash, parent=self.root)
+            sec_id = sec_to_name(s, sidx)
+            sec_text = ''.join([str(n) for n in s.nodes])
+            self.secname_to_text[sec_id] = sec_text
+            s_node = OrderedNode(sec_id, ntype="Section", mwnode=s, section=sec_id, parent=self.root)
+            for n in s.nodes:
+                n_node = OrderedNode(node_to_name(n, self.lang), ntype=simple_node_class(n, self.lang), mwnode=n,
+                                     section=s_node.name, parent=s_node)
 
     def expand_nested(self):
         """Expand nested nodes in tree -- e.g., Ref tags with templates/links contained in them."""
         for n in PostOrderIter(self.root):
-            if n.ntype not in ('Article', 'Section', 'Heading', 'Text'):  # leaves tag, link, etc.
+            if n.ntype not in ('Article', 'Section'):
                 n.unnest(self.lang)
 
 
 class Differ:
     """
     Find structural differences between two WikitextTrees
     """
 
     def __init__(self, t1, t2, timeout=False, expand_nodes=True):
         self.timeout = timeout  # if True, limit size of trees compared
         self.prune_trees(t1, t2, expand_nodes)
         self.t1 = []
+        self.t1_keyroots = []
         self.t2 = []
+        self.t2_keyroots = []
         for i, n in enumerate(PostOrderIter(t1.root)):
             n.idx = i
             self.t1.append(n)
+            if n.is_root or leftsibling(n) is not None:
+                self.t1_keyroots.append(n)
         for i, n in enumerate(PostOrderIter(t2.root)):
             n.idx = i
             self.t2.append(n)
+            if n.is_root or leftsibling(n) is not None:
+                self.t2_keyroots.append(n)
         self.ins_cost = 1
         self.rem_cost = 1
         self.chg_cost = 1
         self.nodetype_chg_cost = 10  # arbitrarily high to encourage remove+insert when node types change
 
         # Permanent store of transactions such that transactions[x][y] is the minimum
         # transactions to get from the sub-tree rooted at node x (in tree1) to the sub-tree
@@ -228,16 +227,16 @@
         """Quick heuristic preprocessing to reduce tree differ time by removing matching sections."""
         self.prune_sections(t1, t2)
         # arbitrary: more than 500 nodes altogether even after pruning and before unnesting -- just diff sections
         if self.timeout and (sum(1 for n in PostOrderIter(t1.root)) + sum(1 for n in PostOrderIter(t2.root))) > 500:
             self.prune_to_sections(t1, t2)
         # arbitrary: seems like manageable number of total nodes -- unnest fully before diffing
         elif expand_nodes and (not self.timeout or
-                               (sum([len(mw.parse(n.text).filter()) for n in PostOrderIter(t1.root)]) +
-                               sum([len(mw.parse(n.text).filter()) for n in PostOrderIter(t2.root)])) < 1000):
+                               (sum([len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t1.root)]) +
+                               sum([len(mw.parse(n.mwnode).filter()) for n in PostOrderIter(t2.root)])) < 1000):
             t1.expand_nested()
             t2.expand_nested()
 
     def prune_to_sections(self, t1, t2):
         """Remove all non-section nodes."""
         for n in PostOrderIter(t1.root):
             if n.ntype == 'Section':
@@ -249,37 +248,31 @@
     def prune_sections(self, t1, t2):
         """Prune nodes from any sections that align across revisions"""
         t1_sections = [n for n in PostOrderIter(t1.root) if n.ntype == "Section"]
         t2_sections = [n for n in PostOrderIter(t2.root) if n.ntype == "Section"]
         for secnode1 in t1_sections:
             for sn2_idx in range(len(t2_sections)):
                 secnode2 = t2_sections[sn2_idx]
-                if secnode1.text_hash == secnode2.text_hash:
+                if secnode1.content_hash == secnode2.content_hash:
                     # assumes sections aren't hierarchical in tree
-                    # or if they are, the text_hash must also include nested sections
+                    # or if they are, the content_hash must also include nested sections
                     secnode1.children = []
                     secnode2.children = []
                     t2_sections.pop(sn2_idx)  # only match once
                     break
 
-    def get_key_roots(self, tree):
-        """Get keyroots (node has a left sibling or is the root) of a tree"""
-        for on in tree:
-            if on.is_root or leftsibling(on) is not None:
-                yield on
-
     def populate_transactions(self, transactions):
         """Populate self.transactions with minimum transactions between all possible trees"""
-        for kr1 in self.get_key_roots(self.t1):
+        for kr1 in self.t1_keyroots:
             # Make transactions for tree -> null
             i_nulls = []
             for ii in range(kr1.leftmost(), kr1.idx + 1):
                 i_nulls.append(self.transaction_to_idx[ii][None])
                 transactions[ii][None] = i_nulls.copy()
-            for kr2 in self.get_key_roots(self.t2):
+            for kr2 in self.t2_keyroots:
                 # Make transactions of null -> tree
                 j_nulls = []
                 for jj in range(kr2.leftmost(), kr2.idx + 1):
                     j_nulls.append(self.transaction_to_idx[None][jj])
                     transactions[None][jj] = j_nulls.copy()
 
                 # get the diff
@@ -304,15 +297,15 @@
             return self.ins_cost
         elif n2 is None:
             return self.rem_cost
         # Inserts/Removes are easy. Changes are more complicated and should only be within same node type.
         # Use arbitrarily high-value for nodetype changes to effectively ban.
         elif n1.ntype != n2.ntype:
             return self.nodetype_chg_cost
-        elif n1.text_hash == n2.text_hash:
+        elif n1.content_hash == n2.content_hash:
             return 0
         # if both sections, assert no cost (changes will be captured by headings)
         # except we want to detect moves of sections
         elif n1.ntype == 'Section':
             if not n1.children and not n2.children:
                 return self.chg_cost
             return 0
@@ -401,15 +394,15 @@
                         transactions[i][j] = ic
                     else:
                         # record a change
                         cc = chg.copy()
                         cc.extend(self.transactions[i][j])
                         transactions[i][j] = cc
 
-    def get_corresponding_nodes(self, debug=False):
+    def get_corresponding_nodes(self):
         """Explain transactions.
 
         Skip 'Section' operations as they aren't real nodes and
         any changes to them will be captured via Headings etc.
         """
         if self.transactions:
             transactions = self.transactions[len(self.t1) - 1][len(self.t2) - 1]
@@ -430,16 +423,15 @@
                     prev_node = self.t1[transactions[i][0]]
                     curr_node = self.t2[transactions[i][1]]
                     if prev_node.ntype != 'Section' or not prev_node.children:
                         change.append((prev_node, curr_node))
             diff = {'remove': remove, 'insert': insert, 'change': change}
             self.detect_moves(diff)
             return Diff(nodes_removed=diff['remove'], nodes_inserted=diff['insert'],
-                        nodes_changed=diff['change'], nodes_moved=diff['move'],
-                        debug=debug)
+                        nodes_changed=diff['change'], nodes_moved=diff['move'])
         else:
             return Diff(nodes_removed=[], nodes_inserted=[],
                         nodes_changed=[], nodes_moved=[])
 
     def detect_moves(self, diff):
         """Detect when nodes were moved (as opposed to removed/inserted/changed) and update diff.
 
@@ -455,15 +447,15 @@
           Input: Change(A,B) and Insert(A) -> Move(A,A) and Insert(B)
           Input: Change(A,B) and Remove(B) -> Remove(A) and Move(B,B)
           Input: Change(A,B) and Change(C,A) -> Move(A,A) and Insert(B) and Remove(C)
           Input: Change(A,B) and Change(B,A) -> Move(A,A) and Move(B,B)
         """
 
         # build list of all prev and curr nodes to compare for matches
-        ntypes_to_ignore = ('Text', 'Text Formatting')
+        ntypes_to_ignore = ('Text', 'Text Formatting', 'List')
         prev_nodes = [('remove', i, pn) for i, pn in enumerate(diff['remove']) if pn.ntype not in ntypes_to_ignore]
         curr_nodes = [('insert', j, cn) for j, cn in enumerate(diff['insert']) if cn.ntype not in ntypes_to_ignore]
         for k in range(len(diff['change'])):
             if diff['change'][k][0].ntype not in ntypes_to_ignore:
                 prev_nodes.append(('change', k, diff['change'][k][0]))
                 curr_nodes.append(('change', k, diff['change'][k][1]))
 
@@ -475,15 +467,15 @@
         curr_found = set()
         change_to_insert = {}
         change_to_remove = {}
         for pet, pidx, pn in prev_nodes:
             for cet, cidx, cn in curr_nodes:
                 cid = f'{cet}-{cidx}'
                 # same type/text and not already part of a move
-                if pn.ntype == cn.ntype and pn.text_hash == cn.text_hash and cid not in curr_found:
+                if pn.ntype == cn.ntype and pn.content_hash == cn.content_hash and cid not in curr_found:
                     prev_moved.append((pet, pidx))
                     curr_moved.append((cet, cidx))
                     curr_found.add(cid)
                     if pet == 'change':
                         corresponding_changed_node = diff['change'][pidx][1]
                         change_to_insert[pidx] = corresponding_changed_node
                     if cet == 'change':
@@ -518,23 +510,22 @@
 
 
 class Diff:
     """
     Diff result with helper functions for post-processing / cleaning up the result
     """
 
-    def __init__(self, nodes_removed, nodes_inserted, nodes_changed, nodes_moved, debug=False):
-        self.remove = [n.dump(debug) for n in nodes_removed]
-        self.insert = [n.dump(debug) for n in nodes_inserted]
-        self.change = [{'prev': pn.dump(debug), 'curr': cn.dump(debug)} for pn, cn in nodes_changed]
-        self.move = [{'prev': pn.dump(debug), 'curr': cn.dump(debug)} for pn, cn in nodes_moved]
+    def __init__(self, nodes_removed, nodes_inserted, nodes_changed, nodes_moved):
+        self.remove = [n.dump() for n in nodes_removed]
+        self.insert = [n.dump() for n in nodes_inserted]
+        self.change = [{'prev': pn.dump(), 'curr': cn.dump()} for pn, cn in nodes_changed]
+        self.move = [{'prev': pn.dump(), 'curr': cn.dump()} for pn, cn in nodes_moved]
         self.sections_p_to_c = {}
         self.sections_c_to_p = {}
         self.processed = False
-        self.debug = debug
 
     def post_process(self, sections_prev, sections_curr, lang):
         if not self.processed:
             self._section_mapping(sections_prev, sections_curr)
             self._merge_text_changes(sections_prev, sections_curr, lang)
             self._build_result(sections_prev, sections_curr)
             self.processed = True
@@ -560,17 +551,14 @@
             csec_name = cn['section']
             # update name to section in previous revision for consistency (if it exists)
             csec_id = self.sections_c_to_p[csec_name] or csec_name
             cn['section'] = csec_id
             sc[csec_id] = sections_curr[csec_name]
 
         self.result = {'remove': self.remove, 'insert': self.insert, 'change': self.change, 'move': self.move}
-        if self.debug:
-            self.result['sections-prev'] = sp
-            self.result['sections-curr'] = sc
 
     def _section_mapping(self, sections_prev, sections_curr):
         """Build mapping of sections between previous and current versions of article."""
         prev = list(sections_prev.keys())
         curr = list(sections_curr.keys())
         p_to_c = {}
         c_to_p = {}
```

### Comparing `mwedittypes-2.0.2/mwedittypes/utils.py` & `mwedittypes-2.1.0/mwedittypes/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # helper functions for handling mwparserfromhell / wikitext
-from mwconstants.constants.c_media import DEF_OPTION_TAGS, IMG_OPTION_ALIASES
+import re
+
 import mwparserfromhell as mw
 
 from mwedittypes.constants import *
 
 
 def simple_node_class(mwnode, lang='en'):
     """e.g., "<class 'mwparserfromhell.nodes.heading.Heading'>" -> "Heading"."""
@@ -57,16 +58,21 @@
     if len(n_txt) > 13:
         return f'{simple_node_class(mwnode, lang)}: {n_txt[:10]}...'
     else:
         return f'{simple_node_class(mwnode, lang)}: {n_txt}'
 
 
 def wikitext_to_plaintext(wt, lang='en'):
-    """Helper function for converting wikitext to plaintext."""
-    return ''.join([extract_text(n, lang) for n in mw.parse(wt).nodes])
+    """Helper function for converting wikitext to plaintext.
+
+    Removes text-formatting syntax (italic '', bold ''', bold-italic ''''') from nodes because
+    skip_style_tags is set to True and so these syntax are treated as text by mwparserfromhell.
+    This is to avoid parsing issues that arise from unclosed text-formatting syntax.
+    """
+    return ''.join([re.sub("'{2,}", "", extract_text(n, lang)) for n in mw.parse(wt, skip_style_tags=True).nodes])
 
 
 def extract_text(mwnode, lang='en'):
     """Extract what text would be displayed from any node."""
     ntype = simple_node_class(mwnode, lang)
     if ntype == 'Text':
         return str(mwnode)
@@ -101,15 +107,14 @@
     is to extract the filename and detect when that has been edited.
 
     In galleries, each image is given its own line and formatting/caption options are evaluated just like
     they are for standard bracketed media links. Gallery images do not need a File: etc. prefix however.
     So for galleries, we also extract everything between filename and end-of-line as the media options.
     """
     lc_wt = wikitext.lower()
-    media = []
     end = 0
     while True:
         m = EXTEN_PATTERN.search(lc_wt, pos=end)
         if m is None:
             break
         start, end = m.span()
         if end - start <= max_link_length:
@@ -117,56 +122,33 @@
             if is_gallery:
                 end_of_line = wikitext.find('\n', end)
                 if end_of_line == -1:  # no new-line at end of gallery
                     media_options = wikitext[end:]
                 else:
                     media_options = wikitext[end:end_of_line]
                 media_wikitext += media_options
-            media.append(media_wikitext.strip())
-    return media
+            yield(media_wikitext.strip())
 
 
-def parse_image_options(img_options_wikitext, lang='en'):
-    """Identify any formatting options and caption within media file syntax.
+def find_nested_textformatting(wikitext):
+    """Context-insensitive search for likely text-formatting in wikitext.
 
-    There are a set of allowed keywords/parameters for media formatting that we have fully compiled a list of.
-    Each parameter in a media file is checked against these formatting options and if it does not match,
-    it is assumed to be the caption.
-
-    For more info, see: https://www.mediawiki.org/wiki/Help:Images#Syntax
+    Specifically, there are three viable options:
+    ''italics'' (2 '), '''bold''' (3 '), and '''''bold-italic''''' (5 ')
+    The only rule is that this text-formatting cannot be broken up by a new-line
+    but it can span nodes so a valid chunk of wikitext might only have the start
+    or end of the text-formatting. For this reason, we look for sequences of
+    text-formatting that are 2, 3, or 5 ' and treat them as text-formatting regardless
+    of whether they are the start or end of a block (which is not knowable). The number
+    of final text-formatting nodes across an entire article then has to be divided by
+    two to reach a more accurate count of how many text-formatting blocks there are.
     """
-    options = []
-    caption = None
-    if img_options_wikitext:
-        lang_tags = {}
-        for k in DEF_OPTION_TAGS:
-            lang_tags[k] = DEF_OPTION_TAGS[k] + IMG_OPTION_ALIASES.get(lang, {}).get(k, [])
-        for o in img_options_wikitext.split('|'):
-            o = o.strip()
-            if o in lang_tags['keywords']:
-                options.append(o)
-            elif o.split('=')[0] in lang_tags['params']:
-                options.append(o)
-            else:
-                found = False
-                for t in lang_tags['startswith']:
-                    if o.startswith(t):
-                        options.append(o)
-                        found = True
-                        break
-                if not found:
-                    for t in lang_tags['endswith']:
-                        if o.endswith(t):
-                            options.append(o)
-                            found = True
-                            break
-                if not found:
-                    caption = o
-
-    return options, caption
+    if "''" in wikitext:
+        for tf in re.finditer("'{2,5}", wikitext):
+            yield(tf.group(), tf.span())
 
 
 def full_diff_to_simple(full_diff):
     """Extract simple edit type summary from full edit type response."""
     result = {}
     for ne in full_diff['node-edits']:
         if ne.type not in result:
```

### Comparing `mwedittypes-2.0.2/mwedittypes.egg-info/PKG-INFO` & `mwedittypes-2.1.0/mwedittypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwedittypes
-Version: 2.0.2
+Version: 2.1.0
 Summary: Edit diffs and type detection for Wikipedia
 Home-page: https://github.com/geohci/edit-types
 Author: geohci & Amamgbu (Isaac Johnson & Jesse Amamgbu)
 Author-email: <amamgbujesse@yahoo.com>
 License: MIT License
 Keywords: python,wikipedia,edit types,edit diffs,wiki,edit detection
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mwedittypes-2.0.2/setup.py` & `mwedittypes-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.0.2'
+VERSION = '2.1.0'
 DESCRIPTION = 'Edit diffs and type detection for Wikipedia'
 LONG_DESCRIPTION = 'A package that allows edit diffs and type detection for Wikipedia.'
 
 # Dev dependencies
 EXTRAS_REQUIRE = {
     "tests": ["pytest>=6.2.5"],
 }
```

