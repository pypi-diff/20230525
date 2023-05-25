# Comparing `tmp/neon_speech-3.3.2a5-py3-none-any.whl.zip` & `tmp/neon_speech-3.3.2a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,14 @@
-Zip file size: 23742 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-May-24 19:42 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2914 b- defN 23-May-24 19:42 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-May-24 19:42 neon_speech/cli.py
--rw-r--r--  2.0 unx     9921 b- defN 23-May-24 19:42 neon_speech/listener.py
--rw-r--r--  2.0 unx     5107 b- defN 23-May-24 19:42 neon_speech/mic.py
--rw-r--r--  2.0 unx    21917 b- defN 23-May-24 19:42 neon_speech/service.py
--rw-r--r--  2.0 unx     4478 b- defN 23-May-24 19:42 neon_speech/stt.py
--rw-r--r--  2.0 unx     4285 b- defN 23-May-24 19:42 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2587 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1143 b- defN 23-May-24 19:42 neon_speech-3.3.2a5.dist-info/RECORD
-14 files, 61117 bytes uncompressed, 21850 bytes compressed:  64.2%
+Zip file size: 17849 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-25 16:29 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2914 b- defN 23-May-25 16:29 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-May-25 16:29 neon_speech/cli.py
+-rw-r--r--  2.0 unx    21078 b- defN 23-May-25 16:29 neon_speech/service.py
+-rw-r--r--  2.0 unx     4459 b- defN 23-May-25 16:29 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4395 b- defN 23-May-25 16:29 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2451 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      988 b- defN 23-May-25 16:29 neon_speech-3.3.2a6.dist-info/RECORD
+12 files, 45050 bytes uncompressed, 16191 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -3,41 +3,35 @@
 
 Filename: neon_speech/__main__.py
 Comment: 
 
 Filename: neon_speech/cli.py
 Comment: 
 
-Filename: neon_speech/listener.py
-Comment: 
-
-Filename: neon_speech/mic.py
-Comment: 
-
 Filename: neon_speech/service.py
 Comment: 
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/LICENSE.md
+Filename: neon_speech-3.3.2a6.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/METADATA
+Filename: neon_speech-3.3.2a6.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/WHEEL
+Filename: neon_speech-3.3.2a6.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/entry_points.txt
+Filename: neon_speech-3.3.2a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/top_level.txt
+Filename: neon_speech-3.3.2a6.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.3.2a5.dist-info/RECORD
+Filename: neon_speech-3.3.2a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/service.py

```diff
@@ -23,43 +23,49 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import os
-from tempfile import mkstemp
+import ovos_dinkum_listener.plugins
 
-from threading import Thread, Lock
+from tempfile import mkstemp
+from threading import Lock, Event
 from time import time
-
-from ovos_listener.mic import ListeningMode
-from ovos_utils.process_utils import StatusCallbackMap, ProcessStatus
 from pydub import AudioSegment
 from speech_recognition import AudioData
-
 from neon_utils.file_utils import decode_base64_string_to_file
-from neon_utils.messagebus_utils import get_messagebus
 from ovos_utils.log import LOG
 from neon_utils.configuration_utils import get_neon_user_config
 from neon_utils.user_utils import apply_local_user_profile_updates
-from ovos_utils.json_helper import merge_dict
 from ovos_bus_client import Message
+from ovos_config.config import update_mycroft_config
+from ovos_dinkum_listener.service import OVOSDinkumVoiceService
+from ovos_dinkum_listener.voice_loop.voice_loop import ListeningMode
 
-from ovos_listener.service import SpeechService
-from ovos_config.config import Configuration, update_mycroft_config
-
-from neon_speech.listener import NeonRecognizerLoop
 from neon_speech.stt import STTFactory
 
+ovos_dinkum_listener.plugins.OVOSSTTFactory = STTFactory
+
+_SERVICE_READY = Event()
+
 
 def on_ready():
     LOG.info('Speech client is ready.')
 
 
+def wrapped_ready_hook(ready_hook: callable):
+    def wrapper():
+        _SERVICE_READY.set()
+        LOG.info(f"Set Ready event")
+        ready_hook()
+    return wrapper
+
+
 def on_stopping():
     LOG.info('Speech service is shutting down...')
 
 
 def on_error(e='Unknown'):
     LOG.error('Audio service failed to launch ({}).'.format(repr(e)))
 
@@ -68,15 +74,15 @@
     LOG.debug("Speech client alive")
 
 
 def on_started():
     LOG.debug("Speech client started")
 
 
-class NeonSpeechClient(SpeechService):
+class NeonSpeechClient(OVOSDinkumVoiceService):
     def __init__(self, ready_hook=on_ready, error_hook=on_error,
                  stopping_hook=on_stopping, alive_hook=on_alive,
                  started_hook=on_started, watchdog=lambda: None,
                  speech_config=None, daemonic=False, bus=None):
         """
         Creates a Speech service thread
         :param ready_hook: function callback when service is ready
@@ -89,53 +95,47 @@
         :param bus: Messagebus client
         """
         if speech_config:
             LOG.info("Updating global config with passed config")
             from neon_speech.utils import patch_config
             patch_config(speech_config)
         # Don't init SpeechClient, because we're overriding self.loop
-        Thread.__init__(self)
+        OVOSDinkumVoiceService.__init__(self,
+                                        on_ready=wrapped_ready_hook(ready_hook),
+                                        on_error=error_hook,
+                                        on_stopping=stopping_hook,
+                                        on_alive=alive_hook,
+                                        on_started=started_hook,
+                                        bus=bus,
+                                        watchdog=watchdog)
         self.daemon = daemonic
-        # Init messagebus and handlers
-        self.bus = bus or get_messagebus()
+        self.config.bus = self.bus
         from neon_utils.signal_utils import init_signal_handlers, \
             init_signal_bus
         init_signal_bus(self.bus)
         init_signal_handlers()
 
         self._default_user = get_neon_user_config()
         self._default_user['user']['username'] = "local"
 
-        self.config = Configuration()
         self.lock = Lock()
 
-        callbacks = StatusCallbackMap(on_ready=ready_hook, on_error=error_hook,
-                                      on_stopping=stopping_hook,
-                                      on_alive=alive_hook,
-                                      on_started=started_hook)
-        self.status = ProcessStatus('voice', self.bus, callbacks)
-        self.status.set_started()
-        self.status.bind(self.bus)
-        self.loop = NeonRecognizerLoop(self.bus, watchdog)
-        self.connect_loop_events()
-        self.connect_bus_events()
         if self.config.get('listener', {}).get('enable_stt_api', True):
             self.api_stt = STTFactory.create(config=self.config,
                                              results_event=None)
         else:
             LOG.info("Skipping api_stt init")
             self.api_stt = None
 
     def shutdown(self):
         LOG.info("Shutting Down")
-        self.status.set_stopping()
-        self.loop.stop()
+        self.stop()
 
-    def connect_bus_events(self):
-        SpeechService.connect_bus_events(self)
+    def register_event_handlers(self):
+        OVOSDinkumVoiceService.register_event_handlers(self)
         # Register handler for internet (re-)connection
         self.bus.on("mycroft.internet.connected",
                     self.handle_internet_connected)
         self.bus.on("ovos.phal.wifi.plugin.fully_offline",
                     self.handle_offline)
         self.bus.once("mycroft.ready", self.handle_ready)
 
@@ -175,26 +175,27 @@
             LOG.warning("Not disabling only active ww")
             resp = message.response({"error": "only one active ww",
                                      "active": True,
                                      "wake_word": requested_ww})
         else:
             try:
                 LOG.info(f"Disabling wake word: {requested_ww}")
-                self.config['hotwords'][requested_ww]['active'] = False
                 config_patch = {"hotwords": {requested_ww: {"active": False}}}
-                self.loop.config_loaded.clear()
-                update_mycroft_config(config_patch)
-                self.loop.config_loaded.wait()
+                _SERVICE_READY.clear()
+                update_mycroft_config(config_patch, bus=self.bus)
+                self.reload_configuration()  # TODO Not auto-reloading?
+                if not _SERVICE_READY.wait(15):
+                    raise TimeoutError("Timed out waiting for config reload")
                 resp = message.response({"error": False,
                                          "active": False,
                                          "wake_word": requested_ww})
             except Exception as e:
                 LOG.exception(e)
                 config_patch = {"hotwords": {requested_ww: {"active": True}}}
-                update_mycroft_config(config_patch)
+                update_mycroft_config(config_patch, bus=self.bus)
                 resp = message.response({"error": repr(e),
                                          "active": False,
                                          "wake_word": requested_ww})
         self.bus.emit(resp)
 
     def handle_enable_wake_word(self, message: Message):
         """
@@ -215,100 +216,81 @@
             LOG.warning(f"Requested enabling active ww: {requested_ww}")
             resp = message.response({"error": "ww already enabled",
                                      "active": True,
                                      "wake_word": requested_ww})
         else:
             try:
                 LOG.info(f"Enabling wake word: {requested_ww}")
-                self.config['hotwords'][requested_ww]['active'] = True
                 config_patch = {"hotwords": {requested_ww: {"active": True}}}
-                self.loop.config_loaded.clear()
-                update_mycroft_config(config_patch)
-                self.loop.needs_reload = True
-                self.loop.config_loaded.wait()
+                _SERVICE_READY.clear()
+                update_mycroft_config(config_patch, bus=self.bus)
+                self.reload_configuration()  # TODO Not auto-reloading?
+                if not _SERVICE_READY.wait(30):
+                    raise TimeoutError("Timed out waiting for config reload")
                 resp = message.response({"error": False,
                                          "active": True,
                                          "wake_word": requested_ww})
             except Exception as e:
                 LOG.exception(e)
                 config_patch = {"hotwords": {requested_ww: {"active": False}}}
-                update_mycroft_config(config_patch)
+                update_mycroft_config(config_patch, bus=self.bus)
                 resp = message.response({"error": repr(e),
                                          "active": False,
                                          "wake_word": requested_ww})
 
         self.bus.emit(resp)
 
     def handle_get_wake_words(self, message: Message):
         """
         Handle a request to get configured wake words and their current config.
-        This includes enabled and disabled wake words but excludes hotwords that
-        do not specify 'listen'
+        This includes enabled AND disabled wake words but excludes hotwords that
+        do not specify 'listen'.
         """
         hotwords = self.config.get('hotwords')
         wake_words = {ww: config for ww, config in hotwords.items()
                       if config.get('listen')}
         main_ww = self.config['listener'].get('wake_word')
         if wake_words.get(main_ww):
             LOG.debug(f"main_ww={main_ww}")
             wake_words[main_ww].setdefault('active', True)
+        else:
+            LOG.warning(f"Configured wake_word is not valid: {main_ww}")
         self.bus.emit(message.reply("neon.wake_words", data=wake_words))
 
     def handle_profile_update(self, message):
         """
         Handle an emitted profile update. If username associated with update is
         "local", updates the default profile applied to audio input messages.
         :param message: Message associated with profile update
         """
         updated_profile = message.data.get("profile")
         if updated_profile["user"]["username"] == \
                 self._default_user["user"]["username"]:
             apply_local_user_profile_updates(updated_profile,
                                              self._default_user)
 
-    def handle_utterance(self, event: dict):
-        """
-        Handle an utterance event on the Recognizer Loop
-        :param event: Utterance event
-        """
-        LOG.info("Utterance: " + str(event['utterances']))
-        context = event["context"]  # from audio transformers
-        context.update({'client_name': 'mycroft_listener',
-                        'source': 'audio',
-                        'ident': event.pop('ident', str(round(time()))),
-                        'raw_audio': event.pop('raw_audio', None),
-                        'destination': ["skills"],
-                        "timing": event.pop("timing", {}),
-                        'username': self._default_user["user"]["username"],
-                        'user_profiles': [self._default_user.content]
-                        })
-        if "data" in event:
-            data = event.pop("data")
-            context = merge_dict(context, data)
-
-        self._emit_utterance_to_skills(Message('recognizer_loop:utterance',
-                                               event, context))
-
     def handle_wake_words_state(self, message):
         """
         Handle a change of WW state
         :param message: Message associated with request
         """
+        # TODO: recognizer_loop:state.set
         enabled = message.data.get("enabled", True)
         mode = ListeningMode.WAKEWORD if enabled else ListeningMode.CONTINUOUS
-        self.loop.listen_mode = mode
-        if mode == ListeningMode.CONTINUOUS:
-            self.loop.responsive_recognizer.trigger_listen()
+        self.voice_loop.listen_mode = mode
+        self.voice_loop.reset_state()
 
     def handle_query_wake_words_state(self, message):
         """
         Query the current WW state
         :param message: Message associated with request
         """
-        enabled = self.loop.listen_mode == ListeningMode.WAKEWORD
+        # TODO: recognizer_loop:state.get
+        enabled = self.voice_loop.listen_mode == ListeningMode.WAKEWORD
+        self.voice_loop.reset_state()
         self.bus.emit(message.response({"enabled": enabled}))
 
     def handle_get_stt(self, message: Message):
         """
         Handles a request for stt.
         Emits a response to the sender with stt data or error data
         :param message: Message associated with request
@@ -388,36 +370,36 @@
             LOG.error(e)
             self.bus.emit(message.reply(ident, data={"error": repr(e)}))
 
     def handle_internet_connected(self, _):
         """
         Handle notification from core that internet connection is established
         """
-        if not self.loop.stt:
+        if not self.voice_loop.stt:
             LOG.debug("Internet connected before STT init")
             return
-        if self.loop.stt.config["module"] != self.config["stt"]["module"]:
+        if self.voice_loop.stt.config["module"] != self.config["stt"]["module"]:
             LOG.info("Reloading STT module")
-            self.loop.stt = STTFactory.create()
-        elif hasattr(self.loop.stt, "results_event"):
+            self.voice_loop.stt = STTFactory.create()
+        elif hasattr(self.voice_loop.stt, "results_event"):
             LOG.info(f"Internet Connected, Resetting STT Stream")
-            self.loop.stt.results_event.set()
+            self.voice_loop.stt.results_event.set()
 
     def handle_offline(self, _):
         """
         Handle notification to operate in offline mode
         """
         LOG.info("Offline mode selected, Reloading STT Plugin")
         config = dict(self.config)
         if config['stt'].get('offline_module'):
             config['stt']['module'] = config['stt'].get('offline_module')
-            self.loop.stt = STTFactory.create(config)
+            self.voice_loop.stt = STTFactory.create(config)
         else:
             LOG.info(f"Offline Mode, Resetting STT Stream")
-            self.loop.stt.results_event.set()
+            self.voice_loop.stt.results_event.set()
 
     def handle_ready(self, message):
         """
         Handle ready notification. If offline when ready, handle offline mode.
         """
         from neon_utils.net_utils import check_online
         if not check_online():
@@ -464,16 +446,15 @@
                 LOG.error(f"Timed out acquiring lock, not processing: {wav_file}")
                 transcriptions = []
         else:
             transcriptions = self.api_stt.execute(audio_data, lang)
         if isinstance(transcriptions, str):
             LOG.warning("Transcriptions is a str, no alternatives provided")
             transcriptions = [transcriptions]
-        audio, audio_context = self.loop.responsive_recognizer. \
-            audio_consumers.transform(audio_data)
+        audio, audio_context = self.transformers.transform(audio_data)
         LOG.info(f"Transcribed: {transcriptions}")
         return audio, audio_context, transcriptions
 
     def _emit_utterance_to_skills(self, message_to_emit: Message) -> bool:
         """
         Emits a message containing a user utterance to skills for intent
         processing and checks that it is received by the skills module.
```

## neon_speech/stt.py

```diff
@@ -28,15 +28,15 @@
 
 from abc import ABC
 from inspect import signature
 from threading import Event
 
 from neon_utils import LOG
 from ovos_plugin_manager.stt import OVOSSTTFactory, get_stt_config
-from ovos_plugin_manager.templates.stt import STT, StreamThread, StreamingSTT
+from ovos_plugin_manager.templates.stt import StreamingSTT
 
 from ovos_config.config import Configuration
 
 
 class WrappedSTT(StreamingSTT, ABC):
     def __new__(cls, base_engine, *args, **kwargs):
         results_event = kwargs.get("results_event") or Event()
```

## neon_speech/utils.py

```diff
@@ -21,31 +21,32 @@
 # CONTRIBUTORS  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import importlib
 
 from tempfile import mkstemp
 from ovos_utils.log import LOG
 from neon_utils.packaging_utils import get_package_dependencies
 
 
 def patch_config(config: dict = None):
     """
     Write the specified speech configuration to the global config file
     :param config: Mycroft-compatible configuration override
     """
-    import ovos_config.config
-
+    from ovos_config.config import LocalConf
+    from ovos_config.locations import USER_CONFIG
+    LOG.warning(f"Patching configuration with: {config}")
     config = config or dict()
-    ovos_config.config.update_mycroft_config(config)
-    importlib.reload(ovos_config.config)
+    local_config = LocalConf(USER_CONFIG)
+    local_config.update(config)
+    local_config.store()
 
 
 def _plugin_to_package(plugin: str) -> str:
     """
     Get a PyPI spec for a known plugin entrypoint
     :param plugin: plugin spec (i.e. config['stt']['module'])
     :returns: package name associated with `plugin` or `plugin`
```

## Comparing `neon_speech-3.3.2a5.dist-info/LICENSE.md` & `neon_speech-3.3.2a6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.3.2a5.dist-info/METADATA` & `neon_speech-3.3.2a6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.3.2a5
+Version: 3.3.2a6
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-listener (>=0.0.2a11,~=0.0.1)
-Requires-Dist: SpeechRecognition (~=3.8)
-Requires-Dist: PyAudio (~=0.2)
+Requires-Dist: ovos-dinkum-listener (>=0.0.2a21,~=0.0.1)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-utils (~=0.0.30)
 Requires-Dist: ovos-plugin-manager (>=0.0.23a17,~=0.0.19)
-Requires-Dist: pydub (~=0.23)
 Requires-Dist: click (~=8.0)
 Requires-Dist: click-default-group (~=1.2)
-Requires-Dist: neon-transformers (~=0.2)
 Requires-Dist: neon-utils[audio,network] (>=1.5.0a5,~=1.3)
 Requires-Dist: ovos-config (~=0.0.7)
 Requires-Dist: ovos-vad-plugin-webrtcvad (~=0.0.1)
 Requires-Dist: ovos-ww-plugin-vosk (~=0.1)
 Provides-Extra: docker
 Requires-Dist: ovos-stt-plugin-vosk (~=0.1) ; extra == 'docker'
 Requires-Dist: neon-stt-plugin-nemo (~=0.0.2) ; extra == 'docker'
```

