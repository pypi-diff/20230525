# Comparing `tmp/aiidalab-23.3.0.tar.gz` & `tmp/aiidalab-23.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab-23.3.0.tar", last modified: Fri Mar 17 13:20:32 2023, max compression
+gzip compressed data, was "aiidalab-23.3.1.tar", last modified: Thu May 25 15:31:35 2023, max compression
```

## Comparing `aiidalab-23.3.0.tar` & `aiidalab-23.3.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 13:20:19.000000 aiidalab-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-17 13:20:19.000000 aiidalab-23.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-17 13:20:32.622447 aiidalab-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-17 13:20:19.000000 aiidalab-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.614447 aiidalab-23.3.0/aiidalab/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35804 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/git_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.618447 aiidalab-23.3.0/aiidalab/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/apps_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.618447 aiidalab-23.3.0/aiidalab/registry/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/app.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/apps.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/apps_index.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/categories.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/environment.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/schemas/metadata.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.614447 aiidalab-23.3.0/aiidalab/registry/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.618447 aiidalab-23.3.0/aiidalab/registry/static/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/api/openapi-v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.618447 aiidalab-23.3.0/aiidalab/registry/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/aiidalab/registry/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/static/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   145281 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/static/gotobutton.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/aiidalab/registry/static/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/static/img/aiidalab_stacked.png
--rw-r--r--   0 runner    (1001) docker     (123)   103940 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/static/static/img/aiidalab_wide.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/template_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/aiidalab/registry/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/app_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/app_page_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/index_base.html
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/registry/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-03-17 13:20:19.000000 aiidalab-23.3.0/aiidalab/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.618447 aiidalab-23.3.0/aiidalab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 13:20:32.000000 aiidalab-23.3.0/aiidalab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.614447 aiidalab-23.3.0/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 13:20:19.000000 aiidalab-23.3.0/jupyter-config/jupyter_notebook_config.d/aiidalab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.614447 aiidalab-23.3.0/jupyter-config/nbconfig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:20:32.622447 aiidalab-23.3.0/jupyter-config/nbconfig/notebook.d/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-17 13:20:19.000000 aiidalab-23.3.0/jupyter-config/nbconfig/notebook.d/aiidalab.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-17 13:20:19.000000 aiidalab-23.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-17 13:20:32.622447 aiidalab-23.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-17 13:20:19.000000 aiidalab-23.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 15:31:26.000000 aiidalab-23.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-25 15:31:26.000000 aiidalab-23.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-25 15:31:35.356939 aiidalab-23.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-25 15:31:26.000000 aiidalab-23.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35801 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/git_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/apps_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab/registry/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/app.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/apps.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/apps_index.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/categories.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/environment.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/schemas/metadata.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.348939 aiidalab-23.3.1/aiidalab/registry/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab/registry/static/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/api/openapi-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab/registry/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/aiidalab/registry/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/static/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   145281 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/static/gotobutton.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/aiidalab/registry/static/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/static/img/aiidalab_stacked.png
+-rw-r--r--   0 runner    (1001) docker     (123)   103940 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/static/static/img/aiidalab_wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/template_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/aiidalab/registry/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/app_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/app_page_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/index_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/registry/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-25 15:31:26.000000 aiidalab-23.3.1/aiidalab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.352939 aiidalab-23.3.1/aiidalab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:31:35.000000 aiidalab-23.3.1/aiidalab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.348939 aiidalab-23.3.1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/jupyter-config/jupyter_notebook_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 15:31:26.000000 aiidalab-23.3.1/jupyter-config/jupyter_notebook_config.d/aiidalab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.348939 aiidalab-23.3.1/jupyter-config/nbconfig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:31:35.356939 aiidalab-23.3.1/jupyter-config/nbconfig/notebook.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 15:31:26.000000 aiidalab-23.3.1/jupyter-config/nbconfig/notebook.d/aiidalab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 15:31:26.000000 aiidalab-23.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 15:31:35.356939 aiidalab-23.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 15:31:26.000000 aiidalab-23.3.1/setup.py
```

### Comparing `aiidalab-23.3.0/LICENSE` & `aiidalab-23.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/MANIFEST.in` & `aiidalab-23.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/PKG-INFO` & `aiidalab-23.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aiidalab
-Version: 23.3.0
+Version: 23.3.1
 Summary: Implements core functions of AiiDAlab.
 Home-page: https://github.com/aiidalab/aiidalab
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/aiidalab/badge/)](https://aiidalab.readthedocs.io/)
 [![codecov](https://codecov.io/gh/aiidalab/aiidalab/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidalab/aiidalab)
```

### Comparing `aiidalab-23.3.0/README.md` & `aiidalab-23.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/__main__.py` & `aiidalab-23.3.1/aiidalab/__main__.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/app.py` & `aiidalab-23.3.1/aiidalab/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,14 @@
         Arguments:
             prereleases (Bool):
                 Set to True to include available preleases. Defaults to False.
         Returns:
             AppRemoteUpdateStatus
         """
         if self.is_installed():
-
             # Check whether app is registered.
             if self.is_registered() is None:
                 return AppRemoteUpdateStatus.CANNOT_REACH_REGISTRY
 
             if self.is_registered() is False:
                 return AppRemoteUpdateStatus.NOT_REGISTERED
 
@@ -436,26 +435,24 @@
         if path.is_dir():
             shutil.copytree(this_or_only_subdir(path), self.path)
         else:
             with tempfile.TemporaryDirectory() as tmp_dir:
                 with tarfile.open(path) as tar_file:
 
                     def is_within_directory(directory, target):
-
                         abs_directory = os.path.abspath(directory)
                         abs_target = os.path.abspath(target)
 
                         prefix = os.path.commonprefix([abs_directory, abs_target])
 
                         return prefix == abs_directory
 
                     def safe_extract(
                         tar, path=".", members=None, *, numeric_owner=False
                     ):
-
                         for member in tar.getmembers():
                             member_path = os.path.join(path, member.name)
                             if not is_within_directory(path, member_path):
                                 raise Exception("Attempted Path Traversal in Tar File")
 
                         tar.extractall(path, members, numeric_owner=numeric_owner)
```

### Comparing `aiidalab-23.3.0/aiidalab/config.py` & `aiidalab-23.3.1/aiidalab/config.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/environment.py` & `aiidalab-23.3.1/aiidalab/environment.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/fetch.py` & `aiidalab-23.3.1/aiidalab/fetch.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/git_util.py` & `aiidalab-23.3.1/aiidalab/git_util.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/metadata.py` & `aiidalab-23.3.1/aiidalab/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     categories: list[str] = field(default_factory=list)
     version: None | str = None
 
     _search_dirs = (".aiidalab", "./")
 
     @staticmethod
     def _parse(path):
-
         try:
             return {
                 key: value
                 for key, value in _parse_setup_cfg(
                     path.joinpath("setup.cfg").read_text()
                 )
                 if value is not None
```

### Comparing `aiidalab-23.3.0/aiidalab/registry/api.py` & `aiidalab-23.3.1/aiidalab/registry/api.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/apps_index.py` & `aiidalab-23.3.1/aiidalab/registry/apps_index.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/core.py` & `aiidalab-23.3.1/aiidalab/registry/core.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/html.py` & `aiidalab-23.3.1/aiidalab/registry/html.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/releases.py` & `aiidalab-23.3.1/aiidalab/registry/releases.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,23 +26,82 @@
     parsed_url = urlsplit(url)
     if "@" in parsed_url.path:
         path, release_line = parsed_url.path.rsplit("@", 1)
         return urlunsplit(parsed_url._replace(path=path)), release_line
     return url, None
 
 
-def _get_release_commits(repo, release_line):
+def _get_tags(repo: GitRepo, branch: str, rev_selection: str):
+    """Get all tags for given revision selection of a branch.
+
+    :param repo: Git repository object.
+    :param branch: Branch name.
+    :param rev_selection: Revision selection, the format is described
+        in https://git-scm.com/docs/git-rev-list
+    """
+    # While the git rev-list command supports listing revisions for a
+    # single ref, in this context we only support rev selections for a
+    # range, not for individual refs.
+    if ".." not in rev_selection:
+        raise ValueError(
+            "The rev_selection '{rev_selection}' must specify a range, "
+            "that means must contain the range operator '..'."
+        )
+
+    # Incomplete revision selections such as `@main:v1..` must be expanded to
+    # `@main:v1..main`. Therefore, we first determine the branch ref for the
+    # given rev:
+    for ref in [f"refs/heads/{branch}", f"refs/remotes/origin/{branch}"]:
+        if ref.encode() in repo.refs:
+            break
+    else:
+        raise RuntimeError(f"Revision '{branch}' not a valid branch name.")
+
+    # Transform a potentially incomplete rev_selection into one that
+    # contains the branch ref. For example `v1..` is expanded to
+    # `v1..{ref}`, where `{ref}` is replaced with the actual reference.
+    start, _, stop = rev_selection.rpartition("..")
+    selected_commits = repo.rev_list(f"{start or ref}..{stop or ref}")
+
+    for tag in repo.get_merged_tags(branch):
+        commit = repo.get_commit_for_tag(tag)
+        if commit in selected_commits:
+            yield tag, commit
+
+
+def _get_release_commits(repo: GitRepo, release_line: str):
+    """Get the commits for a release line.
+
+    :param repo: Git repository object.
+    :param release_line: support standard git revision selection syntax to further
+        reduce the selected commits on a release line. For example, @main:v1.0.0.. means “select all tagged commits on the main branch after commit tagged with v1.0.0”.
+    """
     match = re.match(RELEASE_LINE_PATTERN, release_line)
 
     if not match:
         raise ValueError(f"Invalid release line specification: {release_line}")
 
     rev = match.groupdict()["rev"] or repo.get_current_branch()
 
-    if match.groupdict()["rev_selection"] is None:
+    if match.groupdict()["rev"] == "*":
+        # loop over all remote branches and yield the tags for the commits
+
+        tags = set()
+        for branch in repo.refs.as_dict(b"refs/remotes/origin/").keys():
+            rev = branch.decode()
+            rev_selection = match.groupdict()["rev_selection"]
+
+            for tag, commit in _get_tags(repo, rev, rev_selection):
+                if tag not in tags:
+                    tags.add(tag)
+                    yield tag, commit
+
+        return
+
+    elif match.groupdict()["rev_selection"] is None:
         # No rev_selection means to select this and only this specific
         # revision.  For example: '@main' means, simply checkout 'main' (could
         # be a branch or a tag, however branches have priority).
         for ref in [
             f"refs/heads/{rev}",
             f"refs/remotes/origin/{rev}",
             f"refs/tags/{rev}",
@@ -56,42 +115,16 @@
     elif match.groupdict()["rev_selection"]:
         # A rev selection is provided, we fetch the full rev list for the given
         # selection.  For example: '@main:v1..v2' means all commits from v1
         # (exclusive) to v2 (inclusive).
 
         rev_selection = match.groupdict()["rev_selection"]
 
-        # While the git rev-list command supports listing revisions for a
-        # single ref, in this context we only support rev selections for a
-        # range, not for individual refs.
-        if ".." not in match.groupdict()["rev_selection"]:
-            raise ValueError(
-                "The rev_selection '{rev_selection}' must specify a range, "
-                "that means must contain the range operator '..'."
-            )
-
-        # Incomplete revision selections such as `@main:v1..` must be expanded to
-        # `@main:v1..main`. Therefore, we first determine the branch ref for the
-        # given rev:
-        for ref in [f"refs/heads/{rev}", f"refs/remotes/origin/{rev}"]:
-            if ref.encode() in repo.refs:
-                break
-        else:
-            raise RuntimeError(f"Revision '{rev}' not a valid branch name.")
-
-        # Transform a potentially incomplete rev_selection into one that
-        # contains the branch ref. For example `v1..` is expanded to
-        # `v1..{ref}`, where `{ref}` is replaced with the actual reference.
-        start, _, stop = rev_selection.rpartition("..")
-        selected_commits = repo.rev_list(f"{start or ref}..{stop or ref}")
-
-        for tag in repo.get_merged_tags(rev):
-            commit = repo.get_commit_for_tag(tag)
-            if commit in selected_commits:
-                yield tag, commit
+        for tag, commit in _get_tags(repo, rev, rev_selection):
+            yield tag, commit
 
     else:
         # The rev selection is empty, select all tagged commits for the
         # selected revision.  For example: '@main:' means all tagged commits on
         # the main branch.
         for tag in repo.get_merged_tags(rev):
             yield tag, repo.get_commit_for_tag(tag)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/app.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/app.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/apps.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/apps.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/apps_index.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/apps_index.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/categories.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/categories.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/environment.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/environment.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/schemas/metadata.schema.json` & `aiidalab-23.3.1/aiidalab/registry/schemas/metadata.schema.json`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/api/openapi-v1.yaml` & `aiidalab-23.3.1/aiidalab/registry/static/api/openapi-v1.yaml`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/static/css/style.css` & `aiidalab-23.3.1/aiidalab/registry/static/static/css/style.css`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/static/favicon.png` & `aiidalab-23.3.1/aiidalab/registry/static/static/favicon.png`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/static/gotobutton.svg` & `aiidalab-23.3.1/aiidalab/registry/static/static/gotobutton.svg`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/static/img/aiidalab_stacked.png` & `aiidalab-23.3.1/aiidalab/registry/static/static/img/aiidalab_stacked.png`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/static/static/img/aiidalab_wide.png` & `aiidalab-23.3.1/aiidalab/registry/static/static/img/aiidalab_wide.png`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/templates/app_page_base.html` & `aiidalab-23.3.1/aiidalab/registry/templates/app_page_base.html`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/templates/base.html` & `aiidalab-23.3.1/aiidalab/registry/templates/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!doctype html>
 
-{% set app_registry_url = "http://aiidateam.github.io/aiida-registry" %}
-{% set aiidalab_url = "https://www.materialscloud.org/aiidalab" %}
+{% set app_registry_url = "https://aiidalab.github.io/aiidalab-registry/" %}
+{% set aiidalab_url = "https://www.aiidalab.net/" %}
 
 <html lang="en">
 
 <head>
     <meta charset="utf-8">
 
     <title>{{title}}</title>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
- {% set app_registry_url = "http://aiidateam.github.io/aiida-registry" %} {%
-set aiidalab_url = "https://www.materialscloud.org/aiidalab" %}
+ {% set app_registry_url = "https://aiidalab.github.io/aiidalab-registry/" %}
+{% set aiidalab_url = "https://www.aiidalab.net/" %}
 
  {% block css %}
 
  {% endblock css %}
 {% block header %}
 ****** AiiDAlab application registry ******
  {% endblock header %}
```

### Comparing `aiidalab-23.3.0/aiidalab/registry/templates/index_base.html` & `aiidalab-23.3.1/aiidalab/registry/templates/index_base.html`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/util.py` & `aiidalab-23.3.1/aiidalab/registry/util.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab/registry/web.py` & `aiidalab-23.3.1/aiidalab/registry/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from .core import AppRegistryData, AppRegistrySchemas
 from .html import build_html
 
 logger = logging.getLogger(__name__)
 
 
 def copy_static_tree_from_path(base_path, static_path):
-
     for root, _, files in os.walk(static_path):
         # Create directory
         base_path.joinpath(Path(root).relative_to(static_path)).mkdir(
             parents=True, exist_ok=True
         )
 
         # Copy all files
```

### Comparing `aiidalab-23.3.0/aiidalab/registry/yaml.py` & `aiidalab-23.3.1/aiidalab/registry/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import requests
 from ruamel.yaml import YAML
 
 REQUESTS = cachecontrol.CacheControl(requests.Session())
 
 
 class JsonYamlLoader(jsonref.JsonLoader):
-
     safe_yaml = YAML(typ="safe")
 
     def __call__(self, uri, **kwargs):
         uri_split = urlsplit(uri)
         if Path(uri_split.path).suffix in (".yml", ".yaml"):
             if uri_split.scheme == "file":
                 content = Path(uri_split.path).read_bytes()
```

### Comparing `aiidalab-23.3.0/aiidalab/utils.py` & `aiidalab-23.3.1/aiidalab/utils.py`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab.egg-info/PKG-INFO` & `aiidalab-23.3.1/aiidalab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aiidalab
-Version: 23.3.0
+Version: 23.3.1
 Summary: Implements core functions of AiiDAlab.
 Home-page: https://github.com/aiidalab/aiidalab
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/aiidalab/badge/)](https://aiidalab.readthedocs.io/)
 [![codecov](https://codecov.io/gh/aiidalab/aiidalab/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidalab/aiidalab)
```

### Comparing `aiidalab-23.3.0/aiidalab.egg-info/SOURCES.txt` & `aiidalab-23.3.1/aiidalab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/aiidalab.egg-info/requires.txt` & `aiidalab-23.3.1/aiidalab.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aiidalab-23.3.0/setup.cfg` & `aiidalab-23.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	requests-mock~=1.8
 	ruamel.yaml~=0.16
 	tabulate~=0.8
 	toml~=0.10
 	traitlets~=5.0
 	urllib3~=1.24
 	watchdog~=2.3
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 zip_safe = False
 
 [options.entry_points]
 console_scripts = 
 	aiidalab = aiidalab.__main__:cli
 
@@ -103,15 +103,15 @@
 disallow_untyped_defs = False
 disallow_untyped_calls = False
 disallow_incomplete_defs = False
 warn_return_any = False
 warn_unused_ignores = False
 
 [bumpver]
-current_version = "v23.03.0"
+current_version = "v23.03.1"
 version_pattern = "v0Y.0M.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

