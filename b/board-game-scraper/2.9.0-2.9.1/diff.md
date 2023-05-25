# Comparing `tmp/board-game-scraper-2.9.0.tar.gz` & `tmp/board-game-scraper-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/board-game-scraper-2.9.0.tar", last modified: Wed Aug 19 05:28:10 2020, max compression
+gzip compressed data, was "dist/board-game-scraper-2.9.1.tar", last modified: Mon Aug 24 07:23:46 2020, max compression
```

## Comparing `board-game-scraper-2.9.0.tar` & `board-game-scraper-2.9.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/
--rw-r--r--   0 markus     (501) staff       (20)     1072 2020-03-24 06:31:01.000000 board-game-scraper-2.9.0/LICENSE
--rw-r--r--   0 markus     (501) staff       (20)       68 2020-03-24 06:31:01.000000 board-game-scraper-2.9.0/MANIFEST.in
--rw-r--r--   0 markus     (501) staff       (20)     4047 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)     2363 2020-04-29 08:50:14.000000 board-game-scraper-2.9.0/README.md
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/board_game_scraper/
--rw-r--r--   0 markus     (501) staff       (20)      370 2020-04-29 08:50:14.000000 board-game-scraper-2.9.0/board_game_scraper/__init__.py
--rw-r--r--   0 markus     (501) staff       (20)     5350 2020-05-04 08:01:50.000000 board-game-scraper-2.9.0/board_game_scraper/__main__.py
--rw-r--r--   0 markus     (501) staff       (20)      103 2020-08-19 05:27:41.000000 board-game-scraper-2.9.0/board_game_scraper/__version__.py
--rw-r--r--   0 markus     (501) staff       (20)    11890 2020-04-29 08:50:14.000000 board-game-scraper-2.9.0/board_game_scraper/cluster.py
--rw-r--r--   0 markus     (501) staff       (20)     7841 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/extensions.py
--rw-r--r--   0 markus     (501) staff       (20)      608 2020-03-24 06:31:01.000000 board-game-scraper-2.9.0/board_game_scraper/fields.yaml
--rw-r--r--   0 markus     (501) staff       (20)     9360 2020-08-19 05:25:28.000000 board-game-scraper-2.9.0/board_game_scraper/full_merge.py
--rw-r--r--   0 markus     (501) staff       (20)    16790 2020-04-27 07:59:01.000000 board-game-scraper-2.9.0/board_game_scraper/items.py
--rw-r--r--   0 markus     (501) staff       (20)     1228 2020-04-27 07:59:01.000000 board-game-scraper-2.9.0/board_game_scraper/loaders.py
--rw-r--r--   0 markus     (501) staff       (20)    11394 2020-07-28 08:50:30.000000 board-game-scraper-2.9.0/board_game_scraper/merge.py
--rw-r--r--   0 markus     (501) staff       (20)     5627 2020-07-28 08:50:30.000000 board-game-scraper-2.9.0/board_game_scraper/news.py
--rw-r--r--   0 markus     (501) staff       (20)     5841 2020-04-27 07:59:01.000000 board-game-scraper-2.9.0/board_game_scraper/pipelines.py
--rwxr-xr-x   0 markus     (501) staff       (20)     5953 2020-03-24 06:31:01.000000 board-game-scraper-2.9.0/board_game_scraper/prefixes.py
--rw-r--r--   0 markus     (501) staff       (20)     8614 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/settings.py
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/
--rw-r--r--   0 markus     (501) staff       (20)        0 2020-03-24 06:31:01.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/__init__.py
--rw-r--r--   0 markus     (501) staff       (20)    10131 2020-07-07 12:00:42.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/bga.py
--rw-r--r--   0 markus     (501) staff       (20)    24256 2020-06-26 07:49:45.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/bgg.py
--rw-r--r--   0 markus     (501) staff       (20)     2457 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/bgg_hotness.py
--rw-r--r--   0 markus     (501) staff       (20)    10142 2020-04-27 07:59:01.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/bgg_rankings.py
--rw-r--r--   0 markus     (501) staff       (20)    25885 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/dbpedia.py
--rw-r--r--   0 markus     (501) staff       (20)     3593 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/luding.py
--rw-r--r--   0 markus     (501) staff       (20)     6070 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/spielen.py
--rw-r--r--   0 markus     (501) staff       (20)     9802 2020-04-14 11:15:22.000000 board-game-scraper-2.9.0/board_game_scraper/spiders/wikidata.py
--rw-r--r--   0 markus     (501) staff       (20)     4036 2020-04-29 08:50:14.000000 board-game-scraper-2.9.0/board_game_scraper/split.py
--rw-r--r--   0 markus     (501) staff       (20)    12284 2020-04-29 08:50:14.000000 board-game-scraper-2.9.0/board_game_scraper/utils.py
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/
--rw-r--r--   0 markus     (501) staff       (20)     4047 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)     1133 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 markus     (501) staff       (20)        1 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 markus     (501) staff       (20)      196 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/entry_points.txt
--rw-r--r--   0 markus     (501) staff       (20)      203 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/requires.txt
--rw-r--r--   0 markus     (501) staff       (20)       19 2020-08-19 05:28:08.000000 board-game-scraper-2.9.0/board_game_scraper.egg-info/top_level.txt
--rw-r--r--   0 markus     (501) staff       (20)       81 2020-04-13 13:58:01.000000 board-game-scraper-2.9.0/scrapy.cfg
--rw-r--r--   0 markus     (501) staff       (20)       38 2020-08-19 05:28:10.000000 board-game-scraper-2.9.0/setup.cfg
--rwxr-xr-x   0 markus     (501) staff       (20)     5044 2020-08-06 06:29:36.000000 board-game-scraper-2.9.0/setup.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/
+-rw-r--r--   0 markus     (501) staff       (20)     1072 2019-11-05 15:22:15.000000 board-game-scraper-2.9.1/LICENSE
+-rw-r--r--   0 markus     (501) staff       (20)       68 2019-11-13 09:33:14.000000 board-game-scraper-2.9.1/MANIFEST.in
+-rw-r--r--   0 markus     (501) staff       (20)     4047 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)     2363 2020-04-28 15:48:26.000000 board-game-scraper-2.9.1/README.md
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper/
+-rw-r--r--   0 markus     (501) staff       (20)      370 2020-04-19 20:14:35.000000 board-game-scraper-2.9.1/board_game_scraper/__init__.py
+-rw-r--r--   0 markus     (501) staff       (20)     5350 2020-05-26 05:10:28.000000 board-game-scraper-2.9.1/board_game_scraper/__main__.py
+-rw-r--r--   0 markus     (501) staff       (20)      103 2020-08-24 07:23:28.000000 board-game-scraper-2.9.1/board_game_scraper/__version__.py
+-rw-r--r--   0 markus     (501) staff       (20)    11890 2020-04-19 20:14:35.000000 board-game-scraper-2.9.1/board_game_scraper/cluster.py
+-rw-r--r--   0 markus     (501) staff       (20)     7841 2020-04-14 19:24:37.000000 board-game-scraper-2.9.1/board_game_scraper/extensions.py
+-rw-r--r--   0 markus     (501) staff       (20)      608 2019-11-13 09:33:14.000000 board-game-scraper-2.9.1/board_game_scraper/fields.yaml
+-rw-r--r--   0 markus     (501) staff       (20)     9360 2020-08-24 07:14:24.000000 board-game-scraper-2.9.1/board_game_scraper/full_merge.py
+-rw-r--r--   0 markus     (501) staff       (20)    16790 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/items.py
+-rw-r--r--   0 markus     (501) staff       (20)     1228 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/loaders.py
+-rw-r--r--   0 markus     (501) staff       (20)    11394 2020-07-25 07:05:11.000000 board-game-scraper-2.9.1/board_game_scraper/merge.py
+-rw-r--r--   0 markus     (501) staff       (20)     5627 2020-07-25 07:05:11.000000 board-game-scraper-2.9.1/board_game_scraper/news.py
+-rw-r--r--   0 markus     (501) staff       (20)     5841 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/pipelines.py
+-rwxr-xr-x   0 markus     (501) staff       (20)     5953 2019-11-11 08:40:01.000000 board-game-scraper-2.9.1/board_game_scraper/prefixes.py
+-rw-r--r--   0 markus     (501) staff       (20)     8614 2020-04-14 19:24:37.000000 board-game-scraper-2.9.1/board_game_scraper/settings.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/
+-rw-r--r--   0 markus     (501) staff       (20)        0 2019-11-05 15:22:15.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/__init__.py
+-rw-r--r--   0 markus     (501) staff       (20)    10131 2020-07-25 07:05:11.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/bga.py
+-rw-r--r--   0 markus     (501) staff       (20)    24256 2020-07-25 07:05:11.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/bgg.py
+-rw-r--r--   0 markus     (501) staff       (20)     2457 2020-04-05 20:32:19.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/bgg_hotness.py
+-rw-r--r--   0 markus     (501) staff       (20)    10142 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/bgg_rankings.py
+-rw-r--r--   0 markus     (501) staff       (20)    25885 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/dbpedia.py
+-rw-r--r--   0 markus     (501) staff       (20)     3593 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/luding.py
+-rw-r--r--   0 markus     (501) staff       (20)     6070 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/spielen.py
+-rw-r--r--   0 markus     (501) staff       (20)     9802 2020-04-11 20:24:29.000000 board-game-scraper-2.9.1/board_game_scraper/spiders/wikidata.py
+-rw-r--r--   0 markus     (501) staff       (20)     4036 2020-04-28 15:48:26.000000 board-game-scraper-2.9.1/board_game_scraper/split.py
+-rw-r--r--   0 markus     (501) staff       (20)    12284 2020-04-28 15:48:26.000000 board-game-scraper-2.9.1/board_game_scraper/utils.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/
+-rw-r--r--   0 markus     (501) staff       (20)     4047 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)     1133 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 markus     (501) staff       (20)        1 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 markus     (501) staff       (20)      196 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 markus     (501) staff       (20)      203 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/requires.txt
+-rw-r--r--   0 markus     (501) staff       (20)       19 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/board_game_scraper.egg-info/top_level.txt
+-rw-r--r--   0 markus     (501) staff       (20)       81 2019-11-05 15:22:15.000000 board-game-scraper-2.9.1/scrapy.cfg
+-rw-r--r--   0 markus     (501) staff       (20)       38 2020-08-24 07:23:46.000000 board-game-scraper-2.9.1/setup.cfg
+-rwxr-xr-x   0 markus     (501) staff       (20)     5044 2020-08-19 05:45:17.000000 board-game-scraper-2.9.1/setup.py
```

### Comparing `board-game-scraper-2.9.0/LICENSE` & `board-game-scraper-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/PKG-INFO` & `board-game-scraper-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-scraper
-Version: 2.9.0
+Version: 2.9.1
 Summary: Board games data scraping and processing from BoardGameGeek and more!
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-scraper/blob/master/README.md
 Project-URL: Source, https://gitlab.com/recommend.games/board-game-scraper
```

### Comparing `board-game-scraper-2.9.0/README.md` & `board-game-scraper-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/__main__.py` & `board-game-scraper-2.9.1/board_game_scraper/__main__.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/cluster.py` & `board-game-scraper-2.9.1/board_game_scraper/cluster.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/extensions.py` & `board-game-scraper-2.9.1/board_game_scraper/extensions.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/fields.yaml` & `board-game-scraper-2.9.1/board_game_scraper/fields.yaml`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/full_merge.py` & `board-game-scraper-2.9.1/board_game_scraper/full_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     curr_date_str = curr_date.strftime("%Y-%m-%dT%H-%M-%S")
 
     kwargs["in_paths"] = in_paths or FEEDS_DIR / spider / item / "*"
     kwargs.setdefault("keys", f"{spider}_id")
     kwargs.setdefault("key_types", "int" if spider in ("bgg", "luding") else "str")
     kwargs.setdefault("latest", "scraped_at")
     kwargs.setdefault("latest_types", "date")
-    kwargs.setdefault("latest_min", curr_date - timedelta(days=30))
+    kwargs.setdefault("latest_min", curr_date - timedelta(days=90))
     kwargs.setdefault("concat_output", True)
 
     if parse_bool(full):
         kwargs["out_path"] = (
             out_path or FEEDS_DIR / spider / item / f"{curr_date_str}-merged.jl"
         )
```

### Comparing `board-game-scraper-2.9.0/board_game_scraper/items.py` & `board-game-scraper-2.9.1/board_game_scraper/items.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/loaders.py` & `board-game-scraper-2.9.1/board_game_scraper/loaders.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/merge.py` & `board-game-scraper-2.9.1/board_game_scraper/merge.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/news.py` & `board-game-scraper-2.9.1/board_game_scraper/news.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/pipelines.py` & `board-game-scraper-2.9.1/board_game_scraper/pipelines.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/prefixes.py` & `board-game-scraper-2.9.1/board_game_scraper/prefixes.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/settings.py` & `board-game-scraper-2.9.1/board_game_scraper/settings.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/bga.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/bga.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/bgg.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/bgg.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/bgg_hotness.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/bgg_hotness.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/bgg_rankings.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/bgg_rankings.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/dbpedia.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/dbpedia.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/luding.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/luding.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/spielen.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/spielen.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/spiders/wikidata.py` & `board-game-scraper-2.9.1/board_game_scraper/spiders/wikidata.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/split.py` & `board-game-scraper-2.9.1/board_game_scraper/split.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper/utils.py` & `board-game-scraper-2.9.1/board_game_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/board_game_scraper.egg-info/PKG-INFO` & `board-game-scraper-2.9.1/board_game_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-scraper
-Version: 2.9.0
+Version: 2.9.1
 Summary: Board games data scraping and processing from BoardGameGeek and more!
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-scraper/blob/master/README.md
 Project-URL: Source, https://gitlab.com/recommend.games/board-game-scraper
```

### Comparing `board-game-scraper-2.9.0/board_game_scraper.egg-info/SOURCES.txt` & `board-game-scraper-2.9.1/board_game_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `board-game-scraper-2.9.0/setup.py` & `board-game-scraper-2.9.1/setup.py`

 * *Files identical despite different names*

