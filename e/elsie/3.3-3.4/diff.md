# Comparing `tmp/elsie-3.3.tar.gz` & `tmp/elsie-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsie-3.3.tar", last modified: Sat Feb  5 18:20:58 2022, max compression
+gzip compressed data, was "elsie-3.4.tar", last modified: Thu May 25 12:07:41 2023, max compression
```

## Comparing `elsie-3.3.tar` & `elsie-3.4.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.675050 elsie-3.3/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      549 2022-02-05 18:20:58.675050 elsie-3.3/PKG-INFO
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1403 2021-01-21 13:04:37.000000 elsie-3.3/README.md
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.667050 elsie-3.3/elsie/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      698 2021-01-16 11:36:21.000000 elsie-3.3/elsie/__init__.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.667050 elsie-3.3/elsie/boxtree/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2020-12-28 22:01:17.000000 elsie-3.3/elsie/boxtree/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     4592 2021-01-21 13:04:37.000000 elsie-3.3/elsie/boxtree/box.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      610 2020-12-28 22:01:17.000000 elsie-3.3/elsie/boxtree/boxitem.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)    26993 2022-02-05 18:06:02.000000 elsie-3.3/elsie/boxtree/boxmixin.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     6799 2020-12-28 22:01:17.000000 elsie-3.3/elsie/boxtree/layout.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1719 2020-12-28 22:01:17.000000 elsie-3.3/elsie/boxtree/lazy.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3759 2020-12-28 22:01:17.000000 elsie-3.3/elsie/boxtree/value.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/ext/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      298 2021-01-05 10:30:07.000000 elsie-3.3/elsie/ext/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      538 2021-06-01 08:11:47.000000 elsie-3.3/elsie/ext/export.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3483 2021-01-21 13:04:37.000000 elsie-3.3/elsie/ext/latex.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     9493 2021-01-05 10:30:07.000000 elsie-3.3/elsie/ext/list.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     5716 2021-01-05 10:30:07.000000 elsie-3.3/elsie/ext/markdown.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      414 2021-06-01 08:11:47.000000 elsie-3.3/elsie/ext/todo.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/render/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2020-12-28 22:01:17.000000 elsie-3.3/elsie/render/__init__.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/render/backends/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      173 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1772 2021-03-03 14:21:25.000000 elsie-3.3/elsie/render/backends/backend.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/render/backends/cairo/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2818 2021-03-03 14:21:25.000000 elsie-3.3/elsie/render/backends/cairo/backend.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2645 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/draw.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     8012 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/rcontext.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1686 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/shapes.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3876 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/svg.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     6851 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/text.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      813 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/cairo/utils.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      931 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/rcontext.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/render/backends/svg/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2021-01-16 11:36:21.000000 elsie-3.3/elsie/render/backends/svg/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     4732 2021-03-03 14:21:25.000000 elsie-3.3/elsie/render/backends/svg/backend.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     5450 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/svg/draw.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      599 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/svg/query.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2905 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/backends/svg/rcontext.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1565 2021-01-16 11:36:21.000000 elsie-3.3/elsie/render/backends/svg/utils.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1009 2020-12-28 22:01:17.000000 elsie-3.3/elsie/render/image.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3198 2021-06-01 08:21:05.000000 elsie-3.3/elsie/render/inkscape.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3687 2021-01-21 13:04:37.000000 elsie-3.3/elsie/render/jupyter.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3407 2021-01-16 11:36:21.000000 elsie-3.3/elsie/render/ora.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1203 2020-12-28 22:01:17.000000 elsie-3.3/elsie/render/pdfmerge.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2732 2021-03-03 14:21:25.000000 elsie-3.3/elsie/render/render.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/shapes/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2021-01-16 11:36:21.000000 elsie-3.3/elsie/shapes/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1841 2021-01-21 13:04:37.000000 elsie-3.3/elsie/shapes/arrow.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1636 2021-01-16 11:36:21.000000 elsie-3.3/elsie/shapes/path.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.671050 elsie-3.3/elsie/slides/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2020-12-28 22:01:17.000000 elsie-3.3/elsie/slides/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     3235 2020-12-28 22:01:17.000000 elsie-3.3/elsie/slides/show.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2080 2021-03-03 14:21:25.000000 elsie-3.3/elsie/slides/slide.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)    13373 2021-03-03 14:21:25.000000 elsie-3.3/elsie/slides/slidedeck.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.675050 elsie-3.3/elsie/text/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2020-12-28 22:01:17.000000 elsie-3.3/elsie/text/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1576 2020-12-28 22:01:17.000000 elsie-3.3/elsie/text/highlight.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1893 2021-01-21 13:04:37.000000 elsie-3.3/elsie/text/stylecontainer.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     6146 2021-01-21 13:04:37.000000 elsie-3.3/elsie/text/textboxitem.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     7806 2021-01-16 11:36:21.000000 elsie-3.3/elsie/text/textparser.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     5438 2020-12-28 22:01:17.000000 elsie-3.3/elsie/text/textstyle.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.675050 elsie-3.3/elsie/utils/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        0 2020-12-28 22:01:17.000000 elsie-3.3/elsie/utils/__init__.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2979 2021-03-03 14:21:25.000000 elsie-3.3/elsie/utils/cache.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      220 2021-01-05 10:33:37.000000 elsie-3.3/elsie/utils/files.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     2176 2021-01-16 11:36:21.000000 elsie-3.3/elsie/utils/geom.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1873 2020-12-28 22:01:17.000000 elsie-3.3/elsie/utils/sxml.py
--rw-rw-r--   0 spirali   (1000) spirali   (1000)       93 2022-02-05 18:20:24.000000 elsie-3.3/elsie/version.py
-drwxrwxr-x   0 spirali   (1000) spirali   (1000)        0 2022-02-05 18:20:58.667050 elsie-3.3/elsie.egg-info/
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      549 2022-02-05 18:20:58.000000 elsie-3.3/elsie.egg-info/PKG-INFO
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1685 2022-02-05 18:20:58.000000 elsie-3.3/elsie.egg-info/SOURCES.txt
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        1 2022-02-05 18:20:58.000000 elsie-3.3/elsie.egg-info/dependency_links.txt
--rw-rw-r--   0 spirali   (1000) spirali   (1000)      189 2022-02-05 18:20:58.000000 elsie-3.3/elsie.egg-info/requires.txt
--rw-rw-r--   0 spirali   (1000) spirali   (1000)        6 2022-02-05 18:20:58.000000 elsie-3.3/elsie.egg-info/top_level.txt
--rw-rw-r--   0 spirali   (1000) spirali   (1000)       38 2022-02-05 18:20:58.675050 elsie-3.3/setup.cfg
--rw-rw-r--   0 spirali   (1000) spirali   (1000)     1301 2021-01-21 13:04:37.000000 elsie-3.3/setup.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1080 2018-05-20 18:44:50.000000 elsie-3.4/LICENSE
+-rw-rw-r--   0 ada       (1000) ada       (1000)      536 2023-05-25 12:07:41.919147 elsie-3.4/PKG-INFO
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1403 2023-05-25 08:43:04.000000 elsie-3.4/README.md
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie/
+-rw-rw-r--   0 ada       (1000) ada       (1000)      698 2021-01-16 11:36:21.000000 elsie-3.4/elsie/__init__.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie/boxtree/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2020-12-28 22:01:17.000000 elsie-3.4/elsie/boxtree/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     4592 2021-01-21 13:04:37.000000 elsie-3.4/elsie/boxtree/box.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      610 2020-12-28 22:01:17.000000 elsie-3.4/elsie/boxtree/boxitem.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)    26993 2022-02-05 18:06:02.000000 elsie-3.4/elsie/boxtree/boxmixin.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     6799 2020-12-28 22:01:17.000000 elsie-3.4/elsie/boxtree/layout.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1719 2020-12-28 22:01:17.000000 elsie-3.4/elsie/boxtree/lazy.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3759 2020-12-28 22:01:17.000000 elsie-3.4/elsie/boxtree/value.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie/ext/
+-rw-rw-r--   0 ada       (1000) ada       (1000)      298 2021-01-05 10:30:07.000000 elsie-3.4/elsie/ext/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      538 2021-06-01 08:11:47.000000 elsie-3.4/elsie/ext/export.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3483 2021-01-21 13:04:37.000000 elsie-3.4/elsie/ext/latex.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     9493 2021-01-05 10:30:07.000000 elsie-3.4/elsie/ext/list.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     5716 2021-01-05 10:30:07.000000 elsie-3.4/elsie/ext/markdown.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      414 2021-06-01 08:11:47.000000 elsie-3.4/elsie/ext/todo.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie/render/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2020-12-28 22:01:17.000000 elsie-3.4/elsie/render/__init__.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie/render/backends/
+-rw-rw-r--   0 ada       (1000) ada       (1000)      173 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1772 2021-03-03 14:21:25.000000 elsie-3.4/elsie/render/backends/backend.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/render/backends/cairo/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2818 2021-03-03 14:21:25.000000 elsie-3.4/elsie/render/backends/cairo/backend.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2645 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/draw.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     8012 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/rcontext.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1686 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/shapes.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3876 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/svg.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     6849 2023-05-25 12:05:05.000000 elsie-3.4/elsie/render/backends/cairo/text.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      813 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/cairo/utils.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      931 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/rcontext.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/render/backends/svg/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2021-01-16 11:36:21.000000 elsie-3.4/elsie/render/backends/svg/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     5137 2023-05-25 12:05:05.000000 elsie-3.4/elsie/render/backends/svg/backend.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     5450 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/svg/draw.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      599 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/svg/query.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2905 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/backends/svg/rcontext.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1565 2021-01-16 11:36:21.000000 elsie-3.4/elsie/render/backends/svg/utils.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1009 2020-12-28 22:01:17.000000 elsie-3.4/elsie/render/image.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3198 2022-09-03 08:13:39.000000 elsie-3.4/elsie/render/inkscape.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3687 2021-01-21 13:04:37.000000 elsie-3.4/elsie/render/jupyter.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3407 2021-01-16 11:36:21.000000 elsie-3.4/elsie/render/ora.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1203 2020-12-28 22:01:17.000000 elsie-3.4/elsie/render/pdfmerge.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2732 2021-03-03 14:21:25.000000 elsie-3.4/elsie/render/render.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/shapes/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2021-01-16 11:36:21.000000 elsie-3.4/elsie/shapes/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1841 2021-01-21 13:04:37.000000 elsie-3.4/elsie/shapes/arrow.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1636 2021-01-16 11:36:21.000000 elsie-3.4/elsie/shapes/path.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/slides/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2020-12-28 22:01:17.000000 elsie-3.4/elsie/slides/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     3235 2020-12-28 22:01:17.000000 elsie-3.4/elsie/slides/show.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2080 2021-03-03 14:21:25.000000 elsie-3.4/elsie/slides/slide.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)    13373 2021-03-03 14:21:25.000000 elsie-3.4/elsie/slides/slidedeck.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/text/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2020-12-28 22:01:17.000000 elsie-3.4/elsie/text/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1576 2020-12-28 22:01:17.000000 elsie-3.4/elsie/text/highlight.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1893 2021-01-21 13:04:37.000000 elsie-3.4/elsie/text/stylecontainer.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     6146 2021-01-21 13:04:37.000000 elsie-3.4/elsie/text/textboxitem.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     7806 2021-01-16 11:36:21.000000 elsie-3.4/elsie/text/textparser.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     5438 2020-12-28 22:01:17.000000 elsie-3.4/elsie/text/textstyle.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.919147 elsie-3.4/elsie/utils/
+-rw-rw-r--   0 ada       (1000) ada       (1000)        0 2020-12-28 22:01:17.000000 elsie-3.4/elsie/utils/__init__.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2979 2021-03-03 14:21:25.000000 elsie-3.4/elsie/utils/cache.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)      220 2021-01-05 10:33:37.000000 elsie-3.4/elsie/utils/files.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     2176 2021-01-16 11:36:21.000000 elsie-3.4/elsie/utils/geom.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1873 2020-12-28 22:01:17.000000 elsie-3.4/elsie/utils/sxml.py
+-rw-rw-r--   0 ada       (1000) ada       (1000)       93 2023-05-25 12:06:50.000000 elsie-3.4/elsie/version.py
+drwxrwxr-x   0 ada       (1000) ada       (1000)        0 2023-05-25 12:07:41.915147 elsie-3.4/elsie.egg-info/
+-rw-rw-r--   0 ada       (1000) ada       (1000)      536 2023-05-25 12:07:41.000000 elsie-3.4/elsie.egg-info/PKG-INFO
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1693 2023-05-25 12:07:41.000000 elsie-3.4/elsie.egg-info/SOURCES.txt
+-rw-rw-r--   0 ada       (1000) ada       (1000)        1 2023-05-25 12:07:41.000000 elsie-3.4/elsie.egg-info/dependency_links.txt
+-rw-rw-r--   0 ada       (1000) ada       (1000)      189 2023-05-25 12:07:41.000000 elsie-3.4/elsie.egg-info/requires.txt
+-rw-rw-r--   0 ada       (1000) ada       (1000)        6 2023-05-25 12:07:41.000000 elsie-3.4/elsie.egg-info/top_level.txt
+-rw-rw-r--   0 ada       (1000) ada       (1000)       38 2023-05-25 12:07:41.919147 elsie-3.4/setup.cfg
+-rw-rw-r--   0 ada       (1000) ada       (1000)     1301 2021-01-21 13:04:37.000000 elsie-3.4/setup.py
```

### Comparing `elsie-3.3/README.md` & `elsie-3.4/README.md`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/__init__.py` & `elsie-3.4/elsie/__init__.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/box.py` & `elsie-3.4/elsie/boxtree/box.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/boxitem.py` & `elsie-3.4/elsie/boxtree/boxitem.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/boxmixin.py` & `elsie-3.4/elsie/boxtree/boxmixin.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/layout.py` & `elsie-3.4/elsie/boxtree/layout.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/lazy.py` & `elsie-3.4/elsie/boxtree/lazy.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/boxtree/value.py` & `elsie-3.4/elsie/boxtree/value.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/ext/export.py` & `elsie-3.4/elsie/ext/export.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/ext/latex.py` & `elsie-3.4/elsie/ext/latex.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/ext/list.py` & `elsie-3.4/elsie/ext/list.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/ext/markdown.py` & `elsie-3.4/elsie/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/backend.py` & `elsie-3.4/elsie/render/backends/backend.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/backend.py` & `elsie-3.4/elsie/render/backends/cairo/backend.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/draw.py` & `elsie-3.4/elsie/render/backends/cairo/draw.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/rcontext.py` & `elsie-3.4/elsie/render/backends/cairo/rcontext.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/shapes.py` & `elsie-3.4/elsie/render/backends/cairo/shapes.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/svg.py` & `elsie-3.4/elsie/render/backends/cairo/svg.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/cairo/text.py` & `elsie-3.4/elsie/render/backends/cairo/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def from_pango_units(size: int) -> float:
     return pangocffi.units_to_double(size)
 
 
 def to_pango_color(color: Tuple[float, float, float]) -> Tuple[int, int, int]:
     r, g, b = color
-    max = 2 ** 16 - 1
+    max = 2**16 - 1
     return (int(r * max), int(g * max), int(b * max))
 
 
 def attr_from_scale(scale_factor: float, start_index: int, end_index: int):
     scale_factor = ffi.cast("double", scale_factor)
     attr = Attribute._init_pointer(
         pangocffi.pango.pango_attr_scale_new(scale_factor),
```

### Comparing `elsie-3.3/elsie/render/backends/cairo/utils.py` & `elsie-3.4/elsie/render/backends/cairo/utils.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/rcontext.py` & `elsie-3.4/elsie/render/backends/rcontext.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/svg/backend.py` & `elsie-3.4/elsie/render/backends/svg/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 from .draw import draw_text
 from .query import compute_query
 from .rcontext import SvgRenderingContext
 
 VERSION_REGEX = re.compile(r"Inkscape\s+(\d+\..*)")
 
 
+def detect_inkscape_bin():
+    for path in ["/usr/bin/inkscape", "C:/Program Files/Inkscape/bin/inkscape.exe"]:
+        if os.path.isfile(path):
+            return path
+    raise Exception(
+        "Inkscape not found. "
+        "Install Inkscape to a standard path "
+        "or set ELSIE_INKSCAPE variable to Inkscape binary"
+        "or instantiate InkscapeBackend with the path to Inkscape"
+    )
+
+
 class InkscapeBackend(Backend):
     """Backend that maps Elsie primitives to SVG and renders them to PDF using Inkscape."""
 
     def __init__(
         self,
         inkscape: Union[str, InkscapeShell] = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
@@ -32,15 +44,15 @@
             Cache directory for caching SVG files.
         """
         super().__init__(cache_dir)
         if isinstance(inkscape, InkscapeShell):
             self.inkscape = inkscape
         else:
             inkscape_bin = (
-                inkscape or os.environ.get("ELSIE_INKSCAPE") or "/usr/bin/inkscape"
+                inkscape or os.environ.get("ELSIE_INKSCAPE") or detect_inkscape_bin()
             )
             self.inkscape = InkscapeShell(inkscape_bin)
 
         self.inkscape_version = self.inkscape.get_version()
         match = VERSION_REGEX.search(self.inkscape_version)
         if not match:
             print(f"WARNING: Unknown Inkscape version ({self.inkscape_version})")
```

### Comparing `elsie-3.3/elsie/render/backends/svg/draw.py` & `elsie-3.4/elsie/render/backends/svg/draw.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/svg/query.py` & `elsie-3.4/elsie/render/backends/svg/query.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/svg/rcontext.py` & `elsie-3.4/elsie/render/backends/svg/rcontext.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/backends/svg/utils.py` & `elsie-3.4/elsie/render/backends/svg/utils.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/image.py` & `elsie-3.4/elsie/render/image.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/inkscape.py` & `elsie-3.4/elsie/render/inkscape.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/jupyter.py` & `elsie-3.4/elsie/render/jupyter.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/ora.py` & `elsie-3.4/elsie/render/ora.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/pdfmerge.py` & `elsie-3.4/elsie/render/pdfmerge.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/render/render.py` & `elsie-3.4/elsie/render/render.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/shapes/arrow.py` & `elsie-3.4/elsie/shapes/arrow.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/shapes/path.py` & `elsie-3.4/elsie/shapes/path.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/slides/show.py` & `elsie-3.4/elsie/slides/show.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/slides/slide.py` & `elsie-3.4/elsie/slides/slide.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/slides/slidedeck.py` & `elsie-3.4/elsie/slides/slidedeck.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/text/highlight.py` & `elsie-3.4/elsie/text/highlight.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/text/stylecontainer.py` & `elsie-3.4/elsie/text/stylecontainer.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/text/textboxitem.py` & `elsie-3.4/elsie/text/textboxitem.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/text/textparser.py` & `elsie-3.4/elsie/text/textparser.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/text/textstyle.py` & `elsie-3.4/elsie/text/textstyle.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/utils/cache.py` & `elsie-3.4/elsie/utils/cache.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/utils/geom.py` & `elsie-3.4/elsie/utils/geom.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie/utils/sxml.py` & `elsie-3.4/elsie/utils/sxml.py`

 * *Files identical despite different names*

### Comparing `elsie-3.3/elsie.egg-info/SOURCES.txt` & `elsie-3.4/elsie.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 elsie/__init__.py
 elsie/version.py
 elsie.egg-info/PKG-INFO
 elsie.egg-info/SOURCES.txt
 elsie.egg-info/dependency_links.txt
```

### Comparing `elsie-3.3/setup.py` & `elsie-3.4/setup.py`

 * *Files identical despite different names*

