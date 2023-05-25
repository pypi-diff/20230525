# Comparing `tmp/cracker-0.7.0.tar.gz` & `tmp/cracker-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cracker-0.7.0.tar", last modified: Sat May 13 19:36:43 2023, max compression
+gzip compressed data, was "cracker-0.7.1.tar", last modified: Thu May 25 03:41:32 2023, max compression
```

## Comparing `cracker-0.7.0.tar` & `cracker-0.7.1.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.832904 cracker-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.836904 cracker-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-13 19:36:31.000000 cracker-0.7.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-13 19:36:31.000000 cracker-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 19:36:31.000000 cracker-0.7.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-13 19:36:31.000000 cracker-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-13 19:36:31.000000 cracker-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-13 19:36:43.840904 cracker-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-13 19:36:31.000000 cracker-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.836904 cracker-0.7.0/cracker/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.836904 cracker-0.7.0/cracker/config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/config/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/config/parser.json
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/cracker_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/icon.jpeg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/keylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/mp3_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/cracker/speaker/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/speaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/speaker/abstract_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/speaker/espeak.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/speaker/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/speaker/polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/ssml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/cracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/tests/test_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/text_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/cracker/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/view/config_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/view/parser_config_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-13 19:36:31.000000 cracker-0.7.0/cracker/view/speaker_config_tab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.836904 cracker-0.7.0/cracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-13 19:36:43.000000 cracker-0.7.0/cracker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-13 19:36:31.000000 cracker-0.7.0/docs/macos.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-13 19:36:31.000000 cracker-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 19:36:43.840904 cracker-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:36:43.840904 cracker-0.7.0/ubuntu/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-13 19:36:31.000000 cracker-0.7.0/ubuntu/cracker.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-13 19:36:31.000000 cracker-0.7.0/ubuntu/icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-13 19:36:31.000000 cracker-0.7.0/ubuntu/install_ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.583131 cracker-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.571131 cracker-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.575131 cracker-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 03:41:17.000000 cracker-0.7.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 03:41:17.000000 cracker-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 03:41:17.000000 cracker-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 03:41:17.000000 cracker-0.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 03:41:32.583131 cracker-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-25 03:41:17.000000 cracker-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.575131 cracker-0.7.1/cracker/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/config/parser.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/cracker_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/icon.jpeg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4856 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/keylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/mp3_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/speaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/abstract_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/espeak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/speaker/polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/ssml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/tests/test_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   425242 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/config_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/parser_config_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-25 03:41:17.000000 cracker-0.7.1/cracker/view/speaker_config_tab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/cracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 03:41:32.000000 cracker-0.7.1/cracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 03:41:17.000000 cracker-0.7.1/docs/macos.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 03:41:17.000000 cracker-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:41:32.583131 cracker-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:41:32.579131 cracker-0.7.1/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/cracker.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-05-25 03:41:17.000000 cracker-0.7.1/ubuntu/install_ubuntu.sh
```

### Comparing `cracker-0.7.0/.github/workflows/publish-pypi.yml` & `cracker-0.7.1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/LICENSE` & `cracker-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/PKG-INFO` & `cracker-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.0
+Version: 0.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.0/README.md` & `cracker-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/config/configuration.py` & `cracker-0.7.1/cracker/config/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pkgutil
 from typing import Any, Dict, Optional
 
 import yaml
 
 from cracker.speaker import LANGUAGES
-from cracker.utils import get_logger, deep_dict_merge
+from cracker.utils import deep_dict_merge, get_logger
 
 
 class Configuration:
     """Holds configuration values for the application."""
 
     singleton = None
     _logger = get_logger(__name__)
@@ -68,14 +68,18 @@
             yaml.safe_dump(config, f)
 
     @property
     def user_config_path(self):
         return os.path.join(self.USER_CONFIG_DIR_PATH, "settings.yaml")
 
     @property
+    def user_parser_path(self):
+        return os.path.join(self.USER_CONFIG_DIR_PATH, "parser.json")
+
+    @property
     def default_config(self) -> Dict:
         if self._default_config is None:
             return {}
         return self._default_config
 
     def _read_user_config(self, config: Dict) -> Dict:
         if not os.path.isdir(self.USER_CONFIG_DIR_PATH):
@@ -98,29 +102,30 @@
             "speaker": self.speaker or self.default_config["cracker"]["speaker"],
             "language": self.language or self.default_config["cracker"]["language"],
             "speed": str(self.speed) or self.default_config["cracker"]["speed"],
             "voice": self.voice or self.default_config["cracker"].get("voice", ""),
         }
         if extra_config is not None:
             config = deep_dict_merge(config, extra_config)
+
+        self.save_regex_config(self.user_parser_path)
         self._write_yaml(config)
 
     def apply_config(self, configuration: Dict) -> Dict[str, Any]:
         """Applies parsed config to Cracker and UI components.
 
         Returns:
             Dict of the most important values which might be used by other components.
             This includes: speaker, language, speed and voices with their settings.
         """
         config = configuration["cracker"]
         config_speakers = configuration["speakers"]
 
         # Current setting
         _config = {}
-        _config["parser_config_path"] = self.parser_config_path = config["parser_config_path"]
         _config["speaker"] = self.speaker = config["speaker"]
         _config["language"] = self.language = config["language"]
         _config["speed"] = self.speed = int(config["speed"])
         _config["voice"] = self.voice = config_speakers[self.speaker.lower()].get("voice", "")
 
         # Augment setting based on speaker
         speaker_config = self.load_speaker_config(self.speaker, self.language)
@@ -136,16 +141,16 @@
 
         # Check for different than default AWS profile_name
         _config["polly"]["profile_name"] = config_speakers.get("polly", {}).get("profile_name", "default")
 
         if self.voice not in self.lang_voices:
             _config["voice"] = self.voice = self.lang_voices[0]
 
-        if self.parser_config_path is not None:
-            self.regex_config = self.load_regex_config()
+        self.regex_config = self.load_regex_config()
+        print(f"Regex: {self.regex_config}")
 
         return _config
 
     def load_speaker_config(self, speaker, language=None):
         """Loads speaker's default and available configuration.
 
         Args:
@@ -167,12 +172,27 @@
             config["voice"] = self.voice = self.lang_voices[0]
 
         return config
 
     def load_regex_config(self):
         """From provided path to a config it extracts configuration for the TextParser"""
         regex_config = None
-        file_content = pkgutil.get_data("cracker", self.parser_config_path)
-        if file_content is None:
-            raise FileNotFoundError(f"Could not find config file {self.parser_config_path}")
-        regex_config = json.loads(file_content.decode("utf-8"))["parser_rules"]
-        return regex_config
+
+        if not os.path.isdir(self.USER_CONFIG_DIR_PATH):
+            self._logger.debug("Creating user dir in '%s'", self.USER_CONFIG_DIR_PATH)
+            os.mkdir(self.USER_CONFIG_DIR_PATH)
+
+        if not os.path.isfile(self.user_parser_path):
+            file_content = pkgutil.get_data("cracker", "config/parser.json")
+            file_content = file_content.decode("utf-8")
+        else:
+            with open(self.user_parser_path) as f:
+                file_content = f.read()
+        regex_config = json.loads(file_content)["parser_rules"]
+        return {v["name"]: v for v in regex_config}
+
+    def save_regex_config(self, parser_config_path: str) -> None:
+        """Writes configuration to file system."""
+        parser_rules = {"parser_rules": self.regex_config}
+        print(parser_rules)
+        with open(parser_config_path, "w") as f:
+            json.dump(parser_rules, f, indent=4)
```

### Comparing `cracker-0.7.0/cracker/config/parser.json` & `cracker-0.7.1/cracker/config/parser.json`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/cracker.py` & `cracker-0.7.1/cracker/cracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.app = app
 
         self.config = Configuration()
         _ = self.config.read_config()
 
         self.player = QMediaPlayer()
         self.speaker: AbstractSpeaker = self.get_speaker(self.config.speaker, self.player)
-        self.textParser = TextParser(config_path=self.config.parser_config_path)
+        self.text_parser = TextParser()
 
         self.gui = MainWindow(self.config, speakers=self.SPEAKER)
         self.gui.speaker = self.speaker
         self.gui.player = self.player
 
         self.key_manager = KeyBoardManager(self.app)
 
@@ -65,51 +65,51 @@
     def run(self):
         self.gui.init()
         self.set_action()
         self.gui.show()
 
     def reduce_text(self):
         text = self.gui.textEdit.toPlainText()
-        new_text = self.textParser.reduce_text(text)
+        new_text = self.text_parser.reduce_text(text)
         self.gui.textEdit.setText(new_text)
 
     def reduce_cite(self):
         text = self.gui.textEdit.toPlainText()
-        new_text = self.textParser.reduce_cite(text)
+        new_text = self.text_parser.reduce_cite(text)
         self.gui.textEdit.setText(new_text)
 
     def wiki_text(self):
         """Sets the text box with wikipedia specific cleaned text.
         Example of this is removing `citation needed` and other references.
         """
         text = self.gui.textEdit.toPlainText()
-        text = self.textParser.wiki_text(text)
+        text = self.text_parser.wiki_text(text)
         self.gui.textEdit.setText(text)
 
     def read_text_area(self):
         """Reads out text in the text_box with selected speaker."""
         self.stop_text()
         text = self.gui.textEdit.toPlainText()  # TODO: toHtml() gives more control
 
-        self.textParser.parser_rules = self.config.regex_config
-        text = self.textParser.reduce_text(text)
+        self.text_parser.parser_rules = self.config.regex_config
+        text = self.text_parser.reduce_text(text)
         self._read(text)
 
     def toggle_read_text_clipboard(self):
         """Reads out text from the clipboard with selected speaker."""
         self._logger.debug("Reading text from clipboard")
         if self.player.state() == QMediaPlayer.PlayingState:
             self.stop_text()
             self.player.stop()
         else:
             self.stop_text()
             text = self.app.clipboard().text()
 
-            self.textParser.parser_rules = self.config.regex_config
-            text = self.textParser.reduce_text(text)
+            self.text_parser.parser_rules = self.config.regex_config
+            text = self.text_parser.reduce_text(text)
             self._read(text)
 
     def _read(self, text):
         self._logger.debug(f"Reading text: {text}")
         speaker_config = self._prepare_config()
         self._last_pid = self.speaker.read_text(text, **speaker_config)
```

### Comparing `cracker-0.7.0/cracker/cracker_gui.py` & `cracker-0.7.1/cracker/cracker_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         self.config_window = ConfigWindow()
 
     def init(self):
         self.set_action()
         self.set_widgets()
         self.init_values()
-        self.config_window.init(regex_file_path=self.config.parser_config_path)
+        self.config_window.init()
 
     def set_action(self):
         assert self.player, "Cannot set actions on non-defined Player"
         _exit = QAction("Exit", self)
         _exit.setShortcut("Ctrl+Q")
         _exit.setStatusTip("Exit application")
         _exit.triggered.connect(self.closeEvent)
```

### Comparing `cracker-0.7.0/cracker/icon.jpeg` & `cracker-0.7.1/cracker/icon.jpeg`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/icon.png` & `cracker-0.7.1/cracker/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/keylogger.py` & `cracker-0.7.1/cracker/keylogger.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/main.py` & `cracker-0.7.1/cracker/main.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/mp3_helper.py` & `cracker-0.7.1/cracker/mp3_helper.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/speaker/__init__.py` & `cracker-0.7.1/cracker/speaker/__init__.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/speaker/abstract_speaker.py` & `cracker-0.7.1/cracker/speaker/abstract_speaker.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/speaker/espeak.py` & `cracker-0.7.1/cracker/speaker/espeak.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/speaker/google.py` & `cracker-0.7.1/cracker/speaker/google.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/speaker/polly.py` & `cracker-0.7.1/cracker/speaker/polly.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/ssml.py` & `cracker-0.7.1/cracker/ssml.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/tests/test_config.py` & `cracker-0.7.1/cracker/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,28 @@
 
     cracker_config = default_config["cracker"]
     assert cracker_config["speaker"] == "polly"
     assert cracker_config["speed"] == 4
     assert cracker_config["language"] == "English"
 
 
+@patch("cracker.config.configuration.os.mkdir")
+@patch("cracker.config.configuration.os.path.isfile", return_value=False)
 @patch("cracker.config.configuration.os.path.isdir", return_value=False)
-def test_read_config(mock_isdir):
+def test_read_config(mock_isdir, mock_isfile, mock_mkdir):
     config = Configuration()
     config.read_config()
     assert config.speaker == "polly"
     assert config.speed == 4
     assert config.language == "English"
 
-    mock_isdir.assert_called_once_with(config.USER_CONFIG_DIR_PATH)
+    mock_mkdir.assert_called_once_with(config.USER_CONFIG_DIR_PATH)
+    mock_isdir.assert_called_with(config.USER_CONFIG_DIR_PATH)
+    mock_isfile.assert_called_once_with(config.user_parser_path)
+    assert mock_isdir.call_count == 2
 
 
 @patch("cracker.config.configuration.os.path.isfile", return_value=False)
 @patch("cracker.config.configuration.os.path.isdir", return_value=True)
 def test_read_user_config_dir_exists_file_not(mock_isdir, mock_isfile):
     config = Configuration()
     test_config = {"cracker": {"speaker": "polly", "speed": 2, "language": "pnglish"}}
```

### Comparing `cracker-0.7.0/cracker/tests/test_text_parser.py` & `cracker-0.7.1/cracker/tests/test_text_parser.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/text_parser.py` & `cracker-0.7.1/cracker/text_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import html
-import json
 import logging
-import pkgutil
 import re
 from collections import OrderedDict
-from typing import Optional
+
+from cracker.config import Configuration
 
 
 class TextParser:
     _logger = logging.getLogger(__name__)
 
     citation_author_year = re.compile(r"[\(\[]\w+, \d{4}(;\s\w+, \d{4})*[\)\]]")
     citation_numbers_comma = re.compile(r"\[\d+(,\s*\d+)*\]")
 
-    def __init__(self, config_path: Optional[str] = None):
+    def __init__(self):
         self._config = None
         self._parser_rules = None
         self._regex_rules = OrderedDict()
 
-        # Check that this is a file
-        if self._config is None and config_path is not None:
-            self.config = self.read_config_path(config_path)
+        global_config = Configuration()
+        self.config = global_config.load_regex_config()
 
     @property
     def config(self):
         return self._config
 
     @config.setter
     def config(self, config):
@@ -37,32 +35,23 @@
 
     @parser_rules.setter
     def parser_rules(self, parser_rules):
         assert self._config, "Need to provide config before parser"
         self._config["parser_rules"] = parser_rules
         self.update_config()
 
-    def read_config_path(self, config_path: str):
-        """From provided path to a config it extracts configuration for the TextParser"""
-        self._logger.info("parsing read config path")
-        file_content = pkgutil.get_data("cracker", config_path)
-        if file_content is None:
-            raise FileNotFoundError(f"Could not find config file {config_path}")
-        config = json.loads(file_content.decode("utf-8"))
-        return config
-
     def update_config(self):
         """Goes through the config and extracts regex rules."""
         if self.config is None:
             return
 
         # Clears all regex rules
         self._regex_rules.clear()
 
-        for rule in self.config["parser_rules"]:
+        for rule in self.config.values():
             if not rule["active"]:
                 continue
             self._regex_rules[rule["key"]] = rule["value"]
 
     @classmethod
     def reduce_cite(cls, text: str) -> str:
         """Removes citations from pasted text."""
```

### Comparing `cracker-0.7.0/cracker/themes.py` & `cracker-0.7.1/cracker/themes.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/utils.py` & `cracker-0.7.1/cracker/utils.py`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/cracker/view/config_window.py` & `cracker-0.7.1/cracker/view/config_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from PyQt5.QtWidgets import QGridLayout, QPushButton, QWidget, QTabWidget
+from PyQt5.QtWidgets import QGridLayout, QPushButton, QTabWidget, QWidget
 
 from cracker.config import Configuration
 from cracker.view.parser_config_tab import ParserConfig
 from cracker.view.speaker_config_tab import SpeakerConfig
 
 
 class ConfigWindow(QWidget):
@@ -37,17 +37,17 @@
 
         self._layout.addWidget(self.tabs, 1, 0, 1, 4)
         self._layout.addWidget(self.cancel_btn, 2, 2)
         self._layout.addWidget(self.confirm_btn, 2, 3)
 
         self.resize(500, self.height())
 
-    def init(self, regex_file_path=""):
+    def init(self):
         self._logger.debug("Init config window")
-        self.parser_tab.init(regex_file_path)
+        self.parser_tab.init()
 
     def cancel_action(self):
         self.hide()
 
     def confirm_action(self):
         self._logger.debug("Confirm action")
         self.config.regex_config = self.parser_tab.confirm_action()
```

### Comparing `cracker-0.7.0/cracker/view/parser_config_tab.py` & `cracker-0.7.1/cracker/view/parser_config_tab.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 import json
 import logging
 import pkgutil
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from PyQt5.QtWidgets import QCheckBox, QGridLayout, QLabel, QLineEdit, QWidget
+
 from cracker.config import Configuration
 
 
 class ParserConfig(QWidget):
     _logger = logging.getLogger(__name__)
 
-    def __init__(self, regex_file_path=""):
+    def __init__(self):
         super().__init__()
 
         self.config = Configuration()
 
-        self.regex_file_path = regex_file_path
         self.regex_config = {}
-        # self.setWindowTitle("Configuration")
 
         self.layout = QGridLayout()
         self.setLayout(self.layout)
 
-    def init(self, regex_file_path=""):
-        self.regex_file_path = regex_file_path
-
-        self.regex_config = self.refresh_reduce_rules()
+    def init(self):
+        self.regex_config = self.config.regex_config
         self.create_options(self.regex_config)
 
-    def confirm_action(self):
+    def confirm_action(self) -> List:
         self.check_update()
-        # self.config.regex_config = self.get_regex_config()
-        # self.hide()
         return self.get_regex_config()
 
     def clearLayout(layout):
         while layout.count():
             child = layout.takeAt(0)
             if child.widget():
                 child.widget().deleteLater()
 
     def refresh_reduce_rules(self) -> Optional[Dict]:
         """From provided path to a config it extracts configuration for the TextParser"""
-        if len(self.regex_file_path) == 0:
-            print("Couldn't find config file. Skipping configuration.")
-            return
-
         regex_config_list = {}
         try:
             file_content = pkgutil.get_data("cracker", self.regex_file_path)
             if file_content is None:
                 raise FileNotFoundError(f"Could not find config file {self.regex_file_path}")
             regex_config_list = json.loads(file_content.decode("utf-8"))
         except Exception:
@@ -65,25 +56,31 @@
     def create_options(self, options):
         regex_config_options = RegexConfigOptions(options)
         self.layout.addWidget(regex_config_options, 0, 0, 1, 5)
 
     def check_update(self) -> None:
         """Iterate through every option and see it they're active"""
         assert self.regex_config, "Regex config hasn't been loaded"
-        regex_config_options_layout = self.layout.itemAtPosition(0, 0).widget().layout
-        for row in range(1, regex_config_options_layout.rowCount()):
-            active_box = regex_config_options_layout.itemAtPosition(row, RegexConfigOptions.ACTIVE_POS).widget()
-            name_widget = regex_config_options_layout.itemAtPosition(row, RegexConfigOptions.NAME_POS).widget()
+        _layout = self.layout.itemAtPosition(0, 0).widget().layout
+        for row in range(1, _layout.rowCount()):
+            active_box = _layout.itemAtPosition(row, RegexConfigOptions.ACTIVE_POS).widget()
+            key_box = _layout.itemAtPosition(row, RegexConfigOptions.KEY_POS).widget()
+            value_box = _layout.itemAtPosition(row, RegexConfigOptions.VALUE_POS).widget()
+            name_widget = _layout.itemAtPosition(row, RegexConfigOptions.NAME_POS).widget()
             name = name_widget.text()
+
+            # TODO: Oopsy! Can't change name!
             if name in self.regex_config:
                 self.regex_config[name]["active"] = active_box.isChecked()
+                self.regex_config[name]["key"] = key_box.text()
+                self.regex_config[name]["value"] = value_box.text()
 
-    def get_regex_config(self):
+    def get_regex_config(self) -> List:
         assert self.regex_config, "Regex config hasn't been loaded"
-        return self.regex_config.values()
+        return list(self.regex_config.values())
 
 
 class RegexConfigOptions(QWidget):
     ACTIVE_POS = 1
     NAME_POS = 2
     KEY_POS = 6
     VALUE_POS = 10
```

### Comparing `cracker-0.7.0/cracker/view/speaker_config_tab.py` & `cracker-0.7.1/cracker/view/speaker_config_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     _logger = logging.getLogger(__name__)
 
     def __init__(self):
         super().__init__()
         self.config = Configuration()
 
         user_config = self.config.read_config()
-        print(user_config)
         self.aws_profile = user_config.get("polly", {}).get("profile_name", "default")
         self.aws_region = user_config.get("polly", {}).get("region_name", "")
 
         self._layout = QGridLayout()
         self.setLayout(self._layout)
 
         # Name section "AWS Polly"
```

### Comparing `cracker-0.7.0/cracker.egg-info/PKG-INFO` & `cracker-0.7.1/cracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cracker
-Version: 0.7.0
+Version: 0.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
 Provides-Extra: test
 License-File: LICENSE
 
 # Cracker
```

### Comparing `cracker-0.7.0/cracker.egg-info/SOURCES.txt` & `cracker-0.7.1/cracker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .gitignore
-.python-version
 LICENSE
 Makefile
 README.md
 pyproject.toml
 .github/workflows/publish-pypi.yml
 cracker/__init__.py
 cracker/cracker.py
```

### Comparing `cracker-0.7.0/pyproject.toml` & `cracker-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/ubuntu/icon.png` & `cracker-0.7.1/ubuntu/icon.png`

 * *Files identical despite different names*

### Comparing `cracker-0.7.0/ubuntu/install_ubuntu.sh` & `cracker-0.7.1/ubuntu/install_ubuntu.sh`

 * *Files identical despite different names*

