# Comparing `tmp/stable-ts-2.6.4.tar.gz` & `tmp/stable-ts-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.6.4.tar", last modified: Fri Jun  9 16:54:09 2023, max compression
+gzip compressed data, was "stable-ts-2.7.0.tar", last modified: Thu Jul 13 00:56:15 2023, max compression
```

## Comparing `stable-ts-2.6.4.tar` & `stable-ts-2.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.808747 stable-ts-2.6.4/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.4/LICENSE
--rw-rw-rw-   0        0        0    11608 2023-06-09 16:54:09.807744 stable-ts-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    11312 2023-06-09 01:22:48.000000 stable-ts-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 16:54:09.808747 stable-ts-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.749234 stable-ts-2.6.4/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11608 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 16:54:09.000000 stable-ts-2.6.4/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 16:54:09.805738 stable-ts-2.6.4/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.4/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.4/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-06-09 16:50:46.000000 stable-ts-2.6.4/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.4/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.4/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.4/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.4/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    40573 2023-06-09 01:03:20.000000 stable-ts-2.6.4/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.4/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.4/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.4/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.4/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53434 2023-06-09 16:49:15.000000 stable-ts-2.6.4/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.247666 stable-ts-2.7.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0    11472 2023-07-13 00:56:15.246663 stable-ts-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11176 2023-07-13 00:51:01.000000 stable-ts-2.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 00:56:15.247666 stable-ts-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.226222 stable-ts-2.7.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11472 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-07-13 00:56:15.000000 stable-ts-2.7.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 00:56:14.000000 stable-ts-2.7.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 00:56:15.244670 stable-ts-2.7.0/stable_whisper/
+-rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-07-09 22:10:17.000000 stable-ts-2.7.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.0/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.0/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    42984 2023-07-13 00:51:01.000000 stable-ts-2.7.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.4/LICENSE` & `stable-ts-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/PKG-INFO` & `stable-ts-2.7.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: stable-ts
-Version: 2.6.4
-Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
-Home-page: https://github.com/jianfch/stable-ts
-Author: Jian
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Stabilizing Timestamps for Whisper
 
 This script modifies [OpenAI's Whisper](https://github.com/openai/whisper) to produce more reliable timestamps.
 
 https://user-images.githubusercontent.com/28970749/225826345-ef7115db-51e4-4b23-aedd-069389b8ae43.mp4
 
 * [Setup](#setup)
@@ -21,14 +10,15 @@
   * [Output](#output)
   * [Regrouping Words](#regrouping-words)
   * [Locating Words](#locating-words)
   * [Boosting Performance](#boosting-performance)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Tips](#tips)
+  * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
 ```
 pip install -U stable-ts
 ```
 
@@ -47,28 +37,28 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L637-L652), 
-[transcribe()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L75-L199)
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
 result.to_tsv('audio.tsv') #TSV
 ```
 Parameters: 
-[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L267-L291),
-[to_ass()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L401-L434),
-[to_tsv()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L335-L353)
+[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L261-L297),
+[to_ass()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L393-L440),
+[to_tsv()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L329-L359)
 <br /><br />
 There are word-level and segment-level timestamps. All output formats support them. 
 They also support will both levels simultaneously except TSV. 
 By default, `segment_level` and `word_level` are both `True` for all the formats that support both simultaneously.<br /><br />
 Examples in VTT.
 
 Default: `segment_level=True` + `word_level=True` or `--segment_level true` + `--word_level true` for CLI
@@ -136,24 +126,28 @@
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+
+# To undo all regrouping operations:
+result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -168,15 +162,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
@@ -202,42 +196,46 @@
 #### With [Silero VAD](https://github.com/snakers4/silero-vad)
 ```python
 # [vad_threshold]=0.35 (default)
 stable_whisper.visualize_suppression('audio.mp3', 'image.png', vad=True, vad_threshold=0.35)
 ```
 ![vad](https://user-images.githubusercontent.com/28970749/225825446-980924a5-7485-41e1-b0d9-c9b069d605f2.png)
 Parameters: 
-[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/stabilization.py#L334-L355)
+[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/stabilization.py#L328-L357)
 
 ### Encode Comparison 
 You can encode videos similar to the ones in the doc for comparing transcriptions of the same audio. 
 ```python
 stable_whisper.encode_video_comparison(
     'audio.mp3', 
     ['audio_sub1.srt', 'audio_sub2.srt'], 
     output_videopath='audio.mp4', 
     labels=['Example 1', 'Example 2']
 )
 ```
 Parameters: 
-[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/video_output.py#L10-L27)
+[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/video_output.py#L10-L27)
 
 ### Tips
 - for reliable segment timestamps, do not disable word timestamps with `word_timestamps=False` because word timestamps are also used to correct segment timestamps
 - use `demucs=True` and `vad=True` for music but also works for non-music
 - if audio is not transcribing properly compared to whisper, try `mel_first=True` at the cost of more memory usage for long audio tracks
 - enable dynamic quantization to decrease memory usage for inference on CPU (also increases inference speed for large model);
 `--dq true`/`dq=True` for `stable_whisper.load_model`
 
 #### Multiple Files with CLI 
 Transcribe multiple audio files then process the results directly into SRT files.
 ```commandline
 stable-ts audio1.mp3 audio2.mp3 audio3.mp3 -o audio1.srt audio2.srt audio3.srt
 ```
 
+### Any ASR
+You can use most of the features of Stable-ts improve the results of any ASR model/APIs. 
+[Just follow this notebook](https://github.com/jianfch/stable-ts/blob/main/examples/non-whisper.ipynb).
+
 ## Quick 1.X → 2.X Guide
 ### What's new in 2.0.0?
 - updated to use Whisper's more reliable word-level timestamps method. 
 - the more reliable word timestamps allow regrouping all words into segments with more natural boundaries.
 - can now suppress silence with [Silero VAD](https://github.com/snakers4/silero-vad) (requires PyTorch 1.12.0+)
 - non-VAD silence suppression is also more robust
 ### Usage changes
```

### Comparing `stable-ts-2.6.4/README.md` & `stable-ts-2.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: stable-ts
+Version: 2.7.0
+Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
+Home-page: https://github.com/jianfch/stable-ts
+Author: Jian
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Stabilizing Timestamps for Whisper
 
 This script modifies [OpenAI's Whisper](https://github.com/openai/whisper) to produce more reliable timestamps.
 
 https://user-images.githubusercontent.com/28970749/225826345-ef7115db-51e4-4b23-aedd-069389b8ae43.mp4
 
 * [Setup](#setup)
@@ -10,14 +21,15 @@
   * [Output](#output)
   * [Regrouping Words](#regrouping-words)
   * [Locating Words](#locating-words)
   * [Boosting Performance](#boosting-performance)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Tips](#tips)
+  * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
 ```
 pip install -U stable-ts
 ```
 
@@ -36,28 +48,28 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L637-L652), 
-[transcribe()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L75-L199)
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
 result.to_tsv('audio.tsv') #TSV
 ```
 Parameters: 
-[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L267-L291),
-[to_ass()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L401-L434),
-[to_tsv()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L335-L353)
+[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L261-L297),
+[to_ass()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L393-L440),
+[to_tsv()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L329-L359)
 <br /><br />
 There are word-level and segment-level timestamps. All output formats support them. 
 They also support will both levels simultaneously except TSV. 
 By default, `segment_level` and `word_level` are both `True` for all the formats that support both simultaneously.<br /><br />
 Examples in VTT.
 
 Default: `segment_level=True` + `word_level=True` or `--segment_level true` + `--word_level true` for CLI
@@ -125,24 +137,28 @@
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+
+# To undo all regrouping operations:
+result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -157,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
@@ -191,42 +207,46 @@
 #### With [Silero VAD](https://github.com/snakers4/silero-vad)
 ```python
 # [vad_threshold]=0.35 (default)
 stable_whisper.visualize_suppression('audio.mp3', 'image.png', vad=True, vad_threshold=0.35)
 ```
 ![vad](https://user-images.githubusercontent.com/28970749/225825446-980924a5-7485-41e1-b0d9-c9b069d605f2.png)
 Parameters: 
-[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/stabilization.py#L334-L355)
+[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/stabilization.py#L328-L357)
 
 ### Encode Comparison 
 You can encode videos similar to the ones in the doc for comparing transcriptions of the same audio. 
 ```python
 stable_whisper.encode_video_comparison(
     'audio.mp3', 
     ['audio_sub1.srt', 'audio_sub2.srt'], 
     output_videopath='audio.mp4', 
     labels=['Example 1', 'Example 2']
 )
 ```
 Parameters: 
-[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/video_output.py#L10-L27)
+[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/video_output.py#L10-L27)
 
 ### Tips
 - for reliable segment timestamps, do not disable word timestamps with `word_timestamps=False` because word timestamps are also used to correct segment timestamps
 - use `demucs=True` and `vad=True` for music but also works for non-music
 - if audio is not transcribing properly compared to whisper, try `mel_first=True` at the cost of more memory usage for long audio tracks
 - enable dynamic quantization to decrease memory usage for inference on CPU (also increases inference speed for large model);
 `--dq true`/`dq=True` for `stable_whisper.load_model`
 
 #### Multiple Files with CLI 
 Transcribe multiple audio files then process the results directly into SRT files.
 ```commandline
 stable-ts audio1.mp3 audio2.mp3 audio3.mp3 -o audio1.srt audio2.srt audio3.srt
 ```
 
+### Any ASR
+You can use most of the features of Stable-ts improve the results of any ASR model/APIs. 
+[Just follow this notebook](https://github.com/jianfch/stable-ts/blob/main/examples/non-whisper.ipynb).
+
 ## Quick 1.X → 2.X Guide
 ### What's new in 2.0.0?
 - updated to use Whisper's more reliable word-level timestamps method. 
 - the more reliable word timestamps allow regrouping all words into segments with more natural boundaries.
 - can now suppress silence with [Silero VAD](https://github.com/snakers4/silero-vad) (requires PyTorch 1.12.0+)
 - non-VAD silence suppression is also more robust
 ### Usage changes
```

### Comparing `stable-ts-2.6.4/setup.py` & `stable-ts-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.7.0/stable_ts.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.4
+Version: 2.7.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,14 +21,15 @@
   * [Output](#output)
   * [Regrouping Words](#regrouping-words)
   * [Locating Words](#locating-words)
   * [Boosting Performance](#boosting-performance)
   * [Visualizing Suppression](#visualizing-suppression)
   * [Encode Comparison](#encode-comparison)
   * [Tips](#tips)
+  * [Use with any ASR](#any-asr)
 * [Quick 1.X → 2.X Guide](#quick-1x--2x-guide)
 
 ## Setup
 ```
 pip install -U stable-ts
 ```
 
@@ -47,28 +48,28 @@
 ```python
 import stable_whisper
 model = stable_whisper.load_model('base')
 result = model.transcribe('audio.mp3')
 result.to_srt_vtt('audio.srt')
 ```
 Parameters: 
-[load_model()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L637-L652), 
-[transcribe()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/whisper_word_level.py#L75-L199)
+[load_model()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L633-L658), 
+[transcribe()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/whisper_word_level.py#L68-L203)
 ### Output
 Stable-ts supports various text output formats.
 ```python
 result.to_srt_vtt('audio.srt') #SRT
 result.to_srt_vtt('audio.vtt') #VTT
 result.to_ass('audio.ass') #ASS
 result.to_tsv('audio.tsv') #TSV
 ```
 Parameters: 
-[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L267-L291),
-[to_ass()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L401-L434),
-[to_tsv()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/text_output.py#L335-L353)
+[to_srt_vtt()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L261-L297),
+[to_ass()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L393-L440),
+[to_tsv()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/text_output.py#L329-L359)
 <br /><br />
 There are word-level and segment-level timestamps. All output formats support them. 
 They also support will both levels simultaneously except TSV. 
 By default, `segment_level` and `word_level` are both `True` for all the formats that support both simultaneously.<br /><br />
 Examples in VTT.
 
 Default: `segment_level=True` + `word_level=True` or `--segment_level true` + `--word_level true` for CLI
@@ -136,24 +137,28 @@
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
     .merge_by_gap(.15, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
 result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+
+# To undo all regrouping operations:
+result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L808-L854)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L526-L543)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L579-L595)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L637-L658)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L547-L573)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L599-L624)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/7c6953526dce5d9058b23e8d0c223272bf808be7/stable_whisper/result.py#L630-L633)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L864-L911)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L678-L690)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L731-L742)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L792-L808)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L702-L720)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L754-L772)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L779-L781)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L815-L830)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -168,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/result.py#L898-L913)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L956-L972)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
@@ -202,42 +207,46 @@
 #### With [Silero VAD](https://github.com/snakers4/silero-vad)
 ```python
 # [vad_threshold]=0.35 (default)
 stable_whisper.visualize_suppression('audio.mp3', 'image.png', vad=True, vad_threshold=0.35)
 ```
 ![vad](https://user-images.githubusercontent.com/28970749/225825446-980924a5-7485-41e1-b0d9-c9b069d605f2.png)
 Parameters: 
-[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/stabilization.py#L334-L355)
+[visualize_suppression()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/stabilization.py#L328-L357)
 
 ### Encode Comparison 
 You can encode videos similar to the ones in the doc for comparing transcriptions of the same audio. 
 ```python
 stable_whisper.encode_video_comparison(
     'audio.mp3', 
     ['audio_sub1.srt', 'audio_sub2.srt'], 
     output_videopath='audio.mp4', 
     labels=['Example 1', 'Example 2']
 )
 ```
 Parameters: 
-[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/d30d0d1cfb5b17b4bf59c3fafcbbd21e37598ab9/stable_whisper/video_output.py#L10-L27)
+[encode_video_comparison()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/video_output.py#L10-L27)
 
 ### Tips
 - for reliable segment timestamps, do not disable word timestamps with `word_timestamps=False` because word timestamps are also used to correct segment timestamps
 - use `demucs=True` and `vad=True` for music but also works for non-music
 - if audio is not transcribing properly compared to whisper, try `mel_first=True` at the cost of more memory usage for long audio tracks
 - enable dynamic quantization to decrease memory usage for inference on CPU (also increases inference speed for large model);
 `--dq true`/`dq=True` for `stable_whisper.load_model`
 
 #### Multiple Files with CLI 
 Transcribe multiple audio files then process the results directly into SRT files.
 ```commandline
 stable-ts audio1.mp3 audio2.mp3 audio3.mp3 -o audio1.srt audio2.srt audio3.srt
 ```
 
+### Any ASR
+You can use most of the features of Stable-ts improve the results of any ASR model/APIs. 
+[Just follow this notebook](https://github.com/jianfch/stable-ts/blob/main/examples/non-whisper.ipynb).
+
 ## Quick 1.X → 2.X Guide
 ### What's new in 2.0.0?
 - updated to use Whisper's more reliable word-level timestamps method. 
 - the more reliable word timestamps allow regrouping all words into segments with more natural boundaries.
 - can now suppress silence with [Silero VAD](https://github.com/snakers4/silero-vad) (requires PyTorch 1.12.0+)
 - non-VAD silence suppression is also more robust
 ### Usage changes
```

### Comparing `stable-ts-2.6.4/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.7.0/stable_ts.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 stable_ts.egg-info/top_level.txt
 stable_whisper/__init__.py
 stable_whisper/__main__.py
 stable_whisper/_version.py
 stable_whisper/audio.py
 stable_whisper/decode.py
 stable_whisper/enhancement.py
+stable_whisper/non_whisper.py
 stable_whisper/quantization.py
 stable_whisper/result.py
 stable_whisper/stabilization.py
 stable_whisper/text_output.py
 stable_whisper/timing.py
 stable_whisper/video_output.py
 stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.4/stable_whisper/audio.py` & `stable-ts-2.7.0/stable_whisper/audio.py`

 * *Files 9% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     if isinstance(audio, (str, bytes)):
         if isinstance(audio, str) and not track_name:
             track_name = f'"{audio}"'
         audio = torch.from_numpy(load_audio(audio, model.samplerate))
     elif input_sr != model.samplerate:
         if input_sr is None:
-            raise ValueError('No samplerate provided for audio tensor.')
+            raise ValueError('No [input_sr] specified for audio tensor.')
         audio = torchaudio.functional.resample(audio,
                                                orig_freq=input_sr,
                                                new_freq=model.samplerate,
                                                resampling_method="kaiser_window")
     if not track_name:
         track_name = 'audio track'
     audio_dims = audio.dim()
@@ -181,14 +181,33 @@
 
     if output_sr is not None and model.samplerate != output_sr:
         vocals = torchaudio.functional.resample(vocals,
                                                 orig_freq=model.samplerate,
                                                 new_freq=output_sr,
                                                 resampling_method="kaiser_window")
 
-    if save_path:
-        if not save_path.lower().endswith('.wav'):
+    if save_path is not None:
+        if isinstance(save_path, str) and not save_path.lower().endswith('.wav'):
             save_path += '.wav'
         torchaudio.save(save_path, vocals[None], output_sr or model.samplerate)
         print(f'Saved: {save_path}')
 
     return vocals
+
+
+def get_samplerate(audiofile: (str, bytes)) -> (int, None):
+    import re
+    if isinstance(audiofile, str):
+        metadata = subprocess.run(f'ffmpeg -i {audiofile}', capture_output=True, shell=True).stderr.decode()
+    else:
+        p = subprocess.Popen(f'ffmpeg -i -',  stderr=subprocess.PIPE, stdin=subprocess.PIPE, shell=True)
+        try:
+            p.stdin.write(audiofile)
+        except BrokenPipeError:
+            pass
+        finally:
+            metadata = p.communicate()[-1]
+            if metadata is not None:
+                metadata = metadata.decode()
+    sr = re.findall(r'\n.+Stream.+Audio.+\D+(\d+) Hz', metadata)
+    if sr:
+        return int(sr[0])
```

### Comparing `stable-ts-2.6.4/stable_whisper/decode.py` & `stable-ts-2.7.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/enhancement.py` & `stable-ts-2.7.0/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/quantization.py` & `stable-ts-2.7.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/result.py` & `stable-ts-2.7.0/stable_whisper/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,21 @@
         suppress_silence(self, silent_starts, silent_ends, min_word_dur)
         return self
 
     def rescale_time(self, scale_factor: float):
         self.start = round(self.start * scale_factor, 3)
         self.end = round(self.end * scale_factor, 3)
 
+    def clamp_max(self, max_dur: float, clip_start: bool = False):
+        if self.duration > max_dur:
+            if clip_start:
+                self.start = round(self.end - max_dur, 3)
+            else:
+                self.end = round(self.start + max_dur, 3)
+
 
 @dataclass
 class Segment:
     start: float
     end: float
     text: str
     seek: float = None
@@ -800,14 +807,63 @@
 
         """
         if force_len:
             self.merge_all_segments()
         self._split_segments(lambda x: x.get_length_indices(max_chars=max_chars, max_words=max_words), lock=lock)
         return self
 
+    def clamp_max(self, medium_factor: float = 2.5, max_dur: float = None, clip_start: bool = None):
+        """
+
+        Clamp all word durations above certain value.
+
+        Parameters
+        ----------
+        medium_factor: float
+            Clamp durations above ([medium_factor] * medium duration) per segment. (Default: 2.5)
+            If [medium_factor]=None/0 or segment has less than 3 words, it will be ignored and use only [max_dur].
+        max_dur: float
+            Clamp durations above [max_dur]. (Default: None)
+        clip_start: bool
+            Whether to clamp the start of a word. (Default: None)
+            Default only clamps the start of first word and end of last word per segment.
+
+        """
+        if not (medium_factor or max_dur):
+            raise ValueError('At least one of following arguments requires non-zero value: medium_factor; max_dur')
+
+        if not self.has_words:
+            warnings.warn('Cannot clamp due to missing/no word-timestamps')
+            return self
+
+        for seg in self.segments:
+            curr_max_dur = None
+            if medium_factor and len(seg.words) > 2:
+                durations = np.array([word.duration for word in seg.words])
+                print(durations)
+                durations.sort()
+                curr_max_dur = medium_factor * durations[len(durations)//2 + 1]
+
+            if max_dur and (not curr_max_dur or curr_max_dur > max_dur):
+                curr_max_dur = max_dur
+
+            if not curr_max_dur:
+                continue
+
+            if clip_start is None:
+                seg.words[0].clamp_max(curr_max_dur, clip_start=True)
+                seg.words[-1].clamp_max(curr_max_dur, clip_start=False)
+            else:
+                for i, word in enumerate(seg.words):
+                    word.clamp_max(curr_max_dur, clip_start=clip_start)
+
+            seg.update_seg_with_words()
+
+        return self
+
     def regroup(self, regroup_algo: str = None, verbose: bool = False, only_show: bool = False):
         """
 
         Regroup (in-place) all words into segments with more natural boundaries without locking.
 
         Parameters
         ----------
@@ -817,14 +873,15 @@
                 Method keys:
                     sg: split_by_gap
                     sp: split_by_punctuation
                     sl: split_by_length
                     mg: merge_by_gap
                     mp: merge_by_punctuation
                     ms: merge_all_segment
+                    cm: clamp_max
 
                 Metacharacters:
                     = separates a method key and its arguments (not used if no argument)
                     _ separates method keys (after arguments if there are any)
                     + separates arguments for a method key
                     / separates an argument into list of strings
                     * separates an item in list of strings into a nested list of strings
@@ -855,15 +912,16 @@
         if isinstance(regroup_algo, str):
             methods = dict(
                 sg=self.split_by_gap,
                 sp=self.split_by_punctuation,
                 sl=self.split_by_length,
                 mg=self.merge_by_gap,
                 mp=self.merge_by_punctuation,
-                ms=self.merge_all_segments
+                ms=self.merge_all_segments,
+                cm=self.clamp_max
             )
 
             def _to_arg(x: str):
                 if len(x) == 0:
                     return None
                 if '/' in x:
                     return [a.split('*') if '*' in a else a for a in x.split('/')]
@@ -931,14 +989,18 @@
         Restore all values to that in `ori_dict` which is the state at initialization
         or the state store in the `ori_dict` key of the dictionary that initialized this instance.
         """
         self.language = self.ori_dict.get('language')
         segments = self.ori_dict.get('segments')
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
 
+    @property
+    def has_words(self):
+        return all(seg.has_words for seg in self.segments)
+
     to_srt_vtt = result_to_srt_vtt
     to_ass = result_to_ass
     to_tsv = result_to_tsv
     save_as_json = save_as_json
 
 
 class SegmentMatch:
```

### Comparing `stable-ts-2.6.4/stable_whisper/stabilization.py` & `stable-ts-2.7.0/stable_whisper/stabilization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import warnings
-from typing import List, Union, Tuple
+from typing import List, Union, Tuple, Optional
 from itertools import chain
 
 import torch
 import torch.nn.functional as F
 import numpy as np
 
 from whisper.audio import TOKENS_PER_SECOND, SAMPLE_RATE, N_SAMPLES_PER_TOKEN
 
 
+NONVAD_SAMPLE_RATES = (16000,)
+VAD_SAMPLE_RATES = (16000, 8000)
+
+
 def is_ascending_sequence(
         seq: List[Union[int, float]],
         verbose=True
 ) -> bool:
     """
     check if a sequence of numbers are in ascending order
     """
@@ -110,23 +114,33 @@
         elif len(end_match) != 0:
             new_end = silent_starts[end_match[0]]
             if new_end - result_obj.start > min_word_dur:
                 result_obj.end = new_end
 
 
 def standardize_audio(
-        audio: Union[torch.Tensor, np.ndarray, str]
+        audio: Union[torch.Tensor, np.ndarray, str, bytes],
+        resample_sr: Tuple[Optional[int], Union[int, Tuple[int]]] = None
 ) -> torch.Tensor:
-    if isinstance(audio, str):
-        from whisper.audio import load_audio
+    if isinstance(audio, (str, bytes)):
+        from .audio import load_audio
         audio = load_audio(audio)
     if isinstance(audio, np.ndarray):
         audio = torch.from_numpy(audio)
+    audio = audio.float()
+    if resample_sr:
+        in_sr, out_sr = resample_sr
+        if in_sr:
+            if isinstance(out_sr, int):
+                out_sr = [out_sr]
+            if in_sr not in out_sr:
+                from torchaudio.functional import resample
+                audio = resample(audio, in_sr, out_sr[0], resampling_method="kaiser_window")
 
-    return audio.float()
+    return audio
 
 
 def audio2loudness(
         audio_tensor: torch.Tensor
 ) -> (torch.Tensor, None):
     assert audio_tensor.dim() == 1, f'waveform must be 1D, but got {audio_tensor.dim()}D'
     audio_tensor = audio_tensor.abs()
@@ -197,22 +211,24 @@
             else:
                 im.show(im)
         if output:
             print(f'Save: {output}')
 
 
 def wav2mask(
-        audio: (torch.Tensor, np.ndarray, str),
+        audio: (torch.Tensor, np.ndarray, str, bytes),
         q_levels: int = 20,
-        k_size: int = 5
+        k_size: int = 5,
+        sr: int = None
 ) -> (Tuple[torch.Tensor, Tuple[np.ndarray, np.ndarray]], None):
     """
     Generate 1D mask from waveform for suppressing timestamp tokens.
     """
-    loudness_tensor = audio2loudness(standardize_audio(audio))
+    audio = standardize_audio(audio, (sr, NONVAD_SAMPLE_RATES))
+    loudness_tensor = audio2loudness(audio)
     if loudness_tensor is None:
         return
     p = k_size // 2 if k_size else 0
     if p and p < loudness_tensor.shape[-1]:
         assert k_size % 2, f'kernel_size must be odd but got {k_size}'
         mask = torch.avg_pool1d(
             F.pad(
@@ -247,17 +263,16 @@
 
 
 _model_cache = {}
 
 
 def get_vad_silence_func(
         onnx=False,
-        verbose: bool = False
+        verbose: (bool, None) = False
 ):
-    assert SAMPLE_RATE in (16000, 8000), f'silero-vad does not support samplerate: {SAMPLE_RATE}'
     if onnx in _model_cache:
         model, get_ts = _model_cache[onnx]
     else:
         model, utils = torch.hub.load(repo_or_dir='snakers4/silero-vad',
                                       model='silero_vad',
                                       verbose=verbose,
                                       onnx=onnx)
@@ -266,19 +281,20 @@
 
     warnings.filterwarnings('ignore', message=r'operator \(\) profile_node.*', category=UserWarning)
 
     def get_speech_timestamps(wav: torch.Tensor, threshold: float = .35):
         return get_ts(wav, model, threshold, min_speech_duration_ms=100, min_silence_duration_ms=20)
 
     def vad_silence_timing(
-            audio: (torch.Tensor, np.ndarray, str),
-            speech_threshold: float = .35
+            audio: (torch.Tensor, np.ndarray, str, bytes),
+            speech_threshold: float = .35,
+            sr: int = None
     ) -> (Tuple[np.ndarray, np.ndarray], None):
 
-        audio = standardize_audio(audio)
+        audio = standardize_audio(audio, (sr, VAD_SAMPLE_RATES))
 
         total_duration = round(audio.shape[-1] / SAMPLE_RATE, 3)
         if not total_duration:
             return
         ori_t = torch.get_num_threads()
         if verbose is not None:
             print(f'Predicting silences(s) with VAD...\r', end='')
@@ -312,30 +328,30 @@
 
         return silent_starts, silent_ends
 
     return vad_silence_timing
 
 
 def visualize_suppression(
-        audio: Union[torch.Tensor, np.ndarray, str],
+        audio: Union[torch.Tensor, np.ndarray, str, bytes],
         output: str = None,
         q_levels: int = 20,
         k_size: int = 5,
         vad_threshold: float = 0.35,
         vad: bool = False,
         max_width: int = 1500,
         height: int = 200
 ):
     """
 
     Regions on the waveform colored red is where it will be likely be suppressed and marked to as silent.
 
     Parameters
     ----------
-    audio: Union[torch.Tensor, np.ndarray, str]
+    audio: Union[torch.Tensor, np.ndarray, str, bytes]
         Audio to visualize.
     output: str
         Path to save visualization. If none is provided, image will be shown directly via Pillow or opencv-python.
     q_levels: int
         Quantization levels for generating timestamp suppression mask; ignored if [vad]=true. (Default: 20)
         Acts as a threshold to marking sound as silent.
         Fewer levels will increase the threshold of volume at which to mark a sound as silent.
```

### Comparing `stable-ts-2.6.4/stable_whisper/text_output.py` & `stable-ts-2.7.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/timing.py` & `stable-ts-2.7.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/video_output.py` & `stable-ts-2.7.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.4/stable_whisper/whisper_word_level.py` & `stable-ts-2.7.0/stable_whisper/whisper_word_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from .stabilization import get_vad_silence_func, wav2mask, mask2timing, timing2mask
 
 if TYPE_CHECKING:
     from whisper.model import Whisper
 
 __all__ = ['modify_model', 'load_model']
 
-_processes = {}
-
 warnings.filterwarnings('ignore', module='whisper', message='.*Triton.*', category=UserWarning)
 
 
 # modified version of whisper.transcribe.transcribe
 def transcribe_stable(
         model: "Whisper",
         audio: Union[str, np.ndarray, torch.Tensor, bytes],
@@ -58,15 +56,15 @@
         vad_onnx: bool = False,
         min_word_dur: float = 0.1,
         only_voice_freq: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         mel_first: bool = False,
         split_callback: Callable = None,
-        suppress_ts_tokens: bool = True,
+        suppress_ts_tokens: bool = False,
         gap_padding: str = ' ...',
         only_ffmpeg: bool = False,
         **decode_options) \
         -> WhisperResult:
     """
     Transcribe an audio file using Whisper
 
@@ -181,15 +179,15 @@
 
     split_callback: Callable
         Custom callback for grouping tokens up with their corresponding words.
         Takes argument: list of tokens; default tokenizer
         Returns a tuple pair containing: list of words; list of token groups (i.e. each group is list of token(s))
 
     suppress_ts_tokens: bool
-        Whether to use silence mask to suppress silent timestamp tokens during inference. (Default: True)
+        Whether to use silence mask to suppress silent timestamp tokens during inference. (Default: False)
         Reduces hallucinations in some cases,
             but also can reduce 'verbatimness' (i.e. ignores disfluencies and repetitions).
 
     gap_padding: str
         Padding prepend to each segments for word timing alignment. (Default: ' ...')
         Used to reduce the probability of model predicting timestamps earlier than the first utterance.
 
@@ -197,16 +195,15 @@
         Whether to use only FFmpeg (and not yt-dlp) for URls. (Default: False)
 
     decode_options: dict
         Keyword arguments to construct `DecodingOptions` instances
 
     Returns
     -------
-    A dictionary containing the resulting text ("text") and segment-level details ("segments"), and
-    the spoken language ("language"), which is detected when `decode_options["language"]` is None.
+    An instance of WhisperResult.
     """
 
     dtype = torch.float16 if decode_options.get("fp16", True) and not getattr(model, 'dq', False) else torch.float32
     if model.device == torch.device("cpu"):
         if torch.cuda.is_available():
             warnings.warn("Performing inference on CPU when CUDA is available")
         if dtype == torch.float16:
@@ -761,15 +758,15 @@
     parser.add_argument('--suppress_silence', type=str2bool, default=True,
                         help="whether to suppress timestamp where audio is silent at segment-level"
                              "and word-level if [suppress_word_ts]=True")
     parser.add_argument('--suppress_word_ts', type=str2bool, default=True,
                         help="whether to suppress timestamps where audio is silent at word-level; "
                              "ignored if [suppress_silence]=False")
 
-    parser.add_argument('--suppress_ts_tokens', type=str2bool, default=True,
+    parser.add_argument('--suppress_ts_tokens', type=str2bool, default=False,
                         help="whether to use silence mask to suppress silent timestamp tokens during inference; "
                              "increases word accuracy in some cases, but tends reduce 'verbatimness' of the transcript"
                              "ignored if [suppress_silence]=False")
 
     parser.add_argument("--q_levels", type=int, default=20,
                         help="quantization levels for generating timestamp suppression mask; "
                              "acts as a threshold to marking sound as silent;"
```

