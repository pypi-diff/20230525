# Comparing `tmp/schemathesis-3.9.6.tar.gz` & `tmp/schemathesis-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemathesis-3.9.6.tar", max compression
+gzip compressed data, was "schemathesis-3.9.7.tar", max compression
```

## Comparing `schemathesis-3.9.6.tar` & `schemathesis-3.9.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1098 2021-07-15 18:24:02.014131 schemathesis-3.9.6/LICENSE
--rw-r--r--   0        0        0     5778 2021-07-15 18:24:02.014131 schemathesis-3.9.6/README.rst
--rw-r--r--   0        0        0     2952 2021-07-15 18:24:02.018131 schemathesis-3.9.6/pyproject.toml
--rw-r--r--   0        0        0      900 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/__init__.py
--rw-r--r--   0        0        0     1406 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/_compat.py
--rw-r--r--   0        0        0     5294 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/_hypothesis.py
--rw-r--r--   0        0        0     1166 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/checks.py
--rw-r--r--   0        0        0    33611 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/__init__.py
--rw-r--r--   0        0        0     6899 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/callbacks.py
--rw-r--r--   0        0        0     8942 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/cassettes.py
--rw-r--r--   0        0        0       63 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/constants.py
--rw-r--r--   0        0        0     1380 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/context.py
--rw-r--r--   0        0        0      579 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/debug.py
--rw-r--r--   0        0        0     1347 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/handlers.py
--rw-r--r--   0        0        0     1897 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/junitxml.py
--rw-r--r--   0        0        0     1771 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/options.py
--rw-r--r--   0        0        0       29 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/output/__init__.py
--rw-r--r--   0        0        0    16108 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/output/default.py
--rw-r--r--   0        0        0     1628 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/cli/output/short.py
--rw-r--r--   0        0        0     2164 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/constants.py
--rw-r--r--   0        0        0     7017 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/exceptions.py
--rw-r--r--   0        0        0        0 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/extra/__init__.py
--rw-r--r--   0        0        0      952 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/extra/_aiohttp.py
--rw-r--r--   0        0        0      285 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/extra/_flask.py
--rw-r--r--   0        0        0      518 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/extra/_server.py
--rw-r--r--   0        0        0     8633 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/extra/pytest_plugin.py
--rw-r--r--   0        0        0     4546 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/failures.py
--rw-r--r--   0        0        0      763 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/fixups/__init__.py
--rw-r--r--   0        0        0     1022 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/fixups/fast_api.py
--rw-r--r--   0        0        0     8704 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/hooks.py
--rw-r--r--   0        0        0     9463 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/lazy.py
--rw-r--r--   0        0        0    39919 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/models.py
--rw-r--r--   0        0        0     2382 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/parameters.py
--rw-r--r--   0        0        0        0 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/py.typed
--rw-r--r--   0        0        0    16674 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/__init__.py
--rw-r--r--   0        0        0     8522 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/events.py
--rw-r--r--   0        0        0      199 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/impl/__init__.py
--rw-r--r--   0        0        0    26695 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/impl/core.py
--rw-r--r--   0        0        0     2710 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/impl/solo.py
--rw-r--r--   0        0        0    11375 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/impl/threadpool.py
--rw-r--r--   0        0        0     6598 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/runner/serialization.py
--rw-r--r--   0        0        0    14365 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/schemas.py
--rw-r--r--   0        0        0     8312 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/serializers.py
--rw-r--r--   0        0        0        0 2021-07-15 18:24:02.018131 schemathesis-3.9.6/src/schemathesis/specs/__init__.py
--rw-r--r--   0        0        0       85 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/graphql/__init__.py
--rw-r--r--   0        0        0     7328 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/graphql/loaders.py
--rw-r--r--   0        0        0     4369 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/graphql/schemas.py
--rw-r--r--   0        0        0      120 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/__init__.py
--rw-r--r--   0        0        0    16766 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/_hypothesis.py
--rw-r--r--   0        0        0     4590 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/checks.py
--rw-r--r--   0        0        0      151 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/constants.py
--rw-r--r--   0        0        0      841 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/converter.py
--rw-r--r--   0        0        0    65299 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/definitions.py
--rw-r--r--   0        0        0     8958 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/examples.py
--rw-r--r--   0        0        0      660 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/__init__.py
--rw-r--r--   0        0        0      314 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/context.py
--rw-r--r--   0        0        0      219 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/errors.py
--rw-r--r--   0        0        0     4046 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/lexer.py
--rw-r--r--   0        0        0     3707 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/nodes.py
--rw-r--r--   0        0        0     3520 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/parser.py
--rw-r--r--   0        0        0      879 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/pointers.py
--rw-r--r--   0        0        0     1335 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/filters.py
--rw-r--r--   0        0        0    14733 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/links.py
--rw-r--r--   0        0        0    13412 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/loaders.py
--rw-r--r--   0        0        0     1636 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/__init__.py
--rw-r--r--   0        0        0    19544 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/mutations.py
--rw-r--r--   0        0        0      174 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/types.py
--rw-r--r--   0        0        0      269 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/utils.py
--rw-r--r--   0        0        0    13823 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/parameters.py
--rw-r--r--   0        0        0     3828 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/references.py
--rw-r--r--   0        0        0    33326 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/schemas.py
--rw-r--r--   0        0        0     6076 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/security.py
--rw-r--r--   0        0        0    11457 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/serialization.py
--rw-r--r--   0        0        0     3787 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/stateful/__init__.py
--rw-r--r--   0        0        0     3245 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/stateful/links.py
--rw-r--r--   0        0        0      488 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/specs/openapi/utils.py
--rw-r--r--   0        0        0    14066 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/stateful.py
--rw-r--r--   0        0        0      850 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/targets.py
--rw-r--r--   0        0        0     1095 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/types.py
--rw-r--r--   0        0        0    12822 2021-07-15 18:24:02.022131 schemathesis-3.9.6/src/schemathesis/utils.py
--rw-r--r--   0        0        0     7765 2021-07-15 18:24:10.165353 schemathesis-3.9.6/setup.py
--rw-r--r--   0        0        0     7837 2021-07-15 18:24:10.166036 schemathesis-3.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1098 2021-07-26 17:56:40.520843 schemathesis-3.9.7/LICENSE
+-rw-r--r--   0        0        0     5778 2021-07-26 17:56:40.520843 schemathesis-3.9.7/README.rst
+-rw-r--r--   0        0        0     2952 2021-07-26 17:56:40.524844 schemathesis-3.9.7/pyproject.toml
+-rw-r--r--   0        0        0      900 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/__init__.py
+-rw-r--r--   0        0        0     1406 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/_compat.py
+-rw-r--r--   0        0        0     5294 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/_hypothesis.py
+-rw-r--r--   0        0        0     1166 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/checks.py
+-rw-r--r--   0        0        0    33962 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/__init__.py
+-rw-r--r--   0        0        0     6899 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/callbacks.py
+-rw-r--r--   0        0        0     8942 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/cassettes.py
+-rw-r--r--   0        0        0       63 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/constants.py
+-rw-r--r--   0        0        0     1380 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/context.py
+-rw-r--r--   0        0        0      579 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/debug.py
+-rw-r--r--   0        0        0     1347 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/handlers.py
+-rw-r--r--   0        0        0     1897 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/junitxml.py
+-rw-r--r--   0        0        0     1771 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/options.py
+-rw-r--r--   0        0        0       29 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/output/__init__.py
+-rw-r--r--   0        0        0    16108 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/output/default.py
+-rw-r--r--   0        0        0     1628 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/cli/output/short.py
+-rw-r--r--   0        0        0     2164 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/constants.py
+-rw-r--r--   0        0        0     7017 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/exceptions.py
+-rw-r--r--   0        0        0        0 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/extra/__init__.py
+-rw-r--r--   0        0        0      952 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/extra/_aiohttp.py
+-rw-r--r--   0        0        0      285 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/extra/_flask.py
+-rw-r--r--   0        0        0      518 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/extra/_server.py
+-rw-r--r--   0        0        0     8633 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/extra/pytest_plugin.py
+-rw-r--r--   0        0        0     4546 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/failures.py
+-rw-r--r--   0        0        0      763 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/fixups/__init__.py
+-rw-r--r--   0        0        0     1022 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/fixups/fast_api.py
+-rw-r--r--   0        0        0     8704 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/hooks.py
+-rw-r--r--   0        0        0     9463 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/lazy.py
+-rw-r--r--   0        0        0    39919 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/models.py
+-rw-r--r--   0        0        0     2382 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/parameters.py
+-rw-r--r--   0        0        0        0 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/py.typed
+-rw-r--r--   0        0        0    16674 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/__init__.py
+-rw-r--r--   0        0        0     8522 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/events.py
+-rw-r--r--   0        0        0      199 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/impl/__init__.py
+-rw-r--r--   0        0        0    27102 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/impl/core.py
+-rw-r--r--   0        0        0     2710 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/impl/solo.py
+-rw-r--r--   0        0        0    11375 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/impl/threadpool.py
+-rw-r--r--   0        0        0     6598 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/runner/serialization.py
+-rw-r--r--   0        0        0    14365 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/schemas.py
+-rw-r--r--   0        0        0     8312 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/serializers.py
+-rw-r--r--   0        0        0        0 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/__init__.py
+-rw-r--r--   0        0        0       85 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/graphql/__init__.py
+-rw-r--r--   0        0        0     7328 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/graphql/loaders.py
+-rw-r--r--   0        0        0     4369 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/graphql/schemas.py
+-rw-r--r--   0        0        0      120 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/__init__.py
+-rw-r--r--   0        0        0    16766 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/_hypothesis.py
+-rw-r--r--   0        0        0     4590 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/checks.py
+-rw-r--r--   0        0        0      151 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/constants.py
+-rw-r--r--   0        0        0      841 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/converter.py
+-rw-r--r--   0        0        0    65299 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/definitions.py
+-rw-r--r--   0        0        0     8958 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/examples.py
+-rw-r--r--   0        0        0      660 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/__init__.py
+-rw-r--r--   0        0        0      314 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/context.py
+-rw-r--r--   0        0        0      219 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/errors.py
+-rw-r--r--   0        0        0     4046 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/lexer.py
+-rw-r--r--   0        0        0     3707 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/nodes.py
+-rw-r--r--   0        0        0     3520 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/parser.py
+-rw-r--r--   0        0        0      879 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/pointers.py
+-rw-r--r--   0        0        0     1335 2021-07-26 17:56:40.524844 schemathesis-3.9.7/src/schemathesis/specs/openapi/filters.py
+-rw-r--r--   0        0        0    14839 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/links.py
+-rw-r--r--   0        0        0    13412 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/loaders.py
+-rw-r--r--   0        0        0     1636 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/__init__.py
+-rw-r--r--   0        0        0    19544 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/mutations.py
+-rw-r--r--   0        0        0      174 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/types.py
+-rw-r--r--   0        0        0      269 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/utils.py
+-rw-r--r--   0        0        0    13823 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/parameters.py
+-rw-r--r--   0        0        0     3828 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/references.py
+-rw-r--r--   0        0        0    33326 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/schemas.py
+-rw-r--r--   0        0        0     6076 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/security.py
+-rw-r--r--   0        0        0    11457 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/serialization.py
+-rw-r--r--   0        0        0     3787 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/stateful/__init__.py
+-rw-r--r--   0        0        0     3245 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/stateful/links.py
+-rw-r--r--   0        0        0      488 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/specs/openapi/utils.py
+-rw-r--r--   0        0        0    14066 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/stateful.py
+-rw-r--r--   0        0        0      850 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/targets.py
+-rw-r--r--   0        0        0     1095 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/types.py
+-rw-r--r--   0        0        0    12822 2021-07-26 17:56:40.528843 schemathesis-3.9.7/src/schemathesis/utils.py
+-rw-r--r--   0        0        0     7765 2021-07-26 17:56:48.996804 schemathesis-3.9.7/setup.py
+-rw-r--r--   0        0        0     7837 2021-07-26 17:56:48.997606 schemathesis-3.9.7/PKG-INFO
```

### Comparing `schemathesis-3.9.6/LICENSE` & `schemathesis-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/README.rst` & `schemathesis-3.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/pyproject.toml` & `schemathesis-3.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemathesis"
-version = "3.9.6"
+version = "3.9.7"
 description = "Property-based testing framework for Open API and GraphQL based apps"
 keywords = ["pytest", "hypothesis", "openapi", "swagger", "graphql", "testing"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Pytest",
     "Framework :: Hypothesis",
```

### Comparing `schemathesis-3.9.6/src/schemathesis/__init__.py` & `schemathesis-3.9.7/src/schemathesis/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/_compat.py` & `schemathesis-3.9.7/src/schemathesis/_compat.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/_hypothesis.py` & `schemathesis-3.9.7/src/schemathesis/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/checks.py` & `schemathesis-3.9.7/src/schemathesis/checks.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/__init__.py` & `schemathesis-3.9.7/src/schemathesis/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,7 +945,16 @@
 
     Note that you need to modify the response in-place.
 
     Use cases:
      - Response post-processing, like modifying its payload.
      - Logging
     """
+
+
+@HookDispatcher.register_spec([HookScope.GLOBAL])
+def process_call_kwargs(context: HookContext, case: Case, kwargs: Dict[str, Any]) -> None:
+    """Called before every network call in CLI tests.
+
+    Aims to modify the argument passed to `case.call` / `case.call_wsgi` / `case.call_asgi`.
+    Note that you need to modify `kwargs` in-place.
+    """
```

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/callbacks.py` & `schemathesis-3.9.7/src/schemathesis/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/cassettes.py` & `schemathesis-3.9.7/src/schemathesis/cli/cassettes.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/context.py` & `schemathesis-3.9.7/src/schemathesis/cli/context.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/debug.py` & `schemathesis-3.9.7/src/schemathesis/cli/debug.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/handlers.py` & `schemathesis-3.9.7/src/schemathesis/cli/handlers.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/junitxml.py` & `schemathesis-3.9.7/src/schemathesis/cli/junitxml.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/options.py` & `schemathesis-3.9.7/src/schemathesis/cli/options.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/output/default.py` & `schemathesis-3.9.7/src/schemathesis/cli/output/default.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/cli/output/short.py` & `schemathesis-3.9.7/src/schemathesis/cli/output/short.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/constants.py` & `schemathesis-3.9.7/src/schemathesis/constants.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/exceptions.py` & `schemathesis-3.9.7/src/schemathesis/exceptions.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/extra/_aiohttp.py` & `schemathesis-3.9.7/src/schemathesis/extra/_aiohttp.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/extra/_server.py` & `schemathesis-3.9.7/src/schemathesis/extra/_server.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/extra/pytest_plugin.py` & `schemathesis-3.9.7/src/schemathesis/extra/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/failures.py` & `schemathesis-3.9.7/src/schemathesis/failures.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/fixups/__init__.py` & `schemathesis-3.9.7/src/schemathesis/fixups/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/fixups/fast_api.py` & `schemathesis-3.9.7/src/schemathesis/fixups/fast_api.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/hooks.py` & `schemathesis-3.9.7/src/schemathesis/hooks.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/lazy.py` & `schemathesis-3.9.7/src/schemathesis/lazy.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/models.py` & `schemathesis-3.9.7/src/schemathesis/models.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/parameters.py` & `schemathesis-3.9.7/src/schemathesis/parameters.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/__init__.py` & `schemathesis-3.9.7/src/schemathesis/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/events.py` & `schemathesis-3.9.7/src/schemathesis/runner/events.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/impl/core.py` & `schemathesis-3.9.7/src/schemathesis/runner/impl/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,15 +523,22 @@
     request_tls_verify: bool,
     max_response_time: Optional[int],
 ) -> requests.Response:
     check_results: List[Check] = []
     try:
         hook_context = HookContext(operation=case.operation)
         hooks.dispatch("before_call", hook_context, case)
-        response = case.call(session=session, headers=headers, timeout=timeout, verify=request_tls_verify)
+        kwargs: Dict[str, Any] = {
+            "session": session,
+            "headers": headers,
+            "timeout": timeout,
+            "verify": request_tls_verify,
+        }
+        hooks.dispatch("process_call_kwargs", hook_context, case, kwargs)
+        response = case.call(**kwargs)
         hooks.dispatch("after_call", hook_context, case, response)
     except CheckFailed as exc:
         check_name = "request_timeout"
         requests_kwargs = case.as_requests_kwargs(base_url=case.get_full_base_url(), headers=headers)
         request = requests.Request(**requests_kwargs).prepare()
         elapsed = cast(float, timeout)  # It is defined and not empty, since the exception happened
         check_result = result.add_failure(
@@ -614,15 +621,17 @@
     feedback: Feedback,
     max_response_time: Optional[int],
 ) -> WSGIResponse:
     with catching_logs(LogCaptureHandler(), level=logging.DEBUG) as recorded:
         start = time.monotonic()
         hook_context = HookContext(operation=case.operation)
         hooks.dispatch("before_call", hook_context, case)
-        response = case.call_wsgi(headers=headers)
+        kwargs = {"headers": headers}
+        hooks.dispatch("process_call_kwargs", hook_context, case, kwargs)
+        response = case.call_wsgi(**kwargs)
         hooks.dispatch("after_call", hook_context, case, response)
         elapsed = time.monotonic() - start
     context = TargetContext(case=case, response=response, response_time=elapsed)
     run_targets(targets, context)
     result.logs.extend(recorded.records)
     status = Status.success
     check_results: List[Check] = []
@@ -700,15 +709,17 @@
     store_interactions: bool,
     headers: Optional[Dict[str, Any]],
     feedback: Feedback,
     max_response_time: Optional[int],
 ) -> requests.Response:
     hook_context = HookContext(operation=case.operation)
     hooks.dispatch("before_call", hook_context, case)
-    response = case.call_asgi(headers=headers)
+    kwargs: Dict[str, Any] = {"headers": headers}
+    hooks.dispatch("process_call_kwargs", hook_context, case, kwargs)
+    response = case.call_asgi(**kwargs)
     hooks.dispatch("after_call", hook_context, case, response)
     context = TargetContext(case=case, response=response, response_time=response.elapsed.total_seconds())
     run_targets(targets, context)
     status = Status.success
     check_results: List[Check] = []
     try:
         run_checks(case, checks, check_results, result, response, context.response_time * 1000, max_response_time)
```

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/impl/solo.py` & `schemathesis-3.9.7/src/schemathesis/runner/impl/solo.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/impl/threadpool.py` & `schemathesis-3.9.7/src/schemathesis/runner/impl/threadpool.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/runner/serialization.py` & `schemathesis-3.9.7/src/schemathesis/runner/serialization.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/schemas.py` & `schemathesis-3.9.7/src/schemathesis/schemas.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/serializers.py` & `schemathesis-3.9.7/src/schemathesis/serializers.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/graphql/loaders.py` & `schemathesis-3.9.7/src/schemathesis/specs/graphql/loaders.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/graphql/schemas.py` & `schemathesis-3.9.7/src/schemathesis/specs/graphql/schemas.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/_hypothesis.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/checks.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/checks.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/converter.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/converter.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/definitions.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/definitions.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/examples.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/examples.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/__init__.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/lexer.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/lexer.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/nodes.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/nodes.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/parser.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/parser.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/expressions/pointers.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/expressions/pointers.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/filters.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/filters.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/links.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
 
 
 def get_links(response: GenericResponse, operation: APIOperation, field: str) -> Sequence[Link]:
     """Get `x-links` / `links` definitions from the schema."""
     responses = operation.definition.resolved["responses"]
     if str(response.status_code) in responses:
         response_definition = responses[str(response.status_code)]
+    elif response.status_code in responses:
+        response_definition = responses[response.status_code]
     else:
         response_definition = responses.get("default", {})
     links = response_definition.get(field, {})
     return [Link.from_definition(name, definition, operation) for name, definition in links.items()]
 
 
 @attr.s(slots=True, repr=False)  # pragma: no mutate
```

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/loaders.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/loaders.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/__init__.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/negative/mutations.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/negative/mutations.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/parameters.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/references.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/references.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/schemas.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/schemas.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/security.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/security.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/serialization.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/serialization.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/stateful/__init__.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/stateful/__init__.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/specs/openapi/stateful/links.py` & `schemathesis-3.9.7/src/schemathesis/specs/openapi/stateful/links.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/stateful.py` & `schemathesis-3.9.7/src/schemathesis/stateful.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/targets.py` & `schemathesis-3.9.7/src/schemathesis/targets.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/types.py` & `schemathesis-3.9.7/src/schemathesis/types.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/src/schemathesis/utils.py` & `schemathesis-3.9.7/src/schemathesis/utils.py`

 * *Files identical despite different names*

### Comparing `schemathesis-3.9.6/setup.py` & `schemathesis-3.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 entry_points = \
 {'console_scripts': ['schemathesis = schemathesis.cli:schemathesis'],
  'pytest11': ['schemathesis = schemathesis.extra.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'schemathesis',
-    'version': '3.9.6',
+    'version': '3.9.7',
     'description': 'Property-based testing framework for Open API and GraphQL based apps',
     'long_description': 'Schemathesis\n============\n\n|Build| |Coverage| |Version| |Python versions| |Docs| |Chat| |License|\n\nSchemathesis is a modern API testing tool for web applications built with Open API and GraphQL specifications.\n\nIt reads the application schema and generates test cases, which will ensure that your application is compliant with its schema.\n\nThe application under test could be written in any language; the only thing you need is a valid API schema in a supported format.\n\nSimple to use and yet powerful to uncover hard-to-find errors thanks to the property-based testing approach backed by state-of-the-art `Hypothesis <http://hypothesis.works/>`_ library.\n\n📣 **Please fill out our** `quick survey <https://forms.gle/dv4s5SXAYWzvuwFWA>`_ so that we can learn how satisfied you are with Schemathesis, and what improvements we should make. Thank you!\n\nFeatures\n--------\n\n- Content-Type, schema, and status code conformance checks for Open API;\n- Testing of explicit examples from the input schema;\n- Stateful testing via Open API links;\n- Concurrent test execution;\n- Targeted testing;\n- Storing and replaying network requests;\n- Built-in ASGI / WSGI application support;\n- Code samples for easy failure reproduction;\n- Ready-to-go Docker image;\n- Configurable with user-defined checks, string formats, hooks, and targets.\n\nInstallation\n------------\n\nTo install Schemathesis via ``pip`` run the following command:\n\n.. code:: bash\n\n    pip install schemathesis\n\nUsage\n-----\n\nYou can use Schemathesis in the command line:\n\n.. code:: bash\n\n  schemathesis run --stateful=links --checks all http://0.0.0.0:8081/schema.yaml\n\n.. image:: https://raw.githubusercontent.com/schemathesis/schemathesis/master/img/schemathesis.gif\n\nOr in your Python tests:\n\n.. code:: python\n\n    import schemathesis\n\n    schema = schemathesis.from_uri("http://0.0.0.0:8081/schema.yaml")\n\n\n    @schema.parametrize()\n    def test_api(case):\n        case.call_and_validate()\n\nCLI is simple to use and requires no coding; the in-code approach gives more flexibility.\n\nBoth examples above will run hundreds of requests against the API under test and report all found failures and inconsistencies along with instructions to reproduce them.\n\n💡 See a complete working example project in the ``/example`` directory. 💡\n\nContributing\n------------\n\nAny contribution to development, testing, or any other area is highly appreciated and useful to the project.\nFor guidance on how to contribute to Schemathesis, see the `contributing guidelines <https://github.com/schemathesis/schemathesis/blob/master/CONTRIBUTING.rst>`_.\n\nSupport this project\n--------------------\n\nHi, my name is Dmitry! I started this project during my work at `Kiwi.com <https://kiwi.com/>`_. I am grateful to them for all the support they\nprovided to this project during its early days and for the opportunity to evolve Schemathesis independently.\n\nIn order to grow the community of contributors and users, and allow me to devote more time to this project, please `donate today <https://github.com/sponsors/Stranger6667>`_.\n\nAlso, I occasionally write posts about Schemathesis in `my blog <https://dygalo.dev/>`_ and offer consulting services for businesses.\n\nCommercial support\n------------------\n\nIf you are interested in the effective integration of Schemathesis to your private project, you can contact me via email or `Twitter <https://twitter.com/Stranger6667>`_ and I will help you do that.\n\nLinks\n-----\n\n- **Documentation**: https://schemathesis.readthedocs.io/en/stable/\n- **Releases**: https://pypi.org/project/schemathesis/\n- **Code**: https://github.com/schemathesis/schemathesis\n- **Issue tracker**: https://github.com/schemathesis/schemathesis/issues\n- **Chat**: https://gitter.im/schemathesis/schemathesis\n\nAdditional content:\n\n- `An article <https://dygalo.dev/blog/schemathesis-property-based-testing-for-api-schemas/>`_ about Schemathesis by **@Stranger6667**\n- `Effective API schemas testing <https://youtu.be/VVLZ25JgjD4>`_ from DevConf.cz by **@Stranger6667**\n- `A video <https://www.youtube.com/watch?v=9FHRwrv-xuQ>`_ from EuroPython 2020 by **@hultner**\n- `Schemathesis tutorial <https://appdev.consulting.redhat.com/tracks/contract-first/automated-testing-with-schemathesis.html>`_  with an accompanying `video <https://www.youtube.com/watch?v=4r7OC-lBKMg>`_ by Red Hat\n- `Using Hypothesis and Schemathesis to Test FastAPI <https://testdriven.io/blog/fastapi-hypothesis/>`_ by **@amalshaji**\n\nLicense\n-------\n\nThe code in this project is licensed under `MIT license`_.\nBy contributing to Schemathesis, you agree that your contributions will be licensed under its MIT license.\n\n.. |Build| image:: https://github.com/schemathesis/schemathesis/workflows/build/badge.svg\n   :target: https://github.com/schemathesis/schemathesis/actions\n.. |Coverage| image:: https://codecov.io/gh/schemathesis/schemathesis/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/schemathesis/schemathesis/branch/master\n   :alt: codecov.io status for master branch\n.. |Version| image:: https://img.shields.io/pypi/v/schemathesis.svg\n   :target: https://pypi.org/project/schemathesis/\n.. |Python versions| image:: https://img.shields.io/pypi/pyversions/schemathesis.svg\n   :target: https://pypi.org/project/schemathesis/\n.. |License| image:: https://img.shields.io/pypi/l/schemathesis.svg\n   :target: https://opensource.org/licenses/MIT\n.. |Chat| image:: https://img.shields.io/gitter/room/schemathesis/schemathesis.svg\n   :target: https://gitter.im/schemathesis/schemathesis\n   :alt: Gitter\n.. |Docs| image:: https://readthedocs.org/projects/schemathesis/badge/?version=stable\n   :target: https://schemathesis.readthedocs.io/en/stable/?badge=stable\n   :alt: Documentation Status\n\n.. _MIT license: https://opensource.org/licenses/MIT\n',
     'author': 'Dmitry Dygalo',
     'author_email': 'dadygalo@gmail.com',
     'maintainer': 'Dmitry Dygalo',
     'maintainer_email': 'dadygalo@gmail.com',
     'url': 'https://github.com/schemathesis/schemathesis',
```

### Comparing `schemathesis-3.9.6/PKG-INFO` & `schemathesis-3.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemathesis
-Version: 3.9.6
+Version: 3.9.7
 Summary: Property-based testing framework for Open API and GraphQL based apps
 Home-page: https://github.com/schemathesis/schemathesis
 License: MIT
 Keywords: pytest,hypothesis,openapi,swagger,graphql,testing
 Author: Dmitry Dygalo
 Author-email: dadygalo@gmail.com
 Maintainer: Dmitry Dygalo
```

