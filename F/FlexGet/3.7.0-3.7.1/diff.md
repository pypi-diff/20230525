# Comparing `tmp/FlexGet-3.7.0.tar.gz` & `tmp/FlexGet-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-3784uq3o/FlexGet-3.7.0.tar", last modified: Thu May 11 03:12:52 2023, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-a46h_m61/FlexGet-3.7.1.tar", last modified: Thu May 25 15:12:12 2023, max compression
```

## Comparing `FlexGet-3.7.0.tar` & `FlexGet-3.7.1.tar`

### file list

```diff
@@ -1,982 +1,982 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 03:12:52.000000 FlexGet-3.7.0/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-11 03:12:30.000000 FlexGet-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 03:12:30.000000 FlexGet-3.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-11 03:12:52.000000 FlexGet-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-11 03:12:30.000000 FlexGet-3.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-11 03:12:30.000000 FlexGet-3.7.0/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-11 03:12:30.000000 FlexGet-3.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-11 03:12:42.000000 FlexGet-3.7.0/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83287 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/plex_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47009 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    56988 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26049 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42193 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    42591 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    40203 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-05-11 03:12:43.000000 FlexGet-3.7.0/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-11 03:12:45.000000 FlexGet-3.7.0/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 03:12:52.000000 FlexGet-3.7.0/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16956 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-11 03:12:30.000000 FlexGet-3.7.0/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-11 03:12:30.000000 FlexGet-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-11 03:12:30.000000 FlexGet-3.7.0/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-11 03:12:30.000000 FlexGet-3.7.0/requirements-release.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-11 03:12:30.000000 FlexGet-3.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 03:12:52.000000 FlexGet-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39131 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 15:12:12.000000 FlexGet-3.7.1/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 15:11:47.000000 FlexGet-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 15:11:47.000000 FlexGet-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 15:12:12.000000 FlexGet-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-25 15:11:47.000000 FlexGet-3.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-25 15:11:47.000000 FlexGet-3.7.1/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-25 15:11:47.000000 FlexGet-3.7.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 15:11:57.000000 FlexGet-3.7.1/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83806 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23176 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57306 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53392 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31634 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25915 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40203 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25048 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22421 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-05-25 15:11:58.000000 FlexGet-3.7.1/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-25 15:12:03.000000 FlexGet-3.7.1/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:12:12.000000 FlexGet-3.7.1/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28524 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19296 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-25 15:11:47.000000 FlexGet-3.7.1/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-25 15:11:47.000000 FlexGet-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-25 15:11:47.000000 FlexGet-3.7.1/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-25 15:11:47.000000 FlexGet-3.7.1/requirements-release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-25 15:11:47.000000 FlexGet-3.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:12:12.000000 FlexGet-3.7.1/setup.cfg
```

### Comparing `FlexGet-3.7.0/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.7.1/FlexGet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.0
+Version: 3.7.1
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.0/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.7.1/FlexGet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/FlexGet.egg-info/requires.txt` & `FlexGet-3.7.1/requirements-release.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,35 @@
-
-[:python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"]
-greenlet==2.0.1
-
-[:python_version >= "3.7" and python_version < "3.10"]
-importlib-metadata==6.1.0
-zipp==3.11.0
-
-[:python_version >= "3.7" and python_version < "3.9"]
-backports-zoneinfo==0.2.1
-importlib-resources==5.10.1
-pkgutil-resolve-name==1.3.10
-
-[:python_version >= "3.7" and python_version < "4"]
-apscheduler==3.9.1.post1
-certifi==2022.12.7
-charset-normalizer==2.1.1
-idna==3.4
-pytz-deprecation-shim==0.1.0.post0
-pytz==2022.6
-requests==2.28.1
-setuptools==65.6.3
-six==1.16.0
-tzdata==2022.7
-tzlocal==4.2
-urllib3==1.26.13
-
-[:python_version >= "3.7" and python_version < "4.0"]
-aniso8601==9.0.1
-attrs==22.1.0
-autocommand==2.2.2
-babelfish==0.6.0
-beautifulsoup4==4.11.1
-brotli==1.0.9
-cheroot==9.0.0
-cherrypy==18.8.0
-click==8.1.3
-colorama==0.4.6
-commonmark==0.9.1
-feedparser==6.0.10
-flask-compress==1.13
-flask-cors==3.0.10
-flask-login==0.6.2
-flask-restful==0.3.9
-flask-restx==1.0.3
-flask==2.2.5
-guessit==3.5.0
-html5lib==1.1
-inflect==6.0.2
-itsdangerous==2.1.2
-jaraco-classes==3.2.3
-jaraco-collections==3.8.0
-jaraco-context==4.2.0
-jaraco-functools==3.5.2
-jaraco-text==3.11.0
-jinja2==3.1.2
-jsonschema==4.17.3
-loguru==0.6.0
-markupsafe==2.1.1
-more-itertools==9.0.0
-packaging==22.0
-plumbum==1.8.0
-portend==3.1.0
-psutil==5.9.4
-pydantic==1.10.2
-pygments==2.13.0
-pynzb==0.1.0
-pyparsing==3.0.9
-pyrsistent==0.19.2
-pyrss2gen==1.1
-python-dateutil==2.8.2
-pyyaml==6.0
-rebulk==3.1.0
-rich==12.6.0
-rpyc==5.3.1
-sgmllib3k==1.0.0
-soupsieve==2.3.2.post1
-sqlalchemy==1.4.45
-tempora==5.1.0
-typing-extensions==4.4.0
-webencodings==0.5.1
-werkzeug==2.2.3
-zc-lockfile==2.0
-zxcvbn-python==4.4.24
-
-[:python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"]
-win32-setctime==1.1.0
-
-[:sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"]
-pywin32==305
+bleach==5.0.1 ; python_version >= "3.7" and python_version < "4.0"
+build==0.9.0 ; python_version >= "3.7" and python_version < "4.0"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4.0"
+cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
+click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
+colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and (os_name == "nt" or platform_system == "Windows")
+commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
+cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
+idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
+importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
+jeepney==0.8.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+keyring==23.11.0 ; python_version >= "3.7" and python_version < "4.0"
+more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
+packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
+pep517==0.13.0 ; python_version >= "3.7" and python_version < "4.0"
+pkginfo==1.9.2 ; python_version >= "3.7" and python_version < "4.0"
+pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
+pywin32-ctypes==0.2.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
+readme-renderer==37.3 ; python_version >= "3.7" and python_version < "4.0"
+requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
+requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
+rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
+rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
+secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
+tomli==2.0.1 ; python_version >= "3.7" and python_version < "3.11"
+twine==4.0.2 ; python_version >= "3.7" and python_version < "4.0"
+typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "3.9"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
+webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
+zipp==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.7.0/LICENSE` & `FlexGet-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/PKG-INFO` & `FlexGet-3.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.7.0
+Version: 3.7.1
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
```

### Comparing `FlexGet-3.7.0/README.rst` & `FlexGet-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/dev-requirements-extras.txt` & `FlexGet-3.7.1/dev-requirements-extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 appdirs==1.4.4 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 bcrypt==4.0.1 ; python_version >= "3.7" and python_version < "4.0"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 boto3==1.26.27 ; python_version >= "3.7" and python_version < "4.0"
 botocore==1.29.27 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0"
 chardet==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
-charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
+charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
 cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.7" and python_version < "4.0"
 dogpile-cache==1.1.8 ; python_version >= "3.7" and python_version < "4.0"
 enzyme==0.4.1 ; python_version >= "3.7" and python_version < "4.0"
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
-idna==3.4 ; python_version >= "3.7" and python_version < "4"
+idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.8"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 jmespath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
 paramiko==2.12.0 ; python_version >= "3.7" and python_version < "4.0"
 pbr==5.11.0 ; python_version >= "3.7" and python_version < "4.0"
 plexapi==4.13.1 ; python_version >= "3.7" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0"
 pynacl==1.5.0 ; python_version >= "3.7" and python_version < "4.0"
 pysftp==0.2.9 ; python_version >= "3.7" and python_version < "4.0"
 pysrt==1.1.2 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 rarfile==4.0 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
+requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 s3transfer==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 stevedore==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
 subliminal==2.1.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "3.8"
 urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.7.0/dev-requirements.txt` & `FlexGet-3.7.1/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 alabaster==0.7.12 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
 babel==2.11.0 ; python_version >= "3.7" and python_version < "4.0"
 black==22.12.0 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4.0"
 cfgv==3.3.1 ; python_version >= "3.7" and python_version < "4.0"
-charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
+charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 codacy-coverage==1.3.11 ; python_version >= "3.7" and python_version < "4.0"
-colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32" or python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
+colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and (sys_platform == "win32" or platform_system == "Windows")
 coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
 exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
 execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
 filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
 gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
 gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
 identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
-idna==3.4 ; python_version >= "3.7" and python_version < "4"
+idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
 imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
 iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
@@ -36,15 +36,15 @@
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
-requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
+requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 ruff==0.0.261 ; python_version >= "3.7" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
 snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
@@ -54,13 +54,13 @@
 sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy-stubs==0.4 ; python_version >= "3.7" and python_version < "4.0"
 toml==0.10.2 ; python_version >= "3.7" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.7" and python_full_version < "3.11.0a7"
 typed-ast==1.5.4 ; python_version < "3.8" and python_version >= "3.7"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 vcrpy==4.2.1 ; python_version >= "3.7" and python_version < "4.0"
 virtualenv==20.17.1 ; python_version >= "3.7" and python_version < "4.0"
 wrapt==1.14.1 ; python_version >= "3.7" and python_version < "4.0"
 yarl==1.8.2 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
```

### Comparing `FlexGet-3.7.0/flexget/__init__.py` & `FlexGet-3.7.1/flexget/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/api/app.py` & `FlexGet-3.7.1/flexget/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
         return pagination
 
 
 api_app = Flask(__name__, template_folder=os.path.join(__path__[0], 'templates'))
 api_app.config['REMEMBER_COOKIE_NAME'] = 'flexget.token'
 api_app.config['DEBUG'] = True
-api_app.config['ERROR_404_HELP'] = False
+api_app.config['RESTX_ERROR_404_HELP'] = False
 api_app.url_map.strict_slashes = False
 
 CORS(api_app, expose_headers='Link, Total-Count, Count, ETag')
 Compress(api_app)
 
 api = API(
     api_app,
```

### Comparing `FlexGet-3.7.0/flexget/api/core/authentication.py` & `FlexGet-3.7.1/flexget/api/core/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 
 @auth_api.route('/login/')
 class LoginAPI(APIResource):
     @api.validate(login_api_schema, description='Username and Password')
     @api.response(Unauthorized)
     @api.response(200, 'Login successful', model=base_message_schema)
-    @api.doc(parser=login_parser)
+    @api.doc(expect=[login_parser])
     def post(self, session: Session = None) -> Response:
         """Login with username and password"""
         data = request.json
         user_name = data.get('username')
         password = data.get('password')
 
         if data:
```

### Comparing `FlexGet-3.7.0/flexget/api/core/cached.py` & `FlexGet-3.7.1/flexget/api/core/cached.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 @cached_api.route('/')
 @api.doc(description='Returns a cached copy of the requested resource, matching its mime type')
 class CachedResource(APIResource):
     @api.response(200, description='Cached resource')
     @api.response(BadRequest)
     @api.response(APIError)
-    @api.doc(parser=cached_parser)
+    @api.doc(expect=[cached_parser])
     def get(self, session: Session = None) -> Response:
         """Cache remote resources"""
         args = cached_parser.parse_args()
         url = args.get('url')
         force = args.get('force')
         try:
             file_path, mime_type = cached_resource(url, self.manager.config_base, force=force)
```

### Comparing `FlexGet-3.7.0/flexget/api/core/database.py` & `FlexGet-3.7.1/flexget/api/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from flask import Response, jsonify, request
+from sqlalchemy import text
 from sqlalchemy.orm import Session
 
 from flexget.api import APIResource, api
 from flexget.api.app import BadRequest, base_message_schema, success_response
 from flexget.db_schema import plugin_schemas, reset_schema
 
 db_api = api.namespace('database', description='Manage Flexget DB')
@@ -35,15 +36,15 @@
         msg = ''
         data = request.json
         operation = data['operation']
         if operation == 'cleanup':
             self.manager.db_cleanup(force=True)
             msg = 'DB Cleanup finished'
         elif operation == 'vacuum':
-            session.execute('VACUUM')
+            session.execute(text('VACUUM'))
             session.commit()
             msg = 'DB VACUUM finished'
         elif operation == 'plugin_reset':
             plugin_name = data.get('plugin_name')
             if not plugin_name:
                 raise BadRequest(
                     "'plugin_name' attribute must be used when trying to reset plugin"
```

### Comparing `FlexGet-3.7.0/flexget/api/core/format_checker.py` & `FlexGet-3.7.1/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/api/core/plugins.py` & `FlexGet-3.7.1/flexget/api/core/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 @plugins_api.route('/')
 class PluginsAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, model=plugin_list_reply_schema)
     @api.response(BadRequest)
     @api.response(NotFoundError)
-    @api.doc(parser=plugins_parser)
+    @api.doc(expect=[plugins_parser])
     def get(self, session: Session = None) -> Response:
         """Get list of registered plugins"""
         args = plugins_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
@@ -150,15 +150,15 @@
 
 
 @plugins_api.route('/<string:plugin_name>/')
 class PluginAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(BadRequest)
     @api.response(200, model=plugin_schema)
-    @api.doc(parser=plugin_parser, params={'plugin_name': 'Name of the plugin to return'})
+    @api.doc(expect=[plugin_parser], params={'plugin_name': 'Name of the plugin to return'})
     def get(self, plugin_name: str, session=None):
         """Return plugin data by name"""
         args = plugin_parser.parse_args()
         try:
             plugin = get_plugin_by_name(plugin_name, issued_by='plugins API')
         except DependencyError as e:
             raise BadRequest(e.message)
```

### Comparing `FlexGet-3.7.0/flexget/api/core/schema.py` & `FlexGet-3.7.1/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/api/core/server.py` & `FlexGet-3.7.1/flexget/api/core/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
     finally:
         if fd:
             os.close(fd)
 
 
 @server_api.route('/log/')
 class ServerLogAPI(APIResource):
-    @api.doc(parser=server_log_parser)
+    @api.doc(expect=[server_log_parser])
     @api.response(200, description='Streams as line delimited JSON')
     def get(self, session: Session = None) -> Response:
         """Stream Flexget log Streams as line delimited JSON"""
         args = server_log_parser.parse_args()
 
         def follow(lines, search):
             log_parser = LogParser(search)
```

### Comparing `FlexGet-3.7.0/flexget/api/core/tasks.py` & `FlexGet-3.7.1/flexget/api/core/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 
 @tasks_api.route('/')
 @api.doc(description=task_api_desc)
 class TasksAPI(APIResource):
     @etag
     @api.response(200, model=tasks_list_schema)
-    @api.doc(parser=tasks_parser)
+    @api.doc(expect=[tasks_parser])
     def get(self, session: Session = None) -> Response:
         """List all tasks"""
 
         active_tasks = {
             task: task_data
             for task, task_data in self.manager.user_config.get('tasks', {}).items()
             if not task.startswith('_')
```

### Comparing `FlexGet-3.7.0/flexget/api/core/user.py` & `FlexGet-3.7.1/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/api/templates/api_response.html` & `FlexGet-3.7.1/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/api/templates/swagger-ui.html` & `FlexGet-3.7.1/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archive/archive.py` & `FlexGet-3.7.1/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archive/cli.py` & `FlexGet-3.7.1/flexget/components/archive/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archive/db.py` & `FlexGet-3.7.1/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archives/archives.py` & `FlexGet-3.7.1/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archives/decompress.py` & `FlexGet-3.7.1/flexget/components/archives/decompress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/archives/utils.py` & `FlexGet-3.7.1/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/backlog/backlog.py` & `FlexGet-3.7.1/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/backlog/cli.py` & `FlexGet-3.7.1/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/backlog/db.py` & `FlexGet-3.7.1/flexget/components/backlog/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,29 +52,29 @@
         )
         ver = 1
     if ver == 1:
         table = table_schema('backlog', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('backlog', session)
-        for row in session.execute(select([table.c.id, table.c.entry])):
+        for row in session.execute(select(table.c.id, table.c.entry)):
             try:
                 p = pickle.loads(row['entry'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
             except KeyError as e:
                 logger.error('Unable error upgrading backlog pickle object due to {}', str(e))
 
         ver = 2
     if ver == 2:
         table = table_schema('backlog', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.7.1/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.7.1/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.7.1/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent_alive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent_match.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class TorrentMatchFile:
     def __init__(self, path, size):
         self.path = path
         self.size = size
 
     def __repr__(self):
-        return f"{self.__class__.__name__}(path={str(self.path)}, size={self.size})"
+        return f"{self.__class__.__name__}(path={self.path!s}, size={self.size})"
 
 
 class TorrentMatch:
     """Plugin that attempts to match .torrents to local files"""
 
     schema = {
         'type': 'object',
```

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/torrent_size.py` & `FlexGet-3.7.1/flexget/components/bittorrent/torrent_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/bittorrent/trackers.py` & `FlexGet-3.7.1/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/emby/api_emby.py` & `FlexGet-3.7.1/flexget/components/emby/api_emby.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     EMBY_VERSION = get_current_flexget_version()
 
     host = EMBY_DEF_HOST
     return_host = None
 
     _userid = ''
     _token = ''
+    _host_name = ''
     _connect_token = ''
     _connect_token_link = ''
     _connect_username = ''
     _serverid = ''
     _logged = False
     _username = None
     _password = None
@@ -238,15 +239,18 @@
                         )
 
                     for server in connect_servers:
                         if 'Name' not in server:
                             raise PluginError(
                                 f'Could not login to Emby Connect account `{self._connect_username}`, no server list'
                             )
-                        if server['Name'].lower() == self.host.lower():
+                        if (
+                            server['Name'].lower() == self.host.lower()
+                            or server['Name'].lower() == self.host_name.lower()
+                        ):
                             connect_server = server
                             break
                     else:
                         raise PluginError(
                             f'No server with name `{self.host}`` on `{self._connect_username}` account'
                         )
 
@@ -338,28 +342,33 @@
 
     def logout(self):
         """Logout user from API"""
         self._token = None
         self._logged = False
         self._connect_username = ''
 
+        if self.host_name:
+            self.host = self.host_name
+            self._host_name = ""
+
         if 'token_data' in persist:
             persist['token_data']['token'] = None
 
     def check_token_data(self, token_data, login_type):
         """Checks saved tokens"""
         if not token_data:
             return False
 
         if login_type == LOGIN_CONNECT:
+            self._host_name = self.host
             connect_username = self._connect_username if self._connect_username else self._username
             if (
                 'token' not in token_data
                 or 'userid' not in token_data
-                or token_data.get('connect_username') != connect_username
+                or token_data.get('connect_username').lower() != connect_username.lower()
                 or login_type != token_data.get('login_type')
             ):
                 self.logout()
                 return False
         else:
             if (
                 'token' not in token_data
@@ -369,20 +378,25 @@
                 or login_type != token_data.get('login_type')
             ):
                 self.logout()
                 return False
 
         self._userid = token_data.get('userid')
         self._token = token_data.get('token')
-        self._login_type = token_data.get('type')
+        self._login_type = token_data.get('login_type')
         self._connect_username = token_data.get('connect_username', '')
         self.host = token_data.get('host', '')
         self._logged = True
         endpoint = EMBY_ENDPOINT_USERINFO.format(userid=token_data['userid'])
-        response = EmbyApi.resquest_emby(endpoint, self, 'GET')
+
+        try:
+            response = EmbyApi.resquest_emby(endpoint, self, 'GET')
+        except PluginError:
+            response = None
+
         if not response:
             self.logout()
             return False
 
         if self._userid != response.get('Id'):
             self.logout()
             return False
@@ -419,14 +433,18 @@
         return self._userid
 
     @property
     def username(self) -> str:
         return self._username
 
     @property
+    def host_name(self) -> str:
+        return self._host_name
+
+    @property
     def logged(self) -> bool:
         return self._logged
 
     @property
     def can_download(self) -> bool:
         return self._can_download
 
@@ -2707,15 +2725,21 @@
             return EmbyApiSerie.TYPE
         elif EmbyApiMovie.is_type(**kwargs):
             return EmbyApiMovie.TYPE
 
         return EmbyApiMedia.TYPE
 
     @staticmethod
-    def resquest_emby(endpoint: str, auth: 'EmbyAuth', method: str, emby_connect=False, **kwargs):
+    def resquest_emby(
+        endpoint: str,
+        auth: 'EmbyAuth',
+        method: str,
+        emby_connect=False,
+        **kwargs,
+    ):
         verify_certificates = True if emby_connect else False
 
         if not auth:
             auth = EmbyApi.get_auth(**kwargs)
             return
 
         if not auth.host:
@@ -2763,14 +2787,15 @@
                 )
         except HTTPError as e:  # Autentication Problem
             if e.response.status_code == 401:
                 logger.error('Autentication Error: {}', str(e))
                 return False
             else:
                 raise PluginError('Could not connect to Emby Server: %s' % str(e)) from e
+
         except RequestException as e:
             raise PluginError('Could not connect to Emby Server: %s' % str(e)) from e
 
         if response.status_code == 200 or response.status_code == 204:
             try:
                 return response.json()
             except ValueError:
```

### Comparing `FlexGet-3.7.0/flexget/components/emby/emby_list.py` & `FlexGet-3.7.1/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/emby/emby_lookup.py` & `FlexGet-3.7.1/flexget/components/emby/emby_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/emby/emby_refresh.py` & `FlexGet-3.7.1/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/emby/emby_util.py` & `FlexGet-3.7.1/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/emby/from_emby.py` & `FlexGet-3.7.1/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.7.1/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.7.1/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/failed/api.py` & `FlexGet-3.7.1/flexget/components/failed/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 @retry_failed_api.route('/')
 class RetryFailed(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, model=retry_entries_list_schema)
-    @api.doc(parser=failed_parser)
+    @api.doc(expect=[failed_parser])
     def get(self, session=None):
         """List all failed entries"""
         args = failed_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
```

### Comparing `FlexGet-3.7.0/flexget/components/failed/cli.py` & `FlexGet-3.7.1/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/failed/db.py` & `FlexGet-3.7.1/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/failed/retry_failed.py` & `FlexGet-3.7.1/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/ftp/ftp_download.py` & `FlexGet-3.7.1/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/ftp/ftp_list.py` & `FlexGet-3.7.1/flexget/components/ftp/ftp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/ftp/sftp.py` & `FlexGet-3.7.1/flexget/components/ftp/sftp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/ftp/sftp_client.py` & `FlexGet-3.7.1/flexget/components/ftp/sftp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         if self.is_file(source):
             source_file: str = parsed_path.name
             source_dir: str = parsed_path.parent.as_posix()
             try:
                 self._sftp.cwd(source_dir)
                 self._download_file(to, delete_origin and not is_symlink, source_file)
             except Exception as e:
-                raise SftpError(f'Failed to download file {source} ({str(e)})')
+                raise SftpError(f'Failed to download file {source} ({e!s})')
 
             if delete_origin and is_symlink:
                 self.remove_file(source)
 
         elif self.is_dir(source):
             base_path: str = parsed_path.joinpath('..').as_posix()
             dir_name: str = parsed_path.name
@@ -198,15 +198,15 @@
                 self._download_file, to, delete_origin and not is_symlink
             )
 
             try:
                 self._sftp.cwd(base_path)
                 self._sftp.walktree(dir_name, handle_file, dir_handler, unknown_handler, recursive)
             except Exception as e:
-                raise SftpError(f'Failed to download directory {source} ({str(e)})')
+                raise SftpError(f'Failed to download directory {source} ({e!s})')
 
             if delete_origin:
                 if self.is_link(source):
                     self.remove_file(source)
                 else:
                     self.remove_dir(source)
         else:
@@ -287,15 +287,15 @@
         :param path: path to build
         """
 
         if not self.path_exists(path):
             try:
                 self._sftp.makedirs(path)
             except Exception as e:
-                raise SftpError(f'Failed to create remote directory {path} ({str(e)})')
+                raise SftpError(f'Failed to create remote directory {path} ({e!s})')
 
     def close(self) -> None:
         """
         Close the sftp connection
         """
         self._sftp.close()
 
@@ -363,26 +363,26 @@
         destination = self._get_upload_path(source, to)
         destination_url: str = urljoin(self.prefix, destination)
 
         if not self.path_exists(to):
             try:
                 self.make_dirs(to)
             except Exception as e:
-                raise SftpError(f'Failed to create remote directory {to} ({str(e)})')
+                raise SftpError(f'Failed to create remote directory {to} ({e!s})')
 
         if not self.is_dir(to):
             raise SftpError(f'Not a directory: {to}')
 
         try:
             self._put_file(source, destination)
             logger.verbose('Successfully uploaded {} to {}', source, destination_url)  # type: ignore
         except OSError:
             raise SftpError(f'Remote directory does not exist: {to}')
         except Exception as e:
-            raise SftpError(f'Failed to upload {source} ({str(e)})')
+            raise SftpError(f'Failed to upload {source} ({e!s})')
 
     def _download_file(self, destination: str, delete_origin: bool, source: str) -> None:
         destination_path: str = self._get_download_path(source, destination)
         destination_dir: str = Path(destination_path).parent.as_posix()
 
         if Path(destination_path).exists():
             logger.verbose(  # type: ignore
```

### Comparing `FlexGet-3.7.0/flexget/components/history/api.py` & `FlexGet-3.7.1/flexget/components/history/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # Create pagination parser
 history_parser = api.pagination_parser(sort_choices=sort_choices, default='time')
 history_parser.add_argument('task', help='Filter by task name')
 
 
 @history_api.route('/')
-@api.doc(parser=history_parser)
+@api.doc(expect=[history_parser])
 class HistoryAPI(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, model=history_list_schema)
     def get(self, session=None):
         """List of previously accepted entries"""
         args = history_parser.parse_args()
```

### Comparing `FlexGet-3.7.0/flexget/components/history/cli.py` & `FlexGet-3.7.1/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/history/db.py` & `FlexGet-3.7.1/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/history/history.py` & `FlexGet-3.7.1/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/api.py` & `FlexGet-3.7.1/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/db.py` & `FlexGet-3.7.1/flexget/components/imdb/db.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta
 
 from loguru import logger
 from sqlalchemy import Boolean, Column, DateTime, Float, Integer, String, Table, Unicode
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey, Index
 
 from flexget import db_schema
 from flexget.components.imdb.utils import extract_id
 from flexget.db_schema import UpgradeImpossible
 
 logger = logger.bind(name='imdb.db')
@@ -67,20 +67,20 @@
 
     id = Column(Integer, primary_key=True)
     title = Column(Unicode)
     original_title = Column(Unicode)
     url = Column(String, index=True)
 
     # many-to-many relations
-    genres = relation('Genre', secondary=genres_table, backref='movies')
-    actors = relation('Actor', secondary=actors_table, backref='movies')
-    directors = relation('Director', secondary=directors_table, backref='movies')
-    writers = relation('Writer', secondary=writers_table, backref='movies')
-    plot_keywords = relation('PlotKeyword', secondary=plot_keywords_table, backref='movies')
-    languages = relation('MovieLanguage', order_by='MovieLanguage.prominence')
+    genres = relationship('Genre', secondary=genres_table, backref='movies')
+    actors = relationship('Actor', secondary=actors_table, backref='movies')
+    directors = relationship('Director', secondary=directors_table, backref='movies')
+    writers = relationship('Writer', secondary=writers_table, backref='movies')
+    plot_keywords = relationship('PlotKeyword', secondary=plot_keywords_table, backref='movies')
+    languages = relationship('MovieLanguage', order_by='MovieLanguage.prominence')
 
     score = Column(Float)
     votes = Column(Integer)
     meta_score = Column(Integer)
     year = Column(Integer)
     plot_outline = Column(Unicode)
     mpaa_rating = Column(String, default='')
@@ -117,15 +117,15 @@
 class MovieLanguage(Base):
     __tablename__ = 'imdb_movie_languages'
 
     movie_id = Column(Integer, ForeignKey('imdb_movies.id'), primary_key=True)
     language_id = Column(Integer, ForeignKey('imdb_languages.id'), primary_key=True)
     prominence = Column(Integer)
 
-    language = relation('Language')
+    language = relationship('Language')
 
     def __init__(self, language, prominence=None):
         self.language = language
         self.prominence = prominence
 
 
 class Language(Base):
```

### Comparing `FlexGet-3.7.0/flexget/components/imdb/from_imdb.py` & `FlexGet-3.7.1/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/imdb.py` & `FlexGet-3.7.1/flexget/components/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.7.1/flexget/components/imdb/imdb_lookup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,15 @@
         movie.score = parser.score
         movie.votes = parser.votes
         movie.meta_score = parser.meta_score
         movie.year = parser.year
         movie.mpaa_rating = parser.mpaa_rating
         movie.plot_outline = parser.plot_outline
         movie.url = imdb_url
+        session.add(movie)
         for name in parser.genres:
             genre = session.query(db.Genre).filter(db.Genre.name == name).first()
             if not genre:
                 genre = db.Genre(name)
             movie.genres.append(genre)  # pylint:disable=E1101
         for index, name in enumerate(parser.languages):
             language = session.query(db.Language).filter(db.Language.name == name).first()
@@ -305,15 +306,14 @@
                 session.query(db.PlotKeyword).filter(db.PlotKeyword.name == name).first()
             )
             if not plot_keyword:
                 plot_keyword = db.PlotKeyword(name)
             movie.plot_keywords.append(plot_keyword)  # pylint:disable=E1101
         # so that we can track how long since we've updated the info later
         movie.updated = datetime.now()
-        session.add(movie)
         return movie
 
     @property
     def movie_identifier(self):
         """Returns the plugin main identifier type"""
         return 'imdb_id'
```

### Comparing `FlexGet-3.7.0/flexget/components/imdb/imdb_url.py` & `FlexGet-3.7.1/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.7.1/flexget/components/imdb/imdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/imdb/utils.py` & `FlexGet-3.7.1/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/irc/api.py` & `FlexGet-3.7.1/flexget/components/irc/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     return_response = {'type': 'array', 'items': connection}
 
 
 return_schema = api.schema_model('irc.connections', ObjectsContainer.return_response)
 
 
 @irc_api.route('/connections/')
-@api.doc(parser=irc_parser)
+@api.doc(expect=[irc_parser])
 class IRCStatus(APIResource):
     @api.response(200, model=return_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
     def get(self, session=None):
         """Returns status of IRC connections"""
         from .irc import irc_manager
@@ -72,15 +72,15 @@
             from irc_bot import simple_irc_bot
         except ImportError:
             raise BadRequest('irc_bot dep is not installed')
         return jsonify(simple_irc_bot.IRCChannelStatus().enum_dict)
 
 
 @irc_api.route('/restart/')
-@api.doc(parser=irc_parser)
+@api.doc(expect=[irc_parser])
 class IRCRestart(APIResource):
     @api.response(200, model=base_message_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
     def get(self, session=None):
         """Restarts IRC connections"""
         from .irc import irc_manager
@@ -100,15 +100,15 @@
 irc_stop_parser = irc_parser.copy()
 irc_stop_parser.add_argument(
     'wait', type=inputs.boolean, default=False, help='Wait for connection to exit gracefully'
 )
 
 
 @irc_api.route('/stop/')
-@api.doc(parser=irc_stop_parser)
+@api.doc(expect=[irc_stop_parser])
 class IRCStop(APIResource):
     @api.response(200, model=base_message_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
     def get(self, session=None):
         """Stops IRC connections"""
         from .irc import irc_manager
```

### Comparing `FlexGet-3.7.0/flexget/components/irc/cli.py` & `FlexGet-3.7.1/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/irc/irc.py` & `FlexGet-3.7.1/flexget/components/irc/irc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/list_add.py` & `FlexGet-3.7.1/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.7.1/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/list_match.py` & `FlexGet-3.7.1/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.7.1/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 entry_list_parser = api.parser()
 entry_list_parser.add_argument('name', help='Filter results by list name')
 
 
 @entry_list_api.route('/')
 class EntryListListsAPI(APIResource):
     @etag
-    @api.doc(parser=entry_list_parser)
+    @api.doc(expect=[entry_list_parser])
     @api.response(200, 'Successfully retrieved entry lists', entry_list_return_lists_schema)
     def get(self, session=None):
         """Get entry lists"""
         args = entry_list_parser.parse_args()
         name = args.get('name')
 
         entry_lists = [
@@ -160,15 +160,15 @@
 
 
 @entry_list_api.route('/<int:list_id>/entries/')
 @api.response(NotFoundError)
 class EntryListEntriesAPI(APIResource):
     @etag
     @api.response(200, model=entry_lists_entries_return_schema)
-    @api.doc(params={'list_id': 'ID of the list'}, parser=entries_parser)
+    @api.doc(params={'list_id': 'ID of the list'}, expect=[entries_parser])
     def get(self, list_id, session=None):
         """Get entries by list ID"""
         try:
             list = db.get_list_by_id(list_id=list_id, session=session)
         except NoResultFound:
             raise NotFoundError('list_id %d does not exist' % list_id)
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
     if None is ver:
         ver = 0
     if ver == 0:
         table = table_schema('entry_list_entries', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('entry_list_entries', session)
-        for row in session.execute(select([table.c.id, table.c.entry])):
+        for row in session.execute(select(table.c.id, table.c.entry)):
             try:
                 p = pickle.loads(row['entry'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
             except KeyError as e:
                 logger.error('Unable error upgrading entry_list pickle object due to {}', str(e))
 
         ver = 1
     if ver == 1:
         table = table_schema('entry_list_entries', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from json import loads as json_loads
 from pathlib import Path
 
 from loguru import logger
 from requests.exceptions import RequestException
 from requests.utils import cookiejar_from_dict
 from sqlalchemy import Column, String, Unicode
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema, plugin
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.plugin import PluginError
@@ -38,15 +38,15 @@
     __tablename__ = "imdb_list_user"
 
     user_id = Column(String, primary_key=True)
     user_name = Column(Unicode)
     _cookies = Column('cookies', Unicode)
     cookies = json_synonym('_cookies')
 
-    lists = relation('IMDBListList', backref='imdb_user', cascade='all, delete, delete-orphan')
+    lists = relationship('IMDBListList', backref='imdb_user', cascade='all, delete, delete-orphan')
 
     def __init__(self, user_name, user_id, cookies):
         self.user_name = user_name
         self.user_id = user_id
         self.cookies = cookies
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 movie_list_parser.add_argument('name', help='Filter results by list name')
 
 
 @movie_list_api.route('/')
 class MovieListAPI(APIResource):
     @etag
     @api.response(200, model=return_lists_schema)
-    @api.doc(parser=movie_list_parser)
+    @api.doc(expect=[movie_list_parser])
     def get(self, session=None):
         """Gets movies lists"""
         args = movie_list_parser.parse_args()
         name = args.get('name')
         movie_lists = [
             movie_list.to_dict() for movie_list in db.get_movie_lists(name=name, session=session)
         ]
@@ -192,15 +192,15 @@
 
 
 @movie_list_api.route('/<int:list_id>/movies/')
 class MovieListMoviesAPI(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, model=return_movies_schema)
-    @api.doc(params={'list_id': 'ID of the list'}, parser=movies_parser)
+    @api.doc(params={'list_id': 'ID of the list'}, expect=[movies_parser])
     def get(self, list_id, session=None):
         """Get movies by list ID"""
         args = movies_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 list_parser = api.parser()
 list_parser.add_argument('name', help='Filter results by list name')
 
 
 @pending_list_api.route('/')
 class PendingListListsAPI(APIResource):
     @etag
-    @api.doc(parser=list_parser)
+    @api.doc(expect=[list_parser])
     @api.response(200, 'Successfully retrieved pending lists', pending_list_return_lists_schema)
     def get(self, session=None):
         """Get pending lists"""
         args = list_parser.parse_args()
         name = args.get('name')
 
         pending_lists = [
@@ -194,15 +194,15 @@
 
 sort_choices = ('id', 'added', 'title', 'original_url', 'list_id', 'approved')
 entries_parser = api.pagination_parser(sort_choices=sort_choices, default='title')
 entries_parser.add_argument('filter', help='Filter by title name')
 
 
 @pending_list_api.route('/<int:list_id>/entries/')
-@api.doc(params={'list_id': 'ID of the list'}, parser=entries_parser)
+@api.doc(params={'list_id': 'ID of the list'}, expect=[entries_parser])
 @api.response(NotFoundError)
 class PendingListEntriesAPI(APIResource):
     @etag
     @api.response(200, model=pending_lists_entries_return_schema)
     def get(self, list_id, session=None):
         """Get entries by list ID"""
         try:
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 @db_schema.upgrade(plugin_name)
 def upgrade(ver, session):
     if ver is None:
         ver = 0
     if ver == 0:
         table = table_schema('wait_list_entries', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/plex_watchlist.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/plex_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from collections.abc import MutableSet
 from urllib.parse import quote, urlparse
 
 import requests
 from loguru import logger
 from requests import RequestException
 
@@ -71,15 +70,15 @@
     except RequestException as e:
         raise RadarrRequestError(f"Unable to connect to Radarr at {url}. Error: {e}")
 
 
 def request_post_json(url, headers, data):
     """Makes a POST request and returns the JSON response"""
     try:
-        response = requests.post(url, headers=headers, data=data, timeout=10)
+        response = requests.post(url, headers=headers, json=data, timeout=10)
         if response.status_code == 201:
             return response.json()
         else:
             error_message = None
             try:
                 json_response = response.json()
                 if len(json_response) > 0 and "errorMessage" in json_response[0]:
@@ -119,39 +118,39 @@
     def __init__(self, api_key, base_url, port=None):
         self.api_key = api_key
         parsed_base_url = urlparse(base_url)
 
         if parsed_base_url.port:
             port = int(parsed_base_url.port)
 
-        self.api_url = "{}://{}:{}{}/api/".format(
+        self.api_url = "{}://{}:{}{}/api/v3/".format(
             parsed_base_url.scheme,
             parsed_base_url.netloc,
             port,
             parsed_base_url.path,
         )
 
     def get_profiles(self):
         """Gets all profiles"""
-        request_url = self.api_url + "profile"
+        request_url = self.api_url + "qualityProfile"
         headers = self._default_headers()
         return request_get_json(request_url, headers)
 
     def get_tags(self):
         """Gets all tags"""
         request_url = self.api_url + "tag"
         headers = self._default_headers()
         return request_get_json(request_url, headers)
 
     def add_tag(self, label):
         """Adds a tag"""
         request_url = self.api_url + "tag"
         headers = self._default_headers()
         data = {"label": label}
-        return request_post_json(request_url, headers, json.dumps(data))
+        return request_post_json(request_url, headers, data)
 
     def get_movies(self):
         """Gets all movies"""
         request_url = self.api_url + "movie"
         headers = self._default_headers()
         return request_get_json(request_url, headers)
 
@@ -216,15 +215,15 @@
             "tags": tags,
         }
 
         if add_options:
             data["addOptions"] = add_options
 
         try:
-            json_response = request_post_json(request_url, headers, json.dumps(data))
+            json_response = request_post_json(request_url, headers, data)
         except RadarrRequestError as ex:
             spec_ex = spec_exception_from_response_ex(ex)
             if spec_ex:
                 raise spec_ex
             else:
                 raise
 
@@ -524,15 +523,15 @@
             if self.config.get("only_monitored") and not movie["monitored"]:
                 continue
 
             quality_requirements = []
 
             # Check if we should add quality requirement
             if self.config.get("include_data"):
-                movie_profile_id = movie["profileId"]
+                movie_profile_id = movie["qualityProfileId"]
                 for profile in profiles:
                     profile_id = profile["id"]
                     if profile_id == movie_profile_id:
                         if profile_id not in profile_to_requirement_cache:
                             profile_to_requirement_cache[profile_id] = get_flexget_qualities(
                                 profile, self.config["only_use_cutoff_quality"]
                             )
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from flexget.event import event
 from flexget.utils import requests
 
 logger = logger.bind(name='sonarr_list')
 
 SERIES_ENDPOINT = 'series'
 LOOKUP_ENDPOINT = 'series/lookup'
-PROFILE_ENDPOINT = 'profile'
+PROFILE_ENDPOINT = 'qualityProfile'
 ROOTFOLDER_ENDPOINT = 'Rootfolder'
 DELETE_ENDPOINT = 'series/{}'
 
 # Sonarr qualities that do no exist in Flexget
 QUALITY_MAP = {'Raw-HD': 'remux', 'DVD': 'dvdrip'}
 
 
@@ -32,14 +32,15 @@
             'include_ended': {'type': 'boolean', 'default': True},
             'only_monitored': {'type': 'boolean', 'default': True},
             'include_data': {'type': 'boolean', 'default': False},
             'search_missing_episodes': {'type': 'boolean', 'default': True},
             'ignore_episodes_without_files': {'type': 'boolean', 'default': False},
             'ignore_episodes_with_files': {'type': 'boolean', 'default': False},
             'profile_id': {'type': 'integer', 'default': 1},
+            'language_id': {'type': 'integer', 'default': 1},
             'season_folder': {'type': 'boolean', 'default': False},
             'monitored': {'type': 'boolean', 'default': True},
             'root_folder_path': {'type': 'string'},
             'series_type': {
                 'type': 'string',
                 'enum': ['standard', 'daily', 'anime'],
                 'default': 'standard',
@@ -57,15 +58,15 @@
         # cache tags
         self._tags = None
 
     def _sonarr_request(self, endpoint, term=None, method='get', data=None):
         base_url = self.config['base_url']
         port = self.config['port']
         base_path = self.config['base_path']
-        url = f'{base_url}:{port}{base_path}/api/{endpoint}'
+        url = f'{base_url}:{port}{base_path}/api/v3/{endpoint}'
         headers = {'X-Api-Key': self.config['api_key']}
         if term:
             url += f'?term={term}'
         try:
             rsp = requests.request(method, url, headers=headers, json=data)
             data = rsp.json()
             logger.trace('sonarr response: {}', data)
@@ -143,15 +144,15 @@
             if filters:
                 # Checks if to retrieve just monitored shows
                 if not show['monitored'] and self.config.get('only_monitored'):
                     continue
                 # Checks if to retrieve ended shows
                 if show['status'] == 'ended' and not self.config.get('include_ended'):
                     continue
-            profile = profiles_dict.get(show['profileId'])
+            profile = profiles_dict.get(show['qualityProfileId'])
             if profile:
                 fg_qualities, fg_cutoff = self.quality_requirement_builder(profile)
 
             entry = Entry(
                 title=show['title'],
                 url='',
                 series_name=show['title'],
@@ -203,14 +204,15 @@
         else:
             root_folder = self._sonarr_request(ROOTFOLDER_ENDPOINT)
             root_path = root_folder[0]['path']
 
         # Setting defaults for Sonarr
         show['profileId'] = self.config.get('profile_id')
         show['qualityProfileId'] = self.config.get('profile_id')
+        show['languageProfileId'] = self.config.get('language_id')
         show['seasonFolder'] = self.config.get('season_folder')
         show['monitored'] = self.config.get('monitored')
         show['seriesType'] = self.config.get('series_type')
         show['tags'] = self.get_tag_ids(entry)
         show['rootFolderPath'] = root_path
         show['addOptions'] = {
             "ignoreEpisodesWithFiles": self.config.get('ignore_episodes_with_files'),
```

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.7.1/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notification_framework.py` & `FlexGet-3.7.1/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/email.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/gotify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/join.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/matrix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/mqtt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/ntfysh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/pushsafer.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/pushsafer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/toast.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.7.1/flexget/components/notify/notifiers/xmpp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/notify/notify.py` & `FlexGet-3.7.1/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.7.1/flexget/components/parsing/parsers/parser_common.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.7.1/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.7.1/flexget/components/parsing/parsers/parser_internal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.7.1/flexget/components/parsing/plugin_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         if config:
             selected_parsers.append(config)
         else:
             selected_parsers.append({})
 
     def on_task_exit(self, task, config):
         # Restore default parsers for next task run
-        selected_parsers.pop()
+        if selected_parsers:
+            selected_parsers.pop()
 
     on_task_abort = on_task_exit
 
     @property
     def selected(self) -> dict:
         if selected_parsers:
             return selected_parsers[-1]
```

### Comparing `FlexGet-3.7.0/flexget/components/pending_approval/api.py` & `FlexGet-3.7.1/flexget/components/pending_approval/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 @pending_api.route('/')
 class PendingEntriesAPI(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, model=pending_entry_list_schema)
-    @api.doc(parser=pending_parser)
+    @api.doc(expect=[pending_parser])
     def get(self, session=None):
         """List all pending entries"""
         args = pending_parser.parse_args()
 
         # Filter params
         task_name = args.get('task_name')
         approved = args.get('approved')
@@ -129,15 +129,15 @@
         rsp.headers.extend(pagination)
 
         return rsp
 
     @api.validate(operation_schema, description=description)
     @api.response(201, model=pending_entry_list_schema)
     @api.response(204, 'No entries modified')
-    @api.doc(parser=just_task_parser)
+    @api.doc(expect=[just_task_parser])
     def put(self, session=None):
         """Approve/Reject the status of pending entries"""
         args = filter_parser.parse_args()
 
         data = request.json
         approved = data['operation'] == 'approve'
         task_name = args.get('task_name')
@@ -149,15 +149,15 @@
                 pending_entries.append(entry.to_dict())
 
         rsp = jsonify(pending_entries)
         rsp.status_code = 201 if pending_entries else 204
         return rsp
 
     @api.response(200, model=base_message_schema)
-    @api.doc(parser=filter_parser)
+    @api.doc(expect=[filter_parser])
     def delete(self, session=None):
         """Delete pending entries"""
         args = filter_parser.parse_args()
 
         # Filter params
         task_name = args.get('task_name')
         approved = args.get('approved')
```

### Comparing `FlexGet-3.7.0/flexget/components/pending_approval/cli.py` & `FlexGet-3.7.1/flexget/components/pending_approval/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/pending_approval/db.py` & `FlexGet-3.7.1/flexget/components/pending_approval/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Base = db_schema.versioned_base('pending_approval', 1)
 
 
 @db_schema.upgrade('pending_approval')
 def upgrade(ver, session):
     if ver == 0:
         table = table_schema('pending_entries', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.7.1/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/rejected/api.py` & `FlexGet-3.7.1/flexget/components/rejected/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 @rejected_api.route('/')
 class Rejected(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, model=rejected_entries_list_schema)
-    @api.doc(parser=rejected_parser)
+    @api.doc(expect=[rejected_parser])
     def get(self, session=None):
         """List all rejected entries"""
         args = rejected_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
```

### Comparing `FlexGet-3.7.0/flexget/components/rejected/cli.py` & `FlexGet-3.7.1/flexget/components/rejected/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/rejected/db.py` & `FlexGet-3.7.1/flexget/components/rejected/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta
 
 from loguru import logger
 from sqlalchemy import Column, DateTime, ForeignKey, Index, Integer, String, Unicode
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 
 from flexget import db_schema
 from flexget.event import event
 from flexget.utils.sqlalchemy_utils import table_add_column, table_columns
 
 logger = logger.bind(name='remember_rej')
 Base = db_schema.versioned_base('remember_rejected', 3)
@@ -38,15 +38,15 @@
 
 class RememberTask(Base):
     __tablename__ = 'remember_rejected_feeds'
 
     id = Column(Integer, primary_key=True)
     name = Column(Unicode)
 
-    entries = relation('RememberEntry', backref='task', cascade='all, delete, delete-orphan')
+    entries = relationship('RememberEntry', backref='task', cascade='all, delete, delete-orphan')
 
 
 class RememberEntry(Base):
     __tablename__ = 'remember_rejected_entry'
 
     id = Column(Integer, primary_key=True)
     added = Column(DateTime, default=datetime.now)
```

### Comparing `FlexGet-3.7.0/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.7.1/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/scheduler/api.py` & `FlexGet-3.7.1/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/scheduler/scheduler.py` & `FlexGet-3.7.1/flexget/components/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/seen/api.py` & `FlexGet-3.7.1/flexget/components/seen/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 @seen_api.route('/')
 class SeenSearchAPI(APIResource):
     @etag
     @api.response(NotFoundError)
     @api.response(200, 'Successfully retrieved seen objects', seen_search_schema)
-    @api.doc(parser=seen_search_parser, description='Get seen entries')
+    @api.doc(expect=[seen_search_parser], description='Get seen entries')
     def get(self, session):
         """Search for seen entries"""
         args = seen_search_parser.parse_args()
 
         # Filter params
         value = args['value']
         local = args['local']
@@ -132,15 +132,15 @@
         rsp = jsonify(converted_seen_entry_list)
 
         # Add link header to response
         rsp.headers.extend(pagination)
         return rsp
 
     @api.response(200, 'Successfully delete all entries', model=base_message_schema)
-    @api.doc(parser=seen_base_parser, description='Delete seen entries')
+    @api.doc(expect=[seen_base_parser], description='Delete seen entries')
     def delete(self, session):
         """Delete seen entries"""
         args = seen_base_parser.parse_args()
         value = args['value']
         local = args['local']
 
         if value:
```

### Comparing `FlexGet-3.7.0/flexget/components/seen/cli.py` & `FlexGet-3.7.1/flexget/components/seen/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/seen/db.py` & `FlexGet-3.7.1/flexget/components/seen/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Index,
     Integer,
     Unicode,
     or_,
     select,
     update,
 )
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 
 from flexget import db_schema, plugin
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.database import with_session
 from flexget.utils.sqlalchemy_utils import table_add_column, table_schema
 
@@ -79,15 +79,15 @@
     id = Column(Integer, primary_key=True)
     title = Column(Unicode)
     reason = Column(Unicode)
     task = Column('feed', Unicode)
     added = Column(DateTime)
     local = Column(Boolean)
 
-    fields = relation('SeenField', backref='seen_entry', cascade='all, delete, delete-orphan')
+    fields = relationship('SeenField', backref='seen_entry', cascade='all, delete, delete-orphan')
 
     def __init__(self, title, task, reason=None, local=None):
         if local is None:
             local = False
         self.title = title
         self.reason = reason
         self.task = task
@@ -289,15 +289,15 @@
         query = query.filter(SeenEntry.task.in_(tasks))
     if count:
         return query.group_by(SeenEntry).count()
     if descending:
         query = query.order_by(getattr(SeenEntry, order_by).desc())
     else:
         query = query.order_by(getattr(SeenEntry, order_by))
-    return query.group_by(SeenEntry).slice(start, stop).from_self()
+    return query.group_by(SeenEntry).slice(start, stop)
 
 
 @with_session
 def get_entry_by_id(entry_id, session=None):
     return session.query(SeenEntry).filter(SeenEntry.id == entry_id).one()
```

### Comparing `FlexGet-3.7.0/flexget/components/seen/seen.py` & `FlexGet-3.7.1/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.7.1/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/seen/seen_movies.py` & `FlexGet-3.7.1/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/all_series.py` & `FlexGet-3.7.1/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/api.py` & `FlexGet-3.7.1/flexget/components/series/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 
 @series_api.route('/')
 class SeriesAPI(APIResource):
     @etag
     @api.response(200, 'Series list retrieved successfully', series_list_schema)
     @api.response(NotFoundError)
-    @api.doc(parser=series_list_parser, description="Get a  list of Flexget's shows in DB")
+    @api.doc(expect=[series_list_parser], description="Get a  list of Flexget's shows in DB")
     def get(self, session=None):
         """List existing shows"""
         args = series_list_parser.parse_args()
 
         # Filter params
         configured = args['in_config']
         premieres = args['premieres']
@@ -341,15 +341,15 @@
 @series_api.route('/search/<string:name>/')
 @api.doc(
     description='Searches for a show in the DB via its name. Returns a list of matching shows.'
 )
 class SeriesGetShowsAPI(APIResource):
     @etag
     @api.response(200, 'Show list retrieved successfully', series_list_schema)
-    @api.doc(params={'name': 'Name of the show(s) to search'}, parser=base_series_parser)
+    @api.doc(params={'name': 'Name of the show(s) to search'}, expect=[base_series_parser])
     def get(self, name, session):
         """List of shows matching lookup name"""
         name = normalize_series_name(name)
         matches = db.shows_by_name(name, session=session)
 
         args = series_list_parser.parse_args()
         begin = args.get('begin')
@@ -374,30 +374,30 @@
 
 @series_api.route('/<int:show_id>/')
 @api.doc(params={'show_id': 'ID of the show'})
 @api.response(NotFoundError)
 class SeriesShowAPI(APIResource):
     @etag
     @api.response(200, 'Show information retrieved successfully', show_details_schema)
-    @api.doc(description='Get a specific show using its ID', parser=base_series_parser)
+    @api.doc(description='Get a specific show using its ID', expect=[base_series_parser])
     def get(self, show_id, session):
         """Get show details by ID"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('Show with ID %s not found' % show_id)
 
         args = series_list_parser.parse_args()
         begin = args.get('begin')
         latest = args.get('latest')
 
         return jsonify(series_details(show, begin, latest))
 
     @api.response(200, 'Removed series from DB', model=base_message_schema)
-    @api.doc(description='Delete a specific show using its ID', parser=delete_parser)
+    @api.doc(description='Delete a specific show using its ID', expect=[delete_parser])
     def delete(self, show_id, session):
         """Remove series from DB"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('Show with ID %s not found' % show_id)
 
@@ -444,15 +444,15 @@
 @api.doc(
     params={'show_id': 'ID of the show'},
     description='The \'Series-ID\' header will be appended to the result headers',
 )
 class SeriesSeasonsAPI(APIResource):
     @etag
     @api.response(200, 'Seasons retrieved successfully for show', season_list_schema)
-    @api.doc(description='Get all show seasons via its ID', parser=entity_parser)
+    @api.doc(description='Get all show seasons via its ID', expect=[entity_parser])
     def get(self, show_id, session):
         """Get seasons by show ID"""
         args = entity_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
@@ -501,15 +501,15 @@
         # Add series ID header
         rsp.headers.extend({'Series-ID': show_id})
         return rsp
 
     @api.response(200, 'Successfully forgotten all seasons from show', model=base_message_schema)
     @api.doc(
         description='Delete all show seasons via its ID. Deleting a season will mark it as wanted again',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, session):
         """Deletes all seasons of a show"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -547,15 +547,15 @@
         rsp.headers.extend({'Series-ID': show_id})
         return rsp
 
     @api.response(200, 'Season successfully forgotten for show', model=base_message_schema)
     @api.doc(
         description='Delete a specific season via its ID and show ID. Deleting a season will mark it as '
         'wanted again',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, season_id, session):
         """Forgets season by show ID and season ID"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -577,15 +577,15 @@
 @api.doc(
     params={'show_id': 'ID of the show'},
     description='The \'Series-ID\' header will be appended to the result headers',
 )
 class SeriesEpisodesAPI(APIResource):
     @etag
     @api.response(200, 'Episodes retrieved successfully for show', episode_list_schema)
-    @api.doc(description='Get all show episodes via its ID', parser=entity_parser)
+    @api.doc(description='Get all show episodes via its ID', expect=[entity_parser])
     def get(self, show_id, session):
         """Get episodes by show ID"""
         args = entity_parser.parse_args()
 
         # Pagination and sorting params
         page = args['page']
         per_page = args['per_page']
@@ -634,15 +634,15 @@
         # Add series ID header
         rsp.headers.extend({'Series-ID': show_id})
         return rsp
 
     @api.response(200, 'Successfully forgotten all episodes from show', model=base_message_schema)
     @api.doc(
         description='Delete all show episodes via its ID. Deleting an episode will mark it as wanted again',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, session):
         """Deletes all episodes of a show"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -680,15 +680,15 @@
         rsp.headers.extend({'Series-ID': show_id})
         return rsp
 
     @api.response(200, 'Episode successfully forgotten for show', model=base_message_schema)
     @api.doc(
         description='Delete a specific episode via its ID and show ID. Deleting an episode will mark it as '
         'wanted again',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, ep_id, session):
         """Forgets episode by show ID and episode ID"""
         try:
             show = db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -733,15 +733,15 @@
     'The \'Season-ID\' header will be appended to the result headers.',
 )
 class SeriesSeasonsReleasesAPI(APIResource):
     @etag
     @api.response(200, 'Releases retrieved successfully for season', season_release_list_schema)
     @api.doc(
         description='Get all matching releases for a specific season of a specific show.',
-        parser=release_list_parser,
+        expect=[release_list_parser],
     )
     def get(self, show_id, season_id, session):
         """Get all season releases by show ID and season ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -809,15 +809,15 @@
         rsp.headers.extend({'Series-ID': show_id, 'Season-ID': season_id})
 
         return rsp
 
     @api.response(200, 'Successfully deleted all releases for season', model=base_message_schema)
     @api.doc(
         description='Delete all releases for a specific season of a specific show.',
-        parser=release_delete_parser,
+        expect=[release_delete_parser],
     )
     def delete(self, show_id, season_id, session):
         """Deletes all season releases by show ID and season ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -917,15 +917,15 @@
         rsp = jsonify(release.to_dict())
         rsp.headers.extend({'Series-ID': show_id, 'Season-ID': season_id})
         return rsp
 
     @api.response(200, 'Release successfully deleted', model=base_message_schema)
     @api.doc(
         description='Delete a specific releases for a specific season of a specific show.',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, season_id, rel_id, session):
         """Delete episode release by show ID, season ID and release ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -992,15 +992,15 @@
     'The \'Episode-ID\' header will be appended to the result headers.',
 )
 class SeriesEpisodeReleasesAPI(APIResource):
     @etag
     @api.response(200, 'Releases retrieved successfully for episode', episode_release_list_schema)
     @api.doc(
         description='Get all matching releases for a specific episode of a specific show.',
-        parser=release_list_parser,
+        expect=[release_list_parser],
     )
     def get(self, show_id, ep_id, session):
         """Get all episodes releases by show ID and episode ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -1068,15 +1068,15 @@
         rsp.headers.extend({'Series-ID': show_id, 'Episode-ID': ep_id})
 
         return rsp
 
     @api.response(200, 'Successfully deleted all releases for episode', model=base_message_schema)
     @api.doc(
         description='Delete all releases for a specific episode of a specific show.',
-        parser=release_delete_parser,
+        expect=[release_delete_parser],
     )
     def delete(self, show_id, ep_id, session):
         """Deletes all episodes releases by show ID and episode ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
@@ -1174,15 +1174,15 @@
         rsp = jsonify(release.to_dict())
         rsp.headers.extend({'Series-ID': show_id, 'Episode-ID': ep_id})
         return rsp
 
     @api.response(200, 'Release successfully deleted', model=base_message_schema)
     @api.doc(
         description='Delete a specific releases for a specific episode of a specific show.',
-        parser=delete_parser,
+        expect=[delete_parser],
     )
     def delete(self, show_id, ep_id, rel_id, session):
         """Delete episode release by show ID, episode ID and release ID"""
         try:
             db.show_by_id(show_id, session=session)
         except NoResultFound:
             raise NotFoundError('show with ID %s not found' % show_id)
```

### Comparing `FlexGet-3.7.0/flexget/components/series/cli.py` & `FlexGet-3.7.1/flexget/components/series/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/configure_series.py` & `FlexGet-3.7.1/flexget/components/series/configure_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/db.py` & `FlexGet-3.7.1/flexget/components/series/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
     String,
     Unicode,
     and_,
     delete,
     desc,
     func,
     select,
+    text,
     update,
 )
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.ext.hybrid import Comparator, hybrid_property
-from sqlalchemy.orm import backref, relation
+from sqlalchemy.orm import backref, relationship
 
 from flexget import db_schema, plugin
 from flexget.components.series.utils import normalize_series_name
 from flexget.event import event, fire_event
 from flexget.manager import Session
 from flexget.utils.database import quality_property, with_session
 from flexget.utils.sqlalchemy_utils import (
@@ -67,38 +68,38 @@
     id = Column(Integer, primary_key=True)
     _name = Column('name', Unicode)
     _name_normalized = Column('name_lower', Unicode, index=True, unique=True)
     identified_by = Column(String)
     begin_episode_id = Column(
         Integer, ForeignKey('series_episodes.id', name='begin_episode_id', use_alter=True)
     )
-    begin = relation(
+    begin = relationship(
         'Episode',
         uselist=False,
         primaryjoin="Series.begin_episode_id == Episode.id",
         foreign_keys=[begin_episode_id],
         post_update=True,
         backref='begins_series',
     )
-    episodes = relation(
+    episodes = relationship(
         'Episode',
         backref='series',
         cascade='all, delete, delete-orphan',
         primaryjoin='Series.id == Episode.series_id',
     )
-    in_tasks = relation(
+    in_tasks = relationship(
         'SeriesTask',
         backref=backref('series', uselist=False),
         cascade='all, delete, delete-orphan',
     )
-    alternate_names = relation(
+    alternate_names = relationship(
         'AlternateNames', backref='series', cascade='all, delete, delete-orphan'
     )
 
-    seasons = relation('Season', backref='series', cascade='all, delete, delete-orphan')
+    seasons = relationship('Season', backref='series', cascade='all, delete, delete-orphan')
 
     # Make a special property that does indexed case insensitive lookups on name, but stores/returns specified case
     @hybrid_property
     def name(self):
         return self._name
 
     @name.setter
@@ -140,15 +141,17 @@
     id = Column(Integer, primary_key=True)
     identifier = Column(String)
 
     identified_by = Column(String)
     season = Column(Integer)
     series_id = Column(Integer, ForeignKey('series.id'), nullable=False)
 
-    releases = relation('SeasonRelease', backref='season', cascade='all, delete, delete-orphan')
+    releases = relationship(
+        'SeasonRelease', backref='season', cascade='all, delete, delete-orphan'
+    )
 
     is_season = True
 
     @property
     def completed(self):
         """
         Return True if the season has any released marked as downloaded
@@ -166,15 +169,15 @@
         if not self.releases:
             return None
         return min(release.first_seen for release in self.releases)
 
     @first_seen.expression
     def first_seen(cls):
         return (
-            select([func.min(SeasonRelease.first_seen)])
+            select(func.min(SeasonRelease.first_seen))
             .where(SeasonRelease.season_id == cls.id)
             .correlate(Season.__table__)
             .label('first_seen')
         )
 
     @property
     def age(self):
@@ -265,28 +268,30 @@
     identifier = Column(String)
 
     season = Column(Integer)
     number = Column(Integer)
 
     identified_by = Column(String)
     series_id = Column(Integer, ForeignKey('series.id'), nullable=False)
-    releases = relation('EpisodeRelease', backref='episode', cascade='all, delete, delete-orphan')
+    releases = relationship(
+        'EpisodeRelease', backref='episode', cascade='all, delete, delete-orphan'
+    )
 
     is_season = False
 
     @hybrid_property
     def first_seen(self):
         if not self.releases:
             return None
         return min(release.first_seen for release in self.releases)
 
     @first_seen.expression
     def first_seen(cls):
         return (
-            select([func.min(EpisodeRelease.first_seen)])
+            select(func.min(EpisodeRelease.first_seen))
             .where(EpisodeRelease.episode_id == cls.id)
             .correlate(Episode.__table__)
             .label('first_seen')
         )
 
     @property
     def age(self):
@@ -581,15 +586,15 @@
             Base.metadata.create_all(bind=session.bind)
         # Upgrade episode_releases table to have a proper count and seed it with appropriate numbers
         columns = table_columns('episode_releases', session)
         if 'proper_count' not in columns:
             logger.info('Upgrading episode_releases table to have proper_count column')
             table_add_column('episode_releases', 'proper_count', Integer, session)
             release_table = table_schema('episode_releases', session)
-            for row in session.execute(select([release_table.c.id, release_table.c.title])):
+            for row in session.execute(select(release_table.c.id, release_table.c.title)):
                 # Recalculate the proper_count from title for old episodes
                 proper_count = (
                     plugin.get('parsing', 'series.db').parse_series(row['title']).proper_count
                 )
                 session.execute(
                     update(
                         release_table,
@@ -601,15 +606,15 @@
     if ver == 0:
         logger.info('Migrating first_seen column from series_episodes to episode_releases table.')
         # Create the column in episode_releases
         table_add_column('episode_releases', 'first_seen', DateTime, session)
         # Seed the first_seen value for all the past releases with the first_seen of their episode.
         episode_table = table_schema('series_episodes', session)
         release_table = table_schema('episode_releases', session)
-        for row in session.execute(select([episode_table.c.id, episode_table.c.first_seen])):
+        for row in session.execute(select(episode_table.c.id, episode_table.c.first_seen)):
             session.execute(
                 update(
                     release_table,
                     release_table.c.episode_id == row['id'],
                     {'first_seen': row['first_seen']},
                 )
             )
@@ -621,76 +626,84 @@
     if ver == 2:
         logger.info('Creating index on episode_releases table.')
         create_index('episode_releases', session, 'episode_id')
         ver = 3
     if ver == 3:
         # Remove index on Series.name
         try:
-            session.execute("DROP INDEX ix_series_name")
+            session.execute(text("DROP INDEX ix_series_name"))
             # This way doesn't work on sqlalchemy 1.4 for some reason
             # Index('ix_series_name').drop(bind=session.bind)
         except OperationalError:
             logger.debug('There was no ix_series_name index to remove.')
         # Add Series.name_lower column
         logger.info('Adding `name_lower` column to series table.')
         table_add_column('series', 'name_lower', Unicode, session)
         series_table = table_schema('series', session)
         create_index('series', session, 'name_lower')
         # Fill in lower case name column
         session.execute(
-            update(series_table, values={'name_lower': func.lower(series_table.c.name)})
+            update(series_table).values(
+                {series_table.c.name_lower: func.lower(series_table.c.name)}
+            )
         )
         ver = 4
     if ver == 4:
         logger.info('Adding `identified_by` column to episodes table.')
         table_add_column('series_episodes', 'identified_by', String, session)
         series_table = table_schema('series', session)
         # Clear out identified_by id series so that they can be auto detected again
         session.execute(
-            update(series_table, series_table.c.identified_by != 'ep', {'identified_by': None})
+            update(series_table)
+            .where(series_table.c.identified_by != 'ep')
+            .values({series_table.c.identified_by: None})
         )
         # Warn users about a possible config change needed.
         logger.warning(
             'If you are using `identified_by: id` for the series plugin for a date-identified '
             'or abolute-numbered series, you will need to update your config. Two new identified_by modes have '
             'been added: `date` and `sequence`. In addition, if you are using `identified_by: auto`, it will'
             'be relearned based on upcoming episodes.'
         )
         ver = 5
     if ver == 5:
         # Episode advancement now relies on identified_by being filled for the episodes.
         # This action retroactively marks 'ep' mode for all episodes where the series is already in 'ep' mode.
         series_table = table_schema('series', session)
         ep_table = table_schema('series_episodes', session)
-        ep_mode_series = select([series_table.c.id], series_table.c.identified_by == 'ep')
+        ep_mode_series = select(series_table.c.id).where(series_table.c.identified_by == 'ep')
         where_clause = and_(
             ep_table.c.series_id.in_(ep_mode_series),
             ep_table.c.season != None,
             ep_table.c.number != None,
             ep_table.c.identified_by == None,
         )
-        session.execute(update(ep_table, where_clause, {'identified_by': 'ep'}))
+        session.execute(
+            update(ep_table).where(where_clause).values({ep_table.c.identified_by: 'ep'})
+        )
         ver = 6
     if ver == 6:
         # Translate old qualities into new quality requirements
         release_table = table_schema('episode_releases', session)
-        for row in session.execute(select([release_table.c.id, release_table.c.quality])):
+        for row in session.execute(select(release_table.c.id, release_table.c.quality)):
             # Webdl quality no longer has dash
             new_qual = row['quality'].replace('web-dl', 'webdl')
             if row['quality'] != new_qual:
                 session.execute(
-                    update(release_table, release_table.c.id == row['id'], {'quality': new_qual})
+                    update(release_table)
+                    .where(release_table.c.id == row['id'])
+                    .values({release_table.c.quality: new_qual})
                 )
         ver = 7
     # Normalization rules changed for 7 and 8, but only run this once
     if ver in [7, 8]:
         # Merge series that qualify as duplicates with new normalization scheme
         series_table = table_schema('series', session)
         ep_table = table_schema('series_episodes', session)
-        all_series = session.execute(select([series_table.c.name, series_table.c.id]))
+        all_series = session.execute(select(series_table.c.name, series_table.c.id))
         unique_series = {}
         for row in all_series:
             unique_series.setdefault(normalize_series_name(row['name']), []).append(row['id'])
         for series, ids in unique_series.items():
             session.execute(update(ep_table, ep_table.c.series_id.in_(ids), {'series_id': ids[0]}))
             if len(ids) > 1:
                 session.execute(delete(series_table, series_table.c.id.in_(ids[1:])))
@@ -703,28 +716,30 @@
         ver = 10
     if ver == 10:
         # Due to bad db cleanups there may be invalid entries in series_tasks table
         series_tasks = table_schema('series_tasks', session)
         series_table = table_schema('series', session)
         logger.verbose('Repairing series_tasks table data')
         session.execute(
-            delete(series_tasks, ~series_tasks.c.series_id.in_(select([series_table.c.id])))
+            delete(series_tasks).where(~series_tasks.c.series_id.in_(select(series_table.c.id)))
         )
         ver = 11
     if ver == 11:
         # SeriesTasks was cleared out due to a bug, make sure they get recalculated next run #2772
         from flexget.task import config_changed
 
         config_changed(session=session)
         ver = 12
     if ver == 12:
         # Force identified_by value None to 'auto'
         series_table = table_schema('series', session)
         session.execute(
-            update(series_table, series_table.c.identified_by == None, {'identified_by': 'auto'})
+            update(series_table)
+            .where(series_table.c.identified_by == None)
+            .values({series_table.c.identified_by: 'auto'})
         )
         ver = 13
     if ver == 13:
         # New season_releases table, added by "create_all"
         logger.info('Adding season_releases table')
         ver = 14
     return ver
@@ -799,15 +814,15 @@
     """Return all seasons of a given series"""
     seasons = session.query(Season).filter(Season.series_id == series.id)
     if count:
         return seasons.count()
     seasons = (
         seasons.order_by(Season.season.desc()) if descending else seasons.order_by(Season.season)
     )
-    return seasons.slice(start, stop).from_self().all()
+    return seasons.slice(start, stop).all()
 
 
 def get_all_entities(
     series: Series, session: Session, sort_by: str = 'age', reverse: bool = False
 ) -> List[Union[Episode, Season]]:
     episodes = show_episodes(series, session=session)
     seasons = show_seasons(series, session=session)
@@ -836,20 +851,20 @@
 ) -> List[EpisodeRelease]:
     """Return all releases for a given episode"""
     releases = session.query(EpisodeRelease).filter(EpisodeRelease.episode_id == episode.id)
     if downloaded is not None:
         releases = releases.filter(EpisodeRelease.downloaded == downloaded)
     if count:
         return releases.count()
-    releases = releases.slice(start, stop).from_self()
+    releases = releases
     if descending:
         releases = releases.order_by(getattr(EpisodeRelease, sort_by).desc())
     else:
         releases = releases.order_by(getattr(EpisodeRelease, sort_by))
-    return releases.all()
+    return releases.slice(start, stop).all()
 
 
 def get_season_releases(
     season: Season,
     downloaded: bool = None,
     start: int = None,
     stop: int = None,
@@ -860,20 +875,20 @@
 ) -> Union[int, List[SeasonRelease]]:
     """Return all releases for a given season"""
     releases = session.query(SeasonRelease).filter(SeasonRelease.season_id == season.id)
     if downloaded is not None:
         releases = releases.filter(SeasonRelease.downloaded == downloaded)
     if count:
         return releases.count()
-    releases = releases.slice(start, stop).from_self()
+    releases = releases
     if descending:
         releases = releases.order_by(getattr(SeasonRelease, sort_by).desc())
     else:
         releases = releases.order_by(getattr(SeasonRelease, sort_by))
-    return releases.all()
+    return releases.slice(start, stop).all()
 
 
 def episode_in_show(series_id: int, episode_id: int) -> bool:
     """Return True if `episode_id` is part of show with `series_id`, else return False"""
     with Session() as session:
         episode = session.query(Episode).filter(Episode.id == episode_id).one()
         return episode.series_id == series_id
@@ -978,15 +993,15 @@
         return query.group_by(Series).count()
     if sort_by == 'show_name':
         order_by = Series.name
     else:
         order_by = func.max(EpisodeRelease.first_seen)
     query = query.order_by(desc(order_by)) if descending else query.order_by(order_by)
 
-    return query.slice(start, stop).from_self()
+    return query.slice(start, stop)
 
 
 def auto_identified_by(series: Series) -> str:
     """
     Determine if series `name` should be considered identified by episode or id format
 
     Returns 'ep', 'sequence', 'date' or 'id' if enough history is present to identify the series' id type.
@@ -1041,15 +1056,18 @@
     :param Series series: Series object
     :param bool downloaded: Flag to return only downloaded season packs
     :param season: Filter by season number
     :return: Latest release of a season object
     """
     session = Session.object_session(series)
     releases = (
-        session.query(Season).join(Season.releases, Season.series).filter(Series.id == series.id)
+        session.query(Season)
+        .join(Season.releases)
+        .join(Season.series)
+        .filter(Series.id == series.id)
     )
 
     if downloaded:
         releases = releases.filter(SeasonRelease.downloaded == True)
 
     if season is not None:
         releases = releases.filter(Season.season == season)
@@ -1080,15 +1098,16 @@
     :param downloaded: find only downloaded releases
     :param season: season to find newest release for
     :return: Instance of Episode or None if not found.
     """
     session = Session.object_session(series)
     releases = (
         session.query(Episode)
-        .join(Episode.releases, Episode.series)
+        .join(Episode.releases)
+        .join(Episode.series)
         .filter(Series.id == series.id)
     )
 
     if downloaded:
         releases = releases.filter(EpisodeRelease.downloaded == True)
 
     if season is not None:
@@ -1417,15 +1436,15 @@
         )
     else:
         episodes = (
             episodes.order_by(Episode.identifier.desc())
             if descending
             else episodes.order_by(Episode.identifier)
         )
-    return episodes.slice(start, stop).from_self().all()
+    return episodes.slice(start, stop).all()
 
 
 def store_parser(
     session: Session, parser: 'SeriesParseResult', series: Series = None, quality: 'Quality' = None
 ) -> List[Union[SeasonRelease, EpisodeRelease]]:
     """
     Push series information into database. Returns added/existing release.
```

### Comparing `FlexGet-3.7.0/flexget/components/series/gen_series.py` & `FlexGet-3.7.1/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/internal_estimator.py` & `FlexGet-3.7.1/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/metainfo_series.py` & `FlexGet-3.7.1/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/next_series_episodes.py` & `FlexGet-3.7.1/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/next_series_seasons.py` & `FlexGet-3.7.1/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/series.py` & `FlexGet-3.7.1/flexget/components/series/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
         # Prefetch series
         with Session() as session:
             # str() added to make sure number shows (e.g. 24) are turned into strings
             series_names = [str(list(s.keys())[0]) for s in config]
             existing_series = (
                 session.query(db.Series)
                 .filter(db.Series.name.in_(series_names))
-                .options(joinedload('alternate_names'))
+                .options(joinedload(db.Series.alternate_names))
                 .all()
             )
             existing_series_map = {s.name_normalized: s for s in existing_series}
             # Expunge so we can work on de-attached while processing the series to minimize db locks
             session.expunge_all()
 
         start_time = preferred_clock()
@@ -1118,15 +1118,15 @@
             config = self.prepare_config(task.config['series'])
 
             # Prefetch series
             names = [str(list(series.keys())[0]) for series in config]
             existing_series = (
                 session.query(db.Series)
                 .filter(db.Series.name.in_(names))
-                .options(joinedload('alternate_names'))
+                .options(joinedload(db.Series.alternate_names))
                 .all()
             )
             existing_series_map = {s.name_normalized: s for s in existing_series}
 
             for series_item in config:
                 series_name, series_config = list(series_item.items())[0]
                 # Make sure number shows (e.g. 24) are turned into strings
```

### Comparing `FlexGet-3.7.0/flexget/components/series/series_begin.py` & `FlexGet-3.7.1/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/series_premiere.py` & `FlexGet-3.7.1/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/series/series_remove.py` & `FlexGet-3.7.1/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.7.1/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.7.1/flexget/components/sites/sites/alpharatio.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.7.1/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/anirena.py` & `FlexGet-3.7.1/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.7.1/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.7.1/flexget/components/sites/sites/argenteam.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.7.1/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.7.1/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/btn.py` & `FlexGet-3.7.1/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.7.1/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.7.1/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.7.1/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.7.1/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/ettv.py` & `FlexGet-3.7.1/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/eztv.py` & `FlexGet-3.7.1/flexget/components/sites/sites/eztv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/filelist.py` & `FlexGet-3.7.1/flexget/components/sites/sites/filelist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.7.1/flexget/components/sites/sites/filelist_api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.7.1/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.7.1/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.7.1/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/hebits.py` & `FlexGet-3.7.1/flexget/components/sites/sites/hebits.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/hliang.py` & `FlexGet-3.7.1/flexget/components/sites/sites/hliang.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @plugin.internet(logger)
     def parse_download_page(self, url, requests):
         txheaders = {'User-agent': 'Mozilla/4.0 (compatible; MSIE 5.5; Windows NT)'}
         try:
             page = requests.get(url, headers=txheaders)
         except requests.exceptions.RequestException as e:
-            msg = f'Cannot open "{url}" : {str(e)}'
+            msg = f'Cannot open "{url}" : {e!s}'
             logger.error(msg)
             raise UrlRewritingError(msg)
 
         try:
             soup = get_soup(page.text)
         except Exception as e:
             raise UrlRewritingError(str(e))
```

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.7.1/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.7.1/flexget/components/sites/sites/iptorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/koreus.py` & `FlexGet-3.7.1/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.7.1/flexget/components/sites/sites/limetorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.7.1/flexget/components/sites/sites/lostfilm.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
                     if group == 'settings':
                         continue
                     LostFilm._add_names_from_cfg_list(names_list, series_list)
             else:
                 logger.warning('Unsupported series configuration type')
                 return None
         except Exception as e:
-            logger.warning(f'Error parsing series config: {repr(e):s}')
+            logger.warning(f'Error parsing series config: {e!r:s}')
             names_list = None
 
         return names_list
 
     @staticmethod
     def _add_names_from_cfg_list(names_list: set, cfg_list: list) -> None:
         for s_item in cfg_list:
```

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.7.1/flexget/components/sites/sites/magnetdl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.7.1/flexget/components/sites/sites/morethantv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/ncore.py` & `FlexGet-3.7.1/flexget/components/sites/sites/ncore.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.7.1/flexget/components/sites/sites/newtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/newznab.py` & `FlexGet-3.7.1/flexget/components/sites/sites/newznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.7.1/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.7.1/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.7.1/flexget/components/sites/sites/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.7.1/flexget/components/sites/sites/piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/ptn.py` & `FlexGet-3.7.1/flexget/components/sites/sites/ptn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.7.1/flexget/components/sites/sites/rarbg.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/redirect.py` & `FlexGet-3.7.1/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.7.1/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/rmz.py` & `FlexGet-3.7.1/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/rss.py` & `FlexGet-3.7.1/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.7.1/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.7.1/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/shortened.py` & `FlexGet-3.7.1/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.7.1/flexget/components/sites/sites/site_1337x.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.7.1/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.7.1/flexget/components/sites/sites/solidtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.7.1/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.7.1/flexget/components/sites/sites/torrentday.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.7.1/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.7.1/flexget/components/sites/sites/torrentz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.7.1/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/sites/yts.py` & `FlexGet-3.7.1/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/urlrewrite.py` & `FlexGet-3.7.1/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.7.1/flexget/components/sites/urlrewrite_search.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/urlrewriting.py` & `FlexGet-3.7.1/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/sites/utils.py` & `FlexGet-3.7.1/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/status/api.py` & `FlexGet-3.7.1/flexget/components/status/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     default=True,
     help='Include the last execution of the task',
 )
 
 
 @tasks_api.route('/status/')
 @status_api.route('/')
-@api.doc(parser=tasks_parser)
+@api.doc(expect=[tasks_parser])
 class TasksStatusAPI(APIResource):
     @etag
     @api.response(200, model=task_status_list)
     def get(self, session=None):
         """Get status tasks"""
         args = tasks_parser.parse_args()
 
@@ -135,15 +135,15 @@
         # Add link header to response
         rsp.headers.extend(pagination)
         return rsp
 
 
 @tasks_api.route('/status/<int:task_id>/')
 @status_api.route('/<int:task_id>/')
-@api.doc(params={'task_id': 'ID of the status task'}, parser=tasks_parser)
+@api.doc(params={'task_id': 'ID of the status task'}, expect=[tasks_parser])
 class TaskStatusAPI(APIResource):
     @etag
     @api.response(200, model=task_status)
     @api.response(NotFoundError)
     def get(self, task_id, session=None):
         """Get status task by ID"""
         try:
@@ -197,15 +197,15 @@
     'abort_reason',
 )
 executions_parser = api.pagination_parser(executions_parser, sort_choices=sort_choices)
 
 
 @tasks_api.route('/status/<int:task_id>/executions/')
 @status_api.route('/<int:task_id>/executions/')
-@api.doc(parser=executions_parser, params={'task_id': 'ID of the status task'})
+@api.doc(expect=[executions_parser], params={'task_id': 'ID of the status task'})
 class TaskStatusExecutionsAPI(APIResource):
     @etag
     @api.response(200, model=task_executions)
     @api.response(NotFoundError)
     def get(self, task_id, session=None):
         """Get task executions by ID"""
         try:
```

### Comparing `FlexGet-3.7.0/flexget/components/status/cli.py` & `FlexGet-3.7.1/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/status/db.py` & `FlexGet-3.7.1/flexget/components/status/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 from datetime import timedelta
 
 from loguru import logger
 from sqlalchemy import Boolean, Column, DateTime, Index, Integer, String, func, select
 from sqlalchemy.ext.hybrid import hybrid_property
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema
 from flexget.event import event
 from flexget.utils.database import with_session
 from flexget.utils.sqlalchemy_utils import create_index
 
@@ -25,15 +25,15 @@
     return ver
 
 
 class StatusTask(Base):
     __tablename__ = 'status_task'
     id = Column(Integer, primary_key=True)
     name = Column('task', String)
-    executions = relation(
+    executions = relationship(
         'TaskExecution', backref='task', cascade='all, delete, delete-orphan', lazy='dynamic'
     )
 
     def __repr__(self):
         return f'<StatusTask(id={self.id},name={self.name})>'
 
     @hybrid_property
@@ -41,15 +41,15 @@
         if self.executions.count() == 0:
             return None
         return max(execution.start for execution in self.executions)
 
     @last_execution_time.expression
     def last_execution_time(cls):
         return (
-            select([func.max(TaskExecution.start)])
+            select(func.max(TaskExecution.start))
             .where(TaskExecution.task_id == cls.id)
             .correlate(StatusTask.__table__)
             .label('last_execution_time')
         )
 
     def to_dict(self):
         return {
```

### Comparing `FlexGet-3.7.0/flexget/components/status/status.py` & `FlexGet-3.7.1/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/thetvdb/api.py` & `FlexGet-3.7.1/flexget/components/thetvdb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 series_parser = base_parser.copy()
 series_parser.add_argument(
     'include_actors', type=inputs.boolean, help='Include actors in response'
 )
 
 
 @tvdb_api.route('/series/<string:title>/')
-@api.doc(params={'title': 'TV Show name or TVDB ID'}, parser=series_parser)
+@api.doc(params={'title': 'TV Show name or TVDB ID'}, expect=[series_parser])
 class TVDBSeriesLookupAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully found show', tvdb_series_schema)
     @api.response(NotFoundError)
     def get(self, title, session=None):
         """TheTVDB series lookup"""
         args = series_parser.parse_args()
@@ -178,15 +178,15 @@
 episode_parser.add_argument('absolute_number', type=int, help='Absolute episode number')
 episode_parser.add_argument(
     'air_date', type=inputs.date, help='Episode airdate in `YYYY-mm-dd` format'
 )
 
 
 @tvdb_api.route('/episode/<int:tvdb_id>/')
-@api.doc(params={'tvdb_id': 'TVDB ID of show'}, parser=episode_parser)
+@api.doc(params={'tvdb_id': 'TVDB ID of show'}, expect=[episode_parser])
 class TVDBEpisodeSearchAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully found episode', tvdb_episode_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
     def get(self, tvdb_id, session=None):
         """TheTVDB episode lookup"""
@@ -228,15 +228,15 @@
     'force_search',
     type=inputs.boolean,
     help='Force online lookup or allow for result to be retrieved from cache',
 )
 
 
 @tvdb_api.route('/search/')
-@api.doc(parser=search_parser)
+@api.doc(expect=[search_parser])
 class TVDBSeriesSearchAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully got results', search_results_schema)
     @api.response(BadRequest)
     @api.response(NotFoundError)
     def get(self, session=None):
         """TheTVDB series search"""
```

### Comparing `FlexGet-3.7.0/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.7.1/flexget/components/thetvdb/api_tvdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 
 from loguru import logger
 from sqlalchemy import Boolean, Column, DateTime, Float, Integer, Table, Text, Unicode
 from sqlalchemy.ext.associationproxy import association_proxy
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema
 from flexget.utils import requests
 from flexget.utils.database import Session, json_synonym, text_date_synonym, with_session
 from flexget.utils.simple_persistence import SimplePersistence
 from flexget.utils.tools import chunked, split_title_year
@@ -165,18 +165,18 @@
     _aliases = Column('aliases', Unicode)
     aliases = json_synonym('_aliases')
     _actors = Column('actors', Unicode)
     actors_list = json_synonym('_actors')
     _posters = Column('posters', Unicode)
     posters_list = json_synonym('_posters')
 
-    _genres = relation('TVDBGenre', secondary=genres_table)
+    _genres = relationship('TVDBGenre', secondary=genres_table)
     genres = association_proxy('_genres', 'name')
 
-    episodes = relation('TVDBEpisode', backref='series', cascade='all, delete, delete-orphan')
+    episodes = relationship('TVDBEpisode', backref='series', cascade='all, delete, delete-orphan')
 
     def __init__(self, tvdb_id, language):
         """
         Looks up movie on tvdb and creates a new database model for it.
         These instances should only be added to a session via `session.merge`.
         """
         self.id = tvdb_id
@@ -388,15 +388,15 @@
 
 class TVDBSearchResult(Base):
     __tablename__ = 'tvdb_search_results'
 
     id = Column(Integer, primary_key=True)
     search = Column(Unicode, nullable=False, unique=True)
     series_id = Column(Integer, ForeignKey('tvdb_series.id'), nullable=True)
-    series = relation(TVDBSeries, backref='search_strings')
+    series = relationship(TVDBSeries, backref='search_strings')
 
     def __init__(self, search, series_id=None, series=None):
         self.search = search.lower()
         if series_id:
             self.series_id = series_id
         if series:
             self.series = series
```

### Comparing `FlexGet-3.7.0/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.7.1/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         'tvdb_language': 'language',
         'tvdb_airs_day_of_week': 'airs_dayofweek',
         'imdb_url': lambda series: series.imdb_id
         and f'http://www.imdb.com/title/{series.imdb_id}',
         'imdb_id': 'imdb_id',
         'zap2it_id': 'zap2it_id',
         'tvdb_id': 'id',
-        'tvdb_url': lambda series: f'http://thetvdb.com/index.php?tab=series&id={str(series.id)}',
+        'tvdb_url': lambda series: f'http://thetvdb.com/index.php?tab=series&id={series.id!s}',
     }
 
     series_actor_map = {'tvdb_actors': 'actors'}
     series_poster_map = {'tvdb_posters': 'posters'}
 
     # Episode info
     episode_map = {
```

### Comparing `FlexGet-3.7.0/flexget/components/tmdb/api.py` & `FlexGet-3.7.1/flexget/components/tmdb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 @tmdb_api.route('/movies/')
 @api.doc(description=description)
 class TMDBMoviesAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, model=return_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
-    @api.doc(parser=tmdb_parser)
+    @api.doc(expect=[tmdb_parser])
     def get(self, session=None):
         """Get TMDB movie data"""
         args = tmdb_parser.parse_args()
         title = args.get('title')
         tmdb_id = args.get('tmdb_id')
         imdb_id = args.get('imdb_id')
```

### Comparing `FlexGet-3.7.0/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.7.1/flexget/components/tmdb/api_tmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     String,
     Table,
     Unicode,
     func,
     or_,
 )
 from sqlalchemy.ext.associationproxy import association_proxy
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema, plugin
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils import requests
 from flexget.utils.database import json_synonym, with_session, year_property
@@ -113,17 +113,19 @@
     votes = Column(Integer)
     popularity = Column(Float)
     adult = Column(Boolean)
     budget = Column(Integer)
     revenue = Column(Integer)
     homepage = Column(Unicode)
     lookup_language = Column(String)
-    _posters = relation('TMDBPoster', backref='movie', cascade='all, delete, delete-orphan')
-    _backdrops = relation('TMDBBackdrop', backref='movie', cascade='all, delete, delete-orphan')
-    _genres = relation('TMDBGenre', secondary=genres_table, backref='movies')
+    _posters = relationship('TMDBPoster', backref='movie', cascade='all, delete, delete-orphan')
+    _backdrops = relationship(
+        'TMDBBackdrop', backref='movie', cascade='all, delete, delete-orphan'
+    )
+    _genres = relationship('TMDBGenre', secondary=genres_table, backref='movies')
     genres = association_proxy('_genres', 'name')
     updated = Column(DateTime, default=datetime.now, nullable=False)
 
     def __init__(self, id, language):
         """
         Looks up movie on tmdb and creates a new database model for it.
         These instances should only be added to a session via `session.merge`.
@@ -260,15 +262,15 @@
 
 
 class TMDBSearchResult(Base):
     __tablename__ = 'tmdb_search_results'
 
     search = Column(Unicode, primary_key=True)
     movie_id = Column(Integer, ForeignKey('tmdb_movies.id'), nullable=True)
-    movie = relation(TMDBMovie)
+    movie = relationship(TMDBMovie)
 
     def __init__(self, search, movie_id=None, movie=None):
         self.search = search.lower()
         if movie_id:
             self.movie_id = movie_id
         if movie:
             self.movie = movie
```

### Comparing `FlexGet-3.7.0/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.7.1/flexget/components/tmdb/tmdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/trakt/api.py` & `FlexGet-3.7.1/flexget/components/trakt/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
 
 @trakt_api.route('/series/')
 class TraktSeriesSearchApi(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully found show', series_return_schema)
     @api.response(NotFoundError)
-    @api.doc(parser=lookup_parser)
+    @api.doc(expect=[lookup_parser])
     def get(self, session=None):
         """Trakt series lookup"""
         args = lookup_parser.parse_args()
         include_actors = args.pop('include_actors')
         include_translations = args.pop('include_translations')
         kwargs = args
         try:
@@ -183,28 +183,28 @@
             result['translations'] = db.get_translations_dict(series.translations, 'show')
         return jsonify(result)
 
 
 @trakt_api.route('/series/<string:title>')
 @api.doc(params={'title': 'Series name'})
 class TraktSeriesWithTitleSearchApi(APIResource):
-    @api.doc(parser=lookup_parser)
+    @api.doc(expect=[lookup_parser])
     @api.response(301)
     def get(self, title, session=None):
         kwargs = lookup_parser.parse_args()
         kwargs['title'] = title
         return redirect(api.url_for(TraktSeriesSearchApi, **kwargs), code=301)
 
 
 @trakt_api.route('/movies/')
 class TraktMovieSearchApi(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully found show', movie_return_schema)
     @api.response(NotFoundError)
-    @api.doc(parser=lookup_parser)
+    @api.doc(expect=[lookup_parser])
     def get(self, session=None):
         """Trakt movie lookup"""
         args = lookup_parser.parse_args()
         include_actors = args.pop('include_actors')
         include_translations = args.pop('include_translations')
         kwargs = args
         try:
@@ -218,13 +218,13 @@
             result['translations'] = db.get_translations_dict(movie.translations, 'movie')
         return jsonify(result)
 
 
 @trakt_api.route('/movies/<string:title>')
 @api.doc(params={'title': 'Movie name'})
 class TraktMovieWithTitleSearchApi(APIResource):
-    @api.doc(parser=lookup_parser)
+    @api.doc(expect=[lookup_parser])
     @api.response(301)
     def get(self, title, session=None):
         kwargs = lookup_parser.parse_args()
         kwargs['title'] = title
         return redirect(api.url_for(TraktMovieSearchApi, **kwargs), code=301)
```

### Comparing `FlexGet-3.7.0/flexget/components/trakt/api_trakt.py` & `FlexGet-3.7.1/flexget/components/trakt/api_trakt.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,17 @@
             elif series and title and not found:
                 if (
                     not session.query(db.TraktShowSearchResult)
                     .filter(db.TraktShowSearchResult.search == title.lower())
                     .first()
                 ):
                     logger.debug('Adding search result to db')
-                    session.merge(db.TraktShowSearchResult(search=title, series=series))
+                    result = session.merge(db.TraktShowSearchResult(search=title))
+                    result.series = series
+
             elif series and found:
                 logger.debug('Updating search result in db')
                 found.series = series
             return series
         finally:
             session.commit()
 
@@ -243,15 +245,16 @@
             if movie and title and not found:
                 if (
                     not session.query(db.TraktMovieSearchResult)
                     .filter(db.TraktMovieSearchResult.search == title.lower())
                     .first()
                 ):
                     logger.debug('Adding search result to db')
-                    session.merge(db.TraktMovieSearchResult(search=title, movie=movie))
+                    result = session.merge(db.TraktMovieSearchResult(search=title))
+                    result.movie = movie
             elif movie and found:
                 logger.debug('Updating search result in db')
                 found.movie = movie
             return movie
         finally:
             session.commit()
```

### Comparing `FlexGet-3.7.0/flexget/components/trakt/cli.py` & `FlexGet-3.7.1/flexget/components/trakt/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/trakt/db.py` & `FlexGet-3.7.1/flexget/components/trakt/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from datetime import datetime, timedelta
 from typing import List
 
 from dateutil.parser import parse as dateutil_parse
 from loguru import logger
 from sqlalchemy import Column, Date, DateTime, Integer, String, Table, Time, Unicode, and_, or_
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema, plugin
 from flexget.manager import Session
 from flexget.terminal import console
 from flexget.utils import requests
 from flexget.utils.database import json_synonym
@@ -567,25 +567,25 @@
     status = Column(String)
     rating = Column(Integer)
     votes = Column(Integer)
     language = Column(Unicode)
     homepage = Column(Unicode)
     trailer = Column(Unicode)
     aired_episodes = Column(Integer)
-    _translations = relation(TraktShowTranslation)
+    _translations = relationship(TraktShowTranslation)
     _translation_languages = Column('translation_languages', Unicode)
     translation_languages = json_synonym('_translation_languages')
-    episodes = relation(
+    episodes = relationship(
         TraktEpisode, backref='show', cascade='all, delete, delete-orphan', lazy='dynamic'
     )
-    seasons = relation(
+    seasons = relationship(
         TraktSeason, backref='show', cascade='all, delete, delete-orphan', lazy='dynamic'
     )
-    genres = relation(TraktGenre, secondary=show_genres_table)
-    _actors = relation(TraktActor, secondary=show_actors_table)
+    genres = relationship(TraktGenre, secondary=show_genres_table)
+    _actors = relationship(TraktActor, secondary=show_actors_table)
     updated_at = Column(DateTime)
     cached_at = Column(DateTime)
 
     def to_dict(self):
         return {
             "id": self.id,
             "title": self.title,
@@ -784,19 +784,19 @@
     rating = Column(Integer)
     votes = Column(Integer)
     trailer = Column(Unicode)
     homepage = Column(Unicode)
     language = Column(Unicode)
     updated_at = Column(DateTime)
     cached_at = Column(DateTime)
-    _translations = relation(TraktMovieTranslation, backref='movie')
+    _translations = relationship(TraktMovieTranslation, backref='movie')
     _translation_languages = Column('translation_languages', Unicode)
     translation_languages = json_synonym('_translation_languages')
-    genres = relation(TraktGenre, secondary=movie_genres_table)
-    _actors = relation(TraktActor, secondary=movie_actors_table)
+    genres = relationship(TraktGenre, secondary=movie_genres_table)
+    _actors = relationship(TraktActor, secondary=movie_actors_table)
 
     def __init__(self, trakt_movie, session):
         super().__init__()
         self.update(trakt_movie, session)
 
     def to_dict(self):
         return {
@@ -881,15 +881,15 @@
 
 class TraktShowSearchResult(Base):
     __tablename__ = 'trakt_show_search_results'
 
     id = Column(Integer, primary_key=True)
     search = Column(Unicode, unique=True, nullable=False)
     series_id = Column(Integer, ForeignKey('trakt_shows.id'), nullable=True)
-    series = relation(TraktShow, backref='search_strings')
+    series = relationship(TraktShow, backref='search_strings')
 
     def __init__(self, search, series_id=None, series=None):
         self.search = search.lower()
         if series_id:
             self.series_id = series_id
         if series:
             self.series = series
@@ -897,15 +897,15 @@
 
 class TraktMovieSearchResult(Base):
     __tablename__ = 'trakt_movie_search_results'
 
     id = Column(Integer, primary_key=True)
     search = Column(Unicode, unique=True, nullable=False)
     movie_id = Column(Integer, ForeignKey('trakt_movies.id'), nullable=True)
-    movie = relation(TraktMovie, backref='search_strings')
+    movie = relationship(TraktMovie, backref='search_strings')
 
     def __init__(self, search, movie_id=None, movie=None):
         self.search = search.lower()
         if movie_id:
             self.movie_id = movie_id
         if movie:
             self.movie = movie
```

### Comparing `FlexGet-3.7.0/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.7.1/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.7.1/flexget/components/trakt/trakt_calendar.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/trakt/trakt_list.py` & `FlexGet-3.7.1/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.7.1/flexget/components/trakt/trakt_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/tvmaze/api.py` & `FlexGet-3.7.1/flexget/components/tvmaze/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 episode_parser.add_argument(
     'air_date', type=inputs.date_from_iso8601, help="Air date in the format of '2012-01-01'"
 )
 
 
 @tvmaze_api.route('/episode/<int:tvmaze_id>/')
 @api.doc(params={'tvmaze_id': 'TVMaze ID of show'})
-@api.doc(parser=episode_parser)
+@api.doc(expect=[episode_parser])
 class TVDBEpisodeSearchAPI(APIResource):
     @etag(cache_age=3600)
     @api.response(200, 'Successfully found episode', tvmaze_episode_schema)
     @api.response(NotFoundError)
     @api.response(BadRequest)
     def get(self, tvmaze_id, session=None):
         """TVMaze episode lookup"""
```

### Comparing `FlexGet-3.7.0/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.7.1/flexget/components/tvmaze/api_tvmaze.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Integer,
     String,
     Table,
     Unicode,
     and_,
     or_,
 )
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import MultipleResultsFound
 
 from flexget import db_schema, plugin
 from flexget.event import event
 from flexget.utils import requests
 from flexget.utils.database import json_synonym, with_session
 from flexget.utils.tools import split_title_year
@@ -65,15 +65,15 @@
 
 class TVMazeLookup(Base):
     __tablename__ = 'tvmaze_lookup'
 
     id = Column(Integer, primary_key=True, autoincrement=True)
     search_name = Column(Unicode, index=True, unique=True)
     series_id = Column(Integer, ForeignKey('tvmaze_series.tvmaze_id'))
-    series = relation('TVMazeSeries', backref='search_strings')
+    series = relationship('TVMazeSeries', backref='search_strings')
 
     def __init__(self, search_name, series_id=None, series=None):
         self.search_name = search_name.lower()
         if series_id:
             self.series_id = series_id
         if series:
             self.series = series
@@ -86,15 +86,15 @@
 
 class TVMazeSeries(Base):
     __tablename__ = 'tvmaze_series'
 
     tvmaze_id = Column(Integer, primary_key=True)
     status = Column(Unicode)
     rating = Column(Float)
-    genres = relation(TVMazeGenre, secondary=genres_table)
+    genres = relationship(TVMazeGenre, secondary=genres_table)
     weight = Column(Integer)
     updated = Column(DateTime)  # last time show was updated at tvmaze
     name = Column(Unicode)
     language = Column(Unicode)
     _schedule = Column('schedule', Unicode)
     schedule = json_synonym('_schedule')
     url = Column(String)
@@ -105,21 +105,21 @@
     premiered = Column(DateTime)
     year = Column(Integer)
     summary = Column(Unicode)
     webchannel = Column(String)
     runtime = Column(Integer)
     show_type = Column(String)
     network = Column(Unicode)
-    episodes = relation(
+    episodes = relationship(
         'TVMazeEpisodes',
         order_by='TVMazeEpisodes.season_number',
         cascade='all, delete, delete-orphan',
         backref='series',
     )
-    seasons = relation(
+    seasons = relationship(
         'TVMazeSeason',
         order_by='TVMazeSeason.number',
         cascade='all, delete, delete-orphan',
         backref='series',
     )
 
     last_update = Column(DateTime)  # last time we updated the db for the show
@@ -394,15 +394,17 @@
     logger.debug('trying to add search title {} to series {} in lookup table', title, series.name)
     exist = session.query(TVMazeLookup).filter(TVMazeLookup.search_name == title.lower()).first()
     if exist:
         logger.debug(
             'title {} already exist for series {}, no need to save lookup', title, series.name
         )
         return
-    session.add(TVMazeLookup(search_name=title, series=series))
+    result = TVMazeLookup(search_name=title)
+    session.add(result)
+    result.series = series
 
 
 def prepare_lookup_for_tvmaze(**lookup_params):
     """
     Return a dict of params which is valid with tvmaze API lookups
 
     :param lookup_params: Search parameters
```

### Comparing `FlexGet-3.7.0/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.7.1/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/variables/api.py` & `FlexGet-3.7.1/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/components/variables/variables.py` & `FlexGet-3.7.1/flexget/components/variables/variables.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/config_schema.py` & `FlexGet-3.7.1/flexget/config_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/db_schema.py` & `FlexGet-3.7.1/flexget/db_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import sqlalchemy.event
 from loguru import logger
 from sqlalchemy import Column, DateTime, Integer, String, Table
 from sqlalchemy.exc import OperationalError
-from sqlalchemy.ext.declarative import DeclarativeMeta, as_declarative
+from sqlalchemy.ext.declarative import DeclarativeMeta
+from sqlalchemy.orm import as_declarative
 
 import flexget
 from flexget.event import event
 from flexget.manager import Base, Session
 from flexget.utils.database import with_session
 from flexget.utils.sqlalchemy_utils import table_schema
 from flexget.utils.tools import get_current_flexget_version
@@ -198,15 +199,15 @@
     if plugin not in plugin_schemas:
         raise ValueError('The plugin %s has no stored schema to reset.' % plugin)
     table_names = plugin_schemas[plugin].get('tables', [])
     tables = [table_schema(name, session) for name in table_names]
     # Remove the plugin's tables
     for table in tables:
         try:
-            table.drop()
+            table.drop(bind=session.bind)
         except OperationalError as e:
             if 'no such table' in str(e):
                 continue
             raise e  # Remove the plugin from schema table
     session.query(PluginSchema).filter(PluginSchema.plugin == plugin).delete()
     # We need to commit our current changes to close the session before calling create_all
     session.commit()
```

### Comparing `FlexGet-3.7.0/flexget/entry.py` & `FlexGet-3.7.1/flexget/entry.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/event.py` & `FlexGet-3.7.1/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ipc.py` & `FlexGet-3.7.1/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/log.py` & `FlexGet-3.7.1/flexget/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/manager.py` & `FlexGet-3.7.1/flexget/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 )
 
 import sqlalchemy
 import yaml
 from loguru import logger
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import OperationalError
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker
+from sqlalchemy.orm import declarative_base, sessionmaker
 
 # These need to be declared before we start importing from other flexget modules, since they might import them
 from flexget.config_schema import ConfigError
 from flexget.utils.sqlalchemy_utils import ContextSession
 from flexget.utils.tools import get_current_flexget_version, io_encoding, pid_exists
 
 Base = declarative_base()
```

### Comparing `FlexGet-3.7.0/flexget/options.py` & `FlexGet-3.7.1/flexget/options.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugin.py` & `FlexGet-3.7.1/flexget/plugin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/check.py` & `FlexGet-3.7.1/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/cli_config.py` & `FlexGet-3.7.1/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/database.py` & `FlexGet-3.7.1/flexget/plugins/cli/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from argparse import ArgumentParser
 
+from sqlalchemy import text
+
 from flexget import options
 from flexget.db_schema import plugin_schemas, reset_schema
 from flexget.event import event
 from flexget.manager import Base, Session
 from flexget.terminal import console
 
 
@@ -24,15 +26,15 @@
     console('Database cleanup complete.')
 
 
 def vacuum():
     console('Running VACUUM on sqlite database, this could take a while.')
     session = Session()
     try:
-        session.execute('VACUUM')
+        session.execute(text('VACUUM'))
         session.commit()
     finally:
         session.close()
     console('VACUUM complete.')
 
 
 def reset(manager):
```

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/debug_info.py` & `FlexGet-3.7.1/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/doc.py` & `FlexGet-3.7.1/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.7.1/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/filters.py` & `FlexGet-3.7.1/flexget/plugins/cli/filters.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/inject.py` & `FlexGet-3.7.1/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.7.1/flexget/plugins/cli/perf_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     from flexget.components.imdb.db import Movie
     from flexget.plugins.cli.performance import log_query_count
 
     imdb_urls = []
 
     logger.info('Getting imdb_urls ...')
     # query so that we avoid loading whole object (maybe cached?)
-    for _, url in session.execute(select([Movie.id, Movie.url])):
+    for _, url in session.execute(select(Movie.id, Movie.url)):
         imdb_urls.append(url)
     logger.info('Got {} urls from database', len(imdb_urls))
     if not imdb_urls:
         logger.info('so .. aborting')
         return
 
     # commence testing
```

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/performance.py` & `FlexGet-3.7.1/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/plugins.py` & `FlexGet-3.7.1/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/templates.py` & `FlexGet-3.7.1/flexget/plugins/cli/templates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.7.1/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/web.py` & `FlexGet-3.7.1/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.7.1/flexget/plugins/cli/wiki_qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/cli/win32_service.py` & `FlexGet-3.7.1/flexget/plugins/cli/win32_service.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/aria2.py` & `FlexGet-3.7.1/flexget/plugins/clients/aria2.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/deluge.py` & `FlexGet-3.7.1/flexget/plugins/clients/deluge.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/nzbget.py` & `FlexGet-3.7.1/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/pyload.py` & `FlexGet-3.7.1/flexget/plugins/clients/pyload.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.7.1/flexget/plugins/clients/qbittorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
         if not isinstance(hash_torrent, str):
             logger.error('Error getting torrent info, invalid hash {}', hash_torrent)
             return False
 
         hash_torrent = hash_torrent.lower()
 
-        logger.debug(f'Checking if torrent with hash {repr(hash)} already in session.')
+        logger.debug(f'Checking if torrent with hash {hash!r} already in session.')
 
         url = f'{self.url}{self.api_url_info}'
         params = {'hashes': hash_torrent}
 
         try:
             respose = self.session.request(
                 'get',
```

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.7.1/flexget/plugins/clients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/clients/transmission.py` & `FlexGet-3.7.1/flexget/plugins/clients/transmission.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/daemon/web_server.py` & `FlexGet-3.7.1/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.7.1/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/accept_all.py` & `FlexGet-3.7.1/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/age.py` & `FlexGet-3.7.1/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/best_quality.py` & `FlexGet-3.7.1/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/content_filter.py` & `FlexGet-3.7.1/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/content_size.py` & `FlexGet-3.7.1/flexget/plugins/filter/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.7.1/flexget/plugins/filter/crossmatch.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/delay.py` & `FlexGet-3.7.1/flexget/plugins/filter/delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         ver = 1
     if ver == 1:
         table = table_schema('delay', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('delay', session)
         failures = 0
-        for row in session.execute(select([table.c.id, table.c.entry])):
+        for row in session.execute(select(table.c.id, table.c.entry)):
             try:
                 p = pickle.loads(row['entry'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
@@ -61,15 +61,15 @@
             logger.error(
                 'Error upgrading {} pickle objects. Some delay information has been lost.',
                 failures,
             )
         ver = 2
     if ver == 2:
         table = table_schema('delay', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/duplicates.py` & `FlexGet-3.7.1/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/exists.py` & `FlexGet-3.7.1/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.7.1/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/exists_series.py` & `FlexGet-3.7.1/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/if_condition.py` & `FlexGet-3.7.1/flexget/plugins/filter/if_condition.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/limit_new.py` & `FlexGet-3.7.1/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/magnets.py` & `FlexGet-3.7.1/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/only_new.py` & `FlexGet-3.7.1/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.7.1/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/quality.py` & `FlexGet-3.7.1/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/regexp.py` & `FlexGet-3.7.1/flexget/plugins/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/require_field.py` & `FlexGet-3.7.1/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.7.1/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.7.1/flexget/plugins/filter/thetvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/timeframe.py` & `FlexGet-3.7.1/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/unique.py` & `FlexGet-3.7.1/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/filter/upgrade.py` & `FlexGet-3.7.1/flexget/plugins/filter/upgrade.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/generic/cron_env.py` & `FlexGet-3.7.1/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.7.1/flexget/plugins/generic/db_vacuum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
 
 from loguru import logger
+from sqlalchemy import text
 from sqlalchemy.exc import OperationalError
 
 from flexget.event import event
 from flexget.manager import Session
 from flexget.utils.simple_persistence import SimplePersistence
 
 logger = logger.bind(name='db_vacuum')
@@ -17,13 +18,13 @@
     # Vacuum can take a long time, and is not needed frequently
     persistence = SimplePersistence('db_vacuum')
     last_vacuum = persistence.get('last_vacuum')
     if not last_vacuum or last_vacuum < datetime.now() - VACUUM_INTERVAL:
         logger.info('Running VACUUM on database to improve performance and decrease db size.')
         with Session() as session:
             try:
-                session.execute('VACUUM')
+                session.execute(text('VACUUM'))
             except OperationalError as e:
                 # Does not work on python 3.6, github issue #1596
                 logger.error('Could not execute VACUUM command: {}', e)
             else:
                 persistence['last_vacuum'] = datetime.now()
```

### Comparing `FlexGet-3.7.0/flexget/plugins/generic/log_start.py` & `FlexGet-3.7.1/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/generic/urlfix.py` & `FlexGet-3.7.1/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/generic/welcome.py` & `FlexGet-3.7.1/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/anidb_list.py` & `FlexGet-3.7.1/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/anilist.py` & `FlexGet-3.7.1/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.7.1/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.7.1/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/discover.py` & `FlexGet-3.7.1/flexget/plugins/input/discover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/filesystem.py` & `FlexGet-3.7.1/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.7.1/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.7.1/flexget/plugins/input/from_piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/from_task.py` & `FlexGet-3.7.1/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/from_telegram.py` & `FlexGet-3.7.1/flexget/plugins/input/from_telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
             # Create Base Entry
             text = message['message']['text']
             entry = Entry()
             entry['title'] = text
 
             # We need a url, so we add a dummy
-            entry['url'] = f"http://localhost?update_id={str(update_id)}"
+            entry['url'] = f"http://localhost?update_id={update_id!s}"
 
             # Store the message if we need to use it in other plugins
             entry['telegram_message'] = message['message']
 
             # Check From
             message_from = message['message']['from']
             message_chat = message['message']['chat']
```

### Comparing `FlexGet-3.7.0/flexget/plugins/input/gazelle.py` & `FlexGet-3.7.1/flexget/plugins/input/gazelle.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/generate.py` & `FlexGet-3.7.1/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/html.py` & `FlexGet-3.7.1/flexget/plugins/input/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/input_csv.py` & `FlexGet-3.7.1/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/inputs.py` & `FlexGet-3.7.1/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/json.py` & `FlexGet-3.7.1/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/kitsu.py` & `FlexGet-3.7.1/flexget/plugins/input/kitsu.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/letterboxd.py` & `FlexGet-3.7.1/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/limit.py` & `FlexGet-3.7.1/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/medusa.py` & `FlexGet-3.7.1/flexget/plugins/input/medusa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/mock.py` & `FlexGet-3.7.1/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.7.1/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.7.1/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.7.1/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.7.1/flexget/plugins/input/npo_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/parameterize.py` & `FlexGet-3.7.1/flexget/plugins/input/parameterize.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/plex.py` & `FlexGet-3.7.1/flexget/plugins/input/plex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/pogcal.py` & `FlexGet-3.7.1/flexget/plugins/input/pogcal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.7.1/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/rlslog.py` & `FlexGet-3.7.1/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.7.1/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/rss.py` & `FlexGet-3.7.1/flexget/plugins/input/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/sceper.py` & `FlexGet-3.7.1/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/sickbeard.py` & `FlexGet-3.7.1/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/tail.py` & `FlexGet-3.7.1/flexget/plugins/input/tail.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/text.py` & `FlexGet-3.7.1/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/torznab.py` & `FlexGet-3.7.1/flexget/plugins/input/torznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.7.1/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.7.1/flexget/plugins/internal/api_bluray.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from json.decoder import JSONDecodeError
 from typing import Any, Dict, Optional
 
 from dateutil.parser import parse as dateutil_parse
 from loguru import logger
 from sqlalchemy import Column, Date, DateTime, Float, Integer, Table, Unicode, func
 from sqlalchemy.ext.associationproxy import association_proxy
-from sqlalchemy.orm import Session, relation
+from sqlalchemy.orm import Session, relationship
 from sqlalchemy.schema import ForeignKey
 
 from flexget import db_schema, plugin
 from flexget.event import event
 from flexget.plugin import PluginError
 from flexget.utils import requests
 from flexget.utils.database import year_property
@@ -66,15 +66,15 @@
     runtime = Column(Integer)
     overview = Column(Unicode)
     country = Column(Unicode)
     studio = Column(Unicode)
     rating = Column(Float)
     bluray_rating = Column(Integer)
     certification = Column(Unicode)
-    _genres = relation('BlurayGenre', secondary=genres_table, backref='movies')
+    _genres = relationship('BlurayGenre', secondary=genres_table, backref='movies')
     genres = association_proxy('_genres', 'name')
     updated = Column(DateTime, default=datetime.now, nullable=False)
 
     def __init__(self, title: str, year: Optional[int]) -> None:
         if year:
             title_year = f'{title} ({year})'
         else:
@@ -184,15 +184,15 @@
 
 
 class BluraySearchResult(Base):
     __tablename__ = 'bluray_search_results'
 
     search = Column(Unicode, primary_key=True)
     movie_id = Column(Integer, ForeignKey('bluray_movies.id'), nullable=True)
-    movie = relation(BlurayMovie)
+    movie = relationship(BlurayMovie)
 
     def __init__(
         self, search: str, movie_id: Optional[int] = None, movie: Optional[BlurayMovie] = None
     ) -> None:
         self.search = search.lower()
         if movie_id:
             self.movie_id = movie_id
```

### Comparing `FlexGet-3.7.0/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.7.1/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict, Optional, Type
 from urllib.error import URLError
 from urllib.parse import quote_plus
 
 from loguru import logger
 from sqlalchemy import Column, DateTime, Integer, String, Table, func, sql
-from sqlalchemy.orm import Session, relation
+from sqlalchemy.orm import Session, relationship
 from sqlalchemy.schema import ForeignKey, Index
 
 from flexget import db_schema, plugin
 from flexget.plugin import PluginError, internet
 from flexget.utils import requests
 from flexget.utils.database import text_date_synonym, with_session
 from flexget.utils.sqlalchemy_utils import table_add_column, table_schema
@@ -106,35 +106,39 @@
 
 class RottenTomatoesMovie(RottenTomatoesContainer, Base):
     __tablename__ = 'rottentomatoes_movies'
 
     id = Column(Integer, primary_key=True, autoincrement=False, nullable=False)
     title = Column(String)
     year = Column(Integer)
-    genres = relation('RottenTomatoesGenre', secondary=genres_table, backref='movies')
+    genres = relationship('RottenTomatoesGenre', secondary=genres_table, backref='movies')
     mpaa_rating = Column(String)
     runtime = Column(Integer)
     critics_consensus = Column(String)
-    release_dates = relation('ReleaseDate', backref='movie', cascade='all, delete, delete-orphan')
+    release_dates = relationship(
+        'ReleaseDate', backref='movie', cascade='all, delete, delete-orphan'
+    )
     critics_rating = Column(String)
     critics_score = Column(Integer)
     audience_rating = Column(String)
     audience_score = Column(Integer)
     synopsis = Column(String)
-    posters = relation(
+    posters = relationship(
         'RottenTomatoesPoster', backref='movie', cascade='all, delete, delete-orphan'
     )
-    cast = relation('RottenTomatoesActor', secondary=actors_table, backref='movies')
-    directors = relation('RottenTomatoesDirector', secondary=directors_table, backref='movies')
+    cast = relationship('RottenTomatoesActor', secondary=actors_table, backref='movies')
+    directors = relationship('RottenTomatoesDirector', secondary=directors_table, backref='movies')
     studio = Column(String)
     # NOTE: alternate_ids is not anymore used, it used to store imdb_id
-    alternate_ids = relation(
+    alternate_ids = relationship(
         'RottenTomatoesAlternateId', backref='movie', cascade='all, delete, delete-orphan'
     )
-    links = relation('RottenTomatoesLink', backref='movie', cascade='all, delete, delete-orphan')
+    links = relationship(
+        'RottenTomatoesLink', backref='movie', cascade='all, delete, delete-orphan'
+    )
 
     # updated time, so we can grab new rating counts after 48 hours
     # set a default, so existing data gets updated with a rating
     updated = Column(DateTime)
 
     @property
     def expired(self) -> bool:
@@ -244,15 +248,15 @@
 
 class RottenTomatoesSearchResult(Base):
     __tablename__ = 'rottentomatoes_search_results'
 
     id = Column(Integer, primary_key=True)
     search = Column(String, nullable=False)
     movie_id = Column(Integer, ForeignKey('rottentomatoes_movies.id'), nullable=False)
-    movie = relation(RottenTomatoesMovie, backref='search_strings')
+    movie = relationship(RottenTomatoesMovie, backref='search_strings')
 
     def __repr__(self) -> str:
         return '<RottenTomatoesSearchResult(search={},movie_id={},movie={})>'.format(
             self.search,
             self.movie_id,
             self.movie,
         )
```

### Comparing `FlexGet-3.7.0/flexget/plugins/internal/change_warn.py` & `FlexGet-3.7.1/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/media_id.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/nzb_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/quality.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/subtitles_check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/metainfo/task.py` & `FlexGet-3.7.1/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/extension.py` & `FlexGet-3.7.1/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/headers.py` & `FlexGet-3.7.1/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/manipulate.py` & `FlexGet-3.7.1/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.7.1/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.7.1/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.7.1/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.7.1/flexget/plugins/modify/regex_extract.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.7.1/flexget/plugins/modify/reorder_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/set_field.py` & `FlexGet-3.7.1/flexget/plugins/modify/set_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/sort_by.py` & `FlexGet-3.7.1/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.7.1/flexget/plugins/modify/sort_by_weight.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.7.1/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/cookies.py` & `FlexGet-3.7.1/flexget/plugins/operate/cookies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.7.1/flexget/plugins/operate/debug_db_sessions.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.7.1/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/digest.py` & `FlexGet-3.7.1/flexget/plugins/operate/digest.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
     if None is ver:
         ver = 0
     if ver == 0:
         table = table_schema('digest_entries', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('digest_entries', session)
-        for row in session.execute(select([table.c.id, table.c.entry])):
+        for row in session.execute(select(table.c.id, table.c.entry)):
             try:
                 p = pickle.loads(row['entry'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
             except KeyError as e:
                 logger.error('Unable error upgrading backlog pickle object due to {}', str(e))
 
         ver = 1
     if ver == 1:
         table = table_schema('digest_entries', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             title = str(data.pop('title'))
             e = Entry(title=title, **data)
```

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/disable.py` & `FlexGet-3.7.1/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.7.1/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.7.1/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.7.1/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/formlogin.py` & `FlexGet-3.7.1/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/free_space.py` & `FlexGet-3.7.1/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/include.py` & `FlexGet-3.7.1/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/interval.py` & `FlexGet-3.7.1/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/log_filter.py` & `FlexGet-3.7.1/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/manual.py` & `FlexGet-3.7.1/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.7.1/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.7.1/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/priority.py` & `FlexGet-3.7.1/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/proxy.py` & `FlexGet-3.7.1/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/rerun.py` & `FlexGet-3.7.1/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/run_task.py` & `FlexGet-3.7.1/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/sequence.py` & `FlexGet-3.7.1/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/sleep.py` & `FlexGet-3.7.1/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.7.1/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/template.py` & `FlexGet-3.7.1/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/verbose.py` & `FlexGet-3.7.1/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.7.1/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.7.1/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/operate/version_checker.py` & `FlexGet-3.7.1/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/download.py` & `FlexGet-3.7.1/flexget/plugins/output/download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/download_auth.py` & `FlexGet-3.7.1/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/dump.py` & `FlexGet-3.7.1/flexget/plugins/output/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                         renderable = escape(value.replace('\r', '').replace('\n', ''))
                     elif is_expandable(value):
                         renderable = Pretty(value)
                     else:
                         try:
                             renderable = highlighter(str(value))
                         except Exception:
-                            renderable = f'[[i]not printable[/i]] ({repr(value)})'
+                            renderable = f'[[i]not printable[/i]] ({value!r})'
             entry_table.add_row(f'{field}', ': ', renderable)
         console(entry_table)
         if trace:
             console('── Processing trace:', style='italic')
             trace_table = TerminalTable(
                 'Plugin',
                 'Operation',
```

### Comparing `FlexGet-3.7.0/flexget/plugins/output/dump_config.py` & `FlexGet-3.7.1/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/exec.py` & `FlexGet-3.7.1/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/file_operations.py` & `FlexGet-3.7.1/flexget/plugins/output/file_operations.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/html.py` & `FlexGet-3.7.1/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/memusage.py` & `FlexGet-3.7.1/flexget/plugins/output/memusage.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/mock_output.py` & `FlexGet-3.7.1/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/rss.py` & `FlexGet-3.7.1/flexget/plugins/output/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.7.1/flexget/plugins/output/rtorrent_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.7.1/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/sns.py` & `FlexGet-3.7.1/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/subtitles.py` & `FlexGet-3.7.1/flexget/plugins/output/subtitles.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.7.1/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.7.1/flexget/plugins/output/subtitles_subliminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/symlink.py` & `FlexGet-3.7.1/flexget/plugins/output/symlink.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/output/utorrent.py` & `FlexGet-3.7.1/flexget/plugins/output/utorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/services/kodi_library.py` & `FlexGet-3.7.1/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/plugins/services/myepisodes.py` & `FlexGet-3.7.1/flexget/plugins/services/myepisodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         """
 
         url = "http://www.myepisodes.com/ajax/service.php?mode=eps_update"
         myepisodes_id = entry['myepisodes_id']
         season = entry['series_season']
         episode = entry['series_episode']
 
-        super_secret_code = f"A{str(myepisodes_id)}-{str(season)}-{str(episode)}"
+        super_secret_code = f"A{myepisodes_id!s}-{season!s}-{episode!s}"
 
         payload = {super_secret_code: "true"}
 
         if self.test_mode:
             logger.info(
                 'Would mark {} of `{}` as acquired.', entry['series_id'], entry['series_name']
             )
```

### Comparing `FlexGet-3.7.0/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.7.1/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/resources/flexget.png` & `FlexGet-3.7.1/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/task.py` & `FlexGet-3.7.1/flexget/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/task_queue.py` & `FlexGet-3.7.1/flexget/task_queue.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/templates/task/default.template` & `FlexGet-3.7.1/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/templates/task/html.template` & `FlexGet-3.7.1/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/templates/task/rss.template` & `FlexGet-3.7.1/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/terminal.py` & `FlexGet-3.7.1/flexget/terminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/tray_icon.py` & `FlexGet-3.7.1/flexget/tray_icon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/__init__.py` & `FlexGet-3.7.1/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/app.html` & `FlexGet-3.7.1/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.7.1/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.7.1/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.7.1/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.7.1/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.7.1/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.7.1/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.7.1/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.7.1/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.7.1/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/bower.json` & `FlexGet-3.7.1/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/build.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/server.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/test.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.7.1/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/karma.conf.js` & `FlexGet-3.7.1/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/package.json` & `FlexGet-3.7.1/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/specs.html` & `FlexGet-3.7.1/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/app.html` & `FlexGet-3.7.1/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/app.module.js` & `FlexGet-3.7.1/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/app.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.7.1/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.7.1/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.7.1/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.7.1/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.7.1/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.7.1/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.7.1/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/__init__.py` & `FlexGet-3.7.1/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.7.1/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/ui/v2/dist/index.html` & `FlexGet-3.7.1/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/bittorrent.py` & `FlexGet-3.7.1/flexget/utils/bittorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/cache.py` & `FlexGet-3.7.1/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/cached_input.py` & `FlexGet-3.7.1/flexget/utils/cached_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timedelta
 from functools import partial
 from typing import TYPE_CHECKING, Callable, Iterable, List, Optional
 
 from loguru import logger
 from sqlalchemy import Column, DateTime, ForeignKey, Integer, String, Unicode, select
 from sqlalchemy.orm import Session as DBSession
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import relationship
 
 from flexget import db_schema
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.manager import Session
 from flexget.plugin import PluginError
 from flexget.utils import json, serialization
@@ -34,28 +34,28 @@
 @db_schema.upgrade('input_cache')
 def upgrade(ver: int, session: DBSession) -> int:
     if ver == 0:
         table = table_schema('input_cache_entry', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('input_cache_entry', session)
-        for row in session.execute(select([table.c.id, table.c.entry])):
+        for row in session.execute(select(table.c.id, table.c.entry)):
             try:
                 p = pickle.loads(row['entry'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
             except KeyError as ex:
                 logger.error(f'Unable error upgrading input_cache pickle object due to {ex}')
         ver = 1
     if ver == 1:
         table = table_schema('input_cache_entry', session)
-        for row in session.execute(select([table.c.id, table.c.json])):
+        for row in session.execute(select(table.c.id, table.c.json)):
             if not row['json']:
                 # Seems there could be invalid data somehow. See #2590
                 continue
             data = json.loads(row['json'], decode_datetime=True)
             # If title looked like a date, make sure it's a string
             # Had a weird case of an entry without a title: https://github.com/Flexget/Flexget/issues/2636
             title = data.pop('title', None)
@@ -73,15 +73,17 @@
     __tablename__ = 'input_cache'
 
     id = Column(Integer, primary_key=True)
     name = Column(Unicode)
     hash = Column(String)
     added = Column(DateTime, default=datetime.now)
 
-    entries = relation('InputCacheEntry', backref='cache', cascade='all, delete, delete-orphan')
+    entries = relationship(
+        'InputCacheEntry', backref='cache', cascade='all, delete, delete-orphan'
+    )
 
 
 class InputCacheEntry(Base):
     __tablename__ = 'input_cache_entry'
 
     id = Column(Integer, primary_key=True)
     _json = Column('json', Unicode)
```

### Comparing `FlexGet-3.7.0/flexget/utils/database.py` & `FlexGet-3.7.1/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/json.py` & `FlexGet-3.7.1/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/lazy_dict.py` & `FlexGet-3.7.1/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/log.py` & `FlexGet-3.7.1/flexget/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @db_schema.upgrade('log_once')
 def upgrade(ver: Optional[int], session: Session):
     if ver is None:
         logger.info('Adding index to md5sum column of log_once table.')
         table = table_schema('log_once', session)
-        Index('log_once_md5sum', table.c.md5sum, unique=True).create()
+        Index('log_once_md5sum', table.c.md5sum, unique=True).create(bind=session.bind)
         ver = 0
     return ver
 
 
 class LogMessage(Base):
     """Declarative"""
```

### Comparing `FlexGet-3.7.0/flexget/utils/parsers/generic.py` & `FlexGet-3.7.1/flexget/utils/parsers/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __unicode__(self):
         return self.value
 
     def __str__(self):
         return self.__unicode__().encode('utf-8')
 
     def __repr__(self):
-        return f'ParseWarning({self}, **{repr(self.kwargs)})'
+        return f'ParseWarning({self}, **{self.kwargs!r})'
 
 
 default_ignore_prefixes = [
     r'(?:\[[^\[\]]*\])',  # ignores group names before the name, eg [foobar] name
     r'(?:HD.720p?:)',
     r'(?:HD.1080p?:)',
     r'(?:HD.2160p?:)',
```

### Comparing `FlexGet-3.7.0/flexget/utils/parsers/movie.py` & `FlexGet-3.7.1/flexget/utils/parsers/movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/parsers/parser.py` & `FlexGet-3.7.1/flexget/utils/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/parsers/series.py` & `FlexGet-3.7.1/flexget/utils/parsers/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/pathscrub.py` & `FlexGet-3.7.1/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/qualities.py` & `FlexGet-3.7.1/flexget/utils/qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/requests.py` & `FlexGet-3.7.1/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/serialization.py` & `FlexGet-3.7.1/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/simple_persistence.py` & `FlexGet-3.7.1/flexget/utils/simple_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         # Upgrade to version 0 was a failed attempt at cleaning bad entries from our table, better attempt in ver 1
         ver = 0
     if ver == 0:
         try:
             # Remove any values that are not loadable.
             table = table_schema('simple_persistence', session)
             for row in session.execute(
-                select([table.c.id, table.c.plugin, table.c.key, table.c.value])
+                select(table.c.id, table.c.plugin, table.c.key, table.c.value)
             ):
                 try:
                     pickle.loads(row['value'])
                 except Exception as e:
                     logger.warning(
                         "Couldn't load {}:{} removing from db: {}", row['plugin'], row['key'], e
                     )
@@ -59,15 +59,15 @@
         ver = 2
     if ver == 2 or ver == 3:
         table = table_schema('simple_persistence', session)
         table_add_column(table, 'json', Unicode, session)
         # Make sure we get the new schema with the added column
         table = table_schema('simple_persistence', session)
         failures = 0
-        for row in session.execute(select([table.c.id, table.c.value])):
+        for row in session.execute(select(table.c.id, table.c.value)):
             try:
                 p = pickle.loads(row['value'])
                 session.execute(
                     table.update()
                     .where(table.c.id == row['id'])
                     .values(json=json.dumps(p, encode_datetime=True))
                 )
```

### Comparing `FlexGet-3.7.0/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.7.1/flexget/utils/sqlalchemy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Miscellaneous SQLAlchemy helpers.
 """
 from typing import Any, List, Optional, Union
 
 from loguru import logger
-from sqlalchemy import ColumnDefault, Index, Sequence
+from sqlalchemy import ColumnDefault, Index, Sequence, text
 from sqlalchemy.exc import NoSuchTableError, OperationalError
 from sqlalchemy.orm import Session
 from sqlalchemy.schema import MetaData, Table
 from sqlalchemy.types import TypeEngine
 
 logger = logger.bind(name='sql_utils')
 
@@ -30,15 +30,15 @@
 
 
 def table_schema(name: str, session: Session) -> Table:
     """
     :returns: Table schema using SQLAlchemy reflect as it currently exists in the db
     :rtype: Table
     """
-    return Table(name, MetaData(bind=session.bind), autoload=True)
+    return Table(name, MetaData(), autoload_with=session.bind)
 
 
 def table_columns(table: Union[str, Table], session: Session) -> List[str]:
     """
     :param string table: Name of table or table schema
     :param Session session: SQLAlchemy Session
     :returns: List of column names in the table or empty list
@@ -77,15 +77,15 @@
         return
     # Add the column to the table
     if not isinstance(col_type, TypeEngine):
         # If we got a type class instead of an instance of one, instantiate it
         col_type = col_type()
     type_string = session.bind.engine.dialect.type_compiler.process(col_type)
     statement = f'ALTER TABLE {table.name} ADD {name} {type_string}'
-    session.execute(statement)
+    session.execute(text(statement))
     session.commit()
     # Update the table with the default value if given
     if default is not None:
         # Get the new schema with added column
         table = table_schema(table.name, session)
         if not isinstance(default, (ColumnDefault, Sequence)):
             default = ColumnDefault(default)
@@ -131,20 +131,23 @@
     try:
         Index(index_name, *columns).create(bind=session.bind)
     except OperationalError:
         logger.opt(exception=True).debug('Error creating index.')
 
 
 class ContextSession(Session):
-    """:class:`sqlalchemy.orm.Session` which can be used as context manager"""
+    """:class:`sqlalchemy.orm.Session` which automatically commits when used as context manager without errors"""
+
+    # TODO: This auto-committing might be a bad idea and need to be removed
+    # might be hard to figure out where exactly code needs to be updated to compensate though.
 
     def __enter__(self) -> 'ContextSession':
-        return self
+        return super().__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             if exc_type is None:
                 self.commit()
             else:
                 self.rollback()
         finally:
-            self.close()
+            super().__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `FlexGet-3.7.0/flexget/utils/template.py` & `FlexGet-3.7.1/flexget/utils/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/flexget/utils/tools.py` & `FlexGet-3.7.1/flexget/utils/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 if isinstance(v, dict):
                     merge_dict_from_to(d1[k], d2[k])
                 elif isinstance(v, list):
                     d2[k].extend(copy.deepcopy(v))
                 elif isinstance(v, (str, bool, int, float, type(None))):
                     pass
                 else:
-                    raise Exception(f'Unknown type: {type(v)} value: {repr(v)} in dictionary')
+                    raise Exception(f'Unknown type: {type(v)} value: {v!r} in dictionary')
             elif isinstance(v, (str, bool, int, float, list, type(None))) and isinstance(
                 d2[k], (str, bool, int, float, list, type(None))
             ):
                 # Allow overriding of non-container types with other non-container types
                 pass
             else:
                 raise MergeException(
```

### Comparing `FlexGet-3.7.0/flexget/webserver.py` & `FlexGet-3.7.1/flexget/webserver.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.7.0/pyproject.toml` & `FlexGet-3.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 name = "flexget"
 version = "0.0.0"
 description = ""
 authors = []
 
 [tool.poetry.dependencies]
 python = "^3.7"
-apscheduler = ">=3.2.0"
+apscheduler = ">=3.10.0"
 beautifulsoup4 = ">=4.5"
 colorama = ">=0.4.4"
 feedparser = ">=6.0.2"
 guessit = ">=3.4,<4.0"
 html5lib = ">=0.11"
 importlib-metadata = { version = "*", python = "<3.8" }  # TODO: remove this after we drop python3.7
 jinja2 = ">=3.0,<4.0"
@@ -70,27 +70,27 @@
 pyrss2gen = "^1.1"
 python-dateutil = "^2.8.2"
 pyyaml = ">=4.2b1"
 rebulk = ">=2.0.0"
 requests = ">=2.20.0"
 rich = ">=9.0.0"
 rpyc = ">=5.0,!=5.2.*,!=5.3.0"  # 5.2.1-5.3.0 cause a hang https://github.com/Flexget/Flexget/issues/3601
-sqlalchemy = ">=1.3.10,<1.999"
+sqlalchemy = ">=2.0,<2.999"
 # WebUI/API Deps
 cherrypy = ">=18.0.0"
 flask-compress = ">=1.2.1"
 flask-cors = ">=2.1.2"
 flask-login = ">=0.4.0"
 flask-restful = ">=0.3.3"
 flask-restx = ">=0.5.1"
 flask = ">=0.7"
 packaging = ">=21.3"
 pyparsing = ">=2.4.7"
 werkzeug = ">=2.2.3"
-zxcvbn-python = "^4.4.24"
+zxcvbn = "^4.4.24"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=18.9b0"
 codacy-coverage = ">=1.2.18"
 coverage = ">=6.0"
 gitpython = ">=3.1.18"
 pre-commit = ">=2.9.0"
```

### Comparing `FlexGet-3.7.0/requirements-docker.txt` & `FlexGet-3.7.1/requirements-docker.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "4.0"
-apscheduler==3.9.1.post1 ; python_version >= "3.7" and python_version < "4"
+apscheduler==3.10.1 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
 autocommand==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
-charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4.0"
+charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 cloudscraper==1.2.69 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 deluge-client==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.1 ; python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"
+greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
-idna==3.4 ; python_version >= "3.7" and python_version < "4"
+idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
@@ -48,34 +48,34 @@
 pydantic==1.10.2 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pynzb==0.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
-pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
-pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
+pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4.0"
+pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
 qbittorrent-api==2023.3.44 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
-requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
+requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
-setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
-six==1.16.0 ; python_version >= "3.7" and python_version < "4"
+six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
-sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
+sqlalchemy==2.0.15 ; python_version >= "3.7" and python_version < "4.0"
 tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 transmission-rpc==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
-tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
-urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
+tzdata==2022.7 ; python_version >= "3.7" and python_version < "4.0"
+tzlocal==4.2 ; python_version >= "3.7" and python_version < "4.0"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
-zxcvbn-python==4.4.24 ; python_version >= "3.7" and python_version < "4.0"
+zxcvbn==4.4.28 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.7.0/requirements.txt` & `FlexGet-3.7.1/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "4.0"
-apscheduler==3.9.1.post1 ; python_version >= "3.7" and python_version < "4"
+apscheduler==3.10.1 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
 autocommand==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
-charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4.0"
+charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.5 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.1 ; python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"
+greenlet==2.0.1 ; python_version >= "3.7" and python_version < "4.0" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32")
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
-idna==3.4 ; python_version >= "3.7" and python_version < "4"
+idna==3.4 ; python_version >= "3.7" and python_version < "4.0"
 importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
 importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
@@ -46,31 +46,31 @@
 pydantic==1.10.2 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pynzb==0.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
-pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
-pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
+pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4.0"
+pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
+requests==2.31.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
-setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
-six==1.16.0 ; python_version >= "3.7" and python_version < "4"
+six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
-sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
+sqlalchemy==2.0.15 ; python_version >= "3.7" and python_version < "4.0"
 tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
-tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
-urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
+tzdata==2022.7 ; python_version >= "3.7" and python_version < "4.0"
+tzlocal==4.2 ; python_version >= "3.7" and python_version < "4.0"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
 zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
-zxcvbn-python==4.4.24 ; python_version >= "3.7" and python_version < "4.0"
+zxcvbn==4.4.28 ; python_version >= "3.7" and python_version < "4.0"
```

