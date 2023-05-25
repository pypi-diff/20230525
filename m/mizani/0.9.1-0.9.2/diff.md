# Comparing `tmp/mizani-0.9.1.tar.gz` & `tmp/mizani-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizani-0.9.1.tar", last modified: Fri May 19 16:40:47 2023, max compression
+gzip compressed data, was "mizani-0.9.2.tar", last modified: Thu May 25 18:59:06 2023, max compression
```

## Comparing `mizani-0.9.1.tar` & `mizani-0.9.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 16:40:38.000000 mizani-0.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.725091 mizani-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-19 16:40:38.000000 mizani-0.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-19 16:40:38.000000 mizani-0.9.1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-19 16:40:38.000000 mizani-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-19 16:40:38.000000 mizani-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 16:40:38.000000 mizani-0.9.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-19 16:40:38.000000 mizani-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-19 16:40:38.000000 mizani-0.9.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 16:40:47.737091 mizani-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-19 16:40:38.000000 mizani-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 16:40:38.000000 mizani-0.9.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/bounds.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/breaks.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/palettes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/scale.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/sphinxext/inline_code_highlight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbar-2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbarsearchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/navbartoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/relations.html
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/searchresults.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/sourcelink.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.725091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.729091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/
--rw-r--r--   0 runner    (1001) docker     (123)   124135 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-sphinx.css_t
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/bootstrap-sphinx.js_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/doc/theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/js/jquery-1.12.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/static/js/jquery-fix.js
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-19 16:40:38.000000 mizani-0.9.1/doc/transforms.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/licences/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/HUSL_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SCALES_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SEABORN_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 16:40:38.000000 mizani-0.9.1/licences/SIX_LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/breaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/colors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/colors/brewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/diverging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/qualitative.py
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/brewer/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/colors/color_palette.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani/external/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/crayon_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/husl.py
--rw-r--r--   0 runner    (1001) docker     (123)    28029 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/external/xkcd_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22688 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/palettes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/mizani/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_breaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_palettes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21685 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-19 16:40:38.000000 mizani-0.9.1/mizani/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.733091 mizani-0.9.1/mizani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 16:40:47.000000 mizani-0.9.1/mizani.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-19 16:40:38.000000 mizani-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:40:47.737091 mizani-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:40:47.737091 mizani-0.9.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/build_theme.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/gha_check_semver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 16:40:38.000000 mizani-0.9.1/tools/release-checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 18:58:55.000000 mizani-0.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.006120 mizani-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-25 18:58:55.000000 mizani-0.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-25 18:58:55.000000 mizani-0.9.2/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 18:58:55.000000 mizani-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 18:58:55.000000 mizani-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 18:58:55.000000 mizani-0.9.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-25 18:58:55.000000 mizani-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-25 18:58:55.000000 mizani-0.9.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-25 18:59:06.018121 mizani-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 18:58:55.000000 mizani-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-25 18:58:55.000000 mizani-0.9.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/bounds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/breaks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/palettes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/scale.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.010120 mizani-0.9.2/doc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/sphinxext/inline_code_highlight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbar-2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbarsearchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/navbartoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/searchresults.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/sourcelink.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.006120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   124135 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40021 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/bootstrap-sphinx.js_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/doc/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    97163 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/js/jquery-1.12.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/static/js/jquery-fix.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 18:58:55.000000 mizani-0.9.2/doc/transforms.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/licences/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/HUSL_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SCALES_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SEABORN_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 18:58:55.000000 mizani-0.9.2/licences/SIX_LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.014120 mizani-0.9.2/mizani/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26005 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/breaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/colors/brewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/diverging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/qualitative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/brewer/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/colors/color_palette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/crayon_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/husl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28029 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/external/xkcd_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22688 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_breaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_palettes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21685 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-25 18:58:55.000000 mizani-0.9.2/mizani/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/mizani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-25 18:59:06.000000 mizani-0.9.2/mizani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 18:59:05.000000 mizani-0.9.2/mizani.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-25 18:58:55.000000 mizani-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:59:06.018121 mizani-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:59:06.018121 mizani-0.9.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/build_theme.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/gha_check_semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 18:58:55.000000 mizani-0.9.2/tools/release-checklist.md
```

### Comparing `mizani-0.9.1/.github/workflows/release.yml` & `mizani-0.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/.github/workflows/testing.yml` & `mizani-0.9.2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/.gitignore` & `mizani-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/.readthedocs.yaml` & `mizani-0.9.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/LICENSE` & `mizani-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/Makefile` & `mizani-0.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/PKG-INFO` & `mizani-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.1
+Version: 0.9.2
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.1/README.md` & `mizani-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/Makefile` & `mizani-0.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/_static/copybutton.js` & `mizani-0.9.2/doc/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/_static/custom.css` & `mizani-0.9.2/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/changelog.rst` & `mizani-0.9.2/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 Changelog
 =========
 
+v0.9.2
+------
+
+*2023-05-25*
+
+Bug Fixes
+*********
+
+- Fixed regression in but in :class:`~mizani.formatters.date_format` where
+  it cannot deal with UTC timezone from :class:`~datetime.timezone`
+  :issue:`30`.
+
 v0.9.1
 ------
 
 *2023-05-19*
 
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7951172.svg
+   :target: https://doi.org/10.5281/zenodo.7951172
+
 Bug Fixes
 *********
 
 - Fixed but in :class:`~mizani.formatters.date_format` to handle datetime
   sequences within the same timezone but a mixed daylight saving state.
   `(plotnine #687) <https://github.com/has2k1/plotnine/issues/687>`_
 
 v0.9.0
 ------
 
 *2023-04-15*
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7951171.svg
+   :target: https://doi.org/10.5281/zenodo.7951171
+
 API Changes
 ************
 
 - `palettable` dropped as a dependency.
 
 Bug Fixes
 *********
```

### Comparing `mizani-0.9.1/doc/conf.py` & `mizani-0.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/installation.rst` & `mizani-0.9.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/layout.html` & `mizani-0.9.2/doc/theme/layout.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/navbar-2.html` & `mizani-0.9.2/doc/theme/navbar-2.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/navbar.html` & `mizani-0.9.2/doc/theme/navbar.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/relations.html` & `mizani-0.9.2/doc/theme/relations.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/search.html` & `mizani-0.9.2/doc/theme/search.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/searchresults.html` & `mizani-0.9.2/doc/theme/searchresults.html`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css` & `mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js` & `mizani-0.9.2/doc/theme/static/bootstrap-3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/static/bootstrap-sphinx.css_t` & `mizani-0.9.2/doc/theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/static/bootstrap-sphinx.js_t` & `mizani-0.9.2/doc/theme/static/bootstrap-sphinx.js_t`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/static/js/jquery-1.12.4.min.js` & `mizani-0.9.2/doc/theme/static/js/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/doc/theme/theme.conf` & `mizani-0.9.2/doc/theme/theme.conf`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/licences/HUSL_LICENSE` & `mizani-0.9.2/licences/HUSL_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/licences/SEABORN_LICENSE` & `mizani-0.9.2/licences/SEABORN_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/licences/SIX_LICENSE` & `mizani-0.9.2/licences/SIX_LICENSE`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/bounds.py` & `mizani-0.9.2/mizani/bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/breaks.py` & `mizani-0.9.2/mizani/breaks.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/colors/brewer/__init__.py` & `mizani-0.9.2/mizani/colors/brewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/colors/brewer/diverging.py` & `mizani-0.9.2/mizani/colors/brewer/diverging.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/colors/brewer/qualitative.py` & `mizani-0.9.2/mizani/colors/brewer/qualitative.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/colors/brewer/sequential.py` & `mizani-0.9.2/mizani/colors/brewer/sequential.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/colors/color_palette.py` & `mizani-0.9.2/mizani/colors/color_palette.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/external/crayon_rgb.py` & `mizani-0.9.2/mizani/external/crayon_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/external/husl.py` & `mizani-0.9.2/mizani/external/husl.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/external/xkcd_rgb.py` & `mizani-0.9.2/mizani/external/xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/formatters.py` & `mizani-0.9.2/mizani/formatters.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/palettes.py` & `mizani-0.9.2/mizani/palettes.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/scale.py` & `mizani-0.9.2/mizani/scale.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_bounds.py` & `mizani-0.9.2/mizani/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_breaks.py` & `mizani-0.9.2/mizani/tests/test_breaks.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_formatters.py` & `mizani-0.9.2/mizani/tests/test_formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     # Unknown Timezone
     class myTzInfo(tzinfo):
         def __str__(self):
             return "None"
 
     TZ = myTzInfo()
     x = [datetime(2023, 10, 1, tzinfo=TZ), datetime(2023, 11, 1, tzinfo=TZ)]
-    with pytest.raises(ValueError, match=r"^Unrecognised timezone class"):
+    with pytest.raises(NotImplementedError, match=r"^a tzinfo subclass"):
         date_format()(x)
 
 
 def test_timedelta_format():
     x = [timedelta(days=7 * i) for i in range(5)]
     labels = timedelta_format()(x)
     assert labels == ["0", "1 week", "2 weeks", "3 weeks", "4 weeks"]
```

### Comparing `mizani-0.9.1/mizani/tests/test_palettes.py` & `mizani-0.9.2/mizani/tests/test_palettes.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_scale.py` & `mizani-0.9.2/mizani/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_transforms.py` & `mizani-0.9.2/mizani/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/tests/test_utils.py` & `mizani-0.9.2/mizani/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/transforms.py` & `mizani-0.9.2/mizani/transforms.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/typing.py` & `mizani-0.9.2/mizani/typing.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/mizani/utils.py` & `mizani-0.9.2/mizani/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
 
 import typing
 from collections import OrderedDict, defaultdict
 from collections.abc import Iterator
+from datetime import timezone, tzinfo
 from itertools import chain
 from warnings import warn
 
-try:
-    from zoneinfo import ZoneInfo
-except ImportError:
-    # python < 3.9
-    from backports.zoneinfo import ZoneInfo
-
 import numpy as np
 
 if typing.TYPE_CHECKING:
     from datetime import datetime
     from typing import Sequence
 
 
@@ -326,48 +321,33 @@
     elif base == np.e:
         res = np.log(x)
     else:
         res = np.log(x) / np.log(base)
     return res
 
 
-def get_timezone(x: Sequence[datetime]) -> ZoneInfo:
+def get_timezone(x: Sequence[datetime]) -> tzinfo:
     """
     Return a single timezone for the sequence of datetimes
 
     Returns the timezone of first item and warns if any other item
     has a different timezone
     """
 
-    from pytz.tzinfo import BaseTzInfo
-
     # Ref: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
 
     info = x[0].tzinfo
     if info is None:
-        return ZoneInfo("UTC")
-
-    # We recognise two sources of timezone info:
-    #   1. zoneinfo
-    #   2. pytz
-    # These are all subclasses of datetime.tzinfo but they store the
-    # timezone identifier e.g. (Africa/Uganda) in different properties
-    # We assume that all items in the sequence do not mix
-    if isinstance(info, ZoneInfo):
-        prop = "key"
-    elif isinstance(info, BaseTzInfo):
-        prop = "zone"
-    else:
-        raise ValueError(f"Unrecognised timezone class {info.__class__}")
+        return timezone.utc
 
     # Consistency check
-    tz = ZoneInfo(getattr(info, prop))
-    tz_ids = (getattr(value.tzinfo, prop) for value in x)
-    if any(id != tz.key for id in tz_ids):
+    tzname0 = info.tzname(x[0])
+    tznames = (dt.tzinfo.tzname(dt) if dt.tzinfo else None for dt in x)
+    if any(tzname0 != name for name in tznames):
         msg = (
             "Dates in column have different time zones. "
             "Choosen `{}` the time zone of the first date. "
             "To use a different time zone, create a "
             "formatter and pass the time zone."
         )
-        warn(msg.format(tz.key))
-    return tz
+        warn(msg.format(tzname0))
+    return info
```

### Comparing `mizani-0.9.1/mizani.egg-info/PKG-INFO` & `mizani-0.9.2/mizani.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizani
-Version: 0.9.1
+Version: 0.9.2
 Summary: Scales for Python
 Author-email: Hassan Kibirige <has2k1@gmail.com>
 License: Copyright (c) 2016, Hassan Kibirige
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `mizani-0.9.1/mizani.egg-info/SOURCES.txt` & `mizani-0.9.2/mizani.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/pyproject.toml` & `mizani-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/tools/build_theme.sh` & `mizani-0.9.2/tools/build_theme.sh`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/tools/gha_check_semver.py` & `mizani-0.9.2/tools/gha_check_semver.py`

 * *Files identical despite different names*

### Comparing `mizani-0.9.1/tools/release-checklist.md` & `mizani-0.9.2/tools/release-checklist.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,29 +93,27 @@
 
   </details>
 
 - [ ] Create conda release
 
   <details>
 
-  ```sh
-  sha256sum dist/*.tar.gz
-  # copy hash
-  ```
+
+  - [ ] Copy _SHA256 hash_. Click view hashes, for the [Source Distribution](https://pypi.org/project/mizani/<VERSION>/#files) (`.tar.gz`).
 
   - [ ] Update [mizani-feedsock](https://github.com/conda-forge/mizani-feedstock)
 
     ```sh
     cd ../mizani-feestock
     git switch main
-    git pull upstream/main
-    git switch -c <VERSION>
+    git pull upstream main
+    git switch -c v<VERSION>
     nvim recipe/meta.yml
     git commit -am  "Version <VERSION>"
-    git push -u origin <VERSION>
+    git push -u origin v<VERSION>
     ```
   - [ ] Create a [PR](https://github.com/conda-forge/mizani-feedstock/pulls)
   - [ ] Complete PR (follow the steps and merge)
 
   </details>
 
 - [ ] Add [zenodo badge](https://zenodo.org/account/settings/github/repository/has2k1/mizani) to the changelog.
```

