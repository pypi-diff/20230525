# Comparing `tmp/sqlfluff-2.1.0.tar.gz` & `tmp/sqlfluff-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-k_3si0rm/sqlfluff-2.1.0.tar", last modified: Wed May  3 23:19:59 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-a8ni5akz/sqlfluff-2.1.1.tar", last modified: Thu May 25 16:29:29 2023, max compression
```

## Comparing `sqlfluff-2.1.0.tar` & `sqlfluff-2.1.1.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)   384369 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129958 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68071 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    32904 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80702 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   165834 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   200331 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   102212 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172023 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 23:19:59.000000 sqlfluff-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-03 23:19:45.000000 sqlfluff-2.1.0/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   387901 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24440 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50768 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34592 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131078 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23153 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68489 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95470 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80767 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165834 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69805 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200331 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102326 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172937 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93437 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:29.000000 sqlfluff-2.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 16:29:13.000000 sqlfluff-2.1.1/test/test_testing.py
```

### Comparing `sqlfluff-2.1.0/CHANGELOG.md` & `sqlfluff-2.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,49 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.1.1] - 2023-05-25
+
+## Highlights
+
+This releases fixes a compatability issue with the latest version of dbt. It also ships various dialect improvements.
+
+## What’s Changed
+
+* profiles dir env var or default [#4886](https://github.com/sqlfluff/sqlfluff/pull/4886) [@JasonGluck](https://github.com/JasonGluck)
+* Bigquery: Allow empty `struct` in `TO_JSON` [#4879](https://github.com/sqlfluff/sqlfluff/pull/4879) [@dimitris-flyr](https://github.com/dimitris-flyr)
+* Set type of ARRAY function for BigQuery [#4880](https://github.com/sqlfluff/sqlfluff/pull/4880) [@tunetheweb](https://github.com/tunetheweb)
+* Full athena SHOW coverage [#4876](https://github.com/sqlfluff/sqlfluff/pull/4876) [@dogversioning](https://github.com/dogversioning)
+* Sparksql add star support in multiparameter functions [#4874](https://github.com/sqlfluff/sqlfluff/pull/4874) [@spex66](https://github.com/spex66)
+* Oracle create view with EDITIONING & FORCE [#4872](https://github.com/sqlfluff/sqlfluff/pull/4872) [@ulixius9](https://github.com/ulixius9)
+* Fixes pip installation link on Getting Started [#4867](https://github.com/sqlfluff/sqlfluff/pull/4867) [@segoldma](https://github.com/segoldma)
+* Athena: add "weird" test cases for `group by` [#4869](https://github.com/sqlfluff/sqlfluff/pull/4869) [@KulykDmytro](https://github.com/KulykDmytro)
+* Athena: add support for `CUBE` `ROLLUP` `GROUPING SETS` [#4862](https://github.com/sqlfluff/sqlfluff/pull/4862) [@KulykDmytro](https://github.com/KulykDmytro)
+* Add show tables/views to athena [#4854](https://github.com/sqlfluff/sqlfluff/pull/4854) [@dogversioning](https://github.com/dogversioning)
+* Adding support for NOCOPY and INSTANT algorithm on CREATE INDEX on MySQL dialect [#4865](https://github.com/sqlfluff/sqlfluff/pull/4865) [@wfelipew](https://github.com/wfelipew)
+* Add link to Trino keywords (Athena v3) [#4858](https://github.com/sqlfluff/sqlfluff/pull/4858) [@KulykDmytro](https://github.com/KulykDmytro)
+* TSQL: Create Role Authorization [#4852](https://github.com/sqlfluff/sqlfluff/pull/4852) [@greg-finley](https://github.com/greg-finley)
+* TSQL: DEADLOCK_PRIORITY [#4853](https://github.com/sqlfluff/sqlfluff/pull/4853) [@greg-finley](https://github.com/greg-finley)
+* fix(dialect-clickhouse): Support SYSTEM queries [#4625](https://github.com/sqlfluff/sqlfluff/pull/4625) [@germainlefebvre4](https://github.com/germainlefebvre4)
+* Fix #4807: LT02 & LT12 issues with empty files. [#4834](https://github.com/sqlfluff/sqlfluff/pull/4834) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Sqlite: COLLATE column constraint [#4845](https://github.com/sqlfluff/sqlfluff/pull/4845) [@greg-finley](https://github.com/greg-finley)
+* Hive: Support REGEXP and IREGEXP [#4846](https://github.com/sqlfluff/sqlfluff/pull/4846) [@greg-finley](https://github.com/greg-finley)
+
+## New Contributors
+
+* [@dogversioning](https://github.com/dogversioning) made their first contribution in [#4854](https://github.com/sqlfluff/sqlfluff/pull/4854)
+* [@segoldma](https://github.com/segoldma) made their first contribution in [#4867](https://github.com/sqlfluff/sqlfluff/pull/4867)
+* [@spex66](https://github.com/spex66) made their first contribution in [#4874](https://github.com/sqlfluff/sqlfluff/pull/4874)
+* [@dimitris-flyr](https://github.com/dimitris-flyr) made their first contribution in [#4879](https://github.com/sqlfluff/sqlfluff/pull/4879)
+* [@JasonGluck](https://github.com/JasonGluck) made their first contribution in [#4886](https://github.com/sqlfluff/sqlfluff/pull/4886)
+
 ## [2.1.0] - 2023-05-03
 
 ## Highlights
 
 This release brings support for dbt 1.5+. Some internals of dbt mean
 that SQFluff versions prior to this release may experience errors with
 dbt versions post 1.5. In addition to that there are some dialect and
```

### Comparing `sqlfluff-2.1.0/LICENSE.md` & `sqlfluff-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/PKG-INFO` & `sqlfluff-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.0
+Version: 2.1.1
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.0/README.md` & `sqlfluff-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/setup.cfg` & `sqlfluff-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.1.0
+version = 2.1.1
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.1.0
+stable_version = 2.1.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/api/simple.py` & `sqlfluff-2.1.1/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/commands.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/commands.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.1.1/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/config.py` & `sqlfluff-2.1.1/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.1.1/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.1.1/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.1.1/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/enums.py` & `sqlfluff-2.1.1/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/errors.py` & `sqlfluff-2.1.1/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.1.1/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.1.1/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.1.1/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.1.1/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.1.1/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.1.1/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.1.1/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/core/timing.py` & `sqlfluff-2.1.1/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -843,14 +843,34 @@
     type = "typed_struct_literal"
     match_grammar: Matchable = Sequence(
         Ref("StructTypeSegment"),
         Ref("StructLiteralSegment"),
     )
 
 
+class EmptyStructLiteralBracketsSegment(BaseSegment):
+    """An empty struct literal segment - `()`.
+
+    NOTE: This is only to set the right type so spacing rules are applied correctly.
+    """
+
+    type = "struct_literal"
+    match_grammar: Matchable = Bracketed()
+
+
+class EmptyStructLiteralSegment(BaseSegment):
+    """An empty array literal segment - `STRUCT()`."""
+
+    type = "typed_struct_literal"
+    match_grammar: Matchable = Sequence(
+        Ref("StructTypeSegment"),
+        Ref("EmptyStructLiteralBracketsSegment"),
+    )
+
+
 class ObjectLiteralSegment(BaseSegment):
     """An object literal segment."""
 
     type = "object_literal"
     match_grammar: Matchable = Bracketed(
         Delimited(
             Ref("ObjectLiteralElementSegment"),
@@ -1277,14 +1297,15 @@
                 Ref("QuotedLiteralSegment"),
                 Ref("SingleIdentifierGrammar"),
                 Ref("ColumnReferenceSegment"),
             ),
         ),
         Ref("IgnoreRespectNullsGrammar"),
         Ref("IndexColumnDefinitionSegment"),
+        Ref("EmptyStructLiteralSegment"),
     ),
     PostFunctionGrammar=OneOf(
         # Optional OVER suffix for window functions.
         # This is supported in bigquery & postgres (and its derivatives)
         # and so is included here for now.
         Ref("OverClauseSegment"),
         # Filter clause supported by both Postgres and SQLite
@@ -2814,14 +2835,17 @@
                 ),
             ),
             Ref("PrimaryKeyGrammar"),
             Ref("UniqueKeyGrammar"),  # UNIQUE
             Ref("AutoIncrementGrammar"),
             Ref("ReferenceDefinitionGrammar"),  # REFERENCES reftable [ ( refcolumn) ]x
             Ref("CommentClauseSegment"),
+            Sequence(
+                "COLLATE", Ref("CollationReferenceSegment")
+            ),  # https://www.sqlite.org/datatype3.html#collation
         ),
     )
 
 
 class ColumnDefinitionSegment(BaseSegment):
     """A column definition, e.g. for CREATE TABLE or ALTER TABLE."""
 
@@ -4054,7 +4078,24 @@
     """The `LOCAL.ALIAS` syntax allows to use an alias name of a column within clauses.
 
     A hookpoint for other dialects e.g. Exasol.
     """
 
     type = "local_alias_segment"
     match_grammar: Matchable = Nothing()
+
+
+class PathSegment(BaseSegment):
+    """A reference to a path."""
+
+    type = "path_segment"
+    match_grammar: Matchable = OneOf(
+        Sequence(
+            Ref("SlashSegment"),
+            Delimited(
+                Ref("CodeSegment"),
+                delimiter=Ref("SlashSegment"),
+                allow_gaps=False,
+            ),
+        ),
+        Ref("QuotedLiteralSegment"),
+    )
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 """
 
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.core.parser import (
     AnyNumberOf,
     BaseSegment,
     Bracketed,
+    Dedent,
     Delimited,
-    TypedParser,
+    Indent,
+    Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     Ref,
     RegexParser,
     SegmentGenerator,
     Sequence,
     StringLexer,
     StringParser,
     SymbolSegment,
+    TypedParser,
 )
 from sqlfluff.core.parser.segments.raw import CodeSegment, KeywordSegment
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects.dialect_athena_keywords import (
     athena_reserved_keywords,
     athena_unreserved_keywords,
 )
@@ -389,14 +392,15 @@
 
     parse_grammar = ansi.StatementSegment.parse_grammar.copy(
         insert=[
             Ref("MsckRepairTableStatementSegment"),
             Ref("UnloadStatementSegment"),
             Ref("PrepareStatementSegment"),
             Ref("ExecuteStatementSegment"),
+            Ref("ShowStatementSegment"),
         ],
         remove=[
             Ref("TransactionStatementSegment"),
             Ref("CreateSchemaStatementSegment"),
             Ref("SetSchemaStatementSegment"),
             Ref("CreateModelStatementSegment"),
             Ref("DropModelStatementSegment"),
@@ -477,15 +481,15 @@
                 Sequence("WITH NO DATA", optional=True),
             ),
         ),
     )
 
 
 class MsckRepairTableStatementSegment(BaseSegment):
-    """An `MSCK REPAIR TABLE`statement.
+    """An `MSCK REPAIR TABLE` statement.
 
     The `MSCK REPAIR TABLE` command scans a file system such as Amazon S3 for
     Hive compatible partitions that were added to the file system after the
     table was created.
 
     https://docs.aws.amazon.com/athena/latest/ug/msck-repair-table.html
     """
@@ -639,7 +643,128 @@
                     Bracketed(Ref("ExpressionSegment")),
                 ),
                 Ref("DatetimeUnitSegment"),
                 Sequence("TO", Ref("DatetimeUnitSegment"), optional=True),
             ),
         ),
     )
+
+
+class GroupByClauseSegment(ansi.GroupByClauseSegment):
+    """A `GROUP BY` clause like in `SELECT`.
+
+    https://docs.aws.amazon.com/athena/latest/ug/select.html#:~:text=%5B-,GROUP,-BY%20%5B%20ALL%20%7C%20DISTINCT%20%5D%20grouping_expressions
+    """
+
+    match_grammar: Matchable = Sequence(
+        "GROUP",
+        "BY",
+        Indent,
+        Delimited(
+            OneOf(
+                Ref("CubeRollupClauseSegment"),
+                Ref("GroupingSetsClauseSegment"),
+                Ref("ColumnReferenceSegment"),
+                Ref("NumericLiteralSegment"),  # Can `GROUP BY 1`
+                Ref("ExpressionSegment"),  # Can `GROUP BY coalesce(col, 1)`
+            ),
+            terminator=OneOf(
+                Sequence("ORDER", "BY"),
+                "LIMIT",
+                "OFFSET",
+                "HAVING",
+                Ref("SetOperatorSegment"),
+            ),
+        ),
+        Dedent,
+    )
+
+
+class CubeRollupClauseSegment(BaseSegment):
+    """`[CUBE | ROLLUP]` clause within the `GROUP BY` clause."""
+
+    type = "cube_rollup_clause"
+
+    match_grammar = Sequence(
+        OneOf("CUBE", "ROLLUP"),
+        Bracketed(Delimited(Ref("ColumnReferenceSegment"))),
+    )
+
+
+class GroupingSetsClauseSegment(BaseSegment):
+    """`GROUPING SETS` clause within the `GROUP BY` clause."""
+
+    type = "grouping_sets_clause"
+
+    match_grammar = Sequence(
+        "GROUPING",
+        "SETS",
+        Bracketed(
+            Delimited(
+                Ref("ColumnReferenceSegment"),
+                Bracketed(Delimited(Ref("ColumnReferenceSegment"), optional=True)),
+            ),
+        ),
+    )
+
+
+class ShowStatementSegment(BaseSegment):
+    """A `show` execute statement.
+
+    Full Apache Hive `SHOW` reference:
+    https://cwiki.apache.org/confluence/display/Hive/LanguageManual+DDL#LanguageManualDDL-Show
+
+    Athena supported subset:
+    https://docs.aws.amazon.com/athena/latest/ug/ddl-reference.html
+    """
+
+    type = "show_statement"
+    match_grammar = Sequence(
+        "SHOW",
+        OneOf(
+            Sequence(
+                "COLUMNS",
+                OneOf("FROM", "IN"),
+                OneOf(
+                    Sequence(
+                        Ref("DatabaseReferenceSegment"), Ref("TableReferenceSegment")
+                    ),
+                    Sequence(
+                        Ref("TableReferenceSegment"),
+                        Sequence(
+                            OneOf("FROM", "IN"),
+                            Ref("DatabaseReferenceSegment"),
+                            optional=True,
+                        ),
+                    ),
+                ),
+            ),
+            Sequence(
+                "CREATE",
+                OneOf("TABLE", "VIEW"),
+                Ref("TableReferenceSegment"),
+            ),
+            Sequence(
+                OneOf("DATABASES", "SCHEMAS"),
+                Sequence("LIKE", Ref("QuotedLiteralSegment"), optional=True),
+            ),
+            Sequence(
+                "PARTITIONS",
+                Ref("TableReferenceSegment"),
+            ),
+            Sequence(
+                "TABLES",
+                Sequence("IN", Ref("DatabaseReferenceSegment"), optional=True),
+                Ref("QuotedLiteralSegment", optional=True),
+            ),
+            Sequence(
+                "TBLPROPERTIES",
+                Ref("TableReferenceSegment"),
+                Bracketed(Ref("QuotedLiteralSegment"), optional=True),
+            ),
+            Sequence(
+                "VIEWS",
+                Sequence("IN", Ref("DatabaseReferenceSegment"), optional=True),
+                Sequence("LIKE", Ref("QuotedLiteralSegment"), optional=True),
+            ),
+        ),
+    )
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A list of all Athena keywords.
 
-Presto List: https://prestodb.io/docs/0.217/language/reserved.html
+Presto List (for Athena v2): https://prestodb.io/docs/0.217/language/reserved.html
+Trino List (for Athena v3): https://trino.io/docs/current/language/reserved.html
 Hive List: https://cwiki.apache.org/confluence/display/Hive/LanguageManual+DDL
 """
 
 athena_reserved_keywords = [
     "ALL",
     "ALTER",
     "AND",
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -771,14 +771,29 @@
     match_grammar: Matchable = StringParser(
         "EXTRACT",
         CodeSegment,
         type="function_name_identifier",
     )
 
 
+class ArrayFunctionNameSegment(BaseSegment):
+    """ARRAY function name segment.
+
+    Need to be able to specify this as type `function_name_identifier`
+    within a `function_name` so that linting rules identify it properly.
+    """
+
+    type = "function_name"
+    match_grammar: Matchable = StringParser(
+        "ARRAY",
+        CodeSegment,
+        type="function_name_identifier",
+    )
+
+
 class DatePartWeekSegment(BaseSegment):
     """WEEK(<WEEKDAY>) in EXTRACT, DATE_DIFF, DATE_TRUNC, LAST_DAY.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/date_functions#extract
     https://cloud.google.com/bigquery/docs/reference/standard-sql/date_functions#date_diff
     https://cloud.google.com/bigquery/docs/reference/standard-sql/date_functions#date_trunc
     https://cloud.google.com/bigquery/docs/reference/standard-sql/date_functions#last_day
@@ -1078,15 +1093,15 @@
 class ArrayExpressionSegment(ansi.ArrayExpressionSegment):
     """Expression to construct a ARRAY from a subquery.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/array_functions#array
     """
 
     match_grammar = Sequence(
-        "ARRAY",
+        Ref("ArrayFunctionNameSegment"),
         Bracketed(
             Ref("SelectableGrammar"),
         ),
     )
 
 
 class TupleSegment(BaseSegment):
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     UNRESERVED_KEYWORDS,
 )
 
 ansi_dialect = load_raw_dialect("ansi")
 
 clickhouse_dialect = ansi_dialect.copy_as("clickhouse")
 clickhouse_dialect.sets("unreserved_keywords").update(UNRESERVED_KEYWORDS)
+clickhouse_dialect.replace(
+    SingleIdentifierGrammar=OneOf(
+        Ref("NakedIdentifierSegment"),
+        Ref("QuotedIdentifierSegment"),
+        Ref("SingleQuotedIdentifierSegment"),
+    ),
+)
 
 clickhouse_dialect.insert_lexer_matchers(
     # https://clickhouse.com/docs/en/sql-reference/functions#higher-order-functions---operator-and-lambdaparams-expr-function
     [StringLexer("lambda", r"->", SymbolSegment, segment_kwargs={"type": "lambda"})],
     before="newline",
 )
 
@@ -104,14 +111,15 @@
         # This case ANY JOIN
         "ANY",
         # This case ALL JOIN
         "ALL",
     ),
     LambdaFunctionSegment=TypedParser("lambda", SymbolSegment, type="lambda"),
 )
+
 clickhouse_dialect.replace(
     BinaryOperatorGrammar=OneOf(
         Ref("ArithmeticBinaryOperatorGrammar"),
         Ref("StringBinaryOperatorGrammar"),
         Ref("BooleanBinaryOperatorGrammar"),
         Ref("ComparisonOperatorGrammar"),
         # Add Lambda Function
@@ -315,14 +323,25 @@
                 # Engine functions may omit brackets.
                 optional=True,
             ),
         ),
     )
 
 
+class OnClusterClauseSegment(BaseSegment):
+    """A `ON CLUSTER` clause."""
+
+    type = "on_cluster"
+    match_grammar = Sequence(
+        "ON",
+        "CLUSTER",
+        Ref("SingleIdentifierGrammar"),
+    )
+
+
 class EngineSegment(BaseSegment):
     """An `ENGINE` used in `CREATE TABLE`."""
 
     type = "engine"
 
     match_grammar = Sequence(
         "ENGINE",
@@ -496,20 +515,15 @@
             Ref("OrReplaceGrammar"),
             Ref.keyword("TEMPORARY"),
             optional=True,
         ),
         "TABLE",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("ExpressionSegment"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
         OneOf(
             # CREATE TABLE (...):
             Sequence(
                 Bracketed(
                     Delimited(
                         OneOf(
                             Ref("TableConstraintSegment"),
@@ -562,20 +576,15 @@
 
     match_grammar = Sequence(
         "CREATE",
         "MATERIALIZED",
         "VIEW",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("ExpressionSegment"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
         OneOf(
             Sequence(
                 "TO",
                 Ref("TableReferenceSegment"),
                 Ref("EngineSegment", optional=True),
             ),
             Sequence(
@@ -600,21 +609,15 @@
 
     match_grammar = Sequence(
         "DROP",
         Ref.keyword("TEMPORARY", optional=True),
         "TABLE",
         Ref("IfExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
         Ref.keyword("SYNC", optional=True),
     )
 
 
 class DropDatabaseStatementSegment(ansi.DropDatabaseStatementSegment):
     """A `DROP DATABASE` statement.
 
@@ -625,21 +628,15 @@
     type = "drop_database_statement"
 
     match_grammar = Sequence(
         "DROP",
         "DATABASE",
         Ref("IfExistsGrammar", optional=True),
         Ref("DatabaseReferenceSegment"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
         Ref.keyword("SYNC", optional=True),
     )
 
 
 class DropDictionaryStatementSegment(BaseSegment):
     """A `DROP DICTIONARY` statement.
 
@@ -668,21 +665,15 @@
     type = "drop_user_statement"
 
     match_grammar = Sequence(
         "DROP",
         "USER",
         Ref("IfExistsGrammar", optional=True),
         Ref("SingleIdentifierGrammar"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
     )
 
 
 class DropRoleStatementSegment(ansi.DropRoleStatementSegment):
     """A `DROP ROLE` statement.
 
     As specified in
@@ -692,21 +683,15 @@
     type = "drop_user_statement"
 
     match_grammar = Sequence(
         "DROP",
         "ROLE",
         Ref("IfExistsGrammar", optional=True),
         Ref("SingleIdentifierGrammar"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
     )
 
 
 class DropQuotaStatementSegment(BaseSegment):
     """A `DROP QUOTA` statement.
 
     As specified in
@@ -716,21 +701,15 @@
     type = "drop_quota_statement"
 
     match_grammar = Sequence(
         "DROP",
         "QUOTA",
         Ref("IfExistsGrammar", optional=True),
         Ref("SingleIdentifierGrammar"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
     )
 
 
 class DropSettingProfileStatementSegment(BaseSegment):
     """A `DROP setting PROFILE` statement.
 
     As specified in
@@ -744,21 +723,15 @@
         Delimited(
             Ref("NakedIdentifierSegment"),
             min_delimiters=0,
         ),
         "PROFILE",
         Ref("IfExistsGrammar", optional=True),
         Ref("SingleIdentifierGrammar"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
     )
 
 
 class DropViewStatementSegment(ansi.DropViewStatementSegment):
     """A `DROP VIEW` statement.
 
     As specified in
@@ -768,21 +741,15 @@
     type = "drop_view_statement"
 
     match_grammar = Sequence(
         "DROP",
         "VIEW",
         Ref("IfExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
-        # Ref("OnClusterClauseSegment", optional=True),
-        Sequence(
-            "ON",
-            "CLUSTER",
-            Ref("SingleIdentifierGrammar"),
-            optional=True,
-        ),
+        Ref("OnClusterClauseSegment", optional=True),
         Ref.keyword("SYNC", optional=True),
     )
 
 
 class DropFunctionStatementSegment(ansi.DropFunctionStatementSegment):
     """A `DROP FUNCTION` statement.
 
@@ -793,20 +760,313 @@
     type = "drop_function_statement"
 
     match_grammar = Sequence(
         "DROP",
         "FUNCTION",
         Ref("IfExistsGrammar", optional=True),
         Ref("SingleIdentifierGrammar"),
-        # Ref("OnClusterClauseSegment", optional=True),
+        Ref("OnClusterClauseSegment", optional=True),
+    )
+
+
+class SystemMergesSegment(BaseSegment):
+    """A `SYSTEM ... MERGES` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_merges_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "MERGES",
+        OneOf(
+            Sequence(
+                "ON",
+                "VOLUME",
+                Ref("ObjectReferenceSegment"),
+            ),
+            Ref("TableReferenceSegment"),
+        ),
+    )
+
+
+class SystemTTLMergesSegment(BaseSegment):
+    """A `SYSTEM ... TTL MERGES` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_ttl_merges_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "TTL",
+        "MERGES",
+        Ref("TableReferenceSegment", optional=True),
+    )
+
+
+class SystemMovesSegment(BaseSegment):
+    """A `SYSTEM ... MOVES` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_moves_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "MOVES",
+        Ref("TableReferenceSegment", optional=True),
+    )
+
+
+class SystemReplicaSegment(BaseSegment):
+    """A `SYSTEM ... REPLICA` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_replica_segment"
+
+    match_grammar = OneOf(
         Sequence(
-            "ON",
-            "CLUSTER",
+            "SYNC",
+            "REPLICA",
+            Ref("OnClusterClauseSegment", optional=True),
+            Ref("TableReferenceSegment"),
+            Sequence("STRICT", optional=True),
+        ),
+        Sequence(
+            "DROP",
+            "REPLICA",
             Ref("SingleIdentifierGrammar"),
-            optional=True,
+            Sequence(
+                "FROM",
+                OneOf(
+                    Sequence(
+                        "DATABASE",
+                        Ref("ObjectReferenceSegment"),
+                    ),
+                    Sequence(
+                        "TABLE",
+                        Ref("TableReferenceSegment"),
+                    ),
+                    Sequence(
+                        "ZKPATH",
+                        Ref("PathSegment"),
+                    ),
+                ),
+                optional=True,
+            ),
+        ),
+        Sequence(
+            "RESTART",
+            "REPLICA",
+            Ref("TableReferenceSegment"),
+        ),
+        Sequence(
+            "RESTORE",
+            "REPLICA",
+            Ref("TableReferenceSegment"),
+            Ref("OnClusterClauseSegment", optional=True),
+        ),
+    )
+
+
+class SystemFilesystemSegment(BaseSegment):
+    """A `SYSTEM ... FILESYSTEM` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_filesystem_segment"
+
+    match_grammar = Sequence(
+        "DROP",
+        "FILESYSTEM",
+        "CACHE",
+    )
+
+
+class SystemReplicatedSegment(BaseSegment):
+    """A `SYSTEM ... REPLICATED` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_replicated_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "REPLICATED",
+        "SENDS",
+        Ref("TableReferenceSegment", optional=True),
+    )
+
+
+class SystemReplicationSegment(BaseSegment):
+    """A `SYSTEM ... REPLICATION` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_replication_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "REPLICATION",
+        "QUEUES",
+        Ref("TableReferenceSegment", optional=True),
+    )
+
+
+class SystemFetchesSegment(BaseSegment):
+    """A `SYSTEM ... FETCHES` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_fetches_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            "START",
+            "STOP",
+        ),
+        "FETCHES",
+        Ref("TableReferenceSegment", optional=True),
+    )
+
+
+class SystemDistributedSegment(BaseSegment):
+    """A `SYSTEM ... DISTRIBUTED` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_distributed_segment"
+
+    match_grammar = Sequence(
+        OneOf(
+            Sequence(
+                OneOf(
+                    "START",
+                    "STOP",
+                ),
+                "DISTRIBUTED",
+                "SENDS",
+                Ref("TableReferenceSegment"),
+            ),
+            Sequence(
+                "FLUSH",
+                "DISTRIBUTED",
+                Ref("TableReferenceSegment"),
+            ),
+        ),
+        # Ref("TableReferenceSegment"),
+    )
+
+
+class SystemModelSegment(BaseSegment):
+    """A `SYSTEM ... MODEL` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_model_segment"
+
+    match_grammar = Sequence(
+        "RELOAD",
+        OneOf(
+            Sequence(
+                "MODELS",
+                Ref("OnClusterClauseSegment", optional=True),
+            ),
+            Sequence(
+                "MODEL",
+                AnySetOf(
+                    Ref("OnClusterClauseSegment", optional=True),
+                    Ref("PathSegment"),
+                ),
+            ),
+        ),
+    )
+
+
+class SystemFileSegment(BaseSegment):
+    """A `SYSTEM ... FILE` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_file_segment"
+
+    match_grammar = Sequence(
+        "SYNC",
+        "FILE",
+        "CACHE",
+    )
+
+
+class SystemUnfreezeSegment(BaseSegment):
+    """A `SYSTEM ... UNFREEZE` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_unfreeze_segment"
+
+    match_grammar = Sequence(
+        "UNFREEZE",
+        "WITH",
+        "NAME",
+        Ref("ObjectReferenceSegment"),
+    )
+
+
+class SystemStatementSegment(BaseSegment):
+    """A `SYSTEM ...` statement.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/system
+    """
+
+    type = "system_statement"
+
+    match_grammar: Matchable = Sequence(
+        "SYSTEM",
+        OneOf(
+            Ref("SystemMergesSegment"),
+            Ref("SystemTTLMergesSegment"),
+            Ref("SystemMovesSegment"),
+            Ref("SystemReplicaSegment"),
+            Ref("SystemReplicatedSegment"),
+            Ref("SystemReplicationSegment"),
+            Ref("SystemFetchesSegment"),
+            Ref("SystemDistributedSegment"),
+            Ref("SystemFileSegment"),
+            Ref("SystemFilesystemSegment"),
+            Ref("SystemUnfreezeSegment"),
+            Ref("SystemModelSegment"),
         ),
     )
 
 
 class StatementSegment(ansi.StatementSegment):
     """Overriding StatementSegment to allow for additional segment parsing."""
 
@@ -814,9 +1074,10 @@
     parse_grammar = ansi.StatementSegment.parse_grammar.copy(
         insert=[
             Ref("CreateTableStatementSegment"),
             Ref("CreateMaterializedViewStatementSegment"),
             Ref("DropDictionaryStatementSegment"),
             Ref("DropQuotaStatementSegment"),
             Ref("DropSettingProfileStatementSegment"),
+            Ref("SystemStatementSegment"),
         ]
     )
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     "EPHEMERAL",
     "EVENTS",
     "EXISTS",
     "EXPLAIN",
     "EXPRESSION",
     "EXTRACT",
     "FETCHES",
+    "FILE",
+    "FILESYSTEM",
     "FINAL",
     "FIRST",
     "FLUSH",
     "FOR",
     "FORMAT",
     "FREEZE",
     "FROM",
@@ -100,17 +102,20 @@
     "LOGS",
     "MATERIALIZE",
     "MATERIALIZED",
     "MAX",
     "MERGES",
     "MIN",
     "MINUTE",
+    "MODEL",
+    "MODELS",
     "MODIFY",
     "MONTH",
     "MOVE",
+    "MOVES",
     "MUTATION",
     "NAN_SQL",
     "NO",
     "NOT",
     "NULL_SQL",
     "NULLS",
     "OFFSET",
@@ -120,25 +125,28 @@
     "POPULATE",
     "PREWHERE",
     "PRIMARY",
     "PROFILE",
     "PROJECTION",
     "QUARTER",
     "QUOTA",
+    "QUEUES",
     "RANGE",
     "RELOAD",
     "REMOVE",
     "RENAME",
     "REPLACE",
     "REPLICA",
     "REPLICATED",
+    "REPLICATION",
     "ROLLUP",
     "SAMPLE",
     "SECOND",
     "SEMI",
+    "SEND",
     "SENDS",
     "SETTINGS",
     "SHOW",
     "SOURCE",
     "START",
     "STOP",
     "SUBSTRING",
@@ -157,20 +165,22 @@
     "TOP",
     "TOTALS",
     "TRAILING",
     "TRIM",
     "TRUNCATE",
     "TTL",
     "TYPE",
+    "UNFREEZE",
     "UPDATE",
     "USE",
     "UUID",
     "VALUES",
     "VIEW",
     "VOLUME",
     "WATCH",
     "WEEK",
     "WHEN",
     "WHERE",
     "WITH",
     "YEAR",
+    "ZKPATH",
 ]
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,17 @@
                 Ref("PartitionSpecGrammar"),
                 "WITH",
                 "TABLE",
                 Ref("TableReferenceSegment"),
             ),
         ]
     ),
+    LikeGrammar=OneOf(
+        "LIKE", "RLIKE", "ILIKE", "REGEXP", "IREGEXP"
+    ),  # Impala dialect uses REGEXP and IREGEXP
 )
 
 
 class ArrayTypeSegment(ansi.ArrayTypeSegment):
     """Prefix for array literals specifying the type."""
 
     type = "array_type"
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     "IDXPROPERTIES",
     "IGNORE",
     "INDEX",
     "INDEXES",
     "INPATH",
     "INPUTDRIVER",
     "INPUTFORMAT",
+    "IREGEXP",  # Impala dialect
     "ITEMS",
     "JAR",
     "KEYS",
     "KEY_TYPE",
     "LIMIT",
     "LINES",
     "LOAD",
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -800,14 +800,15 @@
     )
 
 
 class CreateIndexStatementSegment(ansi.CreateIndexStatementSegment):
     """A `CREATE INDEX` statement.
 
     https://dev.mysql.com/doc/refman/8.0/en/create-index.html
+    https://mariadb.com/kb/en/create-index/
     """
 
     match_grammar = Sequence(
         "CREATE",
         OneOf("UNIQUE", "FULLTEXT", "SPATIAL", optional=True),
         "INDEX",
         Ref("IndexReferenceSegment"),
@@ -816,15 +817,15 @@
         Ref("TableReferenceSegment"),
         Ref("BracketedKeyPartListGrammar"),
         Ref("IndexOptionsSegment", optional=True),
         AnySetOf(
             Sequence(
                 "ALGORITHM",
                 Ref("EqualsSegment", optional=True),
-                OneOf("DEFAULT", "INPLACE", "COPY"),
+                OneOf("DEFAULT", "INPLACE", "COPY", "NOCOPY", "INSTANT"),
             ),
             Sequence(
                 "LOCK",
                 Ref("EqualsSegment", optional=True),
                 OneOf("DEFAULT", "NONE", "SHARED", "EXCLUSIVE"),
             ),
         ),
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -781,8 +781,10 @@
 ZONE
 """
 
 # These are not MySQL keywords, but SQLFluff needs them to parse well.
 mysql_unreserved_keywords += """NOW
 SHARED
 INPLACE
+NOCOPY
+INSTANT
 """
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,19 @@
 from sqlfluff.dialects import dialect_ansi as ansi
 
 ansi_dialect = load_raw_dialect("ansi")
 oracle_dialect = ansi_dialect.copy_as("oracle")
 
 oracle_dialect.sets("unreserved_keywords").difference_update(["COMMENT"])
 oracle_dialect.sets("reserved_keywords").update(
-    ["COMMENT", "ON", "UPDATE", "INDEXTYPE", "PROMPT"]
+    ["COMMENT", "ON", "UPDATE", "INDEXTYPE", "PROMPT", "FORCE"]
+)
+
+oracle_dialect.sets("unreserved_keywords").update(
+    ["EDITIONABLE", "EDITIONING", "NONEDITIONABLE"]
 )
 
 oracle_dialect.sets("bare_functions").clear()
 oracle_dialect.sets("bare_functions").update(
     [
         "current_date",
         "current_timestamp",
@@ -375,7 +379,33 @@
             Ref("ColonSegment"),
             Ref("DelimiterGrammar"),
             Ref("JoinLikeClauseGrammar"),
             BracketedSegment,
         ),
         allow_gaps=False,
     )
+
+
+class CreateViewStatementSegment(ansi.CreateViewStatementSegment):
+    """A `CREATE VIEW` statement."""
+
+    type = "create_view_statement"
+    # https://docs.oracle.com/en/database/oracle/oracle-database/19/sqlrf/CREATE-VIEW.html
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        Ref("OrReplaceGrammar", optional=True),
+        Sequence(Ref.keyword("NO", optional=True), "FORCE", optional=True),
+        OneOf(
+            "EDITIONING",
+            Sequence("EDITIONABLE", Ref.keyword("EDITIONING", optional=True)),
+            "NONEDITIONABLE",
+            optional=True,
+        ),
+        "VIEW",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("TableReferenceSegment"),
+        # Optional list of column names
+        Ref("BracketedColumnReferenceListGrammar", optional=True),
+        "AS",
+        ansi.OptionallyBracketed(Ref("SelectableGrammar")),
+        Ref("WithNoSchemaBindingClauseSegment", optional=True),
+    )
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,14 +394,18 @@
         Ref("StartSquareBracketSegment"),
         Ref("StartBracketSegment"),
         Ref("BinaryOperatorGrammar"),
         Ref("DelimiterGrammar"),
         Ref("JoinLikeClauseGrammar"),
         ansi.BracketedSegment,
     ),
+    FunctionContentsExpressionGrammar=OneOf(
+        Ref("ExpressionSegment"),
+        Ref("StarSegment"),
+    ),
 )
 
 sparksql_dialect.add(
     FileLiteralSegment=TypedParser(
         "file_literal", ansi.LiteralSegment, type="file_literal"
     ),
     BackQuotedIdentifierSegment=TypedParser(
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,8 +197,11 @@
     "FAST",
     "EXTRA",
     "FILE",
     "PASSIVE",
     "RESTART",
     "RESET",
     "STRICT",
+    "BINARY",
+    "NOCASE",
+    "RTRIM",
 ]
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -2439,14 +2439,21 @@
                     OneOf(
                         "ON",
                         "OFF",
                         Sequence(
                             Ref("EqualsSegment"),
                             Ref("ExpressionSegment"),
                         ),
+                        # The below for https://learn.microsoft.com/en-us/sql/t-sql/statements/set-deadlock-priority-transact-sql?view=sql-server-ver16 # noqa
+                        "LOW",
+                        "NORMAL",
+                        "HIGH",
+                        Ref("ParameterNameSegment"),
+                        Ref("NumericLiteralSegment"),
+                        Ref("QualifiedNumericLiteralSegment"),
                     ),
                 ),
                 Sequence(
                     Ref("ParameterNameSegment"),
                     Ref("AssignmentOperatorSegment"),
                     Ref("ExpressionSegment"),
                 ),
@@ -5566,7 +5573,27 @@
                     "REJECTED_ROW_LOCATION",
                     Ref("EqualsSegment"),
                     Ref("QuotedLiteralSegment"),
                 ),
             ),
         ),
     )
+
+
+class CreateRoleStatementSegment(ansi.CreateRoleStatementSegment):
+    """A `CREATE ROLE` statement.
+
+    https://learn.microsoft.com/en-us/sql/t-sql/statements/create-role-transact-sql?view=sql-server-ver16
+    """
+
+    type = "create_role_statement"
+
+    match_grammar = Sequence(
+        "CREATE",
+        "ROLE",
+        Ref("RoleReferenceSegment"),
+        Sequence(
+            "AUTHORIZATION",
+            Ref("RoleReferenceSegment"),
+            optional=True,
+        ),
+    )
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.1.1/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,15 @@
     "FORMAT",
     "FORMATFILE_DATA_SOURCE",
     "FORMATFILE",
     "GENERATED",
     "HASH",
     "HEAP",  # Azure Synapse Analytics specific
     "HIDDEN",
+    "HIGH",
     "HINT",
     "HISTORY_RETENTION_PERIOD",
     "HISTORY_TABLE",
     "IGNORE_CONSTRAINTS",
     "IGNORE_DUP_KEY",
     "IGNORE_NONCLUSTERED_COLUMNSTORE_INDEX",
     "IGNORE_TRIGGERS",
@@ -359,14 +360,15 @@
     "LOAD",  # listed as reserved but functionally unreserved
     "LOB_COMPACTION",
     "LOCATION",
     "LOCK_TIMEOUT",
     "LOG",
     "LOGIN",
     "LOOP",
+    "LOW",
     "MASKED",
     "MATCHED",
     "MAX_DURATION",
     "MAX_GRANT_PERCENT",
     "MAX",
     "MAXDOP",
     "MAXERRORS",
@@ -381,14 +383,15 @@
     "NO_PERFORMANCE_SPOOL",
     "NO",
     "NOCOUNT",
     "NOEXEC",
     "NOEXPAND",
     "NOLOCK",
     "NONE",
+    "NORMAL",
     "NOWAIT",
     "NTILE",
     "NUMERIC_ROUNDABORT",
     "OBJECT",
     "OFFSET",
     "ONLINE",
     "OPENJSON",
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.1.1/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT12.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,18 @@
         We only care about the segment and the siblings which come after it
         for this rule, we discard the others into the kwargs argument.
 
         """
         # We only care about the final segment of the parse tree.
         parent_stack, segment = get_last_segment(FunctionalContext(context).segment)
         self.logger.debug("Found last segment as: %s", segment)
+        if not segment:
+            # NOTE: Edge case. If the file is totally empty, we won't find a final
+            # segment. In this case return without error.
+            return None
 
         trailing_newlines = Segments(*get_trailing_newlines(context.segment))
         trailing_literal_newlines = trailing_newlines
         self.logger.debug(
             "Untemplated trailing newlines: %s", trailing_literal_newlines
         )
         if context.templated_file:
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.1.1/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/reflow/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,18 @@
 
     def get_raw(self) -> str:
         """Get the current raw representation."""
         return "".join(elem.raw for elem in self.elements)
 
     @staticmethod
     def _validate_reflow_sequence(elements: ReflowSequenceType):
-        assert elements, "ReflowSequence has empty elements."
+        # An empty set of elements _is_ allowed as an edge case.
+        if not elements:
+            # Return early if so
+            return None
         # Check odds and evens
         OddType = elements[0].__class__
         EvenType = ReflowPoint if OddType is ReflowBlock else ReflowBlock
         try:
             # Check odds are all points
             assert all(
                 isinstance(elem, OddType) for elem in elements[::2]
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.1.1/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.1.1/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.1.0
+Version: 2.1.1
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.1.0/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.1.1/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.1.1/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.1.0/test/test_testing.py` & `sqlfluff-2.1.1/test/test_testing.py`

 * *Files identical despite different names*

