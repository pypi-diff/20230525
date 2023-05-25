# Comparing `tmp/pytubemusic-0.1.1.tar.gz` & `tmp/pytubemusic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubemusic-0.1.1.tar", last modified: Mon Apr 17 20:58:29 2023, max compression
+gzip compressed data, was "pytubemusic-0.1.2.tar", last modified: Thu May 25 09:06:57 2023, max compression
```

## Comparing `pytubemusic-0.1.1.tar` & `pytubemusic-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.173236 pytubemusic-0.1.1/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.1.1/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4799 2023-04-17 20:58:29.173078 pytubemusic-0.1.1/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3092 2023-04-17 20:40:33.000000 pytubemusic-0.1.1/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-04-17 20:57:47.000000 pytubemusic-0.1.1/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-04-17 20:36:11.000000 pytubemusic-0.1.1/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-04-17 20:58:29.173275 pytubemusic-0.1.1/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.168256 pytubemusic-0.1.1/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.170516 pytubemusic-0.1.1/src/pytubemusic/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.1.1/src/pytubemusic/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3428 2023-04-17 20:41:20.000000 pytubemusic-0.1.1/src/pytubemusic/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2005 2023-04-17 20:36:11.000000 pytubemusic-0.1.1/src/pytubemusic/audio.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3185 2023-04-16 01:35:20.000000 pytubemusic-0.1.1/src/pytubemusic/logutils.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6017 2023-04-17 20:32:15.000000 pytubemusic-0.1.1/src/pytubemusic/track.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3625 2023-04-16 01:34:45.000000 pytubemusic-0.1.1/src/pytubemusic/utils.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.171687 pytubemusic-0.1.1/src/pytubemusic/validation/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1143 2023-04-16 03:47:20.000000 pytubemusic-0.1.1/src/pytubemusic/validation/__init__.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.172450 pytubemusic-0.1.1/src/pytubemusic/validation/schemata/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1879 2023-04-16 01:15:44.000000 pytubemusic-0.1.1/src/pytubemusic/validation/schemata/album.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1830 2023-04-16 01:20:40.000000 pytubemusic-0.1.1/src/pytubemusic/validation/schemata/playlist.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1189 2023-04-16 01:15:44.000000 pytubemusic-0.1.1/src/pytubemusic/validation/schemata/track.schema.json
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.171558 pytubemusic-0.1.1/src/pytubemusic.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4799 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      668 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-04-17 20:58:29.000000 pytubemusic-0.1.1/src/pytubemusic.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-17 20:58:29.172686 pytubemusic-0.1.1/tests/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.128493 pytubemusic-0.1.2/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.1.2/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5274 2023-05-25 09:06:57.128340 pytubemusic-0.1.2/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3567 2023-05-25 09:05:25.000000 pytubemusic-0.1.2/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-05-25 09:06:40.000000 pytubemusic-0.1.2/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 08:59:56.000000 pytubemusic-0.1.2/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-05-25 09:06:57.128535 pytubemusic-0.1.2/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.123354 pytubemusic-0.1.2/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.125565 pytubemusic-0.1.2/src/pytubemusic/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.1.2/src/pytubemusic/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3428 2023-04-17 20:41:20.000000 pytubemusic-0.1.2/src/pytubemusic/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2005 2023-04-17 20:36:11.000000 pytubemusic-0.1.2/src/pytubemusic/audio.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3185 2023-04-16 01:35:20.000000 pytubemusic-0.1.2/src/pytubemusic/logutils.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5710 2023-05-09 07:34:40.000000 pytubemusic-0.1.2/src/pytubemusic/track.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3625 2023-04-16 01:34:45.000000 pytubemusic-0.1.2/src/pytubemusic/utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.126680 pytubemusic-0.1.2/src/pytubemusic/validation/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1143 2023-04-16 03:47:20.000000 pytubemusic-0.1.2/src/pytubemusic/validation/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.127756 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1879 2023-04-16 01:15:44.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/album.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1830 2023-04-16 01:20:40.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/playlist.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1189 2023-04-16 01:15:44.000000 pytubemusic-0.1.2/src/pytubemusic/validation/schemata/track.schema.json
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.126567 pytubemusic-0.1.2/src/pytubemusic.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5274 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      668 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-05-25 09:06:57.000000 pytubemusic-0.1.2/src/pytubemusic.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-25 09:06:57.127964 pytubemusic-0.1.2/tests/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.1.2/tests/test_utils.py
```

### Comparing `pytubemusic-0.1.1/LICENSE` & `pytubemusic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/PKG-INFO` & `pytubemusic-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,14 +40,27 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
+### Installation Note
+
+PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
+can occasionally break. However, patches are usually quickly released as new
+versions or as pull requests. Try upgrading to the latest version of PyTube if
+downloading fails.
+
+> Note, to pip install from a pull request do:
+> ```text
+>  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
+> ```
+> Where `<PR_NUM>` is the number of the pull request.
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
```

### Comparing `pytubemusic-0.1.1/README.md` & `pytubemusic-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
+### Installation Note
+
+PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
+can occasionally break. However, patches are usually quickly released as new
+versions or as pull requests. Try upgrading to the latest version of PyTube if
+downloading fails.
+
+> Note, to pip install from a pull request do:
+> ```text
+>  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
+> ```
+> Where `<PR_NUM>` is the number of the pull request.
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
```

### Comparing `pytubemusic-0.1.1/pyproject.toml` & `pytubemusic-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubemusic"
-version = "0.1.1"
+version = "0.1.2"
 description = 'A cli that may or may not download albums from a certain website'
 
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `pytubemusic-0.1.1/src/pytubemusic/__main__.py` & `pytubemusic-0.1.2/src/pytubemusic/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/audio.py` & `pytubemusic-0.1.2/src/pytubemusic/audio.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/logutils.py` & `pytubemusic-0.1.2/src/pytubemusic/logutils.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/track.py` & `pytubemusic-0.1.2/src/pytubemusic/track.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from datetime import timedelta
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any, Self
 
-import backoff
 from pipe_utils import Pipe
-from pytube import Playlist, YouTube
-from pytube.exceptions import PytubeError
+from pytube import Playlist
 
 from pytubemusic.audio import Audio
 from pytubemusic.logutils import log_call
 from pytubemusic.utils import *
 
 __all__ = ["Track"]
 
@@ -160,19 +158,12 @@
         for i, (video, data) in enumerate(video_data, start=1):
             yield cls.from_video(
                 video.watch_url,
                 cover_url=cover_url,
                 metadata={
                     **metadata,
                     "track": i,
-                    # Hack to avoid issues with titles not being
-                    # found on playlist videos
-                    "title": get_title(video.watch_url),
+                    "title": video.title,
                     **data.get("metadata", {}),
                 },
                 **{k: v for k, v in data.items() if k != "metadata"},
             )
-
-
-@backoff.on_exception(backoff.expo, PytubeError, max_tries=5)
-def get_title(url):
-    return YouTube(url).title
```

### Comparing `pytubemusic-0.1.1/src/pytubemusic/utils.py` & `pytubemusic-0.1.2/src/pytubemusic/utils.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/validation/__init__.py` & `pytubemusic-0.1.2/src/pytubemusic/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/validation/schemata/album.schema.json` & `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/album.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/validation/schemata/playlist.schema.json` & `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/playlist.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic/validation/schemata/track.schema.json` & `pytubemusic-0.1.2/src/pytubemusic/validation/schemata/track.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/src/pytubemusic.egg-info/PKG-INFO` & `pytubemusic-0.1.2/src/pytubemusic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,14 +40,27 @@
 
 ```
 pip install pytubemusic
 ```
 
 **Requires [ffmpeg](https://ffmpeg.org/) to be installed on your machine.**
 
+### Installation Note
+
+PyTubeMusic uses the [PyTube](https://github.com/pytube/pytube) library. This
+can occasionally break. However, patches are usually quickly released as new
+versions or as pull requests. Try upgrading to the latest version of PyTube if
+downloading fails.
+
+> Note, to pip install from a pull request do:
+> ```text
+>  pip install git+https://github.com/pytube/pytube.git@refs/pull/<PR_NUM>/head
+> ```
+> Where `<PR_NUM>` is the number of the pull request.
+
 ## Usage
 
 PyTubeMusic can download tracks in three formats:
 
 - Tracks (Single files)
 - Albums (A single video that is split up into individual tracks on an album)
 - Playlists (Videos in a playlist that are downloaded as tracks on an album)
```

### Comparing `pytubemusic-0.1.1/src/pytubemusic.egg-info/SOURCES.txt` & `pytubemusic-0.1.2/src/pytubemusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.1.1/tests/test_utils.py` & `pytubemusic-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

