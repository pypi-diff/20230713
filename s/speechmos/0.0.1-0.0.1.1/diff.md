# Comparing `tmp/speechmos-0.0.1.tar.gz` & `tmp/speechmos-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechmos-0.0.1.tar", last modified: Fri Jun 30 09:00:07 2023, max compression
+gzip compressed data, was "speechmos-0.0.1.1.tar", last modified: Thu Jul 13 07:01:22 2023, max compression
```

## Comparing `speechmos-0.0.1.tar` & `speechmos-0.0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.579883 speechmos-0.0.1/
--rw-rw-rw-   0        0        0     1160 2023-06-27 08:18:05.000000 speechmos-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       72 2023-06-28 13:12:13.000000 speechmos-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7045 2023-06-30 09:00:07.578887 speechmos-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6044 2023-06-29 11:36:11.000000 speechmos-0.0.1/README.md
--rw-rw-rw-   0        0        0     1611 2023-06-30 08:58:10.000000 speechmos-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 09:00:07.579883 speechmos-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.434034 speechmos-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.458089 speechmos-0.0.1/src/speechmos/
--rw-rw-rw-   0        0        0        0 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/__init__.py
--rw-rw-rw-   0        0        0     7858 2023-06-29 11:02:01.000000 speechmos-0.0.1/src/speechmos/aecmos.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.502272 speechmos-0.0.1/src/speechmos/aecmos_models/
--rw-rw-rw-   0        0        0  1170947 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/aecmos_models/Run_1663829550_Stage_0.onnx
--rw-rw-rw-   0        0        0  1170192 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/aecmos_models/Run_1663915512_Stage_0.onnx
--rw-rw-rw-   0        0        0  2682822 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/aecmos_models/Run_1668423760_Stage_0.onnx
--rw-rw-rw-   0        0        0     6070 2023-06-29 11:41:34.000000 speechmos-0.0.1/src/speechmos/dnsmos.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.546115 speechmos-0.0.1/src/speechmos/dnsmos_models/
--rw-rw-rw-   0        0        0   742375 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/dnsmos_models/bak_ovr.onnx
--rw-rw-rw-   0        0        0   224860 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/dnsmos_models/model_v8.onnx
--rw-rw-rw-   0        0        0   742203 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/dnsmos_models/sig.onnx
--rw-rw-rw-   0        0        0  1157965 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/dnsmos_models/sig_bak_ovr.onnx
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.554113 speechmos-0.0.1/src/speechmos/pdnsmos_models/
--rw-rw-rw-   0        0        0  1157962 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/pdnsmos_models/sig_bak_ovr.onnx
--rw-rw-rw-   0        0        0     6548 2023-06-29 11:01:41.000000 speechmos-0.0.1/src/speechmos/plcmos.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.575884 speechmos-0.0.1/src/speechmos/plcmos_models/
--rw-rw-rw-   0        0        0  1344808 2023-06-27 08:18:05.000000 speechmos-0.0.1/src/speechmos/plcmos_models/plcmos_v2.onnx
-drwxrwxrwx   0        0        0        0 2023-06-30 09:00:07.484165 speechmos-0.0.1/src/speechmos.egg-info/
--rw-rw-rw-   0        0        0     7045 2023-06-30 09:00:07.000000 speechmos-0.0.1/src/speechmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      716 2023-06-30 09:00:07.000000 speechmos-0.0.1/src/speechmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:00:07.000000 speechmos-0.0.1/src/speechmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 09:00:07.000000 speechmos-0.0.1/src/speechmos.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:22.067218 speechmos-0.0.1.1/
+-rw-rw-rw-   0        0        0     1160 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       72 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7043 2023-07-13 07:01:22.067218 speechmos-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6040 2023-07-13 06:55:31.000000 speechmos-0.0.1.1/README.md
+-rw-rw-rw-   0        0        0     1613 2023-07-13 06:55:29.000000 speechmos-0.0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:01:22.067218 speechmos-0.0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:21.942377 speechmos-0.0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:21.958008 speechmos-0.0.1.1/src/speechmos/
+-rw-rw-rw-   0        0        0        0 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/__init__.py
+-rw-rw-rw-   0        0        0     7858 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/aecmos.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:21.978776 speechmos-0.0.1.1/src/speechmos/aecmos_models/
+-rw-rw-rw-   0        0        0  1170947 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1663829550_Stage_0.onnx
+-rw-rw-rw-   0        0        0  1170192 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1663915512_Stage_0.onnx
+-rw-rw-rw-   0        0        0  2682822 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1668423760_Stage_0.onnx
+-rw-rw-rw-   0        0        0     6070 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/dnsmos.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:22.021016 speechmos-0.0.1.1/src/speechmos/dnsmos_models/
+-rw-rw-rw-   0        0        0   742375 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/dnsmos_models/bak_ovr.onnx
+-rw-rw-rw-   0        0        0   224860 2023-07-13 06:27:05.000000 speechmos-0.0.1.1/src/speechmos/dnsmos_models/model_v8.onnx
+-rw-rw-rw-   0        0        0   742203 2023-07-13 06:27:06.000000 speechmos-0.0.1.1/src/speechmos/dnsmos_models/sig.onnx
+-rw-rw-rw-   0        0        0  1157965 2023-07-13 06:27:06.000000 speechmos-0.0.1.1/src/speechmos/dnsmos_models/sig_bak_ovr.onnx
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:22.036022 speechmos-0.0.1.1/src/speechmos/pdnsmos_models/
+-rw-rw-rw-   0        0        0  1157962 2023-07-13 06:27:06.000000 speechmos-0.0.1.1/src/speechmos/pdnsmos_models/sig_bak_ovr.onnx
+-rw-rw-rw-   0        0        0     6548 2023-07-13 06:27:06.000000 speechmos-0.0.1.1/src/speechmos/plcmos.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:22.051682 speechmos-0.0.1.1/src/speechmos/plcmos_models/
+-rw-rw-rw-   0        0        0  1344808 2023-07-13 06:27:06.000000 speechmos-0.0.1.1/src/speechmos/plcmos_models/plcmos_v2.onnx
+drwxrwxrwx   0        0        0        0 2023-07-13 07:01:21.973545 speechmos-0.0.1.1/src/speechmos.egg-info/
+-rw-rw-rw-   0        0        0     7043 2023-07-13 07:01:21.000000 speechmos-0.0.1.1/src/speechmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2023-07-13 07:01:21.000000 speechmos-0.0.1.1/src/speechmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:01:21.000000 speechmos-0.0.1.1/src/speechmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 07:01:21.000000 speechmos-0.0.1.1/src/speechmos.egg-info/top_level.txt
```

### Comparing `speechmos-0.0.1/LICENSE.txt` & `speechmos-0.0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/PKG-INFO` & `speechmos-0.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmos
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: MOS (Mean Opinion Score) models for evaluating audio quality.
 Author-email: Marju Purin <marjupurin@microsoft.com>, AEC Challenge Organizers <aec_challenge@microsoft.com>
 Maintainer-email: AEC Challenge Organizers <aec_challenge@microsoft.com>, Marju Purin <marjupurin@microsoft.com>
 Project-URL: AEC (acoustic echo cancellation), https://github.com/microsoft/AEC-Challenge
 Project-URL: DNS (deep noise suppression), https://github.com/microsoft/DNS-Challenge
 Project-URL: PLC (packet loss concealment), https://github.com/microsoft/PLC-Challenge
 Keywords: aecmos,dnsmos,plcmos,acoustic echo cancellation,noise suppression,packet loss concealment,audio evaluation,speech evaluation,mean opinion score,MOS,audio quality,speech quality
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # AECMOS, DNSMOS, PLCMOS
 
-* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836, "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108, "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127, "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
+* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836 "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108 "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127 "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
 
 ## Prerequisites
 - Python 3.7 and above
 - librosa 0.9.1
 - numpy 1.21.5
 - onnxruntime 1.10.0
 - pandas
@@ -44,15 +44,15 @@
     
     All audio should be single channel (mono) audio.  
     Alternatively, `sample` can be a list of items of one of the above types.  
 
 -  `sr` denotes the sampling rate. Sampling rate should be either 16000 or 48000. AECMOS is available at 48kHz, all other models are available at 16kHz. All audio should be provided at the correct sampling rate.
 
 For AECMOS:
-- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model will be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
+- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model can be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
 
 For DNSMOS: 
 - `model_type` controls which DNSMOS model to use: `'dnsmos'` or `'dnsmos_personalized'`. The default is `'dnsmos'`.
 
 Additional arguments:
 - `return_df` controls whether a pandas dataframe is returned containing sample information and MOS scores when evaluating a list of samples. The default is `return_df = True`. If set to `False`, a list of dictionaries is returned instead.
 - `verbose` controls whether more details are printed on the screen. The default is `verbose = False`.
```

### Comparing `speechmos-0.0.1/README.md` & `speechmos-0.0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AECMOS, DNSMOS, PLCMOS
 
-* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836, "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108, "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127, "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
+* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836 "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108 "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127 "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
 
 ## Prerequisites
 - Python 3.7 and above
 - librosa 0.9.1
 - numpy 1.21.5
 - onnxruntime 1.10.0
 - pandas
@@ -28,15 +28,15 @@
     
     All audio should be single channel (mono) audio.  
     Alternatively, `sample` can be a list of items of one of the above types.  
 
 -  `sr` denotes the sampling rate. Sampling rate should be either 16000 or 48000. AECMOS is available at 48kHz, all other models are available at 16kHz. All audio should be provided at the correct sampling rate.
 
 For AECMOS:
-- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model will be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
+- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model can be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
 
 For DNSMOS: 
 - `model_type` controls which DNSMOS model to use: `'dnsmos'` or `'dnsmos_personalized'`. The default is `'dnsmos'`.
 
 Additional arguments:
 - `return_df` controls whether a pandas dataframe is returned containing sample information and MOS scores when evaluating a list of samples. The default is `return_df = True`. If set to `False`, a list of dictionaries is returned instead.
 - `verbose` controls whether more details are printed on the screen. The default is `verbose = False`.
```

### Comparing `speechmos-0.0.1/pyproject.toml` & `speechmos-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "numpy>=1.21.5", "librosa>=0.9.1", "onnxruntime>=1.10.0",
 "tqdm", "pandas", ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speechmos"
-version = "0.0.1"
+version = "0.0.1.1"
 authors = [{name="Marju Purin", email="marjupurin@microsoft.com"},
 {name="AEC Challenge Organizers", email="aec_challenge@microsoft.com"},  
 ]
 maintainers = [{name="AEC Challenge Organizers", email="aec_challenge@microsoft.com"},
 {name="Marju Purin", email="marjupurin@microsoft.com"},
 ]
 description = "MOS (Mean Opinion Score) models for evaluating audio quality."
```

### Comparing `speechmos-0.0.1/src/speechmos/aecmos.py` & `speechmos-0.0.1.1/src/speechmos/aecmos.py`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/aecmos_models/Run_1663829550_Stage_0.onnx` & `speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1663829550_Stage_0.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/aecmos_models/Run_1663915512_Stage_0.onnx` & `speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1663915512_Stage_0.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/aecmos_models/Run_1668423760_Stage_0.onnx` & `speechmos-0.0.1.1/src/speechmos/aecmos_models/Run_1668423760_Stage_0.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/dnsmos.py` & `speechmos-0.0.1.1/src/speechmos/dnsmos.py`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/dnsmos_models/bak_ovr.onnx` & `speechmos-0.0.1.1/src/speechmos/dnsmos_models/bak_ovr.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/dnsmos_models/model_v8.onnx` & `speechmos-0.0.1.1/src/speechmos/dnsmos_models/model_v8.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/dnsmos_models/sig.onnx` & `speechmos-0.0.1.1/src/speechmos/dnsmos_models/sig.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/dnsmos_models/sig_bak_ovr.onnx` & `speechmos-0.0.1.1/src/speechmos/dnsmos_models/sig_bak_ovr.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/pdnsmos_models/sig_bak_ovr.onnx` & `speechmos-0.0.1.1/src/speechmos/pdnsmos_models/sig_bak_ovr.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/plcmos.py` & `speechmos-0.0.1.1/src/speechmos/plcmos.py`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos/plcmos_models/plcmos_v2.onnx` & `speechmos-0.0.1.1/src/speechmos/plcmos_models/plcmos_v2.onnx`

 * *Files identical despite different names*

### Comparing `speechmos-0.0.1/src/speechmos.egg-info/PKG-INFO` & `speechmos-0.0.1.1/src/speechmos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechmos
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: MOS (Mean Opinion Score) models for evaluating audio quality.
 Author-email: Marju Purin <marjupurin@microsoft.com>, AEC Challenge Organizers <aec_challenge@microsoft.com>
 Maintainer-email: AEC Challenge Organizers <aec_challenge@microsoft.com>, Marju Purin <marjupurin@microsoft.com>
 Project-URL: AEC (acoustic echo cancellation), https://github.com/microsoft/AEC-Challenge
 Project-URL: DNS (deep noise suppression), https://github.com/microsoft/DNS-Challenge
 Project-URL: PLC (packet loss concealment), https://github.com/microsoft/PLC-Challenge
 Keywords: aecmos,dnsmos,plcmos,acoustic echo cancellation,noise suppression,packet loss concealment,audio evaluation,speech evaluation,mean opinion score,MOS,audio quality,speech quality
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # AECMOS, DNSMOS, PLCMOS
 
-* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836, "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108, "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127, "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
+* We release the [AECMOS](https://ieeexplore.ieee.org/document/9747836 "AECMOS: A Speech Quality Assessment Metric for Echo Impairment."), [DNSMOS](https://ieeexplore.ieee.org/document/9746108 "DNSMOS P.835: A Non-Intrusive Perceptual Objective Speech Quality Metric to Evaluate Noise Suppressors."), and [PLCMOS](https://arxiv.org/abs/2305.15127 "PLCMOS--a data-driven non-intrusive metric for the evaluation of packet loss concealment algorithms.") models that we have developed for evaluating audio degradations due to echo, noise, packet loss and other sources.
 
 ## Prerequisites
 - Python 3.7 and above
 - librosa 0.9.1
 - numpy 1.21.5
 - onnxruntime 1.10.0
 - pandas
@@ -44,15 +44,15 @@
     
     All audio should be single channel (mono) audio.  
     Alternatively, `sample` can be a list of items of one of the above types.  
 
 -  `sr` denotes the sampling rate. Sampling rate should be either 16000 or 48000. AECMOS is available at 48kHz, all other models are available at 16kHz. All audio should be provided at the correct sampling rate.
 
 For AECMOS:
-- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model will be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
+- `talk_type` specifies the scenario: `'st'` (far-end single talk), `'nst'` (near-end single talk), or `'dt'` (double talk) if known. `talk_type` can be `None` in which case the 16kHz scenarioless model can be used. The performance is about 2% lower in correlation with the ground truth than the scenario based model.
 
 For DNSMOS: 
 - `model_type` controls which DNSMOS model to use: `'dnsmos'` or `'dnsmos_personalized'`. The default is `'dnsmos'`.
 
 Additional arguments:
 - `return_df` controls whether a pandas dataframe is returned containing sample information and MOS scores when evaluating a list of samples. The default is `return_df = True`. If set to `False`, a list of dictionaries is returned instead.
 - `verbose` controls whether more details are printed on the screen. The default is `verbose = False`.
```

### Comparing `speechmos-0.0.1/src/speechmos.egg-info/SOURCES.txt` & `speechmos-0.0.1.1/src/speechmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

