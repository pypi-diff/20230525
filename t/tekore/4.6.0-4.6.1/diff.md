# Comparing `tmp/tekore-4.6.0.tar.gz` & `tmp/tekore-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tekore-4.6.0.tar", last modified: Wed Apr 12 18:05:49 2023, max compression
+gzip compressed data, was "tekore-4.6.1.tar", last modified: Thu May 25 06:12:13 2023, max compression
```

## Comparing `tekore-4.6.0.tar` & `tekore-4.6.1.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.319480 tekore-4.6.0/
--rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-4.6.0/LICENSE
--rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-4.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5362 2023-04-12 18:05:49.319480 tekore-4.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4184 2023-01-05 23:44:39.000000 tekore-4.6.0/contributing.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.220962 tekore-4.6.0/docs/
--rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.227964 tekore-4.6.0/docs/src/
--rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/404.rst
--rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/advanced_usage.rst
--rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/auth_guide.rst
--rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-4.6.0/docs/src/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.230964 tekore-4.6.0/docs/src/examples/
--rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-4.6.0/docs/src/examples/artist_follower.rst
--rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-4.6.0/docs/src/examples/async_server.rst
--rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-4.6.0/docs/src/examples/auth_server.rst
--rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-4.6.0/docs/src/examples/creating_scripts.rst
--rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-4.6.0/docs/src/examples/discord_bot.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.236465 tekore-4.6.0/docs/src/examples/scripts/
--rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/albums_top_artist.rst
--rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/analyse_from_playlist.rst
--rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/follow_by_search.rst
--rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/follow_category_playlist.rst
--rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/play_saved_album.rst
--rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/recommended_playlist.rst
--rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/related_artists_top_artist.rst
--rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-4.6.0/docs/src/examples/scripts/scrape_playlists.rst
--rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/tracks_new_release.rst
--rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/examples/scripts.rst
--rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/examples.rst
--rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-4.6.0/docs/src/getting_started.rst
--rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-4.6.0/docs/src/index.rst
--rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-4.6.0/docs/src/logo.png
--rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-4.6.0/docs/src/logo_small.png
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.240966 tekore-4.6.0/docs/src/reference/
--rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-4.6.0/docs/src/reference/auth.rst
--rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/client.rst
--rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/reference/config.rst
--rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-4.6.0/docs/src/reference/conversions.rst
--rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/errors.rst
--rw-rw-rw-   0        0        0     7784 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/models.rst
--rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-4.6.0/docs/src/reference/senders.rst
--rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference.rst
--rw-rw-rw-   0        0        0    19676 2023-04-12 17:55:05.000000 tekore-4.6.0/docs/src/release_notes.rst
--rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-4.6.0/docs/src/resources.rst
--rw-rw-rw-   0        0        0     2069 2023-04-12 17:36:57.000000 tekore-4.6.0/pyproject.toml
--rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-4.6.0/readme_pypi.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.243466 tekore-4.6.0/requirements/
--rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/build
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/checks
--rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/dev
--rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/docs
--rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/tests
--rw-rw-rw-   0        0        0       42 2023-04-12 18:05:49.319480 tekore-4.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.212961 tekore-4.6.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.245467 tekore-4.6.0/src/tekore/
--rw-rw-rw-   0        0        0     2610 2023-04-12 17:55:05.000000 tekore-4.6.0/src/tekore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.250968 tekore-4.6.0/src/tekore/_auth/
--rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.252968 tekore-4.6.0/src/tekore/_auth/expiring/
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/__init__.py
--rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/client.py
--rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/decor.py
--rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/token.py
--rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/refreshing.py
--rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/scope.py
--rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.256969 tekore-4.6.0/src/tekore/_client/
--rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.266470 tekore-4.6.0/src/tekore/_client/api/
--rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/__init__.py
--rw-rw-rw-   0        0        0     1955 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/album.py
--rw-rw-rw-   0        0        0     3186 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/artist.py
--rw-rw-rw-   0        0        0     2866 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/audiobook.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.267971 tekore-4.6.0/src/tekore/_client/api/browse/
--rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/browse/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/browse/validate.py
--rw-rw-rw-   0        0        0     1761 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/chapter.py
--rw-rw-rw-   0        0        0     1762 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/episode.py
--rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/follow.py
--rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/library.py
--rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/markets.py
--rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/personalisation.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.269971 tekore-4.6.0/src/tekore/_client/api/player/
--rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/__init__.py
--rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/modify.py
--rw-rw-rw-   0        0        0     4091 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/view.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.272471 tekore-4.6.0/src/tekore/_client/api/playlist/
--rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/__init__.py
--rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/items.py
--rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/modify.py
--rw-rw-rw-   0        0        0     7617 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/view.py
--rw-rw-rw-   0        0        0     3578 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/search.py
--rw-rw-rw-   0        0        0     2985 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/show.py
--rw-rw-rw-   0        0        0     2469 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/track.py
--rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/user.py
--rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/base.py
--rw-rw-rw-   0        0        0     4194 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/chunked.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.273471 tekore-4.6.0/src/tekore/_client/decor/
--rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/decor/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/decor/handle.py
--rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/full.py
--rw-rw-rw-   0        0        0     4299 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/paging.py
--rw-rw-rw-   0        0        0     1316 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/process.py
--rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_config.py
--rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.287474 tekore-4.6.0/src/tekore/_model/
--rw-rw-rw-   0        0        0     2394 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.288974 tekore-4.6.0/src/tekore/_model/album/
--rw-rw-rw-   0        0        0     1442 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/album/__init__.py
--rw-rw-rw-   0        0        0      990 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/album/base.py
--rw-rw-rw-   0        0        0     1788 2023-03-26 08:36:33.000000 tekore-4.6.0/src/tekore/_model/album/full.py
--rw-rw-rw-   0        0        0     1369 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/artist.py
--rw-rw-rw-   0        0        0     2336 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audio_analysis.py
--rw-rw-rw-   0        0        0      518 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audio_features.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.290475 tekore-4.6.0/src/tekore/_model/audiobook/
--rw-rw-rw-   0        0        0      607 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/base.py
--rw-rw-rw-   0        0        0      468 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/full.py
--rw-rw-rw-   0        0        0      335 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/base.py
--rw-rw-rw-   0        0        0      679 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/category.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.291975 tekore-4.6.0/src/tekore/_model/chapter/
--rw-rw-rw-   0        0        0      860 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_model/chapter/__init__.py
--rw-rw-rw-   0        0        0      900 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/chapter/base.py
--rw-rw-rw-   0        0        0      627 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_model/chapter/full.py
--rw-rw-rw-   0        0        0      522 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/context.py
--rw-rw-rw-   0        0        0     3070 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/currently_playing.py
--rw-rw-rw-   0        0        0      845 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/device.py
--rw-rw-rw-   0        0        0     2563 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/episode.py
--rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/error.py
--rw-rw-rw-   0        0        0     1362 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/local.py
--rw-rw-rw-   0        0        0     1110 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/member.py
--rw-rw-rw-   0        0        0      834 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/paging.py
--rw-rw-rw-   0        0        0     1291 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/play_history.py
--rw-rw-rw-   0        0        0     3789 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/playlist.py
--rw-rw-rw-   0        0        0     1259 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/recommendations.py
--rw-rw-rw-   0        0        0     7555 2023-04-12 17:42:29.000000 tekore-4.6.0/src/tekore/_model/serialise.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.293475 tekore-4.6.0/src/tekore/_model/show/
--rw-rw-rw-   0        0        0     1176 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/__init__.py
--rw-rw-rw-   0        0        0      907 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/base.py
--rw-rw-rw-   0        0        0      582 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/full.py
--rw-rw-rw-   0        0        0     4011 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/track.py
--rw-rw-rw-   0        0        0     1808 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/user.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.297475 tekore-4.6.0/src/tekore/_sender/
--rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/base.py
--rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/client.py
--rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/concrete.py
--rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/error.py
--rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/extending.py
--rw-rw-rw-   0        0        0     4202 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/model.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.248467 tekore-4.6.0/src/tekore.egg-info/
--rw-rw-rw-   0        0        0     5362 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4979 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.301476 tekore-4.6.0/tests/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/_util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.303977 tekore-4.6.0/tests/auth/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/auth/__init__.py
--rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/expiring.py
--rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/refreshing.py
--rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/scope.py
--rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/util.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.315979 tekore-4.6.0/tests/client/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.0/tests/client/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/_resources.py
--rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/album.py
--rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/artist.py
--rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-4.6.0/tests/client/audiobook.py
--rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/base.py
--rw-rw-rw-   0        0        0     3444 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/browse.py
--rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-4.6.0/tests/client/chapter.py
--rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/episode.py
--rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/follow.py
--rw-rw-rw-   0        0        0    13417 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/full.py
--rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/library.py
--rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-4.6.0/tests/client/markets.py
--rw-rw-rw-   0        0        0     3652 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/paging.py
--rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/client/personalisation.py
--rw-rw-rw-   0        0        0     6147 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/player.py
--rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/playlist.py
--rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/search.py
--rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/show.py
--rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/track.py
--rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-4.6.0/tests/client/user.py
--rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/config.py
--rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/conftest.py
--rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/convert.py
--rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/error.py
--rw-rw-rw-   0        0        0     6902 2023-04-12 17:33:26.000000 tekore-4.6.0/tests/model.py
-drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.318479 tekore-4.6.0/tests/sender/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/sender/__init__.py
--rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/base.py
--rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/caching.py
--rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/client.py
--rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/retrying.py
--rw-rw-rw-   0        0        0     2404 2023-04-12 18:04:45.000000 tekore-4.6.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.886470 tekore-4.6.1/
+-rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-4.6.1/LICENSE
+-rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-4.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5362 2023-05-25 06:12:13.885970 tekore-4.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4184 2023-01-05 23:44:39.000000 tekore-4.6.1/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.799455 tekore-4.6.1/docs/
+-rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.806455 tekore-4.6.1/docs/src/
+-rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/404.rst
+-rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/advanced_usage.rst
+-rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/auth_guide.rst
+-rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-4.6.1/docs/src/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.809956 tekore-4.6.1/docs/src/examples/
+-rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-4.6.1/docs/src/examples/artist_follower.rst
+-rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-4.6.1/docs/src/examples/async_server.rst
+-rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-4.6.1/docs/src/examples/auth_server.rst
+-rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-4.6.1/docs/src/examples/creating_scripts.rst
+-rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-4.6.1/docs/src/examples/discord_bot.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.814957 tekore-4.6.1/docs/src/examples/scripts/
+-rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/albums_top_artist.rst
+-rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/analyse_from_playlist.rst
+-rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/follow_by_search.rst
+-rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/follow_category_playlist.rst
+-rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/play_saved_album.rst
+-rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/recommended_playlist.rst
+-rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/related_artists_top_artist.rst
+-rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-4.6.1/docs/src/examples/scripts/scrape_playlists.rst
+-rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-4.6.1/docs/src/examples/scripts/tracks_new_release.rst
+-rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/examples/scripts.rst
+-rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/examples.rst
+-rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-4.6.1/docs/src/getting_started.rst
+-rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-4.6.1/docs/src/index.rst
+-rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-4.6.1/docs/src/logo.png
+-rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-4.6.1/docs/src/logo_small.png
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.818957 tekore-4.6.1/docs/src/reference/
+-rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-4.6.1/docs/src/reference/auth.rst
+-rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/client.rst
+-rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-4.6.1/docs/src/reference/config.rst
+-rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-4.6.1/docs/src/reference/conversions.rst
+-rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/errors.rst
+-rw-rw-rw-   0        0        0     7784 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference/models.rst
+-rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-4.6.1/docs/src/reference/senders.rst
+-rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-4.6.1/docs/src/reference.rst
+-rw-rw-rw-   0        0        0    19851 2023-05-25 05:58:59.000000 tekore-4.6.1/docs/src/release_notes.rst
+-rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-4.6.1/docs/src/resources.rst
+-rw-rw-rw-   0        0        0     2069 2023-04-12 17:36:57.000000 tekore-4.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-4.6.1/readme_pypi.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.821458 tekore-4.6.1/requirements/
+-rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/build
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/checks
+-rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/dev
+-rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/docs
+-rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-4.6.1/requirements/tests
+-rw-rw-rw-   0        0        0       42 2023-05-25 06:12:13.886470 tekore-4.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.792954 tekore-4.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.823958 tekore-4.6.1/src/tekore/
+-rw-rw-rw-   0        0        0     2610 2023-05-25 05:58:59.000000 tekore-4.6.1/src/tekore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.828959 tekore-4.6.1/src/tekore/_auth/
+-rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.831460 tekore-4.6.1/src/tekore/_auth/expiring/
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/client.py
+-rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/decor.py
+-rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/expiring/token.py
+-rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/refreshing.py
+-rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/scope.py
+-rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_auth/util.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.834461 tekore-4.6.1/src/tekore/_client/
+-rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.841962 tekore-4.6.1/src/tekore/_client/api/
+-rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/album.py
+-rw-rw-rw-   0        0        0     3186 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/artist.py
+-rw-rw-rw-   0        0        0     2866 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/audiobook.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.842962 tekore-4.6.1/src/tekore/_client/api/browse/
+-rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/browse/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/browse/validate.py
+-rw-rw-rw-   0        0        0     1761 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/chapter.py
+-rw-rw-rw-   0        0        0     1762 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/episode.py
+-rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/follow.py
+-rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/library.py
+-rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/markets.py
+-rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/personalisation.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.844462 tekore-4.6.1/src/tekore/_client/api/player/
+-rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/modify.py
+-rw-rw-rw-   0        0        0     4091 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/player/view.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.846463 tekore-4.6.1/src/tekore/_client/api/playlist/
+-rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/__init__.py
+-rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/items.py
+-rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/modify.py
+-rw-rw-rw-   0        0        0     7617 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/playlist/view.py
+-rw-rw-rw-   0        0        0     3578 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/search.py
+-rw-rw-rw-   0        0        0     2985 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/show.py
+-rw-rw-rw-   0        0        0     2469 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/track.py
+-rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/api/user.py
+-rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/base.py
+-rw-rw-rw-   0        0        0     4194 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/chunked.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.847463 tekore-4.6.1/src/tekore/_client/decor/
+-rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/decor/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/decor/handle.py
+-rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/full.py
+-rw-rw-rw-   0        0        0     4299 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/paging.py
+-rw-rw-rw-   0        0        0     1316 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_client/process.py
+-rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_config.py
+-rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_convert.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.857465 tekore-4.6.1/src/tekore/_model/
+-rw-rw-rw-   0        0        0     2394 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.858965 tekore-4.6.1/src/tekore/_model/album/
+-rw-rw-rw-   0        0        0     1442 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/album/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/album/base.py
+-rw-rw-rw-   0        0        0     1720 2023-05-25 05:45:42.000000 tekore-4.6.1/src/tekore/_model/album/full.py
+-rw-rw-rw-   0        0        0     1369 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/artist.py
+-rw-rw-rw-   0        0        0     2336 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audio_analysis.py
+-rw-rw-rw-   0        0        0      518 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audio_features.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.860465 tekore-4.6.1/src/tekore/_model/audiobook/
+-rw-rw-rw-   0        0        0      607 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/base.py
+-rw-rw-rw-   0        0        0      468 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/audiobook/full.py
+-rw-rw-rw-   0        0        0      335 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/base.py
+-rw-rw-rw-   0        0        0      679 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/category.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.861966 tekore-4.6.1/src/tekore/_model/chapter/
+-rw-rw-rw-   0        0        0      860 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_model/chapter/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/chapter/base.py
+-rw-rw-rw-   0        0        0      627 2023-03-26 09:38:45.000000 tekore-4.6.1/src/tekore/_model/chapter/full.py
+-rw-rw-rw-   0        0        0      522 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/context.py
+-rw-rw-rw-   0        0        0     3070 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/currently_playing.py
+-rw-rw-rw-   0        0        0      845 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/device.py
+-rw-rw-rw-   0        0        0     2563 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/episode.py
+-rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/error.py
+-rw-rw-rw-   0        0        0     1362 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/local.py
+-rw-rw-rw-   0        0        0     1110 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/member.py
+-rw-rw-rw-   0        0        0      834 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/paging.py
+-rw-rw-rw-   0        0        0     1291 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/play_history.py
+-rw-rw-rw-   0        0        0     3789 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/playlist.py
+-rw-rw-rw-   0        0        0     1259 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/recommendations.py
+-rw-rw-rw-   0        0        0     7555 2023-04-12 17:42:29.000000 tekore-4.6.1/src/tekore/_model/serialise.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.862966 tekore-4.6.1/src/tekore/_model/show/
+-rw-rw-rw-   0        0        0     1176 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/base.py
+-rw-rw-rw-   0        0        0      582 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/show/full.py
+-rw-rw-rw-   0        0        0     4011 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/track.py
+-rw-rw-rw-   0        0        0     1808 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_model/user.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.866466 tekore-4.6.1/src/tekore/_sender/
+-rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/base.py
+-rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/client.py
+-rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/concrete.py
+-rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/error.py
+-rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/_sender/extending.py
+-rw-rw-rw-   0        0        0     4202 2023-01-05 23:44:39.000000 tekore-4.6.1/src/tekore/model.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.826959 tekore-4.6.1/src/tekore.egg-info/
+-rw-rw-rw-   0        0        0     5362 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4979 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 06:12:13.000000 tekore-4.6.1/src/tekore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.869467 tekore-4.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/_util.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.871967 tekore-4.6.1/tests/auth/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/auth/__init__.py
+-rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/expiring.py
+-rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/refreshing.py
+-rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/scope.py
+-rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/auth/util.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.882969 tekore-4.6.1/tests/client/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.1/tests/client/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-05-25 05:51:13.000000 tekore-4.6.1/tests/client/_resources.py
+-rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/album.py
+-rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/artist.py
+-rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-4.6.1/tests/client/audiobook.py
+-rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/base.py
+-rw-rw-rw-   0        0        0     3444 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/browse.py
+-rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-4.6.1/tests/client/chapter.py
+-rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/episode.py
+-rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/follow.py
+-rw-rw-rw-   0        0        0    13417 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/full.py
+-rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/library.py
+-rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-4.6.1/tests/client/markets.py
+-rw-rw-rw-   0        0        0     3652 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/paging.py
+-rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/client/personalisation.py
+-rw-rw-rw-   0        0        0     6147 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/player.py
+-rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/playlist.py
+-rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/search.py
+-rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/show.py
+-rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/client/track.py
+-rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-4.6.1/tests/client/user.py
+-rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/config.py
+-rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/convert.py
+-rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/error.py
+-rw-rw-rw-   0        0        0     6902 2023-04-12 17:33:26.000000 tekore-4.6.1/tests/model.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:12:13.885470 tekore-4.6.1/tests/sender/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.1/tests/sender/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/base.py
+-rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/caching.py
+-rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/client.py
+-rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-4.6.1/tests/sender/retrying.py
+-rw-rw-rw-   0        0        0     2404 2023-04-12 18:04:45.000000 tekore-4.6.1/tox.ini
```

### Comparing `tekore-4.6.0/LICENSE` & `tekore-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/PKG-INFO` & `tekore-4.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 4.6.0
+Version: 4.6.1
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
```

### Comparing `tekore-4.6.0/contributing.rst` & `tekore-4.6.1/contributing.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/advanced_usage.rst` & `tekore-4.6.1/docs/src/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/auth_guide.rst` & `tekore-4.6.1/docs/src/auth_guide.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/conf.py` & `tekore-4.6.1/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/artist_follower.rst` & `tekore-4.6.1/docs/src/examples/artist_follower.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/async_server.rst` & `tekore-4.6.1/docs/src/examples/async_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/auth_server.rst` & `tekore-4.6.1/docs/src/examples/auth_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/creating_scripts.rst` & `tekore-4.6.1/docs/src/examples/creating_scripts.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/discord_bot.rst` & `tekore-4.6.1/docs/src/examples/discord_bot.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/albums_top_artist.rst` & `tekore-4.6.1/docs/src/examples/scripts/albums_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/analyse_from_playlist.rst` & `tekore-4.6.1/docs/src/examples/scripts/analyse_from_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/follow_by_search.rst` & `tekore-4.6.1/docs/src/examples/scripts/follow_by_search.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/follow_category_playlist.rst` & `tekore-4.6.1/docs/src/examples/scripts/follow_category_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/play_saved_album.rst` & `tekore-4.6.1/docs/src/examples/scripts/play_saved_album.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/recommended_playlist.rst` & `tekore-4.6.1/docs/src/examples/scripts/recommended_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/related_artists_top_artist.rst` & `tekore-4.6.1/docs/src/examples/scripts/related_artists_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/scrape_playlists.rst` & `tekore-4.6.1/docs/src/examples/scripts/scrape_playlists.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/examples/scripts/tracks_new_release.rst` & `tekore-4.6.1/docs/src/examples/scripts/tracks_new_release.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/getting_started.rst` & `tekore-4.6.1/docs/src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/index.rst` & `tekore-4.6.1/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/logo.png` & `tekore-4.6.1/docs/src/logo.png`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/logo_small.png` & `tekore-4.6.1/docs/src/logo_small.png`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/auth.rst` & `tekore-4.6.1/docs/src/reference/auth.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/client.rst` & `tekore-4.6.1/docs/src/reference/client.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/config.rst` & `tekore-4.6.1/docs/src/reference/config.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/conversions.rst` & `tekore-4.6.1/docs/src/reference/conversions.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/errors.rst` & `tekore-4.6.1/docs/src/reference/errors.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/models.rst` & `tekore-4.6.1/docs/src/reference/models.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference/senders.rst` & `tekore-4.6.1/docs/src/reference/senders.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/reference.rst` & `tekore-4.6.1/docs/src/reference.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/docs/src/release_notes.rst` & `tekore-4.6.1/docs/src/release_notes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. _release-notes:
 .. currentmodule:: tekore
 
 Release notes
 =============
+4.6.1 (2023-05-25)
+------------------
+Fixed
+*****
+- :class:`FullAlbum <model.FullAlbum>` - remove "album_group" attribute
+  introduced in version 4.6.0 (:issue:`291`)
+
 4.6.0 (2023-04-12)
 ------------------
 Added
 *****
 - Make enumerations case insensitive (:issue:`285`)
 - Support HTTPX 0.24 (:issue:`289`)
```

### Comparing `tekore-4.6.0/docs/src/resources.rst` & `tekore-4.6.1/docs/src/resources.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/pyproject.toml` & `tekore-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/readme_pypi.rst` & `tekore-4.6.1/readme_pypi.rst`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/__init__.py` & `tekore-4.6.1/src/tekore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ServerError,
     ServiceUnavailable,
     SyncSender,
     TooManyRequests,
     Unauthorised,
 )
 
-__version__ = "4.6.0"
+__version__ = "4.6.1"
 
 # Change the module of classes to hide module structure
 # and fix Sphinx base class links
 _classes = [
     Spotify,
     Credentials,
     Token,
```

### Comparing `tekore-4.6.0/src/tekore/_auth/expiring/client.py` & `tekore-4.6.1/src/tekore/_auth/expiring/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_auth/expiring/decor.py` & `tekore-4.6.1/src/tekore/_auth/expiring/decor.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_auth/expiring/token.py` & `tekore-4.6.1/src/tekore/_auth/expiring/token.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_auth/refreshing.py` & `tekore-4.6.1/src/tekore/_auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_auth/scope.py` & `tekore-4.6.1/src/tekore/_auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_auth/util.py` & `tekore-4.6.1/src/tekore/_auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/__init__.py` & `tekore-4.6.1/src/tekore/_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/album.py` & `tekore-4.6.1/src/tekore/_client/api/album.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/artist.py` & `tekore-4.6.1/src/tekore/_client/api/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/audiobook.py` & `tekore-4.6.1/src/tekore/_client/api/audiobook.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/browse/__init__.py` & `tekore-4.6.1/src/tekore/_client/api/browse/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/browse/validate.py` & `tekore-4.6.1/src/tekore/_client/api/browse/validate.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/chapter.py` & `tekore-4.6.1/src/tekore/_client/api/chapter.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/episode.py` & `tekore-4.6.1/src/tekore/_client/api/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/follow.py` & `tekore-4.6.1/src/tekore/_client/api/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/library.py` & `tekore-4.6.1/src/tekore/_client/api/library.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/personalisation.py` & `tekore-4.6.1/src/tekore/_client/api/personalisation.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/player/modify.py` & `tekore-4.6.1/src/tekore/_client/api/player/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/player/view.py` & `tekore-4.6.1/src/tekore/_client/api/player/view.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/playlist/items.py` & `tekore-4.6.1/src/tekore/_client/api/playlist/items.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/playlist/modify.py` & `tekore-4.6.1/src/tekore/_client/api/playlist/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/playlist/view.py` & `tekore-4.6.1/src/tekore/_client/api/playlist/view.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/search.py` & `tekore-4.6.1/src/tekore/_client/api/search.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/show.py` & `tekore-4.6.1/src/tekore/_client/api/show.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/track.py` & `tekore-4.6.1/src/tekore/_client/api/track.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/api/user.py` & `tekore-4.6.1/src/tekore/_client/api/user.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/base.py` & `tekore-4.6.1/src/tekore/_client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/chunked.py` & `tekore-4.6.1/src/tekore/_client/chunked.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/decor/__init__.py` & `tekore-4.6.1/src/tekore/_client/decor/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/decor/handle.py` & `tekore-4.6.1/src/tekore/_client/decor/handle.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/full.py` & `tekore-4.6.1/src/tekore/_client/full.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/paging.py` & `tekore-4.6.1/src/tekore/_client/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_client/process.py` & `tekore-4.6.1/src/tekore/_client/process.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_config.py` & `tekore-4.6.1/src/tekore/_config.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_convert.py` & `tekore-4.6.1/src/tekore/_convert.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/__init__.py` & `tekore-4.6.1/src/tekore/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/album/__init__.py` & `tekore-4.6.1/src/tekore/_model/album/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/album/base.py` & `tekore-4.6.1/src/tekore/_model/album/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/album/full.py` & `tekore-4.6.1/src/tekore/_model/album/full.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,16 @@
     """
     Complete album object.
 
     :attr:`available_markets` is available when market is not specified.
 
     The presence of :attr:`is_playable` is undocumented
     and it appears to only be ``True`` when it is present.
-    :attr:`album_group` is undocumented too.
     """
 
-    album_group: str
     copyrights: List[Copyright]
     external_ids: dict
     genres: List[str]
     label: str
     popularity: int
     tracks: SimpleTrackPaging
     available_markets: Optional[List[str]] = None
```

### Comparing `tekore-4.6.0/src/tekore/_model/artist.py` & `tekore-4.6.1/src/tekore/_model/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/audio_analysis.py` & `tekore-4.6.1/src/tekore/_model/audio_analysis.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/audio_features.py` & `tekore-4.6.1/src/tekore/_model/audio_features.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/audiobook/__init__.py` & `tekore-4.6.1/src/tekore/_model/audiobook/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/audiobook/base.py` & `tekore-4.6.1/src/tekore/_model/audiobook/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/category.py` & `tekore-4.6.1/src/tekore/_model/category.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/chapter/__init__.py` & `tekore-4.6.1/src/tekore/_model/chapter/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/chapter/base.py` & `tekore-4.6.1/src/tekore/_model/chapter/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/chapter/full.py` & `tekore-4.6.1/src/tekore/_model/chapter/full.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/context.py` & `tekore-4.6.1/src/tekore/_model/context.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/currently_playing.py` & `tekore-4.6.1/src/tekore/_model/currently_playing.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/device.py` & `tekore-4.6.1/src/tekore/_model/device.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/episode.py` & `tekore-4.6.1/src/tekore/_model/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/error.py` & `tekore-4.6.1/src/tekore/_model/error.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/local.py` & `tekore-4.6.1/src/tekore/_model/local.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/member.py` & `tekore-4.6.1/src/tekore/_model/member.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/paging.py` & `tekore-4.6.1/src/tekore/_model/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/play_history.py` & `tekore-4.6.1/src/tekore/_model/play_history.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/playlist.py` & `tekore-4.6.1/src/tekore/_model/playlist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/recommendations.py` & `tekore-4.6.1/src/tekore/_model/recommendations.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/serialise.py` & `tekore-4.6.1/src/tekore/_model/serialise.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/show/__init__.py` & `tekore-4.6.1/src/tekore/_model/show/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/show/base.py` & `tekore-4.6.1/src/tekore/_model/show/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/show/full.py` & `tekore-4.6.1/src/tekore/_model/show/full.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/track.py` & `tekore-4.6.1/src/tekore/_model/track.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_model/user.py` & `tekore-4.6.1/src/tekore/_model/user.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_sender/base.py` & `tekore-4.6.1/src/tekore/_sender/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_sender/client.py` & `tekore-4.6.1/src/tekore/_sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_sender/concrete.py` & `tekore-4.6.1/src/tekore/_sender/concrete.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_sender/error.py` & `tekore-4.6.1/src/tekore/_sender/error.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/_sender/extending.py` & `tekore-4.6.1/src/tekore/_sender/extending.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore/model.py` & `tekore-4.6.1/src/tekore/model.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/src/tekore.egg-info/PKG-INFO` & `tekore-4.6.1/src/tekore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 4.6.0
+Version: 4.6.1
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
```

### Comparing `tekore-4.6.0/src/tekore.egg-info/SOURCES.txt` & `tekore-4.6.1/src/tekore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/auth/expiring.py` & `tekore-4.6.1/tests/auth/expiring.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/auth/refreshing.py` & `tekore-4.6.1/tests/auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/auth/scope.py` & `tekore-4.6.1/tests/auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/auth/util.py` & `tekore-4.6.1/tests/auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/_resources.py` & `tekore-4.6.1/tests/client/_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 user_id = "spinninrecordsofficial"
 user_id_hash = "a#a"
 user_ids = [user_id, "samsmithworld"]
 
 show_id = "0Lsi13D8nWRkwbEkfNeItS"
 show_ids = [show_id, "7Arl2fVUFHCGyNZwM39bJO"]
-episode_id = "40KE0vkrH0WhirGTrF4n9O"
-episode_ids = [episode_id, "4cvdWMfkjYiLISibNcvDZe"]
+episode_id = "3YPKYYsqrWZUdZTzF6dZ3F"
+episode_ids = [episode_id, "3b0ZXFhLeMqopV3rHpWZ6V"]
 
 image = (
     "/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAIBAQIBAQICAgICAgICAwUDAwMDAwYEBAMFBwYHB"
     "wcGBwcICQsJCAgKCAcHCg0KCgsMDAwMBwkODw0MDgsMDAz/2wBDAQICAgMDAwYDAwYMCAcIDA"
     "wMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAz/wAARCAA"
     "QABADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgED"
     "AwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYG"
```

### Comparing `tekore-4.6.0/tests/client/album.py` & `tekore-4.6.1/tests/client/album.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/artist.py` & `tekore-4.6.1/tests/client/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/audiobook.py` & `tekore-4.6.1/tests/client/audiobook.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/base.py` & `tekore-4.6.1/tests/client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/browse.py` & `tekore-4.6.1/tests/client/browse.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/chapter.py` & `tekore-4.6.1/tests/client/chapter.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/episode.py` & `tekore-4.6.1/tests/client/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/follow.py` & `tekore-4.6.1/tests/client/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/full.py` & `tekore-4.6.1/tests/client/full.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/library.py` & `tekore-4.6.1/tests/client/library.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/paging.py` & `tekore-4.6.1/tests/client/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/player.py` & `tekore-4.6.1/tests/client/player.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/playlist.py` & `tekore-4.6.1/tests/client/playlist.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/search.py` & `tekore-4.6.1/tests/client/search.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/show.py` & `tekore-4.6.1/tests/client/show.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/client/track.py` & `tekore-4.6.1/tests/client/track.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/config.py` & `tekore-4.6.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/conftest.py` & `tekore-4.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/convert.py` & `tekore-4.6.1/tests/convert.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/model.py` & `tekore-4.6.1/tests/model.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/sender/caching.py` & `tekore-4.6.1/tests/sender/caching.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/sender/client.py` & `tekore-4.6.1/tests/sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tests/sender/retrying.py` & `tekore-4.6.1/tests/sender/retrying.py`

 * *Files identical despite different names*

### Comparing `tekore-4.6.0/tox.ini` & `tekore-4.6.1/tox.ini`

 * *Files identical despite different names*

