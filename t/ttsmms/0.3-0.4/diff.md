# Comparing `tmp/ttsmms-0.3.tar.gz` & `tmp/ttsmms-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttsmms-0.3.tar", last modified: Tue May 23 06:00:53 2023, max compression
+gzip compressed data, was "ttsmms-0.4.tar", last modified: Thu May 25 06:42:09 2023, max compression
```

## Comparing `ttsmms-0.3.tar` & `ttsmms-0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:00:53.541065 ttsmms-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 06:00:42.000000 ttsmms-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 06:00:53.541065 ttsmms-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 06:00:42.000000 ttsmms-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:00:53.541065 ttsmms-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 06:00:42.000000 ttsmms-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:00:53.541065 ttsmms-0.3/ttsmms/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-23 06:00:42.000000 ttsmms-0.3/ttsmms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-23 06:00:42.000000 ttsmms-0.3/ttsmms/attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-23 06:00:42.000000 ttsmms-0.3/ttsmms/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-05-23 06:00:42.000000 ttsmms-0.3/ttsmms/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/mel_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:00:53.541065 ttsmms-0.3/ttsmms/text/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/text/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-23 06:00:43.000000 ttsmms-0.3/ttsmms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:00:53.541065 ttsmms-0.3/ttsmms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 06:00:53.000000 ttsmms-0.3/ttsmms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:42:09.530291 ttsmms-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 06:41:54.000000 ttsmms-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 06:42:09.526291 ttsmms-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 06:41:54.000000 ttsmms-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:42:09.530291 ttsmms-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-25 06:41:54.000000 ttsmms-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:42:09.526291 ttsmms-0.4/ttsmms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15055 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/mel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:42:09.526291 ttsmms-0.4/ttsmms/text/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/text/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-25 06:41:54.000000 ttsmms-0.4/ttsmms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:42:09.526291 ttsmms-0.4/ttsmms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 06:42:09.000000 ttsmms-0.4/ttsmms.egg-info/top_level.txt
```

### Comparing `ttsmms-0.3/LICENSE` & `ttsmms-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/PKG-INFO` & `ttsmms-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.3
+Version: 0.4
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
@@ -21,22 +21,22 @@
 License-File: LICENSE
 
 # ttsmms
 Text-to-speech with The Massively Multilingual Speech (MMS) project
 
 This project want to help you for use Text-to-speech model from MMS project in Python.
 
-Support 1,143 Languages! (See support_list.txt)
+Support 1,107 Languages! (See support_list.txt)
 
 - VITS: [GitHub](https://github.com/jaywalnut310/vits)
 - MMS: Scaling Speech Technology to 1000+ languages: [GitHub](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)
 
 [Google colab](https://colab.research.google.com/github/wannaphong/ttsmms/blob/main/notebook/test.ipynb)
 
-**Don't forget the TTS model in MMS project use CC-BY-ND license.**
+**Don't forget the TTS model in MMS project use CC-BY-NC license.**
 
 ## Install
 
 > pip install ttsmms
 
 
 ## Usage
```

### Comparing `ttsmms-0.3/README.md` & `ttsmms-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ttsmms
 Text-to-speech with The Massively Multilingual Speech (MMS) project
 
 This project want to help you for use Text-to-speech model from MMS project in Python.
 
-Support 1,143 Languages! (See support_list.txt)
+Support 1,107 Languages! (See support_list.txt)
 
 - VITS: [GitHub](https://github.com/jaywalnut310/vits)
 - MMS: Scaling Speech Technology to 1000+ languages: [GitHub](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)
 
 [Google colab](https://colab.research.google.com/github/wannaphong/ttsmms/blob/main/notebook/test.ipynb)
 
-**Don't forget the TTS model in MMS project use CC-BY-ND license.**
+**Don't forget the TTS model in MMS project use CC-BY-NC license.**
 
 ## Install
 
 > pip install ttsmms
 
 
 ## Usage
```

### Comparing `ttsmms-0.3/setup.py` & `ttsmms-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "torchvision",
     "Unidecode",
     "monotonic-align"
 ]
 
 setup(
     name="ttsmms",
-    version="0.3",
+    version="0.4",
     description="Text-to-speech with The Massively Multilingual Speech (MMS) project",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/ttsmms",
     packages=find_packages(),
```

### Comparing `ttsmms-0.3/ttsmms/__init__.py` & `ttsmms-0.4/ttsmms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import argparse
 from ttsmms.data_utils import TextAudioLoader, TextAudioCollate, TextAudioSpeakerLoader, TextAudioSpeakerCollate
 from ttsmms.models import SynthesizerTrn
 from scipy.io.wavfile import write
 
 class TextMapper(object):
     def __init__(self, vocab_file):
-        self.symbols = [x.replace("\n", "") for x in open(vocab_file).readlines()]
+        self.symbols = [x.replace("\n", "") for x in open(vocab_file, encoding="utf-8").readlines()]
         self.SPACE_ID = self.symbols.index(" ")
         self._symbol_to_id = {s: i for i, s in enumerate(self.symbols)}
         self._id_to_symbol = {i: s for i, s in enumerate(self.symbols)}
 
     def text_to_sequence(self, text, cleaner_names):
         '''Converts a string of text to a sequence of IDs corresponding to the symbols in the text.
         Args:
```

### Comparing `ttsmms-0.3/ttsmms/attentions.py` & `ttsmms-0.4/ttsmms/attentions.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/commons.py` & `ttsmms-0.4/ttsmms/commons.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/data_utils.py` & `ttsmms-0.4/ttsmms/data_utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/losses.py` & `ttsmms-0.4/ttsmms/losses.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/mel_processing.py` & `ttsmms-0.4/ttsmms/mel_processing.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/models.py` & `ttsmms-0.4/ttsmms/models.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/modules.py` & `ttsmms-0.4/ttsmms/modules.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/preprocess.py` & `ttsmms-0.4/ttsmms/preprocess.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/text/__init__.py` & `ttsmms-0.4/ttsmms/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/text/cleaners.py` & `ttsmms-0.4/ttsmms/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/text/symbols.py` & `ttsmms-0.4/ttsmms/text/symbols.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/transforms.py` & `ttsmms-0.4/ttsmms/transforms.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms/utils.py` & `ttsmms-0.4/ttsmms/utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.3/ttsmms.egg-info/PKG-INFO` & `ttsmms-0.4/ttsmms.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.3
+Version: 0.4
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
@@ -21,22 +21,22 @@
 License-File: LICENSE
 
 # ttsmms
 Text-to-speech with The Massively Multilingual Speech (MMS) project
 
 This project want to help you for use Text-to-speech model from MMS project in Python.
 
-Support 1,143 Languages! (See support_list.txt)
+Support 1,107 Languages! (See support_list.txt)
 
 - VITS: [GitHub](https://github.com/jaywalnut310/vits)
 - MMS: Scaling Speech Technology to 1000+ languages: [GitHub](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)
 
 [Google colab](https://colab.research.google.com/github/wannaphong/ttsmms/blob/main/notebook/test.ipynb)
 
-**Don't forget the TTS model in MMS project use CC-BY-ND license.**
+**Don't forget the TTS model in MMS project use CC-BY-NC license.**
 
 ## Install
 
 > pip install ttsmms
 
 
 ## Usage
```

