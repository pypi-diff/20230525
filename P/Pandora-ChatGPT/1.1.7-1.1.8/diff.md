# Comparing `tmp/Pandora-ChatGPT-1.1.7.tar.gz` & `tmp/Pandora-ChatGPT-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-b2y1runx/Pandora-ChatGPT-1.1.7.tar", last modified: Thu May 25 11:15:31 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-lut41h6v/Pandora-ChatGPT-1.1.8.tar", last modified: Thu May 25 12:20:50 2023, max compression
```

## Comparing `Pandora-ChatGPT-1.1.7.tar` & `Pandora-ChatGPT-1.1.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:15:31.000000 Pandora-ChatGPT-1.1.7/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-25 11:15:14.000000 Pandora-ChatGPT-1.1.7/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:49.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:20:50.000000 Pandora-ChatGPT-1.1.8/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-25 12:20:35.000000 Pandora-ChatGPT-1.1.8/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-1.1.7/LICENSE` & `Pandora-ChatGPT-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/PKG-INFO` & `Pandora-ChatGPT-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.1.7
+Version: 1.1.8
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.7 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.8 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 1.1.7
+Version: 1.1.8
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.7 Summary: A command-
+Metadata-Version: 2.1 Name: Pandora-ChatGPT Version: 1.1.8 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/pengzhile/pandora Project-URL: Tracker, https://github.com/
 pengzhile/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Pandora-ChatGPT-1.1.7/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.1.8/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/README.md` & `Pandora-ChatGPT-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/setup.py` & `Pandora-ChatGPT-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/pengzhile/pandora',
     packages=find_packages('src'),
     package_dir={'pandora': 'src/pandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['pandora-cloud~=0.3.0'],
+        'cloud': ['pandora-cloud~=0.3.1'],
     },
     entry_points={
         'console_scripts': [
             'pandora = pandora.launcher:run',
             'pandora-cloud = pandora.cloud_launcher:run',
         ]
     },
```

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.1.8/src/pandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.1.8/src/pandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.1.8/src/pandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.1.8/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.1.8/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.1.8/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/launcher.py` & `Pandora-ChatGPT-1.1.8/src/pandora/launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.1.8/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.1.8/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.1.8/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.1.8/src/pandora/openai/api.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.1.8/src/pandora/openai/auth.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.1.8/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.1.8/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-1.1.7/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.1.8/src/pandora/turbo/chat.py`

 * *Files identical despite different names*

