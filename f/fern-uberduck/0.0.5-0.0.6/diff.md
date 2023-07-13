# Comparing `tmp/fern_uberduck-0.0.5.tar.gz` & `tmp/fern_uberduck-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_uberduck-0.0.5.tar", max compression
+gzip compressed data, was "fern_uberduck-0.0.6.tar", max compression
```

## Comparing `fern_uberduck-0.0.5.tar` & `fern_uberduck-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     2980 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/README.md
--rw-r--r--   0        0        0      376 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1346 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/__init__.py
--rw-r--r--   0        0        0    41671 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/client.py
--rw-r--r--   0        0        0      348 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      160 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/environment.py
--rw-r--r--   0        0        0      170 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-06 18:46:28.374219 fern_uberduck-0.0.5/src/uberduck/py.typed
--rw-r--r--   0        0        0      162 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/resources/backing_tracks/__init__.py
--rw-r--r--   0        0        0     3080 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/resources/backing_tracks/client.py
--rw-r--r--   0        0        0       65 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/resources/reference_audios/__init__.py
--rw-r--r--   0        0        0     6420 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/resources/reference_audios/client.py
--rw-r--r--   0        0        0     1651 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/__init__.py
--rw-r--r--   0        0        0      830 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/add_reference_audio_response.py
--rw-r--r--   0        0        0      858 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/backing_track_options.py
--rw-r--r--   0        0        0     1238 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/backing_track_options_genre.py
--rw-r--r--   0        0        0      534 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/convert_english_to_ipa_phonemes_request_phones.py
--rw-r--r--   0        0        0      860 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/dataset_speaker.py
--rw-r--r--   0        0        0      206 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/freestyle_request_backing_track.py
--rw-r--r--   0        0        0      796 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/g_2_p_response.py
--rw-r--r--   0        0        0      715 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/get_voice_data_request_mode.py
--rw-r--r--   0        0        0      853 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/get_voices_request_mode.py
--rw-r--r--   0        0        0      843 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/http_validation_error.py
--rw-r--r--   0        0        0      757 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/memberships.py
--rw-r--r--   0        0        0      801 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/mix_item.py
--rw-r--r--   0        0        0      447 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/mix_item_type.py
--rw-r--r--   0        0        0      823 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/reference_audio_response.py
--rw-r--r--   0        0        0      762 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/sample.py
--rw-r--r--   0        0        0      920 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/speak_status_response.py
--rw-r--r--   0        0        0     1174 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/tts_request.py
--rw-r--r--   0        0        0      738 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/uuid.py
--rw-r--r--   0        0        0      788 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/validation_error.py
--rw-r--r--   0        0        0     1628 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/voice_return.py
--rw-r--r--   0        0        0      823 2023-07-06 18:46:28.378219 fern_uberduck-0.0.5/src/uberduck/types/voice_stats.py
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 fern_uberduck-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2980 2023-07-13 17:52:59.598439 fern_uberduck-0.0.6/README.md
+-rw-r--r--   0        0        0      376 2023-07-13 17:52:59.598439 fern_uberduck-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1346 2023-07-13 17:52:59.598439 fern_uberduck-0.0.6/src/uberduck/__init__.py
+-rw-r--r--   0        0        0    41671 2023-07-13 17:52:59.598439 fern_uberduck-0.0.6/src/uberduck/client.py
+-rw-r--r--   0        0        0      348 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      160 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/environment.py
+-rw-r--r--   0        0        0      170 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/py.typed
+-rw-r--r--   0        0        0      162 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/resources/backing_tracks/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/resources/backing_tracks/client.py
+-rw-r--r--   0        0        0       65 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/resources/reference_audios/__init__.py
+-rw-r--r--   0        0        0     6420 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/resources/reference_audios/client.py
+-rw-r--r--   0        0        0     1651 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/add_reference_audio_response.py
+-rw-r--r--   0        0        0      858 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/backing_track_options.py
+-rw-r--r--   0        0        0     1238 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/backing_track_options_genre.py
+-rw-r--r--   0        0        0      534 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/convert_english_to_ipa_phonemes_request_phones.py
+-rw-r--r--   0        0        0      860 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/dataset_speaker.py
+-rw-r--r--   0        0        0      206 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/freestyle_request_backing_track.py
+-rw-r--r--   0        0        0      796 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/g_2_p_response.py
+-rw-r--r--   0        0        0      715 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/get_voice_data_request_mode.py
+-rw-r--r--   0        0        0      853 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/get_voices_request_mode.py
+-rw-r--r--   0        0        0      843 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/http_validation_error.py
+-rw-r--r--   0        0        0      757 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/memberships.py
+-rw-r--r--   0        0        0      801 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/mix_item.py
+-rw-r--r--   0        0        0      447 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/mix_item_type.py
+-rw-r--r--   0        0        0      823 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/reference_audio_response.py
+-rw-r--r--   0        0        0      762 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/sample.py
+-rw-r--r--   0        0        0      920 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/speak_status_response.py
+-rw-r--r--   0        0        0     1174 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/tts_request.py
+-rw-r--r--   0        0        0      738 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/uuid.py
+-rw-r--r--   0        0        0      788 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/validation_error.py
+-rw-r--r--   0        0        0     1628 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/voice_return.py
+-rw-r--r--   0        0        0      823 2023-07-13 17:52:59.602439 fern_uberduck-0.0.6/src/uberduck/types/voice_stats.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 fern_uberduck-0.0.6/PKG-INFO
```

### Comparing `fern_uberduck-0.0.5/README.md` & `fern_uberduck-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/__init__.py` & `fern_uberduck-0.0.6/src/uberduck/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/client.py` & `fern_uberduck-0.0.6/src/uberduck/client.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/core/datetime_utils.py` & `fern_uberduck-0.0.6/src/uberduck/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/core/jsonable_encoder.py` & `fern_uberduck-0.0.6/src/uberduck/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/resources/backing_tracks/client.py` & `fern_uberduck-0.0.6/src/uberduck/resources/backing_tracks/client.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/resources/reference_audios/client.py` & `fern_uberduck-0.0.6/src/uberduck/resources/reference_audios/client.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/__init__.py` & `fern_uberduck-0.0.6/src/uberduck/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/add_reference_audio_response.py` & `fern_uberduck-0.0.6/src/uberduck/types/add_reference_audio_response.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/backing_track_options.py` & `fern_uberduck-0.0.6/src/uberduck/types/backing_track_options.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/backing_track_options_genre.py` & `fern_uberduck-0.0.6/src/uberduck/types/backing_track_options_genre.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/convert_english_to_ipa_phonemes_request_phones.py` & `fern_uberduck-0.0.6/src/uberduck/types/convert_english_to_ipa_phonemes_request_phones.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/dataset_speaker.py` & `fern_uberduck-0.0.6/src/uberduck/types/dataset_speaker.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/g_2_p_response.py` & `fern_uberduck-0.0.6/src/uberduck/types/g_2_p_response.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/get_voice_data_request_mode.py` & `fern_uberduck-0.0.6/src/uberduck/types/get_voice_data_request_mode.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/get_voices_request_mode.py` & `fern_uberduck-0.0.6/src/uberduck/types/get_voices_request_mode.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/http_validation_error.py` & `fern_uberduck-0.0.6/src/uberduck/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/memberships.py` & `fern_uberduck-0.0.6/src/uberduck/types/memberships.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/mix_item.py` & `fern_uberduck-0.0.6/src/uberduck/types/mix_item.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/reference_audio_response.py` & `fern_uberduck-0.0.6/src/uberduck/types/reference_audio_response.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/sample.py` & `fern_uberduck-0.0.6/src/uberduck/types/sample.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/speak_status_response.py` & `fern_uberduck-0.0.6/src/uberduck/types/speak_status_response.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/tts_request.py` & `fern_uberduck-0.0.6/src/uberduck/types/tts_request.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/uuid.py` & `fern_uberduck-0.0.6/src/uberduck/types/uuid.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/validation_error.py` & `fern_uberduck-0.0.6/src/uberduck/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/voice_return.py` & `fern_uberduck-0.0.6/src/uberduck/types/voice_return.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/src/uberduck/types/voice_stats.py` & `fern_uberduck-0.0.6/src/uberduck/types/voice_stats.py`

 * *Files identical despite different names*

### Comparing `fern_uberduck-0.0.5/PKG-INFO` & `fern_uberduck-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-uberduck
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

