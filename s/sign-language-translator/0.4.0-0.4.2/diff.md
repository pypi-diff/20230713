# Comparing `tmp/sign_language_translator-0.4.0.tar.gz` & `tmp/sign_language_translator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sign_language_translator-0.4.0.tar", max compression
+gzip compressed data, was "sign_language_translator-0.4.2.tar", max compression
```

## Comparing `sign_language_translator-0.4.0.tar` & `sign_language_translator-0.4.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12461 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/README.md
--rw-r--r--   0        0        0     1083 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2565 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/config/__init__.py
--rw-r--r--   0        0        0     1132 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/config/enums.py
--rw-r--r--   0        0        0      616 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/config/helpers.py
--rw-r--r--   0        0        0      329 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/config/settings.py
--rw-r--r--   0        0        0        0 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/data_collection/__init__.py
--rwxr-xr-x   0        0        0    10252 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/data_collection/completeness.py
--rwxr-xr-x   0        0        0     7713 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/data_collection/scraping.py
--rwxr-xr-x   0        0        0     2107 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/data_collection/synonyms.py
--rw-r--r--   0        0        0      168 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/__init__.py
--rw-r--r--   0        0        0      642 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/sign/__init__.py
--rw-r--r--   0        0        0     4982 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/sign/mapping_rules.py
--rw-r--r--   0        0        0     7759 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/sign/pakistan_sign_language.py
--rw-r--r--   0        0        0     3773 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/sign/sign_language.py
--rw-r--r--   0        0        0      355 2023-07-11 14:47:19.697829 sign_language_translator-0.4.0/sign_language_translator/languages/text/__init__.py
--rw-r--r--   0        0        0       80 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/languages/text/english.py
--rw-r--r--   0        0        0     1070 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/languages/text/text_language.py
--rw-r--r--   0        0        0    12816 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/languages/text/urdu.py
--rw-r--r--   0        0        0     2453 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/languages/utils.py
--rw-r--r--   0        0        0    11710 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/languages/vocab.py
--rw-r--r--   0        0        0      353 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/__init__.py
--rwxr-xr-x   0        0        0     1171 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/abstract_language_model.py
--rwxr-xr-x   0        0        0     3277 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/beam_sampling.py
--rwxr-xr-x   0        0        0     2785 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/mixer.py
--rwxr-xr-x   0        0        0     9002 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/simple_language_model.py
--rwxr-xr-x   0        0        0       74 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/language_models/transformer_language_model.py
--rw-r--r--   0        0        0        0 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/sign_to_text/__init__.py
--rw-r--r--   0        0        0      158 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/text_to_sign/__init__.py
--rw-r--r--   0        0        0     3237 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
--rw-r--r--   0        0        0      536 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/text_to_sign/t2s_model.py
--rw-r--r--   0        0        0     1100 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/models/utils.py
--rw-r--r--   0        0        0      446 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/__init__.py
--rwxr-xr-x   0        0        0     3320 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/metrics.py
--rwxr-xr-x   0        0        0      882 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/preprocess.py
--rwxr-xr-x   0        0        0     1333 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/subtitles.py
--rw-r--r--   0        0        0     4194 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/tagger.py
--rw-r--r--   0        0        0     4800 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/tokenizer.py
--rwxr-xr-x   0        0        0     9223 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/text/utils.py
--rwxr-xr-x   0        0        0       43 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/utils/__init__.py
--rwxr-xr-x   0        0        0     3675 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/utils/data_loader.py
--rwxr-xr-x   0        0        0    13542 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/utils/landmarks_info.py
--rwxr-xr-x   0        0        0    10351 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/utils/sign_data_attributes.py
--rwxr-xr-x   0        0        0     2822 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/utils/tree.py
--rw-r--r--   0        0        0        0 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/vision/__init__.py
--rwxr-xr-x   0        0        0    18024 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/vision/concatenate.py
--rwxr-xr-x   0        0        0     7980 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/vision/embed.py
--rwxr-xr-x   0        0        0    33628 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/vision/transforms.py
--rwxr-xr-x   0        0        0    30236 2023-07-11 14:47:19.701829 sign_language_translator-0.4.0/sign_language_translator/vision/visualization.py
--rw-r--r--   0        0        0    13897 1970-01-01 00:00:00.000000 sign_language_translator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    12937 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/README.md
+-rw-r--r--   0        0        0     1083 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2565 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/config/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-13 11:14:41.823696 sign_language_translator-0.4.2/sign_language_translator/config/enums.py
+-rw-r--r--   0        0        0      616 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/config/helpers.py
+-rw-r--r--   0        0        0      329 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/config/settings.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/__init__.py
+-rwxr-xr-x   0        0        0    10252 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/completeness.py
+-rwxr-xr-x   0        0        0     7713 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/scraping.py
+-rwxr-xr-x   0        0        0     2107 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/data_collection/synonyms.py
+-rw-r--r--   0        0        0      250 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/mapping_rules.py
+-rw-r--r--   0        0        0     7759 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/pakistan_sign_language.py
+-rw-r--r--   0        0        0     3773 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/sign/sign_language.py
+-rw-r--r--   0        0        0      355 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/english.py
+-rw-r--r--   0        0        0     1070 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/text_language.py
+-rw-r--r--   0        0        0    12816 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/text/urdu.py
+-rw-r--r--   0        0        0     2453 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/utils.py
+-rw-r--r--   0        0        0    11710 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/languages/vocab.py
+-rw-r--r--   0        0        0      573 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/__init__.py
+-rwxr-xr-x   0        0        0     1171 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/abstract_language_model.py
+-rwxr-xr-x   0        0        0     3277 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/beam_sampling.py
+-rwxr-xr-x   0        0        0     2785 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/mixer.py
+-rwxr-xr-x   0        0        0     9002 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/simple_language_model.py
+-rwxr-xr-x   0        0        0       74 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/language_models/transformer_language_model.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/sign_to_text/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/__init__.py
+-rw-r--r--   0        0        0     3237 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/concatenative_synthesis.py
+-rw-r--r--   0        0        0      536 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/t2s_model.py
+-rw-r--r--   0        0        0     1100 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/models/utils.py
+-rw-r--r--   0        0        0      446 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/__init__.py
+-rwxr-xr-x   0        0        0     3320 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/metrics.py
+-rwxr-xr-x   0        0        0      882 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/preprocess.py
+-rwxr-xr-x   0        0        0     1333 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/subtitles.py
+-rw-r--r--   0        0        0     4194 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/tagger.py
+-rw-r--r--   0        0        0     4800 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/tokenizer.py
+-rwxr-xr-x   0        0        0     9223 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/text/utils.py
+-rwxr-xr-x   0        0        0       43 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3675 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/data_loader.py
+-rwxr-xr-x   0        0        0    13542 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/landmarks_info.py
+-rwxr-xr-x   0        0        0    10351 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/sign_data_attributes.py
+-rwxr-xr-x   0        0        0     2822 2023-07-13 11:14:41.827696 sign_language_translator-0.4.2/sign_language_translator/utils/tree.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/__init__.py
+-rwxr-xr-x   0        0        0    18024 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/concatenate.py
+-rwxr-xr-x   0        0        0     7980 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/embed.py
+-rwxr-xr-x   0        0        0    33628 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/transforms.py
+-rwxr-xr-x   0        0        0    30236 2023-07-13 11:14:41.831696 sign_language_translator-0.4.2/sign_language_translator/vision/visualization.py
+-rw-r--r--   0        0        0    14366 1970-01-01 00:00:00.000000 sign_language_translator-0.4.2/PKG-INFO
```

### Comparing `sign_language_translator-0.4.0/README.md` & `sign_language_translator-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Sign Language Translator ⠎⠇⠞
 
-[![python](https://img.shields.io/pypi/pyversions/sign-language-tranlator)](https://pypi.org/project/sign-language-tranlator/)
-
-[![PyPi](https://img.shields.io/pypi/v/sign-language-tranlator)](https://pypi.org/project/sign-language-tranlator/)
-
+[![python](https://img.shields.io/pypi/pyversions/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
+[![PyPi](https://img.shields.io/pypi/v/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
 [![Downloads](https://pepy.tech/badge/sign-language-translator)](https://pepy.tech/project/sign-language-translator)
 
 1. [Overview](#overview)
    1. [Solution](#solution)
    2. [Major Components and Goals](#major-components-and-goals)
    3. [Datasets](#datasets)
 2. [How to install the package](#how-to-install-the-package)
 3. [Usage](#usage)
    1. [basic translation](#basic-translation)
    2. [text language processor](#text-language-processor)
    3. [sign language processor](#sign-language-processor)
+   4. [language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Credits and Gratitude](#credits-and-gratitude)
 7. [Bonus](#bonus)
    1. number of lines of code
    2. just for fun
    3. publish package on PyPI
@@ -184,17 +183,31 @@
 ###### sign language processor
 
 ```python
 from sign_language_translator.languages.sign import PakistanSignLanguage
 
 psl = PakistanSignLanguage()
 
-tokens = ["he", "school", "went"]
-file_labels = psl.to_file_label(tokens)
-# file_labels = ["pk-hfad-1_وہ", "pk-hfad-1_school", "pk-hfad-1_گیا"]
+tokens = ["he", " ", "went", " ", "to", " ", "school", "."]
+tags = [Tags.WORD, Tags.SPACE] * 3 + [Tags.WORD, Tags.PUNCTUATION]
+tokens, tags, _ = psl.restructure_sentence(tokens, tags) # ["he", "school", "go"]
+signs  = psl.tokens_to_sign_dicts(tokens, tags)
+# signs = [
+#   {'signs': [['pk-hfad-1_وہ']], 'weights': [1.0]},
+#   {'signs': [['pk-hfad-1_school']], 'weights': [1.0]},
+#   {'signs': [['pk-hfad-1_گیا']], 'weights': [1.0]}
+# ]
+```
+
+###### language models
+
+```python
+from sign_language_translator.models.language_models import BeamSampling, SimpleLanguageModel, Mixer, TransformerLanguageModel
+
+
 ```
 
 ## Directory Tree
 
 ```text
 sign-language-translator
 ├── README.md
@@ -263,30 +276,30 @@
 
 ## Research Paper
 
 Stay Tuned!
 
 ## Credits and Gratitude
 
-This project started in October 2021 as a BS Computer Science final year project with 3 students and 1 supervisor at PUCIT. After 9 months at university, it became a hobby project for Mudassar who has continued it till at least 2023-07-11.
+This project started in October 2021 as a BS Computer Science final year project with 3 students and 1 supervisor. After 9 months at university, it became a hobby project for Mudassar who has continued it till at least 2023-07-11.
 
 Immense gratitude towards:
 
 - [Mudassar Iqbal](https://github.com/mdsrqbl) for leading and coding the project so far.
 - Rabbia Arshad for help in initial R&D and web development.
 - Waqas Bin Abbas for assistance in video data collection process.
-- Dr Kamran Malik for teaching us AI, setting the initial project scope, idea of motion transfer and connecting us with Hamza Foundation.
+- Kamran Malik for setting the initial project scope, idea of motion transfer and connecting us with Hamza Foundation.
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **6580** + Tests: **780**):
+Count total number of **lines of code** (Package: **6595** + Tests: **781**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for fun**
```

### Comparing `sign_language_translator-0.4.0/pyproject.toml` & `sign_language_translator-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "sign_language_translator"
-version = "0.4.0"
+version = "0.4.2"
 description = "Translate between spoken/text and sign language using AI."
 authors = ["Mudassar Iqbal <mdsriqb@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "sign_language_translator"}]
 repository = "https://github.com/sign-language-translator/sign-language-translator"
 keywords = ["sign", "translation", "pose", "pakistan", "deep-learning", "computer-vision", "nlp", "sign-language", "sign-language-translation"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pytest = "^7.0.0"
 matplotlib = "^3.7.2"
-mediapipe = "^0.10.2"
+mediapipe = "0.9.1.0"
 moviepy = "^1.0.3"
 numpy = "^1.25.1"
 pandas = "^2.0.3"
 pillow = "^10.0.0"
 scipy = "^1.11.1"
 torch = "^2.0.1"
 scikit-image = "^0.21.0"
```

### Comparing `sign_language_translator-0.4.0/sign_language_translator/__init__.py` & `sign_language_translator-0.4.2/sign_language_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/config/enums.py` & `sign_language_translator-0.4.2/sign_language_translator/config/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,16 +41,22 @@
 
     # Body Mesh Grid
 
     # Image Segmentation
 
 
 class ModelCodes(enum.Enum):
+    # text-to-sign
     CONCATENATIVE_SYNTHESIS = "concatenative-synthesis"
 
+    # language-models
+    SIMPLE_LM = "simple-language-model"
+    MIXER_LM = "mixer"
+    TRANSFORMER_LM = "transformer-language-model"
+
 
 __all__ = [
     "Countries",
     "Organizations",
     "SignCollections",
     "TextLanguages",
     "SignLanguages",
```

### Comparing `sign_language_translator-0.4.0/sign_language_translator/config/helpers.py` & `sign_language_translator-0.4.2/sign_language_translator/config/helpers.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/data_collection/completeness.py` & `sign_language_translator-0.4.2/sign_language_translator/data_collection/completeness.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/data_collection/scraping.py` & `sign_language_translator-0.4.2/sign_language_translator/data_collection/scraping.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/data_collection/synonyms.py` & `sign_language_translator-0.4.2/sign_language_translator/data_collection/synonyms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/sign/__init__.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/sign/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/sign/mapping_rules.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/sign/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/sign/pakistan_sign_language.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/sign/pakistan_sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/sign/sign_language.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/sign/sign_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/text/text_language.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/text/text_language.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/text/urdu.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/text/urdu.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/utils.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/languages/vocab.py` & `sign_language_translator-0.4.2/sign_language_translator/languages/vocab.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/language_models/abstract_language_model.py` & `sign_language_translator-0.4.2/sign_language_translator/models/language_models/abstract_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/language_models/beam_sampling.py` & `sign_language_translator-0.4.2/sign_language_translator/models/language_models/beam_sampling.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/language_models/mixer.py` & `sign_language_translator-0.4.2/sign_language_translator/models/language_models/mixer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/language_models/simple_language_model.py` & `sign_language_translator-0.4.2/sign_language_translator/models/language_models/simple_language_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/text_to_sign/concatenative_synthesis.py` & `sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/concatenative_synthesis.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/text_to_sign/t2s_model.py` & `sign_language_translator-0.4.2/sign_language_translator/models/text_to_sign/t2s_model.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/models/utils.py` & `sign_language_translator-0.4.2/sign_language_translator/models/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/metrics.py` & `sign_language_translator-0.4.2/sign_language_translator/text/metrics.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/preprocess.py` & `sign_language_translator-0.4.2/sign_language_translator/text/preprocess.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/subtitles.py` & `sign_language_translator-0.4.2/sign_language_translator/text/subtitles.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/tagger.py` & `sign_language_translator-0.4.2/sign_language_translator/text/tagger.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/tokenizer.py` & `sign_language_translator-0.4.2/sign_language_translator/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/text/utils.py` & `sign_language_translator-0.4.2/sign_language_translator/text/utils.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/utils/data_loader.py` & `sign_language_translator-0.4.2/sign_language_translator/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/utils/landmarks_info.py` & `sign_language_translator-0.4.2/sign_language_translator/utils/landmarks_info.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/utils/sign_data_attributes.py` & `sign_language_translator-0.4.2/sign_language_translator/utils/sign_data_attributes.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/utils/tree.py` & `sign_language_translator-0.4.2/sign_language_translator/utils/tree.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/vision/concatenate.py` & `sign_language_translator-0.4.2/sign_language_translator/vision/concatenate.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/vision/embed.py` & `sign_language_translator-0.4.2/sign_language_translator/vision/embed.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/vision/transforms.py` & `sign_language_translator-0.4.2/sign_language_translator/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/sign_language_translator/vision/visualization.py` & `sign_language_translator-0.4.2/sign_language_translator/vision/visualization.py`

 * *Files identical despite different names*

### Comparing `sign_language_translator-0.4.0/PKG-INFO` & `sign_language_translator-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sign-language-translator
-Version: 0.4.0
+Version: 0.4.2
 Summary: Translate between spoken/text and sign language using AI.
 Home-page: https://github.com/sign-language-translator/sign-language-translator
 License: Apache-2.0
 Keywords: sign,translation,pose,pakistan,deep-learning,computer-vision,nlp,sign-language,sign-language-translation
 Author: Mudassar Iqbal
 Author-email: mdsriqb@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: deep-translator (>=1.11.4,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: mediapipe (>=0.10.2,<0.11.0)
+Requires-Dist: mediapipe (==0.9.1.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: opencv-contrib-python (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
 Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
@@ -28,29 +28,28 @@
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/sign-language-translator/sign-language-translator
 Description-Content-Type: text/markdown
 
 # Sign Language Translator ⠎⠇⠞
 
-[![python](https://img.shields.io/pypi/pyversions/sign-language-tranlator)](https://pypi.org/project/sign-language-tranlator/)
-
-[![PyPi](https://img.shields.io/pypi/v/sign-language-tranlator)](https://pypi.org/project/sign-language-tranlator/)
-
+[![python](https://img.shields.io/pypi/pyversions/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
+[![PyPi](https://img.shields.io/pypi/v/sign-language-translator)](https://pypi.org/project/sign-language-translator/)
 [![Downloads](https://pepy.tech/badge/sign-language-translator)](https://pepy.tech/project/sign-language-translator)
 
 1. [Overview](#overview)
    1. [Solution](#solution)
    2. [Major Components and Goals](#major-components-and-goals)
    3. [Datasets](#datasets)
 2. [How to install the package](#how-to-install-the-package)
 3. [Usage](#usage)
    1. [basic translation](#basic-translation)
    2. [text language processor](#text-language-processor)
    3. [sign language processor](#sign-language-processor)
+   4. [language models](#language-models)
 4. [Directory Tree](#directory-tree)
 5. [Research Paper](#research-paper)
 6. [Credits and Gratitude](#credits-and-gratitude)
 7. [Bonus](#bonus)
    1. number of lines of code
    2. just for fun
    3. publish package on PyPI
@@ -216,17 +215,31 @@
 ###### sign language processor
 
 ```python
 from sign_language_translator.languages.sign import PakistanSignLanguage
 
 psl = PakistanSignLanguage()
 
-tokens = ["he", "school", "went"]
-file_labels = psl.to_file_label(tokens)
-# file_labels = ["pk-hfad-1_وہ", "pk-hfad-1_school", "pk-hfad-1_گیا"]
+tokens = ["he", " ", "went", " ", "to", " ", "school", "."]
+tags = [Tags.WORD, Tags.SPACE] * 3 + [Tags.WORD, Tags.PUNCTUATION]
+tokens, tags, _ = psl.restructure_sentence(tokens, tags) # ["he", "school", "go"]
+signs  = psl.tokens_to_sign_dicts(tokens, tags)
+# signs = [
+#   {'signs': [['pk-hfad-1_وہ']], 'weights': [1.0]},
+#   {'signs': [['pk-hfad-1_school']], 'weights': [1.0]},
+#   {'signs': [['pk-hfad-1_گیا']], 'weights': [1.0]}
+# ]
+```
+
+###### language models
+
+```python
+from sign_language_translator.models.language_models import BeamSampling, SimpleLanguageModel, Mixer, TransformerLanguageModel
+
+
 ```
 
 ## Directory Tree
 
 ```text
 sign-language-translator
 ├── README.md
@@ -295,30 +308,30 @@
 
 ## Research Paper
 
 Stay Tuned!
 
 ## Credits and Gratitude
 
-This project started in October 2021 as a BS Computer Science final year project with 3 students and 1 supervisor at PUCIT. After 9 months at university, it became a hobby project for Mudassar who has continued it till at least 2023-07-11.
+This project started in October 2021 as a BS Computer Science final year project with 3 students and 1 supervisor. After 9 months at university, it became a hobby project for Mudassar who has continued it till at least 2023-07-11.
 
 Immense gratitude towards:
 
 - [Mudassar Iqbal](https://github.com/mdsrqbl) for leading and coding the project so far.
 - Rabbia Arshad for help in initial R&D and web development.
 - Waqas Bin Abbas for assistance in video data collection process.
-- Dr Kamran Malik for teaching us AI, setting the initial project scope, idea of motion transfer and connecting us with Hamza Foundation.
+- Kamran Malik for setting the initial project scope, idea of motion transfer and connecting us with Hamza Foundation.
 - [Hamza Foundation](https://www.youtube.com/@pslhamzafoundationacademyf7624/videos) (especially Ms Benish, Ms Rashda & Mr Zeeshan) for agreeing for collaboration and providing the reference clips, hearing-impaired performers for data creation, and creating the text2gloss dataset.
 - [UrduHack](https://github.com/urduhack/urduhack) (espacially Ikram Ali) for their work on Urdu character normalization.
 
 - [Telha Bilal](https://github.com/TelhaBilal) for help in designing the architecture of some modules.
 
 ## Bonus
 
-Count total number of **lines of code** (Package: **6580** + Tests: **780**):
+Count total number of **lines of code** (Package: **6595** + Tests: **781**):
 
 ```bash
 git ls-files | grep '\.py' | xargs wc -l
 ```
 
 **Just for fun**
```

