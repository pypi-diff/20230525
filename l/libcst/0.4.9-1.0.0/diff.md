# Comparing `tmp/libcst-0.4.9.tar.gz` & `tmp/libcst-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcst-0.4.9.tar", last modified: Thu Nov 10 21:32:33 2022, max compression
+gzip compressed data, was "libcst-1.0.0.tar", last modified: Thu May 25 19:14:47 2023, max compression
```

## Comparing `libcst-0.4.9.tar` & `libcst-1.0.0.tar`

### file list

```diff
@@ -1,489 +1,494 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.cargo/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-11-10 21:32:16.000000 libcst-0.4.9/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-10 21:32:16.000000 libcst-0.4.9/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 21:32:16.000000 libcst-0.4.9/.fixit.config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-11-10 21:32:16.000000 libcst-0.4.9/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-10 21:32:16.000000 libcst-0.4.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/build-matrix.json
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/pypi_upload.yml
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-10 21:32:16.000000 libcst-0.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-10 21:32:16.000000 libcst-0.4.9/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-10 21:32:16.000000 libcst-0.4.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-10 21:32:16.000000 libcst-0.4.9/.watchmanconfig
--rw-r--r--   0 runner    (1001) docker     (121)    32176 2022-11-10 21:32:16.000000 libcst-0.4.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-11-10 21:32:16.000000 libcst-0.4.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-11-10 21:32:16.000000 libcst-0.4.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-10 21:32:16.000000 libcst-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-10 21:32:16.000000 libcst-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 21:32:33.894809 libcst-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10297 2022-11-10 21:32:16.000000 libcst-0.4.9/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      992 2022-11-10 21:32:16.000000 libcst-0.4.9/check_copyright.sh
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-10 21:32:16.000000 libcst-0.4.9/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.834809 libcst-0.4.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.846809 libcst-0.4.9/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.846809 libcst-0.4.9/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (121)   108465 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/img/python_scopes.png
--rw-r--r--   0 runner    (1001) docker     (121)    30400 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/img/python_scopes.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon_16px.png
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon_32px.png
--rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal_white_sidebar.png
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/icon_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/vertical_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/codemods.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/codemods_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/matchers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13597 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/matchers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9920 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/metadata_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9632 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/parser.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/scope_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9873 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/visitors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15454 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/why_libcst.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.854809 libcst-0.4.9/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)     8492 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (121)     5666 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_flatten_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_maybe_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_metadata_dependent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.858809 libcst-0.4.9/libcst/_nodes/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19439 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (121)   140076 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/internal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    31193 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/op.py
--rw-r--r--   0 runner    (1001) docker     (121)   131699 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.866809 libcst-0.4.9/libcst/_nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10350 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)    45724 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     7138 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_await.py
--rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_boolean_op.py
--rw-r--r--   0 runner    (1001) docker     (121)    22698 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)    12963 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_classdef.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (121)    13640 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_cst_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_del.py
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_dict_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_else.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_flatten_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     7665 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_for.py
--rw-r--r--   0 runner    (1001) docker     (121)    93215 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_funcdef.py
--rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_if.py
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_ifexp.py
--rw-r--r--   0 runner    (1001) docker     (121)    29777 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_indented_block.py
--rw-r--r--   0 runner    (1001) docker     (121)    40077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_leaf_small_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    22302 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_matrix_multiply.py
--rw-r--r--   0 runner    (1001) docker     (121)     8290 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_namedexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_newline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_raise.py
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_removal_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_return.py
--rw-r--r--   0 runner    (1001) docker     (121)     4868 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    20094 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)    13989 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_small_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)    16758 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_subscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_trailing_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)    25792 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_try.py
--rw-r--r--   0 runner    (1001) docker     (121)    11237 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_unary_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_while.py
--rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_with.py
--rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_yield.py
--rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.866809 libcst-0.4.9/libcst/_parser/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/conversions/
--rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53078 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/params.py
--rw-r--r--   0 runner    (1001) docker     (121)    47301 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/terminals.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/custom_itertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7270 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/detect_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    12408 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/pgen2/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13727 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/grammar_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/python/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/py_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    44145 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    14001 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/production_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9370 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/py_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/python_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14086 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_detect_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10662 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_footer_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_node_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     6660 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_version_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    83462 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_wrapped_tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/types/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7020 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/partials.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/production.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_whitespace_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/types/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/token.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/whitespace_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     8319 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/wrapped_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_removal_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (121)   179734 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_typed_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_typed_visitor_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6835 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gather.py
--rw-r--r--   0 runner    (1001) docker     (121)    20436 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_matcher_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_visitor_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5810 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codegen/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/tests/test_codegen_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codemod/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24234 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_codemod.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_dummy_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     5850 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (121)    16030 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    32682 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    16562 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/rename.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/strip_strings_from_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (121)    11173 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     4650 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    15194 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (121)     5813 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_strip_strings_from_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_unnecessary_format_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/unnecessary_format_string.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/codemod_formatter_error_input.py.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_codemod.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_codemod_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/visitors/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17416 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    53287 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     5642 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    20494 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/visitors/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20692 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    50145 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     6031 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    23821 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19403 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)    10497 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)    11776 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/matchers/
--rw-r--r--   0 runner    (1001) docker     (121)   535179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    81853 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_matcher_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9718 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_return_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    35199 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/matchers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35418 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    15761 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     6721 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_findall.py
--rw-r--r--   0 runner    (1001) docker     (121)    53908 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_matchers.py
--rw-r--r--   0 runner    (1001) docker     (121)    23189 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_matchers_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    10927 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)    20190 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7825 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7363 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/name_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/position_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     8391 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    46368 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/span_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_base_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)    14931 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    12198 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_metadata_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    19874 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_name_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_position_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    75819 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_span_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6107 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/tests/pyre/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/simple_class.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/simple_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_deep_clone.py
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_deep_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8102 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_pyre_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25336 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8028 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    30607 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.854809 libcst-0.4.9/libcst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15607 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/
--rw-r--r--   0 runner    (1001) docker     (121)    25856 2022-11-10 21:32:16.000000 libcst-0.4.9/native/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 21:32:16.000000 libcst-0.4.9/native/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)    32411 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/Grammar
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/benches/
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/benches/parser_benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/src/
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (121)    80125 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/expression.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/inflate_helpers.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/macros.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/module.rs
--rw-r--r--   0 runner    (1001) docker     (121)    50731 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/op.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/parser_config.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/py_cached.rs
--rw-r--r--   0 runner    (1001) docker     (121)   104571 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/statement.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/test_utils.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/traits.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/whitespace.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/errors.rs
--rw-r--r--   0 runner    (1001) docker     (121)   109918 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/grammar.rs
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/numbers.rs
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/py.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    49640 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/string_types.rs
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/debug_utils.rs
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/operators.rs
--rw-r--r--   0 runner    (1001) docker     (121)    22036 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/tests.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/text_position/
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/text_position/char_width.rs
--rw-r--r--   0 runner    (1001) docker     (121)    11761 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/text_position/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)    12813 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/whitespace_parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/big_binary_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/class_craziness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/comments.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/dangling_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/decorated_function_without_body.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/dysfunctional_del.py
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/expr_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/fun_with_func_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/global_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/import.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/just_a_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/malicious_match.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/pep646.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/raise.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/smol_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/spacious_spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/starry_tries.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/suicidal_slices.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/super_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/terrible_tries.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/trailing_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/tuple_shenanigans.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/vast_emptiness.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/with_wickedness.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/wonky_walrus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/parser_roundtrip.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/cstnode.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/inflate.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/into_py.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/parenthesized_node.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.838809 libcst-0.4.9/native/libcst_derive/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/tests/pass/
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/tests/pass/minimal_cst.rs
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/tests/pass/simple.rs
--rwxr-xr-x   0 runner    (1001) docker     (121)      270 2022-11-10 21:32:16.000000 libcst-0.4.9/native/roundtrip.sh
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-10 21:32:16.000000 libcst-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-10 21:32:16.000000 libcst-0.4.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-10 21:32:16.000000 libcst-0.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 21:32:33.894809 libcst-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-10 21:32:16.000000 libcst-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/hypothesis.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/hypothesmith.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst/native.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/libcst_native/
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/parser_config.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/token_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/whitespace_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/whitespace_state.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/setuptools.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/typing_inspect.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 19:11:37.000000 libcst-1.0.0/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 19:11:37.000000 libcst-1.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 19:11:37.000000 libcst-1.0.0/.fixit.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-25 19:11:37.000000 libcst-1.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 19:11:37.000000 libcst-1.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/build-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 19:11:37.000000 libcst-1.0.0/.github/workflows/pypi_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 19:11:37.000000 libcst-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 19:11:37.000000 libcst-1.0.0/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 19:11:37.000000 libcst-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 19:11:37.000000 libcst-1.0.0/.watchmanconfig
+-rw-r--r--   0 runner    (1001) docker     (123)    37188 2023-05-25 19:11:37.000000 libcst-1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-25 19:11:37.000000 libcst-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-25 19:11:37.000000 libcst-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-25 19:11:37.000000 libcst-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 19:11:37.000000 libcst-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-05-25 19:14:47.966725 libcst-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-25 19:11:37.000000 libcst-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 19:11:37.000000 libcst-1.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.902724 libcst-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.910724 libcst-1.0.0/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   108465 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/img/python_scopes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30400 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/img/python_scopes.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon_16px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/favicon_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/horizontal_white_sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/icon_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_static/logo/vertical_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/codemods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/codemods_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/matchers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/matchers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/metadata_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/scope_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/visitors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15454 2023-05-25 19:11:37.000000 libcst-1.0.0/docs/source/why_libcst.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.914724 libcst-1.0.0/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_flatten_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_maybe_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_metadata_dependent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.918724 libcst-1.0.0/libcst/_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140091 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31193 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_boolean_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_classdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_cst_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_dict_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_else.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_empty_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_flatten_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94136 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_funcdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_if.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_ifexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29777 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_indented_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_leaf_small_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_matrix_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_namedexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_newline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_removal_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_simple_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_small_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_trailing_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_try.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_unary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_while.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/tests/test_yield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_nodes/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/conversions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53078 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/conversions/terminals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/custom_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.926724 libcst-1.0.0/libcst/_parser/parso/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/pgen2/grammar_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44145 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/python/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/parso/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/parso/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/production_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/py_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/python_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_footer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_node_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_version_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83462 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/tests/test_wrapped_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/partials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/py_whitespace_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.930724 libcst-1.0.0/libcst/_parser/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/types/whitespace_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_parser/wrapped_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_removal_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179734 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_typed_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_typed_visitor_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_matcher_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/gen_visitor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codegen/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/tests/test_codegen_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codegen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.934724 libcst-1.0.0/libcst/codemod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_dummy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/strip_strings_from_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/commands/unnecessary_format_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.938724 libcst-1.0.0/libcst/codemod/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/codemod_formatter_error_input.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_codemod_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/codemod/visitors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50584 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20494 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/codemod/visitors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54487 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/codemod/visitors/tests/test_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.942724 libcst-1.0.0/libcst/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/helpers/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.946725 libcst-1.0.0/libcst/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)   534993 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81855 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.950724 libcst-1.0.0/libcst/matchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35211 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_findall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53908 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_matchers_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20190 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/matchers/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.950724 libcst-1.0.0/libcst/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/span_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_file_path_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_metadata_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75819 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_span_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/tests/test_type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/metadata/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/libcst/tests/pyre/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/simple_class.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/pyre/simple_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_deep_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_deep_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_pyre_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25336 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tests/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31223 2023-05-25 19:11:37.000000 libcst-1.0.0/libcst/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.918724 libcst-1.0.0/libcst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 19:14:47.000000 libcst-1.0.0/libcst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/native/
+-rw-r--r--   0 runner    (1001) docker     (123)    25856 2023-05-25 19:11:37.000000 libcst-1.0.0/native/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:11:37.000000 libcst-1.0.0/native/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.954725 libcst-1.0.0/native/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/Grammar
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/benches/parser_benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    80125 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/inflate_helpers.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/module.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/op.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/parser_config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/py_cached.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   104571 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/test_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/nodes/whitespace.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   109927 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/grammar.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/parser/numbers.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/py.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.958725 libcst-1.0.0/native/libcst/src/tokenizer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/src/tokenizer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    49644 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/core/string_types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/debug_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/operators.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/tests.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/src/tokenizer/text_position/
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/text_position/char_width.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/text_position/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/src/tokenizer/whitespace_parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/big_binary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/class_craziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/dangling_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/decorated_function_without_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/dysfunctional_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/expr_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/fun_with_func_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/global_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/just_a_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/malicious_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/pep646.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/smol_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/spacious_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/starry_tries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/suicidal_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/super_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/terrible_tries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/trailing_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/tuple_shenanigans.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/vast_emptiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/with_wickedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/fixtures/wonky_walrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst/tests/parser_roundtrip.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.962725 libcst-1.0.0/native/libcst_derive/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/native/libcst_derive/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/cstnode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/inflate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/into_py.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/src/parenthesized_node.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.906724 libcst-1.0.0/native/libcst_derive/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/native/libcst_derive/tests/pass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/tests/pass/minimal_cst.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-25 19:11:37.000000 libcst-1.0.0/native/libcst_derive/tests/pass/simple.rs
+-rwxr-xr-x   0 runner    (1001) docker     (123)      270 2023-05-25 19:11:37.000000 libcst-1.0.0/native/roundtrip.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-25 19:11:37.000000 libcst-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-25 19:11:37.000000 libcst-1.0.0/scripts/check_copyright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-25 19:11:37.000000 libcst-1.0.0/scripts/regenerate-fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:14:47.966725 libcst-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 19:11:37.000000 libcst-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/hypothesis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/hypothesmith.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/libcst/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst/native.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:14:47.966725 libcst-1.0.0/stubs/libcst_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/parser_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/token_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/whitespace_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/libcst_native/whitespace_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/setuptools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:11:37.000000 libcst-1.0.0/stubs/typing_inspect.pyi
```

### Comparing `libcst-0.4.9/.flake8` & `libcst-1.0.0/.flake8`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/.github/build-matrix.json` & `libcst-1.0.0/.github/build-matrix.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {'2': "{'os': 'macos-latest'}", '3': "{'os': 'macos-latest'}"}*

```diff
@@ -4,19 +4,19 @@
         "vers": "x86_64"
     },
     {
         "os": "ubuntu-20.04",
         "vers": "i686"
     },
     {
-        "os": "macos-10.15",
+        "os": "macos-latest",
         "vers": "arm64"
     },
     {
-        "os": "macos-10.15",
+        "os": "macos-latest",
         "vers": "auto64"
     },
     {
         "os": "windows-2019",
         "vers": "auto64"
     },
     {
```

### Comparing `libcst-0.4.9/.github/workflows/build.yml` & `libcst-1.0.0/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   # Build python wheels
   build_matrix:
     name: Prepare job matrix for build job
     runs-on: ubuntu-latest
     outputs:
       matrix: ${{ steps.set-matrix.outputs.matrix }}
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v3
       - id: set-matrix
         # match github.ref to the on_ref_regex field in the json
         # to skip running linux/aarch64 builds on PRs
         run: |
           matrix=$(jq --arg ref "${{ github.ref }}" \
             'map(select(.on_ref_regex as $pat | $pat == null or ($ref | test($pat))) | del(.on_ref_regex))' \
             .github/build-matrix.json)
@@ -35,33 +35,31 @@
       CIBW_BEFORE_ALL_MACOS: "rustup target add aarch64-apple-darwin x86_64-apple-darwin"
       CIBW_BEFORE_ALL_WINDOWS: "rustup target add x86_64-pc-windows-msvc i686-pc-windows-msvc"
       CIBW_ENVIRONMENT: 'PATH="$PATH:$HOME/.cargo/bin" LIBCST_NO_LOCAL_SCHEME=$LIBCST_NO_LOCAL_SCHEME'
       CIBW_SKIP: "cp27-* cp34-* cp35-* pp* *-win32 *-win_arm64 *-musllinux_*"
       CIBW_ARCHS: ${{ matrix.vers }}
       CIBW_BUILD_VERBOSITY: 1
     steps:
-      - uses: actions/checkout@v1
-      - uses: actions/setup-python@v2
-        if: ${{ !contains(matrix.os, 'self-hosted') }}
+      - uses: actions/checkout@v3
         with:
-          python-version: "3.10"
-      - uses: actions/cache@v2
-        id: cache
+          fetch-depth: 0
+      - uses: actions/setup-python@v4
         if: ${{ !contains(matrix.os, 'self-hosted') }}
         with:
-          path: ${{ env.pythonLocation }}
-          key: ${{ env.pythonLocation }}-${{ hashFiles('requirements.txt', 'requirements-dev.txt', 'setup.py') }}
+          cache: pip
+          cache-dependency-path: "pyproject.toml"
+          python-version: "3.10"
       - name: Rust Cache
         if: ${{ !contains(matrix.os, 'self-hosted') }}
-        uses: Swatinem/rust-cache@v1.3.0
+        uses: Swatinem/rust-cache@v2.4.0
         with:
           working-directory: native
       - name: Disable scmtools local scheme
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         run: >-
           echo LIBCST_NO_LOCAL_SCHEME=1 >> $GITHUB_ENV
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.2
+        uses: pypa/cibuildwheel@v2.12.3
       - uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
           name: wheels
```

### Comparing `libcst-0.4.9/.github/workflows/pypi_upload.yml` & `libcst-1.0.0/.github/workflows/pypi_upload.yml`

 * *Files 12% similar despite different names*

```diff
@@ -13,39 +13,35 @@
   build:
     uses: Instagram/LibCST/.github/workflows/build.yml@main
   upload_release:
     name: Upload wheels to pypi
     runs-on: ubuntu-latest
     needs: build
     steps:
-      - uses: actions/checkout@v1
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
       - name: Download binary wheels
         id: download
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: wheels
           path: wheelhouse
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
+          cache: pip
+          cache-dependency-path: "pyproject.toml"
           python-version: "3.10"
-      - uses: actions/cache@v2
-        id: cache
-        with:
-          path: ${{ env.pythonLocation }}
-          key: ${{ env.pythonLocation }}-${{ hashFiles('requirements.txt', 'requirements-dev.txt', 'setup.py') }}
-      - name: Install Dependencies
-        if: steps.cache.outputs.cache-hit != 'true'
-        run: |
-          pip install --upgrade --upgrade-strategy eager build -r requirements.txt -r requirements-dev.txt
-      - name: Disable scmtools local scheme
-        run: >-
-          echo LIBCST_NO_LOCAL_SCHEME=1 >> $GITHUB_ENV
+      - name: Install hatch
+        run: pip install -U hatch
       - name: Build a source tarball
+        env:
+          LIBCST_NO_LOCAL_SCHEME: 1
         run: >-
-          python -m
+          hatch run python -m
           build
           --sdist
           --outdir ${{ steps.download.outputs.download-path }}
       - name: Publish distribution 📦 to Test PyPI
         if: github.event_name == 'push'
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `libcst-0.4.9/CHANGELOG.md` & `libcst-1.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,84 @@
+# 1.0.0 - 2023-05-25
+
+The first major release of LibCST is essentially the same as 0.4.10, but using the
+newer, Rust-based parser implementation by default. The old, pure Python parser is
+scheduled for removal in the next (non-patch) release. Until then, it is available with
+the `LIBCST_PARSER_TYPE` environment variable set to `pure`.
+
+## Updated
+
+* Switch the default parser implementation to native by @zsol in https://github.com/Instagram/LibCST/pull/929
+
+# 0.4.10 - 2023-05-23
+
+## New Contributors
+* @and-semakin made their first contribution in https://github.com/Instagram/LibCST/pull/816
+* @carljm made their first contribution in https://github.com/Instagram/LibCST/pull/828
+* @sagarbadiyani made their first contribution in https://github.com/Instagram/LibCST/pull/841
+* @podtserkovskiy made their first contribution in https://github.com/Instagram/LibCST/pull/894
+* @rchen152 made their first contribution in https://github.com/Instagram/LibCST/pull/903
+* @Kludex made their first contribution in https://github.com/Instagram/LibCST/pull/913
+* @jakkdl made their first contribution in https://github.com/Instagram/LibCST/pull/921
+
+## Added
+* Add py3.11 classifier by @and-semakin in https://github.com/Instagram/LibCST/pull/816
+* Script to regenerate test fixtures, upgrade to Pyre 0.9.10 by @amyreese in https://github.com/Instagram/LibCST/pull/872
+* Allow FullyQualifiedNameProvider to work with absolute paths by @amyreese in https://github.com/Instagram/LibCST/pull/867
+* Allow running codemods without configuring in YAML by @akx in https://github.com/Instagram/LibCST/pull/879
+* Support PEP 604 in ApplyTypeAnnotationsVisitor by @hauntsaninja in https://github.com/Instagram/LibCST/pull/868
+
+## Fixed
+* fix PEP 604 union annotations in decorators by @carljm in https://github.com/Instagram/LibCST/pull/828
+* [AddImportsVisitor] Docstring Check Only for the Top Element of the Body by @sagarbadiyani in https://github.com/Instagram/LibCST/pull/841
+* Fix [#855](https://github.com/Instagram/LibCST/issues/855) - fail to parse with statement by @stroxler in https://github.com/Instagram/LibCST/pull/861
+* Add setuptools-rust to build requirements in setup.py by @amyreese in https://github.com/Instagram/LibCST/pull/873
+* Relative imports from '' package are not allowed by @podtserkovskiy in https://github.com/Instagram/LibCST/pull/894
+* Use subprocess.DEVNULL instead of opening os.devnull by hand by @akx in https://github.com/Instagram/LibCST/pull/897
+* Ensure current Python interpreter is used for subprocesses by @akx in https://github.com/Instagram/LibCST/pull/898
+* Fix ApplyTypeAnnotationsVisitor behavior on attribute assignments. by @rchen152 in https://github.com/Instagram/LibCST/pull/903
+* Fix spelling and grammar in some comments by @stroxler in https://github.com/Instagram/LibCST/pull/908
+* skip escaped backslash in rf-string by @jakkdl in https://github.com/Instagram/LibCST/pull/921
+* relax validation rules on decorators by @jakkdl in https://github.com/Instagram/LibCST/pull/926
+
+**Full Changelog**: https://github.com/Instagram/LibCST/compare/v0.4.9...v0.4.10
+
+# 0.4.9 - 2022-11-10
+
+## Updated
+* Bump setuptools-rust version by @zsol in https://github.com/Instagram/LibCST/pull/809
+
+**Full Changelog**: https://github.com/Instagram/LibCST/compare/v0.4.8...v0.4.9
+
+# 0.4.8 - 2022-11-10
+
+## New Contributors
+* @dhruvmanila made their first contribution in https://github.com/Instagram/LibCST/pull/728
+* @vfazio made their first contribution in https://github.com/Instagram/LibCST/pull/801
+* @matthewshaer made their first contribution in https://github.com/Instagram/LibCST/pull/807
+
+
+## Fixed
+* Fix parse error message for number parsing by @zzl0 in https://github.com/Instagram/LibCST/pull/724
+* Fix problematic doc build, due to the new builder image provided by readthedocs doesn't has the `graphviz-dev` package pre-installed any more by @MapleCCC in https://github.com/Instagram/LibCST/pull/751
+* Fix docstring of `FullRepoManager` by @MapleCCC in https://github.com/Instagram/LibCST/pull/750
+* Fix bug when `TypeOf` is one of options in `OneOf` / `AllOf` by @MapleCCC in https://github.com/Instagram/LibCST/pull/756
+* Tighten the metadata type of `ExpressionContextProvider` by @MapleCCC in https://github.com/Instagram/LibCST/pull/760
+* Fix the bug that the use of formatter in codemods has undetermined target Python version, resulting in hard-to-reason-with behavior by @MapleCCC in https://github.com/Instagram/LibCST/pull/771
+
+
+## Added
+* Python 3.11 rutime support
+  * test using python 3.11 beta versions by @zsol in https://github.com/Instagram/LibCST/pull/723
+  * Python 3.11 wheels by @vfazio in https://github.com/Instagram/LibCST/pull/801
+* Raise informative exception when metadata is unresolved in a metadata-based match by @MapleCCC in https://github.com/Instagram/LibCST/pull/757
+* Add AccessorProvider by @matthewshaer in https://github.com/Instagram/LibCST/pull/807
+
+**Full Changelog**: https://github.com/Instagram/LibCST/compare/v0.4.7...v0.4.8
+
 # 0.4.7 - 2022-07-12
 
 ## New Contributors
 * @Chenguang-Zhu made their first contribution in https://github.com/Instagram/LibCST/pull/720
 
 ## Fixed
 * Fix get_qualified_names_for matching on prefixes of the given name by @lpetre in https://github.com/Instagram/LibCST/pull/719
```

### Comparing `libcst-0.4.9/CODE_OF_CONDUCT.md` & `libcst-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/CONTRIBUTING.md` & `libcst-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/LICENSE` & `libcst-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/PKG-INFO` & `libcst-1.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: libcst
-Version: 0.4.9
-Summary: A concrete syntax tree with AST-like properties for Python 3.5, 3.6, 3.7, 3.8, 3.9, and 3.10 programs.
-Home-page: https://github.com/Instagram/LibCST
-License: MIT
-Project-URL: Changelog, https://github.com/Instagram/LibCST/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://libcst.readthedocs.io/en/latest/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: docs/source/_static/logo/horizontal.svg
    :width: 600 px
    :alt: LibCST
 
 A Concrete Syntax Tree (CST) parser and serializer library for Python
 
 |support-ukraine| |readthedocs-badge| |ci-badge| |codecov-badge| |pypi-badge| |pypi-download| |notebook-badge|
@@ -163,56 +144,55 @@
 - `Refactoring Python with LibCST. <https://chairnerd.seatgeek.com/refactoring-python-with-libcst/>`_
 
 Development
 -----------
 
 You'll need a recent `Rust toolchain <https://rustup.rs>`_ for developing.
 
-Then, start by setting up and activating a virtualenv:
+We recommend using `hatch <https://hatch.pypa.io/>` for running tests, linters,
+etc.
+
+Then, start by setting up and building the project:
 
 .. code-block:: shell
 
     git clone git@github.com:Instagram/LibCST.git libcst
     cd libcst
-    python3 -m venv ../libcst-env/  # just an example, put this wherever you want
-    source ../libcst-env/bin/activate
-    pip install --upgrade pip  # optional, if you have an old system version of pip
-    pip install -r requirements.txt -r requirements-dev.txt
-    # If you're done with the virtualenv, you can leave it by running:
-    deactivate
+    hatch env create
 
-We use `ufmt <https://ufmt.omnilib.dev/en/stable/>`_ to format code. To format
-changes to be conformant, run the following in the root:
+To run the project's test suite, you can:
 
 .. code-block:: shell
 
-    ufmt format && python -m fixit.cli.apply_fix
+    hatch run test
 
-We use `slotscheck <https://slotscheck.rtfd.io>`_ to check the correctness
-of class ``__slots__``. To check that slots are defined properly, run:
+You can also run individual tests by using unittest and specifying a module like
+this:
 
 .. code-block:: shell
 
-    python -m slotscheck libcst
+    hatch run python -m unittest libcst.tests.test_batched_visitor
+
+See the `unittest documentation <https://docs.python.org/3/library/unittest.html>`_
+for more examples of how to run tests.
 
-To run all tests, you'll need to do the following in the root:
+We have multiple linters, including copyright checks and
+`slotscheck <https://slotscheck.rtfd.io>`_ to check the correctness of class
+``__slots__``. To run all of the linters:
 
 .. code-block:: shell
 
-    python -m unittest
+    hatch run lint
 
-You can also run individual tests by using unittest and specifying a module like
-this:
+We use `ufmt <https://ufmt.omnilib.dev/en/stable/>`_ to format code. To format
+changes to be conformant, run the following in the root:
 
 .. code-block:: shell
 
-    python -m unittest libcst.tests.test_batched_visitor
-
-See the `unittest documentation <https://docs.python.org/3/library/unittest.html>`_
-for more examples of how to run tests.
+    hatch run format
 
 Building
 ~~~~~~~~
 
 In order to build LibCST, which includes a native parser module, you
 will need to have the Rust build tool ``cargo`` on your path. You can
 usually install ``cargo`` using your system package manager, but the
@@ -222,44 +202,39 @@
 To build just the native parser, do the following from the ``native``
 directory:
 
 .. code-block:: shell
 
     cargo build
 
-To build the ``libcst.native`` module and install ``libcst``, run this
-from the root:
+To rebuild the ``libcst.native`` module, from the repo root:
 
 .. code-block:: shell
 
-    pip uninstall -y libcst
-    pip install -e .
+    hatch env prune && hatch env create
 
 Type Checking
 ~~~~~~~~~~~~~
 
 We use `Pyre <https://github.com/facebook/pyre-check>`_ for type-checking.
 
 To verify types for the library, do the following in the root:
 
 .. code-block:: shell
 
-    pyre check
-
-*Note:* You may need to run the ``pip install -e .`` command prior
-to type checking, see the section above on building.
+    hatch run typecheck
 
 Generating Documents
 ~~~~~~~~~~~~~~~~~~~~
 
 To generate documents, do the following in the root:
 
 .. code-block:: shell
 
-    sphinx-build docs/source/ docs/build/
+    hatch run docs
 
 Future
 ======
 
 - Advanced full repository facts providers like fully qualified name and call graph.
 
 License
```

### Comparing `libcst-0.4.9/docs/source/_static/img/python_scopes.png` & `libcst-1.0.0/docs/source/_static/img/python_scopes.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/img/python_scopes.svg` & `libcst-1.0.0/docs/source/_static/img/python_scopes.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/favicon.ico` & `libcst-1.0.0/docs/source/_static/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/favicon.svg` & `libcst-1.0.0/docs/source/_static/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/favicon_16px.png` & `libcst-1.0.0/docs/source/_static/logo/favicon_16px.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/favicon_32px.png` & `libcst-1.0.0/docs/source/_static/logo/favicon_32px.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/horizontal.svg` & `libcst-1.0.0/docs/source/_static/logo/horizontal.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/horizontal_white.svg` & `libcst-1.0.0/docs/source/_static/logo/horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/horizontal_white_sidebar.png` & `libcst-1.0.0/docs/source/_static/logo/horizontal_white_sidebar.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/icon.svg` & `libcst-1.0.0/docs/source/_static/logo/icon.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/icon_white.svg` & `libcst-1.0.0/docs/source/_static/logo/icon_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/vertical.svg` & `libcst-1.0.0/docs/source/_static/logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/_static/logo/vertical_white.svg` & `libcst-1.0.0/docs/source/_static/logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/best_practices.rst` & `libcst-1.0.0/docs/source/best_practices.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/codemods.rst` & `libcst-1.0.0/docs/source/codemods.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/codemods_tutorial.rst` & `libcst-1.0.0/docs/source/codemods_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/conf.py` & `libcst-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/helpers.rst` & `libcst-1.0.0/docs/source/helpers.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/index.rst` & `libcst-1.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/matchers.rst` & `libcst-1.0.0/docs/source/matchers.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/matchers_tutorial.ipynb` & `libcst-1.0.0/docs/source/matchers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/metadata.rst` & `libcst-1.0.0/docs/source/metadata.rst`

 * *Files 1% similar despite different names*

```diff
@@ -222,23 +222,31 @@
 tree traversal is doable. Sometimes user may want to access the parent :class:`~libcst.CSTNode`
 for more information or traverse in bottom-up manner.
 We provide :class:`~libcst.metadata.ParentNodeProvider` for those use cases.
 
 .. autoclass:: libcst.metadata.ParentNodeProvider
    :no-undoc-members:
 
+File Path Metadata
+------------------
+This provides the absolute file path on disk for any module being visited.
+Requires an active :class:`~libcst.metadata.FullRepoManager` when using this provider.
+
+.. autoclass:: libcst.metadata.FilePathProvider
+   :no-undoc-members:
+
 Type Inference Metadata
 -----------------------
 `Type inference <https://en.wikipedia.org/wiki/Type_inference>`__ is to automatically infer
 data types of expression for deeper understanding source code.
 In Python, type checkers like `Mypy <https://github.com/python/mypy>`_ or
 `Pyre <https://pyre-check.org/>`__ analyze `type annotations <https://docs.python.org/3/library/typing.html>`__
 and infer types for expressions.
 :class:`~libcst.metadata.TypeInferenceProvider` is provided by `Pyre Query API <https://pyre-check.org/docs/querying-pyre.html>`__
-which requires `setup watchman <https://pyre-check.org/docs/watchman-integration.html>`_ for incremental typechecking.
+which requires `setup watchman <https://pyre-check.org/docs/getting-started/>`_ for incremental typechecking.
 :class:`~libcst.metadata.FullRepoManger` is built for manage the inter process communication to Pyre.
 
 .. autoclass:: libcst.metadata.TypeInferenceProvider
    :no-undoc-members:
 
 .. autoclass:: libcst.metadata.FullRepoManager
    :no-undoc-members:
```

### Comparing `libcst-0.4.9/docs/source/metadata_tutorial.ipynb` & `libcst-1.0.0/docs/source/metadata_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/motivation.rst` & `libcst-1.0.0/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/nodes.rst` & `libcst-1.0.0/docs/source/nodes.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/parser.rst` & `libcst-1.0.0/docs/source/parser.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/scope_tutorial.ipynb` & `libcst-1.0.0/docs/source/scope_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/tutorial.ipynb` & `libcst-1.0.0/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/visitors.rst` & `libcst-1.0.0/docs/source/visitors.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/docs/source/why_libcst.rst` & `libcst-1.0.0/docs/source/why_libcst.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/__init__.py` & `libcst-1.0.0/libcst/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_add_slots.py` & `libcst-1.0.0/libcst/_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_batched_visitor.py` & `libcst-1.0.0/libcst/_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_exceptions.py` & `libcst-1.0.0/libcst/_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_flatten_sentinel.py` & `libcst-1.0.0/libcst/_flatten_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_maybe_sentinel.py` & `libcst-1.0.0/libcst/_maybe_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_metadata_dependent.py` & `libcst-1.0.0/libcst/_metadata_dependent.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/base.py` & `libcst-1.0.0/libcst/_nodes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         return val.deep_clone()
     except AttributeError:
         return deepcopy(val)
 
 
 @dataclass(frozen=True)
 class CSTNode(ABC):
-
     __slots__: ClassVar[Sequence[str]] = ()
 
     def __post_init__(self) -> None:
         # PERF: It might make more sense to move validation work into the visitor, which
         # would allow us to avoid validating the tree when parsing a file.
         self._validate()
 
@@ -467,15 +466,14 @@
         """
         # pyre-ignore Pyre is complaining about CSTNode not being instantiable,
         # but we're only going to call this from concrete subclasses.
         return field(default_factory=lambda: cls(*args, **kwargs))
 
 
 class BaseLeaf(CSTNode, ABC):
-
     __slots__ = ()
 
     @property
     def children(self) -> Sequence[CSTNode]:
         # override this with an optimized implementation
         return _EMPTY_SEQUENCE
```

### Comparing `libcst-0.4.9/libcst/_nodes/deep_equals.py` & `libcst-1.0.0/libcst/_nodes/deep_equals.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/expression.py` & `libcst-1.0.0/libcst/_nodes/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         )
 
     def _validate(self) -> None:
         super(Name, self)._validate()
         if len(self.value) == 0:
             raise CSTValidationError("Cannot have empty name identifier.")
         if not self.value.isidentifier():
-            raise CSTValidationError("Name is not a valid identifier.")
+            raise CSTValidationError(f"Name {self.value!r} is not a valid identifier.")
 
     def _codegen_impl(self, state: CodegenState) -> None:
         with self._parenthesize(state):
             state.add_token(self.value)
 
 
 @add_slots
@@ -531,15 +531,14 @@
     __slots__ = ()
 
 
 StringQuoteLiteral = Literal['"', "'", '"""', "'''"]
 
 
 class _BasePrefixedString(BaseString, ABC):
-
     __slots__ = ()
 
     @property
     def prefix(self) -> str:
         """
         Returns the string's prefix, if any exists.
```

### Comparing `libcst-0.4.9/libcst/_nodes/internal.py` & `libcst-1.0.0/libcst/_nodes/internal.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/module.py` & `libcst-1.0.0/libcst/_nodes/module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/op.py` & `libcst-1.0.0/libcst/_nodes/op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/statement.py` & `libcst-1.0.0/libcst/_nodes/statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     Annotation,
     Arg,
     Asynchronous,
     Attribute,
     BaseAssignTargetExpression,
     BaseDelTargetExpression,
     BaseExpression,
-    Call,
     ConcatenatedString,
     ExpressionPosition,
     From,
     LeftCurlyBrace,
     LeftParen,
     LeftSquareBracket,
     List,
@@ -1615,40 +1614,27 @@
 class Decorator(CSTNode):
     """
     A single decorator that decorates a :class:`FunctionDef` or a :class:`ClassDef`.
     """
 
     #: The decorator that will return a new function wrapping the parent
     #: of this decorator.
-    decorator: Union[Name, Attribute, Call]
+    decorator: BaseExpression
 
     #: Line comments and empty lines before this decorator. The parent
     #: :class:`FunctionDef` or :class:`ClassDef` node owns leading lines before
     #: the first decorator so that if the first decorator is removed, spacing is preserved.
     leading_lines: Sequence[EmptyLine] = ()
 
     #: Whitespace after the ``@`` and before the decorator expression itself.
     whitespace_after_at: SimpleWhitespace = SimpleWhitespace.field("")
 
     #: Optional trailing comment and newline following the decorator before the next line.
     trailing_whitespace: TrailingWhitespace = TrailingWhitespace.field()
 
-    def _validate(self) -> None:
-        decorator = self.decorator
-        if len(decorator.lpar) > 0 or len(decorator.rpar) > 0:
-            raise CSTValidationError(
-                "Cannot have parens around decorator in a Decorator."
-            )
-        if isinstance(decorator, Call) and not isinstance(
-            decorator.func, (Name, Attribute)
-        ):
-            raise CSTValidationError(
-                "Decorator call function must be Name or Attribute node."
-            )
-
     def _visit_and_replace_children(self, visitor: CSTVisitorT) -> "Decorator":
         return Decorator(
             leading_lines=visit_sequence(
                 self, "leading_lines", self.leading_lines, visitor
             ),
             whitespace_after_at=visit_required(
                 self, "whitespace_after_at", self.whitespace_after_at, visitor
```

### Comparing `libcst-0.4.9/libcst/_nodes/tests/base.py` & `libcst-1.0.0/libcst/_nodes/tests/base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_assert.py` & `libcst-1.0.0/libcst/_nodes/tests/test_assert.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_assign.py` & `libcst-1.0.0/libcst/_nodes/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_atom.py` & `libcst-1.0.0/libcst/_nodes/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_attribute.py` & `libcst-1.0.0/libcst/_nodes/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_await.py` & `libcst-1.0.0/libcst/_nodes/tests/test_await.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_binary_op.py` & `libcst-1.0.0/libcst/_nodes/tests/test_binary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_boolean_op.py` & `libcst-1.0.0/libcst/_nodes/tests/test_boolean_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_call.py` & `libcst-1.0.0/libcst/_nodes/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_classdef.py` & `libcst-1.0.0/libcst/_nodes/tests/test_classdef.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_comment.py` & `libcst-1.0.0/libcst/_nodes/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_comparison.py` & `libcst-1.0.0/libcst/_nodes/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_cst_node.py` & `libcst-1.0.0/libcst/_nodes/tests/test_cst_node.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_del.py` & `libcst-1.0.0/libcst/_nodes/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_dict.py` & `libcst-1.0.0/libcst/_nodes/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_dict_comp.py` & `libcst-1.0.0/libcst/_nodes/tests/test_dict_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_docstring.py` & `libcst-1.0.0/libcst/_nodes/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_else.py` & `libcst-1.0.0/libcst/_nodes/tests/test_else.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_empty_line.py` & `libcst-1.0.0/libcst/_nodes/tests/test_empty_line.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_flatten_behavior.py` & `libcst-1.0.0/libcst/_nodes/tests/test_flatten_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_for.py` & `libcst-1.0.0/libcst/_nodes/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_funcdef.py` & `libcst-1.0.0/libcst/_nodes/tests/test_funcdef.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,14 +619,54 @@
                         whitespace_after_func=cst.SimpleWhitespace(" "),
                         whitespace_before_args=cst.SimpleWhitespace("  "),
                     ),
                 ),
                 "code": "@ bar (  )\n",
                 "expected_position": CodeRange((1, 0), (1, 10)),
             },
+            # Allow nested calls on decorator
+            {
+                "node": cst.FunctionDef(
+                    cst.Name("foo"),
+                    cst.Parameters(),
+                    cst.SimpleStatementSuite((cst.Pass(),)),
+                    (cst.Decorator(cst.Call(func=cst.Call(func=cst.Name("bar")))),),
+                ),
+                "code": "@bar()()\ndef foo(): pass\n",
+            },
+            # Allow any expression in decorator
+            {
+                "node": cst.FunctionDef(
+                    cst.Name("foo"),
+                    cst.Parameters(),
+                    cst.SimpleStatementSuite((cst.Pass(),)),
+                    (
+                        cst.Decorator(
+                            cst.BinaryOperation(cst.Name("a"), cst.Add(), cst.Name("b"))
+                        ),
+                    ),
+                ),
+                "code": "@a + b\ndef foo(): pass\n",
+            },
+            # Allow parentheses around decorator
+            {
+                "node": cst.FunctionDef(
+                    cst.Name("foo"),
+                    cst.Parameters(),
+                    cst.SimpleStatementSuite((cst.Pass(),)),
+                    (
+                        cst.Decorator(
+                            cst.Name(
+                                "bar", lpar=(cst.LeftParen(),), rpar=(cst.RightParen(),)
+                            )
+                        ),
+                    ),
+                ),
+                "code": "@(bar)\ndef foo(): pass\n",
+            },
             # Parameters
             {
                 "node": cst.Parameters(
                     params=(
                         cst.Param(cst.Name("first")),
                         cst.Param(cst.Name("second")),
                         cst.Param(cst.Name("third"), default=cst.Float("1.0")),
@@ -918,30 +958,14 @@
                 lambda: cst.FunctionDef(
                     cst.Name("foo"),
                     cst.Parameters(star_kwarg=cst.Param(cst.Name("bar"), star="*")),
                     cst.SimpleStatementSuite((cst.Pass(),)),
                 ),
                 r"Expecting a star prefix of '\*\*'",
             ),
-            # Validate decorator name semantics
-            (
-                lambda: cst.FunctionDef(
-                    cst.Name("foo"),
-                    cst.Parameters(),
-                    cst.SimpleStatementSuite((cst.Pass(),)),
-                    (
-                        cst.Decorator(
-                            cst.Name(
-                                "bar", lpar=(cst.LeftParen(),), rpar=(cst.RightParen(),)
-                            )
-                        ),
-                    ),
-                ),
-                "Cannot have parens around decorator in a Decorator",
-            ),
         )
     )
     def test_invalid(
         self, get_node: Callable[[], cst.CSTNode], expected_re: str
     ) -> None:
         self.assert_invalid(get_node, expected_re)
```

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_global.py` & `libcst-1.0.0/libcst/_nodes/tests/test_global.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_if.py` & `libcst-1.0.0/libcst/_nodes/tests/test_if.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_ifexp.py` & `libcst-1.0.0/libcst/_nodes/tests/test_ifexp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_import.py` & `libcst-1.0.0/libcst/_nodes/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_indented_block.py` & `libcst-1.0.0/libcst/_nodes/tests/test_indented_block.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_lambda.py` & `libcst-1.0.0/libcst/_nodes/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_leaf_small_statements.py` & `libcst-1.0.0/libcst/_nodes/tests/test_leaf_small_statements.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_list.py` & `libcst-1.0.0/libcst/_nodes/tests/test_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from libcst._nodes.tests.base import CSTNodeTest, parse_expression_as
 from libcst._parser.entrypoints import is_native
 from libcst.metadata import CodeRange
 from libcst.testing.utils import data_provider
 
 
 class ListTest(CSTNodeTest):
-
     # A lot of Element/StarredElement tests are provided by the tests for Tuple, so we
     # we don't need to duplicate them here.
     @data_provider(
         [
             # zero-element list
             {"node": cst.List([]), "code": "[]", "parser": parse_expression},
             # one-element list, sentinel comma value
```

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_match.py` & `libcst-1.0.0/libcst/_nodes/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_matrix_multiply.py` & `libcst-1.0.0/libcst/_nodes/tests/test_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_module.py` & `libcst-1.0.0/libcst/_nodes/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_namedexpr.py` & `libcst-1.0.0/libcst/_nodes/tests/test_namedexpr.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_newline.py` & `libcst-1.0.0/libcst/_nodes/tests/test_newline.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_nonlocal.py` & `libcst-1.0.0/libcst/_nodes/tests/test_nonlocal.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_number.py` & `libcst-1.0.0/libcst/_nodes/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_raise.py` & `libcst-1.0.0/libcst/_nodes/tests/test_raise.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_removal_behavior.py` & `libcst-1.0.0/libcst/_nodes/tests/test_removal_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_return.py` & `libcst-1.0.0/libcst/_nodes/tests/test_return.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_set.py` & `libcst-1.0.0/libcst/_nodes/tests/test_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from libcst import parse_expression
 from libcst._nodes.tests.base import CSTNodeTest, parse_expression_as
 from libcst._parser.entrypoints import is_native
 from libcst.testing.utils import data_provider
 
 
 class ListTest(CSTNodeTest):
-
     # A lot of Element/StarredElement tests are provided by the tests for Tuple, so we
     # we don't need to duplicate them here.
     @data_provider(
         [
             # one-element list, sentinel comma value
             {
                 "node": cst.Set([cst.Element(cst.Name("single_element"))]),
```

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_simple_comp.py` & `libcst-1.0.0/libcst/_nodes/tests/test_simple_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_simple_statement.py` & `libcst-1.0.0/libcst/_nodes/tests/test_simple_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_simple_string.py` & `libcst-1.0.0/libcst/_nodes/tests/test_simple_string.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_simple_whitespace.py` & `libcst-1.0.0/libcst/_nodes/tests/test_simple_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_small_statement.py` & `libcst-1.0.0/libcst/_nodes/tests/test_small_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_subscript.py` & `libcst-1.0.0/libcst/_nodes/tests/test_subscript.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_trailing_whitespace.py` & `libcst-1.0.0/libcst/_nodes/tests/test_trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_try.py` & `libcst-1.0.0/libcst/_nodes/tests/test_try.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_tuple.py` & `libcst-1.0.0/libcst/_nodes/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_unary_op.py` & `libcst-1.0.0/libcst/_nodes/tests/test_unary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_while.py` & `libcst-1.0.0/libcst/_nodes/tests/test_while.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_with.py` & `libcst-1.0.0/libcst/_nodes/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/tests/test_yield.py` & `libcst-1.0.0/libcst/_nodes/tests/test_yield.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_nodes/whitespace.py` & `libcst-1.0.0/libcst/_nodes/whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/base_parser.py` & `libcst-1.0.0/libcst/_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/README.md` & `libcst-1.0.0/libcst/_parser/conversions/README.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/expression.py` & `libcst-1.0.0/libcst/_parser/conversions/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/module.py` & `libcst-1.0.0/libcst/_parser/conversions/module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/params.py` & `libcst-1.0.0/libcst/_parser/conversions/params.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/statement.py` & `libcst-1.0.0/libcst/_parser/conversions/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/conversions/terminals.py` & `libcst-1.0.0/libcst/_parser/conversions/terminals.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/custom_itertools.py` & `libcst-1.0.0/libcst/_parser/custom_itertools.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/detect_config.py` & `libcst-1.0.0/libcst/_parser/detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/entrypoints.py` & `libcst-1.0.0/libcst/_parser/entrypoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libcst._parser.types.config import PartialParserConfig
 
 _DEFAULT_PARTIAL_PARSER_CONFIG: PartialParserConfig = PartialParserConfig()
 
 
 def is_native() -> bool:
     typ = os.environ.get("LIBCST_PARSER_TYPE")
-    return typ == "native"
+    return typ != "pure"
 
 
 def _parse(
     entrypoint: str,
     source: Union[str, bytes],
     config: PartialParserConfig,
     *,
```

### Comparing `libcst-0.4.9/libcst/_parser/grammar.py` & `libcst-1.0.0/libcst/_parser/grammar.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/pgen2/generator.py` & `libcst-1.0.0/libcst/_parser/parso/pgen2/generator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/pgen2/grammar_parser.py` & `libcst-1.0.0/libcst/_parser/parso/pgen2/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/python/py_token.py` & `libcst-1.0.0/libcst/_parser/parso/python/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/python/token.py` & `libcst-1.0.0/libcst/_parser/parso/python/token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/python/tokenize.py` & `libcst-1.0.0/libcst/_parser/parso/python/tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/tests/test_fstring.py` & `libcst-1.0.0/libcst/_parser/parso/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/tests/test_tokenize.py` & `libcst-1.0.0/libcst/_parser/parso/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/tests/test_utils.py` & `libcst-1.0.0/libcst/_parser/parso/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/parso/utils.py` & `libcst-1.0.0/libcst/_parser/parso/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/production_decorator.py` & `libcst-1.0.0/libcst/_parser/production_decorator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/py_whitespace_parser.py` & `libcst-1.0.0/libcst/_parser/py_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/python_parser.py` & `libcst-1.0.0/libcst/_parser/python_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_config.py` & `libcst-1.0.0/libcst/_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_detect_config.py` & `libcst-1.0.0/libcst/_parser/tests/test_detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_footer_behavior.py` & `libcst-1.0.0/libcst/_parser/tests/test_footer_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_node_identity.py` & `libcst-1.0.0/libcst/_parser/tests/test_node_identity.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_parse_errors.py` & `libcst-1.0.0/libcst/_parser/tests/test_parse_errors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_version_compare.py` & `libcst-1.0.0/libcst/_parser/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_whitespace_parser.py` & `libcst-1.0.0/libcst/_parser/tests/test_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/tests/test_wrapped_tokenize.py` & `libcst-1.0.0/libcst/_parser/tests/test_wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/config.py` & `libcst-1.0.0/libcst/_parser/types/config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/conversions.py` & `libcst-1.0.0/libcst/_parser/types/conversions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/partials.py` & `libcst-1.0.0/libcst/_parser/types/partials.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/py_config.py` & `libcst-1.0.0/libcst/_parser/types/py_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/py_token.py` & `libcst-1.0.0/libcst/_parser/types/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/py_whitespace_state.py` & `libcst-1.0.0/libcst/_parser/types/py_whitespace_state.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/types/tests/test_config.py` & `libcst-1.0.0/libcst/_parser/types/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/whitespace_parser.py` & `libcst-1.0.0/libcst/_parser/whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_parser/wrapped_tokenize.py` & `libcst-1.0.0/libcst/_parser/wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_position.py` & `libcst-1.0.0/libcst/_position.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_removal_sentinel.py` & `libcst-1.0.0/libcst/_removal_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_tabs.py` & `libcst-1.0.0/libcst/_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_type_enforce.py` & `libcst-1.0.0/libcst/_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_typed_visitor.py` & `libcst-1.0.0/libcst/_typed_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_typed_visitor_base.py` & `libcst-1.0.0/libcst/_typed_visitor_base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/_visitors.py` & `libcst-1.0.0/libcst/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/gather.py` & `libcst-1.0.0/libcst/codegen/gather.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/gen_matcher_classes.py` & `libcst-1.0.0/libcst/codegen/gen_matcher_classes.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/gen_type_mapping.py` & `libcst-1.0.0/libcst/codegen/gen_type_mapping.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/gen_visitor_functions.py` & `libcst-1.0.0/libcst/codegen/gen_visitor_functions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/generate.py` & `libcst-1.0.0/libcst/codegen/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,19 @@
 from libcst.codegen.transforms import (
     DoubleQuoteForwardRefsTransformer,
     SimplifyUnionsTransformer,
 )
 
 
 def format_file(fname: str) -> None:
-    with open(os.devnull, "w") as devnull:
-        subprocess.check_call(["ufmt", "format", fname], stdout=devnull, stderr=devnull)
+    subprocess.check_call(
+        ["ufmt", "format", fname],
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
 
 
 def clean_generated_code(code: str) -> str:
     """
     Generalized sanity clean-up for all codegen so we can fix issues such as
     Union[SingleType]. The transforms found here are strictly for form and
     do not affect functionality.
@@ -61,20 +64,19 @@
         new_code = clean_generated_code("\n".join(visitor_codegen.generated_code))
         with open(visitors_file, "w") as fp:
             fp.write(new_code)
             fp.close()
 
         # Now, see if the file we generated causes any import errors
         # by attempting to run codegen again in a new process.
-        with open(os.devnull, "w") as devnull:
-            subprocess.check_call(
-                ["python3", "-m", "libcst.codegen.gen_visitor_functions"],
-                cwd=base,
-                stdout=devnull,
-            )
+        subprocess.check_call(
+            [sys.executable, "-m", "libcst.codegen.gen_visitor_functions"],
+            cwd=base,
+            stdout=subprocess.DEVNULL,
+        )
 
         # If it worked, lets format the file
         format_file(visitors_file)
 
         # Since we were successful with importing, we can remove the backup.
         os.remove(f"{visitors_file}.bak")
```

### Comparing `libcst-0.4.9/libcst/codegen/tests/test_codegen_clean.py` & `libcst-1.0.0/libcst/codegen/tests/test_codegen_clean.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codegen/transforms.py` & `libcst-1.0.0/libcst/codegen/transforms.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/__init__.py` & `libcst-1.0.0/libcst/codemod/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_cli.py` & `libcst-1.0.0/libcst/codemod/_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_codemod.py` & `libcst-1.0.0/libcst/codemod/_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_command.py` & `libcst-1.0.0/libcst/codemod/_command.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_context.py` & `libcst-1.0.0/libcst/codemod/_context.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_dummy_pool.py` & `libcst-1.0.0/libcst/codemod/_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_runner.py` & `libcst-1.0.0/libcst/codemod/_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_testing.py` & `libcst-1.0.0/libcst/codemod/_testing.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/_visitor.py` & `libcst-1.0.0/libcst/codemod/_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/add_pyre_directive.py` & `libcst-1.0.0/libcst/codemod/commands/add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/add_trailing_commas.py` & `libcst-1.0.0/libcst/codemod/commands/add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/convert_format_to_fstring.py` & `libcst-1.0.0/libcst/codemod/commands/convert_format_to_fstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,14 @@
                 pass
 
         # Either failed to parse the new string, or don't need to make changes.
         return updated_node
 
 
 class ConvertFormatStringCommand(VisitorBasedCodemodCommand):
-
     DESCRIPTION: str = "Converts instances of str.format() to f-string."
 
     @staticmethod
     def add_args(arg_parser: argparse.ArgumentParser) -> None:
         arg_parser.add_argument(
             "--allow-strip-comments",
             dest="allow_strip_comments",
@@ -267,15 +266,15 @@
             ),
         )
         if extraction is not None:
             fstring: List[cst.BaseFormattedStringContent] = []
             inserted_sequence: int = 0
             stringnode = cst.ensure_type(extraction["string"], cst.SimpleString)
             tokens = _get_tokens(stringnode.raw_value)
-            for (literal_text, field_name, format_spec, conversion) in tokens:
+            for literal_text, field_name, format_spec, conversion in tokens:
                 if literal_text:
                     fstring.append(cst.FormattedStringText(literal_text))
                 if field_name is None:
                     # This is not a format-specification
                     continue
                 # Auto-insert field sequence if it is empty
                 if field_name == "":
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/convert_namedtuple_to_dataclass.py` & `libcst-1.0.0/libcst/codemod/commands/convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/convert_percent_format_to_fstring.py` & `libcst-1.0.0/libcst/codemod/commands/convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/convert_type_comments.py` & `libcst-1.0.0/libcst/codemod/commands/convert_type_comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,15 +702,15 @@
     #
     # As a result, we use two different patterns:
     # (A) we aggressively strip out type comments from whitespace between the
     #     start of a function define and the start of the body, whenever we were
     #     able to extract type information. This is done via mutable state and the
     #     usual visitor pattern.
     # (B) we also manually reach down to the first statement inside of the
-    #     funciton body and aggressively strip type comments from leading
+    #     function body and aggressively strip type comments from leading
     #     whitespaces
     #
     # PEP 484 underspecifies how to apply type comments to (non-static)
     # methods - it would be possible to provide a type for `self`, or to omit
     # it. So we accept either approach when interpreting type comments on
     # non-static methods: the first argument an have a type provided or not.
 
@@ -782,15 +782,15 @@
         else:
             return updated_node
 
     def visit_FunctionDef_body(
         self,
         node: cst.FunctionDef,
     ) -> None:
-        "Turn off aggressive type comment removal when we've leaved the header."
+        "Turn off aggressive type comment removal when we've left the header."
         self.aggressively_strip_type_comments = False
 
     def leave_IndentedBlock(
         self,
         original_node: cst.IndentedBlock,
         updated_node: cst.IndentedBlock,
     ) -> cst.IndentedBlock:
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/ensure_import_present.py` & `libcst-1.0.0/libcst/codemod/commands/ensure_import_present.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Generator, Type
 
 from libcst.codemod import Codemod, MagicArgsCodemodCommand
 from libcst.codemod.visitors import AddImportsVisitor
 
 
 class EnsureImportPresentCommand(MagicArgsCodemodCommand):
-
     DESCRIPTION: str = (
         "Given a module and possibly an entity in that module, add an import "
         + "as long as one does not already exist."
     )
 
     @staticmethod
     def add_args(arg_parser: argparse.ArgumentParser) -> None:
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/fix_pyre_directives.py` & `libcst-1.0.0/libcst/codemod/commands/fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/remove_pyre_directive.py` & `libcst-1.0.0/libcst/codemod/commands/remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/remove_unused_imports.py` & `libcst-1.0.0/libcst/codemod/commands/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/rename.py` & `libcst-1.0.0/libcst/codemod/commands/rename.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
         else:
             new_names = []
             for import_alias in names:
                 alias_name = get_full_name_for_node(import_alias.name)
                 if alias_name is not None:
                     qual_name = f"{imported_module_name}.{alias_name}"
                     if self.old_name == qual_name:
-
                         replacement_module = self.gen_replacement_module(
                             imported_module_name
                         )
                         replacement_obj = self.gen_replacement(alias_name)
                         if not replacement_obj:
                             # The user has requested an `import` statement rather than an `from ... import`.
                             # This will be taken care of in `leave_Module`, in the meantime, schedule for potential removal.
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/strip_strings_from_types.py` & `libcst-1.0.0/libcst/codemod/commands/strip_strings_from_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from libcst import parse_expression
 from libcst.codemod import VisitorBasedCodemodCommand
 from libcst.codemod.visitors import AddImportsVisitor
 from libcst.metadata import QualifiedNameProvider
 
 
 class StripStringsCommand(VisitorBasedCodemodCommand):
-
     DESCRIPTION: str = (
         "Converts string type annotations to 3.7-compatible forward references."
     )
 
     METADATA_DEPENDENCIES = (QualifiedNameProvider,)
 
     # We want to gate the SimpleString visitor below to only SimpleStrings inside
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_add_pyre_directive.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_add_pyre_directive.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.add_pyre_directive import AddPyreUnsafeCommand
 
 
 class TestAddPyreUnsafeCommand(CodemodTest):
-
     TRANSFORM = AddPyreUnsafeCommand
 
     def test_add_to_file(self) -> None:
         before = """
             def baz() -> List[Foo]:
                 pass
         """
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_add_trailing_commas.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_format_to_fstring.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_format_to_fstring.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.convert_format_to_fstring import ConvertFormatStringCommand
 
 
 class ConvertFormatStringCommandTest(CodemodTest):
-
     TRANSFORM = ConvertFormatStringCommand
 
     def test_noop(self) -> None:
         """
         Should do nothing, since there's nothing to do.
         """
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.convert_namedtuple_to_dataclass import (
     ConvertNamedTupleToDataclassCommand,
 )
 
 
 class ConvertNamedTupleToDataclassCommandTest(CodemodTest):
-
     TRANSFORM = ConvertNamedTupleToDataclassCommand
 
     def test_no_change(self) -> None:
         """
         Should result in no change as there are no children of NamedTuple.
         """
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_type_comments.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_convert_type_comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Any
 
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.convert_type_comments import ConvertTypeComments
 
 
 class TestConvertTypeCommentsBase(CodemodTest):
-
     maxDiff = 1500
     TRANSFORM = ConvertTypeComments
 
     def assertCodemod39Plus(self, before: str, after: str, **kwargs: Any) -> None:
         """
         Assert that the codemod works on Python 3.9+, and that we raise
         a NotImplementedError on other Python versions.
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_ensure_import_present.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_fix_pyre_directives.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_fix_pyre_directives.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.fix_pyre_directives import FixPyreDirectivesCommand
 
 
 class TestFixPyreDirectivesCommand(CodemodTest):
-
     TRANSFORM = FixPyreDirectivesCommand
 
     def test_no_need_to_fix_simple(self) -> None:
         """
         Tests that a pyre-strict inside the module header doesn't get touched.
         """
         before = """
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_noop.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_noop.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.noop import NOOPCommand
 
 
 class TestNOOPCodemod(CodemodTest):
-
     TRANSFORM = NOOPCommand
 
     def test_noop(self) -> None:
         before = """
             foo: str = ""
 
             class Class:
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_remove_pyre_directive.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_remove_pyre_directive.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from libcst.codemod.commands.remove_pyre_directive import (
     RemovePyreStrictCommand,
     RemovePyreUnsafeCommand,
 )
 
 
 class TestRemovePyreStrictCommand(CodemodTest):
-
     TRANSFORM = RemovePyreStrictCommand
 
     def test_remove_from_file(self) -> None:
         before = """
             # pyre-strict
             def baz() -> List[Foo]:
                 pass
@@ -93,15 +92,14 @@
             def baz() -> List[Foo]:
                 pass
         """
         self.assertCodemod(before, after)
 
 
 class TestRemovePyreUnsafeCommand(CodemodTest):
-
     TRANSFORM = RemovePyreUnsafeCommand
 
     def test_remove_from_file(self) -> None:
         before = """
             # pyre-unsafe
             def baz() -> List[Foo]:
                 pass
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_remove_unused_imports.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_rename.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 # pyre-strict
 
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.rename import RenameCommand
 
 
 class TestRenameCommand(CodemodTest):
-
     TRANSFORM = RenameCommand
 
     def test_rename_name(self) -> None:
-
         before = """
             from foo import bar
 
             def test() -> None:
                 bar(5)
         """
         after = """
@@ -27,15 +25,14 @@
             def test() -> None:
                 qux(5)
         """
 
         self.assertCodemod(before, after, old_name="foo.bar", new_name="baz.qux")
 
     def test_rename_name_asname(self) -> None:
-
         before = """
             from foo import bar as bla
 
             def test() -> None:
                 bla(5)
         """
         after = """
@@ -69,15 +66,14 @@
             before,
             after,
             old_name="foo.foo",
             new_name="baz.qux",
         )
 
     def test_rename_attr(self) -> None:
-
         before = """
             import a.b
 
             def test() -> None:
                 a.b.c(5)
         """
         after = """
@@ -91,15 +87,14 @@
             before,
             after,
             old_name="a.b.c",
             new_name="d.e.f",
         )
 
     def test_rename_attr_asname(self) -> None:
-
         before = """
             import foo as bar
 
             def test() -> None:
                 bar.qux(5)
         """
         after = """
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_strip_strings_from_types.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_strip_strings_from_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodTest
 from libcst.codemod.commands.strip_strings_from_types import StripStringsCommand
 
 
 class TestStripStringsCodemod(CodemodTest):
-
     TRANSFORM = StripStringsCommand
 
     def test_noop(self) -> None:
         before = """
             foo: str = ""
 
             class Class:
```

### Comparing `libcst-0.4.9/libcst/codemod/commands/tests/test_unnecessary_format_string.py` & `libcst-1.0.0/libcst/codemod/commands/tests/test_unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/commands/unnecessary_format_string.py` & `libcst-1.0.0/libcst/codemod/commands/unnecessary_format_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #
 import libcst
 import libcst.matchers as m
 from libcst.codemod import VisitorBasedCodemodCommand
 
 
 class UnnecessaryFormatString(VisitorBasedCodemodCommand):
-
     DESCRIPTION: str = (
         "Converts f-strings which perform no formatting to regular strings."
     )
 
     @m.leave(m.FormattedString(parts=(m.FormattedStringText(),)))
     def _check_formatted_string(
         self,
```

### Comparing `libcst-0.4.9/libcst/codemod/tests/test_codemod.py` & `libcst-1.0.0/libcst/codemod/tests/test_codemod.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         if self.skip:
             raise SkipFile()
         else:
             return tree
 
 
 class TestSkipDetection(CodemodTest):
-
     TRANSFORM = SimpleCodemod
 
     def test_detect_skip(self) -> None:
         code = """
             def foo() -> None:
                 pass
 
@@ -83,15 +82,14 @@
                 lambda node, _: node.with_changes(value=str(int(node.value) + 1)),
             ),
             cst.Module,
         )
 
 
 class TestMultipass(CodemodTest):
-
     TRANSFORM = IncrementCodemod
 
     def test_multi_iterations(self) -> None:
         before = """
             x = 5
         """
         after = """
```

### Comparing `libcst-0.4.9/libcst/codemod/tests/test_codemod_cli.py` & `libcst-1.0.0/libcst/codemod/tests/test_codemod_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 #
 
 
+import platform
 import subprocess
+import sys
 from pathlib import Path
+from unittest import skipIf
 
 from libcst._parser.entrypoints import is_native
 from libcst.testing.utils import UnitTest
 
 
 class TestCodemodCLI(UnitTest):
+    # pyre-ignore - no idea why pyre is complaining about this
+    @skipIf(platform.system() == "Windows", "Windows")
     def test_codemod_formatter_error_input(self) -> None:
         rlt = subprocess.run(
             [
-                "python",
+                sys.executable,
                 "-m",
                 "libcst.tool",
                 "codemod",
                 "remove_unused_imports.RemoveUnusedImportsCommand",
                 # `ArgumentParser.parse_known_args()`'s behavior dictates that options
                 # need to go after instead of before the codemod command identifier.
                 "--python-version",
@@ -36,7 +41,25 @@
                 rlt.stderr.decode("utf-8"),
             )
         else:
             self.assertIn(
                 "error: cannot format -: Cannot parse: 13:10:     async with AsyncExitStack() as stack:",
                 rlt.stderr.decode("utf-8"),
             )
+
+    def test_codemod_external(self) -> None:
+        # Test running the NOOP command as an "external command"
+        # against this very file.
+        output = subprocess.check_output(
+            [
+                sys.executable,
+                "-m",
+                "libcst.tool",
+                "codemod",
+                "-x",  # external module
+                "libcst.codemod.commands.noop.NOOPCommand",
+                str(Path(__file__)),
+            ],
+            encoding="utf-8",
+            stderr=subprocess.STDOUT,
+        )
+        assert "Finished codemodding 1 files!" in output
```

### Comparing `libcst-0.4.9/libcst/codemod/tests/test_metadata.py` & `libcst-1.0.0/libcst/codemod/tests/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 from libcst import parse_module
 from libcst.codemod import CodemodContext, ContextAwareTransformer, ContextAwareVisitor
 from libcst.metadata import PositionProvider
 from libcst.testing.utils import UnitTest
 
 
 class TestingCollector(ContextAwareVisitor):
-
     METADATA_DEPENDENCIES = (PositionProvider,)
 
     def visit_Pass(self, node: cst.Pass) -> None:
         position = self.get_metadata(PositionProvider, node)
         self.context.scratch["pass"] = (position.start.line, position.start.column)
 
 
 class TestingTransform(ContextAwareTransformer):
-
     METADATA_DEPENDENCIES = (PositionProvider,)
 
     def visit_FunctionDef(self, node: cst.FunctionDef) -> None:
         position = self.get_metadata(PositionProvider, node)
         self.context.scratch[node.name.value] = (
             position.start.line,
             position.start.column,
```

### Comparing `libcst-0.4.9/libcst/codemod/tests/test_runner.py` & `libcst-1.0.0/libcst/codemod/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/__init__.py` & `libcst-1.0.0/libcst/codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_add_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/_add_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         self.all_imports = gatherer.all_imports
 
         self.module_imports = self.module_imports - gatherer.module_imports
         for module, alias in gatherer.module_aliases.items():
             if module in self.module_aliases and self.module_aliases[module] == alias:
                 del self.module_aliases[module]
         for module, aliases in gatherer.alias_mapping.items():
-            for (obj, alias) in aliases:
+            for obj, alias in aliases:
                 if (
                     module in self.alias_mapping
                     and (obj, alias) in self.alias_mapping[module]
                 ):
                     self.alias_mapping[module].remove((obj, alias))
                     if len(self.alias_mapping[module]) == 0:
                         del self.alias_mapping[module]
@@ -279,15 +279,15 @@
             statement_before_import_location = import_add_location = 1
 
         # This works under the principle that while we might modify node contents,
         # we have yet to modify the number of statements. So we can match on the
         # original tree but break up the statements of the modified tree. If we
         # change this assumption in this visitor, we will have to change this code.
         for i, statement in enumerate(orig_module.body):
-            if m.matches(
+            if i == 0 and m.matches(
                 statement, m.SimpleStatementLine(body=[m.Expr(value=m.SimpleString())])
             ):
                 statement_before_import_location = import_add_location = 1
             elif isinstance(statement, libcst.SimpleStatementLine):
                 for possible_import in statement.body:
                     for last_import in self.all_imports:
                         if possible_import is last_import:
```

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_apply_type_annotations.py` & `libcst-1.0.0/libcst/codemod/visitors/_apply_type_annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,43 +251,46 @@
         QualifiedNameProvider,
     )
 
     def __init__(self, existing_imports: Set[str], context: CodemodContext) -> None:
         super().__init__()
         self.existing_imports: Set[str] = existing_imports
         self.imported_symbols: Dict[str, Set[ImportedSymbol]] = defaultdict(set)
+        self.in_annotation: bool = False
+
+    def visit_Annotation(self, node: cst.Annotation) -> None:
+        self.in_annotation = True
+
+    def leave_Annotation(self, original_node: cst.Annotation) -> None:
+        self.in_annotation = False
 
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         for base in node.bases:
             value = base.value
             if isinstance(value, NAME_OR_ATTRIBUTE):
                 self._handle_NameOrAttribute(value)
-            elif isinstance(value, cst.Subscript):
-                self._handle_Subscript(value)
 
-    def visit_FunctionDef(self, node: cst.FunctionDef) -> bool:
-        if node.returns is not None:
-            self._handle_Annotation(annotation=node.returns)
-        self._handle_Parameters(node.params)
-
-        # pyi files don't support inner functions, return False to stop the traversal.
-        return False
+    def visit_Name(self, node: cst.Name) -> None:
+        if self.in_annotation:
+            self._handle_NameOrAttribute(node)
 
-    def visit_AnnAssign(self, node: cst.AnnAssign) -> None:
-        self._handle_Annotation(annotation=node.annotation)
+    def visit_Attribute(self, node: cst.Attribute) -> None:
+        if self.in_annotation:
+            self._handle_NameOrAttribute(node)
 
-    # Handler functions.
-    #
-    # These ultimately all call _handle_NameOrAttribute, which adds the
-    # qualified name to the list of imported symbols
+    def visit_Subscript(self, node: cst.Subscript) -> bool:
+        if isinstance(node.value, NAME_OR_ATTRIBUTE):
+            return True
+        return _get_unique_qualified_name(self, node) not in ("Type", "typing.Type")
 
     def _handle_NameOrAttribute(
         self,
         node: NameOrAttribute,
     ) -> None:
+        # Adds the qualified name to the list of imported symbols
         obj = sym = None  # keep pyre happy
         if isinstance(node, cst.Name):
             obj = None
             sym = node.value
         elif isinstance(node, cst.Attribute):
             obj = node.value.value  # pyre-ignore[16]
             sym = node.attr.value
@@ -300,56 +303,14 @@
                 module_name=module,
                 module_alias=obj if obj != module else None,
                 target_name=target,
                 target_alias=sym if sym != target else None,
             )
             self.imported_symbols[sym].add(mod)
 
-    def _handle_Index(self, slice: cst.Index) -> None:
-        value = slice.value
-        if isinstance(value, cst.Subscript):
-            self._handle_Subscript(value)
-        elif isinstance(value, cst.Attribute):
-            self._handle_NameOrAttribute(value)
-
-    def _handle_Subscript(self, node: cst.Subscript) -> None:
-        value = node.value
-        if isinstance(value, NAME_OR_ATTRIBUTE):
-            self._handle_NameOrAttribute(value)
-        else:
-            raise ValueError("Expected any indexed type to have")
-        if _get_unique_qualified_name(self, node) in ("Type", "typing.Type"):
-            return
-        slice = node.slice
-        if isinstance(slice, tuple):
-            for item in slice:
-                if isinstance(item.slice.value, NAME_OR_ATTRIBUTE):
-                    self._handle_NameOrAttribute(item.slice.value)
-                else:
-                    if isinstance(item.slice, cst.Index):
-                        self._handle_Index(item.slice)
-        elif isinstance(slice, cst.Index):
-            self._handle_Index(slice)
-
-    def _handle_Annotation(self, annotation: cst.Annotation) -> None:
-        node = annotation.annotation
-        if isinstance(node, cst.Subscript):
-            self._handle_Subscript(node)
-        elif isinstance(node, NAME_OR_ATTRIBUTE):
-            self._handle_NameOrAttribute(node)
-        elif isinstance(node, cst.SimpleString):
-            pass
-        else:
-            raise ValueError(f"Unexpected annotation node: {node}")
-
-    def _handle_Parameters(self, parameters: cst.Parameters) -> None:
-        for parameter in list(parameters.params):
-            if parameter.annotation is not None:
-                self._handle_Annotation(annotation=parameter.annotation)
-
 
 class TypeCollector(m.MatcherDecoratableVisitor):
     """
     Collect type annotations from a stub module.
     """
 
     METADATA_DEPENDENCIES = (
@@ -388,17 +349,17 @@
         node: cst.ClassDef,
     ) -> None:
         self.qualifier.append(node.name.value)
         new_bases = []
         for base in node.bases:
             value = base.value
             if isinstance(value, NAME_OR_ATTRIBUTE):
-                new_value = self._handle_NameOrAttribute(value)
+                new_value = value.visit(_TypeCollectorDequalifier(self))
             elif isinstance(value, cst.Subscript):
-                new_value = self._handle_Subscript(value)
+                new_value = value.visit(_TypeCollectorDequalifier(self))
             else:
                 start = self.get_metadata(PositionProvider, node).start
                 raise ValueError(
                     "Invalid type used as base class in stub file at "
                     + f"{start.line}:{start.column}. Only subscripts, names, and "
                     + "attributes are valid base classes for static typing."
                 )
@@ -417,15 +378,20 @@
     def visit_FunctionDef(
         self,
         node: cst.FunctionDef,
     ) -> bool:
         self.qualifier.append(node.name.value)
         returns = node.returns
         return_annotation = (
-            self._handle_Annotation(annotation=returns) if returns is not None else None
+            returns.visit(_TypeCollectorDequalifier(self))
+            if returns is not None
+            else None
+        )
+        assert return_annotation is None or isinstance(
+            return_annotation, cst.Annotation
         )
         parameter_annotations = self._handle_Parameters(node.params)
         name = ".".join(self.qualifier)
         key = FunctionKey.make(name, node.params)
         self.annotations.functions[key] = FunctionAnnotation(
             parameters=parameter_annotations, returns=return_annotation
         )
@@ -442,15 +408,16 @@
     def visit_AnnAssign(
         self,
         node: cst.AnnAssign,
     ) -> bool:
         name = get_full_name_for_node(node.target)
         if name is not None:
             self.qualifier.append(name)
-        annotation_value = self._handle_Annotation(annotation=node.annotation)
+        annotation_value = node.annotation.visit(_TypeCollectorDequalifier(self))
+        assert isinstance(annotation_value, cst.Annotation)
         self.annotations.attributes[".".join(self.qualifier)] = annotation_value
         return True
 
     def leave_AnnAssign(
         self,
         original_node: cst.AnnAssign,
     ) -> None:
@@ -537,126 +504,98 @@
                     module,
                     target,
                     asname=asname,
                 )
                 return False
         return False
 
-    # Handler functions.
-    #
-    # Each of these does one of two things, possibly recursively, over some
-    # valid CST node for a static type:
-    #  - process the qualified name and ensure we will add necessary imports
-    #  - dequalify the node
-
-    def _handle_NameOrAttribute(
-        self,
-        node: NameOrAttribute,
-    ) -> Union[cst.Name, cst.Attribute]:
-        qualified_name = _get_unique_qualified_name(self, node)
-        should_qualify = self._handle_qualification_and_should_qualify(
-            qualified_name, node
-        )
-        self.annotations.names.add(qualified_name)
-        if should_qualify:
-            qualified_node = (
-                cst.parse_module(qualified_name) if isinstance(node, cst.Name) else node
-            )
-            return qualified_node  # pyre-ignore[7]
-        else:
-            dequalified_node = node.attr if isinstance(node, cst.Attribute) else node
-            return dequalified_node
-
-    def _handle_Index(
-        self,
-        slice: cst.Index,
-    ) -> cst.Index:
-        value = slice.value
-        if isinstance(value, cst.Subscript):
-            return slice.with_changes(value=self._handle_Subscript(value))
-        elif isinstance(value, cst.Attribute):
-            return slice.with_changes(value=self._handle_NameOrAttribute(value))
-        else:
-            if isinstance(value, cst.SimpleString):
-                self.annotations.names.add(_get_string_value(value))
-            return slice
-
-    def _handle_Subscript(
-        self,
-        node: cst.Subscript,
-    ) -> cst.Subscript:
-        value = node.value
-        if isinstance(value, NAME_OR_ATTRIBUTE):
-            new_node = node.with_changes(value=self._handle_NameOrAttribute(value))
-        else:
-            raise ValueError("Expected any indexed type to have")
-        if _get_unique_qualified_name(self, node) in ("Type", "typing.Type"):
-            # Note: we are intentionally not handling qualification of
-            # anything inside `Type` because it's common to have nested
-            # classes, which we cannot currently distinguish from classes
-            # coming from other modules, appear here.
-            return new_node
-        slice = node.slice
-        if isinstance(slice, tuple):
-            new_slice = []
-            for item in slice:
-                value = item.slice.value
-                if isinstance(value, NAME_OR_ATTRIBUTE):
-                    name = self._handle_NameOrAttribute(item.slice.value)
-                    new_index = item.slice.with_changes(value=name)
-                    new_slice.append(item.with_changes(slice=new_index))
-                else:
-                    if isinstance(item.slice, cst.Index):
-                        new_index = item.slice.with_changes(
-                            value=self._handle_Index(item.slice)
-                        )
-                        item = item.with_changes(slice=new_index)
-                    new_slice.append(item)
-            return new_node.with_changes(slice=tuple(new_slice))
-        elif isinstance(slice, cst.Index):
-            new_slice = self._handle_Index(slice)
-            return new_node.with_changes(slice=new_slice)
-        else:
-            return new_node
-
-    def _handle_Annotation(
-        self,
-        annotation: cst.Annotation,
-    ) -> cst.Annotation:
-        node = annotation.annotation
-        if isinstance(node, cst.SimpleString):
-            self.annotations.names.add(_get_string_value(node))
-            return annotation
-        elif isinstance(node, cst.Subscript):
-            return cst.Annotation(annotation=self._handle_Subscript(node))
-        elif isinstance(node, NAME_OR_ATTRIBUTE):
-            return cst.Annotation(annotation=self._handle_NameOrAttribute(node))
-        else:
-            raise ValueError(f"Unexpected annotation node: {node}")
+    # Handler functions
 
     def _handle_Parameters(
         self,
         parameters: cst.Parameters,
     ) -> cst.Parameters:
         def update_annotations(
             parameters: Sequence[cst.Param],
         ) -> List[cst.Param]:
             updated_parameters = []
             for parameter in list(parameters):
                 annotation = parameter.annotation
                 if annotation is not None:
                     parameter = parameter.with_changes(
-                        annotation=self._handle_Annotation(annotation=annotation)
+                        annotation=annotation.visit(_TypeCollectorDequalifier(self))
                     )
                 updated_parameters.append(parameter)
             return updated_parameters
 
         return parameters.with_changes(params=update_annotations(parameters.params))
 
 
+class _TypeCollectorDequalifier(cst.CSTTransformer):
+    def __init__(self, type_collector: "TypeCollector") -> None:
+        self.type_collector = type_collector
+
+    def leave_Name(self, original_node: cst.Name, updated_node: cst.Name) -> cst.Name:
+        qualified_name = _get_unique_qualified_name(self.type_collector, original_node)
+        should_qualify = self.type_collector._handle_qualification_and_should_qualify(
+            qualified_name, original_node
+        )
+        self.type_collector.annotations.names.add(qualified_name)
+        if should_qualify:
+            qualified_node = cst.parse_module(qualified_name)
+            return qualified_node  # pyre-ignore[7]
+        else:
+            return original_node
+
+    def visit_Attribute(self, node: cst.Attribute) -> bool:
+        return False
+
+    def leave_Attribute(
+        self, original_node: cst.Attribute, updated_node: cst.Attribute
+    ) -> cst.BaseExpression:
+        qualified_name = _get_unique_qualified_name(self.type_collector, original_node)
+        should_qualify = self.type_collector._handle_qualification_and_should_qualify(
+            qualified_name, original_node
+        )
+        self.type_collector.annotations.names.add(qualified_name)
+        if should_qualify:
+            return original_node
+        else:
+            return original_node.attr
+
+    def leave_Index(
+        self, original_node: cst.Index, updated_node: cst.Index
+    ) -> cst.Index:
+        if isinstance(original_node.value, cst.SimpleString):
+            self.type_collector.annotations.names.add(
+                _get_string_value(original_node.value)
+            )
+        return updated_node
+
+    def visit_Subscript(self, node: cst.Subscript) -> bool:
+        return _get_unique_qualified_name(self.type_collector, node) not in (
+            "Type",
+            "typing.Type",
+        )
+
+    def leave_Subscript(
+        self, original_node: cst.Subscript, updated_node: cst.Subscript
+    ) -> cst.Subscript:
+        if _get_unique_qualified_name(self.type_collector, original_node) in (
+            "Type",
+            "typing.Type",
+        ):
+            # Note: we are intentionally not handling qualification of
+            # anything inside `Type` because it's common to have nested
+            # classes, which we cannot currently distinguish from classes
+            # coming from other modules, appear here.
+            return original_node.with_changes(value=original_node.value.visit(self))
+        return updated_node
+
+
 @dataclass
 class AnnotationCounts:
     global_annotations: int = 0
     attribute_annotations: int = 0
     parameter_annotations: int = 0
     return_annotations: int = 0
     classes_added: int = 0
@@ -1004,15 +943,15 @@
             pass
         else:
             name = get_full_name_for_node(only_target)
             if name is not None:
                 self.qualifier.append(name)
                 if (
                     self._qualifier_name() in self.annotations.attributes
-                    and not isinstance(only_target, cst.Subscript)
+                    and not isinstance(only_target, (cst.Attribute, cst.Subscript))
                 ):
                     annotation = self.annotations.attributes[self._qualifier_name()]
                     self.qualifier.pop()
                     return self._apply_annotation_to_attribute_or_global(
                         name=name,
                         annotation=annotation,
                         value=node.value,
@@ -1297,15 +1236,14 @@
             self.current_assign = None
 
     def leave_Assign(
         self,
         original_node: cst.Assign,
         updated_node: cst.Assign,
     ) -> Union[cst.Assign, cst.AnnAssign]:
-
         self.current_assign = None
 
         if len(original_node.targets) > 1:
             for assign in original_node.targets:
                 target = assign.target
                 if isinstance(target, (cst.Name, cst.Attribute)):
                     name = get_full_name_for_node(target)
```

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_comments.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_exports.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_global_names.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_string_annotation_names.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_gather_unused_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/_gather_unused_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         Return the imports in ``candidates`` which are not used.
 
         This function implements the main logic of this visitor, and is called after traversal. It calls :meth:`~is_in_use` on each import.
 
         Override this in a subclass for additional filtering.
         """
         unused_imports = set()
-        for (alias, parent) in candidates:
+        for alias, parent in candidates:
             scope = self.get_metadata(ScopeProvider, parent)
             if scope is None:
                 continue
             if not self.is_in_use(scope, alias):
                 unused_imports.add((alias, parent))
         return unused_imports
```

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/_remove_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_add_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_add_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # LICENSE file in the root directory of this source tree.
 #
 from libcst.codemod import CodemodContext, CodemodTest
 from libcst.codemod.visitors import AddImportsVisitor, ImportItem
 
 
 class TestAddImportsCodemod(CodemodTest):
-
     TRANSFORM = AddImportsVisitor
 
     def test_noop(self) -> None:
         """
         Should do nothing.
         """
 
@@ -887,7 +886,40 @@
             before,
             after,
             [ImportItem("__future__", "annotations", None)],
             context_override=CodemodContext(
                 full_module_name="a.b.foobar", full_package_name="a.b"
             ),
         )
+
+    def test_import_in_module_with_standalone_string_not_a_docstring(
+        self,
+    ) -> None:
+        """
+        The import should be added after the __future__ imports.
+        """
+        before = """
+            from __future__ import annotations
+            from __future__ import division
+
+            '''docstring.'''
+            def func():
+                pass
+        """
+        after = """
+            from __future__ import annotations
+            from __future__ import division
+            import typing
+
+            '''docstring.'''
+            def func():
+                pass
+        """
+
+        self.assertCodemod(
+            before,
+            after,
+            [ImportItem("typing", None, None)],
+            context_override=CodemodContext(
+                full_module_name="a.b.foobar", full_package_name="a.b"
+            ),
+        )
```

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_apply_type_annotations.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_apply_type_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,15 +465,15 @@
 
                 def foo(x: int) -> List[Union[Example, str]]:
                     return [barfoo(), ""]
                 """,
             ),
             "deeply_nested_example_with_multiline_annotation": (
                 """
-                def foo(x: int)-> Union[
+                def foo(x: int) -> Union[
                     Coroutine[Any, Any, django.http.response.HttpResponse], str
                 ]:
                     ...
                 """,
                 """
                 def foo(x: int):
                     pass
@@ -1117,14 +1117,91 @@
             before=before,
             after=after,
             overwrite_existing_annotations=True,
         )
 
     @data_provider(
         {
+            "pep_604": (
+                """
+                def f(a: int | str, b: int | list[int | list[int | str]]) -> str: ...
+                """,
+                """
+                def f(a, b):
+                    return 'hello'
+                """,
+                """
+                def f(a: int | str, b: int | list[int | list[int | str]]) -> str:
+                    return 'hello'
+                """,
+            ),
+            "pep_604_import": (
+                """
+                from typing import Callable
+                from collections.abc import Sequence
+                def f(a: int | str, b: int | list[int | Callable[[str], Sequence]]) -> str: ...
+                """,
+                """
+                def f(a, b):
+                    return 'hello'
+                """,
+                """
+                from collections.abc import Sequence
+                from typing import Callable
+
+                def f(a: int | str, b: int | list[int | Callable[[str], Sequence]]) -> str:
+                    return 'hello'
+                """,
+            ),
+        }
+    )
+    def test_annotate_functions_pep_604(
+        self, stub: str, before: str, after: str
+    ) -> None:
+        self.run_test_case_with_flags(
+            stub=stub,
+            before=before,
+            after=after,
+            overwrite_existing_annotations=True,
+        )
+
+    @data_provider(
+        {
+            "import_inside_list": (
+                """
+                from typing import Callable
+                from collections.abc import Sequence
+                def f(a: Callable[[Sequence[int]], int], b: int) -> str: ...
+                """,
+                """
+                def f(a, b):
+                    return 'hello'
+                """,
+                """
+                from collections.abc import Sequence
+                from typing import Callable
+
+                def f(a: Callable[[Sequence[int]], int], b: int) -> str:
+                    return 'hello'
+                """,
+            ),
+        }
+    )
+    def test_annotate_function_nested_imports(
+        self, stub: str, before: str, after: str
+    ) -> None:
+        self.run_test_case_with_flags(
+            stub=stub,
+            before=before,
+            after=after,
+            overwrite_existing_annotations=True,
+        )
+
+    @data_provider(
+        {
             "return_self": (
                 """
                 class Foo:
                     def f(self) -> Foo: ...
                 """,
                 """
                 class Foo:
@@ -1741,7 +1818,95 @@
     )
     def test_signature_matching_with_always_qualify(
         self, stub: str, before: str, after: str
     ) -> None:
         self.run_test_case_with_flags(
             stub=stub, before=before, after=after, always_qualify_annotations=True
         )
+
+    @data_provider(
+        {
+            "attribute": (
+                """
+                class C:
+                    x: int
+                """,
+                """
+                class C:
+                    x = 0
+                C.x = 1
+                """,
+                """
+                class C:
+                    x: int = 0
+                C.x = 1
+                """,
+            ),
+            "subscript": (
+                """
+                d: dict[str, int]
+                """,
+                """
+                d = {}
+                d["k"] = 0
+                """,
+                """
+                d: dict[str, int] = {}
+                d["k"] = 0
+                """,
+            ),
+            "starred": (
+                """
+                a: int
+                b: list[int]
+                """,
+                """
+                a, *b = [1, 2, 3]
+                """,
+                """
+                a: int
+                b: list[int]
+
+                a, *b = [1, 2, 3]
+                """,
+            ),
+            "name": (
+                """
+                a: int
+                """,
+                """
+                a = 0
+                """,
+                """
+                a: int = 0
+                """,
+            ),
+            "list": (
+                """
+                a: int
+                """,
+                """
+                [a] = [0]
+                """,
+                """
+                a: int
+
+                [a] = [0]
+                """,
+            ),
+            "tuple": (
+                """
+                a: int
+                """,
+                """
+                (a,) = [0]
+                """,
+                """
+                a: int
+
+                (a,) = [0]
+                """,
+            ),
+        }
+    )
+    def test_valid_assign_expressions(self, stub: str, before: str, after: str) -> None:
+        self.run_simple_test_case(stub=stub, before=before, after=after)
```

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_comments.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_exports.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_global_names.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_unused_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/codemod/visitors/tests/test_remove_imports.py` & `libcst-1.0.0/libcst/codemod/visitors/tests/test_remove_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     QualifiedNameSource,
     ScopeProvider,
 )
 from libcst.testing.utils import data_provider
 
 
 class TestRemoveImportsCodemod(CodemodTest):
-
     TRANSFORM = RemoveImportsVisitor
 
     def test_noop(self) -> None:
         """
         Should do nothing.
         """
 
@@ -753,15 +752,14 @@
         """
         Given a node that's directly referenced in an import,
         make sure that the import is removed when the node
         is also removed.
         """
 
         class RemoveBarTransformer(VisitorBasedCodemodCommand):
-
             METADATA_DEPENDENCIES = (QualifiedNameProvider, ScopeProvider)
 
             @m.leave(
                 m.SimpleStatementLine(
                     body=[
                         m.Expr(
                             m.Call(
@@ -817,15 +815,14 @@
 
             def fun() -> None:
                 baz()
                 other2()
         """
 
         class RemoveImportTransformer(VisitorBasedCodemodCommand):
-
             METADATA_DEPENDENCIES = (QualifiedNameProvider, ScopeProvider)
 
             def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
                 RemoveImportsVisitor.remove_unused_import_by_node(self.context, node)
 
         module = cst.parse_module(self.make_fixture_data(before))
         self.assertCodeEqual(
@@ -856,15 +853,14 @@
 
             def fun() -> None:
                 qux.baz()
                 other2.baz()
         """
 
         class RemoveImportTransformer(VisitorBasedCodemodCommand):
-
             METADATA_DEPENDENCIES = (QualifiedNameProvider, ScopeProvider)
 
             def visit_Import(self, node: cst.Import) -> None:
                 RemoveImportsVisitor.remove_unused_import_by_node(self.context, node)
 
         module = cst.parse_module(self.make_fixture_data(before))
         self.assertCodeEqual(
@@ -888,15 +884,14 @@
         after = """
             from qux import baz
 
             __all__ = ["baz"]
         """
 
         class RemoveImportTransformer(VisitorBasedCodemodCommand):
-
             METADATA_DEPENDENCIES = (QualifiedNameProvider, ScopeProvider)
 
             def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
                 RemoveImportsVisitor.remove_unused_import_by_node(self.context, node)
 
         module = cst.parse_module(self.make_fixture_data(before))
         self.assertCodeEqual(
```

### Comparing `libcst-0.4.9/libcst/helpers/__init__.py` & `libcst-1.0.0/libcst/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/helpers/_template.py` & `libcst-1.0.0/libcst/helpers/_template.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/helpers/common.py` & `libcst-1.0.0/libcst/helpers/common.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/helpers/expression.py` & `libcst-1.0.0/libcst/helpers/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/helpers/module.py` & `libcst-1.0.0/libcst/helpers/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 from dataclasses import dataclass
 from itertools import islice
 from pathlib import PurePath
 from typing import List, Optional
 
 from libcst import Comment, EmptyLine, ImportFrom, Module
+from libcst._types import StrPath
 from libcst.helpers.expression import get_full_name_for_node
 
 
 def insert_header_comments(node: Module, comments: List[str]) -> Module:
     """
     Insert comments after last non-empty line in header. Use this to insert one or more
     comments after any copyright preamble in a :class:`~libcst.Module`. Each comment in
@@ -85,15 +86,15 @@
 
 def get_absolute_module_from_package(
     current_package: Optional[str], module_name: Optional[str], num_dots: int
 ) -> Optional[str]:
     if num_dots == 0:
         # This is an absolute import, so the module is correct.
         return module_name
-    if current_package is None:
+    if current_package is None or current_package == "":
         # We don't actually have the current module available, so we can't compute
         # the absolute module from relative.
         return None
 
     # see importlib._bootstrap._resolve_name
     # https://github.com/python/cpython/blob/3.10/Lib/importlib/_bootstrap.py#L902
     bits = current_package.rsplit(".", num_dots - 1)
@@ -126,15 +127,17 @@
 
 @dataclass(frozen=True)
 class ModuleNameAndPackage:
     name: str
     package: str
 
 
-def calculate_module_and_package(repo_root: str, filename: str) -> ModuleNameAndPackage:
+def calculate_module_and_package(
+    repo_root: StrPath, filename: StrPath
+) -> ModuleNameAndPackage:
     # Given an absolute repo_root and an absolute filename, calculate the
     # python module name for the file.
     relative_filename = PurePath(filename).relative_to(repo_root)
     relative_filename = relative_filename.with_suffix("")
 
     # handle special cases
     if relative_filename.stem in ["__init__", "__main__"]:
```

### Comparing `libcst-0.4.9/libcst/helpers/tests/test_expression.py` & `libcst-1.0.0/libcst/helpers/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/helpers/tests/test_module.py` & `libcst-1.0.0/libcst/helpers/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         (
             # Simple imports that are already absolute.
             (None, "from a.b import c", "a.b"),
             ("x/y/z.py", "from a.b import c", "a.b"),
             ("x/y/z/__init__.py", "from a.b import c", "a.b"),
             # Relative import that can't be resolved due to missing module.
             (None, "from ..w import c", None),
+            # Attempted relative import with no known parent package
+            ("__init__.py", "from .y import z", None),
+            ("x.py", "from .y import z", None),
             # Relative import that goes past the module level.
             ("x.py", "from ...y import z", None),
             ("x/y/z.py", "from ... import c", None),
             ("x/y/z.py", "from ...w import c", None),
             ("x/y/z/__init__.py", "from .... import c", None),
             ("x/y/z/__init__.py", "from ....w import c", None),
             # Correct resolution of absolute from relative modules.
```

### Comparing `libcst-0.4.9/libcst/helpers/tests/test_template.py` & `libcst-1.0.0/libcst/helpers/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/__init__.py` & `libcst-1.0.0/libcst/matchers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3085,33 +3085,26 @@
         MetadataMatchType,
         DoNotCareSentinel,
         OneOf[MetadataMatchType],
         AllOf[MetadataMatchType],
     ] = DoNotCare()
 
 
-NameOrAttributeOrCallMatchType = Union[
-    "Name",
-    "Attribute",
-    "Call",
-    MetadataMatchType,
-    MatchIfTrue[Union[cst.Name, cst.Attribute, cst.Call]],
-]
 TrailingWhitespaceMatchType = Union[
     "TrailingWhitespace", MetadataMatchType, MatchIfTrue[cst.TrailingWhitespace]
 ]
 
 
 @dataclass(frozen=True, eq=False, unsafe_hash=False)
 class Decorator(BaseMatcherNode):
     decorator: Union[
-        NameOrAttributeOrCallMatchType,
+        BaseExpressionMatchType,
         DoNotCareSentinel,
-        OneOf[NameOrAttributeOrCallMatchType],
-        AllOf[NameOrAttributeOrCallMatchType],
+        OneOf[BaseExpressionMatchType],
+        AllOf[BaseExpressionMatchType],
     ] = DoNotCare()
     leading_lines: Union[
         Sequence[
             Union[
                 EmptyLineMatchType,
                 DoNotCareSentinel,
                 OneOf[EmptyLineMatchType],
```

### Comparing `libcst-0.4.9/libcst/matchers/_decorators.py` & `libcst-1.0.0/libcst/matchers/_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/_matcher_base.py` & `libcst-1.0.0/libcst/matchers/_matcher_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1520,17 +1520,17 @@
                 return None
             all_captures = {**all_captures, **node_capture}
         return all_captures
     else:
         return _node_matches(node, matcher, metadata_lookup)
 
 
-def _construct_metadata_fetcher_null() -> Callable[
-    [meta.ProviderT, libcst.CSTNode], object
-]:
+def _construct_metadata_fetcher_null() -> (
+    Callable[[meta.ProviderT, libcst.CSTNode], object]
+):
     def _fetch(provider: meta.ProviderT, node: libcst.CSTNode) -> NoReturn:
         raise LookupError(
             f"{provider.__name__} is not resolved; did you forget a MetadataWrapper?"
         )
 
     return _fetch
```

### Comparing `libcst-0.4.9/libcst/matchers/_return_types.py` & `libcst-1.0.0/libcst/matchers/_return_types.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/_visitors.py` & `libcst-1.0.0/libcst/matchers/_visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,23 @@
     MatchMetadata,
     MatchMetadataIfTrue,
     OneOf,
     replace,
 )
 from libcst.matchers._return_types import TYPED_FUNCTION_RETURN_MAPPING
 
+try:
+    # PEP 604 unions, in Python 3.10+
+    from types import UnionType
+except ImportError:
+    # We use this for isinstance; no annotation will be an instance of this
+    class UnionType:
+        pass
+
+
 CONCRETE_METHODS: Set[str] = {
     *{f"visit_{cls.__name__}" for cls in TYPED_FUNCTION_RETURN_MAPPING},
     *{f"leave_{cls.__name__}" for cls in TYPED_FUNCTION_RETURN_MAPPING},
 }
 
 
 # pyre-ignore We don't care about Any here, its not exposed.
@@ -74,26 +83,23 @@
 def _get_possible_match_classes(matcher: BaseMatcherNode) -> List[Type[cst.CSTNode]]:
     if isinstance(matcher, (OneOf, AllOf)):
         return [getattr(cst, m.__class__.__name__) for m in matcher.options]
     else:
         return [getattr(cst, matcher.__class__.__name__)]
 
 
-def _annotation_looks_like_union(annotation: object) -> bool:
-    if getattr(annotation, "__origin__", None) is Union:
-        return True
-    # support PEP-604 style unions introduced in Python 3.10
+def _annotation_is_union(annotation: object) -> bool:
     return (
-        annotation.__class__.__name__ == "Union"
-        and annotation.__class__.__module__ == "types"
+        isinstance(annotation, UnionType)
+        or getattr(annotation, "__origin__", None) is Union
     )
 
 
 def _get_possible_annotated_classes(annotation: object) -> List[Type[object]]:
-    if _annotation_looks_like_union(annotation):
+    if _annotation_is_union(annotation):
         return getattr(annotation, "__args__", [])
     else:
         return [cast(Type[object], annotation)]
 
 
 def _get_valid_leave_annotations_for_classes(
     classes: Sequence[Type[cst.CSTNode]],
@@ -313,18 +319,14 @@
             continue
         matchers = getattr(func, CONSTRUCTED_VISIT_MATCHER_ATTR, [])
         if matchers:
             # Make sure that we aren't accidentally putting a @visit on a visit_Node.
             _assert_not_concrete("visit", func)
         for matcher in matchers:
             casted_matcher = cast(BaseMatcherNode, matcher)
-            # pyre-fixme[6]: Expected
-            #  `Sequence[typing.Callable[[cst._nodes.base.CSTNode], None]]` for 2nd
-            #  param but got `Tuple[*Tuple[(CSTNode) -> None, ...], (CSTNode) ->
-            #  None]`.
             constructed_visitors[casted_matcher] = (
                 *constructed_visitors.get(casted_matcher, ()),
                 func,
             )
 
     return constructed_visitors
 
@@ -352,18 +354,14 @@
             continue
         matchers = getattr(func, CONSTRUCTED_LEAVE_MATCHER_ATTR, [])
         if matchers:
             # Make sure that we aren't accidentally putting a @leave on a leave_Node.
             _assert_not_concrete("leave", func)
         for matcher in matchers:
             casted_matcher = cast(BaseMatcherNode, matcher)
-            # pyre-fixme[6]: Expected
-            #  `Sequence[typing.Callable[[cst._nodes.base.CSTNode], None]]` for 2nd
-            #  param but got `Tuple[*Tuple[(CSTNode) -> None, ...], (CSTNode) ->
-            #  None]`.
             constructed_visitors[casted_matcher] = (
                 *constructed_visitors.get(casted_matcher, ()),
                 func,
             )
 
     return constructed_visitors
```

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_decorators.py` & `libcst-1.0.0/libcst/matchers/tests/test_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+import sys
 from ast import literal_eval
 from textwrap import dedent
 from typing import List, Set
-from unittest.mock import Mock
+from unittest import skipIf
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.matchers import (
     call_if_inside,
     call_if_not_inside,
     leave,
@@ -992,27 +993,19 @@
         visitor = TestVisitor()
         module.visit(visitor)
 
         # We should have only visited a select number of nodes.
         self.assertEqual(visitor.visits, ['"baz"'])
 
 
-# This is meant to simulate `cst.ImportFrom | cst.RemovalSentinel` in py3.10
-FakeUnionClass: Mock = Mock()
-setattr(FakeUnionClass, "__name__", "Union")
-setattr(FakeUnionClass, "__module__", "types")
-FakeUnion: Mock = Mock()
-FakeUnion.__class__ = FakeUnionClass
-FakeUnion.__args__ = [cst.ImportFrom, cst.RemovalSentinel]
-
-
 class MatchersUnionDecoratorsTest(UnitTest):
+    @skipIf(bool(sys.version_info < (3, 10)), "new union syntax not available")
     def test_init_with_new_union_annotation(self) -> None:
         class TransformerWithUnionReturnAnnotation(m.MatcherDecoratableTransformer):
             @m.leave(m.ImportFrom(module=m.Name(value="typing")))
             def test(
                 self, original_node: cst.ImportFrom, updated_node: cst.ImportFrom
-            ) -> FakeUnion:
+            ) -> cst.ImportFrom | cst.RemovalSentinel:
                 pass
 
         # assert that init (specifically _check_types on return annotation) passes
         TransformerWithUnionReturnAnnotation()
```

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_extract.py` & `libcst-1.0.0/libcst/matchers/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_findall.py` & `libcst-1.0.0/libcst/matchers/tests/test_findall.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_matchers.py` & `libcst-1.0.0/libcst/matchers/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_matchers_with_metadata.py` & `libcst-1.0.0/libcst/matchers/tests/test_matchers_with_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_replace.py` & `libcst-1.0.0/libcst/matchers/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/matchers/tests/test_visitors.py` & `libcst-1.0.0/libcst/matchers/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/__init__.py` & `libcst-1.0.0/libcst/metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ProviderT,
     VisitorMetadataProvider,
 )
 from libcst.metadata.expression_context_provider import (
     ExpressionContext,
     ExpressionContextProvider,
 )
+from libcst.metadata.file_path_provider import FilePathProvider
 from libcst.metadata.full_repo_manager import FullRepoManager
 from libcst.metadata.name_provider import (
     FullyQualifiedNameProvider,
     QualifiedNameProvider,
 )
 from libcst.metadata.parent_node_provider import ParentNodeProvider
 from libcst.metadata.position_provider import (
@@ -84,11 +85,12 @@
     "FullyQualifiedNameProvider",
     "ProviderT",
     "Assignments",
     "Accesses",
     "TypeInferenceProvider",
     "FullRepoManager",
     "AccessorProvider",
+    "FilePathProvider",
     # Experimental APIs:
     "ExperimentalReentrantCodegenProvider",
     "CodegenPartial",
 ]
```

### Comparing `libcst-0.4.9/libcst/metadata/accessor_provider.py` & `libcst-1.0.0/libcst/metadata/accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/base_provider.py` & `libcst-1.0.0/libcst/metadata/base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/expression_context_provider.py` & `libcst-1.0.0/libcst/metadata/expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/full_repo_manager.py` & `libcst-1.0.0/libcst/metadata/full_repo_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 # LICENSE file in the root directory of this source tree.
 
 
 from pathlib import Path
 from typing import Collection, Dict, List, Mapping, TYPE_CHECKING
 
 import libcst as cst
+from libcst._types import StrPath
 from libcst.metadata.wrapper import MetadataWrapper
 
 if TYPE_CHECKING:
     from libcst.metadata.base_provider import ProviderT  # noqa: F401
 
 
 class FullRepoManager:
     def __init__(
         self,
-        repo_root_dir: str,
+        repo_root_dir: StrPath,
         paths: Collection[str],
         providers: Collection["ProviderT"],
         timeout: int = 5,
     ) -> None:
         """
         Given project root directory with pyre and watchman setup, :class:`~libcst.metadata.FullRepoManager`
         handles the inter process communication to read the required full repository cache data for
```

### Comparing `libcst-0.4.9/libcst/metadata/name_provider.py` & `libcst-1.0.0/libcst/metadata/name_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     METADATA_DEPENDENCIES = (QualifiedNameProvider,)
 
     @classmethod
     def gen_cache(
         cls, root_path: Path, paths: List[str], timeout: Optional[int] = None
     ) -> Mapping[str, ModuleNameAndPackage]:
-        cache = {path: calculate_module_and_package(".", path) for path in paths}
+        cache = {path: calculate_module_and_package(root_path, path) for path in paths}
         return cache
 
     def __init__(self, cache: ModuleNameAndPackage) -> None:
         super().__init__(cache)
         self.module_name: str = cache.name
         self.package_name: str = cache.package
```

### Comparing `libcst-0.4.9/libcst/metadata/parent_node_provider.py` & `libcst-1.0.0/libcst/metadata/parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/position_provider.py` & `libcst-1.0.0/libcst/metadata/position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/reentrant_codegen.py` & `libcst-1.0.0/libcst/metadata/reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/scope_provider.py` & `libcst-1.0.0/libcst/metadata/scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/span_provider.py` & `libcst-1.0.0/libcst/metadata/span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_accessor_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_base_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_expression_context_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_full_repo_manager.py` & `libcst-1.0.0/libcst/metadata/tests/test_full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_metadata_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_metadata_wrapper.py` & `libcst-1.0.0/libcst/metadata/tests/test_metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_name_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_name_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 )
 from libcst.metadata.full_repo_manager import FullRepoManager
 from libcst.metadata.name_provider import FullyQualifiedNameVisitor
 from libcst.testing.utils import data_provider, UnitTest
 
 
 class QNameVisitor(cst.CSTVisitor):
-
     METADATA_DEPENDENCIES = (QualifiedNameProvider,)
 
     def __init__(self) -> None:
         self.qnames: Dict["CSTNode", Collection[QualifiedName]] = {}
 
     def on_visit(self, node: cst.CSTNode) -> bool:
         qname = self.get_metadata(QualifiedNameProvider, node)
@@ -539,15 +538,15 @@
         )
         for qname in qnames:
             self.assertEqual(qname.source, names[qname.name], msg=f"{qname}")
 
     def test_local_qualification(self) -> None:
         module_name = "some.test.module"
         package_name = "some.test"
-        for (name, expected) in [
+        for name, expected in [
             (".foo", "some.test.foo"),
             ("..bar", "some.bar"),
             ("foo", "some.test.module.foo"),
         ]:
             with self.subTest(name=name):
                 self.assertEqual(
                     FullyQualifiedNameVisitor._fully_qualify_local(
@@ -556,18 +555,21 @@
                     expected,
                 )
 
 
 class FullyQualifiedNameIntegrationTest(UnitTest):
     def test_with_full_repo_manager(self) -> None:
         with TemporaryDirectory() as dir:
-            fname = "pkg/mod.py"
-            (Path(dir) / "pkg").mkdir()
-            (Path(dir) / fname).touch()
-            mgr = FullRepoManager(dir, [fname], [FullyQualifiedNameProvider])
-            wrapper = mgr.get_metadata_wrapper_for_path(fname)
+            root = Path(dir)
+            file_path = root / "pkg/mod.py"
+            file_path.parent.mkdir()
+            file_path.touch()
+
+            file_path_str = file_path.as_posix()
+            mgr = FullRepoManager(root, [file_path_str], [FullyQualifiedNameProvider])
+            wrapper = mgr.get_metadata_wrapper_for_path(file_path_str)
             fqnames = wrapper.resolve(FullyQualifiedNameProvider)
             (mod, names) = next(iter(fqnames.items()))
             self.assertIsInstance(mod, cst.Module)
             self.assertEqual(
                 names, {QualifiedName(name="pkg.mod", source=QualifiedNameSource.LOCAL)}
             )
```

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_parent_node_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_position_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_reentrant_codegen.py` & `libcst-1.0.0/libcst/metadata/tests/test_reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_scope_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_span_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/metadata/tests/test_type_inference_provider.py` & `libcst-1.0.0/libcst/metadata/tests/test_type_inference_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 import json
 import os
 import subprocess
 import sys
 from pathlib import Path
+from typing import cast, Mapping, Optional
 from unittest import skipIf
 
 import libcst as cst
 from libcst import MetadataWrapper
 from libcst.metadata.type_inference_provider import PyreData, TypeInferenceProvider
 from libcst.testing.utils import data_provider, UnitTest
 from libcst.tests.test_pyre_integration import TEST_SUITE_PATH
@@ -53,14 +54,16 @@
 
 
 @skipIf(
     sys.version_info < (3, 7), "TypeInferenceProvider doesn't support 3.6 and below"
 )
 @skipIf(sys.platform == "win32", "TypeInferenceProvider doesn't support windows")
 class TypeInferenceProviderTest(UnitTest):
+    maxDiff: Optional[int] = None
+
     @classmethod
     def setUpClass(cls) -> None:
         os.chdir(TEST_SUITE_PATH)
         try:
             subprocess.run(["pyre", "-n", "start", "--no-watchman"])
         except subprocess.TimeoutExpired as exc:
             raise exc
@@ -75,16 +78,21 @@
     @data_provider(
         ((TEST_SUITE_PATH / "simple_class.py", TEST_SUITE_PATH / "simple_class.json"),)
     )
     def test_gen_cache(self, source_path: Path, data_path: Path) -> None:
         cache = TypeInferenceProvider.gen_cache(
             root_path=source_path.parent, paths=[source_path.name], timeout=None
         )
+        result = cast(Mapping[str, object], cache[source_path.name])
         data: PyreData = json.loads(data_path.read_text())
-        self.assertEqual(data, cache[source_path.name])
+        self.assertDictEqual(
+            data,
+            result,
+            "Pyre query result mismatch, try running `scripts/regenerate-fixtures.py`?",
+        )
 
     @data_provider(
         ((TEST_SUITE_PATH / "simple_class.py", TEST_SUITE_PATH / "simple_class.json"),)
     )
     def test_simple_class_types(self, source_path: Path, data_path: Path) -> None:
         data: PyreData = json.loads(data_path.read_text())
         wrapper = MetadataWrapper(
```

### Comparing `libcst-0.4.9/libcst/metadata/type_inference_provider.py` & `libcst-1.0.0/libcst/metadata/type_inference_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         root_path: Path, paths: List[str], timeout: Optional[int]
     ) -> Mapping[str, object]:
         params = ",".join(f"path='{root_path / path}'" for path in paths)
         cmd_args = ["pyre", "--noninteractive", "query", f"types({params})"]
         try:
             stdout, stderr, return_code = run_command(cmd_args, timeout=timeout)
         except subprocess.TimeoutExpired as exc:
-
             raise exc
 
         if return_code != 0:
             raise Exception(f"stderr:\n {stderr}\nstdout:\n {stdout}")
         try:
             resp = json.loads(stdout)["response"]
         except Exception as e:
```

### Comparing `libcst-0.4.9/libcst/metadata/wrapper.py` & `libcst-1.0.0/libcst/metadata/wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/testing/utils.py` & `libcst-1.0.0/libcst/testing/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     test_methods_to_add: Dict[str, Callable] = {}
     test_methods_to_remove: List[str] = []
     for member_name, member in dct.items():
         provider_data = try_get_provider_attr(
             member_name, member, DATA_PROVIDER_DATA_ATTR_NAME
         )
         if provider_data is not None:
-
             for description, data in (
                 provider_data.items()
                 if isinstance(provider_data, dict)
                 else enumerate(provider_data)
             ):
                 if isinstance(provider_data, dict):
                     description = f"{DATA_PROVIDER_DESCRIPTION_PREFIX}{description}"
```

### Comparing `libcst-0.4.9/libcst/tests/pyre/simple_class.json` & `libcst-1.0.0/libcst/tests/pyre/simple_class.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999599358974359%*

 * *Differences: {"'types'": "{4: {'location': {'stop': {'column': 24}}}, 14: {'location': {'stop': {'column': "*

 * *            '25}}}}'}*

```diff
@@ -56,15 +56,15 @@
             "annotation": "int",
             "location": {
                 "start": {
                     "column": 23,
                     "line": 11
                 },
                 "stop": {
-                    "column": 29,
+                    "column": 24,
                     "line": 11
                 }
             }
         },
         {
             "annotation": "typing.Type[int]",
             "location": {
@@ -186,15 +186,15 @@
             "annotation": "int",
             "location": {
                 "start": {
                     "column": 24,
                     "line": 16
                 },
                 "stop": {
-                    "column": 30,
+                    "column": 25,
                     "line": 16
                 }
             }
         },
         {
             "annotation": "typing.Type[int]",
             "location": {
```

### Comparing `libcst-0.4.9/libcst/tests/pyre/simple_class.py` & `libcst-1.0.0/libcst/tests/pyre/simple_class.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_add_slots.py` & `libcst-1.0.0/libcst/tests/test_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_batched_visitor.py` & `libcst-1.0.0/libcst/tests/test_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_deep_clone.py` & `libcst-1.0.0/libcst/tests/test_deep_clone.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_deep_replace.py` & `libcst-1.0.0/libcst/tests/test_deep_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_e2e.py` & `libcst-1.0.0/libcst/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_exceptions.py` & `libcst-1.0.0/libcst/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_fuzz.py` & `libcst-1.0.0/libcst/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_tabs.py` & `libcst-1.0.0/libcst/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_tool.py` & `libcst-1.0.0/libcst/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_type_enforce.py` & `libcst-1.0.0/libcst/tests/test_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tests/test_visitor.py` & `libcst-1.0.0/libcst/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/libcst/tool.py` & `libcst-1.0.0/libcst/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -387,60 +387,72 @@
     config = _find_and_load_config(proc_name)
 
     # First, try to grab the command with a first pass. We aren't going to react
     # to user input here, so refuse to add help. Help will be parsed in the
     # full parser below once we know the command and have added its arguments.
     parser = argparse.ArgumentParser(add_help=False, fromfile_prefix_chars="@")
     parser.add_argument("command", metavar="COMMAND", type=str, nargs="?", default=None)
+    ext_action = parser.add_argument(
+        "-x",
+        "--external",
+        action="store_true",
+        default=False,
+        help="Interpret `command` as just a module/class specifier",
+    )
     args, _ = parser.parse_known_args(command_args)
 
     # Now, try to load the class and get its arguments for help purposes.
     if args.command is not None:
-        command_path = args.command.split(".")
-        if len(command_path) < 2:
+        command_module_name, _, command_class_name = args.command.rpartition(".")
+        if not (command_module_name and command_class_name):
             print(f"{args.command} is not a valid codemod command", file=sys.stderr)
             return 1
-        command_module_name, command_class_name = (
-            ".".join(command_path[:-1]),
-            command_path[-1],
-        )
-        command_class = None
-        for module in config["modules"]:
-            try:
-                command_class = getattr(
-                    importlib.import_module(f"{module}.{command_module_name}"),
-                    command_class_name,
-                )
-                break
-            # Only swallow known import errors, show the rest of the exceptions
-            # to the user who is trying to run the codemod.
-            except AttributeError:
-                continue
-            except ModuleNotFoundError:
-                continue
-        if command_class is None:
-            print(
-                f"Could not find {command_module_name} in any configured modules",
-                file=sys.stderr,
+        if args.external:
+            # There's no error handling here on purpose; if the user opted in for `-x`,
+            # they'll probably want to see the exact import error too.
+            command_class = getattr(
+                importlib.import_module(command_module_name),
+                command_class_name,
             )
-            return 1
+        else:
+            command_class = None
+            for module in config["modules"]:
+                try:
+                    command_class = getattr(
+                        importlib.import_module(f"{module}.{command_module_name}"),
+                        command_class_name,
+                    )
+                    break
+                # Only swallow known import errors, show the rest of the exceptions
+                # to the user who is trying to run the codemod.
+                except AttributeError:
+                    continue
+                except ModuleNotFoundError:
+                    continue
+            if command_class is None:
+                print(
+                    f"Could not find {command_module_name} in any configured modules",
+                    file=sys.stderr,
+                )
+                return 1
     else:
         # Dummy, specifically to allow for running --help with no arguments.
         command_class = CodemodCommand
 
     # Now, construct the full parser, parse the args and run the class.
     parser = argparse.ArgumentParser(
         description=(
             "Execute a codemod against a series of files."
             if command_class is CodemodCommand
             else command_class.DESCRIPTION
         ),
         prog=f"{proc_name} codemod",
         fromfile_prefix_chars="@",
     )
+    parser._add_action(ext_action)
     parser.add_argument(
         "command",
         metavar="COMMAND",
         type=str,
         help=(
             "The name of the file (minus the path and extension) and class joined with "
             + "a '.' that defines your command (e.g. strip_strings_from_types.StripStringsCommand)"
@@ -518,34 +530,34 @@
     command_class.add_args(parser)
     args = parser.parse_args(command_args)
 
     codemod_args = {
         k: v
         for k, v in vars(args).items()
         if k
-        not in [
+        not in {
             "command",
-            "path",
-            "unified_diff",
-            "jobs",
-            "python_version",
+            "external",
+            "hide_blacklisted_warnings",
+            "hide_generated_warnings",
+            "hide_progress",
             "include_generated",
             "include_stubs",
+            "jobs",
             "no_format",
+            "path",
+            "python_version",
             "show_successes",
-            "hide_generated_warnings",
-            "hide_blacklisted_warnings",
-            "hide_progress",
-        ]
+            "unified_diff",
+        }
     }
     command_instance = command_class(CodemodContext(), **codemod_args)
 
     # Sepcify target version for black formatter
     if os.path.basename(config["formatter"][0]) in ("black", "black.exe"):
-
         parsed_version = parse_version_string(args.python_version)
 
         config["formatter"] = [
             config["formatter"][0],
             "--target-version",
             f"py{parsed_version.major}{parsed_version.minor}",
         ] + config["formatter"][1:]
```

### Comparing `libcst-0.4.9/libcst.egg-info/SOURCES.txt` & `libcst-1.0.0/libcst.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .watchmanconfig
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.rst
-check_copyright.sh
 codecov.yml
 pyproject.toml
-requirements-dev.txt
-requirements.txt
 setup.py
 .cargo/config.toml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/build-matrix.json
 .github/dependabot.yml
 .github/workflows/build.yml
 .github/workflows/ci.yml
@@ -274,17 +271,19 @@
 libcst/codemod/visitors/tests/test_gather_unused_imports.py
 libcst/codemod/visitors/tests/test_remove_imports.py
 libcst/helpers/__init__.py
 libcst/helpers/_template.py
 libcst/helpers/common.py
 libcst/helpers/expression.py
 libcst/helpers/module.py
+libcst/helpers/paths.py
 libcst/helpers/tests/__init__.py
 libcst/helpers/tests/test_expression.py
 libcst/helpers/tests/test_module.py
+libcst/helpers/tests/test_paths.py
 libcst/helpers/tests/test_template.py
 libcst/matchers/__init__.py
 libcst/matchers/_decorators.py
 libcst/matchers/_matcher_base.py
 libcst/matchers/_return_types.py
 libcst/matchers/_visitors.py
 libcst/matchers/tests/__init__.py
@@ -295,40 +294,43 @@
 libcst/matchers/tests/test_matchers_with_metadata.py
 libcst/matchers/tests/test_replace.py
 libcst/matchers/tests/test_visitors.py
 libcst/metadata/__init__.py
 libcst/metadata/accessor_provider.py
 libcst/metadata/base_provider.py
 libcst/metadata/expression_context_provider.py
+libcst/metadata/file_path_provider.py
 libcst/metadata/full_repo_manager.py
 libcst/metadata/name_provider.py
 libcst/metadata/parent_node_provider.py
 libcst/metadata/position_provider.py
 libcst/metadata/reentrant_codegen.py
 libcst/metadata/scope_provider.py
 libcst/metadata/span_provider.py
 libcst/metadata/type_inference_provider.py
 libcst/metadata/wrapper.py
 libcst/metadata/tests/__init__.py
 libcst/metadata/tests/test_accessor_provider.py
 libcst/metadata/tests/test_base_provider.py
 libcst/metadata/tests/test_expression_context_provider.py
+libcst/metadata/tests/test_file_path_provider.py
 libcst/metadata/tests/test_full_repo_manager.py
 libcst/metadata/tests/test_metadata_provider.py
 libcst/metadata/tests/test_metadata_wrapper.py
 libcst/metadata/tests/test_name_provider.py
 libcst/metadata/tests/test_parent_node_provider.py
 libcst/metadata/tests/test_position_provider.py
 libcst/metadata/tests/test_reentrant_codegen.py
 libcst/metadata/tests/test_scope_provider.py
 libcst/metadata/tests/test_span_provider.py
 libcst/metadata/tests/test_type_inference_provider.py
 libcst/testing/__init__.py
 libcst/testing/utils.py
 libcst/tests/__init__.py
+libcst/tests/__main__.py
 libcst/tests/test_add_slots.py
 libcst/tests/test_batched_visitor.py
 libcst/tests/test_deep_clone.py
 libcst/tests/test_deep_replace.py
 libcst/tests/test_e2e.py
 libcst/tests/test_exceptions.py
 libcst/tests/test_fuzz.py
@@ -412,14 +414,16 @@
 native/libcst_derive/src/cstnode.rs
 native/libcst_derive/src/inflate.rs
 native/libcst_derive/src/into_py.rs
 native/libcst_derive/src/lib.rs
 native/libcst_derive/src/parenthesized_node.rs
 native/libcst_derive/tests/pass/minimal_cst.rs
 native/libcst_derive/tests/pass/simple.rs
+scripts/check_copyright.py
+scripts/regenerate-fixtures.py
 stubs/hypothesis.pyi
 stubs/hypothesmith.pyi
 stubs/setuptools.pyi
 stubs/tokenize.pyi
 stubs/typing_inspect.pyi
 stubs/libcst/native.pyi
 stubs/libcst_native/parser_config.pyi
```

### Comparing `libcst-0.4.9/native/Cargo.lock` & `libcst-1.0.0/native/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,17 @@
  "memchr",
  "regex-automata",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.10.0"
+version = "3.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37ccbd214614c6783386c1af30caf03192f17891059cecc394b4fb119e363de3"
+checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
 
 [[package]]
 name = "cast"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c24dab4283a142afa2fdca129b80ad2c6284e073930f964c3a1293c225ee39a"
 dependencies = [
```

### Comparing `libcst-0.4.9/native/libcst/Cargo.toml` & `libcst-1.0.0/native/libcst/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/Grammar` & `libcst-1.0.0/native/libcst/Grammar`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/README.md` & `libcst-1.0.0/native/libcst/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # libcst/native
 
 A native extension to enable parsing of new Python grammar in LibCST.
 
 The extension is written in Rust, and exposed to Python using [PyO3](https://pyo3.rs/).
-This is packaged together with libcst, and can be imported from `libcst.native`. When
-the `LIBCST_PARSER_TYPE` environment variable is set to `native`, the LibCST APIs use
-this module for all parsing.
+This is packaged together with libcst, and can be imported from `libcst.native`. By default
+the LibCST APIs use this module for all parsing.
 
 Later on, the parser library might be packaged separately as 
 [a Rust crate](https://crates.io). Pull requests towards this are much appreciated.
 
 ## Goals
 
 1. Adopt the CPython grammar definition as closely as possible to reduce maintenance
```

### Comparing `libcst-0.4.9/native/libcst/benches/parser_benchmark.rs` & `libcst-1.0.0/native/libcst/benches/parser_benchmark.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/bin.rs` & `libcst-1.0.0/native/libcst/src/bin.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/lib.rs` & `libcst-1.0.0/native/libcst/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/codegen.rs` & `libcst-1.0.0/native/libcst/src/nodes/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/expression.rs` & `libcst-1.0.0/native/libcst/src/nodes/expression.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/inflate_helpers.rs` & `libcst-1.0.0/native/libcst/src/nodes/inflate_helpers.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/macros.rs` & `libcst-1.0.0/native/libcst/src/nodes/macros.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/mod.rs` & `libcst-1.0.0/native/libcst/src/nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/module.rs` & `libcst-1.0.0/native/libcst/src/nodes/module.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/op.rs` & `libcst-1.0.0/native/libcst/src/nodes/op.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/parser_config.rs` & `libcst-1.0.0/native/libcst/src/nodes/parser_config.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/py_cached.rs` & `libcst-1.0.0/native/libcst/src/nodes/py_cached.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/statement.rs` & `libcst-1.0.0/native/libcst/src/nodes/statement.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/test_utils.rs` & `libcst-1.0.0/native/libcst/src/nodes/test_utils.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/traits.rs` & `libcst-1.0.0/native/libcst/src/nodes/traits.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/nodes/whitespace.rs` & `libcst-1.0.0/native/libcst/src/nodes/whitespace.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/parser/errors.rs` & `libcst-1.0.0/native/libcst/src/parser/errors.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/parser/grammar.rs` & `libcst-1.0.0/native/libcst/src/parser/grammar.rs`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
             }
             / asy:tok(Async, "ASYNC") kw:lit("with") items:separated(<with_item()>, <comma()>)
                 col:lit(":") b:block() {
                     make_with(Some(asy), kw, None, comma_separate(items.0, items.1, None), None, col, b)
             }
 
         rule with_item() -> WithItem<'input, 'a>
-            = e:expression() a:lit("as") t:star_target() &(lit(",") / lit(":")) {
+            = e:expression() a:lit("as") t:star_target() &(lit(",") / lit(":") / rpar()) {
                 make_with_item(e, Some(a), Some(t))
             }
             / e:expression() {
                 make_with_item(e, None, None)
             }
 
         // Try statement
```

### Comparing `libcst-0.4.9/native/libcst/src/parser/numbers.rs` & `libcst-1.0.0/native/libcst/src/parser/numbers.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/py.rs` & `libcst-1.0.0/native/libcst/src/py.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/core/LICENSE` & `libcst-1.0.0/native/libcst/src/tokenizer/core/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/core/mod.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/core/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -969,16 +969,16 @@
                                 self.text_pos.next();
                             }
                         }
                     }
                 }
                 (Some('\\'), _) if is_raw_string => {
                     self.text_pos.next();
-                    if let Some('"' | '\'') = self.text_pos.peek() {
-                        // these aren't end of string markers, skip them
+                    // skip escaped end-of-string marker or backslash
+                    if let Some('"' | '\'' | '\\') = self.text_pos.peek() {
                         self.text_pos.next();
                     }
                 }
                 (Some('{'), _) => {
                     if is_in_format_spec {
                         // don't actually consume the {, and generate an OP for it instead
                         break 'outer;
```

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/core/string_types.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/core/string_types.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/operators.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/operators.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/tests.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -525,14 +525,18 @@
         tokenize_all("r'\\''", &default_config()),
         Ok(vec![(TokType::String, "r'\\''")]),
     );
     assert_eq!(
         tokenize_all(r#"r"\"""#, &default_config()),
         Ok(vec![(TokType::String, r#"r"\"""#)]),
     );
+    assert_eq!(
+        tokenize_all(r#"r'\\'"#, &default_config()),
+        Ok(vec![(TokType::String, r#"r'\\'"#)]),
+    );
     let config = TokConfig {
         split_fstring: true,
         ..default_config()
     };
     assert_eq!(
         tokenize_all("rf'\\''", &config),
         Ok(vec![
@@ -545,14 +549,22 @@
         tokenize_all(r#"rf"\"""#, &config),
         Ok(vec![
             (TokType::FStringStart, "rf\""),
             (TokType::FStringString, r#"\""#),
             (TokType::FStringEnd, "\""),
         ]),
     );
+    assert_eq!(
+        tokenize_all(r#"rf'\\'"#, &config),
+        Ok(vec![
+            (TokType::FStringStart, "rf'"),
+            (TokType::FStringString, r#"\\"#),
+            (TokType::FStringEnd, "'"),
+        ]),
+    );
 }
 
 #[test]
 fn test_split_fstring() {
     let config = TokConfig {
         split_fstring: true,
         ..default_config()
```

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/text_position/char_width.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/text_position/char_width.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/text_position/mod.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/text_position/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/src/tokenizer/whitespace_parser.rs` & `libcst-1.0.0/native/libcst/src/tokenizer/whitespace_parser.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/big_binary_operator.py` & `libcst-1.0.0/native/libcst/tests/fixtures/big_binary_operator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/comments.py` & `libcst-1.0.0/native/libcst/tests/fixtures/comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/expr.py` & `libcst-1.0.0/native/libcst/tests/fixtures/expr.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/fun_with_func_defs.py` & `libcst-1.0.0/native/libcst/tests/fixtures/fun_with_func_defs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/malicious_match.py` & `libcst-1.0.0/native/libcst/tests/fixtures/malicious_match.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/pep646.py` & `libcst-1.0.0/native/libcst/tests/fixtures/pep646.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/fixtures/super_strings.py` & `libcst-1.0.0/native/libcst/tests/fixtures/super_strings.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst/tests/parser_roundtrip.rs` & `libcst-1.0.0/native/libcst/tests/parser_roundtrip.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/codegen.rs` & `libcst-1.0.0/native/libcst_derive/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/cstnode.rs` & `libcst-1.0.0/native/libcst_derive/src/cstnode.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/inflate.rs` & `libcst-1.0.0/native/libcst_derive/src/inflate.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/into_py.rs` & `libcst-1.0.0/native/libcst_derive/src/into_py.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/lib.rs` & `libcst-1.0.0/native/libcst_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/src/parenthesized_node.rs` & `libcst-1.0.0/native/libcst_derive/src/parenthesized_node.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/tests/pass/minimal_cst.rs` & `libcst-1.0.0/native/libcst_derive/tests/pass/minimal_cst.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/native/libcst_derive/tests/pass/simple.rs` & `libcst-1.0.0/native/libcst_derive/tests/pass/simple.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/libcst_native/parser_config.pyi` & `libcst-1.0.0/stubs/libcst_native/parser_config.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/libcst_native/token_type.pyi` & `libcst-1.0.0/stubs/libcst_native/token_type.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/libcst_native/tokenize.pyi` & `libcst-1.0.0/stubs/libcst_native/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/libcst_native/whitespace_parser.pyi` & `libcst-1.0.0/stubs/libcst_native/whitespace_parser.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/libcst_native/whitespace_state.pyi` & `libcst-1.0.0/stubs/libcst_native/whitespace_state.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.9/stubs/tokenize.pyi` & `libcst-1.0.0/stubs/tokenize.pyi`

 * *Files identical despite different names*

