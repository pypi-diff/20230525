# Comparing `tmp/chalkpy-2.3.9.tar.gz` & `tmp/chalkpy-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalkpy-2.3.9.tar", last modified: Mon May 15 22:35:46 2023, max compression
+gzip compressed data, was "chalkpy-2.4.0.tar", last modified: Thu May 25 02:33:58 2023, max compression
```

## Comparing `chalkpy-2.3.9.tar` & `chalkpy-2.4.0.tar`

### file list

```diff
@@ -1,935 +1,939 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.776944 chalkpy-2.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 22:35:27.000000 chalkpy-2.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-15 22:35:46.776944 chalkpy-2.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-15 22:35:27.000000 chalkpy-2.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.696943 chalkpy-2.3.9/chalk/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.696943 chalkpy-2.3.9/chalk/_autosql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_autosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_autosql/autosql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.696943 chalkpy-2.3.9/chalk/_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/Chart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/charts_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/charts_enums_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/charts_series_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_monitoring/gql_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.696943 chalkpy-2.3.9/chalk/_reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.696943 chalkpy-2.3.9/chalk/_reporting/rich/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/rich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/rich/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/rich/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_reporting/rich/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_validation/feature_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/client/
--rw-r--r--   0 runner    (1001) docker     (123)    42717 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48304 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/client/client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/client/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/clogging/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/clogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/clogging/chalk_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/config/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/config/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/df/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/df/ChalkDataFrameImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/df/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_1/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_10/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_100/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_100/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_101/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_102/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_102/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_102/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.700943 chalkpy-2.3.9/chalk/feature_n/feature_103/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_103/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_103/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_104/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_104/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_104/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_105/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_105/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_105/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_106/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_106/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_106/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_107/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_107/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_107/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_108/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_108/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_108/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_109/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_109/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_11/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_110/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_110/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_111/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_111/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_111/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_112/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_112/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_112/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_113/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_113/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_113/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_114/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_115/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_115/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_115/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_116/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_116/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_116/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_117/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_117/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.704943 chalkpy-2.3.9/chalk/feature_n/feature_118/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_118/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_118/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_119/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_119/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_12/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_120/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_120/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_121/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_121/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_121/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_122/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_123/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_123/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_124/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_124/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_124/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_125/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_126/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_126/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_126/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_127/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_127/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_127/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_128/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_128/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_128/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_129/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_129/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_129/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_13/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_130/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_130/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_131/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_131/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.708943 chalkpy-2.3.9/chalk/feature_n/feature_132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_132/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_133/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_133/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_133/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_134/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_134/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_134/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_135/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_135/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_135/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_136/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_136/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_136/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_137/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_137/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_137/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_138/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_138/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_138/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_139/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_139/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_139/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_14/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_14/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_140/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_140/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_141/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_141/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_142/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_142/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_142/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_143/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_143/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_143/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_144/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_144/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_144/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_145/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_145/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_145/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_146/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_146/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_146/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.712943 chalkpy-2.3.9/chalk/feature_n/feature_147/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_147/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_147/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_148/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_148/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_148/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_149/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_149/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_149/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_15/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_150/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_150/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_151/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_151/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_152/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_152/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_153/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_153/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_153/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_154/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_154/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_154/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_155/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_155/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_155/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_156/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_156/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_156/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_157/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_157/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_157/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_158/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_158/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_158/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_159/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_159/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_159/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_16/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_16/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_160/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_161/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_161/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_161/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.716943 chalkpy-2.3.9/chalk/feature_n/feature_162/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_162/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_162/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_163/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_163/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_163/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_164/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_164/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_164/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_165/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_165/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_165/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_166/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_166/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_167/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_167/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_167/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_168/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_168/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_168/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_169/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_169/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_169/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_17/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_17/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_170/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_170/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_170/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_171/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_171/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_171/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_172/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_172/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_172/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_173/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_173/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_173/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_174/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_174/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_174/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_175/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_175/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_175/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_176/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_176/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_176/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.720943 chalkpy-2.3.9/chalk/feature_n/feature_177/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_177/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_177/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_178/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_178/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_178/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_179/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_179/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_179/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_18/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_180/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_180/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_180/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_181/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_181/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_182/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_182/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_182/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_183/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_183/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_183/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_184/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_184/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_184/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_185/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_185/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_185/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_186/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_186/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_186/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_187/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_187/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_187/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_188/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_188/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_188/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_189/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_189/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_189/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_19/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_19/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_19/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_190/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_190/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_190/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.724943 chalkpy-2.3.9/chalk/feature_n/feature_191/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_191/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_191/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_192/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_192/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_192/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_193/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_193/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_193/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_194/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_194/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_194/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_195/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_195/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_195/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_196/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_196/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_197/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_197/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_197/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_198/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_198/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_198/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_199/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_199/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_199/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_2/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_20/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_200/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_200/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_201/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_201/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_201/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_202/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_202/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_202/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_203/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_203/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_203/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_204/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_204/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_204/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.728943 chalkpy-2.3.9/chalk/feature_n/feature_205/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_205/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_206/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_206/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_206/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_207/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_207/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_207/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_208/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_208/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_208/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_209/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_21/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_210/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_211/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_211/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_211/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_212/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_212/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_213/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_213/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_213/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_214/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_214/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_214/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_215/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_215/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_215/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_216/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_216/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_216/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_217/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_217/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_217/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_218/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_218/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_218/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_219/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_219/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.732943 chalkpy-2.3.9/chalk/feature_n/feature_22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_22/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_220/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_221/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_221/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_221/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_222/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_222/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_223/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_223/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_223/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_224/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_224/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_224/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_225/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_225/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_226/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_226/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_226/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_227/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_227/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_227/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_228/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_228/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_228/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_229/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_229/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_229/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_23/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_230/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_230/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_230/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_231/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_231/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_232/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_232/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_232/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_233/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_233/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.736943 chalkpy-2.3.9/chalk/feature_n/feature_234/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_234/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_234/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_235/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_235/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_235/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_236/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_236/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_236/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_237/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_237/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_237/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_238/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_238/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_238/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_239/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_239/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_239/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_24/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_24/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_240/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_240/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_241/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_241/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_241/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_242/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_242/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_242/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_243/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_243/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_243/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_244/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_244/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_244/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_245/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_245/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_246/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_246/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_246/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_247/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_247/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_247/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.740943 chalkpy-2.3.9/chalk/feature_n/feature_248/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_248/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_248/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_249/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_249/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_249/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_25/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_25/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_250/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_250/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_250/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_251/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_251/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_251/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_252/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_252/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_252/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_253/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_253/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_253/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_254/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_254/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_254/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_255/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_255/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_255/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_256/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_256/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_256/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_26/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_27/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_27/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_28/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_28/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_28/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_29/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_29/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_29/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_3/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_30/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_30/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_30/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_31/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.744943 chalkpy-2.3.9/chalk/feature_n/feature_32/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_32/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_33/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_34/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_34/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_35/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_35/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_35/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_36/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_36/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_37/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_37/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_38/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_38/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_39/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_39/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_39/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_4/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_40/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_40/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_41/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_41/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_41/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_42/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_42/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_43/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_43/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_43/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_44/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_44/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_44/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_45/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_45/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_45/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_46/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_46/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_46/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.748943 chalkpy-2.3.9/chalk/feature_n/feature_47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_47/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_48/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_48/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_48/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_49/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_49/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_49/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_5/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_50/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_50/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_51/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_51/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_51/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_52/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_52/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_52/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_53/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_53/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_54/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_54/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_54/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_55/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_55/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_55/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_56/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_56/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_57/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_57/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_58/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_58/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_58/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_59/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_59/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_59/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_6/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_60/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_60/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_60/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_61/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_61/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.752943 chalkpy-2.3.9/chalk/feature_n/feature_62/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_62/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_63/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_63/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_63/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_64/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_64/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_65/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_65/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_65/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_66/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_66/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_66/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_67/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_67/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_67/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_68/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_68/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_69/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_69/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_69/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_7/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_70/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_70/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_70/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_71/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_71/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_71/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_72/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_72/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_72/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_73/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_73/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_73/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_74/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_74/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_74/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_75/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_75/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_76/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_76/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_76/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.756943 chalkpy-2.3.9/chalk/feature_n/feature_77/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_77/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_77/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_78/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_78/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_78/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_79/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_79/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_79/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_8/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_80/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_80/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_81/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_81/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_81/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_82/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_82/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_83/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_83/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_83/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_84/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_84/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_84/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_85/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_85/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_85/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_86/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_86/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_87/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_87/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_87/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_88/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_88/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_88/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_89/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_89/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_9/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_90/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_90/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_90/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_91/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_91/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_91/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.760944 chalkpy-2.3.9/chalk/feature_n/feature_92/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_92/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_93/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_93/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_93/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_94/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_94/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_94/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_95/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_95/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_95/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_96/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_96/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_96/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_97/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_97/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_97/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_98/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_98/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_98/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/feature_n/feature_99/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/feature_n/feature_99/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.764943 chalkpy-2.3.9/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_chalkop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_class_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/features/_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/missing_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/_encoding/serialized_dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/features/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/dataframe/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    51213 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/dataframe/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/dataframe/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    30653 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/feature_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29431 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/feature_set_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/feature_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/feature_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/live_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/pseudofeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    64495 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/features/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/gitignore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/gitignore/gitignore_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/gitignore/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/integrations/named.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/parsed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/parsed/_graph_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/parsed/duplicate_input_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/parsed/json_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/parsed/user_types_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/serialization/parsed_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.768944 chalkpy-2.3.9/chalk/sink/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sink/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/sql/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/incremental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/sql/_internal/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/integrations/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24536 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/sql_file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/sql_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/_internal/string_chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/finalized_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/sql/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/streams/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/_file_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/_kafka_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/streams/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.772944 chalkpy-2.3.9/chalk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.776944 chalkpy-2.3.9/chalk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/annotation_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/cached_type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/environment_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/metaprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/missing_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-05-15 22:35:27.000000 chalkpy-2.3.9/chalk/utils/stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:46.776944 chalkpy-2.3.9/chalkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24078 2023-05-15 22:35:46.000000 chalkpy-2.3.9/chalkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-15 22:35:27.000000 chalkpy-2.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:35:46.776944 chalkpy-2.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-15 22:35:27.000000 chalkpy-2.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.265108 chalkpy-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-25 02:33:35.000000 chalkpy-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-25 02:33:58.265108 chalkpy-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-25 02:33:35.000000 chalkpy-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.193107 chalkpy-2.4.0/chalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.193107 chalkpy-2.4.0/chalk/_autosql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_autosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_autosql/autosql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/charts_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/charts_enums_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/charts_series_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_monitoring/gql_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/_reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/_reporting/rich/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/rich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/rich/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/rich/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_reporting/rich/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_validation/feature_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    42717 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32590 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/client/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/client/serialization/query_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/clogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/clogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/clogging/chalk_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/config/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/config/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/df/ChalkDataFrameImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/df/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/feature_n/
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.197107 chalkpy-2.4.0/chalk/feature_n/feature_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_1/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_10/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_100/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_100/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_100/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_101/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_102/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_102/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_102/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_103/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_103/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_103/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_104/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_104/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_104/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_105/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_105/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_105/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_106/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_106/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_106/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_107/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_107/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_107/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_108/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_108/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_108/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_109/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_109/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_11/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_110/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_111/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_111/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_111/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_112/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_112/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_112/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_113/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_113/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_113/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_114/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_115/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_115/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_115/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_116/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_116/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_116/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.201108 chalkpy-2.4.0/chalk/feature_n/feature_117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_117/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_118/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_118/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_118/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_119/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_119/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_12/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_120/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_120/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_121/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_121/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_122/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_123/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_123/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_124/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_124/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_124/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_125/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_126/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_126/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_126/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_127/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_127/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_127/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_128/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_128/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_128/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_129/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_129/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_129/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_13/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_130/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_131/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_131/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_132/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_133/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_133/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_133/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.205108 chalkpy-2.4.0/chalk/feature_n/feature_134/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_134/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_135/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_135/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_135/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_136/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_136/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_136/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_137/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_137/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_137/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_138/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_138/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_138/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_139/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_139/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_139/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_14/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_140/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_141/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_142/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_142/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_142/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_143/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_143/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_143/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_144/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_144/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_144/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_145/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_145/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_145/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_146/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_146/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_146/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_147/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_147/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_147/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_148/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_148/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_148/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_149/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_149/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_15/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_150/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.209107 chalkpy-2.4.0/chalk/feature_n/feature_151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_151/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_152/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_153/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_153/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_153/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_154/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_154/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_154/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_155/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_155/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_155/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_156/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_156/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_156/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_157/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_157/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_157/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_158/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_158/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_158/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_159/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_159/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_159/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_16/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_160/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_161/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_161/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_161/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_162/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_162/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_162/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_163/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_163/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_163/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_164/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_164/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_164/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_165/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_165/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_165/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_166/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_166/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_167/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_167/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_167/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_168/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_168/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_168/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.213107 chalkpy-2.4.0/chalk/feature_n/feature_169/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_169/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_169/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_17/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_170/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_170/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_170/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_171/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_171/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_171/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_172/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_172/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_172/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_173/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_173/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_173/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_174/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_174/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_174/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_175/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_175/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_175/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_176/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_176/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_176/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_177/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_177/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_177/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_178/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_178/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_178/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_179/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_179/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_179/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_18/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_180/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_180/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_180/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_181/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_181/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_182/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_182/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_182/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_183/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_183/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_183/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_184/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_184/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_184/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.217108 chalkpy-2.4.0/chalk/feature_n/feature_185/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_185/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_185/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_186/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_186/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_186/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_187/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_187/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_187/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_188/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_188/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_188/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_189/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_189/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_189/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_19/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_19/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_190/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_190/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_190/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_191/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_191/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_191/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_192/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_192/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_192/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_193/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_193/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_193/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_194/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_194/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_194/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_195/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_195/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_195/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_196/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_196/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_197/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_197/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_198/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_198/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_198/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_199/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_199/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_199/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_2/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_20/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_200/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_200/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.221108 chalkpy-2.4.0/chalk/feature_n/feature_201/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_201/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_201/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_202/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_202/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_202/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_203/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_203/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_203/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_204/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_204/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_204/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_205/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_205/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_206/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_206/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_206/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_207/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_207/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_207/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_208/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_208/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_208/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_209/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_21/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_210/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_211/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_211/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_211/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_212/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_213/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_213/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_213/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_214/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_214/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_214/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_215/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_215/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_215/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_216/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_216/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_216/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_217/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_217/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_217/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.225108 chalkpy-2.4.0/chalk/feature_n/feature_218/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_218/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_218/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_219/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_219/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_22/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_220/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_221/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_221/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_221/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_222/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_222/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_223/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_223/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_223/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_224/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_224/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_224/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_225/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_225/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_226/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_226/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_226/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_227/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_227/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_227/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_228/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_228/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_228/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_229/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_229/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_229/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_23/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_230/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_230/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_230/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_231/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_231/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_232/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_232/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.229108 chalkpy-2.4.0/chalk/feature_n/feature_233/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_233/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_234/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_234/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_234/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_235/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_235/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_235/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_236/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_236/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_236/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_237/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_237/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_237/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_238/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_238/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_238/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_239/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_239/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_239/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_24/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_24/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_240/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_241/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_241/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_241/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_242/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_242/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_242/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_243/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_243/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_243/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_244/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_244/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_244/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_245/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_245/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_245/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_246/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_246/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_246/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_247/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_247/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_247/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_248/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_248/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_248/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_249/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_249/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_249/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.233108 chalkpy-2.4.0/chalk/feature_n/feature_25/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_25/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_250/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_250/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_250/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_251/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_251/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_251/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_252/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_252/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_252/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_253/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_253/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_253/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_254/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_254/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_254/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_255/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_255/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_255/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_256/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_256/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_256/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_26/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_27/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_27/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_28/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_28/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_28/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_29/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_29/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_29/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_3/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_30/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_30/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_30/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_31/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_32/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_33/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_34/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_34/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.237108 chalkpy-2.4.0/chalk/feature_n/feature_35/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_35/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_35/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_36/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_36/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_37/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_37/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_38/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_38/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_39/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_39/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_39/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_4/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_40/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_40/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_41/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_41/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_41/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_42/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_43/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_43/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_43/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_44/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_44/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_44/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_45/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_45/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_45/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_46/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_46/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_46/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_47/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_48/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_48/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_48/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_49/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_49/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_49/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_5/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_50/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_50/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.241108 chalkpy-2.4.0/chalk/feature_n/feature_51/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_51/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_51/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_52/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_52/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_52/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_53/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_53/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_54/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_54/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_54/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_55/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_55/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_55/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_56/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_56/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_57/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_57/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_58/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_58/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_58/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_59/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_59/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_59/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_6/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_60/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_60/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_60/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_61/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_61/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_62/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_62/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_63/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_63/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_63/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_64/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_65/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_65/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_65/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_66/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_66/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_66/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_67/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_67/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_67/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_68/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.245108 chalkpy-2.4.0/chalk/feature_n/feature_69/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_69/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_69/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_7/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_70/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_70/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_70/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_71/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_71/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_71/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_72/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_72/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_72/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_73/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_73/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_73/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_74/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_74/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_74/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_75/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_75/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_76/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_76/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_76/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_77/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_77/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_77/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_78/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_78/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_78/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_79/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_79/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_79/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_8/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_80/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_80/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_81/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_81/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_81/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_82/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_83/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_83/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_83/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.249108 chalkpy-2.4.0/chalk/feature_n/feature_84/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_84/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_84/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_85/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_85/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_85/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_86/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_86/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_87/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_87/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_87/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_88/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_88/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_88/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_89/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_9/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_90/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_90/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_90/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_91/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_91/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_91/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_92/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_92/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_93/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_93/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_93/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_94/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_94/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_94/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_95/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_95/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_95/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_96/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_96/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_96/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_97/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_97/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_97/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_98/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_98/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_98/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.253108 chalkpy-2.4.0/chalk/feature_n/feature_99/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_99/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/feature_n/feature_99/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_chalkop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/features/_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/missing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/_encoding/serialized_dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/features/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/dataframe/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51407 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/dataframe/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/dataframe/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31044 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/feature_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30718 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/feature_set_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/feature_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/feature_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/live_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/pseudofeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69864 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/features/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/gitignore/gitignore_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/gitignore/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/integrations/named.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.257108 chalkpy-2.4.0/chalk/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/parsed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/parsed/_graph_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/parsed/duplicate_input_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/parsed/json_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/parsed/user_types_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/serialization/parsed_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sink/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/sql/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/sql/_internal/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/integrations/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24536 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/sql_file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/sql_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/_internal/string_chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/finalized_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/sql/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.261108 chalkpy-2.4.0/chalk/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/_kafka_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/_kinesis_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/streams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.265108 chalkpy-2.4.0/chalk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.265108 chalkpy-2.4.0/chalk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/annotation_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/cached_type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/environment_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/log_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/metaprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/missing_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-05-25 02:33:35.000000 chalkpy-2.4.0/chalk/utils/stubgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:33:58.265108 chalkpy-2.4.0/chalkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24200 2023-05-25 02:33:58.000000 chalkpy-2.4.0/chalkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-25 02:33:35.000000 chalkpy-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:33:58.265108 chalkpy-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 02:33:35.000000 chalkpy-2.4.0/setup.py
```

### Comparing `chalkpy-2.3.9/PKG-INFO` & `chalkpy-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalkpy
-Version: 2.3.9
+Version: 2.4.0
 Summary: Python SDK for Chalk
 Author: Chalk AI, Inc.
 Project-URL: homepage, https://chalk.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chalkpy-2.3.9/README.md` & `chalkpy-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/__init__.py` & `chalkpy-2.4.0/chalk/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_autosql/autosql.py` & `chalkpy-2.4.0/chalk/_autosql/autosql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_monitoring/Chart.py` & `chalkpy-2.4.0/chalk/_monitoring/Chart.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_monitoring/charts_codegen.py` & `chalkpy-2.4.0/chalk/_monitoring/charts_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_monitoring/charts_enums_codegen.py` & `chalkpy-2.4.0/chalk/_monitoring/charts_enums_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_monitoring/charts_series_base.py` & `chalkpy-2.4.0/chalk/_monitoring/charts_series_base.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_monitoring/gql_conversion.py` & `chalkpy-2.4.0/chalk/_monitoring/gql_conversion.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_reporting/models.py` & `chalkpy-2.4.0/chalk/_reporting/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_reporting/progress.py` & `chalkpy-2.4.0/chalk/_reporting/progress.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_reporting/rich/live.py` & `chalkpy-2.4.0/chalk/_reporting/rich/live.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/_validation/validation.py` & `chalkpy-2.4.0/chalk/_validation/validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/cli.py` & `chalkpy-2.4.0/chalk/cli.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/client/__init__.py` & `chalkpy-2.4.0/chalk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/client/client_impl.py` & `chalkpy-2.4.0/chalk/client/client_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,30 @@
     FeatureDropResponse,
     FeatureObservationDeletionRequest,
     FeatureObservationDeletionResponse,
     FeatureResult,
     GetOfflineQueryJobResponse,
     OfflineQueryContext,
     OfflineQueryInput,
+    OnlineQuery,
     OnlineQueryContext,
     OnlineQueryManyRequest,
     OnlineQueryRequest,
     OnlineQueryResponse,
     ResolverRunResponse,
     TriggerResolverRunRequest,
     UpdateGraphEntityResponse,
     WhoAmIResponse,
 )
+from chalk.client.serialization.query_serialization import (
+    MAGIC_STR,
+    MULTI_QUERY_MAGIC_STR,
+    _decode_multi_query_responses,
+    _write_query_to_buffer,
+)
 from chalk.config.auth_config import load_token
 from chalk.config.project_config import load_project_config
 from chalk.features import DataFrame, Feature, FeatureNotFoundException, FeatureWrapper, ensure_feature, unwrap_feature
 from chalk.features._encoding.inputs import recursive_encode
 from chalk.features.pseudofeatures import CHALK_TS_FEATURE
 from chalk.features.tag import BranchId, EnvironmentId
 from chalk.utils import notebook
@@ -86,26 +93,26 @@
 _logger = get_logger(__name__)
 
 T = TypeVar("T")
 
 
 class _ChalkHTTPException(BaseModel):
     detail: str
-    trace: Optional[str]
+    trace: Optional[str] = None
     errors: Optional[List[ChalkError]] = None
 
 
 class _ChalkClientConfig(BaseModel):
     name: str
     client_id: str
     client_secret: str
     api_server: str
     query_server: str
-    active_environment: Optional[str]
-    branch: Optional[BranchId]
+    active_environment: Optional[str] = None
+    branch: Optional[BranchId] = None
 
 
 class _BranchDeploymentInfo(BaseModel):
     deployment_id: str
     created_at: datetime
 
 
@@ -185,46 +192,90 @@
         data: List[FeatureResult],
         errors: List[ChalkError],
         warnings: List[str],
     ):
         self.data = data
         self.errors = errors
         self.warnings = warnings
+        import math
+
         for d in self.data:
+            if isinstance(d.value, float) and math.isnan(d.value):
+                d.value = None
             if d.value is not None:
                 try:
                     f = Feature.from_root_fqn(d.field)
                 except FeatureNotFoundException:
                     self.warnings.append(
                         f"Return data {d.field}:{d.value} cannot be decoded. Attempting to JSON decode"
                     )
                 else:
                     d.value = f.converter.from_json_to_rich(d.value)
 
         self._values = {d.field: d for d in self.data}
 
     def _df_repr(self):
-        if self.errors:
-            info = [vars(x) for x in self.errors]
-        else:
-            info = []
-            for x in self.data:
-                if isinstance(x.value, pd.DataFrame):
-                    info.append({"Feature": x.field, "Value": "No DataFrame Preview"})
-                elif isinstance(x.value, Enum):
-                    info.append({"Feature": x.field, "Value": x.value.value})
-                else:
-                    info.append({"Feature": x.field, "Value": x.value})
+        info = []
+        for x in self.data:
+            if isinstance(x.value, pd.DataFrame):
+                info.append({"Feature": x.field, "Value": "No DataFrame Preview"})
+            elif isinstance(x.value, Enum):
+                info.append({"Feature": x.field, "Value": x.value.value})
+            else:
+                info.append({"Feature": x.field, "Value": x.value})
         return info
 
     def __repr__(self) -> str:
-        return repr(pd.DataFrame(self._df_repr()))
+        lines = []
+        for e in self.errors:
+            nice_code = str(e.code.value).replace("_", " ").capitalize()
+            # {str(e.category.value).capitalize()}
+            lines.append(
+                f"### {nice_code}{e.feature and f' ({e.feature})' or ''}{e.resolver and f' ({e.resolver})' or ''}"
+            )
+            lines.append(e.message)
+            lines.append("")
+
+            metadata = {
+                "Exception Kind": e.exception and e.exception.kind,
+                "Exception Message": e.exception and e.exception.message,
+                "Stacktrace": e.exception and e.exception.stacktrace,
+            }
+            metadata = {k: v for k, v in metadata.items() if v is not None}
+            for k, v in metadata.items():
+                lines.append(f"*{k}*")
+                lines.append(f"")
+                lines.append(v)
+        errs = "\n".join(lines)
+
+        return repr(pd.DataFrame(self._df_repr())) + "\n" + errs
 
     def __str__(self):
-        return str(pd.DataFrame(self._df_repr()))
+        lines = []
+        for e in self.errors:
+            nice_code = str(e.code.value).replace("_", " ").capitalize()
+            # {str(e.category.value).capitalize()}
+            lines.append(
+                f"### {nice_code}{e.feature and f' ({e.feature})' or ''}{e.resolver and f' ({e.resolver})' or ''}"
+            )
+            lines.append(e.message)
+            lines.append("")
+
+            metadata = {
+                "Exception Kind": e.exception and e.exception.kind,
+                "Exception Message": e.exception and e.exception.message,
+                "Stacktrace": e.exception and e.exception.stacktrace,
+            }
+            metadata = {k: v for k, v in metadata.items() if v is not None}
+            for k, v in metadata.items():
+                lines.append(f"*{k}*")
+                lines.append(f"")
+                lines.append(v)
+        errs = "\n".join(lines)
+        return str(pd.DataFrame(self._df_repr())) + "\n" + errs
 
     def _repr_markdown_(self):
         lines = []
         if len(self.errors) > 0:
             lines.append(f"## {len(self.errors)} Errors")
             lines.append("")
             for e in self.errors:
@@ -243,17 +294,17 @@
                 }
                 metadata = {k: v for k, v in metadata.items() if v is not None}
                 for k, v in metadata.items():
                     lines.append(f"*{k}*")
                     lines.append(f"")
                     lines.append(v)
 
-        import polars as pl
-
         if len(self.data) > 0:
+            import polars as pl
+
             lines.append("")
             lines.append(f"## Features")
             lines.append("```")
             content = str(pl.DataFrame(self._df_repr()))
             split = content.split("\n")
             main = "\n".join(itertools.chain(split[1:3], split[5:]))
             lines.append(main)
@@ -267,17 +318,14 @@
 
     def get_feature_value(self, feature: Any) -> Optional[Any]:
         # Typing `feature` as Any, as the Features will be typed as the underlying datatypes, not as Feature
         v = self.get_feature(feature)
         return v and v.value
 
 
-MAGIC_STR = "chalk".encode("utf-8")
-
-
 class ChalkAPIClientImpl(ChalkClient):
     __name__ = "ChalkClient"
     __qualname__ = "chalk.client.ChalkClient"
 
     _latest_client: Optional[ChalkAPIClientImpl] = None
 
     def __repr__(self):
@@ -625,21 +673,93 @@
             response=OnlineQueryResponse,
             environment_override=environment,
             exception_cls=ChalkOnlineQueryException,
             preview_deployment_id=preview_deployment_id,
             branch=branch,
             metadata_request=False,
             extra_headers=extra_headers,
+            api_server_override=self._get_local_server_override(None),
         )
         return OnlineQueryResponseImpl(
             data=resp.data,
             errors=resp.errors or [],
             warnings=encoding_warnings,
         )
 
+    def multi_query(
+        self,
+        queries: list[OnlineQuery],
+        environment: Optional[EnvironmentId] = None,
+        preview_deployment_id: Optional[str] = None,
+        branch: Optional[BranchId] = None,
+        correlation_id: Optional[str] = None,
+        query_name: Optional[str] = None,
+        meta: Optional[Mapping[str, str]] = None,
+        use_feather: Optional[bool] = True,
+        compression: Optional[str] = "uncompressed",
+    ) -> OnlineQueryResponseImpl:
+        extra_headers = {}
+        if query_name is not None:
+            extra_headers["X-Chalk-Query-Name"] = query_name
+        if use_feather:
+            import pyarrow
+            import pyarrow.feather as feather
+
+            buffer = BytesIO()
+            buffer.write(MULTI_QUERY_MAGIC_STR)
+            for query in queries:
+                tags = query.tags
+                encoded_inputs = {str(k): v for k, v in query.input.items()}
+                outputs: List[str] = [str(feature) for feature in query.output]
+                request = OnlineQueryManyRequest(
+                    inputs=encoded_inputs,
+                    outputs=outputs,
+                    staleness={}
+                    if query.staleness is None
+                    else {ensure_feature(k).root_fqn: v for k, v in query.staleness.items()},
+                    context=OnlineQueryContext(
+                        environment=environment,
+                        tags=tags,
+                    ),
+                    deployment_id=preview_deployment_id,
+                    branch_id=branch,
+                    correlation_id=correlation_id,
+                    query_name=query_name,
+                    meta=meta,
+                )
+
+                _write_query_to_buffer(buffer, request, compression=compression)
+
+            buffer.seek(0)
+            resp = self._request(
+                method="POST",
+                uri="/v1/query/feather",
+                data=buffer.getvalue(),
+                json=None,
+                response=None,
+                environment_override=environment,
+                exception_cls=ChalkOnlineQueryException,
+                preview_deployment_id=preview_deployment_id,
+                branch=branch,
+                metadata_request=False,
+                extra_headers=extra_headers,
+            )
+
+            if resp.headers.get("Content-Type") == "application/octet-stream":
+                responses = _decode_multi_query_responses(resp.content)
+                return responses
+            else:
+                resp = OnlineQueryResponse(**resp.json())
+                return OnlineQueryResponseImpl(
+                    data=resp.data,
+                    errors=resp.errors or [],
+                    # warnings=encoding_warnings, # this seems to be a bogus var
+                    warnings=[],
+                )
+
     def query_many(
         self,
         input: Union[Mapping[FeatureReference, Sequence[Any]], Any],
         output: Sequence[FeatureReference],
         staleness: Optional[Mapping[FeatureReference, str]] = None,
         context: Optional[OnlineQueryContext] = None,  # Deprecated.
         environment: Optional[EnvironmentId] = None,
@@ -647,15 +767,14 @@
         preview_deployment_id: Optional[str] = None,
         branch: Optional[BranchId] = None,
         correlation_id: Optional[str] = None,
         query_name: Optional[str] = None,
         meta: Optional[Mapping[str, str]] = None,
         use_feather: Optional[bool] = True,
     ) -> OnlineQueryResponseImpl:
-
         extra_headers = {}
         if query_name is not None:
             extra_headers["X-Chalk-Query-Name"] = query_name
 
         environment = environment or (context and context.environment)
         tags = tags or (context and context.tags)
         # TODO: We're doing a lame encoding here b/c recursive_encode will treat our lists
@@ -678,22 +797,18 @@
             meta=meta,
         )
 
         if use_feather:
             import pyarrow
             import pyarrow.feather as feather
 
-            data = pyarrow.Table.from_pydict(encoded_inputs)
             buffer = BytesIO()
-            buffer.write(MAGIC_STR)
-            header = request.copy(exclude={"inputs"}).json()
-            header_bytes = header.encode("utf-8")
-            buffer.write(len(header_bytes).to_bytes(8, byteorder="big"))
-            buffer.write(header_bytes)
-            pyarrow.feather.write_feather(data, dest=buffer, compression="lz4")
+
+            buffer.write(MULTI_QUERY_MAGIC_STR)
+            _write_query_to_buffer(buffer, request)
 
             buffer.seek(0)
 
             resp = self._request(
                 method="POST",
                 uri="/v1/query/feather",
                 data=buffer.getvalue(),
@@ -704,15 +819,15 @@
                 preview_deployment_id=preview_deployment_id,
                 branch=branch,
                 metadata_request=False,
                 extra_headers=extra_headers,
             )
 
             if resp.headers.get("Content-Type") == "application/octet-stream":
-                return pyarrow.feather.read_table(source=BytesIO(resp.content))
+                return _decode_multi_query_responses(resp.content)[0]
             else:
                 resp = OnlineQueryResponse(**resp.json())
         else:
             branch = branch or self._config.branch
 
             resp = self._request(
                 method="POST",
@@ -1266,18 +1381,16 @@
                 json=None,
                 environment_override=None,
                 exception_cls=ChalkGetBatchReportException,
                 preview_deployment_id=None,
                 branch=_EMPTY,
                 operation_id=operation_id,
             )
-        except ChalkGetBatchReportException as e:
-            if "404" in e.full_message:  # Hack
-                return None
-            raise e
+        except Exception:
+            return None
 
         return response.report
 
     def _send_updated_entity(
         self, environment: Optional[EnvironmentId], pickled_entity: bytes
     ) -> UpdateGraphEntityResponse:
         resp = self._request(
```

### Comparing `chalkpy-2.3.9/chalk/client/dataset.py` & `chalkpy-2.4.0/chalk/client/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         if column_metadata is not None:
             col_name_set = {x.feature_fqn for x in column_metadata}
             ordered_cols: list[str] = []
             for c in df.columns:
                 if c not in col_name_set:
                     ordered_cols.append(c)
             for x in column_metadata:
-                if x.feature_fqn not in ordered_cols:
+                if x.feature_fqn not in ordered_cols and x.feature_fqn in df.columns:
                     ordered_cols.append(x.feature_fqn)
             df = df.select(ordered_cols)
 
         # Using an OrderedDict so the order will match the order the user set in the
         # output argument
         expected_cols: Dict[str, pl.Expr] = OrderedDict()
         id_col = pl.col(str(ID_FEATURE))
```

### Comparing `chalkpy-2.3.9/chalk/client/exc.py` & `chalkpy-2.4.0/chalk/client/exc.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/client/models.py` & `chalkpy-2.4.0/chalk/client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
+import dataclasses
 import uuid
 from datetime import datetime
 from enum import Enum, IntEnum
-from typing import TYPE_CHECKING, Any, Dict, List, Literal, Mapping, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Literal, Mapping, Optional, Sequence, Union
 
 import numpy as np
 from pydantic import BaseModel, Field, root_validator
 from typing_extensions import TypeAlias
 
 from chalk.features import Feature
 from chalk.features.resolver import Resolver
@@ -274,15 +275,15 @@
     value: Any  # Value should be a TJSON type
     """
     The value of the requested feature.
     If an error was encountered in resolving this feature,
     this field will be empty.
     """
 
-    pkey: Optional[Union[str, int]]
+    pkey: Optional[Union[str, int]] = None
     """The primary key of the resolved feature."""
 
     error: Optional[ChalkError] = None
     """
     The error code encountered in resolving this feature.
     If no error occurred, this field is empty.
     """
@@ -332,14 +333,22 @@
     correlation_id: Optional[str] = None
     query_name: Optional[str] = None
     deployment_id: Optional[str] = None
     branch_id: Optional[str] = None
     meta: Optional[Mapping[str, str]] = None
 
 
+@dataclasses.dataclass
+class OnlineQuery:
+    input: Union[Mapping[FeatureReference, Sequence[Any]], Any]
+    output: List[str]
+    staleness: Optional[Mapping[str, str]] = None
+    tags: Optional[List[str]] = None
+
+
 class OnlineQueryManyRequest(BaseModel):
     inputs: Mapping[str, List[Any]]
     outputs: List[str]
     staleness: Optional[Mapping[str, str]] = None
     context: Optional[OnlineQueryContext] = None
     include_meta: bool = True
     explain: bool = False
```

### Comparing `chalkpy-2.3.9/chalk/config/auth_config.py` & `chalkpy-2.4.0/chalk/config/auth_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/config/project_config.py` & `chalkpy-2.4.0/chalk/config/project_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/df/ast_parser.py` & `chalkpy-2.4.0/chalk/df/ast_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/__init__.py` & `chalkpy-2.4.0/chalk/feature_n/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/codegen.py` & `chalkpy-2.4.0/chalk/feature_n/codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_10/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_10/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_100/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_100/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_101/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_101/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_102/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_102/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_103/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_103/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_104/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_104/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_105/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_105/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_106/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_106/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_107/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_107/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_108/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_108/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_109/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_109/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_11/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_11/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_110/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_110/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_111/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_111/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_112/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_112/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_113/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_113/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_114/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_114/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_115/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_115/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_116/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_116/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_117/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_117/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_118/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_118/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_119/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_119/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_12/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_12/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_120/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_120/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_121/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_121/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_122/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_122/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_123/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_123/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_124/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_124/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_125/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_125/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_126/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_126/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_127/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_127/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_128/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_128/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_129/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_129/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_13/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_13/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_130/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_130/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_131/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_131/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_132/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_132/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_133/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_133/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_134/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_134/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_135/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_135/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_136/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_136/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_137/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_137/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_138/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_138/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_139/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_139/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_14/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_14/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_140/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_140/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_141/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_141/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_142/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_142/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_143/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_143/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_144/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_144/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_145/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_145/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_146/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_146/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_147/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_147/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_148/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_148/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_149/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_149/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_15/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_15/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_150/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_150/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_151/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_151/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_152/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_152/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_153/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_153/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_154/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_154/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_155/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_155/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_156/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_156/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_157/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_157/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_158/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_158/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_159/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_159/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_16/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_16/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_160/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_160/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_161/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_161/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_162/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_162/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_163/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_163/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_164/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_164/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_165/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_165/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_166/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_166/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_167/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_167/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_168/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_168/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_169/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_169/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_17/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_17/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_170/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_170/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_171/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_171/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_172/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_172/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_173/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_173/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_174/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_174/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_175/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_175/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_176/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_176/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_177/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_177/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_178/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_178/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_179/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_179/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_18/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_18/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_180/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_180/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_181/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_181/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_182/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_182/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_183/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_183/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_184/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_184/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_185/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_185/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_186/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_186/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_187/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_187/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_188/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_188/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_189/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_189/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_19/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_19/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_190/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_190/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_191/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_191/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_192/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_192/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_193/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_193/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_194/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_194/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_195/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_195/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_196/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_196/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_197/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_197/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_198/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_198/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_199/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_199/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_20/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_20/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_200/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_200/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_201/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_201/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_202/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_202/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_203/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_203/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_204/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_204/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_205/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_205/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_206/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_206/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_207/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_207/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_208/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_208/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_209/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_209/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_21/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_21/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_210/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_210/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_211/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_211/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_212/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_212/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_213/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_213/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_214/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_214/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_215/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_215/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_216/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_216/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_217/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_217/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_218/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_218/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_219/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_219/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_22/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_22/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_220/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_220/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_221/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_221/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_222/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_222/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_223/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_223/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_224/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_224/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_225/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_225/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_226/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_226/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_227/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_227/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_228/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_228/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_229/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_229/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_23/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_23/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_230/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_230/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_231/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_231/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_232/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_232/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_233/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_233/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_234/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_234/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_235/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_235/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_236/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_236/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_237/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_237/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_238/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_238/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_239/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_239/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_24/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_24/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_240/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_240/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_241/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_241/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_242/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_242/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_243/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_243/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_244/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_244/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_245/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_245/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_246/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_246/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_247/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_247/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_248/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_248/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_249/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_249/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_25/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_25/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_250/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_250/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_251/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_251/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_252/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_252/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_253/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_253/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_254/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_254/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_255/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_255/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_256/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_256/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_26/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_26/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_27/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_27/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_28/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_28/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_29/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_29/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_30/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_30/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_31/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_31/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_32/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_32/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_33/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_33/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_34/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_34/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_35/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_35/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_36/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_36/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_37/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_37/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_38/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_38/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_39/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_39/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_40/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_40/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_41/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_41/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_42/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_42/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_43/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_43/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_44/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_44/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_45/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_45/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_46/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_46/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_47/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_47/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_48/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_48/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_49/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_49/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_50/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_50/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_51/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_51/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_52/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_52/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_53/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_53/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_54/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_54/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_55/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_55/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_56/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_56/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_57/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_57/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_58/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_58/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_59/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_59/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_60/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_60/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_61/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_61/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_62/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_62/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_63/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_63/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_64/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_64/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_65/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_65/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_66/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_66/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_67/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_67/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_68/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_68/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_69/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_69/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_7/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_7/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_70/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_70/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_71/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_71/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_72/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_72/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_73/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_73/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_74/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_74/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_75/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_75/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_76/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_76/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_77/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_77/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_78/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_78/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_79/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_79/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_8/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_8/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_80/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_80/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_81/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_81/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_82/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_82/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_83/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_83/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_84/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_84/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_85/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_85/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_86/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_86/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_87/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_87/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_88/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_88/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_89/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_89/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_9/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_9/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_90/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_90/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_91/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_91/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_92/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_92/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_93/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_93/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_94/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_94/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_95/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_95/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_96/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_96/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_97/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_97/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_98/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_98/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/feature_n/feature_99/feature.py` & `chalkpy-2.4.0/chalk/feature_n/feature_99/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/__init__.py` & `chalkpy-2.4.0/chalk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_chalkop.py` & `chalkpy-2.4.0/chalk/features/_chalkop.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_class_property.py` & `chalkpy-2.4.0/chalk/features/_class_property.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/converter.py` & `chalkpy-2.4.0/chalk/features/_encoding/converter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/inputs.py` & `chalkpy-2.4.0/chalk/features/_encoding/inputs.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/json.py` & `chalkpy-2.4.0/chalk/features/_encoding/json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/pyarrow.py` & `chalkpy-2.4.0/chalk/features/_encoding/pyarrow.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/rich.py` & `chalkpy-2.4.0/chalk/features/_encoding/rich.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,12 +345,29 @@
 _rich_converter.register_structure_hook(float, _structure_rich)
 _rich_converter.register_structure_hook(bytes, _structure_rich)
 _rich_converter.register_structure_hook(str, _structure_rich)
 _rich_converter.register_structure_hook(bool, _structure_rich)
 
 
 def unstructure_rich_to_primitive(val: Any) -> TPrimitive:
+    if val is None or type(val) in (str, int, float, bytes, time, datetime, date, timedelta):
+        # Short-circuit these rich types, as the primitive types are the same
+        return val
     return _rich_converter.unstructure(val)
 
 
 def structure_primitive_to_rich(val: TPrimitive, typ: Type[TRich]) -> TRich:
+    if (val is None or type(val) is typ) and typ in (
+        str,
+        int,
+        bool,
+        float,
+        bytes,
+        timedelta,
+        decimal.Decimal,
+        date,
+        datetime,
+        time,
+    ):
+        # Short circuit these rich types
+        return cast(TRich, val)
     return _rich_converter.structure(val, typ)
```

### Comparing `chalkpy-2.3.9/chalk/features/_encoding/serialized_dtype.py` & `chalkpy-2.4.0/chalk/features/_encoding/serialized_dtype.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/dataframe/_filters.py` & `chalkpy-2.4.0/chalk/features/dataframe/_filters.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/dataframe/_impl.py` & `chalkpy-2.4.0/chalk/features/dataframe/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     Dict,
     Iterable,
     List,
     Literal,
     Mapping,
     Optional,
     Sequence,
-    Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
 )
@@ -1283,10 +1282,18 @@
         """
         return DataFrame(self._underlying.slice(offset, length))
 
 
 # Hack to get VSCode/Pylance/Pyright to type DataFrame as Type[DataFrameImpl]
 # but IntelliJ to type it as Type[Any]
 # Vscode can parse through literal dicts; IntelliJ can't
-_dummy_dict = {"0": DataFrameImpl}
 
+if TYPE_CHECKING:
+
+    class DataFrameProtocol(DataFrameImpl):
+        def __class_getitem__(cls, item: Any) -> "DataFrameProtocol":
+            ...
+
+    _dummy_dict = {"0": DataFrameProtocol}
+else:
+    _dummy_dict = {"0": DataFrameImpl}
 DataFrame = _dummy_dict["0"]
```

### Comparing `chalkpy-2.3.9/chalk/features/dataframe/_validation.py` & `chalkpy-2.4.0/chalk/features/dataframe/_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/feature_field.py` & `chalkpy-2.4.0/chalk/features/feature_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,21 +223,14 @@
                 and self.features_cls.__chalk_ts__ is not None
                 and self.features_cls.__chalk_ts__.name == self.name
             ) or self.typ.is_feature_time
         return self._is_feature_time
 
     @functools.cached_property
     def converter(self) -> FeatureConverter:
-        if self.is_has_one or self.is_has_many:
-            raise RuntimeError(
-                (
-                    f"Feature '{self}' is not a scalar feature, so its values cannot be converted into a serialized type. "
-                    "Please access the converters on the underlying scalar feature."
-                )
-            )
         underlying_typ = self.typ.parsed_annotation
 
         if self.typ.is_document:
 
             def document_encoder(x: _TRich):
                 if isinstance(x, BaseModel):
                     return x.json()
@@ -247,14 +240,34 @@
                 if isinstance(self.typ.document_class, type) and issubclass(self.typ.document_class, BaseModel):
                     return self.typ.document_class.parse_raw(x)
                 raise ValueError("Document classes must be pydantic models")
 
             self._decoder = self._decoder or document_decoder
             self._encoder = self._encoder or document_encoder
             self._pyarrow_dtype = self._pyarrow_dtype or pa.large_utf8()
+
+        if self.typ.is_dataframe:
+            from pandas import DataFrame
+            import ast
+
+            # Here go from a DataFrame instance to a JSON str
+            def frame_encoder(x: _TRich):
+                # TODO DataFrame -> String
+                pass
+
+            # Here go from a JSON str to a DataFrame instance
+            def frame_decoder(x: _TPrim):
+                if isinstance(x, str):
+                    dict = ast.literal_eval(x)
+                    return DataFrame(dict['values'], columns=dict['columns'])
+
+            self._decoder = self._decoder or frame_decoder
+            self._encoder = self._encoder or frame_encoder
+            self._pyarrow_dtype = self._pyarrow_dtype or pa.large_utf8()
+
         if isinstance(underlying_typ, Windowed):
             # TODO -- handle Optional[Windowed]?
             underlying_typ = underlying_typ.kind
         underlying_typ = cast(Type[_TRich], underlying_typ)
         return FeatureConverter(
             name=self.fqn,
             rich_type=underlying_typ,
```

### Comparing `chalkpy-2.3.9/chalk/features/feature_set.py` & `chalkpy-2.4.0/chalk/features/feature_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import timedelta
-from typing import Any, Callable, ClassVar, Dict, Iterator, List, Optional, Tuple, Type, cast
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Iterator, List, Optional, Tuple, Type, cast
 
 from typing_extensions import TypeGuard
 
 from chalk.features.feature_field import Feature
 from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
 from chalk.features.live_updates import register_live_updates_if_in_notebook
 from chalk.utils.collections import ensure_tuple, get_unique_item
@@ -29,15 +29,15 @@
         if hasattr(subcls, "__is_features__"):
             return getattr(subcls, "__is_features__")
         return False
 
     def __instancecheck__(self, instance: object) -> bool:
         return self.__subclasscheck__(type(instance))
 
-    def __getitem__(cls, item: Any) -> Type:
+    def __getitem__(cls, item: Any) -> Any:
         # This lets us subscript by the features
         # Annotating the return type as Type[Any] as instances of @features classes are
         # not recognized as being subclasses of Features by the type checker (even though at runtime they would be)
         from chalk.features.dataframe import DataFrame
 
         # Typing the `__getitem__` as any, since the @features members are typed as the underlying data structure
         # But, they should always be features or a tuple of features
@@ -92,14 +92,15 @@
     __chalk_etl_offline_to_online__: ClassVar[bool]
     __chalk_max_staleness__: ClassVar[timedelta]
     __chalk_namespace__: ClassVar[str]
     __chalk_primary__: ClassVar[Optional[Feature]]  # The primary key feature
     __chalk_owner__: ClassVar[Optional[str]]
     __chalk_tags__: ClassVar[List[str]]
     __chalk_ts__: ClassVar[Optional[Feature]]  # The timestamp feature
+    __chalk_feature_fqns_raw__: ClassVar[List[str]]
     features: ClassVar[Tuple[Feature, ...]] = ()
     __is_features__: ClassVar[bool] = True
 
     # When constructing results, this class is instantiated
 
     def __iter__(self) -> Iterator[Tuple[str, Any]]:
         """Iterating over features yields tuples of (fqn, value) for all scalarish feature values."""
@@ -113,15 +114,21 @@
         """Iterating over features yields tuples of (fqn, value) for all feature values."""
         raise NotImplementedError
 
 
 # Hack to get VSCode/Pylance/Pyright to type Features as Type[FeatureImpl]
 # but IntelliJ to type it as Type[Any]
 # Vscode can parse through literal dicts; IntelliJ can't
-_dummy_dict = {"0": FeaturesImpl}
+if TYPE_CHECKING:
+    class FeaturesProtocol(FeaturesImpl):
+        def __class_getitem__(cls, item: Any) -> "FeaturesProtocol":
+            ...
+    _dummy_dict = {"0": FeaturesProtocol}
+else:
+    _dummy_dict = {"0": FeaturesImpl}
 
 Features = _dummy_dict["0"]
 
 
 class FeatureSetBase:
     """Registry containing all @features classes."""
```

### Comparing `chalkpy-2.3.9/chalk/features/feature_set_decorator.py` & `chalkpy-2.4.0/chalk/features/feature_set_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from chalk.features.feature_field import Feature, _VersionInfo
 from chalk.features.feature_set import Features, FeatureSetBase
 from chalk.features.feature_time import feature_time
 from chalk.features.feature_wrapper import FeatureWrapper, unwrap_feature
 from chalk.features.tag import Tags
 from chalk.serialization.parsed_annotation import ParsedAnnotation
 from chalk.streams import Windowed
+from chalk.utils import notebook
 from chalk.utils.collections import ensure_tuple
 from chalk.utils.duration import Duration, parse_chalk_duration
 from chalk.utils.metaprogramming import MISSING, create_fn, field_assign, set_new_attribute
 from chalk.utils.string import removeprefix, to_snake_case
 
 T = TypeVar("T")
 
@@ -133,28 +134,37 @@
             owner=owner,
             tags=ensure_tuple(tags),
             etl_offline_to_online=etl_offline_to_online,
             max_staleness=max_staleness,
             namespace=namespace,
         )
         assert issubclass(updated_class, Features)
-        FeatureSetBase.registry[updated_class.__chalk_namespace__] = updated_class
-        if FeatureSetBase.hook is not None:
-            FeatureSetBase.hook(cast(Features, updated_class))
-
+        _add_features_class_to_registry(updated_class)
         return cast(Type[T], updated_class)
 
     # See if we're being called as @features or @features().
     if cls is None:
         # We're called with parens.
         return wrap
 
     # We're called as @features without parens.
     return wrap(cls)
 
+def _add_features_class_to_registry(new_features_class: Features):
+    previous_features_class = FeatureSetBase.registry.get(new_features_class.__chalk_namespace__, None)
+    if previous_features_class is not None and notebook.is_notebook():
+        new_feature_fqns = {fqn for fqn in new_features_class.__chalk_feature_fqns_raw__}
+        previous_feature_fqns = {fqn for fqn in previous_features_class.__chalk_feature_fqns_raw__}
+        missing_fqns = previous_feature_fqns - new_feature_fqns
+        if len(missing_fqns) > 0:
+            raise ValueError(f"New feature class definitions must include existing features. The missing features are: {sorted(missing_fqns)}")
+
+    FeatureSetBase.registry[new_features_class.__chalk_namespace__] = new_features_class
+    if FeatureSetBase.hook is not None:
+        FeatureSetBase.hook(cast(Features, new_features_class))
 
 def _discover_feature(
     features: Sequence[Feature], name: str, *conditions: Callable[[Feature], bool]
 ) -> Optional[Feature]:
     for cond in conditions:
         filtered_features = [c for c in features if cond(c)]
         if len(filtered_features) == 1:
@@ -653,15 +663,25 @@
     def __features__(cls: Features) -> List[Feature]:
         features = list(cls_fields)
         if cls.__chalk_ts__ not in features:
             assert cls.__chalk_ts__ is not None
             features.append(cls.__chalk_ts__)
         return features
 
+    def __feature_fqns_raw__(cls: Features) -> List[str]:
+        """
+        List of explicit feature FQN's defined as members in the class.
+        Used for validation; in certain contexts we can't call __features__
+        since it visits the feature definitions (e.g. join keys) which might contain forward references
+        """
+        return [f.fqn for f in cls_fields]
+
     set_new_attribute(cls=cls, name="features", value=classproperty(__features__, cached=True))
+    set_new_attribute(cls=cls, name="__chalk_feature_fqns_raw__",
+                      value=classproperty(__feature_fqns_raw__, cached=True))
     set_new_attribute(cls=cls, name="__repr__", value=_repr_fn(_globals=_globals))
     set_new_attribute(cls=cls, name="__eq__", value=_eq_fn(_globals=_globals))
     set_new_attribute(cls=cls, name="__hash__", value=None)
     set_new_attribute(cls=cls, name="__iter__", value=_iter_fn(_globals=_globals))
     set_new_attribute(cls=cls, name="items", value=_items_fn(_globals=_globals))
 
     set_new_attribute(cls=cls, name="namespace", value=namespace)
```

### Comparing `chalkpy-2.3.9/chalk/features/feature_time.py` & `chalkpy-2.4.0/chalk/features/feature_time.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/feature_wrapper.py` & `chalkpy-2.4.0/chalk/features/feature_wrapper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/filter.py` & `chalkpy-2.4.0/chalk/features/filter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/hooks.py` & `chalkpy-2.4.0/chalk/features/hooks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/primary.py` & `chalkpy-2.4.0/chalk/features/primary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-from typing import Any, Type, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Protocol, Type, TypeVar, overload
 
 from typing_extensions import Annotated
 
 from chalk.features.feature_wrapper import unwrap_feature
 
 T = TypeVar("T")
 
+if TYPE_CHECKING:
 
-class PrimaryMeta(type):
-    def __getitem__(self, item: Type[T]) -> Type[T]:
-        return cast(Type[T], Annotated[item, "__chalk_primary__"])
-
-
-Primary = PrimaryMeta("Primary", (object,), {})
-"""Marks a feature as the primary feature for a feature class.
-
-Features named `id` on feature classes without an explicit primary
-feature are declared primary keys by default, and don't need to be
-marked with `Primary`.
-
-If you have primary key feature with a name other than `id`,
-you can use this marker to indicate the primary key.
-
-Examples
---------
->>> @features
-... class User:
-...     uid: Primary[int]
-"""
+    class Primary(Protocol[T]):
+        """Marks a feature as the primary feature for a feature class.
+
+        Features named `id` on feature classes without an explicit primary
+        feature are declared primary keys by default, and don't need to be
+        marked with `Primary`.
+
+        If you have primary key feature with a name other than `id`,
+        you can use this marker to indicate the primary key.
+
+        Examples
+        --------
+        >>> @features
+        ... class User:
+        ...     uid: Primary[int]
+        """
+
+        @overload
+        def __get__(self, instance: None, owner: Any) -> Type[T]:
+            ...
+
+        @overload
+        def __get__(self, instance: object, owner: Any) -> T:
+            ...
+
+        def __set__(self, instance: Any, value: T) -> None:
+            ...
+
+        def __delete__(self, instance: Any) -> None:
+            ...
+
+else:
+
+    class Primary:
+        def __class_getitem__(cls, item):
+            return Annotated[item, "__chalk_primary__"]
 
 
 def is_primary(f: Any) -> bool:
     """Determine whether a feature is a primary key.
 
     Parameters
     ----------
```

### Comparing `chalkpy-2.3.9/chalk/features/pseudofeatures.py` & `chalkpy-2.4.0/chalk/features/pseudofeatures.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/features/resolver.py` & `chalkpy-2.4.0/chalk/features/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,26 +258,32 @@
         if asyncio.iscoroutinefunction(self.fn):
             # Not awaiting this coroutine here -- when the caller awaits it,
             # it will run
             return cast(T, self._process_async_call(*args, **kwargs))
         else:
             return self._process_call(*args, **kwargs)
 
-    @classmethod
-    def add_to_registry(cls, r: Resolver):
+    def add_to_registry(self, unique_by_shortname: bool = False):
         """
         Adds the given resolver to the registry.
-        If in a notebook, first removes any existing resolvers with the same FQN.
+        If in a notebook or if unique_by_shortname is True, first removes any existing resolvers
+        with the same short-name.
+
+        Note that if a certain type of Resolver, e.g. StreamResolver, defines its own registry,
+        then resolvers of that type will be added to their class-specific registry and NOT
+        to the more general one.
+
+        :param unique_by_shortname: If specified, remove any existing resolver with the same short-name.
         """
-        if notebook.is_notebook():
-            new_resolvers = [r2 for r2 in cls.registry if r2.name != r.name]
-            new_resolvers.append(r)
-            cls.registry[:] = new_resolvers
+        if unique_by_shortname or notebook.is_notebook():
+            new_resolvers = [r2 for r2 in self.registry if r2.name != self.name]
+            new_resolvers.append(self)
+            self.registry[:] = new_resolvers
         else:
-            cls.registry.append(r)
+            self.registry.append(self)
 
     @functools.cached_property
     def name(self) -> str:
         return self.fqn.split(".")[-1]
 
 
 register_live_updates_if_in_notebook(Resolver)
@@ -919,15 +925,15 @@
             when=when,
             owner=owner,
             state=parsed.state,
             default_args=parsed.default_args,
             timeout=timeout,
         )
 
-        Resolver.add_to_registry(resolver)
+        resolver.add_to_registry()
         if Resolver.hook:
             Resolver.hook(resolver)
 
         # Return the decorated resolver, which notably implements __call__() so it acts the same as
         # the underlying function if called directly, e.g. from test code
         return resolver
 
@@ -1082,15 +1088,15 @@
             machine_type=machine_type,
             state=parsed.state,
             when=when,
             owner=owner,
             default_args=parsed.default_args,
             timeout=timeout,
         )
-        Resolver.add_to_registry(resolver)
+        resolver.add_to_registry()
         if Resolver.hook:
             Resolver.hook(resolver)
         return resolver
 
     return decorator(fn) if fn else decorator
 
 
@@ -1225,15 +1231,15 @@
             max_delay=max_delay,
             upsert=upsert,
             integration=integration,
             owner=owner,
             default_args=parsed.input_feature_defaults,
             input_is_df=parsed.input_is_df,
         )
-        SinkResolver.registry.append(resolver)
+        resolver.add_to_registry()
         return resolver
 
     return decorator(fn) if fn else decorator
 
 
 class StreamResolver(Resolver[P, T]):
     registry: "List[StreamResolver]" = []
@@ -1567,14 +1573,131 @@
     else:
         raise TypeError(f"Stream resolver '{stream_fqn}' inputs must be a list or a DataFrame")
     if not issubclass(input_model_type, BaseModel):
         raise TypeError(f"Stream resolver '{stream_fqn}' must take in BaseModels when using continuous mode and keys")
     return input_model_type
 
 
+def _validate_possibly_nested_key(
+    *,
+    stream_fqn: str,
+    input_model_type: Type[BaseModel],
+    key_path: str,
+) -> Any:
+    """
+    Validates that the given key can be used to look up the corresponding `value` in the original model.
+
+    Examples:
+    - if `key` is `"user_id"` then `input_model_type` should have a `user_id` field.
+    - if `key` is `"user.id"` then `input_model_type` should have a `user` field that has a `id` field
+    """
+    if not isinstance(key_path, str):
+        # The key must be a string.
+        raise TypeError(f"Stream resolver '{stream_fqn}' key '{key_path}' should be type string")
+
+    if key_path == "":
+        raise ValueError(
+            (f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. " f"Key must not be empty.")
+        )
+
+    if "." in key_path:
+        if key_path.startswith("."):
+            raise ValueError(
+                (
+                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                    f"Key '{key_path}' must not start with a dot '.'"
+                )
+            )
+        if key_path.endswith("."):
+            raise ValueError(
+                (
+                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                    f"Key '{key_path}' must not end with a dot '.'"
+                )
+            )
+
+        nested_model_type = input_model_type
+        # This is a nested key path, which is treated somewhat differently.
+        key_path_parts = key_path.split(".")
+        for key_path_part_index, key_path_part in enumerate(key_path_parts):
+            # If we're not still on the first field in the path, we should explain how we got here to the user:
+            explain_current_path = (
+                f" (which is the type of '{'.'.join(key_path_parts[:key_path_part_index])}' on input model class '{input_model_type}')"
+                if key_path_part_index != 0
+                else ""
+            )
+
+            if (
+                nested_model_type is None
+                or nested_model_type is str
+                or nested_model_type is bool
+                or nested_model_type is int
+                or nested_model_type is float
+                or nested_model_type is datetime
+            ):
+                raise ValueError(
+                    (
+                        f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                        f"Key field '{key_path_part}' cannot be looked up in type '{nested_model_type}' because the latter cannot have fields"
+                        f"{explain_current_path}"
+                    )
+                )
+
+            if not hasattr(nested_model_type, "__fields__"):
+                # TODO: Alternatively, we can just stop here, and trust that the user knows what they're doing.
+                # It won't immediately break anything here, but could cause problems down the line (but so would type-errors in the actual stream).
+                raise ValueError(
+                    (
+                        f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                        f"Key field '{key_path_part}' cannot be looked up in type '{nested_model_type}' because the latter is not a Pydantic Model"
+                        f"{explain_current_path}"
+                    )
+                )
+
+            if key_path_part == "":
+                raise ValueError(
+                    (
+                        f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                        f"Key '{key_path}' contains an empty key path part"
+                    )
+                )
+            # Otherwise, look it up in the sub-type.
+            if key_path_part not in nested_model_type.__fields__.keys():
+                raise ValueError(
+                    (
+                        f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                        f"Key field '{key_path_part}' is not an attribute in model class '{nested_model_type}'"
+                        f"{explain_current_path}"
+                    )
+                )
+
+            # Now, drill into the nested model type.
+            nested_model_field_info = nested_model_type.__fields__[key_path_part]
+            if not nested_model_field_info.type_:
+                # We need to have a type annotation to be able to move forward.
+                raise ValueError(
+                    (
+                        f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                        f"Key field '{key_path_part}' is not an attribute in model class '{nested_model_type}'"
+                        f"{explain_current_path}"
+                    )
+                )
+            nested_model_type = nested_model_field_info.type_
+
+    else:
+        # This is not a nested key path, so the key should exist as a field directly on the model.
+        if key_path not in input_model_type.__fields__.keys():
+            raise ValueError(
+                (
+                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                    f"Key '{key_path}' is not an attribute in input model class '{input_model_type}'"
+                )
+            )
+
+
 def _validate_keys(
     stream_fn: Callable[P, T],
     keys: Dict[str, Any],
 ) -> Dict[str, Any]:
     stream_fqn = get_resolver_fqn(function=stream_fn)
 
     if not isinstance(keys, dict):
@@ -1586,23 +1709,20 @@
         output_features = return_annotation.features
     elif isinstance(return_annotation, DataFrameMeta):
         output_features = return_annotation.columns
     else:
         raise TypeError(f"Stream resolver '{stream_fqn}' outputs must be Features or DataFrame")
 
     for key, value in keys.items():
-        if not isinstance(key, str):
-            raise TypeError(f"Stream resolver '{stream_fqn}' key '{key}' should be type string")
-        if key not in input_model_type.__fields__.keys():
-            raise ValueError(
-                (
-                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
-                    f"Key '{key}' is not an attribute in input model class '{input_model_type}'"
-                )
-            )
+        _validate_possibly_nested_key(
+            stream_fqn=stream_fqn,
+            input_model_type=input_model_type,
+            key_path=key,
+        )
+
         if not isinstance(value, FeatureWrapper):
             raise TypeError(
                 (
                     f"Stream resolver '{stream_fqn}' maps key '{key}' to value '{value}', "
                     f"but '{value}' is not of type Feature"
                 )
             )
@@ -1619,14 +1739,15 @@
             raise ValueError(
                 (
                     f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping: "
                     f"Key '{key}' is mapped to '{value}', but value '{value}' is not present"
                     f" in output features {output_fqns}"
                 )
             )
+
     return {key: keys[key] for key in sorted(keys.keys())}
 
 
 def _validate_timestamp(stream_fn: Callable[P, T], timestamp: str, source: StreamSource):
     stream_fqn = get_resolver_fqn(function=stream_fn)
     input_model_type = _get_windowed_stream_resolver_input_type(stream_fn)
 
@@ -1756,10 +1877,9 @@
         state=parsed.state,
         sql_query=None,
         owner=owner,
         parse=parse_info,
         keys=keys,
         timestamp=timestamp,
     )
-
-    StreamResolver.registry.append(resolver)
+    resolver.add_to_registry()
     return resolver
```

### Comparing `chalkpy-2.3.9/chalk/features/tag.py` & `chalkpy-2.4.0/chalk/features/tag.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/gitignore/gitignore_parser.py` & `chalkpy-2.4.0/chalk/gitignore/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/gitignore/helper.py` & `chalkpy-2.4.0/chalk/gitignore/helper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/importer.py` & `chalkpy-2.4.0/chalk/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 from pathlib import Path
 from typing import Callable, Iterable, List, Optional, Union
 
 from chalk.features.resolver import Resolver, StreamResolver
 from chalk.gitignore.gitignore_parser import parse_gitignore
 from chalk.gitignore.helper import IgnoreConfig, _get_default_combined_ignore_config, _is_ignored
 from chalk.parsed.duplicate_input_gql import FailedImport
-from chalk.sql._internal.sql_file_resolver import (
-    ResolverResult,
-    get_sql_file_resolvers,
-    get_sql_file_resolvers_from_paths,
-)
+from chalk.sql._internal.sql_file_resolver import get_sql_file_resolvers, get_sql_file_resolvers_from_paths
 from chalk.sql._internal.sql_source import BaseSQLSource
 from chalk.utils.environment_parsing import env_var_bool
 from chalk.utils.log_with_context import get_logger
 from chalk.utils.paths import _search_recursively_for_file, get_directory_root
 
 _logger = get_logger(__name__)
 
@@ -74,22 +70,17 @@
                 sql_file_resolve_location=path,
                 sources=BaseSQLSource.registry,
             )
         )
     failed_imports: List[FailedImport] = []
     for result in sql_resolver_results:
         if result.resolver:
-            if isinstance(result.resolver, StreamResolver):
-                StreamResolver.registry.append(result.resolver)
-                if StreamResolver.hook:
-                    StreamResolver.hook(result.resolver)
-            else:
-                Resolver.registry.append(result.resolver)
-                if Resolver.hook:
-                    Resolver.hook(result.resolver)
+            result.resolver.add_to_registry()
+            if result.resolver.hook:
+                result.resolver.hook(result.resolver)
         if result.errors:
             for error in result.errors:
                 failed_imports.append(
                     FailedImport(
                         traceback=error.display,
                         filename=error.path,
                         module=error.path,
```

### Comparing `chalkpy-2.3.9/chalk/integrations/named.py` & `chalkpy-2.4.0/chalk/integrations/named.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/logging/__init__.py` & `chalkpy-2.4.0/chalk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/mypy_plugin.py` & `chalkpy-2.4.0/chalk/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/parsed/_graph_validation.py` & `chalkpy-2.4.0/chalk/parsed/_graph_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/parsed/duplicate_input_gql.py` & `chalkpy-2.4.0/chalk/parsed/duplicate_input_gql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/parsed/json_conversions.py` & `chalkpy-2.4.0/chalk/parsed/json_conversions.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/parsed/user_types_to_json.py` & `chalkpy-2.4.0/chalk/parsed/user_types_to_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,21 +80,25 @@
         )
         if config.validation
         else None,
     )
 
 
 def get_registered_types_as_json(scope_to: Path, failed: List[FailedImport], indent: int = 2) -> str:
-    features = [
-        convert_type_to_gql(feature)
-        for x in FeatureSetBase.registry.values()
-        if x.__module__ in sys.modules and _is_relative_to(paths.get_classpath(x), scope_to)
-        for feature in x.features
-        if not feature.is_autogenerated and not feature.no_display
-    ]
+    features = []
+    for x in FeatureSetBase.registry.values():
+        if x.__module__ in sys.modules and _is_relative_to(paths.get_classpath(x), scope_to):
+            for feature in x.features:
+                if not feature.is_autogenerated and not feature.no_display:
+                    try:
+                        converted = convert_type_to_gql(feature)
+                        features.append(converted)
+                    except Exception as e:
+                        raise e
+
     stream_resolvers = [
         convert_type_to_gql(t) for t in StreamResolver.registry if _is_relative_to(Path(t.filename), scope_to)
     ]
     resolvers = [convert_type_to_gql(t) for t in Resolver.registry if _is_relative_to(Path(t.filename), scope_to)]
     sink_resolvers = [
         convert_type_to_gql(t) for t in SinkResolver.registry if _is_relative_to(Path(t.filename), scope_to)
     ]
@@ -112,11 +116,12 @@
         failed=failed,
         resolvers=resolvers,
         charts=charts,
         chalkpy=ChalkPYInfo(version=__version__),
     )
     errors = validate_graph(graph)
     graph.errors = errors
+
     return json.dumps(
         dataclasses.asdict(graph),
         indent=indent,
     )
```

### Comparing `chalkpy-2.3.9/chalk/serialization/parsed_annotation.py` & `chalkpy-2.4.0/chalk/serialization/parsed_annotation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/__init__.py` & `chalkpy-2.4.0/chalk/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/chalk_query.py` & `chalkpy-2.4.0/chalk/sql/_internal/chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/incremental.py` & `chalkpy-2.4.0/chalk/sql/_internal/incremental.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/bigquery.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/bigquery.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/cloudsql.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/cloudsql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/mysql.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/mysql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/postgres.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/postgres.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,23 +163,24 @@
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection],
     ) -> pa.Table:
         import psycopg2.sql
         from sqlalchemy.sql import Select
 
-        if env_var_bool("CHALK_FORCE_SQLALCHEMY_QUERY_EXECUTION"):
+        if env_var_bool("CHALK_FORCE_SQLALCHEMY_QUERY_EXECUTION_WITHOUT_EXCEPTION"):
             raise UnsupportedEfficientExecutionError(
                 (
                     f"The SQL statement will be executed into SQLAlchemy objects, as the environment "
                     "variable 'CHALK_FORCE_SQLALCHEMY_QUERY_EXECUTION' is set. Unset this variable to execute "
                     "the query directly into a PyArrow table."
                 ),
                 log_level=logging.DEBUG,
             )
+
         if finalized_query.finalizer in (Finalizer.FIRST, Finalizer.ONE, Finalizer.ONE_OR_NONE):
             raise UnsupportedEfficientExecutionError(
                 (
                     f"Falling back to SQLAlchemy execution for finalizer '{finalized_query.finalizer.value}', "
                     "as it is faster for small results."
                 ),
                 log_level=logging.DEBUG,
@@ -209,24 +210,53 @@
         first_line = buffer.readline()
         column_names = list(
             csv.reader([first_line.decode("utf8")], escapechar="\\", doublequote=False, quoting=csv.QUOTE_ALL)
         )[0]
         buffer.seek(0)
         converters = columns_to_converters(column_names)
 
-        schema = pa.schema([pa.field(k, v.pyarrow_dtype) for (k, v) in converters.items()])
+        if env_var_bool("CSV_READ_THEN_CAST"):
+            # This seems to tolerant unzoned datetimes better
+            parsed_table = pyarrow.csv.read_csv(
+                buffer,
+                parse_options=pyarrow.csv.ParseOptions(
+                    newlines_in_values=True,
+                    escape_char="\\",
+                    double_quote=False,
+                ),
+                convert_options=pyarrow.csv.ConvertOptions(
+                    true_values=["t"],
+                    false_values=["f"],
+                    strings_can_be_null=True,
+                    quoted_strings_can_be_null=False,
+                ),
+            )
 
-        return pyarrow.csv.read_csv(
-            buffer,
-            parse_options=pyarrow.csv.ParseOptions(
-                newlines_in_values=True,
-                escape_char="\\",
-                double_quote=False,
-            ),
-            convert_options=pyarrow.csv.ConvertOptions(
-                true_values=["t"],
-                false_values=["f"],
-                strings_can_be_null=True,
-                quoted_strings_can_be_null=False,
-                column_types=schema,
-            ),
-        )
+            if len(converters) != len(parsed_table.column_names):
+                _logger.warn(
+                    f"mismatch in number of columns between query and converters: {len(converters)=}, {len(parsed_table.column_names)=}"
+                )
+
+            restricted_schema = pa.schema([pa.field(k, v.pyarrow_dtype) for (k, v) in converters.items()])
+            try:
+                return parsed_table.cast(restricted_schema)
+            except:
+                _logger.warn(f"Falling back from cast in postgres")
+                return parsed_table.select([c for c in converters.keys()]).cast(restricted_schema)
+
+        else:
+            schema = pa.schema([pa.field(k, v.pyarrow_dtype) for (k, v) in converters.items()])
+            return pyarrow.csv.read_csv(
+                buffer,
+                parse_options=pyarrow.csv.ParseOptions(
+                    newlines_in_values=True,
+                    escape_char="\\",
+                    double_quote=False,
+                ),
+                convert_options=pyarrow.csv.ConvertOptions(
+                    true_values=["t"],
+                    false_values=["f"],
+                    strings_can_be_null=True,
+                    quoted_strings_can_be_null=False,
+                    column_types=schema,
+                ),
+            )
```

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/psycopg_common.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/redshift.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/redshift.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/snowflake.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/snowflake.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/integrations/sqlite.py` & `chalkpy-2.4.0/chalk/sql/_internal/integrations/sqlite.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/sql_file_resolver.py` & `chalkpy-2.4.0/chalk/sql/_internal/sql_file_resolver.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/sql_source.py` & `chalkpy-2.4.0/chalk/sql/_internal/sql_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,50 +256,55 @@
         raise NotImplementedError
 
     def execute_query(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection] = None,
+        attempt_efficient_execution: bool = True,
     ) -> pa.Table:
-        try:
-            return self.execute_query_efficient(finalized_query, columns_to_converters, connection)
-        except NotImplementedError:
-            _logger.info(
-                (
-                    "The SQL statement will be executed into SQLAlchemy objects, as the database backend does "
-                    "not support a more efficient execution mechanism."
+        if attempt_efficient_execution:
+            try:
+                return self.execute_query_efficient(finalized_query, columns_to_converters, connection)
+            except NotImplementedError:
+                _logger.info(
+                    (
+                        "The SQL statement will be executed into SQLAlchemy objects, as the database backend does "
+                        "not support a more efficient execution mechanism."
+                    )
                 )
-            )
-            pass
-        except UnsupportedEfficientExecutionError as e:
-            log_level = e.log_level
-            _logger.log(log_level, str(e))
+                pass
+            except UnsupportedEfficientExecutionError as e:
+                log_level = e.log_level
+                _logger.log(log_level, str(e))
 
         return self.execute_query_inefficient(finalized_query, columns_to_converters, connection)
 
     async def async_execute_query(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+        attempt_efficient_execution: bool = True,
     ):
-        try:
-            return await self.async_execute_query_efficient(finalized_query, columns_to_converters, connection)
-        except NotImplementedError:
-            _logger.info(
-                (
-                    "The SQL statement will be executed into SQLAlchemy objects, as the database backend does "
-                    "not support a more efficient execution mechanism."
+        if attempt_efficient_execution:
+
+            try:
+                return await self.async_execute_query_efficient(finalized_query, columns_to_converters, connection)
+            except NotImplementedError:
+                _logger.info(
+                    (
+                        "The SQL statement will be executed into SQLAlchemy objects, as the database backend does "
+                        "not support a more efficient execution mechanism."
+                    )
                 )
-            )
-            pass
-        except UnsupportedEfficientExecutionError as e:
-            log_level = e.log_level
-            _logger.log(log_level, str(e))
+                pass
+            except UnsupportedEfficientExecutionError as e:
+                log_level = e.log_level
+                _logger.log(log_level, str(e))
 
         return await self.async_execute_query_inefficient(finalized_query, columns_to_converters, connection)
 
     async def async_execute_query_inefficient(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
```

### Comparing `chalkpy-2.3.9/chalk/sql/_internal/string_chalk_query.py` & `chalkpy-2.4.0/chalk/sql/_internal/string_chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/sql/finalized_query.py` & `chalkpy-2.4.0/chalk/sql/finalized_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     def params(self):
         return self._params
 
     def execute(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
         connection: Optional[Any] = None,
+        attempt_efficient_execution: bool = True,
     ) -> Union[Features, DataFrame, None]:
         """Actually execute the query to a `DataFrame` or set of features.
 
         If the finalizer was ONE, ONE_OR_NONE, or FIRST, then a `Features` instance
         is returned. Otherwise, if the `finalizer` is ALL, then a `DataFrame` instance
         is returned.
 
@@ -115,21 +116,22 @@
         -------
         DataFrame
             A `DataFrame`, if the `.finalizer` is ALL; otherwise, `Features` set.
             If the finalizer is ONE_OR_NONE or FIRST, then the result may be
             `None` if no row was found
         """
 
-        pa_table = self.execute_to_pyarrow(expected_features, connection)
+        pa_table = self.execute_to_pyarrow(expected_features, connection, attempt_efficient_execution)
         return self._pa_table_to_res(pa_table)
 
     async def async_execute(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
         connection: Optional[Any] = None,
+        attempt_efficient_execution: bool = True,
     ) -> Union[Features, DataFrame, None]:
         """Actually execute the query to a `DataFrame` or set of features.
 
         If the finalizer was ONE, ONE_OR_NONE, or FIRST, then a `Features` instance
         is returned. Otherwise, if the `finalizer` is ALL, then a `DataFrame` instance
         is returned.
 
@@ -146,15 +148,15 @@
         -------
         DataFrame
             A `DataFrame`, if the `.finalizer` is ALL; otherwise, `Features` set.
             If the finalizer is ONE_OR_NONE or FIRST, then the result may be
             `None` if no row was found
         """
 
-        pa_table = await self.async_execute_to_pyarrow(expected_features, connection)
+        pa_table = await self.async_execute_to_pyarrow(expected_features, connection, attempt_efficient_execution)
         return self._pa_table_to_res(pa_table)
 
     def _pa_table_to_res(self, pa_table: pa.Table):
         try:
             import polars as pl
         except ImportError:
             raise missing_dependency_exception("chalkpy[runtime]")
@@ -197,14 +199,15 @@
                 )
             )
 
     def execute_to_pyarrow(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
         connection: Optional[Connection] = None,
+        attempt_efficient_execution: bool = True,
     ) -> pa.Table:
         """Actually execute the query, and return a PyArrow table. Unlike :meth:`.execute`, this method will always keep the
         results as a PyArrow table, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
 
         Parameters
         ----------
         expected_features
@@ -218,22 +221,23 @@
         -------
         Table
             A `pa.Table`, even if the result contains 0 or 1 rows.
         """
         self._check_incremental_settings()
         col_to_converters = self._get_col_to_converter(expected_features)
 
-        pa_table = self.source.execute_query(self, col_to_converters, connection)
+        pa_table = self.source.execute_query(self, col_to_converters, connection, attempt_efficient_execution)
 
         return self._postprocess_table(pa_table, expected_features)
 
     async def async_execute_to_pyarrow(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
         connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+        attempt_efficient_execution: bool = True,
     ) -> pa.Table:
         """Actually execute the query, and return a PyArrow table. Unlike :meth:`.execute`, this method will always keep the
         results as a PyArrow table, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
 
         Parameters
         ----------
         expected_features
@@ -247,15 +251,17 @@
         -------
         Table
             A `pa.Table`, even if the result contains 0 or 1 rows.
         """
         self._check_incremental_settings()
         col_to_converters = self._get_col_to_converter(expected_features)
 
-        pa_table = await self.source.async_execute_query(self, col_to_converters, connection)
+        pa_table = await self.source.async_execute_query(
+            self, col_to_converters, connection, attempt_efficient_execution
+        )
 
         return self._postprocess_table(pa_table, expected_features)
 
     def _postprocess_table(self, pa_table: pa.Table, expected_features: Optional[Sequence[Feature]]):
         expected_feature_root_fqns = (
             None if expected_features is None else frozenset(x.root_fqn for x in expected_features)
         )
@@ -353,14 +359,15 @@
 
         return self.source.execute_to_result_handles(self, converter_getters, connection)
 
     def execute_to_dataframe(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
         connection: Optional[Connection] = None,
+        attempt_efficient_execution: bool = True,
     ):
         """Actually execute the query, and return a DataFrame. Unlike :meth:`.execute`, this method will always keep the
         results as a DataFrame, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
 
         Parameters
         ----------
         expected_features
@@ -375,15 +382,15 @@
         DataFrame
             A `DataFrame`, even if the result contains 0 or 1 rows.
         """
         try:
             import polars as pl
         except ImportError:
             raise missing_dependency_exception("chalkpy[runtime]")
-        pa_table = self.execute_to_pyarrow(expected_features, connection)
+        pa_table = self.execute_to_pyarrow(expected_features, connection, attempt_efficient_execution)
         df = pl.from_arrow(pa_table)
         assert isinstance(df, pl.DataFrame)
         return DataFrame(df)
 
     @functools.lru_cache(1024)
     def get_col_name_mapping(
         self,
@@ -423,7 +430,28 @@
                 )
             for normalized_col_name, original_col_name in normalized_to_original_col.items():
                 if original_col_name not in ans:
                     maybe_matching_root_fqn = _get_matching_root_fqn(normalized_col_name, expected_features)
                     if maybe_matching_root_fqn is not None:
                         ans[original_col_name] = maybe_matching_root_fqn
         return ans
+
+
+if TYPE_CHECKING:
+
+    class SingletonFinalizedChalkQuery(FinalizedChalkQuery, Features):
+        """A FinalizedChalkQuery that returns a single row when executed"""
+
+        # Subclassing from Features so it can does not cause type errors when used in a resolver
+        # that is annotated to return a Features instance
+        ...
+
+    class DataframeFinalizedChalkQuery(FinalizedChalkQuery, DataFrame):
+        """A FinalizedChalkQuery that returns a DataFrame when executed"""
+
+        # Subclassing from DataFrame so it can does not cause type errors when used in a resolver
+        # that is annotated to return a DataFrame
+        ...
+
+else:
+    SingletonFinalizedChalkQuery = FinalizedChalkQuery
+    DataframeFinalizedChalkQuery = FinalizedChalkQuery
```

### Comparing `chalkpy-2.3.9/chalk/sql/protocols.py` & `chalkpy-2.4.0/chalk/sql/protocols.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
 if TYPE_CHECKING:
     import sqlalchemy
     import sqlalchemy.ext.asyncio
     from sqlalchemy.engine import Connection
     from sqlalchemy.orm import Session
 
-    from chalk.sql.finalized_query import FinalizedChalkQuery
+    from chalk.sql.finalized_query import (
+        DataframeFinalizedChalkQuery,
+        FinalizedChalkQuery,
+        SingletonFinalizedChalkQuery,
+    )
 
 TTableIngestProtocol = TypeVar("TTableIngestProtocol", bound="TableIngestProtocol")
 
 
 class StringChalkQueryProtocol(Protocol):
     def execute(self) -> DataFrame:
         """Materialize the query.
@@ -51,79 +55,79 @@
         DataFrame
             A `DataFrame` with the results of the query.
         """
         ans = self.all().execute()
         assert isinstance(ans, DataFrame)
         return ans
 
-    def one_or_none(self) -> FinalizedChalkQuery:
+    def one_or_none(self) -> SingletonFinalizedChalkQuery:
         """Return at most one result or raise an exception.
 
         Returns `None` if the query selects no rows. Raises if
         multiple object identities are returned, or if multiple
         rows are returned for a query that returns only scalar
         values as opposed to full identity-mapped entities.
 
         Returns
         -------
-        FinalizedChalkQuery
+        SingletonFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
-    def one(self) -> FinalizedChalkQuery:
+    def one(self) -> SingletonFinalizedChalkQuery:
         """Return exactly one result or raise an exception.
 
         Returns
         -------
-        FinalizedChalkQuery
+        SingletonFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
-    def all(self) -> FinalizedChalkQuery:
+    def all(self) -> DataframeFinalizedChalkQuery:
         """Return the results represented by this Query as a list.
 
         Returns
         -------
-        FinalizedChalkQuery
+        DataframeFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
     @overload
     def incremental(
         self,
         *,
         incremental_column: str,
         lookback_period: Duration = "0s",
         mode: Literal["row", "group"] = "row",
         incremental_timestamp: Literal["feature_time", "resolver_execution_time"] = "feature_time",
-    ) -> FinalizedChalkQuery:
+    ) -> DataframeFinalizedChalkQuery:
         ...
 
     @overload
     def incremental(
         self,
         *,
         incremental_column: None = None,
         lookback_period: None = None,
         mode: Literal["parameter"],
         incremental_timestamp: Literal["feature_time", "resolver_execution_time"] = "feature_time",
-    ) -> FinalizedChalkQuery:
+    ) -> DataframeFinalizedChalkQuery:
         ...
 
     def incremental(
         self,
         *,
         incremental_column: Optional[str] = None,
         lookback_period: Optional[Duration] = "0s",
         mode: Literal["row", "group", "parameter"] = "row",
         incremental_timestamp: Literal["feature_time", "resolver_execution_time"] = "feature_time",
-    ) -> FinalizedChalkQuery:
+    ) -> DataframeFinalizedChalkQuery:
         """Operates like `.all()`, but tracks `previous_latest_row_timestamp` between query executions in
         order to limit the amount of data returned.
 
         `previous_latest_row_timestamp` will be set the start of the query execution, or if you return
         a `FeatureTime`-mapped column, Chalk will update `previous_latest_row_timestamp` to the maximum
         observed `FeatureTime` value.
 
@@ -186,74 +190,74 @@
             than the last observation time. This requires that the query is grouped by a primary key.
         incremental_timestamp
             Defaults to `"feature_time"`, which means that the timestamp associated with the last feature value
             will be used as the incremental time. Alternatively, setting this parameter to `"resolver_execution_time"`
             will use last literal timestamp that the resolver ran.
         Returns
         -------
-        FinalizedChalkQuery
+        DataframeFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
 
 class ChalkQueryProtocol(Protocol):
-    def first(self) -> FinalizedChalkQuery:
+    def first(self) -> SingletonFinalizedChalkQuery:
         """Return the first result of this Query or None if the result doesn't contain any row.
 
         Returns
         -------
-        FinalizedChalkQuery
+        SingletonFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
-    def one_or_none(self) -> FinalizedChalkQuery:
+    def one_or_none(self) -> SingletonFinalizedChalkQuery:
         """Return at most one result or raise an exception.
 
         Returns `None` if the query selects no rows. Raises if
         multiple object identities are returned, or if multiple
         rows are returned for a query that returns only scalar
         values as opposed to full identity-mapped entities.
 
         Returns
         -------
-        FinalizedChalkQuery
+        SingletonFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
-    def one(self) -> FinalizedChalkQuery:
+    def one(self) -> SingletonFinalizedChalkQuery:
         """Return exactly one result or raise an exception.
 
         Returns
         -------
-        FinalizedChalkQuery
+        SingletonFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
-    def all(self) -> FinalizedChalkQuery:
+    def all(self) -> DataframeFinalizedChalkQuery:
         """Return the results represented by this Query as a `DataFrame`.
 
         Returns
         -------
-        FinalizedChalkQuery
+        DataframeFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
     def incremental(
         self,
         lookback_period: Duration = "0s",
         mode: Literal["row", "group", "parameter"] = "row",
         incremental_column: Optional[Union[str, Feature]] = None,
         incremental_timestamp: Literal["feature_time", "resolver_execution_time"] = "feature_time",
         params: Optional[Mapping[str, Any]] = None,
-    ) -> FinalizedChalkQuery:
+    ) -> DataframeFinalizedChalkQuery:
         """Operates like `.all()`, but tracks `previous_latest_row_timestamp` between query executions in
         order to limit the amount of data returned.
 
         `previous_latest_row_timestamp` will be set the start of the query execution, or if you return
         a `FeatureTime`-mapped column, Chalk will update `previous_latest_row_timestamp` to the maximum
         observed `FeatureTime` value.
 
@@ -316,15 +320,15 @@
             than the last observation time. This requires that the query is grouped by a primary key.
         incremental_timestamp
             Defaults to `"feature_time"`, which means that the timestamp associated with the last feature value
             will be used as the incremental time. Alternatively, setting this parameter to `"resolver_execution_time"`
             will use last literal timestamp that the resolver ran.
         Returns
         -------
-        FinalizedChalkQuery
+        DataframeFinalizedChalkQuery
             A query that can be returned from a resolver.
         """
         ...
 
     def filter_by(self, **kwargs: Any) -> "ChalkQueryProtocol":
         """Apply the given filtering criterion to a copy of this Query,
         using keyword expressions.
@@ -509,39 +513,44 @@
         ...
 
     def execute_query(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection] = None,
+        attempt_efficient_execution: bool = True,
     ) -> pa.Table:
         """Execute a query to a `pa.Table`.
 
         Parameters
         ----------
         finalized_query
             The query to execute
         columns_to_converters
             A function that, given the list of column names returned from the database,
             produces a mapping of columns to converters. Columns not in the resulting dictionary should be ignored.
         connection
             A connection to execute the query under. If not specified, then a new connection is acquired.
+        attempt_efficient_execution
+            The executor will attempt to avoid the use of SQLAlchemy and use more efficient methods to
+            retrieve data.
 
         Returns
         -------
         pa.Table
             A `pa.Table` containing the results.
         """
         ...
 
     async def async_execute_query(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+        attempt_efficient_execution: bool = True,
     ) -> pa.Table:
         """Execute a query to a `pa.Table`.
 
         Parameters
         ----------
         finalized_query
             The query to execute
```

### Comparing `chalkpy-2.3.9/chalk/state.py` & `chalkpy-2.4.0/chalk/state.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/streams/__init__.py` & `chalkpy-2.4.0/chalk/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/streams/_kafka_source.py` & `chalkpy-2.4.0/chalk/streams/_kafka_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/streams/_windows.py` & `chalkpy-2.4.0/chalk/streams/_windows.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/streams/types.py` & `chalkpy-2.4.0/chalk/streams/types.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/testing/__init__.py` & `chalkpy-2.4.0/chalk/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/annotation_parsing.py` & `chalkpy-2.4.0/chalk/utils/annotation_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/collections.py` & `chalkpy-2.4.0/chalk/utils/collections.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/duration.py` & `chalkpy-2.4.0/chalk/utils/duration.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/enum.py` & `chalkpy-2.4.0/chalk/utils/enum.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/log_with_context.py` & `chalkpy-2.4.0/chalk/utils/log_with_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 
 # Backwards compatibility
 Logger = get_logger
 
 
 @contextlib.contextmanager
-def add_logging_context(_merge: bool = True, **extra: Any):
+def add_logging_context(*, _merge: bool = True, **extra: Any):
     """A context manager to push and pop `extra` dictionary keys.
 
     Parameters
     ----------
     _merge
         Whether to merge the new context with the existing log context.
     extra
```

### Comparing `chalkpy-2.3.9/chalk/utils/metaprogramming.py` & `chalkpy-2.4.0/chalk/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/paths.py` & `chalkpy-2.4.0/chalk/utils/paths.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/string.py` & `chalkpy-2.4.0/chalk/utils/string.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.3.9/chalk/utils/stubgen.py` & `chalkpy-2.4.0/chalk/utils/stubgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,43 +81,54 @@
         if item_split[0] in ("typing", "typing_extensions"):
             assert len(item_split) == 2
             return item_split[1]
         item_split = tuple(x.replace("_", "__") for x in item_split)
         item = f"__stubgen_{'_'.join(item_split)}"
         return item
 
-    def _register_imports_for_annotation(self, annotation: Union[type, Windowed]) -> str:
+    def _register_imports_for_annotation(self, annotation: Union[type, Windowed]) -> Tuple[str, str]:
+        """Register all necessary imports, and return a tuple of (protocol annotation, init annotation)"""
         if annotation == type(None):
-            return "None"
+            return "None", "None"
         if annotation is ...:
-            return "..."
+            return "...", "..."
         origin, args = get_origin(annotation), get_args(annotation)
         if origin is None:
             assert args == ()
             # Likely a "simple" annotation, like an enum class
             if isinstance(annotation, Windowed):
                 origin_name = self._add_import(annotation, import_as="Windowed")
                 assert annotation._kind is not None
-                arg_name = self._register_imports_for_annotation(annotation._kind)
-                return f"{origin_name}[{arg_name}]"
+                protocol_arg_name, init_arg_name = self._register_imports_for_annotation(annotation._kind)
+                # FIXME: I don't think this is entirely correct, b/c if a user manually constructs a windowed
+                # feature class, then it's unclear what should be passed in for the windowed arg in the init
+                # parameter
+                return f"{origin_name}[{protocol_arg_name}]", f"{origin_name}[{init_arg_name}]"
             elif annotation.__module__ == "builtins":
                 assert isinstance(annotation, type)
-                return annotation.__name__
+                return annotation.__name__, annotation.__name__
             else:
-                return self._add_import(annotation)
+                ans = self._add_import(annotation)
+                return ans, ans
         # Some sort of generic class, like a collection, or optional
         if origin == UnionType:
             # Convert new-style type unions to old-style typing.Unions
             origin = typing.Union
         if origin == Annotated:
             # If annotated, only pay attention to the first arg -- the actual type
+            if args[1] == "__chalk_primary__":
+                protocol_arg_name, init_arg_name = self._register_imports_for_annotation(args[0])
+                return f"Primary[{protocol_arg_name}]", init_arg_name
             return self._register_imports_for_annotation(args[0])
         origin_name = self._add_import(origin)
         arg_names = [self._register_imports_for_annotation(arg) for arg in args]
-        return f"{origin_name}[" + ", ".join(arg_names) + "]"
+        return (
+            f"{origin_name}[" + ", ".join(x[0] for x in arg_names) + "]",
+            f"{origin_name}[" + ", ".join(x[1] for x in arg_names) + "]",
+        )
 
     def register_features_class(self, features_cls: Type[Features]):
         annotations: Dict[str, ParsedAnnotation] = {}
         for f in features_cls.features:
             assert isinstance(f, Feature)
             assert f.typ is not None
             if f.typ.is_dataframe:
@@ -125,25 +136,25 @@
                 annotations[f.attribute_name] = ParsedAnnotation(
                     "DataFrame",
                     include_in_protocol_cls=True,
                     protocol_annotation="DataFrame",
                 )
             else:
                 # Make a best-effort to figure out imports.
-                annotation = self._register_imports_for_annotation(f.typ.parsed_annotation)
+                proto_annotation, init_annotation = self._register_imports_for_annotation(f.typ.parsed_annotation)
                 include_in_proto_cls = not f.is_windowed_pseudofeature and not f.is_autogenerated
                 if include_in_proto_cls:
                     # TODO do not skip the annotations that do not appear in the protocol class
                     annotations[f.attribute_name] = ParsedAnnotation(
-                        annotation,
+                        init_annotation,
                         include_in_protocol_cls=include_in_proto_cls,
                         # If it's a features class (i.e. a has-one), not specifying
                         # the type in the protocol class so the type checker can
                         # still match feature classes that have a circular reference
-                        protocol_annotation="Any" if f.typ.is_features_cls else annotation,
+                        protocol_annotation="Any" if f.typ.is_features_cls else proto_annotation,
                     )
         if features_cls.__name__ in self._parsed_feature_classes:
             raise ValueError(
                 f"Unable to generate stubs due to multiple features sets called {features_cls.__name__}. Feature set names must be unique. Please rename one of these feature sets."
             )
         self._parsed_feature_classes[features_cls.__name__] = ParsedFeaturesClass(
             module=features_cls.__module__,
@@ -154,14 +165,15 @@
         self._add_import("typing.Optional", "Optional")
         self._add_import("typing.Any", "Any")
         self._add_import("typing.Protocol", "Protocol")
         self._add_import("typing.Type", "Type")
         self._add_import("typing.overload", "overload")
         self._add_import("chalk.features.feature_set.FeaturesMeta", "FeaturesMeta")
         self._add_import("chalk.features.Features", "Features")
+        self._add_import("chalk.features.primary.Primary", "Primary")
         self._add_import("chalk.utils.duration.Duration", "Duration")
         self._add_import("chalk.features.Tags", "Tags")
         lines = [
             "# AUTO-GENERATED FILE. Do not edit. Run `chalk stubgen` to generate.",
             "# fmt: off",
             "# isort: skip_file",
             "from __future__ import annotations",
```

### Comparing `chalkpy-2.3.9/chalkpy.egg-info/SOURCES.txt` & `chalkpy-2.4.0/chalkpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 chalk/_validation/feature_validation.py
 chalk/_validation/validation.py
 chalk/client/__init__.py
 chalk/client/client_impl.py
 chalk/client/dataset.py
 chalk/client/exc.py
 chalk/client/models.py
+chalk/client/serialization/__init__.py
+chalk/client/serialization/query_serialization.py
 chalk/clogging/__init__.py
 chalk/clogging/chalk_logger.py
 chalk/config/__init__.py
 chalk/config/auth_config.py
 chalk/config/project_config.py
 chalk/df/ChalkDataFrameImpl.py
 chalk/df/__init__.py
@@ -618,14 +620,15 @@
 chalk/sql/_internal/integrations/sqlite.py
 chalk/sql/_internal/integrations/psycopg3/__init__.py
 chalk/sql/_internal/integrations/psycopg3/psycopg_common.py
 chalk/sql/_internal/integrations/psycopg3/psycopg_dialect.py
 chalk/streams/__init__.py
 chalk/streams/_file_source.py
 chalk/streams/_kafka_source.py
+chalk/streams/_kinesis_source.py
 chalk/streams/_windows.py
 chalk/streams/base.py
 chalk/streams/types.py
 chalk/testing/__init__.py
 chalk/utils/__init__.py
 chalk/utils/annotation_parsing.py
 chalk/utils/async_helpers.py
```

### Comparing `chalkpy-2.3.9/pyproject.toml` & `chalkpy-2.4.0/pyproject.toml`

 * *Files identical despite different names*

