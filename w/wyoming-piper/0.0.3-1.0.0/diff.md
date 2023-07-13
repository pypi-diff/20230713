# Comparing `tmp/wyoming_piper-0.0.3.tar.gz` & `tmp/wyoming_piper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_piper-0.0.3.tar", last modified: Fri May 12 20:29:57 2023, max compression
+gzip compressed data, was "wyoming_piper-1.0.0.tar", last modified: Thu Jul 13 16:27:40 2023, max compression
```

## Comparing `wyoming_piper-0.0.3.tar` & `wyoming_piper-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1205 2023-05-10 19:58:40.000000 wyoming_piper-0.0.3/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/wyoming_piper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4503 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-0.0.3/wyoming_piper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     2603 2023-05-10 20:32:19.000000 wyoming_piper-0.0.3/wyoming_piper/download.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-0.0.3/wyoming_piper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3689 2023-05-11 15:57:03.000000 wyoming_piper-0.0.3/wyoming_piper/handler.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     9186 2023-05-12 17:05:02.000000 wyoming_piper-0.0.3/wyoming_piper/voice_hashes.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-12 20:29:57.984187 wyoming_piper-0.0.3/wyoming_piper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      404 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-05-12 20:29:57.000000 wyoming_piper-0.0.3/wyoming_piper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       59 2023-07-13 15:51:03.000000 wyoming_piper-1.0.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-10 21:09:46.000000 wyoming_piper-1.0.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1378 2023-07-13 15:52:43.000000 wyoming_piper-1.0.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/wyoming_piper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       32 2023-04-21 15:28:34.000000 wyoming_piper-1.0.0/wyoming_piper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4663 2023-07-13 16:26:55.000000 wyoming_piper-1.0.0/wyoming_piper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_piper-1.0.0/wyoming_piper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3866 2023-07-13 14:58:56.000000 wyoming_piper-1.0.0/wyoming_piper/download.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-10 19:58:23.000000 wyoming_piper-1.0.0/wyoming_piper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4802 2023-07-13 16:05:48.000000 wyoming_piper-1.0.0/wyoming_piper/handler.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4280 2023-07-13 15:02:06.000000 wyoming_piper-1.0.0/wyoming_piper/process.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)   116115 2023-07-13 15:29:35.000000 wyoming_piper-1.0.0/wyoming_piper/voices.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-13 16:27:40.031119 wyoming_piper-1.0.0/wyoming_piper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      666 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      425 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       14 2023-07-13 16:27:40.000000 wyoming_piper-1.0.0/wyoming_piper.egg-info/top_level.txt
```

### Comparing `wyoming_piper-0.0.3/PKG-INFO` & `wyoming_piper-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming_piper
-Version: 0.0.3
+Version: 1.0.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

### Comparing `wyoming_piper-0.0.3/wyoming_piper/__main__.py` & `wyoming_piper-1.0.0/wyoming_piper/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 #!/usr/bin/env python3
 import argparse
 import asyncio
-import json
 import logging
-import tempfile
 from functools import partial
-from pathlib import Path
-from typing import Optional
+from typing import Any, Dict
 
-from wyoming.info import Attribution, Info, TtsProgram, TtsVoice
+from wyoming.info import Attribution, Info, TtsProgram, TtsVoice, TtsVoiceSpeaker
 from wyoming.server import AsyncServer
 
-from .download import download_voice, find_voice
+from .download import get_voices
 from .handler import PiperEventHandler
+from .process import PiperProcessManager
 
 _LOGGER = logging.getLogger(__name__)
 
 
 async def main() -> None:
     """Main entry point."""
     parser = argparse.ArgumentParser()
@@ -24,124 +22,126 @@
         "--piper",
         required=True,
         help="Path to piper executable",
     )
     parser.add_argument(
         "--voice",
         required=True,
-        help="Name of Piper voice to use (e.g., en-us-ryan-low)",
+        help="Default Piper voice to use (e.g., en_US-lessac-medium)",
     )
-    parser.add_argument("--uri", required=True, help="unix:// or tcp://")
+    parser.add_argument("--uri", default="stdio://", help="unix:// or tcp://")
     parser.add_argument(
         "--data-dir",
         required=True,
         action="append",
         help="Data directory to check for downloaded models",
     )
     parser.add_argument(
         "--download-dir",
         required=True,
         help="Directory to download voices into",
     )
     #
-    parser.add_argument("--speaker", type=int, help="Id of speaker (default: 0)")
+    parser.add_argument("--speaker", type=int, help="Id of speaker for default voice")
     parser.add_argument("--noise-scale", type=float, help="Generator noise")
     parser.add_argument("--length-scale", type=float, help="Phoneme length")
     parser.add_argument("--noise-w", type=float, help="Phoneme width noise")
     #
     parser.add_argument(
         "--auto-punctuation", default=".?!", help="Automatically add punctuation"
     )
     parser.add_argument("--samples-per-chunk", type=int, default=1024)
+    parser.add_argument(
+        "--max-piper-procs",
+        type=int,
+        default=1,
+        help="Maximum number of piper process to run simultaneously",
+    )
     #
     parser.add_argument("--debug", action="store_true", help="Log DEBUG messages")
     args = parser.parse_args()
 
     logging.basicConfig(level=logging.DEBUG if args.debug else logging.INFO)
 
-    # Look for voice
-    voice_onnx: Optional[Path] = None
-    for data_dir in args.data_dir:
-        voice_onnx = find_voice(args.voice, data_dir)
-        if voice_onnx is not None:
-            break
-
-    if voice_onnx is None:
-        _LOGGER.info("Downloading %s to %s", args.voice, args.download_dir)
-        voice_onnx = download_voice(args.voice, args.download_dir)
-
     # Load voice info
-    voice_config_path = f"{voice_onnx}.json"
-    with open(voice_config_path, "r", encoding="utf-8") as voice_config_file:
-        voice_config = json.load(voice_config_file)
+    voices_info = get_voices()
+
+    # Resolve aliases for backwards compatibility with old voice names
+    aliases_info: Dict[str, Any] = {}
+    for voice_info in voices_info.values():
+        for voice_alias in voice_info.get("aliases", []):
+            aliases_info[voice_alias] = voice_info
+
+    voices_info.update(aliases_info)
 
-    num_speakers = voice_config["num_speakers"]
-    voice_language = voice_config["espeak"]["voice"]
     wyoming_info = Info(
         tts=[
             TtsProgram(
                 name="piper",
+                description="A fast, local, neural text to speech engine",
                 attribution=Attribution(
                     name="rhasspy", url="https://github.com/rhasspy/piper"
                 ),
                 installed=True,
                 voices=[
                     TtsVoice(
-                        name=args.voice,
+                        name=voice_name,
+                        description=get_description(voice_info),
                         attribution=Attribution(
                             name="rhasspy", url="https://github.com/rhasspy/piper"
                         ),
                         installed=True,
-                        languages=[voice_language],
+                        languages=[voice_info["language"]["code"]],
+                        #
+                        # Don't send speakers for now because it overflows StreamReader buffers
+                        # speakers=[
+                        #     TtsVoiceSpeaker(name=speaker_name)
+                        #     for speaker_name in voice_info["speaker_id_map"]
+                        # ]
+                        # if voice_info.get("speaker_id_map")
+                        # else None,
                     )
+                    for voice_name, voice_info in voices_info.items()
                 ],
             )
         ],
     )
 
+    process_manager = PiperProcessManager(args, voices_info)
+
+    # Make sure default voice is loaded.
+    # Other voices will be loaded on-demand.
+    await process_manager.get_process(args.voice)
+
+    # Start server
     server = AsyncServer.from_uri(args.uri)
 
-    with tempfile.TemporaryDirectory() as temp_dir:
-        piper_args = [
-            "--model",
-            str(voice_onnx),
-            "--output_dir",
-            str(temp_dir),
-        ]
-
-        if (args.speaker is not None) and (num_speakers > 1):
-            piper_args.extend(["--speaker", str(args.speaker)])
-
-        if args.noise_scale:
-            piper_args.extend(["--noise-scale", str(args.noise_scale)])
-
-        if args.length_scale:
-            piper_args.extend(["--length-scale", str(args.length_scale)])
-
-        if args.noise_w:
-            piper_args.extend(["--noise-w", str(args.noise_w)])
-
-        proc = await asyncio.create_subprocess_exec(
-            args.piper,
-            *piper_args,
-            stdin=asyncio.subprocess.PIPE,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.DEVNULL,
+    _LOGGER.info("Ready")
+    await server.run(
+        partial(
+            PiperEventHandler,
+            wyoming_info,
+            args,
+            process_manager,
         )
+    )
 
-        _LOGGER.info("Ready")
-        proc_lock = asyncio.Lock()
-        await server.run(
-            partial(
-                PiperEventHandler,
-                wyoming_info,
-                args,
-                proc,
-                proc_lock,
-            )
-        )
+
+# -----------------------------------------------------------------------------
+
+
+def get_description(voice_info: Dict[str, Any]):
+    """Get a human readable description for a voice."""
+    name = voice_info["name"]
+    name = " ".join(name.split("_"))
+    quality = voice_info["quality"]
+
+    return f"{name} ({quality})"
 
 
 # -----------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    try:
+        asyncio.run(main())
+    except KeyboardInterrupt:
+        pass
```

### Comparing `wyoming_piper-0.0.3/wyoming_piper/const.py` & `wyoming_piper-1.0.0/wyoming_piper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.3/wyoming_piper/file_hash.py` & `wyoming_piper-1.0.0/wyoming_piper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_piper-0.0.3/wyoming_piper/handler.py` & `wyoming_piper-1.0.0/wyoming_piper/handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Event handler for clients of the server."""
 import argparse
-import asyncio
+import json
 import logging
 import math
 import os
 import wave
+from typing import Optional
 
 from wyoming.audio import AudioChunk, AudioStart, AudioStop
 from wyoming.event import Event
 from wyoming.info import Describe, Info
 from wyoming.server import AsyncEventHandler
 from wyoming.tts import Synthesize
 
+from .process import PiperProcessManager
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class PiperEventHandler(AsyncEventHandler):
     def __init__(
         self,
         wyoming_info: Info,
         cli_args: argparse.Namespace,
-        piper_proc: asyncio.subprocess.Process,
-        piper_proc_lock: asyncio.Lock,
+        process_manager: PiperProcessManager,
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
 
         self.cli_args = cli_args
         self.wyoming_info_event = wyoming_info.event()
-        self.piper_proc = piper_proc
-        self.piper_proc_lock = piper_proc_lock
+        self.process_manager = process_manager
 
     async def handle_event(self, event: Event) -> bool:
         if Describe.is_type(event.type):
             await self.write_event(self.wyoming_info_event)
             _LOGGER.debug("Sent info")
             return True
 
@@ -55,56 +56,86 @@
                 if text[-1] == punc_char:
                     has_punctuation = True
                     break
 
             if not has_punctuation:
                 text = text + self.cli_args.auto_punctuation[0]
 
-        async with self.piper_proc_lock:
+        async with self.process_manager.processes_lock:
             _LOGGER.debug("synthesize: raw_text=%s, text='%s'", raw_text, text)
+            voice_name: Optional[str] = None
+            voice_speaker: Optional[str] = None
+            if synthesize.voice is not None:
+                voice_name = synthesize.voice.name
+                voice_speaker = synthesize.voice.speaker
+
+            piper_proc = await self.process_manager.get_process(voice_name=voice_name)
+
+            assert piper_proc.proc.stdin is not None
+            assert piper_proc.proc.stdout is not None
+
+            # JSON in, file path out
+            input_obj = {"text": text}
+            if voice_speaker is not None:
+                speaker_id_map = piper_proc.config.get("speaker_id_map", {})
+                speaker_id = speaker_id_map.get(voice_speaker)
+                if speaker_id is None:
+                    try:
+                        # Try to interpret as an id
+                        speaker_id = int(voice_speaker)
+                    except ValueError:
+                        pass
+
+                if speaker_id is not None:
+                    input_obj["speaker_id"] = speaker_id
+                else:
+                    _LOGGER.warning(
+                        "No speaker '%s' for voice '%s'", voice_speaker, voice_name
+                    )
 
-            # Text in, file path out
-            self.piper_proc.stdin.write((text + "\n").encode())
-            await self.piper_proc.stdin.drain()
+            piper_proc.proc.stdin.write(
+                (json.dumps(input_obj, ensure_ascii=False) + "\n").encode()
+            )
+            await piper_proc.proc.stdin.drain()
 
-            output_path = (await self.piper_proc.stdout.readline()).decode().strip()
+            output_path = (await piper_proc.proc.stdout.readline()).decode().strip()
             _LOGGER.debug(output_path)
 
-            wav_file: wave.Wave_read = wave.open(output_path, "rb")
-            with wav_file:
-                rate = wav_file.getframerate()
-                width = wav_file.getsampwidth()
-                channels = wav_file.getnchannels()
-
+        wav_file: wave.Wave_read = wave.open(output_path, "rb")
+        with wav_file:
+            rate = wav_file.getframerate()
+            width = wav_file.getsampwidth()
+            channels = wav_file.getnchannels()
+
+            await self.write_event(
+                AudioStart(
+                    rate=rate,
+                    width=width,
+                    channels=channels,
+                ).event(),
+            )
+
+            # Audio
+            audio_bytes = wav_file.readframes(wav_file.getnframes())
+            bytes_per_sample = width * channels
+            bytes_per_chunk = bytes_per_sample * self.cli_args.samples_per_chunk
+            num_chunks = int(math.ceil(len(audio_bytes) / bytes_per_chunk))
+
+            # Split into chunks
+            for i in range(num_chunks):
+                offset = i * bytes_per_chunk
+                chunk = audio_bytes[offset : offset + bytes_per_chunk]
                 await self.write_event(
-                    AudioStart(
+                    AudioChunk(
+                        audio=chunk,
                         rate=rate,
                         width=width,
                         channels=channels,
                     ).event(),
                 )
 
-                # Audio
-                audio_bytes = wav_file.readframes(wav_file.getnframes())
-                bytes_per_sample = width * channels
-                bytes_per_chunk = bytes_per_sample * self.cli_args.samples_per_chunk
-                num_chunks = int(math.ceil(len(audio_bytes) / bytes_per_chunk))
-
-                # Split into chunks
-                for i in range(num_chunks):
-                    offset = i * bytes_per_chunk
-                    chunk = audio_bytes[offset : offset + bytes_per_chunk]
-                    await self.write_event(
-                        AudioChunk(
-                            audio=chunk,
-                            rate=rate,
-                            width=width,
-                            channels=channels,
-                        ).event(),
-                    )
-
-            await self.write_event(AudioStop().event())
-            _LOGGER.debug("Completed request")
+        await self.write_event(AudioStop().event())
+        _LOGGER.debug("Completed request")
 
-            os.unlink(output_path)
+        os.unlink(output_path)
 
         return True
```

### Comparing `wyoming_piper-0.0.3/wyoming_piper.egg-info/PKG-INFO` & `wyoming_piper-1.0.0/wyoming_piper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wyoming-piper
-Version: 0.0.3
+Version: 1.0.0
 Summary: Wyoming Server for Piper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Description: UNKNOWN
 Keywords: rhasspy wyoming piper
```

