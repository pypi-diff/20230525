# Comparing `tmp/elevenlabslib-0.8.1.tar.gz` & `tmp/elevenlabslib-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.8.1.tar", last modified: Wed May 24 13:43:50 2023, max compression
+gzip compressed data, was "elevenlabslib-0.8.2.tar", last modified: Wed May 24 22:44:06 2023, max compression
```

## Comparing `elevenlabslib-0.8.1.tar` & `elevenlabslib-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.283703 elevenlabslib-0.8.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     3163 2023-05-24 13:43:50.282703 elevenlabslib-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2508 2023-05-21 23:44:11.000000 elevenlabslib-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.277704 elevenlabslib-0.8.1/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    18927 2023-05-21 19:46:46.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    37135 2023-05-24 13:39:53.000000 elevenlabslib-0.8.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.8.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     6285 2023-05-21 19:46:46.000000 elevenlabslib-0.8.1/elevenlabslib/helpers.py
--rw-rw-rw-   0        0        0     3738 2023-05-24 13:33:48.000000 elevenlabslib-0.8.1/elevenlabslib/linuxBugTest.py
--rw-rw-rw-   0        0        0     2291 2023-05-23 14:40:59.000000 elevenlabslib-0.8.1/elevenlabslib/linuxtest2.py
-drwxrwxrwx   0        0        0        0 2023-05-24 13:43:50.281702 elevenlabslib-0.8.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     3163 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-24 13:43:50.000000 elevenlabslib-0.8.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-24 13:41:01.000000 elevenlabslib-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 13:43:50.283703 elevenlabslib-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 22:44:06.191580 elevenlabslib-0.8.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0     3169 2023-05-24 22:44:06.191080 elevenlabslib-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-05-24 22:13:31.000000 elevenlabslib-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 22:44:06.185581 elevenlabslib-0.8.2/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.8.2/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.8.2/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    18927 2023-05-21 19:46:46.000000 elevenlabslib-0.8.2/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    37816 2023-05-24 22:10:06.000000 elevenlabslib-0.8.2/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.8.2/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-05-21 19:46:46.000000 elevenlabslib-0.8.2/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 22:44:06.190079 elevenlabslib-0.8.2/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3169 2023-05-24 22:44:06.000000 elevenlabslib-0.8.2/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-24 22:44:06.000000 elevenlabslib-0.8.2/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 22:44:06.000000 elevenlabslib-0.8.2/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-24 22:44:06.000000 elevenlabslib-0.8.2/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 22:44:06.000000 elevenlabslib-0.8.2/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-24 22:43:33.000000 elevenlabslib-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 22:44:06.191580 elevenlabslib-0.8.2/setup.cfg
```

### Comparing `elevenlabslib-0.8.1/LICENSE` & `elevenlabslib-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/PKG-INFO` & `elevenlabslib-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.8.1
+Version: 0.8.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,15 +53,15 @@
 from elevenlabslib import *
 
 user = ElevenLabsUser("API_KEY")
 voice = user.get_voices_by_name("Rachel")[0]  # This is a list because multiple voices can have the same name
 
 voice.play_preview(playInBackground=False)
 
-voice.generate_and_play_audio("Test.", playInBackground=False)
+voice.generate_play_audio("Test.", playInBackground=False)
 
-for historyItem in user.get_history_items():
+for historyItem in user.get_history_items_paginated():
     if historyItem.text == "Test.":
         # The first items are the newest, so we can stop as soon as we find one.
         historyItem.delete()
         break
 ```
```

### Comparing `elevenlabslib-0.8.1/README.md` & `elevenlabslib-0.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from elevenlabslib import *
 
 user = ElevenLabsUser("API_KEY")
 voice = user.get_voices_by_name("Rachel")[0]  # This is a list because multiple voices can have the same name
 
 voice.play_preview(playInBackground=False)
 
-voice.generate_and_play_audio("Test.", playInBackground=False)
+voice.generate_play_audio("Test.", playInBackground=False)
 
-for historyItem in user.get_history_items():
+for historyItem in user.get_history_items_paginated():
     if historyItem.text == "Test.":
         # The first items are the newest, so we can stop as soon as we find one.
         historyItem.delete()
         break
 ```
```

### Comparing `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.8.2/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.8.2/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.8.2/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.8.2/elevenlabslib/ElevenLabsVoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+import concurrent.futures
 import os
 import queue
 
 import threading
+from concurrent.futures import Future
 from typing import Optional, Tuple, Any
 from warnings import warn
 
 import soundfile as sf
 import sounddevice as sd
 
 from typing import TYPE_CHECKING
@@ -252,17 +254,22 @@
                                 stability:Optional[float]=None, similarity_boost:Optional[float]=None,
                                 onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1") -> bytes:
         warn("This function is deprecated. Please use generate_play_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
         audioData = self.generate_audio_bytes(prompt, stability, similarity_boost, model_id)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
         return audioData
 
-    def generate_and_stream_audio(self, prompt:str, portaudioDeviceID:Optional[int] = None,
+    def generate_and_stream_audio(self, *args, **kwargs) -> str:
+        warn("This function is deprecated. Please use generate_stream_audio instead, which returns both the historyID and a future for the audio OutputStream (for playback control).")
+        return self.generate_stream_audio(*args, **kwargs)[0]
+
+    def generate_stream_audio(self, prompt:str, portaudioDeviceID:Optional[int] = None,
                                   stability:Optional[float]=None, similarity_boost:Optional[float]=None, streamInBackground=False,
-                                  onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> str:
+                                  onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0) -> tuple[
+        str, Future[Any]]:
         """
 
         Note:
             The latencyOptimizationLevel ranges from 0 to 4. Each level trades off some more quality for speed.
 
             The levels are as follows:
                 - 0: Normal, no optimizations applied
@@ -283,30 +290,30 @@
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
             latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply.
 
         Returns:
-            The historyID for the newly created item.
+            A tuple consisting of the historyID for the newly created item and a future which will hold the audio OutputStream (to control playback)
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         path = "/text-to-speech/" + self._voiceID + "/stream"
 
         streamedResponse = requests.post(api_endpoint + path, headers=self._linkedUser.headers, json=payload, stream=True, params={"optimize_streaming_latency":latencyOptimizationLevel})
 
         streamer = _AudioChunkStreamer(portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
-
+        audioStreamFuture = concurrent.futures.Future()
         if streamInBackground:
-            mainThread = threading.Thread(target=streamer.begin_streaming, args=(streamedResponse,))
+            mainThread = threading.Thread(target=streamer.begin_streaming, args=(streamedResponse,audioStreamFuture))
             mainThread.start()
         else:
-            streamer.begin_streaming(streamedResponse)
+            streamer.begin_streaming(streamedResponse,audioStreamFuture)
 
-        return streamedResponse.headers["history-item-id"]
+        return streamedResponse.headers["history-item-id"], audioStreamFuture
 
 
     def get_preview_url(self) -> str|None:
         """
         Returns:
             str|None: The preview URL of the voice, or None if it hasn't been generated.
         """
@@ -529,15 +536,15 @@
             "headerReadyEvent": threading.Event(),
             "soundFileReadyEvent": threading.Event(),
             "downloadDoneEvent": threading.Event(),
             "blockDataAvailable": threading.Event(),
             "playbackStartFired": threading.Event()
         }
 
-    def begin_streaming(self, streamedResponse:requests.Response):
+    def begin_streaming(self, streamedResponse:requests.Response, future:concurrent.futures.Future):
         # Clean all the buffers and reset all events.
         self._q = queue.Queue()
         self._bytesFile = io.BytesIO()
         self._bytesSoundFile: Optional[sf.SoundFile] = None  # Needs to be created later.
         for eventName, event in self._events.items():
             event.clear()
 
@@ -563,14 +570,15 @@
                 self._events["headerReadyEvent"].clear()
                 self._events["soundFileReadyEvent"].set()
 
         stream = sd.RawOutputStream(
             samplerate=self._bytesSoundFile.samplerate, blocksize=_playbackBlockSize,
             device=self._deviceID, channels=self._bytesSoundFile.channels, dtype=_defaultDType,
             callback=self._stream_playback_callback, finished_callback=self._events["playbackFinishedEvent"].set)
+        future.set_result(stream)
         logging.debug("Starting playback...")
         with stream:
             while True:
                 data = self._get_data_from_download_thread()
                 if len(data) == _playbackBlockSize*self._frameSize:
                     logging.debug("Putting " + str(len(data)) + " bytes in queue.")
                     self._q.put(data)
```

### Comparing `elevenlabslib-0.8.1/elevenlabslib/__init__.py` & `elevenlabslib-0.8.2/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/elevenlabslib/helpers.py` & `elevenlabslib-0.8.2/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.8.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.8.2/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.8.1
+Version: 0.8.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,15 +53,15 @@
 from elevenlabslib import *
 
 user = ElevenLabsUser("API_KEY")
 voice = user.get_voices_by_name("Rachel")[0]  # This is a list because multiple voices can have the same name
 
 voice.play_preview(playInBackground=False)
 
-voice.generate_and_play_audio("Test.", playInBackground=False)
+voice.generate_play_audio("Test.", playInBackground=False)
 
-for historyItem in user.get_history_items():
+for historyItem in user.get_history_items_paginated():
     if historyItem.text == "Test.":
         # The first items are the newest, so we can stop as soon as we find one.
         historyItem.delete()
         break
 ```
```

### Comparing `elevenlabslib-0.8.1/pyproject.toml` & `elevenlabslib-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

