# Comparing `tmp/biliup-0.4.8.tar.gz` & `tmp/biliup-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biliup-0.4.8.tar", last modified: Sat Mar  4 14:09:03 2023, max compression
+gzip compressed data, was "biliup-0.4.9.tar", last modified: Mon Mar  6 03:46:59 2023, max compression
```

## Comparing `biliup-0.4.8.tar` & `biliup-0.4.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.481279 biliup-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-04 14:08:25.000000 biliup-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-04 14:09:03.481279 biliup-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-03-04 14:08:25.000000 biliup-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.469278 biliup-0.4.8/biliup/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.473279 biliup-0.4.8/biliup/common/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/Daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/configlog.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/common/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.473279 biliup-0.4.8/biliup/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/engine/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/engine/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/engine/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/engine/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.473279 biliup-0.4.8/biliup/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.473279 biliup-0.4.8/biliup/plugins/Danmaku/
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/douyu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/huya.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.477279 biliup-0.4.8/biliup/plugins/Danmaku/tars/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/EndpointF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/QueryF.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__TimeoutQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    25786 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__adapterproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__packet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__servantproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21129 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__tars.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__tup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/__util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.477279 biliup-0.4.8/biliup/plugins/Danmaku/tars/tars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/Danmaku/tars/tars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/acfun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/afreecaTV.py
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/bili_chromeup.py
--rw-r--r--   0 runner    (1001) docker     (123)    29219 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/bili_webup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/biliuprs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/douyin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/douyu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/egame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/missevan.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/noop_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/plugins/yy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.477279 biliup-0.4.8/biliup/web/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/web/aiohttp_basicauth_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-04 14:08:25.000000 biliup-0.4.8/biliup/web/http_basic_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.477279 biliup-0.4.8/biliup/web/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.477279 biliup-0.4.8/biliup/web/public/build/
--rw-r--r--   0 runner    (1001) docker     (123)    94423 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/build/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)   118921 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/build/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   537043 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/build/bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/global.css
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-04 14:08:56.000000 biliup-0.4.8/biliup/web/public/noface.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 14:09:03.469278 biliup-0.4.8/biliup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-04 14:09:03.000000 biliup-0.4.8/biliup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-04 14:08:25.000000 biliup-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 14:09:03.481279 biliup-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-04 14:08:25.000000 biliup-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-06 03:46:18.000000 biliup-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-06 03:46:59.246419 biliup-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-03-06 03:46:18.000000 biliup-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.238418 biliup-0.4.9/biliup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.238418 biliup-0.4.9/biliup/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/Daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/configlog.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/common/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.238418 biliup-0.4.9/biliup/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/engine/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/engine/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/engine/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/engine/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.242418 biliup-0.4.9/biliup/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.242418 biliup-0.4.9/biliup/plugins/Danmaku/
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/douyu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/huya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/biliup/plugins/Danmaku/tars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/EndpointF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/QueryF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__TimeoutQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25786 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__adapterproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__servantproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21129 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__tars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__tup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/__util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/biliup/plugins/Danmaku/tars/tars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/Danmaku/tars/tars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/acfun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/afreecaTV.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/bili_chromeup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29219 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/bili_webup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/biliuprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/douyin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/douyu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/egame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/missevan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/noop_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/plugins/yy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/biliup/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/web/aiohttp_basicauth_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-06 03:46:18.000000 biliup-0.4.9/biliup/web/http_basic_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/biliup/web/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.246419 biliup-0.4.9/biliup/web/public/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    94423 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/build/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)   118921 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/build/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   537043 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/build/bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/global.css
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-06 03:46:51.000000 biliup-0.4.9/biliup/web/public/noface.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 03:46:59.238418 biliup-0.4.9/biliup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 03:46:59.000000 biliup-0.4.9/biliup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-06 03:46:18.000000 biliup-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 03:46:59.246419 biliup-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-06 03:46:18.000000 biliup-0.4.9/setup.py
```

### Comparing `biliup-0.4.8/LICENSE` & `biliup-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/PKG-INFO` & `biliup-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biliup
-Version: 0.4.8
+Version: 0.4.9
 Summary: stream download and upload
 Author: ForgQi
 Project-URL: Homepage, https://github.com/ForgQi/bilibiliupload
 Keywords: bilibili douyu huya
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: selenium
```

### Comparing `biliup-0.4.8/README.md` & `biliup-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/__init__.py` & `biliup-0.4.9/biliup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import sys
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 LOG_CONF = {
     'version': 1,
     'formatters': {
         'verbose': {
             'format': "%(asctime)s %(filename)s[line:%(lineno)d](Pid:%(process)d "
                       "Tname:%(threadName)s) %(levelname)s %(message)s",
```

### Comparing `biliup-0.4.8/biliup/__main__.py` & `biliup-0.4.9/biliup/__main__.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/common/Daemon.py` & `biliup-0.4.9/biliup/common/Daemon.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/common/configlog.ini` & `biliup-0.4.9/biliup/common/configlog.ini`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/common/log.py` & `biliup-0.4.9/biliup/common/log.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/common/reload.py` & `biliup-0.4.9/biliup/common/reload.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/common/timer.py` & `biliup-0.4.9/biliup/common/timer.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/config.py` & `biliup-0.4.9/biliup/config.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/downloader.py` & `biliup-0.4.9/biliup/downloader.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/engine/decorators.py` & `biliup-0.4.9/biliup/engine/decorators.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/engine/download.py` & `biliup-0.4.9/biliup/engine/download.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/engine/event.py` & `biliup-0.4.9/biliup/engine/event.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/engine/upload.py` & `biliup-0.4.9/biliup/engine/upload.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/handler.py` & `biliup-0.4.9/biliup/handler.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/__init__.py` & `biliup-0.4.9/biliup/plugins/Danmaku/__init__.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/bilibili.py` & `biliup-0.4.9/biliup/plugins/Danmaku/bilibili.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/douyu.py` & `biliup-0.4.9/biliup/plugins/Danmaku/douyu.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/huya.py` & `biliup-0.4.9/biliup/plugins/Danmaku/huya.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/EndpointF.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/EndpointF.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/QueryF.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/QueryF.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__TimeoutQueue.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__TimeoutQueue.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__adapterproxy.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__adapterproxy.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__async.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__async.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__init__.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__init__.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__logger.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__logger.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__packet.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__packet.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__rpc.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__rpc.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__servantproxy.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__servantproxy.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__tars.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__tars.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__trans.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__trans.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__tup.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__tup.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/__util.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/__util.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/core.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/core.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/Danmaku/tars/exception.py` & `biliup-0.4.9/biliup/plugins/Danmaku/tars/exception.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/__init__.py` & `biliup-0.4.9/biliup/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/acfun.py` & `biliup-0.4.9/biliup/plugins/acfun.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/afreecaTV.py` & `biliup-0.4.9/biliup/plugins/afreecaTV.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/bili_chromeup.py` & `biliup-0.4.9/biliup/plugins/bili_chromeup.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/bili_webup.py` & `biliup-0.4.9/biliup/plugins/bili_webup.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/bilibili.py` & `biliup-0.4.9/biliup/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/biliuprs.py` & `biliup-0.4.9/biliup/plugins/biliuprs.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,17 @@
             tags = []
         self.lines = lines
         self.submit_api = submit_api
         self.threads = threads
         self.tid = tid
         self.tags = tags
         if "live_cover_path" in self.data:
-            self.cover_path = self.data["live_cover_path"] 
-        self.cover_path = cover_path #自定义封面的优先级比直播封面高
+            self.cover_path = self.data["live_cover_path"]
+        if cover_path:
+            self.cover_path = cover_path #自定义封面的优先级比直播封面高
         self.desc = description
         self.dynamic = dynamic
         self.copyright = copyright
         self.dtime = dtime
         self.user_cookie = user_cookie
 
     def upload(self, file_list):
@@ -43,19 +44,20 @@
         elif self.lines == 'cos':
             line = stream_gears.UploadLine.Cos
         elif self.lines == 'cos-internal':
             line = stream_gears.UploadLine.CosInternal
         tag = ','.join(self.tags)
         source = self.data["url"] if self.copyright == 2 else ""
         cover = self.cover_path if self.cover_path is not None else ""
+        filtered_list = [file for file in file_list if not file.endswith('.xml')]
         dtime = None
         if self.dtime:
             dtime = int(time.time() + self.dtime)
         stream_gears.upload(
-            file_list,
+            filtered_list,
             self.user_cookie,
             self.data["format_title"][:80],
             self.tid,
             tag,
             self.copyright,
             source,
             self.desc,
```

### Comparing `biliup-0.4.8/biliup/plugins/cc.py` & `biliup-0.4.9/biliup/plugins/cc.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/douyin.py` & `biliup-0.4.9/biliup/plugins/douyin.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/douyu.py` & `biliup-0.4.9/biliup/plugins/douyu.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/egame.py` & `biliup-0.4.9/biliup/plugins/egame.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/general.py` & `biliup-0.4.9/biliup/plugins/general.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/huya.py` & `biliup-0.4.9/biliup/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/missevan.py` & `biliup-0.4.9/biliup/plugins/missevan.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/twitch.py` & `biliup-0.4.9/biliup/plugins/twitch.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/youtube.py` & `biliup-0.4.9/biliup/plugins/youtube.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/plugins/yy.py` & `biliup-0.4.9/biliup/plugins/yy.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/uploader.py` & `biliup-0.4.9/biliup/uploader.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/__init__.py` & `biliup-0.4.9/biliup/web/__init__.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/aiohttp_basicauth_middleware.py` & `biliup-0.4.9/biliup/web/aiohttp_basicauth_middleware.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/http_basic_auth.py` & `biliup-0.4.9/biliup/web/http_basic_auth.py`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/public/build/bundle.css` & `biliup-0.4.9/biliup/web/public/build/bundle.css`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/public/build/bundle.js` & `biliup-0.4.9/biliup/web/public/build/bundle.js`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/public/build/bundle.js.map` & `biliup-0.4.9/biliup/web/public/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/public/config.toml` & `biliup-0.4.9/biliup/web/public/config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 #------录制与下载------#
 ### 选择全局默认的下载插件，默认为stream-gears。可选：
 ### 1.streamlink(streamlink配合ffmpeg混合下载模式，适合用于下载hls_fmp4与hls_ts流，因为streamlink支持多线程拉取）。
 ### 使用该模式下载flv流时，将会仅使用ffmpeg。请手动安装streamlink以及ffmpeg。
 ### 2.ffmpeg（纯ffmpeg下载），请手动安装ffmpeg。
 ### 3.stream-gears
-#downloader = ffmpeg
+#downloader = "ffmpeg"
 # 录像单文件大小限制，单位Byte，超过此大小分段下载
 file_size = 2621440000
 # 录像单文件时间限制，格式'00:00:00'（时分秒），超过此大小分段下载，如需使用大小分段请注释此字段
-#segment_time = '00:50:00'
+#segment_time = "00:50:00"
 # 小于此大小的视频文件将会被过滤删除，单位MB
 filtering_threshold = 20
 
 # 自定义录播文件名模板, 支持变量 {streamer}:你在配置里设置的直播间名 %Y-%m-%d %H_%M_%S:创建文件的时间, {title}:当场直播间标题
 # 如果上传文件，文件名必须包含设定的模板名。其次，如果没有定义时间，文件分片可能会互相覆盖，所以推荐设置时间来避免分段文件名重复。
-#filename_prefix = '{streamer}%Y-%m-%d %H_%M_%S{title}'
+#filename_prefix = "{streamer}%Y-%m-%d %H_%M_%S{title}"
 
 #------上传------#
 ### b站提交接口，默认自动选择，可选web，client
 #submit_api = "client"
 # 选择全局默认上传插件，Noop为不上传，但会执行后处理,可选bili_web，biliup-rs
 #uploader = "Noop"
 # b站上传线路选择，默认为自动模式，目前可手动切换为bda2, kodo, ws, qn, cos, cos-internal(支持腾讯云内网免流+提速)
@@ -64,36 +64,36 @@
 ### 录制BILIBILI弹幕，目前暂时不支持视频按时长分段下的弹幕文件自动分段，默认关闭
 # bilibili_danmaku = false
 ### 哔哩哔哩直播流协议.可选 stream（flv流）,hls_ts(ts流）与hls_fmp4（fmp4流），默认为stream
 ### 仅国内IP可以解析到fmp4流。海外IP只能获取到flv流（ov05与ov07）和ts流（ov105）
 ### 由于fmp4出现需要一定时间，或者某些小主播（大部分只有原画选项的主播）无fmp4流。
 ### 目前的策略是，如果开播时间小于45s，将会反复尝试获取fmp4流，如果没获取到就回退到flv流。
 ### 由于ffmpeg只能单线程下载，并且stream-gears录制有问题，所以目前fmp4流只能使用streamlink+ffmpeg混合模式。
-#bili_protocol = stream
+#bili_protocol = "stream"
 ### 哔哩哔哩直播优选CDN，默认无
-#bili_perfCDN = cn-gotcha01
+#bili_perfCDN = "cn-gotcha01"
 ### 哔哩哔哩直播强制原画（仅限HLS流的 cn-gotcha01 CDN），默认为关闭
 #bili_forceScoure = false
 ### 自定义哔哩哔哩直播api，默认无
-#bili_liveapi = 'https://api.live.bilibili.com'
+#bili_liveapi = "https://api.live.bilibili.com"
 ### CDN自动Fallback开关，默认为开启
 #bili_cdn_fallback = true
 ### 强制替换ov-gotcha05的下载地址为指定的自选IP
 #bili_force_ov05 = true
-#bili_force_ov05_ip = '163.171.197.234'
+#bili_force_ov05_ip = "163.171.197.234"
 ### 强制替换cn-gotcha01（叔叔自建，理论上最稳定）为指定的自选域名组（可多个域名，请用逗号分隔）
 ### 完整CDN列表请参考 https://rec.danmuji.org/dev/bilibili-cdn/ 中"B站视频云"的部分
 ### 此功能需要设置bili_perfCDN为cn-gotcha01，并且设置bili_protocol为hls。
 ### 此功能目前会和stream-gears冲突导致很多分段，请考虑使用ffmpeg录制
 ### 如果海外机器需要使用此功能，需要在bili_liveapi中指定国内的反代API来获取cn-gotcha01的节点信息。
 ### 海外机的玩法：配合一个国内的机器（例如便宜的腾讯云，阿里云等等）自建反代api.live.bilibili.com
 ### 如果海外机到联通或者移动网络线路还不错，就可以参考https://rec.danmuji.org/dev/bilibili-cdn/ 选取一些联通或者移动的节点并填入下面
 ### 每次会随机返回填入的其中一个线路，并且会自动判断所填入的节点是否可用
 #bili_force_cn01 = true
-#bili_force_cn01_domains = 'cn-gdst-cm-01-15.bilivideo.com,cn-gdst-cm-01-06.bilivideo.com,cn-fjqz-cm-01-06.bilivideo.com,cn-jssz-cm-01-02.bilivideo.com,cn-jxnc-cm-01-02.bilivideo.com'
+#bili_force_cn01_domains = "cn-gdst-cm-01-15.bilivideo.com,cn-gdst-cm-01-06.bilivideo.com,cn-fjqz-cm-01-06.bilivideo.com,cn-jssz-cm-01-02.bilivideo.com,cn-jxnc-cm-01-02.bilivideo.com"
 
 #------YouTube------#
 ### 设置偏好的YouTube下载封装格式
 ### 请务必记得安装ffmpeg
 ### 支持同时添加多个编码，自动优选指定编码格式里最好的画质/音质版本。
 ### 视频：其中avc编码最高可以下载到1080p的内容，vp9最高可以下载到4k以及很少部分8k内容，av01画质不是所有视频都有，但是大部分8k视频的8k画质只有av01编码。
 ### 音频：其中opus编码最高48KHz采样，mp4a（AAC）最高44.1KHz采样，理论上来说opus音质会更好一些。
@@ -127,15 +127,15 @@
 # 支持strftime, {title}, {streamer}, {url}占位符。
 description = """
 视频简介: {title} %Y-%m-%d %H:%M:%S
 {streamers}主播直播间地址：{url}
 ---
 Powered By biliup - Github: https://github.com/ForgQi/biliup"""
 dynamic = "#空间动态#"
-# dtime = 14_400 # 设置延时发布时间，距离提交大于2小时，格式为时间戳
+# dtime = 14400 # 设置延时发布时间，距离提交大于2小时，格式为时间戳
 uploader = "biliup-rs"  # 覆盖全局默认上传插件，Noop为不上传，但会执行后处理
 #filename_prefix = '{streamer}%Y-%m-%d %H_%M_%S{title}'  # 覆盖全局自定义录播文件命名规则
 user_cookie = "cookies.json" # 使用指定的账号上传
 #use_live_cover = true # 获取BILIBILI直播间封面并作为投稿封面。此封面优先级低于单个主播指定的自定义封面。
 tags = [ "biliup", "视频标签" ]
 # 上传完成后，将按自定义顺序执行自定义操作
 #postprocessor = [
@@ -148,15 +148,15 @@
 
 
 ### 在填了cookies的情况下优先使用cookies上传，如需使用用户名密码上传请注释掉cookies
 [user]
 #------哔哩哔哩------#
 #------哔哩哔哩获取直播流用COOKIE------#
 ### 参照https://github.com/BililiveRecorder/BililiveRecorder/issues/263
-#bili_cookie = ''
+#bili_cookie = ""
 ### 重要！！！
 ###是否将cookie传入第三方API。将Cookie传入未知的第三方API有几率泄露帐号登录信息。
 ###在开启了自定义Cookie（bili_cookie）又同时设置了第三方API（bili_liveapi）的情况下，如果打开了允许第三方API使用Cookie，那么就使用第三方API，如果没有允许（默认），那么设置的第三方API就不生效
 #customAPI_use_cookie = false
 
 #------抖音------#
 # 如需要录制抖音请在此填入cookie需要__ac_nonce与__ac_signature的值
```

### Comparing `biliup-0.4.8/biliup/web/public/config.yaml` & `biliup-0.4.9/biliup/web/public/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 check_sourcecode: 15
 
 #########各平台分设置#########
 
 #------斗鱼------#
 ### 如遇到斗鱼录制卡顿可以尝试切换线路，tct-h5（备用线路5），ali-h5（备用线路6），akm-h5（主线路1）
 #douyucdn: tct-h5
-# 录制斗鱼弹幕，只有使用FFMPEG作为下载器才支持，默认关闭
+# 录制斗鱼弹幕，目前暂时不支持视频按时长分段下的弹幕文件自动分段，只有使用ffmpeg（包括streamlink混合模式）作为下载器才支持，默认关闭默认关闭
 #douyu_danmaku: false
 
 #------虎牙------#
 ### 如遇到虎牙录制卡顿可以尝试切换线路，AL, HW, TX, WS
 #huyacdn: AL
-### 录制虎牙弹幕，只有使用FFMPEG作为下载器才支持，默认关闭
+### 录制虎牙弹幕，目前暂时不支持视频按时长分段下的弹幕文件自动分段，只有使用ffmpeg（包括streamlink混合模式）作为下载器才支持，默认关闭默认关闭
 #huya_danmaku: false
 
 #------哔哩哔哩------#
 ### 获取BILIBILI直播间封面并作为投稿封面。此封面优先级低于单个主播指定的自定义封面。（直播封面将会保存于cover文件夹下，请自行定期删除）
 #use_live_cover: true
-### 录制BILIBILI弹幕，目前暂时不支持视频按时长分段下的弹幕文件自动分段，默认关闭
+### 录制BILIBILI弹幕，目前暂时不支持视频按时长分段下的弹幕文件自动分段，只有使用ffmpeg（包括streamlink混合模式）作为下载器才支持，默认关闭默认关闭
 # bilibili_danmaku: false
 ### 哔哩哔哩直播流协议.可选 stream（flv流）,hls_ts(ts流）与hls_fmp4（fmp4流），默认为stream
 ### 仅国内IP可以解析到fmp4流。海外IP只能获取到flv流（ov05与ov07）和ts流（ov105）
 ### 由于fmp4出现需要一定时间，或者某些小主播（大部分只有原画选项的主播）无fmp4流。
 ### 目前的策略是，如果开播时间小于45s，将会反复尝试获取fmp4流，如果没获取到就回退到flv流。
 ### 由于ffmpeg只能单线程下载，并且stream-gears录制有问题，所以目前fmp4流只能使用streamlink+ffmpeg混合模式。
 #bili_protocol: stream
@@ -118,19 +118,19 @@
             - https://www.panda.tv/1160340
         title: "{title}第一视角%Y-%m-%d{streamer}{url}" ### 自定义标题的时间格式, {title}代表当场直播间标题 {streamer}代表在本config里面设置的主播名称 {url}代表设置的该主播的第一条直播间链接
         tid: 171 ### 投稿分区码,171为电子竞技分区
         copyright: 2 ### 1为自制
         cover_path: /cover/up.jpg ###封面
         description: |- ### 支持strftime, {title}, {streamer}, {url}占位符。注：此处请注意缩进，确保所有文字的缩进都与"视频简介"相同或者更多。
          视频简介: {title} %Y-%m-%d %H:%M:%S
-         {streamers}主播直播间地址：{url}
+         {streamer}主播直播间地址：{url}
          ---
          Powered By biliup - Github: https://github.com/ForgQi/biliup
         dynamic: '#空间动态#'
-        dtime: 14400 ### 设置延时发布时间，距离提交大于2小时，格式为时间戳
+        dtime: 14_400 ### 设置延时发布时间，距离提交大于2小时，格式为时间戳
         uploader: biliup-rs ### 覆盖全局默认上传插件，Noop为不上传，但会执行后处理
         #filename_prefix: '{streamer}%Y-%m-%d %H_%M_%S{title}'  ### 覆盖全局自定义录播文件命名规则
         user_cookie: cookies.json ### 使用指定的账号上传
         #use_live_cover: true ### 获取BILIBILI直播间封面并作为投稿封面。此封面优先级低于单个主播指定的自定义封面。
         preprocessor: ### 开始下载直播时，将按自定义顺序执行自定义操作 注：preprocessor仅支持shell指令
             #- run: sh ./run.sh
         postprocessor: ### 上传完成后，将按自定义顺序执行自定义操作
```

### Comparing `biliup-0.4.8/biliup/web/public/favicon.png` & `biliup-0.4.9/biliup/web/public/favicon.png`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup/web/public/noface.jpg` & `biliup-0.4.9/biliup/web/public/noface.jpg`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/biliup.egg-info/PKG-INFO` & `biliup-0.4.9/biliup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biliup
-Version: 0.4.8
+Version: 0.4.9
 Summary: stream download and upload
 Author: ForgQi
 Project-URL: Homepage, https://github.com/ForgQi/bilibiliupload
 Keywords: bilibili douyu huya
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: selenium
```

### Comparing `biliup-0.4.8/biliup.egg-info/SOURCES.txt` & `biliup-0.4.9/biliup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biliup-0.4.8/pyproject.toml` & `biliup-0.4.9/pyproject.toml`

 * *Files identical despite different names*

