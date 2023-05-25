# Comparing `tmp/seaplayer-0.5.1.tar.gz` & `tmp/seaplayer-0.5.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.1.tar", max compression
+gzip compressed data, was "seaplayer-0.5.1.dev2.tar", max compression
```

## Comparing `seaplayer-0.5.1.tar` & `seaplayer-0.5.1.dev2.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     1064 2023-05-24 14:13:35.295929 seaplayer-0.5.1/LICENSE
--rw-r--r--   0        0        0     1304 2023-05-24 14:13:35.295929 seaplayer-0.5.1/README.md
--rw-r--r--   0        0        0     1607 2023-05-25 18:51:16.121855 seaplayer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/__init__.py
--rw-r--r--   0        0        0      331 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     2415 2023-05-24 19:25:42.492196 seaplayer-0.5.1/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      459 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2860 2023-05-24 19:26:44.687111 seaplayer-0.5.1/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      455 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      457 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      574 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0      254 2023-05-24 15:00:37.735912 seaplayer-0.5.1/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     1859 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6031 2023-05-24 19:05:33.708654 seaplayer-0.5.1/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1491 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/css/objects.css
--rw-r--r--   0        0        0      555 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      260 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1367 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0     1022 2023-05-25 15:53:15.329317 seaplayer-0.5.1/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1378 2023-05-25 15:52:07.380741 seaplayer-0.5.1/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     2938 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1094 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/Input.py
--rw-r--r--   0        0        0      950 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5430 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      759 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1240 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0      368 2023-05-25 15:52:32.639344 seaplayer-0.5.1/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0       85 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      547 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      730 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     6978 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2100 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0     8329 2023-05-25 15:53:55.959162 seaplayer-0.5.1/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0      982 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0       83 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0    19041 2023-05-25 15:44:13.592874 seaplayer-0.5.1/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     2547 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1553 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0       63 2023-05-24 14:13:35.295929 seaplayer-0.5.1/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1354 2023-05-25 15:54:10.020267 seaplayer-0.5.1/seaplayer/units.py
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 seaplayer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/README.md
+-rw-r--r--   0        0        0     1450 2023-05-24 20:48:50.932426 seaplayer-0.5.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     2415 2023-05-24 19:25:42.492196 seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      459 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2860 2023-05-24 19:26:44.687111 seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      455 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      457 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      574 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0      254 2023-05-24 15:00:37.735912 seaplayer-0.5.1.dev2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     1859 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6031 2023-05-24 19:05:33.708654 seaplayer-0.5.1.dev2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1491 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      555 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      260 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      374 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1367 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0     1022 2023-05-24 15:31:52.607550 seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     2938 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1094 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0      950 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5430 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      759 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1240 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0      316 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      730 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     6978 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2100 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0     9316 2023-05-24 20:38:01.064915 seaplayer-0.5.1.dev2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0      982 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0       83 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0    18891 2023-05-24 20:28:20.713484 seaplayer-0.5.1.dev2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     2547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1553 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0       63 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-24 20:49:18.523757 seaplayer-0.5.1.dev2/seaplayer/units.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 seaplayer-0.5.1.dev2/PKG-INFO
```

### Comparing `seaplayer-0.5.1/LICENSE` & `seaplayer-0.5.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/README.md` & `seaplayer-0.5.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/pyproject.toml` & `seaplayer-0.5.1.dev2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.1"
+version = "0.5.1.dev2"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -28,29 +28,24 @@
     "seaplayer/css/unknown.css"
 ]
 
 [tool.poetry.scripts]
 seaplayer = "seaplayer.__main__:run"
 
 [tool.poetry.dependencies]
-python = "^3.9,<3.12"
+python = "^3.9"
 pillow = "^9.5.0"
 aiofiles = "^23.1.0"
 rich = ">=13.3.5"
 mutagen = "1.45.1"
 textual = ">=0.25.0"
 playsoundsimple-py = "0.7.0"
 properties-py = "1.1.0"
 typing-inspect = "^0.8.0"
 ripix = ">=2.2.3"
 platformdirs = "^3.5.1"
 pydantic = "^1.10.7"
-poetry = {version = "^1.5.0", optional = true}
-pyinstaller = {version = "^5.11.0", optional = true}
-
-[tool.poetry.extras]
-build = ["poetry", "pyinstaller"]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seaplayer-0.5.1/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/codecs/Any.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/codecs/WAV.py` & `seaplayer-0.5.1.dev2/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/codeсbase.py` & `seaplayer-0.5.1.dev2/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/config.py` & `seaplayer-0.5.1.dev2/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/css/objects.css` & `seaplayer-0.5.1.dev2/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/css/seaplayer.css` & `seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/functions.py` & `seaplayer-0.5.1.dev2/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/modules/colorizer.py` & `seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/Configurate.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/Image.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/Input.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/Log.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/MusicList.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/Notification.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.1.dev2/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/screens/Configurate.py` & `seaplayer-0.5.1.dev2/seaplayer/screens/Configurate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,96 @@
 from textual.app import ComposeResult
 from textual.screen import Screen
-from textual.widgets import Header, Footer
+from textual.widgets import Header, Footer, OptionList
+from textual.widgets.option_list import Option
 # > Typing
-try:
-    from sounddevice import query_devices, query_hostapis
-    INIT_SOUNDDEVICE = True
-except:
-    INIT_SOUNDDEVICE = False
-from typing import Optional, Literal, Dict, Any, List
+from sounddevice import query_devices, query_hostapis
+from typing import Optional, Literal, Dict, Any, List, Callable
 # > Local Imports
 from ..types import Converter
 from ..modules.colorizer import richefication
 from ..objects import (
     Nofy,
     InputField,
-    DataOption,
-    DataOptionList,
     ConfigurateList,
     ConfigurateListItem
 )
 
 # ! Vars
 conv = Converter()
 
+# ! Types
+class DataOption(Option):
+    def __init__(
+        self,
+        text: str,
+        selected: bool=False,
+        id: Optional[str]=None,
+        disable: bool=False,
+        **data
+    ) -> None:
+        super().__init__(text, id=id, disabled=disable)
+        self.group = ""
+        self.selected = selected
+        self.data = data
+
+class DataOptionList(OptionList):
+    def __init__(
+        self,
+        *content: DataOption,
+        group: Optional[str]="",
+        after_selected: Callable[[DataOption], None]=lambda option: None
+    ) -> None:
+        super().__init__()
+        self.group = group
+        self.content = content
+        self.after_selected = after_selected
+    
+    def on_mount(self):
+        for index, option in enumerate(self.content):
+            self.add_option(option)
+            if isinstance(option, DataOption):
+                option.group = self.group
+                if option.selected:
+                    self.highlighted = index
+    
+    async def on_option_list_option_selected(self, event: OptionList.OptionSelected) -> None:
+        if isinstance(event.option, DataOption):
+            if self.group == event.option.group:
+                self.app.info("Select OutputSoundDeviceID: " + str(event))
+                await self.after_selected(event.option)
+
 # ! Functions
-if INIT_SOUNDDEVICE:
-    def generate_devices_options(currect: Optional[int]=None):
-        hosts: List[Dict[str, Any]] = [_1 for _1 in query_hostapis()]
-        devices: List[Dict[str, Any]] = [_2 for _2 in query_devices()]
-        devices_options: List[DataOption] = []
-        devices_options.append(DataOption("([cyan]*[/cyan]) [yellow]Auto[/yellow]", device_index=None))
-        
-        for device in devices:
-            if device["max_output_channels"] > 0:
-                try:
-                    format_data = dict(
-                        device_name=device["name"], 
-                        device_index=device["index"],
-                        hostapi_index=device["hostapi"],
-                        hostapi_name=hosts[device["hostapi"]]["name"]
+def generate_devices_options(currect: Optional[int]=None):
+    hosts: List[Dict[str, Any]] = [_1 for _1 in query_hostapis()]
+    devices: List[Dict[str, Any]] = [_2 for _2 in query_devices()]
+    devices_options: List[DataOption] = []
+    devices_options.append(DataOption("([cyan]*[/cyan]) [yellow]Auto[/yellow]", device_index=None))
+    
+    for device in devices:
+        if device["max_output_channels"] > 0:
+            try:
+                format_data = dict(
+                    device_name=device["name"], 
+                    device_index=device["index"],
+                    hostapi_index=device["hostapi"],
+                    hostapi_name=hosts[device["hostapi"]]["name"]
+                )
+                devices_options.append(
+                    DataOption(
+                        "([cyan]{device_index}[/cyan]) [yellow]{device_name}[/yellow] \[[green]{hostapi_name}[/green]]".format(**format_data),
+                        device_index=device["index"]
                     )
-                    devices_options.append(
-                        DataOption(
-                            "([cyan]{device_index}[/cyan]) [yellow]{device_name}[/yellow] \[[green]{hostapi_name}[/green]]".format(**format_data),
-                            device_index=device["index"]
-                        )
-                    )
-                except:
-                    pass
-        for d in devices_options:
-            if d.data["device_index"] == currect:
-                d.selected = True
-        return devices_options
+                )
+            except:
+                pass
+    for d in devices_options:
+        if d.data["device_index"] == currect:
+            d.selected = True
+    return devices_options
 
 # ! Main Class
 class Configurate(Screen):
     """This Configurate Menu screen."""
     BINDINGS = [("escape", "app.pop_screen", "Back")]
     
     # ! Nofy Functions
@@ -82,20 +117,19 @@
         return lambda: self._upfif(attr_name)
     
     # ! Update App Config
     async def _uac(self, attr_name: str, input: InputField, value: str) -> None:
         exec(f"self.{attr_name} = value")
         await self.aio_nofy("Saved!")
     
-    if INIT_SOUNDDEVICE:
-        def gucsdi(self):
-            async def n_ucsdi(option: DataOption) -> None:
-                self.app.config.output_sound_device_id = option.data.get("device_index", None)
-                await self.aio_nofy("Saved!")
-            return n_ucsdi
+    def gucsdi(self):
+        async def n_ucsdi(option: DataOption) -> None:
+            self.app.config.output_sound_device_id = option.data.get("device_index", None)
+            await self.aio_nofy("Saved!")
+        return n_ucsdi
     
     def guac(self, attr_name: str):
         async def an_uac(input: InputField, value: str) -> None: await self._uac(attr_name, input, value)
         return an_uac
 
     # ! Configurator Generators
     def create_configurator_type(
@@ -132,40 +166,38 @@
                 update_placeholder=self.gupfif(attr_name)
             ),
             title="[red]{Key}[/red]: "+title+f" ({richefication(str)})",
             desc=desc+(" [red](restart required)[/red]" if restart_required else ""),
             height=5
         )
     
-    if INIT_SOUNDDEVICE:
-        def create_configurator_sound_devices(self):
-            options_list = DataOptionList(
-                *generate_devices_options(self.app.config.output_sound_device_id),
-                group="SoundDevicesSelect",
-                after_selected=self.gucsdi()
-            )
-            return ConfigurateListItem(
-                options_list,
-                title="[red]{Sound}[/]: Output Sound Device",
-                desc="Select the device that SeaPlayer will work with. [red](restart required)[/red]",
-                height=8
-            )
+    def create_configurator_sound_devices(self):
+        options_list = DataOptionList(
+            *generate_devices_options(self.app.config.output_sound_device_id),
+            group="SoundDevicesSelect",
+            after_selected=self.gucsdi()
+        )
+        return ConfigurateListItem(
+            options_list,
+            title="[red]{Sound}[/]: Output Sound Device",
+            desc="Select the device that SeaPlayer will work with. [red](restart required)[/red]",
+            height=8
+        )
     
     # ! Configurate Main Functions
     def compose(self) -> ComposeResult:
         yield Header()
         with ConfigurateList():
             yield self.create_configurator_type(
                 "app.config.sound_font_path",
                 "Sound", "Sound Font Path",
                 "Path to SF2-file.",
                 conv.optional(conv.filepath), Optional[str], False
             )
-            if INIT_SOUNDDEVICE:
-                yield self.create_configurator_sound_devices()
+            yield self.create_configurator_sound_devices()
             yield self.create_configurator_type(
                 "app.config.image_update_method",
                 "Image", "Image Update Method",
                 "The name of the picture update option.",
                 conv.literal_string("sync", "async"), Literal["sync", "async"]
             )
             yield self.create_configurator_type(
```

### Comparing `seaplayer-0.5.1/seaplayer/screens/Unknown.py` & `seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/seaplayer.py` & `seaplayer-0.5.1.dev2/seaplayer/seaplayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,24 +207,23 @@
                             self.info(f"Playing the next sound: {repr(sound)}")
                 
                 self.last_playback_status = status
             await asyncio.sleep(0.2)
     
     def compose(self) -> ComposeResult:     
         # * Other
-        self.info("--- [pink]SeaPlayer.compose[/pink] [green]Starting[/green] ---")
         self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
         self.info(f"Source          : {__url__}")
         self.info(f"Codecs          : {repr(self.CODECS)}")
         self.info(f"Config Path     : {repr(self.config.filepath)}")
         self.info(f"CSS Dirpath     : {repr(CSS_LOCALDIR)}")
         self.info(f"Assets Dirpath  : {repr(ASSETS_DIRPATH)}")
         self.info(f"Codecs Kwargs   : {repr(self.CODECS_KWARGS)}")
         self.info(f"Sound Device ID : {repr(self.config.output_sound_device_id)}")
-        
+        self.info(f"")
         
         # * Play Screen
         self.music_play_screen = Static(classes="screen-box")
         self.music_play_screen.border_title = "Player"
         
         # * Image Object Init
         self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
@@ -275,15 +274,14 @@
         )
         self.run_worker(
             self.plugin_loader.on_compose,
             name="ON_COMPOSE",
             group="PluginLoader",
             description="<method PluginLoader.on_compose>"
         )
-        self.info("--- [pink]SeaPlayer.compose[/pink] [red]Starting[/red] ---")
     
     async def add_sounds_to_list(self) -> None:
         added_oks = 0
         loading_nofy = await self.aio_callnofy(
             f"Found [cyan]{len(self.last_paths_globalized)}[/cyan] values. Loading..."
         )
         async for path in aiter(self.last_paths_globalized):
```

### Comparing `seaplayer-0.5.1/seaplayer/types/Convert.py` & `seaplayer-0.5.1.dev2/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/types/MusicList.py` & `seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1/seaplayer/units.py` & `seaplayer-0.5.1.dev2/seaplayer/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.1"
+__version__ = "0.5.1.dev2"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
@@ -21,15 +21,15 @@
 ASSETS_DIRPATH = os.path.join(os.path.dirname(__file__), "assets")
 
 CONFIG_DIRPATH = user_config_dir(__title__, __author__, ensure_exists=True)
 CONFIG_FILEPATH = os.path.join(CONFIG_DIRPATH, "config.properties")
 
 PLUGINS_DIRPATH = os.path.join(CONFIG_DIRPATH, "plugins")
 PLUGINS_CONFIG_PATH = os.path.join(CONFIG_DIRPATH, "plugins.json")
-
+#                   You didn't see anything  >:|
 GLOB_PLUGINS_INFO_SEARCH = os.path.join(PLUGINS_DIRPATH, "*", "info.json")
 GLOB_PLUGINS_INIT_SEARCH = os.path.join(PLUGINS_DIRPATH, "*", "__init__.py")
 
 # ! Assets Paths
 IMGPATH_IMAGE_NOT_FOUND = os.path.join(ASSETS_DIRPATH, "image-not-found.png")
 
 # ! Constants
```

### Comparing `seaplayer-0.5.1/PKG-INFO` & `seaplayer-0.5.1.dev2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.1
+Version: 0.5.1.dev2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: build
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: mutagen (==1.45.1)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: playsoundsimple-py (==0.7.0)
-Requires-Dist: poetry (>=1.5.0,<2.0.0) ; extra == "build"
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyinstaller (>=5.11.0,<6.0.0) ; extra == "build"
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
 Requires-Dist: textual (>=0.25.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
```

