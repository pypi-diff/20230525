# Comparing `tmp/picosvg-0.9.0.tar.gz` & `tmp/picosvg-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picosvg-0.9.0.tar", last modified: Mon Dec  7 10:59:29 2020, max compression
+gzip compressed data, was "dist/picosvg-0.9.1.tar", last modified: Tue Dec  8 10:16:32 2020, max compression
```

## Comparing `picosvg-0.9.0.tar` & `picosvg-0.9.1.tar`

### file list

```diff
@@ -1,116 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.058202 picosvg-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-12-07 10:59:16.000000 picosvg-0.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     3642 2020-12-07 10:59:16.000000 picosvg-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-12-07 10:59:16.000000 picosvg-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    11358 2020-12-07 10:59:16.000000 picosvg-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      308 2020-12-07 10:59:29.058202 picosvg-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1024 2020-12-07 10:59:16.000000 picosvg-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2020-12-07 10:59:16.000000 picosvg-0.9.0/docs/contributing.md
--rwxr-xr-x   0 runner    (1001) docker     (116)      749 2020-12-07 10:59:16.000000 picosvg-0.9.0/precommit.sh
--rw-r--r--   0 runner    (1001) docker     (116)       89 2020-12-07 10:59:29.058202 picosvg-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1732 2020-12-07 10:59:16.000000 picosvg-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/src/picosvg/
--rw-r--r--   0 runner    (1001) docker     (116)      700 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      116 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     7576 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/arc_to_cubic.py
--rw-r--r--   0 runner    (1001) docker     (116)     4622 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/geometric_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     1819 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/picosvg.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)    34789 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg.py
--rw-r--r--   0 runner    (1001) docker     (116)     4821 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_meta.py
--rw-r--r--   0 runner    (1001) docker     (116)     2884 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_path_iter.py
--rw-r--r--   0 runner    (1001) docker     (116)     6709 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_pathops.py
--rw-r--r--   0 runner    (1001) docker     (116)     8389 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_reuse.py
--rw-r--r--   0 runner    (1001) docker     (116)     6808 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)    27347 2020-12-07 10:59:16.000000 picosvg-0.9.0/src/picosvg/svg_types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.050202 picosvg-0.9.0/src/picosvg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      308 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2981 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      166 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-07 10:59:28.000000 picosvg-0.9.0/src/picosvg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-07 10:59:29.058202 picosvg-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2886 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/arc_to_cubic_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      428 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/arcs-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2214 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/arcs-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      153 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/bad-defs-0.svg
--rw-r--r--   0 runner    (1001) docker     (116)      110 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/bad-defs-1.svg
--rw-r--r--   0 runner    (1001) docker     (116)      237 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-curves-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      337 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-curves.svg
--rw-r--r--   0 runner    (1001) docker     (116)      319 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-ellipse-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      297 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (116)      209 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-groups-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      451 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-groups.svg
--rw-r--r--   0 runner    (1001) docker     (116)      195 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-multirect-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      339 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-multirect.svg
--rw-r--r--   0 runner    (1001) docker     (116)      144 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-rect-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      266 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-rect.svg
--rw-r--r--   0 runner    (1001) docker     (116)      217 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-rule-evenodd-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      532 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-rule-evenodd.svg
--rw-r--r--   0 runner    (1001) docker     (116)      222 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-use-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      328 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clip-use.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1291 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clipped-strokes-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1414 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/clipped-strokes-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      371 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/degenerate-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      149 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/degenerate-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/drop-anon-symbols-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      261 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/drop-anon-symbols-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)    23193 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/emoji_u1f469_1f3fd_200d_1f91d_200d_1f468_1f3fb.svg
--rw-r--r--   0 runner    (1001) docker     (116)      472 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/fill-rule-evenodd-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      978 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/fill-rule-evenodd-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)     3150 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/geometric_types_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      327 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/good-defs-0.svg
--rw-r--r--   0 runner    (1001) docker     (116)      114 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/group-data-name-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      187 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/group-data-name-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      196 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/group-stroke-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      166 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/group-stroke-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      479 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/inline-css-style-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      508 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/inline-css-style-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      520 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/inline-css-style-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      193 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/invisible-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      500 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/invisible-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      246 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/invisible-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      509 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/matrix-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      382 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/matrix-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      348 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/outside-viewbox-clipped.svg
--rw-r--r--   0 runner    (1001) docker     (116)      336 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/outside-viewbox.svg
--rw-r--r--   0 runner    (1001) docker     (116)      148 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/rotated-rect-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      138 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/rotated-rect.svg
--rw-r--r--   0 runner    (1001) docker     (116)      424 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/scale-strokes-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      440 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/scale-strokes-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      362 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/scale-strokes-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      886 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-capjoinmiterlimit-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      494 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-capjoinmiterlimit-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      339 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-fill-opacity-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      310 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-fill-opacity-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      390 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-path-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      272 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-path-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      252 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-simplepath-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      227 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/stroke-simplepath-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)     3834 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_pathops_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5097 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_reuse_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    17911 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1678 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     5975 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_transform_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    11031 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/svg_types_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      521 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/transform-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      934 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/transform-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      178 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/translate-rect-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      208 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/translate-rect.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1221 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/twemoji-lesotho-flag-after-ungroup.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/twemoji-lesotho-flag-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/twemoji-lesotho-flag-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      695 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      965 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      989 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-multiple-children-after.svg
--rw-r--r--   0 runner    (1001) docker     (116)      906 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-multiple-children-before.svg
--rw-r--r--   0 runner    (1001) docker     (116)      444 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-multiple-children-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      350 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/ungroup-nano.svg
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/use-ellipse-resolved.svg
--rw-r--r--   0 runner    (1001) docker     (116)      355 2020-12-07 10:59:16.000000 picosvg-0.9.0/tests/use-ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1210 2020-12-07 10:59:16.000000 picosvg-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.947519 picosvg-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.939519 picosvg-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2020-12-08 10:16:19.000000 picosvg-0.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.939519 picosvg-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     3598 2020-12-08 10:16:19.000000 picosvg-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       90 2020-12-08 10:16:19.000000 picosvg-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)    11358 2020-12-08 10:16:19.000000 picosvg-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2020-12-08 10:16:32.947519 picosvg-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1024 2020-12-08 10:16:19.000000 picosvg-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.939519 picosvg-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     1097 2020-12-08 10:16:19.000000 picosvg-0.9.1/docs/contributing.md
+-rwxr-xr-x   0 runner    (1001) docker     (116)      749 2020-12-08 10:16:19.000000 picosvg-0.9.1/precommit.sh
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2020-12-08 10:16:32.947519 picosvg-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1732 2020-12-08 10:16:19.000000 picosvg-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.935519 picosvg-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.939519 picosvg-0.9.1/src/picosvg/
+-rw-r--r--   0 runner    (1001) docker     (116)      700 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      116 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7576 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/arc_to_cubic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4622 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/geometric_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1819 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/picosvg.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (116)    35693 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4821 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_meta.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2884 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_path_iter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6709 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_pathops.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8389 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6808 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27347 2020-12-08 10:16:19.000000 picosvg-0.9.1/src/picosvg/svg_types.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.939519 picosvg-0.9.1/src/picosvg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      308 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3129 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       50 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2020-12-08 10:16:32.000000 picosvg-0.9.1/src/picosvg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-08 10:16:32.947519 picosvg-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     2886 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/arc_to_cubic_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      428 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/arcs-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     2214 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/arcs-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      153 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/bad-defs-0.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      110 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/bad-defs-1.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      214 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/bad-ids-1.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      237 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-curves-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      337 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-curves.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      319 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-ellipse-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      297 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      209 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-groups-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      451 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-groups.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      195 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-multirect-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      339 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-multirect.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      144 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-rect-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-rect.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      217 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-rule-evenodd-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      532 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-rule-evenodd.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      222 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-use-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      328 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clip-use.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1291 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clipped-strokes-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1414 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/clipped-strokes-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      371 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/degenerate-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      149 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/degenerate-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      150 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/drop-anon-symbols-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      261 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/drop-anon-symbols-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)    23193 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/emoji_u1f469_1f3fd_200d_1f91d_200d_1f468_1f3fb.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      472 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/fill-rule-evenodd-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      978 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/fill-rule-evenodd-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     3150 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/geometric_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      327 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/good-defs-0.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/group-data-name-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/group-data-name-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      196 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/group-stroke-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/group-stroke-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      479 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/inline-css-style-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      508 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/inline-css-style-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      520 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/inline-css-style-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      193 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/invisible-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      500 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/invisible-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      246 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/invisible-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      509 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/matrix-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      382 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/matrix-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      348 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/outside-viewbox-clipped.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      336 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/outside-viewbox.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      148 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/rotated-rect-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      138 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/rotated-rect.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/scale-strokes-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      440 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/scale-strokes-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      362 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/scale-strokes-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      886 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-capjoinmiterlimit-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      494 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-capjoinmiterlimit-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      339 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-fill-opacity-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      310 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-fill-opacity-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      390 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-path-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-path-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-simplepath-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-simplepath-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      228 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-with-id-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      197 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/stroke-with-id-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     3834 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_pathops_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5097 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_reuse_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18230 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1678 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5975 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11031 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/svg_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      521 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/transform-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      934 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/transform-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/translate-rect-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      208 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/translate-rect.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1221 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/twemoji-lesotho-flag-after-ungroup.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1198 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/twemoji-lesotho-flag-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1638 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/twemoji-lesotho-flag-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      695 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      965 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      989 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-multiple-children-after.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      906 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-multiple-children-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      444 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-multiple-children-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      350 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      354 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-with-ids-before.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      271 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/ungroup-with-ids-nano.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/use-ellipse-resolved.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2020-12-08 10:16:19.000000 picosvg-0.9.1/tests/use-ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (116)     1210 2020-12-08 10:16:19.000000 picosvg-0.9.1/tox.ini
```

### Comparing `picosvg-0.9.0/.github/workflows/ci.yml` & `picosvg-0.9.1/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,16 @@
         PRERELEASE_TAG_PATTERN: "v[[:digit:]]+\\.[[:digit:]]+\\.[[:digit:]]+([ab]|rc)[[:digit:]]+"
       run: |
         # GH checkout action doesn't preserve tag annotations, we must fetch them
         # https://github.com/actions/checkout/issues/290
         git fetch --tags --force
         # strip leading 'refs/tags/' to get the tag name
         TAG_NAME="${GITHUB_REF##*/}"
-        # Dump tag message to temporary .md file (excluding the first title line and PGP
-        # signature at the bottom)
-        TAG_MESSAGE=$(git tag -l --format='%(contents)' $TAG_NAME | tail -n +2 | sed -n '/-----BEGIN PGP SIGNATURE-----/q;p')
+        # Dump tag message to temporary .md file (excluding the PGP signature at the bottom)
+        TAG_MESSAGE=$(git tag -l --format='%(contents)' $TAG_NAME | sed -n '/-----BEGIN PGP SIGNATURE-----/q;p')
         echo "$TAG_MESSAGE" > "${{ runner.temp }}/release_notes.md"
         # if the tag has a pre-release suffix mark the Github Release accordingly
         if egrep -q "$PRERELEASE_TAG_PATTERN" <<< "$TAG_NAME"; then
           echo "Tag contains a pre-release suffix"
           echo "IS_PRERELEASE=true" >> "$GITHUB_ENV"
         else
           echo "Tag does not contain pre-release suffix"
```

### Comparing `picosvg-0.9.0/LICENSE` & `picosvg-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/README.md` & `picosvg-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/docs/contributing.md` & `picosvg-0.9.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/precommit.sh` & `picosvg-0.9.1/precommit.sh`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/setup.py` & `picosvg-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/__init__.py` & `picosvg-0.9.1/src/picosvg/__init__.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/arc_to_cubic.py` & `picosvg-0.9.1/src/picosvg/arc_to_cubic.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/geometric_types.py` & `picosvg-0.9.1/src/picosvg/geometric_types.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/picosvg.py` & `picosvg-0.9.1/src/picosvg/picosvg.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg.py` & `picosvg-0.9.1/src/picosvg/svg.py`

 * *Files 5% similar despite different names*

```diff
@@ -272,46 +272,52 @@
         if not match:
             raise ValueError(f'Unrecognized url "{url}"')
         return self.xpath_one(f'//svg:{el_tag}[@id="{match.group(1)}"]')
 
     def _resolve_use(self, scope_el):
         attrib_not_copied = {"x", "y", "width", "height", _xlink_href_attr_name()}
 
-        swaps = []
-
-        for use_el in self.xpath(".//svg:use", el=scope_el):
-            ref = use_el.attrib.get(_xlink_href_attr_name(), "")
-            if not ref.startswith("#"):
-                raise ValueError(f"Only use #fragment supported, reject {ref}")
-            target = self.xpath_one(f'//svg:*[@id="{ref[1:]}"]')
-
-            new_el = copy.deepcopy(target)
-            del new_el.attrib["id"]
-
-            group = etree.Element(f"{{{svgns()}}}g", nsmap=self.svg_root.nsmap)
-            use_x = use_el.attrib.get("x", 0)
-            use_y = use_el.attrib.get("y", 0)
-            if use_x != 0 or use_y != 0:
-                group.attrib["transform"] = (
-                    group.attrib.get("transform", "") + f" translate({use_x}, {use_y})"
-                ).strip()
-
-            for attr_name in use_el.attrib:
-                if attr_name in attrib_not_copied:
-                    continue
-                group.attrib[attr_name] = use_el.attrib[attr_name]
-
-            if len(group.attrib):
-                group.append(new_el)
-                swaps.append((use_el, group))
-            else:
-                swaps.append((use_el, new_el))
+        while True:
+            swaps = []
+            use_els = list(self.xpath(".//svg:use", el=scope_el))
+            if not use_els:
+                break
+            for use_el in use_els:
+                ref = use_el.attrib.get(_xlink_href_attr_name(), "")
+                if not ref.startswith("#"):
+                    raise ValueError(f"Only use #fragment supported, reject {ref}")
+                target = self.xpath_one(f'//svg:*[@id="{ref[1:]}"]')
+
+                new_el = copy.deepcopy(target)
+
+                group = etree.Element(f"{{{svgns()}}}g", nsmap=self.svg_root.nsmap)
+                use_x = use_el.attrib.get("x", 0)
+                use_y = use_el.attrib.get("y", 0)
+                if use_x != 0 or use_y != 0:
+                    group.attrib["transform"] = (
+                        group.attrib.get("transform", "")
+                        + f" translate({use_x}, {use_y})"
+                    ).strip()
+
+                for attr_name in use_el.attrib:
+                    if attr_name in attrib_not_copied:
+                        continue
+                    group.attrib[attr_name] = use_el.attrib[attr_name]
+
+                if len(group.attrib):
+                    group.append(new_el)
+                    swaps.append((use_el, group))
+                else:
+                    swaps.append((use_el, new_el))
 
-        for old_el, new_el in swaps:
-            old_el.getparent().replace(old_el, new_el)
+            for old_el, new_el in swaps:
+                # leaving id's on <use> instantiated content is a path to duplicate ids
+                for new_el_with_id in self.xpath("//svg:*[@id]", el=new_el):
+                    del new_el_with_id.attrib["id"]
+                old_el.getparent().replace(old_el, new_el)
 
     def resolve_use(self, inplace=False):
         """Instantiate reused elements.
 
         https://www.w3.org/TR/SVG11/struct.html#UseElement"""
         if not inplace:
             svg = SVG(copy.deepcopy(self.svg_root))
@@ -531,14 +537,18 @@
         # remove all the stroke settings
         for cleanmeup in (shape, stroke):
             _reset_attrs(cleanmeup, lambda field: field.name.startswith("stroke"))
 
         if not shape.might_paint():
             return (stroke,)
 
+        # The original id doesn't correctly refer to either
+        # It would be for the best if any id-based operations happened first
+        shape.id = stroke.id = ""
+
         return (shape, stroke)
 
     def strokes_to_paths(self, inplace=False):
         """Convert stroked shapes to equivalent filled shape + path for stroke."""
         if not inplace:
             svg = SVG(copy.deepcopy(self.svg_root))
             svg.strokes_to_paths(inplace=True)
@@ -896,24 +906,33 @@
             r"^/svg\[0\]$",
             r"^/svg\[0\]/defs\[0\]$",
             r"^/svg\[0\]/defs\[0\]/(linear|radial)Gradient\[\d+\](/stop\[\d+\])?$",
             r"^/svg\[0\]/path\[(?!0\])\d+\]$",
         }
 
         # Make a list of xpaths with offsets (/svg/defs[0]/..., etc)
+        ids = {}
         frontier = [(0, self.svg_root, "")]
         while frontier:
             el_idx, el, parent_path = frontier.pop(0)
             el_tag = strip_ns(el.tag)
             el_path = f"{parent_path}/{el_tag}[{el_idx}]"
 
             if not any((re.match(pat, el_path) for pat in path_whitelist)):
                 errors.append(f"BadElement: {el_path}")
                 continue  # no sense reporting all the children as bad
 
+            el_id = el.attrib.get("id", None)
+            if el_id is not None:
+                if el_id in ids:
+                    errors.append(
+                        f'BadElement: {el_path} reuses id="{el_id}", first seen at {ids[el_id]}'
+                    )
+                ids[el_id] = el_path
+
             for child_idx, child in enumerate(el):
                 if child.tag is etree.Comment:
                     continue
                 frontier.append((child_idx, child, el_path))
 
         # TODO paths & gradients should only have specific attributes
```

### Comparing `picosvg-0.9.0/src/picosvg/svg_meta.py` & `picosvg-0.9.1/src/picosvg/svg_meta.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg_path_iter.py` & `picosvg-0.9.1/src/picosvg/svg_path_iter.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg_pathops.py` & `picosvg-0.9.1/src/picosvg/svg_pathops.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg_reuse.py` & `picosvg-0.9.1/src/picosvg/svg_reuse.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg_transform.py` & `picosvg-0.9.1/src/picosvg/svg_transform.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg/svg_types.py` & `picosvg-0.9.1/src/picosvg/svg_types.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/src/picosvg.egg-info/SOURCES.txt` & `picosvg-0.9.1/src/picosvg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/picosvg.egg-info/requires.txt
 src/picosvg.egg-info/top_level.txt
 tests/arc_to_cubic_test.py
 tests/arcs-before.svg
 tests/arcs-nano.svg
 tests/bad-defs-0.svg
 tests/bad-defs-1.svg
+tests/bad-ids-1.svg
 tests/clip-curves-clipped.svg
 tests/clip-curves.svg
 tests/clip-ellipse-clipped.svg
 tests/clip-ellipse.svg
 tests/clip-groups-clipped.svg
 tests/clip-groups.svg
 tests/clip-multirect-clipped.svg
@@ -80,14 +81,16 @@
 tests/stroke-capjoinmiterlimit-before.svg
 tests/stroke-fill-opacity-after.svg
 tests/stroke-fill-opacity-before.svg
 tests/stroke-path-after.svg
 tests/stroke-path-before.svg
 tests/stroke-simplepath-after.svg
 tests/stroke-simplepath-before.svg
+tests/stroke-with-id-before.svg
+tests/stroke-with-id-nano.svg
 tests/svg_pathops_test.py
 tests/svg_reuse_test.py
 tests/svg_test.py
 tests/svg_test_helpers.py
 tests/svg_transform_test.py
 tests/svg_types_test.py
 tests/transform-before.svg
@@ -99,9 +102,11 @@
 tests/twemoji-lesotho-flag-nano.svg
 tests/ungroup-after.svg
 tests/ungroup-before.svg
 tests/ungroup-multiple-children-after.svg
 tests/ungroup-multiple-children-before.svg
 tests/ungroup-multiple-children-nano.svg
 tests/ungroup-nano.svg
+tests/ungroup-with-ids-before.svg
+tests/ungroup-with-ids-nano.svg
 tests/use-ellipse-resolved.svg
 tests/use-ellipse.svg
```

### Comparing `picosvg-0.9.0/tests/arc_to_cubic_test.py` & `picosvg-0.9.1/tests/arc_to_cubic_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/arcs-nano.svg` & `picosvg-0.9.1/tests/arcs-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/clip-rule-evenodd.svg` & `picosvg-0.9.1/tests/clip-rule-evenodd.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/clipped-strokes-before.svg` & `picosvg-0.9.1/tests/clipped-strokes-before.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/clipped-strokes-nano.svg` & `picosvg-0.9.1/tests/clipped-strokes-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/emoji_u1f469_1f3fd_200d_1f91d_200d_1f468_1f3fb.svg` & `picosvg-0.9.1/tests/emoji_u1f469_1f3fd_200d_1f91d_200d_1f468_1f3fb.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/fill-rule-evenodd-nano.svg` & `picosvg-0.9.1/tests/fill-rule-evenodd-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/geometric_types_test.py` & `picosvg-0.9.1/tests/geometric_types_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/inline-css-style-nano.svg` & `picosvg-0.9.1/tests/inline-css-style-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/stroke-capjoinmiterlimit-after.svg` & `picosvg-0.9.1/tests/stroke-capjoinmiterlimit-after.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/svg_pathops_test.py` & `picosvg-0.9.1/tests/svg_pathops_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/svg_reuse_test.py` & `picosvg-0.9.1/tests/svg_reuse_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/svg_test.py` & `picosvg-0.9.1/tests/svg_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,16 @@
         ("degenerate-before.svg", "degenerate-nano.svg"),
         ("fill-rule-evenodd-before.svg", "fill-rule-evenodd-nano.svg"),
         ("twemoji-lesotho-flag-before.svg", "twemoji-lesotho-flag-nano.svg"),
         ("inline-css-style-before.svg", "inline-css-style-nano.svg"),
         ("clipped-strokes-before.svg", "clipped-strokes-nano.svg"),
         ("drop-anon-symbols-before.svg", "drop-anon-symbols-after.svg"),
         ("scale-strokes-before.svg", "scale-strokes-nano.svg"),
+        ("ungroup-with-ids-before.svg", "ungroup-with-ids-nano.svg"),
+        ("stroke-with-id-before.svg", "stroke-with-id-nano.svg"),
     ],
 )
 def test_topicosvg(actual, expected_result):
     _test(actual, expected_result, lambda svg: svg.topicosvg())
 
 
 @pytest.mark.parametrize(
@@ -298,14 +300,20 @@
             "bad-defs-0.svg",
             (
                 "BadElement: /svg[0]/defs[1]",
                 "BadElement: /svg[0]/donkey[2]",
             ),
         ),
         ("bad-defs-1.svg", ("BadElement: /svg[0]/path[0]",)),
+        (
+            "bad-ids-1.svg",
+            (
+                'BadElement: /svg[0]/path[2] reuses id="not_so_unique", first seen at /svg[0]/path[1]',
+            ),
+        ),
     ],
 )
 def test_checkpicosvg(svg_file, expected_violations):
     nano_violations = load_test_svg(svg_file).checkpicosvg()
     assert expected_violations == nano_violations
```

### Comparing `picosvg-0.9.0/tests/svg_test_helpers.py` & `picosvg-0.9.1/tests/svg_test_helpers.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/svg_transform_test.py` & `picosvg-0.9.1/tests/svg_transform_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/svg_types_test.py` & `picosvg-0.9.1/tests/svg_types_test.py`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/transform-before.svg` & `picosvg-0.9.1/tests/transform-before.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/transform-nano.svg` & `picosvg-0.9.1/tests/transform-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/twemoji-lesotho-flag-after-ungroup.svg` & `picosvg-0.9.1/tests/twemoji-lesotho-flag-after-ungroup.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/twemoji-lesotho-flag-before.svg` & `picosvg-0.9.1/tests/twemoji-lesotho-flag-before.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/twemoji-lesotho-flag-nano.svg` & `picosvg-0.9.1/tests/twemoji-lesotho-flag-nano.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/ungroup-after.svg` & `picosvg-0.9.1/tests/ungroup-after.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/ungroup-before.svg` & `picosvg-0.9.1/tests/ungroup-before.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/ungroup-multiple-children-after.svg` & `picosvg-0.9.1/tests/ungroup-multiple-children-after.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tests/ungroup-multiple-children-before.svg` & `picosvg-0.9.1/tests/ungroup-multiple-children-before.svg`

 * *Files identical despite different names*

### Comparing `picosvg-0.9.0/tox.ini` & `picosvg-0.9.1/tox.ini`

 * *Files identical despite different names*

