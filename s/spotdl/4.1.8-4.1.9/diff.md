# Comparing `tmp/spotdl-4.1.8.tar.gz` & `tmp/spotdl-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl-4.1.8.tar", max compression
+gzip compressed data, was "spotdl-4.1.9.tar", max compression
```

## Comparing `spotdl-4.1.8.tar` & `spotdl-4.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1074 2023-04-23 15:56:46.642111 spotdl-4.1.8/LICENSE
--rw-r--r--   0        0        0     5977 2023-04-23 15:56:46.642111 spotdl-4.1.8/README.md
--rw-r--r--   0        0        0     2747 2023-04-23 15:56:46.646111 spotdl-4.1.8/pyproject.toml
--rw-r--r--   0        0        0     4668 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/__init__.py
--rw-r--r--   0        0        0      209 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/__main__.py
--rw-r--r--   0        0        0       58 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/_version.py
--rw-r--r--   0        0        0      186 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/__init__.py
--rw-r--r--   0        0        0      598 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/download.py
--rw-r--r--   0        0        0     4120 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/entry_point.py
--rw-r--r--   0        0        0     5995 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/meta.py
--rw-r--r--   0        0        0     2759 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/save.py
--rw-r--r--   0        0        0     5067 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/sync.py
--rw-r--r--   0        0        0     1702 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/url.py
--rw-r--r--   0        0        0     3041 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/console/web.py
--rw-r--r--   0        0        0       80 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/__init__.py
--rw-r--r--   0        0        0    27263 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/downloader.py
--rw-r--r--   0        0        0    13137 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/download/progress_handler.py
--rw-r--r--   0        0        0       54 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/__init__.py
--rw-r--r--   0        0        0      465 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/__init__.py
--rw-r--r--   0        0        0    11137 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/base.py
--rw-r--r--   0        0        0     2665 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     1840 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/youtube.py
--rw-r--r--   0        0        0     2789 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3304 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3529 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/base.py
--rw-r--r--   0        0        0     3091 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/genius.py
--rw-r--r--   0        0        0     2765 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     1689 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/album.py
--rw-r--r--   0        0        0     3101 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/artist.py
--rw-r--r--   0        0        0     3871 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/options.py
--rw-r--r--   0        0        0     4199 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/playlist.py
--rw-r--r--   0        0        0     2186 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/result.py
--rw-r--r--   0        0        0     3230 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/saved.py
--rw-r--r--   0        0        0     9758 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/types/song.py
--rw-r--r--   0        0        0      103 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/__init__.py
--rw-r--r--   0        0        0     1001 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/archive.py
--rw-r--r--   0        0        0    19690 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/arguments.py
--rw-r--r--   0        0        0     6994 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/config.py
--rw-r--r--   0        0        0     3109 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/console.py
--rw-r--r--   0        0        0      571 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/downloader.py
--rw-r--r--   0        0        0    11688 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/ffmpeg.py
--rw-r--r--   0        0        0    14271 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/formatter.py
--rw-r--r--   0        0        0     7018 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/github.py
--rw-r--r--   0        0        0     5364 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/logging.py
--rw-r--r--   0        0        0      940 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/lrc.py
--rw-r--r--   0        0        0     4144 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/m3u.py
--rw-r--r--   0        0        0    23312 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/matching.py
--rw-r--r--   0        0        0    15621 2023-04-23 15:56:46.646111 spotdl-4.1.8/spotdl/utils/metadata.py
--rw-r--r--   0        0        0    15347 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/search.py
--rw-r--r--   0        0        0     6870 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/spotify.py
--rw-r--r--   0        0        0    28221 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/static.py
--rw-r--r--   0        0        0    15281 2023-04-23 15:56:46.650111 spotdl-4.1.8/spotdl/utils/web.py
--rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 spotdl-4.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-01 11:50:54.916794 spotdl-4.1.9/LICENSE
+-rw-r--r--   0        0        0     5977 2023-05-01 11:50:54.916794 spotdl-4.1.9/README.md
+-rw-r--r--   0        0        0     2745 2023-05-01 11:50:54.920794 spotdl-4.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4668 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/__main__.py
+-rw-r--r--   0        0        0       58 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/_version.py
+-rw-r--r--   0        0        0      186 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/__init__.py
+-rw-r--r--   0        0        0      598 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/download.py
+-rw-r--r--   0        0        0     4120 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/entry_point.py
+-rw-r--r--   0        0        0     5995 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/meta.py
+-rw-r--r--   0        0        0     2759 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/save.py
+-rw-r--r--   0        0        0     5067 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/sync.py
+-rw-r--r--   0        0        0     1702 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/url.py
+-rw-r--r--   0        0        0     3041 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/console/web.py
+-rw-r--r--   0        0        0       80 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/__init__.py
+-rw-r--r--   0        0        0    27263 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/downloader.py
+-rw-r--r--   0        0        0    13137 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/__init__.py
+-rw-r--r--   0        0        0      465 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/__init__.py
+-rw-r--r--   0        0        0    11137 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/base.py
+-rw-r--r--   0        0        0     2665 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     1840 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2789 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      382 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3304 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3529 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3091 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     2765 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     1689 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/__init__.py
+-rw-r--r--   0        0        0     3451 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/album.py
+-rw-r--r--   0        0        0     3101 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/artist.py
+-rw-r--r--   0        0        0     3871 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/options.py
+-rw-r--r--   0        0        0     4199 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/playlist.py
+-rw-r--r--   0        0        0     2186 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/result.py
+-rw-r--r--   0        0        0     3230 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/saved.py
+-rw-r--r--   0        0        0     9758 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/types/song.py
+-rw-r--r--   0        0        0      103 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2023-05-01 11:50:54.920794 spotdl-4.1.9/spotdl/utils/archive.py
+-rw-r--r--   0        0        0    19690 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/arguments.py
+-rw-r--r--   0        0        0     6994 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/config.py
+-rw-r--r--   0        0        0     3109 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/console.py
+-rw-r--r--   0        0        0      571 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/downloader.py
+-rw-r--r--   0        0        0    11688 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/ffmpeg.py
+-rw-r--r--   0        0        0    14271 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/formatter.py
+-rw-r--r--   0        0        0     7018 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/github.py
+-rw-r--r--   0        0        0     5364 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/logging.py
+-rw-r--r--   0        0        0      940 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/lrc.py
+-rw-r--r--   0        0        0     4144 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/m3u.py
+-rw-r--r--   0        0        0    23312 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/matching.py
+-rw-r--r--   0        0        0    15621 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/metadata.py
+-rw-r--r--   0        0        0    15570 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/search.py
+-rw-r--r--   0        0        0     6870 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/static.py
+-rw-r--r--   0        0        0    15281 2023-05-01 11:50:54.924795 spotdl-4.1.9/spotdl/utils/web.py
+-rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 spotdl-4.1.9/PKG-INFO
```

### Comparing `spotdl-4.1.8/LICENSE` & `spotdl-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/README.md` & `spotdl-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/pyproject.toml` & `spotdl-4.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl"
-version = "4.1.8"
+version = "4.1.9"
 description = "Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/spotDL/spotify-downloader.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
@@ -32,57 +32,57 @@
 ytmusicapi = [
     {version = "^0.22.0", python = "<3.8"},
     {version = "^0.24.0", python = ">=3.8"},
 ]
 pytube = "^12.1.3"
 yt-dlp = "^2023.3.4"
 mutagen = "^1.46.0"
-rich = "^13.3.4"
+rich = "^13.3.5"
 beautifulsoup4 = "^4.12.2"
-requests = "^2.28.2"
+requests = "^2.29.0"
 rapidfuzz = "==2.15.1"
 python-slugify = {extras = ["unidecode"], version = "^8.0.1"}
-uvicorn = "^0.21.1"
+uvicorn = "^0.22.0"
 pydantic = "^1.10.7"
 fastapi = "^0.95.1"
-platformdirs = "^3.2.0"
+platformdirs = "^3.5.0"
 pykakasi = "^2.2.1"
 syncedlyrics = "^0.5.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-vcr = "^1.0.2"
 pyfakefs = "^5.2.2"
 pytest-cov = "^4.0.0"
 pytest-subprocess = "^1.5.0"
 pytest-asyncio = "^0.21.0"
 mypy = "^1.2.0"
-pylint = "^2.17.2"
+pylint = "^2.17.3"
 black = "^23.3.0"
 mdformat-gfm = "^0.3.5"
 types-orjson = "^3.6.2"
 types-python-slugify = "^8.0.0.2"
-types-requests = "^2.28.11.17"
+types-requests = "^2.29.0.0"
 types-setuptools = "^67.7.0.0"
 types-toml = "^0.10.8.6"
-types-ujson = "^5.7.0.3"
+types-ujson = "^5.7.0.4"
 pyinstaller = "^5.10.1"
 mkdocs = "^1.4.2"
 isort = [
     {version = "^5.11.4", python = "<3.8"},
     {version = "^5.12.0", python = ">=3.8"},
 ]
 dill = "^0.3.6"
-mkdocs-material = "^9.1.7"
+mkdocs-material = "^9.1.8"
 mkdocstrings = "^0.21.2"
 mkdocstrings-python = "^0.9.0"
 pymdown-extensions = "^9.11"
-mkdocs-gen-files = "^0.4.0"
+mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 
 [tool.poetry.scripts]
 spotdl = "spotdl:console_entry_point"
 
 [tool.isort]
```

### Comparing `spotdl-4.1.8/spotdl/__init__.py` & `spotdl-4.1.9/spotdl/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/download.py` & `spotdl-4.1.9/spotdl/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/entry_point.py` & `spotdl-4.1.9/spotdl/console/entry_point.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/meta.py` & `spotdl-4.1.9/spotdl/console/meta.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/save.py` & `spotdl-4.1.9/spotdl/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/sync.py` & `spotdl-4.1.9/spotdl/console/sync.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/url.py` & `spotdl-4.1.9/spotdl/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/console/web.py` & `spotdl-4.1.9/spotdl/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/download/downloader.py` & `spotdl-4.1.9/spotdl/download/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/download/progress_handler.py` & `spotdl-4.1.9/spotdl/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/audio/base.py` & `spotdl-4.1.9/spotdl/providers/audio/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/audio/sliderkz.py` & `spotdl-4.1.9/spotdl/providers/audio/sliderkz.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/audio/youtube.py` & `spotdl-4.1.9/spotdl/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/audio/ytmusic.py` & `spotdl-4.1.9/spotdl/providers/audio/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/lyrics/azlyrics.py` & `spotdl-4.1.9/spotdl/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/lyrics/base.py` & `spotdl-4.1.9/spotdl/providers/lyrics/base.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/lyrics/genius.py` & `spotdl-4.1.9/spotdl/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/lyrics/musixmatch.py` & `spotdl-4.1.9/spotdl/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/providers/lyrics/synced.py` & `spotdl-4.1.9/spotdl/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/album.py` & `spotdl-4.1.9/spotdl/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/artist.py` & `spotdl-4.1.9/spotdl/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/options.py` & `spotdl-4.1.9/spotdl/types/options.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/playlist.py` & `spotdl-4.1.9/spotdl/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/result.py` & `spotdl-4.1.9/spotdl/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/saved.py` & `spotdl-4.1.9/spotdl/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/types/song.py` & `spotdl-4.1.9/spotdl/types/song.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/archive.py` & `spotdl-4.1.9/spotdl/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/arguments.py` & `spotdl-4.1.9/spotdl/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/config.py` & `spotdl-4.1.9/spotdl/utils/config.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/console.py` & `spotdl-4.1.9/spotdl/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/downloader.py` & `spotdl-4.1.9/spotdl/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/ffmpeg.py` & `spotdl-4.1.9/spotdl/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/formatter.py` & `spotdl-4.1.9/spotdl/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/github.py` & `spotdl-4.1.9/spotdl/utils/github.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/logging.py` & `spotdl-4.1.9/spotdl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/lrc.py` & `spotdl-4.1.9/spotdl/utils/lrc.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/m3u.py` & `spotdl-4.1.9/spotdl/utils/m3u.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/matching.py` & `spotdl-4.1.9/spotdl/utils/matching.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/metadata.py` & `spotdl-4.1.9/spotdl/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/search.py` & `spotdl-4.1.9/spotdl/utils/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,17 @@
 
                     lists.append(ytm_list)
                 else:
                     for index, song in enumerate(spot_list.songs):
                         song.download_url = ytm_list.songs[index].download_url
 
                     lists.append(spot_list)
+        elif "open.spotify.com/intl-" in request and "track" in request:
+            request = request.split("/intl-")[0] + "/track" + request.split("/track")[1]
+            songs.append(Song.from_url(url=request))
         elif "open.spotify.com" in request and "track" in request:
             songs.append(Song.from_url(url=request))
         elif "https://spotify.link/" in request:
             resp = requests.head(request, allow_redirects=True, timeout=10)
             songs.append(Song.from_url(url=resp.url))
         elif "open.spotify.com" in request and "playlist" in request:
             lists.append(Playlist.from_url(request, fetch_songs=False))
@@ -465,16 +468,16 @@
         song = Song.from_missing_data(
             name=track["title"],
             artists=[artist["name"] for artist in track["artists"]],
             artist=track["artists"][0]["name"],
             album_name=track.get("album", {}).get("name")
             if track.get("album") is not None
             else None,
-            duration=track["duration_seconds"],
-            explicit=track["isExplicit"],
+            duration=track.get("duration_seconds"),
+            explicit=track.get("isExplicit"),
             download_url=f"https://music.youtube.com/watch?v={track['videoId']}",
         )
 
         if fetch_songs:
             song = reinit_song(song)
 
         songs.append(song)
```

### Comparing `spotdl-4.1.8/spotdl/utils/spotify.py` & `spotdl-4.1.9/spotdl/utils/spotify.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/static.py` & `spotdl-4.1.9/spotdl/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/spotdl/utils/web.py` & `spotdl-4.1.9/spotdl/utils/web.py`

 * *Files identical despite different names*

### Comparing `spotdl-4.1.8/PKG-INFO` & `spotdl-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl
-Version: 4.1.8
+Version: 4.1.9
 Summary: Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
@@ -26,26 +26,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
-Requires-Dist: platformdirs (>=3.2.0,<4.0.0)
+Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pykakasi (>=2.2.1,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
 Requires-Dist: rapidfuzz (==2.15.1)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: spotipy (>=2.23.0,<3.0.0)
 Requires-Dist: syncedlyrics (>=0.5.0,<0.6.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Requires-Dist: ytmusicapi (>=0.22.0,<0.23.0) ; python_version < "3.8"
 Requires-Dist: ytmusicapi (>=0.24.0,<0.25.0) ; python_version >= "3.8"
 Project-URL: Documentation, https://spotdl.rtfd.io/en/latest/
 Project-URL: Repository, https://github.com/spotDL/spotify-downloader.git
 Description-Content-Type: text/markdown
```

