# Comparing `tmp/yambs-1.5.0.tar.gz` & `tmp/yambs-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.5.0.tar", last modified: Wed May 24 06:57:25 2023, max compression
+gzip compressed data, was "yambs-1.6.0.tar", last modified: Thu May 25 00:21:23 2023, max compression
```

## Comparing `yambs-1.5.0.tar` & `yambs-1.6.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.663806 yambs-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 06:56:15.000000 yambs-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-24 06:57:25.663806 yambs-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-24 06:56:15.000000 yambs-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-24 06:56:15.000000 yambs-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:57:25.663806 yambs-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-24 06:56:15.000000 yambs-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-24 06:56:15.000000 yambs-1.5.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 06:56:15.000000 yambs-1.5.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.663806 yambs-1.5.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.663806 yambs-1.5.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.663806 yambs-1.5.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.663806 yambs-1.5.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-24 06:56:15.000000 yambs-1.5.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:57:25.659805 yambs-1.5.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 06:57:25.000000 yambs-1.5.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 00:20:12.000000 yambs-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-25 00:21:23.143940 yambs-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-25 00:20:12.000000 yambs-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 00:20:12.000000 yambs-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:21:23.143940 yambs-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 00:20:12.000000 yambs-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 00:20:12.000000 yambs-1.6.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 00:20:12.000000 yambs-1.6.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.5.0/LICENSE` & `yambs-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/PKG-INFO` & `yambs-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.5.0
+Version: 1.6.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1636b2d12ea99ca0ac441dc6ffe246a7
+    hash=aa5f774861e316a941fdf5a8220d678d
     =====================================
 -->
 
-# yambs ([1.5.0](https://pypi.org/project/yambs/))
+# yambs ([1.6.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.5.0/README.md` & `yambs-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1636b2d12ea99ca0ac441dc6ffe246a7
+    hash=aa5f774861e316a941fdf5a8220d678d
     =====================================
 -->
 
-# yambs ([1.5.0](https://pypi.org/project/yambs/))
+# yambs ([1.6.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.5.0/pyproject.toml` & `yambs-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.5.0"
+version = "1.6.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.5.0/setup.py` & `yambs-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/tests/test_entry.py` & `yambs-1.6.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/app.py` & `yambs-1.6.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/commands/all.py` & `yambs-1.6.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/commands/gen.py` & `yambs-1.6.0/yambs/commands/gen.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,32 +12,29 @@
 from rcmpy.watch import watch
 from rcmpy.watch.params import WatchParams
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from yambs import PKG_NAME
 from yambs.config import DEFAULT_CONFIG, load
+from yambs.environment import BuildEnvironment
 from yambs.generate import generate
 
 
 def gen_cmd(args: _Namespace) -> int:
     """Execute the gen command."""
 
-    config = load(path=args.config)
-
-    config.root = args.dir
-    config.root.mkdir(parents=True, exist_ok=True)
-
-    generate(config)
+    env = BuildEnvironment(load(path=args.config, root=args.dir))
+    generate(env)
 
     return (
         watch(
             WatchParams(
                 args.dir,
-                _Path(str(config.data["src_root"])),
+                _Path(str(env.config.data["src_root"])),
                 [
                     executable,
                     "-m",
                     PKG_NAME,
                     "-C",
                     str(args.dir),
                     "gen",
```

### Comparing `yambs-1.5.0/yambs/commands/uf2conv.py` & `yambs-1.6.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/config/__init__.py` & `yambs-1.6.0/yambs/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 from typing import Any, Dict, Iterator, List, Tuple
 
 # third-party
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
-from vcorelib.paths import Pathlike, find_file
+from vcorelib.paths import Pathlike, find_file, normalize
 
 # internal
 from yambs import PKG_NAME
 from yambs.config.board import Board
 from yambs.schemas import YambsDictCodec as _YambsDictCodec
 
 
 class Config(_YambsDictCodec, _BasicDictCodec):
     """The top-level configuration object for the package."""
 
     data: Dict[str, Any]
+    root: Path
     board_data: List[Board]
     boards_by_name: Dict[str, Board]
 
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
 
         self.data = data
@@ -65,24 +66,30 @@
         for inst, board in zip(self.board_data, self.data["boards"]):
             yield inst, board
 
 
 DEFAULT_CONFIG = f"{PKG_NAME}.yaml"
 
 
-def load(path: Pathlike = DEFAULT_CONFIG) -> Config:
+def load(path: Pathlike = DEFAULT_CONFIG, root: Pathlike = None) -> Config:
     """Load a configuration."""
 
     src_config = find_file(DEFAULT_CONFIG, package=PKG_NAME)
     assert src_config is not None
 
-    return Config.create(
+    result = Config.create(
         merge(
             _ARBITER.decode(
                 src_config, includes_key="includes", require_success=True
             ).data,
             _ARBITER.decode(path, includes_key="includes").data,
             # Always allow the project-specific configuration to override
             # package data.
             expect_overwrite=True,
         )
     )
+
+    if root is not None:
+        result.root = normalize(root)
+        result.root.mkdir(parents=True, exist_ok=True)
+
+    return result
```

### Comparing `yambs-1.5.0/yambs/config/board.py` & `yambs-1.6.0/yambs/config/board.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     name: str
     chip: Chip
     extra_cflags: List[str]
     targets: List[str]
     extra_dirs: List[str]
     apps: Dict[str, Path]
 
+    def __hash__(self) -> int:
+        """Get a hashing method for this instance."""
+        return hash(self.name)
+
     @property
     def build(self) -> Path:
         """Get a buld directory based on this board."""
         chip = self.chip
         return Path(
             chip.architecture.toolchain, chip.architecture.name, chip.cpu
         )
```

### Comparing `yambs-1.5.0/yambs/data/includes/chips.yaml` & `yambs-1.6.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/data/includes/infineon.yaml` & `yambs-1.6.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/data/includes/microchip.yaml` & `yambs-1.6.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/data/schemas/Chip.yaml` & `yambs-1.6.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/data/schemas/Config.yaml` & `yambs-1.6.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/data/templates/rules.ninja.j2` & `yambs-1.6.0/yambs/data/templates/rules.ninja.j2`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 tool = ${toolchain_prefix}{{cc}}
 
 rule cc
   depfile = $out.d
   deps = gcc
   command = $tool -MD -MF $out.d $cflags -c $in -o $out
 
+rule pio
+  command = pioasm -o c-sdk $in $out
+
 ldflags = $board_ldflags{% for flag in common_ldflags %} {{flag}}{% endfor %}
 
 
 rule link
   command = $tool $cflags $ldflags -Wl,-Map=$out.map $in -o $out
 
 rule bin
@@ -29,7 +32,8 @@
 rule dump
   command = ${toolchain_prefix}objdump -D $in > $out
 
 rule uf2
   command = mbs uf2conv $uf2conv_args -o $out $in
 
 build_dir = {{build_root}}/$toolchain/$architecture/$cpu
+generated_dir = $src_dir/generated
```

### Comparing `yambs-1.5.0/yambs/data/uf2families.json` & `yambs-1.6.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/entry.py` & `yambs-1.6.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/generate/__init__.py` & `yambs-1.6.0/yambs/generate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,54 +9,52 @@
 from datazen.templates import environment
 from jinja2 import FileSystemLoader
 from vcorelib.io import ARBITER
 from vcorelib.paths import resource
 
 # internal
 from yambs import PKG_NAME
-from yambs.config import Config
+from yambs.environment import BuildEnvironment
 from yambs.generate.architectures import generate as generate_architectures
 from yambs.generate.boards import generate as generate_boards
 from yambs.generate.chips import generate as generate_chips
 from yambs.generate.common import render_template
 from yambs.generate.toolchains import generate as generate_toolchains
 
 
-def generate(config: Config) -> None:
+def generate(env: BuildEnvironment) -> None:
     """Generate ninja files."""
 
     templates_dir = resource("templates", package=PKG_NAME)
     assert templates_dir is not None
 
     jinja = environment(
         loader=FileSystemLoader([templates_dir], followlinks=True)
     )
 
     # Render the top-level configuration. This is the only file that's
     # generated into the root directory.
-    render_template(jinja, config.root, "build.ninja", config.data)
-
-    ninja_root = config.directory("ninja_out")
+    render_template(jinja, env.config.root, "build.ninja", env.config.data)
 
     # Generate all other files.
     for gen in [
         generate_chips,
         generate_toolchains,
         generate_architectures,
         generate_boards,
     ]:
-        gen(jinja, ninja_root, config)
+        gen(jinja, env)
 
     board_apps: Dict[str, Any] = {}
 
     # Ensure that the build root directory is present in the full output paths
     # for built applications.
-    for board in config.board_data:
+    for board in env.config.board_data:
         board_apps[board.name] = {
-            short: str(config.build_root.joinpath(path))
+            short: str(env.config.build_root.joinpath(path))
             for short, path in board.apps.items()
         }
 
     ARBITER.encode(
-        ninja_root.joinpath("board_apps.json"),
+        env.ninja_root.joinpath("board_apps.json"),
         board_apps,
     )
```

### Comparing `yambs-1.5.0/yambs/generate/architectures.py` & `yambs-1.6.0/yambs/generate/architectures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 A module for generating architecture-related files.
 """
 
-# built-in
-from pathlib import Path
-
 # third-party
 from jinja2 import Environment
 
 # internal
-from yambs.config import Config
+from yambs.environment import BuildEnvironment
 from yambs.generate.common import render_template
 
 
-def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
+def generate(jinja: Environment, env: BuildEnvironment) -> None:
     """Generate architecture-related ninja files."""
 
-    for name, data in config.data["architectures"].items():
-        architectures_root = ninja_root.joinpath("architectures", name)
+    for name, data in env.config.data["architectures"].items():
+        architectures_root = env.ninja_root.joinpath("architectures", name)
         architectures_root.mkdir(parents=True, exist_ok=True)
 
         render_template(
             jinja,
             architectures_root,
             "architecture.ninja",
             data,
```

### Comparing `yambs-1.5.0/yambs/generate/boards.py` & `yambs-1.6.0/yambs/generate/boards.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 A module for generating board-related files.
 """
 
 # built-in
 from logging import getLogger
 from os import linesep
 from pathlib import Path
-from typing import Any, Dict, Set, TextIO, Tuple
+from typing import Any, Dict, Set, TextIO
 
 # third-party
 from jinja2 import Environment
 from vcorelib.paths import rel
 
 # internal
-from yambs.config import Config
 from yambs.config.board import Board
-from yambs.generate.common import is_source, render_template
-from yambs.generate.ninja import (
-    write_link_line,
-    write_phony,
-    write_source_line,
-)
+from yambs.environment import BuildEnvironment, SourceSets
+from yambs.generate.common import render_template
+from yambs.generate.ninja import write_link_lines, write_source_line
+from yambs.translation import is_source
 
 LOG = getLogger(__name__)
 
 
 def add_dir(
     stream: TextIO,
     paths: Set[Path],
@@ -38,22 +35,24 @@
     """Add a directory to set of paths."""
 
     LOG.debug("%s: checking '%s' for sources.", comment, path)
 
     if path.is_dir():
         stream.write(linesep + f"# {comment}." + linesep)
         for item in path.iterdir():
-            if is_source(item):
+            translator = is_source(item)
+            if translator is not None:
                 paths.add(
                     write_source_line(
                         stream,
                         item,
                         base,
                         current_sources,
                         board,
+                        translator,
                         board_specific=board_specific,
                     )
                 )
 
 
 def create_paths_dict(root: Path, board: Board) -> Dict[str, Any]:
     """Create paths based on common pathing conventions."""
@@ -69,103 +68,78 @@
     }
 
 
 def write_sources(
     stream: TextIO,
     board: Board,
     src_root: Path,
-    global_sources: Set[Path],
-) -> Tuple[Set[Path], Set[Path]]:
+    env: BuildEnvironment,
+) -> SourceSets:
     """Write the source-file manifest."""
 
     # Add regular sources.
     all_srcs: Set[Path] = set()
 
     for kind, path in create_paths_dict(src_root, board).items():
         add_dir(
             stream,
             all_srcs,
             path,
             f"{kind} sources",
             src_root,
-            global_sources,
+            env.global_sources,
             board,
         )
 
     # Add any extra sources this board specified.
     for extra in board.extra_dirs:
         add_dir(
             stream,
             all_srcs,
             src_root.joinpath("third-party", extra),
             "extra sources",
             src_root,
-            global_sources,
+            env.global_sources,
             board,
         )
 
     # Add application sources.
     app_srcs: Set[Path] = set()
     for kind, path in create_paths_dict(
         src_root.joinpath("apps"), board
     ).items():
         add_dir(
             stream,
             app_srcs,
             path,
             f"{kind} application sources",
             src_root,
-            global_sources,
+            env.global_sources,
             board,
             # Avoid having a redundant directory in the path when the source
             # directory is already the board-specific one.
             board_specific="boards" not in str(path),
         )
 
-    return all_srcs, app_srcs
+    # Populate board sources.
+    return env.set_board_sources(board, all_srcs, app_srcs)
 
 
-def generate(
-    jinja: Environment,
-    ninja_root: Path,
-    config: Config,
-) -> None:
+def generate(jinja: Environment, env: BuildEnvironment) -> None:
     """Generate board-related ninja files."""
 
     # Render the board manifest and rules file.
     for template in ["all.ninja", "rules.ninja"]:
-        render_template(jinja, ninja_root, template, config.data)
-
-    src_root = rel(config.src_root)
+        render_template(jinja, env.ninja_root, template, env.config.data)
 
-    # Keep track of all overall sources, so that no duplicate rules are
-    # generated.
-    global_sources: Set[Path] = set()
+    src_root = rel(env.config.src_root)
 
-    for board, raw_data in config.boards():
-        board_root = ninja_root.joinpath("boards", board.name)
+    for board, raw_data in env.config.boards():
+        board_root = env.ninja_root.joinpath("boards", board.name)
         board_root.mkdir(parents=True, exist_ok=True)
         render_template(jinja, board_root, "board.ninja", raw_data)
 
         # Perform source-file discovery.
         with board_root.joinpath("sources.ninja").open("w") as path_fd:
-            path_fd.write(f"src_dir = {config.data['src_root']}" + linesep)
-
-            all_srcs, app_srcs = write_sources(
-                path_fd, board, src_root, global_sources
-            )
-
-        LOG.info(
-            "(%s) Found %d sources and %d applications.",
-            board.name,
-            len(all_srcs),
-            len(app_srcs),
-        )
+            sources = write_sources(path_fd, board, src_root, env)
 
-        # Write the application manifest.
-        with board_root.joinpath("apps.ninja").open("w") as path_fd:
-            for app_src in app_srcs:
-                write_link_line(path_fd, app_src, all_srcs, src_root, board)
-
-            # Write the phony target.
-            path_fd.write("# A target to build all applications." + linesep)
-            write_phony(path_fd, app_srcs, src_root, board.name)
+        write_link_lines(board_root, src_root, board, sources)
```

### Comparing `yambs-1.5.0/yambs/generate/chips.py` & `yambs-1.6.0/yambs/generate/chips.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 A module for generating chip-related files.
 """
 
-# built-in
-from pathlib import Path
-
 # third-party
 from jinja2 import Environment
 
 # internal
-from yambs.config import Config
+from yambs.environment import BuildEnvironment
 from yambs.generate.common import render_template
 
 
-def generate(jinja: Environment, ninja_root: Path, config: Config) -> None:
+def generate(jinja: Environment, env: BuildEnvironment) -> None:
     """Generate chip-related ninja files."""
 
-    for name, data in config.data["chips"].items():
-        chips_root = ninja_root.joinpath("chips", name)
+    for name, data in env.config.data["chips"].items():
+        chips_root = env.ninja_root.joinpath("chips", name)
         chips_root.mkdir(parents=True, exist_ok=True)
 
         # Render chip files and linker scripts.
         render_template(
             jinja,
             chips_root,
             "chip.ninja",
```

### Comparing `yambs-1.5.0/yambs/generate/ninja.py` & `yambs-1.6.0/yambs/generate/ninja.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 # built-in
 from os import linesep
 from pathlib import Path
 from typing import Set, TextIO
 
 # internal
 from yambs.config.board import Board
+from yambs.environment import SourceSets
+from yambs.translation import SourceTranslator
 
 
 def write_source_line(
     stream: TextIO,
     source: Path,
     base: Path,
     current_sources: Set[Path],
     board: Board,
+    translator: SourceTranslator,
     board_specific: bool = False,
 ) -> Path:
     """Write a ninja configuration line for a source file."""
 
     dest = source
     if board_specific:
         dest = source.parent.joinpath(board.name, source.name)
@@ -29,31 +32,36 @@
 
     # Don't generate any duplicate compilation rules.
     if build_loc not in current_sources:
         current_sources.add(build_loc)
 
         stream.write(
             (
-                f"build $build_dir/"
-                f"{dest.relative_to(base).with_suffix('.o')}: "
-                f"cc $src_dir/{source.relative_to(base)}"
+                f"build {translator.output(dest.relative_to(base))}: "
+                f"{translator.rule} $src_dir/{source.relative_to(base)}"
             )
-            + linesep
         )
 
+        # Any regular source file depends on all of the boards generated
+        # depencencies.
+        if not translator.generated_header:
+            stream.write(" || ${board}_generated")
+
+        stream.write(linesep)
+
     return dest
 
 
 def write_continuation(stream: TextIO, offset: str) -> None:
     """Write a line continuation."""
     stream.write(" $" + linesep + offset)
 
 
 def write_link_line(
-    stream: TextIO, source: Path, all_srcs: Set[Path], base: Path, board: Board
+    stream: TextIO, source: Path, base: Path, board: Board, sources: SourceSets
 ) -> None:
     """
     Write a ninja configuration line for an application requiring linking.
     """
 
     source = source.relative_to(base)
 
@@ -63,17 +71,17 @@
     }
 
     elf = f"$build_dir/{by_suffix['elf']}"
     line = f"build {elf}: link "
     offset = " " * len(line)
     stream.write(line + f"$build_dir/{by_suffix['o']}")
 
-    for src in all_srcs:
+    for src, trans in sources.link_sources():
         write_continuation(stream, offset)
-        stream.write(f"$build_dir/{src.relative_to(base).with_suffix('.o')}")
+        stream.write(str(trans.output(src.relative_to(base))))
     stream.write(linesep)
 
     # Add lines for creating binaries.
     stream.write(f"build $build_dir/{by_suffix['bin']}: bin {elf}" + linesep)
 
     # Add an objdump target.
     stream.write(f"build $build_dir/{by_suffix['dump']}: dump {elf}" + linesep)
@@ -88,14 +96,53 @@
     stream.write(linesep + linesep)
 
     # Add this application to the board's data structure.
     out = by_suffix["elf"].with_suffix("")
     board.apps[str(out)] = board.build.joinpath(out)
 
 
+def write_generated_phony(
+    stream: TextIO, sources: SourceSets, src_root: Path
+) -> None:
+    """Write generated-file phony target."""
+
+    # Write generated-file phony target.
+    stream.write("# A target to generate additional headers." + linesep)
+    phony_line = "build ${board}_generated: phony"
+    offset = " " * (len(phony_line) + 1)
+
+    stream.write(phony_line)
+
+    implicit = list(sources.implicit_sources())
+    if implicit:
+        src, trans = implicit[0]
+        stream.write(f" {trans.output(src.relative_to(src_root))}")
+        for src, trans in implicit[1:]:
+            write_continuation(stream, offset)
+            stream.write(str(trans.output(src.relative_to(src_root))))
+    stream.write(linesep + linesep)
+
+
+def write_link_lines(
+    board_root: Path, src_root: Path, board: Board, sources: SourceSets
+) -> None:
+    """Write the application manifest and phony targets."""
+
+    # Write the application manifest.
+    with board_root.joinpath("apps.ninja").open("w") as path_fd:
+        for app_src in sources.apps:
+            write_link_line(path_fd, app_src, src_root, board, sources)
+
+        write_generated_phony(path_fd, sources, src_root)
+
+        # Write the phony target.
+        path_fd.write("# A target to build all applications." + linesep)
+        write_phony(path_fd, sources.apps, src_root, board.name)
+
+
 def write_phony(
     stream: TextIO, app_srcs: Set[Path], base: Path, board: str
 ) -> None:
     """Write the phony target."""
 
     phonies = [
         ("apps", ".bin"),
```

### Comparing `yambs-1.5.0/yambs/schemas.py` & `yambs-1.6.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs/uf2/__init__.py` & `yambs-1.6.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.5.0/yambs.egg-info/PKG-INFO` & `yambs-1.6.0/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.5.0
+Version: 1.6.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=1636b2d12ea99ca0ac441dc6ffe246a7
+    hash=aa5f774861e316a941fdf5a8220d678d
     =====================================
 -->
 
-# yambs ([1.5.0](https://pypi.org/project/yambs/))
+# yambs ([1.6.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.5.0/yambs.egg-info/SOURCES.txt` & `yambs-1.6.0/yambs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 yambs/data/templates/architecture.ninja.j2
 yambs/data/templates/board.ninja.j2
 yambs/data/templates/build.ninja.j2
 yambs/data/templates/chip.ld.j2
 yambs/data/templates/chip.ninja.j2
 yambs/data/templates/rules.ninja.j2
 yambs/data/templates/toolchain.ninja.j2
+yambs/environment/__init__.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
 yambs/generate/ninja.py
 yambs/generate/toolchains.py
+yambs/translation/__init__.py
 yambs/uf2/__init__.py
```

