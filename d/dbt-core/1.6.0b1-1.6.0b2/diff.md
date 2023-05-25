# Comparing `tmp/dbt-core-1.6.0b1.tar.gz` & `tmp/dbt-core-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b1.tar", last modified: Fri May 12 17:40:56 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0b2.tar", last modified: Thu May 25 15:44:07 2023, max compression
```

## Comparing `dbt-core-1.6.0b1.tar` & `dbt-core-1.6.0b2.tar`

### file list

```diff
@@ -1,313 +1,318 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.358163 dbt-core-1.6.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.362163 dbt-core-1.6.0b1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.362163 dbt-core-1.6.0b1/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    55757 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.362163 dbt-core-1.6.0b1/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.362163 dbt-core-1.6.0b1/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/cli/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.366163 dbt-core-1.6.0b1/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.366163 dbt-core-1.6.0b1/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.370163 dbt-core-1.6.0b1/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    59345 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.370163 dbt-core-1.6.0b1/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.370163 dbt-core-1.6.0b1/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48234 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    50566 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.354163 dbt-core-1.6.0b1/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    60037 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   102412 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79357 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.374163 dbt-core-1.6.0b1/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.378163 dbt-core-1.6.0b1/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.378163 dbt-core-1.6.0b1/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.354163 dbt-core-1.6.0b1/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.378163 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.378163 dbt-core-1.6.0b1/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.354163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.382163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.386163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.386163 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.386163 dbt-core-1.6.0b1/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.354163 dbt-core-1.6.0b1/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.354163 dbt-core-1.6.0b1/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.390163 dbt-core-1.6.0b1/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.394163 dbt-core-1.6.0b1/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    74012 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59504 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 17:40:56.000000 dbt-core-1.6.0b1/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:40:56.398163 dbt-core-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-12 17:40:42.000000 dbt-core-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55757 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.768683 dbt-core-1.6.0b2/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59345 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.768683 dbt-core-1.6.0b2/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49014 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.752683 dbt-core-1.6.0b2/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62446 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104888 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.752683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.792684 dbt-core-1.6.0b2/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76488 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/setup.py
```

### Comparing `dbt-core-1.6.0b1/PKG-INFO` & `dbt-core-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b1/README.md` & `dbt-core-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0b2/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/column.py` & `dbt-core-1.6.0b2/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/connections.py` & `dbt-core-1.6.0b2/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/impl.py` & `dbt-core-1.6.0b2/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/meta.py` & `dbt-core-1.6.0b2/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0b2/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0b2/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/base/relation.py` & `dbt-core-1.6.0b2/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/cache.py` & `dbt-core-1.6.0b2/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/factory.py` & `dbt-core-1.6.0b2/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/protocol.py` & `dbt-core-1.6.0b2/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0b2/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0b2/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0b2/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/cli/exceptions.py` & `dbt-core-1.6.0b2/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/cli/main.py` & `dbt-core-1.6.0b2/dbt/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     DbtInternalException,
     DbtUsageException,
 )
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.results import (
     CatalogArtifact,
     RunExecutionResult,
-    RunOperationResultsArtifact,
 )
 from dbt.events.base_types import EventMsg
 from dbt.task.build import BuildTask
 from dbt.task.clean import CleanTask
 from dbt.task.compile import CompileTask
 from dbt.task.debug import DebugTask
 from dbt.task.deps import DepsTask
@@ -49,16 +48,15 @@
     exception: Optional[BaseException] = None
     result: Union[
         bool,  # debug
         CatalogArtifact,  # docs generate
         List[str],  # list/ls
         Manifest,  # parse
         None,  # clean, deps, init, source
-        RunExecutionResult,  # build, compile, run, seed, snapshot, test
-        RunOperationResultsArtifact,  # run-operation
+        RunExecutionResult,  # build, compile, run, seed, snapshot, test, run-operation
     ] = None
 
 
 # Programmatic invocation
 class dbtRunner:
     def __init__(
         self,
@@ -73,14 +71,15 @@
 
     def invoke(self, args: List[str], **kwargs) -> dbtRunnerResult:
         try:
             dbt_ctx = cli.make_context(cli.name, args)
             dbt_ctx.obj = {
                 "manifest": self.manifest,
                 "callbacks": self.callbacks,
+                "_publications": kwargs.get("publications"),
             }
 
             for key, value in kwargs.items():
                 dbt_ctx.params[key] = value
                 # Hack to set parameter source to custom string
                 dbt_ctx.set_parameter_source(key, "kwargs")  # type: ignore
 
@@ -209,14 +208,15 @@
 # dbt clean
 @cli.command("clean")
 @click.pass_context
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.target
+@p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.unset_profile
 @requires.project
 def clean(ctx, **kwargs):
     """Delete all folders in the clean-targets list (usually the dbt_packages and target directories.)"""
@@ -280,14 +280,15 @@
 @click.pass_context
 @p.browser
 @p.port
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.target
+@p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 def docs_serve(ctx, **kwargs):
@@ -473,14 +474,15 @@
 @p.project_dir
 @p.resource_type
 @p.raw_select
 @p.selector
 @p.state
 @p.deprecated_state
 @p.target
+@p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
@@ -573,14 +575,15 @@
 @click.pass_context
 @click.argument("macro")
 @p.args
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.target
+@p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
@@ -687,14 +690,15 @@
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.state
 @p.deprecated_state
 @p.target
+@p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
```

### Comparing `dbt-core-1.6.0b1/dbt/cli/option_types.py` & `dbt-core-1.6.0b2/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/cli/options.py` & `dbt-core-1.6.0b2/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/cli/params.py` & `dbt-core-1.6.0b2/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/cli/requires.py` & `dbt-core-1.6.0b2/dbt/cli/requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,17 @@
 
             runtime_config = ctx.obj["runtime_config"]
             register_adapter(runtime_config)
 
             # a manifest has already been set on the context, so don't overwrite it
             if ctx.obj.get("manifest") is None:
                 manifest = ManifestLoader.get_full_manifest(
-                    runtime_config, write_perf_info=write_perf_info
+                    runtime_config,
+                    write_perf_info=write_perf_info,
+                    publications=ctx.obj.get("_publications"),
                 )
 
                 ctx.obj["manifest"] = manifest
                 if write and ctx.obj["flags"].write_json:
                     write_manifest(manifest, ctx.obj["runtime_config"].target_path)
 
             return func(*args, **kwargs)
```

### Comparing `dbt-core-1.6.0b1/dbt/cli/resolvers.py` & `dbt-core-1.6.0b2/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0b2/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/agate_helper.py` & `dbt-core-1.6.0b2/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/git.py` & `dbt-core-1.6.0b2/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/jinja.py` & `dbt-core-1.6.0b2/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/jinja_static.py` & `dbt-core-1.6.0b2/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/registry.py` & `dbt-core-1.6.0b2/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/clients/system.py` & `dbt-core-1.6.0b2/dbt/clients/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         func(path)
     else:
         raise
 
 
 def resolve_path_from_base(path_to_resolve: str, base_path: str) -> str:
     """
-    If path-to_resolve is a relative path, create an absolute path
+    If path_to_resolve is a relative path, create an absolute path
     with base_path as the base.
 
     If path_to_resolve is an absolute path or a user path (~), just
     resolve it to an absolute path and return.
     """
     return os.path.abspath(os.path.join(base_path, os.path.expanduser(path_to_resolve)))
```

### Comparing `dbt-core-1.6.0b1/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0b2/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/compilation.py` & `dbt-core-1.6.0b2/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/config/profile.py` & `dbt-core-1.6.0b2/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/config/project.py` & `dbt-core-1.6.0b2/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/config/renderer.py` & `dbt-core-1.6.0b2/dbt/config/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, Any, Tuple, Optional, Union, Callable
 import re
 import os
+from datetime import date
 
 from dbt.clients.jinja import get_rendered, catch_jinja
 from dbt.constants import SECRET_ENV_PREFIX
 from dbt.context.target import TargetContext
 from dbt.context.secret import SecretContext, SECRET_PLACEHOLDER
 from dbt.context.base import BaseContext
 from dbt.contracts.connection import HasCredentials
@@ -29,18 +30,18 @@
     def render_entry(self, value: Any, keypath: Keypath) -> Any:
         if not self.should_render_keypath(keypath):
             return value
 
         return self.render_value(value, keypath)
 
     def render_value(self, value: Any, keypath: Optional[Keypath] = None) -> Any:
-        # keypath is ignored.
-        # if it wasn't read as a string, ignore it
+        # keypath is ignored (and someone who knows should explain why here)
         if not isinstance(value, str):
-            return value
+            return value if not isinstance(value, date) else value.isoformat()
+
         try:
             with catch_jinja():
                 return get_rendered(value, self.context, native=True)
         except CompilationError as exc:
             msg = f"Could not render {value}: {exc.msg}"
             raise CompilationError(msg) from exc
 
@@ -178,15 +179,25 @@
     def name(self):
         return "Secret"
 
     def render_value(self, value: Any, keypath: Optional[Keypath] = None) -> Any:
         # First, standard Jinja rendering, with special handling for 'secret' environment variables
         # "{{ env_var('DBT_SECRET_ENV_VAR') }}" -> "$$$DBT_SECRET_START$$$DBT_SECRET_ENV_{VARIABLE_NAME}$$$DBT_SECRET_END$$$"
         # This prevents Jinja manipulation of secrets via macros/filters that might leak partial/modified values in logs
-        rendered = super().render_value(value, keypath)
+
+        try:
+            rendered = super().render_value(value, keypath)
+        except Exception as ex:
+            if keypath and "password" in keypath:
+                # Passwords sometimes contain jinja-esque characters, but we
+                # don't want to render them if they aren't valid jinja.
+                rendered = value
+            else:
+                raise ex
+
         # Now, detect instances of the placeholder value ($$$DBT_SECRET_START...DBT_SECRET_END$$$)
         # and replace them with the actual secret value
         if SECRET_ENV_PREFIX in str(rendered):
             search_group = f"({SECRET_ENV_PREFIX}(.*))"
             pattern = SECRET_PLACEHOLDER.format(search_group).replace("$", r"\$")
             m = re.search(
                 pattern,
```

### Comparing `dbt-core-1.6.0b1/dbt/config/runtime.py` & `dbt-core-1.6.0b2/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/config/selectors.py` & `dbt-core-1.6.0b2/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/config/utils.py` & `dbt-core-1.6.0b2/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/base.py` & `dbt-core-1.6.0b2/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/configured.py` & `dbt-core-1.6.0b2/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/context_config.py` & `dbt-core-1.6.0b2/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/docs.py` & `dbt-core-1.6.0b2/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0b2/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/macro_resolver.py` & `dbt-core-1.6.0b2/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/macros.py` & `dbt-core-1.6.0b2/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/manifest.py` & `dbt-core-1.6.0b2/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/providers.py` & `dbt-core-1.6.0b2/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/secret.py` & `dbt-core-1.6.0b2/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/context/target.py` & `dbt-core-1.6.0b2/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/connection.py` & `dbt-core-1.6.0b2/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/files.py` & `dbt-core-1.6.0b2/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Group,
     UnpatchedSourceDefinition,
     ManifestNode,
     GraphMemberNode,
     ResultNode,
     BaseNode,
     ManifestOrPublicNode,
+    ModelNode,
 )
 from dbt.contracts.graph.unparsed import SourcePatch, NodeVersion, UnparsedVersion
 from dbt.contracts.graph.manifest_upgrade import upgrade_manifest_json
 from dbt.contracts.files import SourceFile, SchemaSourceFile, FileHash, AnySourceFile
 from dbt.contracts.util import BaseArtifactMetadata, SourceKey, ArtifactMixin, schema_version
 from dbt.dataclass_schema import dbtClassMixin
 from dbt.exceptions import (
@@ -184,15 +185,21 @@
     ):
         unique_id = self.get_unique_id(key, package, version, source_node)
         if unique_id is not None:
             node = self.perform_lookup(unique_id, manifest)
             # If this is an unpinned ref (no 'version' arg was passed),
             # AND this is a versioned node,
             # AND this ref is being resolved at runtime -- get_node_info != {}
-            if version is None and node.is_versioned and get_node_info():
+            # Only ModelNodes can be versioned.
+            if (
+                isinstance(node, ModelNode)
+                and version is None
+                and node.is_versioned
+                and get_node_info()
+            ):
                 # Check to see if newer versions are available, and log an "FYI" if so
                 max_version: UnparsedVersion = max(
                     [
                         UnparsedVersion(v.version)
                         for v in manifest.nodes.values()
                         if v.name == node.name and v.version is not None
                     ]
@@ -954,14 +961,31 @@
 
     @property
     def analysis_lookup(self) -> AnalysisLookup:
         if self._analysis_lookup is None:
             self._analysis_lookup = AnalysisLookup(self)
         return self._analysis_lookup
 
+    def resolve_refs(
+        self, source_node: GraphMemberNode, current_project: str
+    ) -> List[MaybeNonSource]:
+        resolved_refs: List[MaybeNonSource] = []
+        for ref in source_node.refs:
+            resolved = self.resolve_ref(
+                source_node,
+                ref.name,
+                ref.package,
+                ref.version,
+                current_project,
+                source_node.package_name,
+            )
+            resolved_refs.append(resolved)
+
+        return resolved_refs
+
     # Called by dbt.parser.manifest._process_refs_for_exposure, _process_refs_for_metric,
     # and dbt.parser.manifest._process_refs_for_node
     def resolve_ref(
         self,
         source_node: GraphMemberNode,
         target_model_name: str,
         target_model_package: Optional[str],
@@ -1312,14 +1336,16 @@
             data = upgrade_manifest_json(data)
         return cls.from_dict(data)
 
     def __post_serialize__(self, dct):
         for unique_id, node in dct["nodes"].items():
             if "config_call_dict" in node:
                 del node["config_call_dict"]
+            if "state_relation" in node:
+                del node["state_relation"]
         return dct
 
 
 def get_manifest_schema_version(dct: dict) -> int:
     schema_version = dct.get("metadata", {}).get("dbt_schema_version", None)
     if not schema_version:
         raise ValueError("Manifest doesn't have schema version")
```

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from datetime import datetime
 import time
 from dataclasses import dataclass, field
 from enum import Enum
 import hashlib
 
 from mashumaro.types import SerializableType
 from typing import (
@@ -36,21 +37,20 @@
     NodeVersion,
     UnparsedSourceDefinition,
     UnparsedSourceTableDefinition,
     UnparsedColumn,
 )
 from dbt.contracts.util import Replaceable, AdditionalPropertiesMixin
 from dbt.events.functions import warn_or_error
-from dbt.exceptions import ParsingError, InvalidAccessTypeError, ContractBreakingChangeError
+from dbt.exceptions import ParsingError, ContractBreakingChangeError
 from dbt.events.types import (
     SeedIncreased,
     SeedExceedsLimitSamePath,
     SeedExceedsLimitAndPathChanged,
     SeedExceedsLimitChecksumChanged,
-    ValidationWarning,
 )
 from dbt.events.contextvars import set_contextvars
 from dbt.flags import get_flags
 from dbt.node_types import ModelLanguage, NodeType, AccessType
 
 from .model_config import (
     NodeConfig,
@@ -267,14 +267,25 @@
 
     def add_public_node(self, value: str):
         if value not in self.public_nodes:
             self.public_nodes.append(value)
 
 
 @dataclass
+class StateRelation(dbtClassMixin):
+    alias: str
+    database: Optional[str]
+    schema: str
+
+    @property
+    def identifier(self):
+        return self.alias
+
+
+@dataclass
 class ParsedNodeMandatory(GraphNode, HasRelationMetadata, Replaceable):
     alias: str
     checksum: FileHash
     config: NodeConfig = field(default_factory=NodeConfig)
 
     @property
     def identifier(self):
@@ -439,71 +450,14 @@
     def build_contract_checksum(self):
         pass
 
     def same_contract(self, old, adapter_type=None) -> bool:
         # This would only apply to seeds
         return True
 
-    def patch(self, patch: "ParsedNodePatch"):
-        """Given a ParsedNodePatch, add the new information to the node."""
-        # NOTE: Constraint patching is awkwardly done in the parse_patch function
-        # which calls this one. We need to combine the logic.
-
-        # explicitly pick out the parts to update so we don't inadvertently
-        # step on the model name or anything
-        # Note: config should already be updated
-        self.patch_path: Optional[str] = patch.file_id
-        # update created_at so process_docs will run in partial parsing
-        self.created_at = time.time()
-        self.description = patch.description
-        self.columns = patch.columns
-        self.name = patch.name
-
-        # TODO: version, latest_version, and access are specific to ModelNodes, consider splitting out to ModelNode
-        if self.resource_type != NodeType.Model:
-            if patch.version:
-                warn_or_error(
-                    ValidationWarning(
-                        field_name="version",
-                        resource_type=self.resource_type.value,
-                        node_name=patch.name,
-                    )
-                )
-            if patch.latest_version:
-                warn_or_error(
-                    ValidationWarning(
-                        field_name="latest_version",
-                        resource_type=self.resource_type.value,
-                        node_name=patch.name,
-                    )
-                )
-        self.version = patch.version
-        self.latest_version = patch.latest_version
-
-        # This might not be the ideal place to validate the "access" field,
-        # but at this point we have the information we need to properly
-        # validate and we don't before this.
-        if patch.access:
-            if self.resource_type == NodeType.Model:
-                if AccessType.is_valid(patch.access):
-                    self.access = AccessType(patch.access)
-                else:
-                    raise InvalidAccessTypeError(
-                        unique_id=self.unique_id,
-                        field_value=patch.access,
-                    )
-            else:
-                warn_or_error(
-                    ValidationWarning(
-                        field_name="access",
-                        resource_type=self.resource_type.value,
-                        node_name=patch.name,
-                    )
-                )
-
     def same_contents(self, old, adapter_type) -> bool:
         if old is None:
             return False
 
         # Need to ensure that same_contract is called because it
         # could throw an error
         same_contract = self.same_contract(old, adapter_type)
@@ -611,14 +565,16 @@
 @dataclass
 class ModelNode(CompiledNode):
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Model]})
     access: AccessType = AccessType.Protected
     constraints: List[ModelLevelConstraint] = field(default_factory=list)
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
+    deprecation_date: Optional[datetime] = None
+    state_relation: Optional[StateRelation] = None
 
     @property
     def is_latest_version(self) -> bool:
         return self.version is not None and self.version == self.latest_version
 
     @property
     def search_name(self):
@@ -793,14 +749,15 @@
 class SeedNode(ParsedNode):  # No SQLDefaults!
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Seed]})
     config: SeedConfig = field(default_factory=SeedConfig)
     # seeds need the root_path because the contents are not loaded initially
     # and we need the root_path to load the seed later
     root_path: Optional[str] = None
     depends_on: MacroDependsOn = field(default_factory=MacroDependsOn)
+    state_relation: Optional[StateRelation] = None
 
     def same_seeds(self, other: "SeedNode") -> bool:
         # for seeds, we check the hashes. If the hashes are different types,
         # no match. If the hashes are both the same 'path', log a warning and
         # assume they are the same
         # if the current checksum is a path, we want to log a warning.
         result = self.checksum == other.checksum
@@ -991,14 +948,15 @@
     config: EmptySnapshotConfig = field(default_factory=EmptySnapshotConfig)
 
 
 @dataclass
 class SnapshotNode(CompiledNode):
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Snapshot]})
     config: SnapshotConfig
+    state_relation: Optional[StateRelation] = None
 
 
 # ====================================
 # Macro
 # ====================================
 
 
@@ -1011,22 +969,14 @@
     meta: Dict[str, Any] = field(default_factory=dict)
     docs: Docs = field(default_factory=Docs)
     patch_path: Optional[str] = None
     arguments: List[MacroArgument] = field(default_factory=list)
     created_at: float = field(default_factory=lambda: time.time())
     supported_languages: Optional[List[ModelLanguage]] = None
 
-    def patch(self, patch: "ParsedMacroPatch"):
-        self.patch_path: Optional[str] = patch.file_id
-        self.description = patch.description
-        self.created_at = time.time()
-        self.meta = patch.meta
-        self.docs = patch.docs
-        self.arguments = patch.arguments
-
     def same_contents(self, other: Optional["Macro"]) -> bool:
         if other is None:
             return False
         # the only thing that makes one macro different from another with the
         # same name/package is its content
         return self.macro_sql == other.macro_sql
 
@@ -1462,14 +1412,16 @@
 # may be empty.
 @dataclass
 class ParsedNodePatch(ParsedPatch):
     columns: Dict[str, ColumnInfo]
     access: Optional[str]
     version: Optional[NodeVersion]
     latest_version: Optional[NodeVersion]
+    constraints: List[Dict[str, Any]]
+    deprecation_date: Optional[datetime]
 
 
 @dataclass
 class ParsedMacroPatch(ParsedPatch):
     arguments: List[MacroArgument] = field(default_factory=list)
```

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/unparsed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import re
 
 from dbt import deprecations
 from dbt.node_types import NodeType
 from dbt.contracts.util import (
     AdditionalPropertiesMixin,
     Mergeable,
@@ -150,14 +151,15 @@
     config: Dict[str, Any] = field(default_factory=dict)
     constraints: List[Dict[str, Any]] = field(default_factory=list)
     docs: Docs = field(default_factory=Docs)
     tests: Optional[List[TestDef]] = None
     columns: Sequence[Union[dbt.helper_types.IncludeExclude, UnparsedColumn]] = field(
         default_factory=list
     )
+    deprecation_date: Optional[datetime.datetime] = None
 
     def __lt__(self, other):
         try:
             v = type(other.v)(self.v)
             return v < other.v
         except ValueError:
             try:
@@ -188,14 +190,16 @@
                     self._include_exclude = column
                     has_include_exclude = True
                 else:
                     raise ParsingError("version can have at most one include/exclude element")
             else:
                 self._unparsed_columns.append(column)
 
+        self.deprecation_date = normalize_date(self.deprecation_date)
+
 
 @dataclass
 class UnparsedAnalysisUpdate(HasConfig, HasColumnDocs, HasColumnProps, HasYamlMetadata):
     access: Optional[str] = None
 
 
 @dataclass
@@ -206,14 +210,15 @@
 
 @dataclass
 class UnparsedModelUpdate(UnparsedNodeUpdate):
     quote_columns: Optional[bool] = None
     access: Optional[str] = None
     latest_version: Optional[NodeVersion] = None
     versions: Sequence[UnparsedVersion] = field(default_factory=list)
+    deprecation_date: Optional[datetime.datetime] = None
 
     def __post_init__(self):
         if self.latest_version:
             version_values = [version.v for version in self.versions]
             if self.latest_version not in version_values:
                 raise ParsingError(
                     f"latest_version: {self.latest_version} is not one of model '{self.name}' versions: {version_values} "
@@ -225,14 +230,16 @@
                 raise ParsingError(
                     f"Found duplicate version: '{version.v}' in versions list of model '{self.name}'"
                 )
             seen_versions.add(str(version.v))
 
         self._version_map = {version.v: version for version in self.versions}
 
+        self.deprecation_date = normalize_date(self.deprecation_date)
+
     def get_columns_for_version(self, version: NodeVersion) -> List[UnparsedColumn]:
         if version not in self._version_map:
             raise DbtInternalError(
                 f"get_columns_for_version called for version '{version}' not in version map"
             )
 
         version_columns = []
@@ -648,7 +655,22 @@
     owner: Owner
 
     @classmethod
     def validate(cls, data):
         super(UnparsedGroup, cls).validate(data)
         if data["owner"].get("name") is None and data["owner"].get("email") is None:
             raise ValidationError("Group owner must have at least one of 'name' or 'email'.")
+
+
+def normalize_date(d: Optional[datetime.date]) -> Optional[datetime.datetime]:
+    """Convert date to datetime (at midnight), and add local time zone if naive"""
+    if d is None:
+        return None
+
+    # convert date to datetime
+    dt = d if type(d) == datetime.datetime else datetime.datetime(d.year, d.month, d.day)
+
+    if not dt.tzinfo:
+        # date is naive, re-interpret as system time zone
+        dt = dt.astimezone()
+
+    return dt
```

### Comparing `dbt-core-1.6.0b1/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0b2/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/project.py` & `dbt-core-1.6.0b2/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/publication.py` & `dbt-core-1.6.0b2/dbt/contracts/publication.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     schema: Optional[str] = None
     identifier: Optional[str] = None
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
     # list of model unique_ids
     public_node_dependencies: List[str] = field(default_factory=list)
     generated_at: datetime = field(default_factory=datetime.utcnow)
+    deprecation_date: Optional[datetime] = None
 
     @property
     def is_latest_version(self) -> bool:
         return self.version is not None and self.version == self.latest_version
 
     # Needed for ref resolution code
     @property
@@ -110,7 +111,16 @@
     the internal manifest. The public_nodes are stored separately in the manifest,
     and just the unique_ids of the public models are stored here."""
 
     metadata: PublicationMetadata = field(default_factory=PublicationMetadata)
     # list of project name strings
     dependencies: List[str] = field(default_factory=list)
     public_node_ids: List[str] = field(default_factory=list)
+
+    @classmethod
+    def from_publication(cls, publication: PublicationArtifact):
+        return cls(
+            project_name=publication.project_name,
+            metadata=publication.metadata,
+            dependencies=publication.dependencies,
+            public_node_ids=list(publication.public_models.keys()),
+        )
```

### Comparing `dbt-core-1.6.0b1/dbt/contracts/relation.py` & `dbt-core-1.6.0b2/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/results.py` & `dbt-core-1.6.0b2/dbt/contracts/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,48 +243,14 @@
         )
         return cls(metadata=meta, results=processed_results, elapsed_time=elapsed_time, args=args)
 
     def write(self, path: str):
         write_json(path, self.to_dict(omit_none=False))
 
 
-@dataclass
-class RunOperationResult(ExecutionResult):
-    success: bool
-
-
-@dataclass
-class RunOperationResultMetadata(BaseArtifactMetadata):
-    dbt_schema_version: str = field(
-        default_factory=lambda: str(RunOperationResultsArtifact.dbt_schema_version)
-    )
-
-
-@dataclass
-@schema_version("run-operation-result", 1)
-class RunOperationResultsArtifact(RunOperationResult, ArtifactMixin):
-    @classmethod
-    def from_success(
-        cls,
-        success: bool,
-        elapsed_time: float,
-        generated_at: datetime,
-    ):
-        meta = RunOperationResultMetadata(
-            dbt_schema_version=str(cls.dbt_schema_version),
-            generated_at=generated_at,
-        )
-        return cls(
-            metadata=meta,
-            results=[],
-            elapsed_time=elapsed_time,
-            success=success,
-        )
-
-
 # due to issues with typing.Union collapsing subclasses, this can't subclass
 # PartialResult
 
 
 @dataclass
 class SourceFreshnessResult(NodeResult):
     node: SourceDefinition
```

### Comparing `dbt-core-1.6.0b1/dbt/contracts/selection.py` & `dbt-core-1.6.0b2/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/sql.py` & `dbt-core-1.6.0b2/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/state.py` & `dbt-core-1.6.0b2/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/contracts/util.py` & `dbt-core-1.6.0b2/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/dataclass_schema.py` & `dbt-core-1.6.0b2/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deprecations.py` & `dbt-core-1.6.0b2/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/base.py` & `dbt-core-1.6.0b2/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/git.py` & `dbt-core-1.6.0b2/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/local.py` & `dbt-core-1.6.0b2/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/registry.py` & `dbt-core-1.6.0b2/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/resolver.py` & `dbt-core-1.6.0b2/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/deps/tarball.py` & `dbt-core-1.6.0b2/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0b2/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/docs/source/conf.py` & `dbt-core-1.6.0b2/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0b2/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/base_types.py` & `dbt-core-1.6.0b2/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/contextvars.py` & `dbt-core-1.6.0b2/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/eventmgr.py` & `dbt-core-1.6.0b2/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/format.py` & `dbt-core-1.6.0b2/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/functions.py` & `dbt-core-1.6.0b2/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/helpers.py` & `dbt-core-1.6.0b2/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/events/types.py` & `dbt-core-1.6.0b2/dbt/events/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # | Code |     Description     |
 # |:----:|:-------------------:|
 # | A    | Pre-project loading |
 # | D    | Deprecations        |
 # | E    | DB adapter          |
 # | I    | Project parsing     |
 # | M    | Deps generation     |
+# | P    | Artifacts           |
 # | Q    | Node execution      |
 # | W    | Node testing        |
 # | Z    | Misc                |
 # | T    | Test only           |
 #
 # The basic idea is that event codes roughly translate to the natural order of running a dbt task
 
@@ -1142,14 +1143,70 @@
             f"When that happens, this reference will resolve to {self.ref_node_name}.v{self.ref_max_version} instead.\n\n"
             f"  Try out v{self.ref_max_version}: {{{{ ref('{self.ref_node_package}', '{self.ref_node_name}', v='{self.ref_max_version}') }}}}\n"
             f"  Pin to  v{self.ref_node_version}: {{{{ ref('{self.ref_node_package}', '{self.ref_node_name}', v='{self.ref_node_version}') }}}}\n"
         )
         return msg
 
 
+class DeprecatedModel(WarnLevel):
+    def code(self):
+        return "I065"
+
+    def message(self) -> str:
+        version = ".v" + self.model_version if self.model_version else ""
+        return (
+            f"Model {self.model_name}{version} has passed its deprecation date of {self.deprecation_date}. "
+            "This model should be disabled or removed."
+        )
+
+
+class UpcomingReferenceDeprecation(WarnLevel):
+    def code(self):
+        return "I066"
+
+    def message(self) -> str:
+        ref_model_version = ".v" + self.ref_model_version if self.ref_model_version else ""
+        msg = (
+            f"While compiling '{self.model_name}': Found a reference to {self.ref_model_name}{ref_model_version}, "
+            f"which is slated for deprecation on '{self.ref_model_deprecation_date}'. "
+        )
+
+        if self.ref_model_version and self.ref_model_version != self.ref_model_latest_version:
+            coda = (
+                f"A new version of '{self.ref_model_name}' is available. Try it out: "
+                f"{{{{ ref('{self.ref_model_package}', '{self.ref_model_name}', "
+                f"v='{self.ref_model_latest_version}') }}}}."
+            )
+            msg = msg + coda
+
+        return msg
+
+
+class DeprecatedReference(WarnLevel):
+    def code(self):
+        return "I067"
+
+    def message(self) -> str:
+        ref_model_version = ".v" + self.ref_model_version if self.ref_model_version else ""
+        msg = (
+            f"While compiling '{self.model_name}': Found a reference to {self.ref_model_name}{ref_model_version}, "
+            f"which was deprecated on '{self.ref_model_deprecation_date}'. "
+        )
+
+        if self.ref_model_version and self.ref_model_version != self.ref_model_latest_version:
+            coda = (
+                f"A new version of '{self.ref_model_name}' is available. Migrate now: "
+                f"{{{{ ref('{self.ref_model_package}', '{self.ref_model_name}', "
+                f"v='{self.ref_model_latest_version}') }}}}."
+            )
+            msg = msg + coda
+
+        return msg
+
+
 # =======================================================
 # M - Deps generation
 # =======================================================
 
 
 class GitSparseCheckoutSubdirectory(DebugLevel):
     def code(self):
@@ -1394,14 +1451,27 @@
 
 
 # =======================================================
 # Q - Node execution
 # =======================================================
 
 
+class PublicationArtifactAvailable(DebugLevel):
+    def code(self):
+        return "P001"
+
+    def message(self) -> str:
+        return "Publication artifact available"
+
+
+# =======================================================
+# Q - Node execution
+# =======================================================
+
+
 class RunningOperationCaughtError(ErrorLevel):
     def code(self):
         return "Q001"
 
     def message(self) -> str:
         return f"Encountered an error while running operation: {self.exc}"
```

### Comparing `dbt-core-1.6.0b1/dbt/events/types_pb2.py` & `dbt-core-1.6.0b2/dbt/events/types_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x86\x01\n\"CollectFreshnessReturnSignatureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"t\n\x1aPublicationArtifactChanged\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x1dPublicationArtifactChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PublicationArtifactChanged\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x86\x01\n\"CollectFreshnessReturnSignatureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"t\n\x1aPublicationArtifactChanged\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x1dPublicationArtifactChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PublicationArtifactChanged\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"f\n\x12\x44\x65precatedModelMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x80\x01\n\x1fUpcomingReferenceDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"n\n\x16\x44\x65precatedReferenceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"M\n\x1cPublicationArtifactAvailable\x12-\n\x0cpub_artifact\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x80\x01\n\x1fPublicationArtifactAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.PublicationArtifactAvailable\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EVENTINFO_EXTRAENTRY._options = None
@@ -440,440 +440,456 @@
   _JINJALOGDEBUG._serialized_end=18813
   _JINJALOGDEBUGMSG._serialized_start=18815
   _JINJALOGDEBUGMSG._serialized_end=18913
   _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_start=18916
   _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_end=19090
   _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_start=19093
   _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_end=19225
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=19227
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=19274
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=19277
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=19407
-  _GITPROGRESSCHECKOUTREVISION._serialized_start=19409
-  _GITPROGRESSCHECKOUTREVISION._serialized_end=19456
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=19458
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=19584
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=19586
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=19638
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=19641
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=19787
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=19789
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=19835
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=19838
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=19972
-  _GITNOTHINGTODO._serialized_start=19974
-  _GITNOTHINGTODO._serialized_end=20003
-  _GITNOTHINGTODOMSG._serialized_start=20005
-  _GITNOTHINGTODOMSG._serialized_end=20105
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=20107
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=20176
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=20179
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=20313
-  _GITPROGRESSCHECKEDOUTAT._serialized_start=20315
-  _GITPROGRESSCHECKEDOUTAT._serialized_end=20357
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=20359
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=20477
-  _REGISTRYPROGRESSGETREQUEST._serialized_start=20479
-  _REGISTRYPROGRESSGETREQUEST._serialized_end=20520
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=20522
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=20646
-  _REGISTRYPROGRESSGETRESPONSE._serialized_start=20648
-  _REGISTRYPROGRESSGETRESPONSE._serialized_end=20709
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=20711
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=20837
-  _SELECTORREPORTINVALIDSELECTOR._serialized_start=20839
-  _SELECTORREPORTINVALIDSELECTOR._serialized_end=20934
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=20937
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=21067
-  _DEPSNOPACKAGESFOUND._serialized_start=21069
-  _DEPSNOPACKAGESFOUND._serialized_end=21090
-  _DEPSNOPACKAGESFOUNDMSG._serialized_start=21092
-  _DEPSNOPACKAGESFOUNDMSG._serialized_end=21202
-  _DEPSSTARTPACKAGEINSTALL._serialized_start=21204
-  _DEPSSTARTPACKAGEINSTALL._serialized_end=21251
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=21253
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=21371
-  _DEPSINSTALLINFO._serialized_start=21373
-  _DEPSINSTALLINFO._serialized_end=21412
-  _DEPSINSTALLINFOMSG._serialized_start=21414
-  _DEPSINSTALLINFOMSG._serialized_end=21516
-  _DEPSUPDATEAVAILABLE._serialized_start=21518
-  _DEPSUPDATEAVAILABLE._serialized_end=21563
-  _DEPSUPDATEAVAILABLEMSG._serialized_start=21565
-  _DEPSUPDATEAVAILABLEMSG._serialized_end=21675
-  _DEPSUPTODATE._serialized_start=21677
-  _DEPSUPTODATE._serialized_end=21691
-  _DEPSUPTODATEMSG._serialized_start=21693
-  _DEPSUPTODATEMSG._serialized_end=21789
-  _DEPSLISTSUBDIRECTORY._serialized_start=21791
-  _DEPSLISTSUBDIRECTORY._serialized_end=21835
-  _DEPSLISTSUBDIRECTORYMSG._serialized_start=21837
-  _DEPSLISTSUBDIRECTORYMSG._serialized_end=21949
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=21951
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=21997
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=21999
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=22123
-  _RETRYEXTERNALCALL._serialized_start=22125
-  _RETRYEXTERNALCALL._serialized_end=22174
-  _RETRYEXTERNALCALLMSG._serialized_start=22176
-  _RETRYEXTERNALCALLMSG._serialized_end=22282
-  _RECORDRETRYEXCEPTION._serialized_start=22284
-  _RECORDRETRYEXCEPTION._serialized_end=22319
-  _RECORDRETRYEXCEPTIONMSG._serialized_start=22321
-  _RECORDRETRYEXCEPTIONMSG._serialized_end=22433
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=22435
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=22481
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=22484
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=22618
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=22620
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=22686
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=22689
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=22825
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=22827
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=22877
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=22880
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=23012
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=23014
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=23064
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=23067
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=23199
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=23201
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=23254
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=23257
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=23395
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=23397
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=23448
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=23451
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=23585
-  _DEPSSETDOWNLOADDIRECTORY._serialized_start=23587
-  _DEPSSETDOWNLOADDIRECTORY._serialized_end=23627
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=23629
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=23749
-  _DEPSUNPINNED._serialized_start=23751
-  _DEPSUNPINNED._serialized_end=23796
-  _DEPSUNPINNEDMSG._serialized_start=23798
-  _DEPSUNPINNEDMSG._serialized_end=23894
-  _NONODESFORSELECTIONCRITERIA._serialized_start=23896
-  _NONODESFORSELECTIONCRITERIA._serialized_end=23943
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=23945
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=24071
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=24073
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=24115
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=24117
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=24243
-  _COMPILECOMPLETE._serialized_start=24245
-  _COMPILECOMPLETE._serialized_end=24262
-  _COMPILECOMPLETEMSG._serialized_start=24264
-  _COMPILECOMPLETEMSG._serialized_end=24366
-  _FRESHNESSCHECKCOMPLETE._serialized_start=24368
-  _FRESHNESSCHECKCOMPLETE._serialized_end=24392
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=24394
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=24510
-  _SEEDHEADER._serialized_start=24512
-  _SEEDHEADER._serialized_end=24540
-  _SEEDHEADERMSG._serialized_start=24542
-  _SEEDHEADERMSG._serialized_end=24634
-  _SQLRUNNEREXCEPTION._serialized_start=24636
-  _SQLRUNNEREXCEPTION._serialized_end=24687
-  _SQLRUNNEREXCEPTIONMSG._serialized_start=24689
-  _SQLRUNNEREXCEPTIONMSG._serialized_end=24797
-  _LOGTESTRESULT._serialized_start=24800
-  _LOGTESTRESULT._serialized_end=24968
-  _LOGTESTRESULTMSG._serialized_start=24970
-  _LOGTESTRESULTMSG._serialized_end=25068
-  _LOGSTARTLINE._serialized_start=25070
-  _LOGSTARTLINE._serialized_end=25177
-  _LOGSTARTLINEMSG._serialized_start=25179
-  _LOGSTARTLINEMSG._serialized_end=25275
-  _LOGMODELRESULT._serialized_start=25278
-  _LOGMODELRESULT._serialized_end=25427
-  _LOGMODELRESULTMSG._serialized_start=25429
-  _LOGMODELRESULTMSG._serialized_end=25529
-  _LOGSNAPSHOTRESULT._serialized_start=25532
-  _LOGSNAPSHOTRESULT._serialized_end=25782
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=25740
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=25782
-  _LOGSNAPSHOTRESULTMSG._serialized_start=25784
-  _LOGSNAPSHOTRESULTMSG._serialized_end=25890
-  _LOGSEEDRESULT._serialized_start=25893
-  _LOGSEEDRESULT._serialized_end=26078
-  _LOGSEEDRESULTMSG._serialized_start=26080
-  _LOGSEEDRESULTMSG._serialized_end=26178
-  _LOGFRESHNESSRESULT._serialized_start=26181
-  _LOGFRESHNESSRESULT._serialized_end=26354
-  _LOGFRESHNESSRESULTMSG._serialized_start=26356
-  _LOGFRESHNESSRESULTMSG._serialized_end=26464
-  _LOGCANCELLINE._serialized_start=26466
-  _LOGCANCELLINE._serialized_end=26500
-  _LOGCANCELLINEMSG._serialized_start=26502
-  _LOGCANCELLINEMSG._serialized_end=26600
-  _DEFAULTSELECTOR._serialized_start=26602
-  _DEFAULTSELECTOR._serialized_end=26633
-  _DEFAULTSELECTORMSG._serialized_start=26635
-  _DEFAULTSELECTORMSG._serialized_end=26737
-  _NODESTART._serialized_start=26739
-  _NODESTART._serialized_end=26792
-  _NODESTARTMSG._serialized_start=26794
-  _NODESTARTMSG._serialized_end=26884
-  _NODEFINISHED._serialized_start=26886
-  _NODEFINISHED._serialized_end=26989
-  _NODEFINISHEDMSG._serialized_start=26991
-  _NODEFINISHEDMSG._serialized_end=27087
-  _QUERYCANCELATIONUNSUPPORTED._serialized_start=27089
-  _QUERYCANCELATIONUNSUPPORTED._serialized_end=27132
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=27134
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=27260
-  _CONCURRENCYLINE._serialized_start=27262
-  _CONCURRENCYLINE._serialized_end=27341
-  _CONCURRENCYLINEMSG._serialized_start=27343
-  _CONCURRENCYLINEMSG._serialized_end=27445
-  _WRITINGINJECTEDSQLFORNODE._serialized_start=27447
-  _WRITINGINJECTEDSQLFORNODE._serialized_end=27516
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=27518
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=27640
-  _NODECOMPILING._serialized_start=27642
-  _NODECOMPILING._serialized_end=27699
-  _NODECOMPILINGMSG._serialized_start=27701
-  _NODECOMPILINGMSG._serialized_end=27799
-  _NODEEXECUTING._serialized_start=27801
-  _NODEEXECUTING._serialized_end=27858
-  _NODEEXECUTINGMSG._serialized_start=27860
-  _NODEEXECUTINGMSG._serialized_end=27958
-  _LOGHOOKSTARTLINE._serialized_start=27960
-  _LOGHOOKSTARTLINE._serialized_end=28069
-  _LOGHOOKSTARTLINEMSG._serialized_start=28071
-  _LOGHOOKSTARTLINEMSG._serialized_end=28175
-  _LOGHOOKENDLINE._serialized_start=28178
-  _LOGHOOKENDLINE._serialized_end=28325
-  _LOGHOOKENDLINEMSG._serialized_start=28327
-  _LOGHOOKENDLINEMSG._serialized_end=28427
-  _SKIPPINGDETAILS._serialized_start=28430
-  _SKIPPINGDETAILS._serialized_end=28577
-  _SKIPPINGDETAILSMSG._serialized_start=28579
-  _SKIPPINGDETAILSMSG._serialized_end=28681
-  _NOTHINGTODO._serialized_start=28683
-  _NOTHINGTODO._serialized_end=28696
-  _NOTHINGTODOMSG._serialized_start=28698
-  _NOTHINGTODOMSG._serialized_end=28792
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=28794
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=28838
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=28841
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=28971
-  _ENDRUNRESULT._serialized_start=28974
-  _ENDRUNRESULT._serialized_end=29121
-  _ENDRUNRESULTMSG._serialized_start=29123
-  _ENDRUNRESULTMSG._serialized_end=29219
-  _NONODESSELECTED._serialized_start=29221
-  _NONODESSELECTED._serialized_end=29238
-  _NONODESSELECTEDMSG._serialized_start=29240
-  _NONODESSELECTEDMSG._serialized_end=29342
-  _COMMANDCOMPLETED._serialized_start=29344
-  _COMMANDCOMPLETED._serialized_end=29463
-  _COMMANDCOMPLETEDMSG._serialized_start=29465
-  _COMMANDCOMPLETEDMSG._serialized_end=29569
-  _SHOWNODE._serialized_start=29571
-  _SHOWNODE._serialized_end=29678
-  _SHOWNODEMSG._serialized_start=29680
-  _SHOWNODEMSG._serialized_end=29768
-  _COMPILEDNODE._serialized_start=29770
-  _COMPILEDNODE._serialized_end=29882
-  _COMPILEDNODEMSG._serialized_start=29884
-  _COMPILEDNODEMSG._serialized_end=29980
-  _CATCHABLEEXCEPTIONONRUN._serialized_start=29982
-  _CATCHABLEEXCEPTIONONRUN._serialized_end=30080
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=30082
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=30200
-  _INTERNALERRORONRUN._serialized_start=30202
-  _INTERNALERRORONRUN._serialized_end=30255
-  _INTERNALERRORONRUNMSG._serialized_start=30257
-  _INTERNALERRORONRUNMSG._serialized_end=30365
-  _GENERICEXCEPTIONONRUN._serialized_start=30367
-  _GENERICEXCEPTIONONRUN._serialized_end=30442
-  _GENERICEXCEPTIONONRUNMSG._serialized_start=30444
-  _GENERICEXCEPTIONONRUNMSG._serialized_end=30558
-  _NODECONNECTIONRELEASEERROR._serialized_start=30560
-  _NODECONNECTIONRELEASEERROR._serialized_end=30638
-  _NODECONNECTIONRELEASEERRORMSG._serialized_start=30640
-  _NODECONNECTIONRELEASEERRORMSG._serialized_end=30764
-  _FOUNDSTATS._serialized_start=30766
-  _FOUNDSTATS._serialized_end=30797
-  _FOUNDSTATSMSG._serialized_start=30799
-  _FOUNDSTATSMSG._serialized_end=30891
-  _MAINKEYBOARDINTERRUPT._serialized_start=30893
-  _MAINKEYBOARDINTERRUPT._serialized_end=30916
-  _MAINKEYBOARDINTERRUPTMSG._serialized_start=30918
-  _MAINKEYBOARDINTERRUPTMSG._serialized_end=31032
-  _MAINENCOUNTEREDERROR._serialized_start=31034
-  _MAINENCOUNTEREDERROR._serialized_end=31069
-  _MAINENCOUNTEREDERRORMSG._serialized_start=31071
-  _MAINENCOUNTEREDERRORMSG._serialized_end=31183
-  _MAINSTACKTRACE._serialized_start=31185
-  _MAINSTACKTRACE._serialized_end=31222
-  _MAINSTACKTRACEMSG._serialized_start=31224
-  _MAINSTACKTRACEMSG._serialized_end=31324
-  _SYSTEMCOULDNOTWRITE._serialized_start=31326
-  _SYSTEMCOULDNOTWRITE._serialized_end=31390
-  _SYSTEMCOULDNOTWRITEMSG._serialized_start=31392
-  _SYSTEMCOULDNOTWRITEMSG._serialized_end=31502
-  _SYSTEMEXECUTINGCMD._serialized_start=31504
-  _SYSTEMEXECUTINGCMD._serialized_end=31537
-  _SYSTEMEXECUTINGCMDMSG._serialized_start=31539
-  _SYSTEMEXECUTINGCMDMSG._serialized_end=31647
-  _SYSTEMSTDOUT._serialized_start=31649
-  _SYSTEMSTDOUT._serialized_end=31677
-  _SYSTEMSTDOUTMSG._serialized_start=31679
-  _SYSTEMSTDOUTMSG._serialized_end=31775
-  _SYSTEMSTDERR._serialized_start=31777
-  _SYSTEMSTDERR._serialized_end=31805
-  _SYSTEMSTDERRMSG._serialized_start=31807
-  _SYSTEMSTDERRMSG._serialized_end=31903
-  _SYSTEMREPORTRETURNCODE._serialized_start=31905
-  _SYSTEMREPORTRETURNCODE._serialized_end=31949
-  _SYSTEMREPORTRETURNCODEMSG._serialized_start=31951
-  _SYSTEMREPORTRETURNCODEMSG._serialized_end=32067
-  _TIMINGINFOCOLLECTED._serialized_start=32069
-  _TIMINGINFOCOLLECTED._serialized_end=32181
-  _TIMINGINFOCOLLECTEDMSG._serialized_start=32183
-  _TIMINGINFOCOLLECTEDMSG._serialized_end=32293
-  _LOGDEBUGSTACKTRACE._serialized_start=32295
-  _LOGDEBUGSTACKTRACE._serialized_end=32333
-  _LOGDEBUGSTACKTRACEMSG._serialized_start=32335
-  _LOGDEBUGSTACKTRACEMSG._serialized_end=32443
-  _CHECKCLEANPATH._serialized_start=32445
-  _CHECKCLEANPATH._serialized_end=32475
-  _CHECKCLEANPATHMSG._serialized_start=32477
-  _CHECKCLEANPATHMSG._serialized_end=32577
-  _CONFIRMCLEANPATH._serialized_start=32579
-  _CONFIRMCLEANPATH._serialized_end=32611
-  _CONFIRMCLEANPATHMSG._serialized_start=32613
-  _CONFIRMCLEANPATHMSG._serialized_end=32717
-  _PROTECTEDCLEANPATH._serialized_start=32719
-  _PROTECTEDCLEANPATH._serialized_end=32753
-  _PROTECTEDCLEANPATHMSG._serialized_start=32755
-  _PROTECTEDCLEANPATHMSG._serialized_end=32863
-  _FINISHEDCLEANPATHS._serialized_start=32865
-  _FINISHEDCLEANPATHS._serialized_end=32885
-  _FINISHEDCLEANPATHSMSG._serialized_start=32887
-  _FINISHEDCLEANPATHSMSG._serialized_end=32995
-  _OPENCOMMAND._serialized_start=32997
-  _OPENCOMMAND._serialized_end=33050
-  _OPENCOMMANDMSG._serialized_start=33052
-  _OPENCOMMANDMSG._serialized_end=33146
-  _FORMATTING._serialized_start=33148
-  _FORMATTING._serialized_end=33173
-  _FORMATTINGMSG._serialized_start=33175
-  _FORMATTINGMSG._serialized_end=33267
-  _SERVINGDOCSPORT._serialized_start=33269
-  _SERVINGDOCSPORT._serialized_end=33317
-  _SERVINGDOCSPORTMSG._serialized_start=33319
-  _SERVINGDOCSPORTMSG._serialized_end=33421
-  _SERVINGDOCSACCESSINFO._serialized_start=33423
-  _SERVINGDOCSACCESSINFO._serialized_end=33460
-  _SERVINGDOCSACCESSINFOMSG._serialized_start=33462
-  _SERVINGDOCSACCESSINFOMSG._serialized_end=33576
-  _SERVINGDOCSEXITINFO._serialized_start=33578
-  _SERVINGDOCSEXITINFO._serialized_end=33599
-  _SERVINGDOCSEXITINFOMSG._serialized_start=33601
-  _SERVINGDOCSEXITINFOMSG._serialized_end=33711
-  _RUNRESULTWARNING._serialized_start=33713
-  _RUNRESULTWARNING._serialized_end=33787
-  _RUNRESULTWARNINGMSG._serialized_start=33789
-  _RUNRESULTWARNINGMSG._serialized_end=33893
-  _RUNRESULTFAILURE._serialized_start=33895
-  _RUNRESULTFAILURE._serialized_end=33969
-  _RUNRESULTFAILUREMSG._serialized_start=33971
-  _RUNRESULTFAILUREMSG._serialized_end=34075
-  _STATSLINE._serialized_start=34077
-  _STATSLINE._serialized_end=34184
-  _STATSLINE_STATSENTRY._serialized_start=34140
-  _STATSLINE_STATSENTRY._serialized_end=34184
-  _STATSLINEMSG._serialized_start=34186
-  _STATSLINEMSG._serialized_end=34276
-  _RUNRESULTERROR._serialized_start=34278
-  _RUNRESULTERROR._serialized_end=34307
-  _RUNRESULTERRORMSG._serialized_start=34309
-  _RUNRESULTERRORMSG._serialized_end=34409
-  _RUNRESULTERRORNOMESSAGE._serialized_start=34411
-  _RUNRESULTERRORNOMESSAGE._serialized_end=34452
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=34454
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=34572
-  _SQLCOMPILEDPATH._serialized_start=34574
-  _SQLCOMPILEDPATH._serialized_end=34605
-  _SQLCOMPILEDPATHMSG._serialized_start=34607
-  _SQLCOMPILEDPATHMSG._serialized_end=34709
-  _CHECKNODETESTFAILURE._serialized_start=34711
-  _CHECKNODETESTFAILURE._serialized_end=34756
-  _CHECKNODETESTFAILUREMSG._serialized_start=34758
-  _CHECKNODETESTFAILUREMSG._serialized_end=34870
-  _FIRSTRUNRESULTERROR._serialized_start=34872
-  _FIRSTRUNRESULTERROR._serialized_end=34906
-  _FIRSTRUNRESULTERRORMSG._serialized_start=34908
-  _FIRSTRUNRESULTERRORMSG._serialized_end=35018
-  _AFTERFIRSTRUNRESULTERROR._serialized_start=35020
-  _AFTERFIRSTRUNRESULTERROR._serialized_end=35059
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=35061
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=35181
-  _ENDOFRUNSUMMARY._serialized_start=35183
-  _ENDOFRUNSUMMARY._serialized_end=35270
-  _ENDOFRUNSUMMARYMSG._serialized_start=35272
-  _ENDOFRUNSUMMARYMSG._serialized_end=35374
-  _LOGSKIPBECAUSEERROR._serialized_start=35376
-  _LOGSKIPBECAUSEERROR._serialized_end=35461
-  _LOGSKIPBECAUSEERRORMSG._serialized_start=35463
-  _LOGSKIPBECAUSEERRORMSG._serialized_end=35573
-  _ENSUREGITINSTALLED._serialized_start=35575
-  _ENSUREGITINSTALLED._serialized_end=35595
-  _ENSUREGITINSTALLEDMSG._serialized_start=35597
-  _ENSUREGITINSTALLEDMSG._serialized_end=35705
-  _DEPSCREATINGLOCALSYMLINK._serialized_start=35707
-  _DEPSCREATINGLOCALSYMLINK._serialized_end=35733
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=35735
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=35855
-  _DEPSSYMLINKNOTAVAILABLE._serialized_start=35857
-  _DEPSSYMLINKNOTAVAILABLE._serialized_end=35882
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=35884
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=36002
-  _DISABLETRACKING._serialized_start=36004
-  _DISABLETRACKING._serialized_end=36021
-  _DISABLETRACKINGMSG._serialized_start=36023
-  _DISABLETRACKINGMSG._serialized_end=36125
-  _SENDINGEVENT._serialized_start=36127
-  _SENDINGEVENT._serialized_end=36157
-  _SENDINGEVENTMSG._serialized_start=36159
-  _SENDINGEVENTMSG._serialized_end=36255
-  _SENDEVENTFAILURE._serialized_start=36257
-  _SENDEVENTFAILURE._serialized_end=36275
-  _SENDEVENTFAILUREMSG._serialized_start=36277
-  _SENDEVENTFAILUREMSG._serialized_end=36381
-  _FLUSHEVENTS._serialized_start=36383
-  _FLUSHEVENTS._serialized_end=36396
-  _FLUSHEVENTSMSG._serialized_start=36398
-  _FLUSHEVENTSMSG._serialized_end=36492
-  _FLUSHEVENTSFAILURE._serialized_start=36494
-  _FLUSHEVENTSFAILURE._serialized_end=36514
-  _FLUSHEVENTSFAILUREMSG._serialized_start=36516
-  _FLUSHEVENTSFAILUREMSG._serialized_end=36624
-  _TRACKINGINITIALIZEFAILURE._serialized_start=36626
-  _TRACKINGINITIALIZEFAILURE._serialized_end=36671
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=36673
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=36795
-  _RUNRESULTWARNINGMESSAGE._serialized_start=36797
-  _RUNRESULTWARNINGMESSAGE._serialized_end=36835
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=36837
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=36955
-  _DEBUGCMDOUT._serialized_start=36957
-  _DEBUGCMDOUT._serialized_end=36983
-  _DEBUGCMDOUTMSG._serialized_start=36985
-  _DEBUGCMDOUTMSG._serialized_end=37079
-  _DEBUGCMDRESULT._serialized_start=37081
-  _DEBUGCMDRESULT._serialized_end=37110
-  _DEBUGCMDRESULTMSG._serialized_start=37112
-  _DEBUGCMDRESULTMSG._serialized_end=37212
-  _LISTCMDOUT._serialized_start=37214
-  _LISTCMDOUT._serialized_end=37239
-  _LISTCMDOUTMSG._serialized_start=37241
-  _LISTCMDOUTMSG._serialized_end=37333
-  _NOTE._serialized_start=37335
-  _NOTE._serialized_end=37354
-  _NOTEMSG._serialized_start=37356
-  _NOTEMSG._serialized_end=37436
+  _DEPRECATEDMODEL._serialized_start=19227
+  _DEPRECATEDMODEL._serialized_end=19313
+  _DEPRECATEDMODELMSG._serialized_start=19315
+  _DEPRECATEDMODELMSG._serialized_end=19417
+  _UPCOMINGREFERENCEDEPRECATION._serialized_start=19420
+  _UPCOMINGREFERENCEDEPRECATION._serialized_end=19618
+  _UPCOMINGREFERENCEDEPRECATIONMSG._serialized_start=19621
+  _UPCOMINGREFERENCEDEPRECATIONMSG._serialized_end=19749
+  _DEPRECATEDREFERENCE._serialized_start=19752
+  _DEPRECATEDREFERENCE._serialized_end=19941
+  _DEPRECATEDREFERENCEMSG._serialized_start=19943
+  _DEPRECATEDREFERENCEMSG._serialized_end=20053
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=20055
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=20102
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=20105
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=20235
+  _GITPROGRESSCHECKOUTREVISION._serialized_start=20237
+  _GITPROGRESSCHECKOUTREVISION._serialized_end=20284
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=20286
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=20412
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=20414
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=20466
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=20469
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=20615
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=20617
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=20663
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=20666
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=20800
+  _GITNOTHINGTODO._serialized_start=20802
+  _GITNOTHINGTODO._serialized_end=20831
+  _GITNOTHINGTODOMSG._serialized_start=20833
+  _GITNOTHINGTODOMSG._serialized_end=20933
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=20935
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=21004
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=21007
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=21141
+  _GITPROGRESSCHECKEDOUTAT._serialized_start=21143
+  _GITPROGRESSCHECKEDOUTAT._serialized_end=21185
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=21187
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=21305
+  _REGISTRYPROGRESSGETREQUEST._serialized_start=21307
+  _REGISTRYPROGRESSGETREQUEST._serialized_end=21348
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=21350
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=21474
+  _REGISTRYPROGRESSGETRESPONSE._serialized_start=21476
+  _REGISTRYPROGRESSGETRESPONSE._serialized_end=21537
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=21539
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=21665
+  _SELECTORREPORTINVALIDSELECTOR._serialized_start=21667
+  _SELECTORREPORTINVALIDSELECTOR._serialized_end=21762
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=21765
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=21895
+  _DEPSNOPACKAGESFOUND._serialized_start=21897
+  _DEPSNOPACKAGESFOUND._serialized_end=21918
+  _DEPSNOPACKAGESFOUNDMSG._serialized_start=21920
+  _DEPSNOPACKAGESFOUNDMSG._serialized_end=22030
+  _DEPSSTARTPACKAGEINSTALL._serialized_start=22032
+  _DEPSSTARTPACKAGEINSTALL._serialized_end=22079
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=22081
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=22199
+  _DEPSINSTALLINFO._serialized_start=22201
+  _DEPSINSTALLINFO._serialized_end=22240
+  _DEPSINSTALLINFOMSG._serialized_start=22242
+  _DEPSINSTALLINFOMSG._serialized_end=22344
+  _DEPSUPDATEAVAILABLE._serialized_start=22346
+  _DEPSUPDATEAVAILABLE._serialized_end=22391
+  _DEPSUPDATEAVAILABLEMSG._serialized_start=22393
+  _DEPSUPDATEAVAILABLEMSG._serialized_end=22503
+  _DEPSUPTODATE._serialized_start=22505
+  _DEPSUPTODATE._serialized_end=22519
+  _DEPSUPTODATEMSG._serialized_start=22521
+  _DEPSUPTODATEMSG._serialized_end=22617
+  _DEPSLISTSUBDIRECTORY._serialized_start=22619
+  _DEPSLISTSUBDIRECTORY._serialized_end=22663
+  _DEPSLISTSUBDIRECTORYMSG._serialized_start=22665
+  _DEPSLISTSUBDIRECTORYMSG._serialized_end=22777
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=22779
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=22825
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=22827
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=22951
+  _RETRYEXTERNALCALL._serialized_start=22953
+  _RETRYEXTERNALCALL._serialized_end=23002
+  _RETRYEXTERNALCALLMSG._serialized_start=23004
+  _RETRYEXTERNALCALLMSG._serialized_end=23110
+  _RECORDRETRYEXCEPTION._serialized_start=23112
+  _RECORDRETRYEXCEPTION._serialized_end=23147
+  _RECORDRETRYEXCEPTIONMSG._serialized_start=23149
+  _RECORDRETRYEXCEPTIONMSG._serialized_end=23261
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=23263
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=23309
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=23312
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=23446
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=23448
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=23514
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=23517
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=23653
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=23655
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=23705
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=23708
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=23840
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=23842
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=23892
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=23895
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=24027
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=24029
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=24082
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=24085
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=24223
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=24225
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=24276
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=24279
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=24413
+  _DEPSSETDOWNLOADDIRECTORY._serialized_start=24415
+  _DEPSSETDOWNLOADDIRECTORY._serialized_end=24455
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=24457
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=24577
+  _DEPSUNPINNED._serialized_start=24579
+  _DEPSUNPINNED._serialized_end=24624
+  _DEPSUNPINNEDMSG._serialized_start=24626
+  _DEPSUNPINNEDMSG._serialized_end=24722
+  _NONODESFORSELECTIONCRITERIA._serialized_start=24724
+  _NONODESFORSELECTIONCRITERIA._serialized_end=24771
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=24773
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=24899
+  _PUBLICATIONARTIFACTAVAILABLE._serialized_start=24901
+  _PUBLICATIONARTIFACTAVAILABLE._serialized_end=24978
+  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_start=24981
+  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_end=25109
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=25111
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=25153
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=25155
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=25281
+  _COMPILECOMPLETE._serialized_start=25283
+  _COMPILECOMPLETE._serialized_end=25300
+  _COMPILECOMPLETEMSG._serialized_start=25302
+  _COMPILECOMPLETEMSG._serialized_end=25404
+  _FRESHNESSCHECKCOMPLETE._serialized_start=25406
+  _FRESHNESSCHECKCOMPLETE._serialized_end=25430
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=25432
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=25548
+  _SEEDHEADER._serialized_start=25550
+  _SEEDHEADER._serialized_end=25578
+  _SEEDHEADERMSG._serialized_start=25580
+  _SEEDHEADERMSG._serialized_end=25672
+  _SQLRUNNEREXCEPTION._serialized_start=25674
+  _SQLRUNNEREXCEPTION._serialized_end=25725
+  _SQLRUNNEREXCEPTIONMSG._serialized_start=25727
+  _SQLRUNNEREXCEPTIONMSG._serialized_end=25835
+  _LOGTESTRESULT._serialized_start=25838
+  _LOGTESTRESULT._serialized_end=26006
+  _LOGTESTRESULTMSG._serialized_start=26008
+  _LOGTESTRESULTMSG._serialized_end=26106
+  _LOGSTARTLINE._serialized_start=26108
+  _LOGSTARTLINE._serialized_end=26215
+  _LOGSTARTLINEMSG._serialized_start=26217
+  _LOGSTARTLINEMSG._serialized_end=26313
+  _LOGMODELRESULT._serialized_start=26316
+  _LOGMODELRESULT._serialized_end=26465
+  _LOGMODELRESULTMSG._serialized_start=26467
+  _LOGMODELRESULTMSG._serialized_end=26567
+  _LOGSNAPSHOTRESULT._serialized_start=26570
+  _LOGSNAPSHOTRESULT._serialized_end=26820
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=26778
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=26820
+  _LOGSNAPSHOTRESULTMSG._serialized_start=26822
+  _LOGSNAPSHOTRESULTMSG._serialized_end=26928
+  _LOGSEEDRESULT._serialized_start=26931
+  _LOGSEEDRESULT._serialized_end=27116
+  _LOGSEEDRESULTMSG._serialized_start=27118
+  _LOGSEEDRESULTMSG._serialized_end=27216
+  _LOGFRESHNESSRESULT._serialized_start=27219
+  _LOGFRESHNESSRESULT._serialized_end=27392
+  _LOGFRESHNESSRESULTMSG._serialized_start=27394
+  _LOGFRESHNESSRESULTMSG._serialized_end=27502
+  _LOGCANCELLINE._serialized_start=27504
+  _LOGCANCELLINE._serialized_end=27538
+  _LOGCANCELLINEMSG._serialized_start=27540
+  _LOGCANCELLINEMSG._serialized_end=27638
+  _DEFAULTSELECTOR._serialized_start=27640
+  _DEFAULTSELECTOR._serialized_end=27671
+  _DEFAULTSELECTORMSG._serialized_start=27673
+  _DEFAULTSELECTORMSG._serialized_end=27775
+  _NODESTART._serialized_start=27777
+  _NODESTART._serialized_end=27830
+  _NODESTARTMSG._serialized_start=27832
+  _NODESTARTMSG._serialized_end=27922
+  _NODEFINISHED._serialized_start=27924
+  _NODEFINISHED._serialized_end=28027
+  _NODEFINISHEDMSG._serialized_start=28029
+  _NODEFINISHEDMSG._serialized_end=28125
+  _QUERYCANCELATIONUNSUPPORTED._serialized_start=28127
+  _QUERYCANCELATIONUNSUPPORTED._serialized_end=28170
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=28172
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=28298
+  _CONCURRENCYLINE._serialized_start=28300
+  _CONCURRENCYLINE._serialized_end=28379
+  _CONCURRENCYLINEMSG._serialized_start=28381
+  _CONCURRENCYLINEMSG._serialized_end=28483
+  _WRITINGINJECTEDSQLFORNODE._serialized_start=28485
+  _WRITINGINJECTEDSQLFORNODE._serialized_end=28554
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=28556
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=28678
+  _NODECOMPILING._serialized_start=28680
+  _NODECOMPILING._serialized_end=28737
+  _NODECOMPILINGMSG._serialized_start=28739
+  _NODECOMPILINGMSG._serialized_end=28837
+  _NODEEXECUTING._serialized_start=28839
+  _NODEEXECUTING._serialized_end=28896
+  _NODEEXECUTINGMSG._serialized_start=28898
+  _NODEEXECUTINGMSG._serialized_end=28996
+  _LOGHOOKSTARTLINE._serialized_start=28998
+  _LOGHOOKSTARTLINE._serialized_end=29107
+  _LOGHOOKSTARTLINEMSG._serialized_start=29109
+  _LOGHOOKSTARTLINEMSG._serialized_end=29213
+  _LOGHOOKENDLINE._serialized_start=29216
+  _LOGHOOKENDLINE._serialized_end=29363
+  _LOGHOOKENDLINEMSG._serialized_start=29365
+  _LOGHOOKENDLINEMSG._serialized_end=29465
+  _SKIPPINGDETAILS._serialized_start=29468
+  _SKIPPINGDETAILS._serialized_end=29615
+  _SKIPPINGDETAILSMSG._serialized_start=29617
+  _SKIPPINGDETAILSMSG._serialized_end=29719
+  _NOTHINGTODO._serialized_start=29721
+  _NOTHINGTODO._serialized_end=29734
+  _NOTHINGTODOMSG._serialized_start=29736
+  _NOTHINGTODOMSG._serialized_end=29830
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=29832
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=29876
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=29879
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=30009
+  _ENDRUNRESULT._serialized_start=30012
+  _ENDRUNRESULT._serialized_end=30159
+  _ENDRUNRESULTMSG._serialized_start=30161
+  _ENDRUNRESULTMSG._serialized_end=30257
+  _NONODESSELECTED._serialized_start=30259
+  _NONODESSELECTED._serialized_end=30276
+  _NONODESSELECTEDMSG._serialized_start=30278
+  _NONODESSELECTEDMSG._serialized_end=30380
+  _COMMANDCOMPLETED._serialized_start=30382
+  _COMMANDCOMPLETED._serialized_end=30501
+  _COMMANDCOMPLETEDMSG._serialized_start=30503
+  _COMMANDCOMPLETEDMSG._serialized_end=30607
+  _SHOWNODE._serialized_start=30609
+  _SHOWNODE._serialized_end=30716
+  _SHOWNODEMSG._serialized_start=30718
+  _SHOWNODEMSG._serialized_end=30806
+  _COMPILEDNODE._serialized_start=30808
+  _COMPILEDNODE._serialized_end=30920
+  _COMPILEDNODEMSG._serialized_start=30922
+  _COMPILEDNODEMSG._serialized_end=31018
+  _CATCHABLEEXCEPTIONONRUN._serialized_start=31020
+  _CATCHABLEEXCEPTIONONRUN._serialized_end=31118
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=31120
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=31238
+  _INTERNALERRORONRUN._serialized_start=31240
+  _INTERNALERRORONRUN._serialized_end=31293
+  _INTERNALERRORONRUNMSG._serialized_start=31295
+  _INTERNALERRORONRUNMSG._serialized_end=31403
+  _GENERICEXCEPTIONONRUN._serialized_start=31405
+  _GENERICEXCEPTIONONRUN._serialized_end=31480
+  _GENERICEXCEPTIONONRUNMSG._serialized_start=31482
+  _GENERICEXCEPTIONONRUNMSG._serialized_end=31596
+  _NODECONNECTIONRELEASEERROR._serialized_start=31598
+  _NODECONNECTIONRELEASEERROR._serialized_end=31676
+  _NODECONNECTIONRELEASEERRORMSG._serialized_start=31678
+  _NODECONNECTIONRELEASEERRORMSG._serialized_end=31802
+  _FOUNDSTATS._serialized_start=31804
+  _FOUNDSTATS._serialized_end=31835
+  _FOUNDSTATSMSG._serialized_start=31837
+  _FOUNDSTATSMSG._serialized_end=31929
+  _MAINKEYBOARDINTERRUPT._serialized_start=31931
+  _MAINKEYBOARDINTERRUPT._serialized_end=31954
+  _MAINKEYBOARDINTERRUPTMSG._serialized_start=31956
+  _MAINKEYBOARDINTERRUPTMSG._serialized_end=32070
+  _MAINENCOUNTEREDERROR._serialized_start=32072
+  _MAINENCOUNTEREDERROR._serialized_end=32107
+  _MAINENCOUNTEREDERRORMSG._serialized_start=32109
+  _MAINENCOUNTEREDERRORMSG._serialized_end=32221
+  _MAINSTACKTRACE._serialized_start=32223
+  _MAINSTACKTRACE._serialized_end=32260
+  _MAINSTACKTRACEMSG._serialized_start=32262
+  _MAINSTACKTRACEMSG._serialized_end=32362
+  _SYSTEMCOULDNOTWRITE._serialized_start=32364
+  _SYSTEMCOULDNOTWRITE._serialized_end=32428
+  _SYSTEMCOULDNOTWRITEMSG._serialized_start=32430
+  _SYSTEMCOULDNOTWRITEMSG._serialized_end=32540
+  _SYSTEMEXECUTINGCMD._serialized_start=32542
+  _SYSTEMEXECUTINGCMD._serialized_end=32575
+  _SYSTEMEXECUTINGCMDMSG._serialized_start=32577
+  _SYSTEMEXECUTINGCMDMSG._serialized_end=32685
+  _SYSTEMSTDOUT._serialized_start=32687
+  _SYSTEMSTDOUT._serialized_end=32715
+  _SYSTEMSTDOUTMSG._serialized_start=32717
+  _SYSTEMSTDOUTMSG._serialized_end=32813
+  _SYSTEMSTDERR._serialized_start=32815
+  _SYSTEMSTDERR._serialized_end=32843
+  _SYSTEMSTDERRMSG._serialized_start=32845
+  _SYSTEMSTDERRMSG._serialized_end=32941
+  _SYSTEMREPORTRETURNCODE._serialized_start=32943
+  _SYSTEMREPORTRETURNCODE._serialized_end=32987
+  _SYSTEMREPORTRETURNCODEMSG._serialized_start=32989
+  _SYSTEMREPORTRETURNCODEMSG._serialized_end=33105
+  _TIMINGINFOCOLLECTED._serialized_start=33107
+  _TIMINGINFOCOLLECTED._serialized_end=33219
+  _TIMINGINFOCOLLECTEDMSG._serialized_start=33221
+  _TIMINGINFOCOLLECTEDMSG._serialized_end=33331
+  _LOGDEBUGSTACKTRACE._serialized_start=33333
+  _LOGDEBUGSTACKTRACE._serialized_end=33371
+  _LOGDEBUGSTACKTRACEMSG._serialized_start=33373
+  _LOGDEBUGSTACKTRACEMSG._serialized_end=33481
+  _CHECKCLEANPATH._serialized_start=33483
+  _CHECKCLEANPATH._serialized_end=33513
+  _CHECKCLEANPATHMSG._serialized_start=33515
+  _CHECKCLEANPATHMSG._serialized_end=33615
+  _CONFIRMCLEANPATH._serialized_start=33617
+  _CONFIRMCLEANPATH._serialized_end=33649
+  _CONFIRMCLEANPATHMSG._serialized_start=33651
+  _CONFIRMCLEANPATHMSG._serialized_end=33755
+  _PROTECTEDCLEANPATH._serialized_start=33757
+  _PROTECTEDCLEANPATH._serialized_end=33791
+  _PROTECTEDCLEANPATHMSG._serialized_start=33793
+  _PROTECTEDCLEANPATHMSG._serialized_end=33901
+  _FINISHEDCLEANPATHS._serialized_start=33903
+  _FINISHEDCLEANPATHS._serialized_end=33923
+  _FINISHEDCLEANPATHSMSG._serialized_start=33925
+  _FINISHEDCLEANPATHSMSG._serialized_end=34033
+  _OPENCOMMAND._serialized_start=34035
+  _OPENCOMMAND._serialized_end=34088
+  _OPENCOMMANDMSG._serialized_start=34090
+  _OPENCOMMANDMSG._serialized_end=34184
+  _FORMATTING._serialized_start=34186
+  _FORMATTING._serialized_end=34211
+  _FORMATTINGMSG._serialized_start=34213
+  _FORMATTINGMSG._serialized_end=34305
+  _SERVINGDOCSPORT._serialized_start=34307
+  _SERVINGDOCSPORT._serialized_end=34355
+  _SERVINGDOCSPORTMSG._serialized_start=34357
+  _SERVINGDOCSPORTMSG._serialized_end=34459
+  _SERVINGDOCSACCESSINFO._serialized_start=34461
+  _SERVINGDOCSACCESSINFO._serialized_end=34498
+  _SERVINGDOCSACCESSINFOMSG._serialized_start=34500
+  _SERVINGDOCSACCESSINFOMSG._serialized_end=34614
+  _SERVINGDOCSEXITINFO._serialized_start=34616
+  _SERVINGDOCSEXITINFO._serialized_end=34637
+  _SERVINGDOCSEXITINFOMSG._serialized_start=34639
+  _SERVINGDOCSEXITINFOMSG._serialized_end=34749
+  _RUNRESULTWARNING._serialized_start=34751
+  _RUNRESULTWARNING._serialized_end=34825
+  _RUNRESULTWARNINGMSG._serialized_start=34827
+  _RUNRESULTWARNINGMSG._serialized_end=34931
+  _RUNRESULTFAILURE._serialized_start=34933
+  _RUNRESULTFAILURE._serialized_end=35007
+  _RUNRESULTFAILUREMSG._serialized_start=35009
+  _RUNRESULTFAILUREMSG._serialized_end=35113
+  _STATSLINE._serialized_start=35115
+  _STATSLINE._serialized_end=35222
+  _STATSLINE_STATSENTRY._serialized_start=35178
+  _STATSLINE_STATSENTRY._serialized_end=35222
+  _STATSLINEMSG._serialized_start=35224
+  _STATSLINEMSG._serialized_end=35314
+  _RUNRESULTERROR._serialized_start=35316
+  _RUNRESULTERROR._serialized_end=35345
+  _RUNRESULTERRORMSG._serialized_start=35347
+  _RUNRESULTERRORMSG._serialized_end=35447
+  _RUNRESULTERRORNOMESSAGE._serialized_start=35449
+  _RUNRESULTERRORNOMESSAGE._serialized_end=35490
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=35492
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=35610
+  _SQLCOMPILEDPATH._serialized_start=35612
+  _SQLCOMPILEDPATH._serialized_end=35643
+  _SQLCOMPILEDPATHMSG._serialized_start=35645
+  _SQLCOMPILEDPATHMSG._serialized_end=35747
+  _CHECKNODETESTFAILURE._serialized_start=35749
+  _CHECKNODETESTFAILURE._serialized_end=35794
+  _CHECKNODETESTFAILUREMSG._serialized_start=35796
+  _CHECKNODETESTFAILUREMSG._serialized_end=35908
+  _FIRSTRUNRESULTERROR._serialized_start=35910
+  _FIRSTRUNRESULTERROR._serialized_end=35944
+  _FIRSTRUNRESULTERRORMSG._serialized_start=35946
+  _FIRSTRUNRESULTERRORMSG._serialized_end=36056
+  _AFTERFIRSTRUNRESULTERROR._serialized_start=36058
+  _AFTERFIRSTRUNRESULTERROR._serialized_end=36097
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=36099
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=36219
+  _ENDOFRUNSUMMARY._serialized_start=36221
+  _ENDOFRUNSUMMARY._serialized_end=36308
+  _ENDOFRUNSUMMARYMSG._serialized_start=36310
+  _ENDOFRUNSUMMARYMSG._serialized_end=36412
+  _LOGSKIPBECAUSEERROR._serialized_start=36414
+  _LOGSKIPBECAUSEERROR._serialized_end=36499
+  _LOGSKIPBECAUSEERRORMSG._serialized_start=36501
+  _LOGSKIPBECAUSEERRORMSG._serialized_end=36611
+  _ENSUREGITINSTALLED._serialized_start=36613
+  _ENSUREGITINSTALLED._serialized_end=36633
+  _ENSUREGITINSTALLEDMSG._serialized_start=36635
+  _ENSUREGITINSTALLEDMSG._serialized_end=36743
+  _DEPSCREATINGLOCALSYMLINK._serialized_start=36745
+  _DEPSCREATINGLOCALSYMLINK._serialized_end=36771
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=36773
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=36893
+  _DEPSSYMLINKNOTAVAILABLE._serialized_start=36895
+  _DEPSSYMLINKNOTAVAILABLE._serialized_end=36920
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=36922
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=37040
+  _DISABLETRACKING._serialized_start=37042
+  _DISABLETRACKING._serialized_end=37059
+  _DISABLETRACKINGMSG._serialized_start=37061
+  _DISABLETRACKINGMSG._serialized_end=37163
+  _SENDINGEVENT._serialized_start=37165
+  _SENDINGEVENT._serialized_end=37195
+  _SENDINGEVENTMSG._serialized_start=37197
+  _SENDINGEVENTMSG._serialized_end=37293
+  _SENDEVENTFAILURE._serialized_start=37295
+  _SENDEVENTFAILURE._serialized_end=37313
+  _SENDEVENTFAILUREMSG._serialized_start=37315
+  _SENDEVENTFAILUREMSG._serialized_end=37419
+  _FLUSHEVENTS._serialized_start=37421
+  _FLUSHEVENTS._serialized_end=37434
+  _FLUSHEVENTSMSG._serialized_start=37436
+  _FLUSHEVENTSMSG._serialized_end=37530
+  _FLUSHEVENTSFAILURE._serialized_start=37532
+  _FLUSHEVENTSFAILURE._serialized_end=37552
+  _FLUSHEVENTSFAILUREMSG._serialized_start=37554
+  _FLUSHEVENTSFAILUREMSG._serialized_end=37662
+  _TRACKINGINITIALIZEFAILURE._serialized_start=37664
+  _TRACKINGINITIALIZEFAILURE._serialized_end=37709
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=37711
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=37833
+  _RUNRESULTWARNINGMESSAGE._serialized_start=37835
+  _RUNRESULTWARNINGMESSAGE._serialized_end=37873
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=37875
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=37993
+  _DEBUGCMDOUT._serialized_start=37995
+  _DEBUGCMDOUT._serialized_end=38021
+  _DEBUGCMDOUTMSG._serialized_start=38023
+  _DEBUGCMDOUTMSG._serialized_end=38117
+  _DEBUGCMDRESULT._serialized_start=38119
+  _DEBUGCMDRESULT._serialized_end=38148
+  _DEBUGCMDRESULTMSG._serialized_start=38150
+  _DEBUGCMDRESULTMSG._serialized_end=38250
+  _LISTCMDOUT._serialized_start=38252
+  _LISTCMDOUT._serialized_end=38277
+  _LISTCMDOUTMSG._serialized_start=38279
+  _LISTCMDOUTMSG._serialized_end=38371
+  _NOTE._serialized_start=38373
+  _NOTE._serialized_end=38392
+  _NOTEMSG._serialized_start=38394
+  _NOTEMSG._serialized_end=38474
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt-core-1.6.0b1/dbt/exceptions.py` & `dbt-core-1.6.0b2/dbt/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,22 +404,21 @@
 class DbtProfileError(DbtConfigError):
     pass
 
 
 class PublicationConfigNotFound(DbtConfigError):
     def __init__(self, project=None, file_name=None):
         self.project = project
-        self.file_name = file_name
         msg = self.message()
         super().__init__(msg, project=project)
 
     def message(self):
         return (
             f"A dependency on project {self.project} was specified, "
-            f"but file {self.file_name} was not found."
+            f"but a publication for {self.project} was not found."
         )
 
 
 class SemverError(Exception):
     def __init__(self, msg: str = None):
         self.msg = msg
         if msg is not None:
@@ -695,14 +694,23 @@
         msg = f"""\
         Something went wrong while cloning {self.repo}
         Check the debug logs for more information
         """
         return msg
 
 
+class NoAdaptersAvailableError(DbtRuntimeError):
+    def __init__(self):
+        super().__init__(msg=self.get_message())
+
+    def get_message(self) -> str:
+        msg = "No adapters available. Learn how to install an adapter by going to https://docs.getdbt.com/docs/supported-data-platforms#adapter-installation"
+        return msg
+
+
 class BadSpecError(DbtInternalError):
     def __init__(self, repo, revision, error):
         self.repo = repo
         self.revision = revision
         self.stderr = scrub_secrets(error.stderr.strip(), env_secrets())
         super().__init__(msg=self.get_message())
```

### Comparing `dbt-core-1.6.0b1/dbt/flags.py` & `dbt-core-1.6.0b2/dbt/flags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Do not import the os package because we expose this package in jinja
 from os import getenv as os_getenv
 from argparse import Namespace
 from multiprocessing import get_context
 from typing import Optional
+from pathlib import Path
 
 
 # for setting up logger for legacy logger
 def env_set_truthy(key: str) -> Optional[str]:
     """Return the value if it was set to a "truthy" string value or None
     otherwise.
     """
@@ -91,14 +92,16 @@
 
 
 # This is used by core/dbt/context/base.py to return a flag object
 # in Jinja.
 def get_flag_obj():
     new_flags = Namespace()
     for key, val in get_flag_dict().items():
+        if isinstance(val, Path):
+            val = str(val)
         setattr(new_flags, key.upper(), val)
     # The following 3 are CLI arguments only so they're not full-fledged flags,
     # but we put in flags for users.
     setattr(new_flags, "FULL_REFRESH", getattr(GLOBAL_FLAGS, "FULL_REFRESH", None))
     setattr(new_flags, "STORE_FAILURES", getattr(GLOBAL_FLAGS, "STORE_FAILURES", None))
     setattr(new_flags, "WHICH", getattr(GLOBAL_FLAGS, "WHICH", None))
     return new_flags
```

### Comparing `dbt-core-1.6.0b1/dbt/graph/cli.py` & `dbt-core-1.6.0b2/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/graph/graph.py` & `dbt-core-1.6.0b2/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/graph/queue.py` & `dbt-core-1.6.0b2/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/graph/selector.py` & `dbt-core-1.6.0b2/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/graph/selector_methods.py` & `dbt-core-1.6.0b2/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/graph/selector_spec.py` & `dbt-core-1.6.0b2/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/helper_types.py` & `dbt-core-1.6.0b2/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/README.md` & `dbt-core-1.6.0b2/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0b2/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,14 @@
     {%- set backup_relation = base_relation.incorporate(
                                   path={"identifier": backup_identifier},
                                   type=backup_relation_type
     ) -%}
     {{ return(backup_relation) }}
 {% endmacro %}
 
-{% macro drop_relation(relation) -%}
-  {{ return(adapter.dispatch('drop_relation', 'dbt')(relation)) }}
-{% endmacro %}
-
-{% macro default__drop_relation(relation) -%}
-  {% call statement('drop_relation', auto_begin=False) -%}
-    drop {{ relation.type }} if exists {{ relation }} cascade
-  {%- endcall %}
-{% endmacro %}
-
 
 {% macro truncate_relation(relation) -%}
   {{ return(adapter.dispatch('truncate_relation', 'dbt')(relation)) }}
 {% endmacro %}
 
 {% macro default__truncate_relation(relation) -%}
   {% call statement('truncate_relation') -%}
```

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/index.html` & `dbt-core-1.6.0b2/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/starter_project/README.md` & `dbt-core-1.6.0b2/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0b2/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/internal_deprecations.py` & `dbt-core-1.6.0b2/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/logger.py` & `dbt-core-1.6.0b2/dbt/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -343,131 +343,31 @@
 
 
 # push Python warnings to debug level logs. This will suppress all import-time
 # warnings.
 DebugWarnings().__enter__()
 
 
-class DelayedFileHandler(logbook.RotatingFileHandler, FormatterMixin):
-    def __init__(
-        self,
-        log_dir: Optional[str] = None,
-        level=logbook.DEBUG,
-        filter=None,
-        bubble=True,
-        max_size=10 * 1024 * 1024,  # 10 mb
-        backup_count=5,
-    ) -> None:
-        self.disabled = False
-        self._msg_buffer: Optional[List[logbook.LogRecord]] = []
-        # if we get 1k messages without a logfile being set, something is wrong
-        self._bufmax = 1000
-        self._log_path: Optional[str] = None
-        # we need the base handler class' __init__ to run so handling works
-        logbook.Handler.__init__(self, level, filter, bubble)
-        if log_dir is not None:
-            self.set_path(log_dir)
-        self._text_format_string = None
-        self._max_size = max_size
-        self._backup_count = backup_count
-
-    def reset(self):
-        if self.initialized:
-            self.close()
-        self._log_path = None
-        self._msg_buffer = []
-        self.disabled = False
-
-    @property
-    def initialized(self):
-        return self._log_path is not None
-
-    def set_path(self, log_dir):
-        """log_dir can be the path to a log directory, or `None` to avoid
-        writing to a file (for `dbt debug`).
-        """
-        if self.disabled:
-            return
-
-        assert not self.initialized, "set_path called after being set"
-
-        if log_dir is None:
-            self.disabled = True
-            return
-
-        make_log_dir_if_missing(log_dir)
-        log_path = os.path.join(log_dir, "dbt.log.legacy")  # TODO hack for now
-        self._super_init(log_path)
-        self._replay_buffered()
-        self._log_path = log_path
-
-    def _super_init(self, log_path):
-        logbook.RotatingFileHandler.__init__(
-            self,
-            filename=log_path,
-            level=self.level,
-            filter=self.filter,
-            delay=True,
-            max_size=self._max_size,
-            backup_count=self._backup_count,
-            bubble=self.bubble,
-            format_string=DEBUG_LOG_FORMAT,
-        )
-        FormatterMixin.__init__(self, DEBUG_LOG_FORMAT)
-
-    def _replay_buffered(self):
-        assert self._msg_buffer is not None, "_msg_buffer should never be None in _replay_buffered"
-        for record in self._msg_buffer:
-            super().emit(record)
-        self._msg_buffer = None
-
-    def format(self, record: logbook.LogRecord) -> str:
-        msg = super().format(record)
-        subbed = str(msg)
-        for escape_sequence in dbt.ui.COLORS.values():
-            subbed = subbed.replace(escape_sequence, "")
-        return subbed
-
-    def emit(self, record: logbook.LogRecord):
-        """emit is not thread-safe with set_path, but it is thread-safe with
-        itself
-        """
-        if self.disabled:
-            return
-        elif self.initialized:
-            super().emit(record)
-        else:
-            assert (
-                self._msg_buffer is not None
-            ), "_msg_buffer should never be None if _log_path is set"
-            self._msg_buffer.append(record)
-            assert (
-                len(self._msg_buffer) < self._bufmax
-            ), "too many messages received before initilization!"
-
-
 class LogManager(logbook.NestedSetup):
     def __init__(self, stdout=sys.stdout, stderr=sys.stderr):
         self.stdout = stdout
         self.stderr = stderr
         self._null_handler = logbook.NullHandler()
         self._output_handler = OutputHandler(self.stdout)
-        self._file_handler = DelayedFileHandler()
         self._relevel_processor = Relevel(allowed=["dbt", "werkzeug"])
         self._state_processor = DbtProcessState("internal")
         self._scrub_processor = ScrubSecrets()
         # keep track of whether we've already entered to decide if we should
         # be actually pushing. This allows us to log in main() and also
         # support entering dbt execution via handle_and_check.
         self._stack_depth = 0
         super().__init__(
             [
                 self._null_handler,
                 self._output_handler,
-                self._file_handler,
                 self._relevel_processor,
                 self._state_processor,
                 self._scrub_processor,
             ]
         )
 
     def push_application(self):
@@ -483,14 +383,23 @@
     def disable(self):
         self.add_handler(logbook.NullHandler())
 
     def add_handler(self, handler):
         """add an handler to the log manager that runs before the file handler."""
         self.objects.append(handler)
 
+    def set_path(self, _):
+        """No-op that allows dbt-rpc to not break. See GH #7661"""
+        pass
+
+    @property
+    def initialized(self):
+        """Dummy return value for dbt-rpc. See GH#7661"""
+        return True
+
     # this is used by `dbt ls` to allow piping stdout to jq, etc
     def stderr_console(self):
         """Output to stderr at WARNING level instead of stdout"""
         self._output_handler.stream = self.stderr
         self._output_handler.level = logbook.WARNING
 
     def stdout_console(self):
@@ -498,20 +407,14 @@
         self._output_handler.stream = self.stdout
         self._output_handler.level = logbook.INFO
 
     def set_debug(self):
         self._output_handler.set_text_format(DEBUG_LOG_FORMAT)
         self._output_handler.level = logbook.DEBUG
 
-    def set_path(self, path):
-        self._file_handler.set_path(path)
-
-    def initialized(self):
-        return self._file_handler.initialized
-
     def format_json(self):
         for handler in self.objects:
             if isinstance(handler, FormatterMixin):
                 handler.format_json()
 
     def format_text(self):
         for handler in self.objects:
```

### Comparing `dbt-core-1.6.0b1/dbt/node_types.py` & `dbt-core-1.6.0b2/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/__init__.py` & `dbt-core-1.6.0b2/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/analysis.py` & `dbt-core-1.6.0b2/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/base.py` & `dbt-core-1.6.0b2/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/docs.py` & `dbt-core-1.6.0b2/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/generic_test.py` & `dbt-core-1.6.0b2/dbt/parser/generic_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def resource_type(self) -> NodeType:
         return NodeType.Macro
 
     @classmethod
     def get_compiled_path(cls, block: FileBlock):
         return block.path.relative_path
 
-    def parse_generic_test(
+    def create_generic_test_macro(
         self, block: jinja.BlockTag, base_node: UnparsedMacro, name: str
     ) -> Macro:
         unique_id = self.generate_unique_id(name)
 
         return Macro(
             path=base_node.path,
             macro_sql=block.full_block,
@@ -72,15 +72,15 @@
 
             generic_test_name = generic_test_nodes[0].name
 
             if not generic_test_name.startswith(MACRO_PREFIX):
                 continue
 
             name: str = generic_test_name.replace(MACRO_PREFIX, "")
-            node = self.parse_generic_test(block, base_node, name)
+            node = self.create_generic_test_macro(block, base_node, name)
             yield node
 
     def parse_file(self, block: FileBlock):
         assert isinstance(block.file, SourceFile)
         source_file = block.file
         assert isinstance(source_file.contents, str)
         original_file_path = source_file.path.original_file_path
```

### Comparing `dbt-core-1.6.0b1/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0b2/dbt/parser/generic_test_builders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 import re
 from copy import deepcopy
-from dataclasses import dataclass
 from typing import (
     Generic,
-    TypeVar,
     Dict,
     Any,
     Tuple,
     Optional,
     List,
 )
 
 from dbt.clients.jinja import get_rendered, GENERIC_TEST_KWARGS_NAME
 from dbt.contracts.graph.nodes import UnpatchedSourceDefinition
 from dbt.contracts.graph.unparsed import (
-    TestDef,
     NodeVersion,
-    UnparsedAnalysisUpdate,
-    UnparsedMacroUpdate,
     UnparsedNodeUpdate,
-    UnparsedExposure,
     UnparsedModelUpdate,
 )
 from dbt.exceptions import (
     CustomMacroPopulatingConfigValueError,
     SameKeyNestedError,
     TagNotStringError,
     TagsNotListOfStringsError,
     TestArgIncludesModelError,
     TestArgsNotDictError,
     TestDefinitionDictLengthError,
     TestTypeError,
     TestNameNotStringError,
     UnexpectedTestNamePatternError,
     UndefinedMacroError,
-    DbtInternalError,
 )
-from dbt.parser.search import FileBlock
+from dbt.parser.common import Testable
 from dbt.utils import md5
 
 
 def synthesize_generic_test_names(
     test_type: str, test_name: str, args: Dict[str, Any]
 ) -> Tuple[str, str]:
     # Using the type, name, and arguments to this generic test, synthesize a (hopefully) unique name
@@ -79,158 +72,14 @@
         short_name = "{}_{}".format(test_trunc_identifier, label)
     else:
         short_name = full_name
 
     return short_name, full_name
 
 
-@dataclass
-class YamlBlock(FileBlock):
-    data: Dict[str, Any]
-
-    @classmethod
-    def from_file_block(cls, src: FileBlock, data: Dict[str, Any]):
-        return cls(
-            file=src.file,
-            data=data,
-        )
-
-
-Versioned = TypeVar("Versioned", bound=UnparsedModelUpdate)
-
-Testable = TypeVar("Testable", UnparsedNodeUpdate, UnpatchedSourceDefinition, UnparsedModelUpdate)
-
-ColumnTarget = TypeVar(
-    "ColumnTarget",
-    UnparsedModelUpdate,
-    UnparsedNodeUpdate,
-    UnparsedAnalysisUpdate,
-    UnpatchedSourceDefinition,
-)
-
-Target = TypeVar(
-    "Target",
-    UnparsedNodeUpdate,
-    UnparsedMacroUpdate,
-    UnparsedAnalysisUpdate,
-    UnpatchedSourceDefinition,
-    UnparsedExposure,
-    UnparsedModelUpdate,
-)
-
-
-@dataclass
-class TargetBlock(YamlBlock, Generic[Target]):
-    target: Target
-
-    @property
-    def name(self):
-        return self.target.name
-
-    @property
-    def columns(self):
-        return []
-
-    @property
-    def tests(self) -> List[TestDef]:
-        return []
-
-    @classmethod
-    def from_yaml_block(cls, src: YamlBlock, target: Target) -> "TargetBlock[Target]":
-        return cls(
-            file=src.file,
-            data=src.data,
-            target=target,
-        )
-
-
-@dataclass
-class TargetColumnsBlock(TargetBlock[ColumnTarget], Generic[ColumnTarget]):
-    @property
-    def columns(self):
-        if self.target.columns is None:
-            return []
-        else:
-            return self.target.columns
-
-
-@dataclass
-class TestBlock(TargetColumnsBlock[Testable], Generic[Testable]):
-    @property
-    def tests(self) -> List[TestDef]:
-        if self.target.tests is None:
-            return []
-        else:
-            return self.target.tests
-
-    @property
-    def quote_columns(self) -> Optional[bool]:
-        return self.target.quote_columns
-
-    @classmethod
-    def from_yaml_block(cls, src: YamlBlock, target: Testable) -> "TestBlock[Testable]":
-        return cls(
-            file=src.file,
-            data=src.data,
-            target=target,
-        )
-
-
-@dataclass
-class VersionedTestBlock(TestBlock, Generic[Versioned]):
-    @property
-    def columns(self):
-        if not self.target.versions:
-            return super().columns
-        else:
-            raise DbtInternalError(".columns for VersionedTestBlock with versions")
-
-    @property
-    def tests(self) -> List[TestDef]:
-        if not self.target.versions:
-            return super().tests
-        else:
-            raise DbtInternalError(".tests for VersionedTestBlock with versions")
-
-    @classmethod
-    def from_yaml_block(cls, src: YamlBlock, target: Versioned) -> "VersionedTestBlock[Versioned]":
-        return cls(
-            file=src.file,
-            data=src.data,
-            target=target,
-        )
-
-
-@dataclass
-class GenericTestBlock(TestBlock[Testable], Generic[Testable]):
-    test: Dict[str, Any]
-    column_name: Optional[str]
-    tags: List[str]
-    version: Optional[NodeVersion]
-
-    @classmethod
-    def from_test_block(
-        cls,
-        src: TestBlock,
-        test: Dict[str, Any],
-        column_name: Optional[str],
-        tags: List[str],
-        version: Optional[NodeVersion],
-    ) -> "GenericTestBlock":
-        return cls(
-            file=src.file,
-            data=src.data,
-            target=src.target,
-            test=test,
-            column_name=column_name,
-            tags=tags,
-            version=version,
-        )
-
-
 class TestBuilder(Generic[Testable]):
     """An object to hold assorted test settings and perform basic parsing
 
     Test names have the following pattern:
         - the test name itself may be namespaced (package.test)
         - or it may not be namespaced (test)
```

### Comparing `dbt-core-1.6.0b1/dbt/parser/hooks.py` & `dbt-core-1.6.0b2/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/macros.py` & `dbt-core-1.6.0b2/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/manifest.py` & `dbt-core-1.6.0b2/dbt/parser/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from dataclasses import dataclass
 from dataclasses import field
-from datetime import datetime
+import datetime
 import os
 import traceback
 from typing import (
     Dict,
     Optional,
     Mapping,
     Callable,
@@ -18,14 +18,15 @@
     MutableMapping,
 )
 from itertools import chain
 import time
 from dbt.events.base_types import EventLevel
 import json
 import pprint
+import msgpack
 
 import dbt.exceptions
 import dbt.tracking
 import dbt.utils
 from dbt.flags import get_flags
 
 from dbt.adapters.factory import (
@@ -47,14 +48,18 @@
     PartialParsingNotEnabled,
     ParsedFileLoadFailed,
     InvalidDisabledTargetInTestNode,
     NodeNotFoundOrDisabled,
     StateCheckVarsHash,
     Note,
     PublicationArtifactChanged,
+    PublicationArtifactAvailable,
+    DeprecatedModel,
+    DeprecatedReference,
+    UpcomingReferenceDeprecation,
 )
 from dbt.logger import DbtProcessState
 from dbt.node_types import NodeType, AccessType
 from dbt.clients.jinja import get_rendered, MacroStack
 from dbt.clients.jinja_static import statically_extract_macro_calls
 from dbt.clients.system import (
     make_directory,
@@ -89,14 +94,15 @@
     SourceDefinition,
     Macro,
     Exposure,
     Metric,
     SeedNode,
     ManifestNode,
     ResultNode,
+    ModelNode,
 )
 from dbt.contracts.graph.unparsed import NodeVersion
 from dbt.contracts.util import Writable
 from dbt.contracts.publication import (
     PublicationConfig,
     PublicationArtifact,
     PublicationMetadata,
@@ -126,14 +132,53 @@
 
 from dbt.dataclass_schema import StrEnum, dbtClassMixin
 
 PARSING_STATE = DbtProcessState("parsing")
 PERF_INFO_FILE_NAME = "perf_info.json"
 
 
+def extended_mashumaro_encoder(data):
+    return msgpack.packb(data, default=extended_msgpack_encoder, use_bin_type=True)
+
+
+def extended_msgpack_encoder(obj):
+    if type(obj) is datetime.date:
+        date_bytes = msgpack.ExtType(1, obj.isoformat().encode())
+        return date_bytes
+    elif type(obj) is datetime.datetime:
+        datetime_bytes = msgpack.ExtType(2, obj.isoformat().encode())
+        return datetime_bytes
+
+    return obj
+
+
+def extended_mashumuro_decoder(data):
+    return msgpack.unpackb(data, ext_hook=extended_msgpack_decoder, raw=False)
+
+
+def extended_msgpack_decoder(code, data):
+    if code == 1:
+        d = datetime.date.fromisoformat(data.decode())
+        return d
+    elif code == 2:
+        dt = datetime.datetime.fromisoformat(data.decode())
+        return dt
+    else:
+        return msgpack.ExtType(code, data)
+
+
+def version_to_str(version: Optional[Union[str, int]]) -> str:
+    if isinstance(version, int):
+        return str(version)
+    elif isinstance(version, str):
+        return version
+
+    return ""
+
+
 class ReparseReason(StrEnum):
     version_mismatch = "01_version_mismatch"
     file_not_found = "02_file_not_found"
     vars_changed = "03_vars_changed"
     profile_changed = "04_profile_changed"
     deps_changed = "05_deps_changed"
     project_config_changed = "06_project_config_changed"
@@ -189,18 +234,20 @@
 class ManifestLoader:
     def __init__(
         self,
         root_project: RuntimeConfig,
         all_projects: Mapping[str, Project],
         macro_hook: Optional[Callable[[Manifest], Any]] = None,
         file_diff: Optional[FileDiff] = None,
+        publications: Optional[List[PublicationArtifact]] = None,
     ) -> None:
         self.root_project: RuntimeConfig = root_project
         self.all_projects: Mapping[str, Project] = all_projects
         self.file_diff = file_diff
+        self.publications = publications
         self.manifest: Manifest = Manifest()
         self.new_manifest = self.manifest
         self.manifest.metadata = root_project.get_metadata()
         self.macro_resolver = None  # built after macros are loaded
         self.started_at = time.time()
         # This is a MacroQueryStringSetter callable, which is called
         # later after we set the MacroManifest in the adapter. It sets
@@ -230,14 +277,15 @@
     def get_full_manifest(
         cls,
         config: RuntimeConfig,
         *,
         file_diff: Optional[FileDiff] = None,
         reset: bool = False,
         write_perf_info=False,
+        publications: Optional[List[PublicationArtifact]] = None,
     ) -> Manifest:
 
         adapter = get_adapter(config)  # type: ignore
         # reset is set in a TaskManager load_manifest call, since
         # the config and adapter may be persistent.
         if reset:
             config.clear_dependencies()
@@ -252,15 +300,21 @@
                 file_diff = FileDiff.from_dict(file_diff_dct)
 
         with PARSING_STATE:  # set up logbook.Processor for parsing
             # Start performance counting
             start_load_all = time.perf_counter()
 
             projects = config.load_dependencies()
-            loader = cls(config, projects, macro_hook=macro_hook, file_diff=file_diff)
+            loader = cls(
+                config,
+                projects,
+                macro_hook=macro_hook,
+                file_diff=file_diff,
+                publications=publications,
+            )
 
             manifest = loader.load()
 
             _check_manifest(manifest, config)
             manifest.build_flat_graph()
 
             # This needs to happen after loading from a partial parse,
@@ -453,16 +507,15 @@
 
             # We need to rebuild disabled in order to include disabled sources
             self.manifest.rebuild_disabled_lookup()
 
             # copy the selectors from the root_project to the manifest
             self.manifest.selectors = self.root_project.manifest_selectors
 
-            # load the publication artifacts and create the external nodes
-            # This also loads manifest.dependencies
+            # load manifest.dependencies and associated publication artifacts to create the external nodes
             public_nodes_changed = self.build_public_nodes()
             if public_nodes_changed:
                 self.manifest.rebuild_ref_lookup()
 
             # update the refs, sources, docs and metrics depends_on.nodes
             # These check the created_at time on the nodes to
             # determine whether they need processing.
@@ -494,20 +547,58 @@
             if public_nodes_changed:
                 self.manifest.rebuild_ref_lookup()
                 self.process_refs(self.root_project.project_name)
                 # parent and child maps will be rebuilt by write_manifest
 
         if not skip_parsing or public_nodes_changed:
             # Write out the <project_name>_publication.json file for this project
-            write_publication_artifact(self.root_project, self.manifest)
+            log_publication_artifact(self.root_project, self.manifest)
             # write out the fully parsed manifest
             self.write_manifest_for_partial_parse()
 
+        self.check_for_model_deprecations()
+
         return self.manifest
 
+    def check_for_model_deprecations(self):
+        for node in self.manifest.nodes.values():
+            if isinstance(node, ModelNode):
+                if (
+                    node.deprecation_date
+                    and node.deprecation_date < datetime.datetime.now().astimezone()
+                ):
+                    fire_event(
+                        DeprecatedModel(
+                            model_name=node.name,
+                            model_version=version_to_str(node.version),
+                            deprecation_date=node.deprecation_date.isoformat(),
+                        )
+                    )
+
+                resolved_refs = self.manifest.resolve_refs(node, self.root_project.project_name)
+                resolved_model_refs = [r for r in resolved_refs if isinstance(r, ModelNode)]
+                for resolved_ref in resolved_model_refs:
+                    if resolved_ref.deprecation_date:
+
+                        if resolved_ref.deprecation_date < datetime.datetime.now().astimezone():
+                            event_cls = DeprecatedReference
+                        else:
+                            event_cls = UpcomingReferenceDeprecation
+
+                        fire_event(
+                            event_cls(
+                                model_name=node.name,
+                                ref_model_package=resolved_ref.package_name,
+                                ref_model_name=resolved_ref.name,
+                                ref_model_version=version_to_str(resolved_ref.version),
+                                ref_model_latest_version=str(resolved_ref.latest_version),
+                                ref_model_deprecation_date=resolved_ref.deprecation_date.isoformat(),
+                            )
+                        )
+
     def load_and_parse_macros(self, project_parser_files):
         for project in self.all_projects.values():
             if project.project_name not in project_parser_files:
                 continue
             parser_files = project_parser_files[project.project_name]
             if "MacroParser" in parser_files:
                 parser = MacroParser(project, self.manifest)
@@ -645,15 +736,15 @@
             # This shouldn't be necessary, but we have gotten bug reports (#3757) of the
             # saved manifest not matching the code version.
             if self.manifest.metadata.dbt_version != __version__:
                 fire_event(
                     UnableToPartialParse(reason="saved manifest contained the wrong version")
                 )
                 self.manifest.metadata.dbt_version = __version__
-            manifest_msgpack = self.manifest.to_msgpack()
+            manifest_msgpack = self.manifest.to_msgpack(extended_mashumaro_encoder)
             make_directory(os.path.dirname(path))
             with open(path, "wb") as fp:
                 fp.write(manifest_msgpack)
         except Exception:
             raise
 
     def build_public_nodes(self) -> bool:
@@ -746,36 +837,27 @@
                 )
                 public_nodes_changed = True
 
         return public_nodes_changed
 
     def load_new_public_nodes(self):
         for project in self.manifest.project_dependencies.projects:
-            # look for a <project_name>_publication.json file for every project in the 'publications' dir
-            publication_file_name = f"{project.name}_publication.json"
-            # TODO: eventually we'll implement publications_dir config
-            path = os.path.join("publications", publication_file_name)
-            if os.path.exists(path):
-                contents = load_file_contents(path)
-                pub_dict = load_yaml_text(contents)
-                PublicationArtifact.validate(pub_dict)
-                # separate out the public_models
-                public_models = pub_dict.pop("public_models")
-                # Create the PublicationConfig to store in internal manifest
-                pub_config = PublicationConfig.from_dict(pub_dict)
-                self.manifest.publications[project.name] = pub_config
+            publication = (
+                next(p for p in self.publications if p.project_name == project.name)
+                if self.publications
+                else None
+            )
+            if publication:
+                publication_config = PublicationConfig.from_publication(publication)
+                self.manifest.publications[project.name] = publication_config
                 # Add to dictionary of public_nodes and save id in PublicationConfig
-                for public_model_dict in public_models.values():
-                    public_node = PublicModel.from_dict(public_model_dict)
+                for public_node in publication.public_models.values():
                     self.manifest.public_nodes[public_node.unique_id] = public_node
-                    pub_config.public_node_ids.append(public_node.unique_id)
             else:
-                raise PublicationConfigNotFound(
-                    project=project.name, file_name=publication_file_name
-                )
+                raise PublicationConfigNotFound(project=project.name)
 
     def is_partial_parsable(self, manifest: Manifest) -> Tuple[bool, Optional[str]]:
         """Compare the global hashes of the read-in parse results' values to
         the known ones, and return if it is ok to re-use the results.
         """
         valid = True
         reparse_reason = None
@@ -868,22 +950,22 @@
 
         reparse_reason = None
 
         if os.path.exists(path):
             try:
                 with open(path, "rb") as fp:
                     manifest_mp = fp.read()
-                manifest: Manifest = Manifest.from_msgpack(manifest_mp)  # type: ignore
+                manifest: Manifest = Manifest.from_msgpack(manifest_mp, decoder=extended_mashumuro_decoder)  # type: ignore
                 # keep this check inside the try/except in case something about
                 # the file has changed in weird ways, perhaps due to being a
                 # different version of dbt
                 is_partial_parsable, reparse_reason = self.is_partial_parsable(manifest)
                 if is_partial_parsable:
                     # We don't want to have stale generated_at dates
-                    manifest.metadata.generated_at = datetime.utcnow()
+                    manifest.metadata.generated_at = datetime.datetime.utcnow()
                     # or invocation_ids
                     manifest.metadata.invocation_id = get_invocation_id()
                     return manifest
             except Exception as exc:
                 fire_event(
                     ParsedFileLoadFailed(path=path, exc=str(exc), exc_info=traceback.format_exc())
                 )
@@ -1399,18 +1481,15 @@
                 target_package=target_model_package,
                 target_version=target_model_version,
                 disabled=(isinstance(target_model, Disabled)),
                 should_warn_if_disabled=False,
             )
 
             continue
-        elif (
-            target_model.resource_type == NodeType.Model
-            and target_model.access == AccessType.Private
-        ):
+        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
             # Exposures do not have a group and so can never reference private models
             raise dbt.exceptions.DbtReferenceError(
                 unique_id=exposure.unique_id,
                 ref_unique_id=target_model.unique_id,
                 group=dbt.utils.cast_to_str(target_model.group),
             )
 
@@ -1451,18 +1530,15 @@
                 target_kind="node",
                 target_package=target_model_package,
                 target_version=target_model_version,
                 disabled=(isinstance(target_model, Disabled)),
                 should_warn_if_disabled=False,
             )
             continue
-        elif (
-            target_model.resource_type == NodeType.Model
-            and target_model.access == AccessType.Private
-        ):
+        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
             if not metric.group or metric.group != target_model.group:
                 raise dbt.exceptions.DbtReferenceError(
                     unique_id=metric.unique_id,
                     ref_unique_id=target_model.unique_id,
                     group=dbt.utils.cast_to_str(target_model.group),
                 )
 
@@ -1558,18 +1634,15 @@
                 target_version=target_model_version,
                 disabled=(isinstance(target_model, Disabled)),
                 should_warn_if_disabled=False,
             )
             continue
 
         # Handle references to models that are private
-        elif (
-            target_model.resource_type == NodeType.Model
-            and target_model.access == AccessType.Private
-        ):
+        elif isinstance(target_model, ModelNode) and target_model.access == AccessType.Private:
             if not node.group or node.group != target_model.group:
                 raise dbt.exceptions.DbtReferenceError(
                     unique_id=node.unique_id,
                     ref_unique_id=target_model.unique_id,
                     group=dbt.utils.cast_to_str(target_model.group),
                 )
 
@@ -1681,39 +1754,40 @@
 
     _process_sources_for_node(manifest, config.project_name, node)
     _process_refs_for_node(manifest, config.project_name, node)
     ctx = generate_runtime_docs_context(config, node, manifest, config.project_name)
     _process_docs_for_node(ctx, node)
 
 
-def write_publication_artifact(root_project: RuntimeConfig, manifest: Manifest):
+def log_publication_artifact(root_project: RuntimeConfig, manifest: Manifest):
     # The manifest.json is written out in a task, so we're not writing it here
 
     # build publication metadata
     metadata = PublicationMetadata(
         adapter_type=root_project.credentials.type,
         quoting=root_project.quoting,
     )
 
     # get a set of public model ids first so it can be used in constructing dependencies
     public_node_ids = {
         node.unique_id
         for node in manifest.nodes.values()
-        if node.resource_type == NodeType.Model and node.access == AccessType.Public
+        if isinstance(node, ModelNode) and node.access == AccessType.Public
     }
 
     # Get the Graph object from the Linker
     from dbt.compilation import Linker
 
     linker = Linker()
     graph = linker.get_graph(manifest)
 
     public_models = {}
     for unique_id in public_node_ids:
         model = manifest.nodes[unique_id]
+        assert isinstance(model, ModelNode)
         # public_node_dependencies is the intersection of all parent nodes plus public nodes
         parents: Set[UniqueId] = graph.select_parents({UniqueId(unique_id)})
         public_node_dependencies: Set[UniqueId] = parents.intersection(public_node_ids)
 
         public_model = PublicModel(
             name=model.name,
             package_name=model.package_name,
@@ -1722,14 +1796,15 @@
             database=model.database,
             schema=model.schema,
             identifier=model.alias,
             version=model.version,
             latest_version=model.latest_version,
             public_node_dependencies=list(public_node_dependencies),
             generated_at=metadata.generated_at,
+            deprecation_date=model.deprecation_date,
         )
         public_models[unique_id] = public_model
 
     dependencies = []
     # Get dependencies from dependencies.yml
     if manifest.project_dependencies:
         for dep_project in manifest.project_dependencies.projects:
@@ -1746,16 +1821,14 @@
 
     publication = PublicationArtifact(
         metadata=metadata,
         project_name=root_project.project_name,
         public_models=public_models,
         dependencies=dependencies,
     )
-    # write out publication artifact <project_name>_publication.json
-    publication_file_name = f"{root_project.project_name}_publication.json"
-    path = os.path.join(root_project.target_path, publication_file_name)
-    publication.write(path)
+
+    fire_event(PublicationArtifactAvailable(pub_artifact=publication.to_dict()))
 
 
 def write_manifest(manifest: Manifest, target_path: str):
     path = os.path.join(target_path, MANIFEST_FILE_NAME)
     manifest.write(path)
```

### Comparing `dbt-core-1.6.0b1/dbt/parser/models.py` & `dbt-core-1.6.0b2/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/partial.py` & `dbt-core-1.6.0b2/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/read_files.py` & `dbt-core-1.6.0b2/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0b2/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/schemas.py` & `dbt-core-1.6.0b2/dbt/parser/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,607 +1,223 @@
-import itertools
-import os
-import pathlib
+import datetime
+import time
 
 from abc import ABCMeta, abstractmethod
-from typing import Iterable, Dict, Any, Union, List, Optional, Generic, TypeVar, Type, Callable
+from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Type, TypeVar
 from dataclasses import dataclass, field
 
 from dbt.dataclass_schema import ValidationError, dbtClassMixin
 
-from dbt.adapters.factory import get_adapter, get_adapter_package_names
-from dbt.clients.jinja import get_rendered, add_rendered_test_kwargs
 from dbt.clients.yaml_helper import load_yaml_text
-from dbt.context.providers import RefArgs
 from dbt.parser.schema_renderer import SchemaYamlRenderer
-from dbt.context.context_config import (
-    ContextConfig,
-    BaseContextConfigGenerator,
-    ContextConfigGenerator,
-    UnrenderedConfigGenerator,
-)
+from dbt.parser.schema_generic_tests import SchemaGenericTestParser
+from dbt.context.context_config import ContextConfig
 from dbt.context.configured import generate_schema_yml_context, SchemaYamlVars
-from dbt.context.providers import (
-    generate_parse_exposure,
-    generate_parse_metrics,
-    generate_test_context,
-)
-from dbt.context.macro_resolver import MacroResolver
-from dbt.contracts.files import FileHash, SchemaSourceFile
-from dbt.contracts.graph.model_config import MetricConfig, ExposureConfig
+from dbt.contracts.files import SchemaSourceFile
 from dbt.contracts.graph.nodes import (
     ParsedNodePatch,
-    ColumnInfo,
-    ColumnLevelConstraint,
-    GenericTestNode,
     ParsedMacroPatch,
     UnpatchedSourceDefinition,
-    Exposure,
-    Metric,
-    Group,
-    ManifestNode,
-    GraphMemberNode,
     ConstraintType,
     ModelNode,
     ModelLevelConstraint,
 )
 from dbt.contracts.graph.unparsed import (
     HasColumnDocs,
     HasColumnTests,
-    HasColumnProps,
     SourcePatch,
     UnparsedAnalysisUpdate,
-    UnparsedColumn,
     UnparsedMacroUpdate,
     UnparsedNodeUpdate,
     UnparsedModelUpdate,
-    UnparsedExposure,
-    UnparsedMetric,
     UnparsedSourceDefinition,
-    UnparsedGroup,
-    NodeVersion,
 )
 from dbt.exceptions import (
-    CompilationError,
     DuplicateMacroPatchNameError,
     DuplicatePatchPathError,
     DuplicateSourcePatchNameError,
     JSONValidationError,
     DbtInternalError,
-    SchemaConfigError,
-    TestConfigError,
     ParsingError,
     DbtValidationError,
     YamlLoadError,
     YamlParseDictError,
     YamlParseListError,
+    InvalidAccessTypeError,
 )
 from dbt.events.functions import warn_or_error
-from dbt.events.types import WrongResourceSchemaFile, NoNodeForYamlKey, MacroNotFoundForPatch
-from dbt.node_types import NodeType
+from dbt.events.types import (
+    WrongResourceSchemaFile,
+    NoNodeForYamlKey,
+    MacroNotFoundForPatch,
+    ValidationWarning,
+)
+from dbt.node_types import NodeType, AccessType
 from dbt.parser.base import SimpleParser
 from dbt.parser.search import FileBlock
-from dbt.parser.generic_test_builders import (
-    TestBuilder,
-    GenericTestBlock,
-    TargetBlock,
+from dbt.parser.common import (
     YamlBlock,
+    TargetBlock,
     TestBlock,
     VersionedTestBlock,
-    Testable,
-    Versioned,
+    ParserRef,
+    trimmed,
 )
-from dbt.utils import get_pseudo_test_path, coerce_dict_str, md5, deep_merge
-
+from dbt.utils import coerce_dict_str, deep_merge
 
-TestDef = Union[str, Dict[str, Any]]
 
 schema_file_keys = (
     "models",
     "seeds",
     "snapshots",
     "sources",
     "macros",
     "analyses",
     "exposures",
     "metrics",
 )
 
 
+# ===============================================================================
+#  Schema Parser classes
+#
+# The SchemaParser is a subclass of the SimpleParser from base.py, as is
+# the SchemaGenericTestParser. The schema sub-parsers are all subclasses of
+# the YamlReader parsing class. Most of the action in creating SourceDefinition
+# nodes actually happens in the SourcePatcher class, in sources.py, which is
+# called as a late-stage parsing step in manifest.py.
+#
+# The "patch" parsers read yaml config and properties and apply them to
+# nodes that were already created from sql files.
+#
+# The SchemaParser and SourcePatcher both use the SchemaGenericTestParser
+# (in schema_generic_tests.py) to create generic test nodes.
+#
+#  YamlReader
+#      MetricParser (metrics) [schema_yaml_readers.py]
+#      ExposureParser (exposures) [schema_yaml_readers.py]
+#      GroupParser  (groups) [schema_yaml_readers.py]
+#      SourceParser (sources)
+#      PatchParser
+#          MacroPatchParser (macros)
+#          NodePatchParser
+#              ModelPatchParser (models)
+#              AnalysisPatchParser (analyses)
+#              TestablePatchParser (seeds, snapshots)
+#
+# ===============================================================================
+
+
 def yaml_from_file(source_file: SchemaSourceFile) -> Dict[str, Any]:
     """If loading the yaml fails, raise an exception."""
     try:
         # source_file.contents can sometimes be None
         return load_yaml_text(source_file.contents or "", source_file.path)
     except DbtValidationError as e:
         raise YamlLoadError(
             project_name=source_file.project_name, path=source_file.path.relative_path, exc=e
         )
 
 
-class ParserRef:
-    """A helper object to hold parse-time references."""
-
-    def __init__(self):
-        self.column_info: Dict[str, ColumnInfo] = {}
-
-    def _add(self, column: HasColumnProps):
-        tags: List[str] = []
-        tags.extend(getattr(column, "tags", ()))
-        quote: Optional[bool]
-        if isinstance(column, UnparsedColumn):
-            quote = column.quote
-        else:
-            quote = None
-
-        if any(
-            c
-            for c in column.constraints
-            if "type" not in c or not ConstraintType.is_valid(c["type"])
-        ):
-            raise ParsingError(f"Invalid constraint type on column {column.name}")
-
-        self.column_info[column.name] = ColumnInfo(
-            name=column.name,
-            description=column.description,
-            data_type=column.data_type,
-            constraints=[ColumnLevelConstraint.from_dict(c) for c in column.constraints],
-            meta=column.meta,
-            tags=tags,
-            quote=quote,
-            _extra=column.extra,
-        )
-
-    @classmethod
-    def from_target(cls, target: Union[HasColumnDocs, HasColumnTests]) -> "ParserRef":
-        refs = cls()
-        for column in target.columns:
-            refs._add(column)
-        return refs
-
-    @classmethod
-    def from_versioned_target(cls, target: Versioned, version: NodeVersion) -> "ParserRef":
-        refs = cls()
-        for base_column in target.get_columns_for_version(version):
-            refs._add(base_column)
-        return refs
-
-
-def _trimmed(inp: str) -> str:
-    if len(inp) < 50:
-        return inp
-    return inp[:44] + "..." + inp[-3:]
-
-
-class SchemaParser(SimpleParser[GenericTestBlock, GenericTestNode]):
+# This is the main schema file parser, but almost everything happens in the
+# the schema sub-parsers.
+class SchemaParser(SimpleParser[YamlBlock, ModelNode]):
     def __init__(
         self,
         project,
         manifest,
         root_project,
     ) -> None:
         super().__init__(project, manifest, root_project)
 
+        self.generic_test_parser = SchemaGenericTestParser(project, manifest, root_project)
+
         self.schema_yaml_vars = SchemaYamlVars()
         self.render_ctx = generate_schema_yml_context(
             self.root_project, self.project.project_name, self.schema_yaml_vars
         )
-        internal_package_names = get_adapter_package_names(self.root_project.credentials.type)
-        self.macro_resolver = MacroResolver(
-            self.manifest.macros, self.root_project.project_name, internal_package_names
-        )
 
     @classmethod
     def get_compiled_path(cls, block: FileBlock) -> str:
         # should this raise an error?
         return block.path.relative_path
 
     @property
     def resource_type(self) -> NodeType:
         return NodeType.Test
 
-    def parse_from_dict(self, dct, validate=True) -> GenericTestNode:
-        if validate:
-            GenericTestNode.validate(dct)
-        return GenericTestNode.from_dict(dct)
-
-    def parse_column_tests(
-        self, block: TestBlock, column: UnparsedColumn, version: Optional[NodeVersion]
-    ) -> None:
-        if not column.tests:
-            return
-
-        for test in column.tests:
-            self.parse_test(block, test, column, version)
-
-    def create_test_node(
-        self,
-        target: Union[UnpatchedSourceDefinition, UnparsedNodeUpdate],
-        path: str,
-        config: ContextConfig,
-        tags: List[str],
-        fqn: List[str],
-        name: str,
-        raw_code: str,
-        test_metadata: Dict[str, Any],
-        file_key_name: str,
-        column_name: Optional[str],
-    ) -> GenericTestNode:
-
-        HASH_LENGTH = 10
-
-        # N.B: This function builds a hashable string from any given test_metadata dict.
-        #   it's a bit fragile for general use (only supports str, int, float, List, Dict)
-        #   but it gets the job done here without the overhead of complete ser(de).
-        def get_hashable_md(data: Union[str, int, float, List, Dict]) -> Union[str, List, Dict]:
-            if type(data) == dict:
-                return {k: get_hashable_md(data[k]) for k in sorted(data.keys())}  # type: ignore
-            elif type(data) == list:
-                return [get_hashable_md(val) for val in data]  # type: ignore
-            else:
-                return str(data)
-
-        hashable_metadata = repr(get_hashable_md(test_metadata))
-        hash_string = "".join([name, hashable_metadata])
-        test_hash = md5(hash_string)[-HASH_LENGTH:]
-
-        dct = {
-            "alias": name,
-            "schema": self.default_schema,
-            "database": self.default_database,
-            "fqn": fqn,
-            "name": name,
-            "resource_type": self.resource_type,
-            "tags": tags,
-            "path": path,
-            "original_file_path": target.original_file_path,
-            "package_name": self.project.project_name,
-            "raw_code": raw_code,
-            "language": "sql",
-            "unique_id": self.generate_unique_id(name, test_hash),
-            "config": self.config_dict(config),
-            "test_metadata": test_metadata,
-            "column_name": column_name,
-            "checksum": FileHash.empty().to_dict(omit_none=True),
-            "file_key_name": file_key_name,
-        }
-        try:
-            GenericTestNode.validate(dct)
-            return GenericTestNode.from_dict(dct)
-        except ValidationError as exc:
-            # this is a bit silly, but build an UnparsedNode just for error
-            # message reasons
-            node = self._create_error_node(
-                name=target.name,
-                path=path,
-                original_file_path=target.original_file_path,
-                raw_code=raw_code,
-            )
-            raise TestConfigError(exc, node)
-
-    # lots of time spent in this method
-    def _parse_generic_test(
-        self,
-        target: Testable,
-        test: Dict[str, Any],
-        tags: List[str],
-        column_name: Optional[str],
-        schema_file_id: str,
-        version: Optional[NodeVersion],
-    ) -> GenericTestNode:
-        try:
-            builder = TestBuilder(
-                test=test,
-                target=target,
-                column_name=column_name,
-                version=version,
-                package_name=target.package_name,
-                render_ctx=self.render_ctx,
-            )
-            if self.schema_yaml_vars.env_vars:
-                self.store_env_vars(target, schema_file_id, self.schema_yaml_vars.env_vars)
-                self.schema_yaml_vars.env_vars = {}
-
-        except ParsingError as exc:
-            context = _trimmed(str(target))
-            msg = "Invalid test config given in {}:\n\t{}\n\t@: {}".format(
-                target.original_file_path, exc.msg, context
-            )
-            raise ParsingError(msg) from exc
-
-        except CompilationError as exc:
-            context = _trimmed(str(target))
-            msg = (
-                "Invalid generic test configuration given in "
-                f"{target.original_file_path}: \n{exc.msg}\n\t@: {context}"
-            )
-            raise CompilationError(msg) from exc
-
-        original_name = os.path.basename(target.original_file_path)
-        compiled_path = get_pseudo_test_path(builder.compiled_name, original_name)
-
-        # fqn is the relative path of the yaml file where this generic test is defined,
-        # minus the project-level directory and the file name itself
-        # TODO pass a consistent path object from both UnparsedNode and UnpatchedSourceDefinition
-        path = pathlib.Path(target.original_file_path)
-        relative_path = str(path.relative_to(*path.parts[:1]))
-        fqn = self.get_fqn(relative_path, builder.fqn_name)
-
-        # this is the ContextConfig that is used in render_update
-        config: ContextConfig = self.initial_config(fqn)
-
-        # builder.args contains keyword args for the test macro,
-        # not configs which have been separated out in the builder.
-        # The keyword args are not completely rendered until compilation.
-        metadata = {
-            "namespace": builder.namespace,
-            "name": builder.name,
-            "kwargs": builder.args,
-        }
-        tags = sorted(set(itertools.chain(tags, builder.tags())))
-
-        if isinstance(target, UnpatchedSourceDefinition):
-            file_key_name = f"{target.source.yaml_key}.{target.source.name}"
-        else:
-            file_key_name = f"{target.yaml_key}.{target.name}"
-
-        node = self.create_test_node(
-            target=target,
-            path=compiled_path,
-            config=config,
-            fqn=fqn,
-            tags=tags,
-            name=builder.fqn_name,
-            raw_code=builder.build_raw_code(),
-            column_name=column_name,
-            test_metadata=metadata,
-            file_key_name=file_key_name,
-        )
-        self.render_test_update(node, config, builder, schema_file_id)
-
-        return node
-
-    def _lookup_attached_node(
-        self, target: Testable, version: Optional[NodeVersion]
-    ) -> Optional[Union[ManifestNode, GraphMemberNode]]:
-        """Look up attached node for Testable target nodes other than sources. Can be None if generic test attached to SQL node with no corresponding .sql file."""
-        attached_node = None  # type: Optional[Union[ManifestNode, GraphMemberNode]]
-        if not isinstance(target, UnpatchedSourceDefinition):
-            attached_node_unique_id = self.manifest.ref_lookup.get_unique_id(
-                target.name, None, version
-            )
-            if attached_node_unique_id:
-                attached_node = self.manifest.nodes[attached_node_unique_id]
-            else:
-                disabled_node = self.manifest.disabled_lookup.find(
-                    target.name, None
-                ) or self.manifest.disabled_lookup.find(target.name.upper(), None)
-                if disabled_node:
-                    attached_node = self.manifest.disabled[disabled_node[0].unique_id][0]
-        return attached_node
-
-    def store_env_vars(self, target, schema_file_id, env_vars):
-        self.manifest.env_vars.update(env_vars)
-        if schema_file_id in self.manifest.files:
-            schema_file = self.manifest.files[schema_file_id]
-            if isinstance(target, UnpatchedSourceDefinition):
-                search_name = target.source.name
-                yaml_key = target.source.yaml_key
-                if "." in search_name:  # source file definitions
-                    (search_name, _) = search_name.split(".")
-            else:
-                search_name = target.name
-                yaml_key = target.yaml_key
-            for var in env_vars.keys():
-                schema_file.add_env_var(var, yaml_key, search_name)
-
-    # This does special shortcut processing for the two
-    # most common internal macros, not_null and unique,
-    # which avoids the jinja rendering to resolve config
-    # and variables, etc, which might be in the macro.
-    # In the future we will look at generalizing this
-    # more to handle additional macros or to use static
-    # parsing to avoid jinja overhead.
-    def render_test_update(self, node, config, builder, schema_file_id):
-        macro_unique_id = self.macro_resolver.get_macro_id(
-            node.package_name, "test_" + builder.name
-        )
-        # Add the depends_on here so we can limit the macros added
-        # to the context in rendering processing
-        node.depends_on.add_macro(macro_unique_id)
-        if macro_unique_id in ["macro.dbt.test_not_null", "macro.dbt.test_unique"]:
-            config_call_dict = builder.get_static_config()
-            config._config_call_dict = config_call_dict
-            # This sets the config from dbt_project
-            self.update_parsed_node_config(node, config)
-            # source node tests are processed at patch_source time
-            if isinstance(builder.target, UnpatchedSourceDefinition):
-                sources = [builder.target.fqn[-2], builder.target.fqn[-1]]
-                node.sources.append(sources)
-            else:  # all other nodes
-                node.refs.append(RefArgs(name=builder.target.name, version=builder.version))
-        else:
-            try:
-                # make a base context that doesn't have the magic kwargs field
-                context = generate_test_context(
-                    node,
-                    self.root_project,
-                    self.manifest,
-                    config,
-                    self.macro_resolver,
-                )
-                # update with rendered test kwargs (which collects any refs)
-                # Note: This does not actually update the kwargs with the rendered
-                # values. That happens in compilation.
-                add_rendered_test_kwargs(context, node, capture_macros=True)
-                # the parsed node is not rendered in the native context.
-                get_rendered(node.raw_code, context, node, capture_macros=True)
-                self.update_parsed_node_config(node, config)
-                # env_vars should have been updated in the context env_var method
-            except ValidationError as exc:
-                # we got a ValidationError - probably bad types in config()
-                raise SchemaConfigError(exc, node=node) from exc
-
-        # Set attached_node for generic test nodes, if available.
-        # Generic test node inherits attached node's group config value.
-        attached_node = self._lookup_attached_node(builder.target, builder.version)
-        if attached_node:
-            node.attached_node = attached_node.unique_id
-            node.group, node.group = attached_node.group, attached_node.group
-
-    def parse_node(self, block: GenericTestBlock) -> GenericTestNode:
-        """In schema parsing, we rewrite most of the part of parse_node that
-        builds the initial node to be parsed, but rendering is basically the
-        same
-        """
-        node = self._parse_generic_test(
-            target=block.target,
-            test=block.test,
-            tags=block.tags,
-            column_name=block.column_name,
-            schema_file_id=block.file.file_id,
-            version=block.version,
-        )
-        self.add_test_node(block, node)
-        return node
-
-    def add_test_node(self, block: GenericTestBlock, node: GenericTestNode):
-        test_from = {"key": block.target.yaml_key, "name": block.target.name}
-        if node.config.enabled:
-            self.manifest.add_node(block.file, node, test_from)
-        else:
-            self.manifest.add_disabled(block.file, node, test_from)
-
-    def render_with_context(
-        self,
-        node: GenericTestNode,
-        config: ContextConfig,
-    ) -> None:
-        """Given the parsed node and a ContextConfig to use during
-        parsing, collect all the refs that might be squirreled away in the test
-        arguments. This includes the implicit "model" argument.
-        """
-        # make a base context that doesn't have the magic kwargs field
-        context = self._context_for(node, config)
-        # update it with the rendered test kwargs (which collects any refs)
-        add_rendered_test_kwargs(context, node, capture_macros=True)
-
-        # the parsed node is not rendered in the native context.
-        get_rendered(node.raw_code, context, node, capture_macros=True)
-
-    def parse_test(
-        self,
-        target_block: TestBlock,
-        test: TestDef,
-        column: Optional[UnparsedColumn],
-        version: Optional[NodeVersion],
-    ) -> None:
-        if isinstance(test, str):
-            test = {test: {}}
-
-        if column is None:
-            column_name: Optional[str] = None
-            column_tags: List[str] = []
-        else:
-            column_name = column.name
-            should_quote = column.quote or (column.quote is None and target_block.quote_columns)
-            if should_quote:
-                column_name = get_adapter(self.root_project).quote(column_name)
-            column_tags = column.tags
-
-        block = GenericTestBlock.from_test_block(
-            src=target_block,
-            test=test,
-            column_name=column_name,
-            tags=column_tags,
-            version=version,
-        )
-        self.parse_node(block)
-
-    def parse_tests(self, block: TestBlock) -> None:
-        for column in block.columns:
-            self.parse_column_tests(block, column, None)
-
-        for test in block.tests:
-            self.parse_test(block, test, None, None)
-
-    def parse_versioned_tests(self, block: VersionedTestBlock) -> None:
-        if not block.target.versions:
-            self.parse_tests(block)
-        else:
-            for version in block.target.versions:
-                for column in block.target.get_columns_for_version(version.v):
-                    self.parse_column_tests(block, column, version.v)
-
-                for test in block.target.get_tests_for_version(version.v):
-                    self.parse_test(block, test, None, version.v)
-
     def parse_file(self, block: FileBlock, dct: Dict = None) -> None:
         assert isinstance(block.file, SchemaSourceFile)
 
         # If partially parsing, dct should be from pp_dict, otherwise
         # dict_from_yaml
         if dct:
             # contains the FileBlock and the data (dictionary)
             yaml_block = YamlBlock.from_file_block(block, dct)
 
-            parser: YamlDocsReader
+            parser: YamlReader
 
-            # There are 7 kinds of parsers:
-            # Model, Seed, Snapshot, Source, Macro, Analysis, Exposures
+            # There are 9 different yaml lists which are parsed by different parsers:
+            # Model, Seed, Snapshot, Source, Macro, Analysis, Exposure, Metric, Group
 
             # ModelPatchParser.parse()
             if "models" in dct:
                 # the models are already in the manifest as nodes when we reach this code,
                 # even if they are disabled in the schema file
                 model_parse_result = ModelPatchParser(self, yaml_block, "models").parse()
                 for versioned_test_block in model_parse_result.versioned_test_blocks:
-                    self.parse_versioned_tests(versioned_test_block)
+                    self.generic_test_parser.parse_versioned_tests(versioned_test_block)
 
-            # NonSourceParser.parse()
+            # PatchParser.parse()
             if "seeds" in dct:
                 seed_parse_result = TestablePatchParser(self, yaml_block, "seeds").parse()
                 for test_block in seed_parse_result.test_blocks:
-                    self.parse_tests(test_block)
+                    self.generic_test_parser.parse_tests(test_block)
 
-            # NonSourceParser.parse()
+            # PatchParser.parse()
             if "snapshots" in dct:
                 snapshot_parse_result = TestablePatchParser(self, yaml_block, "snapshots").parse()
                 for test_block in snapshot_parse_result.test_blocks:
-                    self.parse_tests(test_block)
+                    self.generic_test_parser.parse_tests(test_block)
 
             # This parser uses SourceParser.parse() which doesn't return
             # any test blocks. Source tests are handled at a later point
             # in the process.
             if "sources" in dct:
                 parser = SourceParser(self, yaml_block, "sources")
                 parser.parse()
 
-            # NonSourceParser.parse() (but never test_blocks)
+            # PatchParser.parse() (but never test_blocks)
             if "macros" in dct:
                 parser = MacroPatchParser(self, yaml_block, "macros")
                 parser.parse()
 
-            # NonSourceParser.parse() (but never test_blocks)
+            # PatchParser.parse() (but never test_blocks)
             if "analyses" in dct:
                 parser = AnalysisPatchParser(self, yaml_block, "analyses")
                 parser.parse()
 
-            # parse exposures
+            # ExposureParser.parse()
             if "exposures" in dct:
+                from dbt.parser.schema_yaml_readers import ExposureParser
+
                 exp_parser = ExposureParser(self, yaml_block)
                 exp_parser.parse()
 
-            # parse metrics
+            # MetricParser.parse()
             if "metrics" in dct:
+                from dbt.parser.schema_yaml_readers import MetricParser
+
                 metric_parser = MetricParser(self, yaml_block)
                 metric_parser.parse()
 
-            # parse groups
+            # GroupParser.parse()
             if "groups" in dct:
+                from dbt.parser.schema_yaml_readers import GroupParser
+
                 group_parser = GroupParser(self, yaml_block)
                 group_parser.parse()
 
 
 Parsed = TypeVar("Parsed", UnpatchedSourceDefinition, ParsedNodePatch, ParsedMacroPatch)
 NodeTarget = TypeVar("NodeTarget", UnparsedNodeUpdate, UnparsedAnalysisUpdate, UnparsedModelUpdate)
 NonSourceTarget = TypeVar(
@@ -616,14 +232,15 @@
 @dataclass
 class ParseResult:
     test_blocks: List[TestBlock] = field(default_factory=list)
     versioned_test_blocks: List[VersionedTestBlock] = field(default_factory=list)
 
 
 # abstract base class (ABCMeta)
+# Four subclasses: MetricParser, ExposureParser, GroupParser, SourceParser, PatchParser
 class YamlReader(metaclass=ABCMeta):
     def __init__(self, schema_parser: SchemaParser, yaml: YamlBlock, key: str) -> None:
         self.schema_parser = schema_parser
         # key: models, seeds, snapshots, sources, macros,
         # analyses, exposures
         self.key = key
         self.yaml = yaml
@@ -655,15 +272,15 @@
     # get the list of dicts pointed to by the key in the yaml config,
     # ensure that the dicts have string keys
     def get_key_dicts(self) -> Iterable[Dict[str, Any]]:
         data = self.yaml.data.get(self.key, [])
         if not isinstance(data, list):
             raise ParsingError(
                 "{} must be a list, got {} instead: ({})".format(
-                    self.key, type(data), _trimmed(str(data))
+                    self.key, type(data), trimmed(str(data))
                 )
             )
         path = self.yaml.path.original_file_path
 
         # for each dict in the data (which is a list of dicts)
         for entry in data:
 
@@ -695,36 +312,33 @@
         except ParsingError as exc:
             raise ParsingError(
                 f"Failed to render {self.yaml.file.path.original_file_path} from "
                 f"project {self.project.project_name}: {exc}"
             ) from exc
         return dct
 
-
-class YamlDocsReader(YamlReader):
     @abstractmethod
     def parse(self) -> ParseResult:
         raise NotImplementedError("parse is abstract")
 
 
 T = TypeVar("T", bound=dbtClassMixin)
 
 
 # This parses the 'sources' keys in yaml files.
-class SourceParser(YamlDocsReader):
+class SourceParser(YamlReader):
     def _target_from_dict(self, cls: Type[T], data: Dict[str, Any]) -> T:
         path = self.yaml.path.original_file_path
         try:
             cls.validate(data)
             return cls.from_dict(data)
         except (ValidationError, JSONValidationError) as exc:
             raise YamlParseDictError(path, self.key, data, exc)
 
-    # The other parse method returns TestBlocks. This one doesn't.
-    # This takes the yaml dictionaries in 'sources' keys and uses them
+    # This parse method takes the yaml dictionaries in 'sources' keys and uses them
     # to create UnparsedSourceDefinition objects. They are then turned
     # into UnpatchedSourceDefinition objects in 'add_source_definitions'
     # or SourcePatch objects in 'add_source_patch'
     def parse(self) -> ParseResult:
         # get a verified list of dicts for the key handled by this parser
         for data in self.get_key_dicts():
             data = self.project.credentials.translate_aliases(data, recurse=True)
@@ -767,17 +381,16 @@
                 resource_type=NodeType.Source,
                 fqn=fqn,
                 name=f"{source.name}_{table.name}",
             )
             self.manifest.add_source(self.yaml.file, source_def)
 
 
-# This class has three main subclasses: TestablePatchParser (models,
-# seeds, snapshots), MacroPatchParser, and AnalysisPatchParser
-class NonSourceParser(YamlDocsReader, Generic[NonSourceTarget, Parsed]):
+# This class has two subclasses: NodePatchParser and MacroPatchParser
+class PatchParser(YamlReader, Generic[NonSourceTarget, Parsed]):
     @abstractmethod
     def _target_type(self) -> Type[NonSourceTarget]:
         raise NotImplementedError("_target_type not implemented")
 
     @abstractmethod
     def get_block(self, node: NonSourceTarget) -> TargetBlock:
         raise NotImplementedError("get_block is abstract")
@@ -892,32 +505,40 @@
             self.schema_parser.project.project_name,
         )
         # We need to re-apply the config_call_dict after the patch config
         config._config_call_dict = node.config_call_dict
         self.schema_parser.update_parsed_node_config(node, config, patch_config_dict=patch.config)
 
 
-class NodePatchParser(NonSourceParser[NodeTarget, ParsedNodePatch], Generic[NodeTarget]):
+# Subclasses of NodePatchParser: TestablePatchParser, ModelPatchParser, AnalysisPatchParser,
+# so models, seeds, snapshots, analyses
+class NodePatchParser(PatchParser[NodeTarget, ParsedNodePatch], Generic[NodeTarget]):
     def parse_patch(self, block: TargetBlock[NodeTarget], refs: ParserRef) -> None:
         # We're not passing the ParsedNodePatch around anymore, so we
         # could possibly skip creating one. Leaving here for now for
         # code consistency.
+        deprecation_date: Optional[datetime.datetime] = None
+        if isinstance(block.target, UnparsedModelUpdate):
+            deprecation_date = block.target.deprecation_date
+
         patch = ParsedNodePatch(
             name=block.target.name,
             original_file_path=block.target.original_file_path,
             yaml_key=block.target.yaml_key,
             package_name=block.target.package_name,
             description=block.target.description,
             columns=refs.column_info,
             meta=block.target.meta,
             docs=block.target.docs,
             config=block.target.config,
             access=block.target.access,
             version=None,
             latest_version=None,
+            constraints=block.target.constraints,
+            deprecation_date=deprecation_date,
         )
         assert isinstance(self.yaml.file, SchemaSourceFile)
         source_file: SchemaSourceFile = self.yaml.file
         if patch.yaml_key in ["models", "seeds", "snapshots"]:
             unique_id = self.manifest.ref_lookup.get_unique_id(
                 patch.name, self.project.project_name, None
             ) or self.manifest.ref_lookup.get_unique_id(patch.name, None, None)
@@ -966,15 +587,15 @@
                 for node in found_nodes:
                     node.patch_path = source_file.file_id
                     # re-calculate the node config with the patch config.  Always do this
                     # for the case when no config is set to ensure the default of true gets captured
                     if patch.config:
                         self.patch_node_config(node, patch)
 
-                    node.patch(patch)
+                    self.patch_node_properties(node, patch)
             else:
                 warn_or_error(
                     NoNodeForYamlKey(
                         patch_name=patch.name,
                         yaml_key=patch.yaml_key,
                         file_path=source_file.path.original_file_path,
                     )
@@ -990,56 +611,38 @@
 
             source_file.append_patch(patch.yaml_key, node.unique_id)
             # re-calculate the node config with the patch config.  Always do this
             # for the case when no config is set to ensure the default of true gets captured
             if patch.config:
                 self.patch_node_config(node, patch)
 
-            node.patch(patch)
-            # TODO: We want to do all the actual patching either in the above node.patch() call
-            # or here, but it will require some thought to the details. For now the patching is
-            # awkwardly split.
-            self.patch_constraints(node, block.target.constraints)
-            node.build_contract_checksum()
-
-    def patch_constraints(self, node, constraints):
-        contract_config = node.config.get("contract")
-        if isinstance(node, ModelNode) and contract_config.enforced is True:
-            self._validate_constraint_prerequisites(node)
-
-            if any(
-                c for c in constraints if "type" not in c or not ConstraintType.is_valid(c["type"])
-            ):
-                raise ParsingError(
-                    f"Invalid constraint type on model {node.name}: "
-                    f"Type must be one of {[ct.value for ct in ConstraintType]}"
-                )
-
-            node.constraints = [ModelLevelConstraint.from_dict(c) for c in constraints]
-
-    def _validate_constraint_prerequisites(self, model_node: ModelNode):
-        errors = []
-        if not model_node.columns:
-            errors.append(
-                "Constraints must be defined in a `yml` schema configuration file like `schema.yml`."
-            )
+            self.patch_node_properties(node, patch)
 
-        if model_node.config.materialized not in ["table", "view", "incremental"]:
-            errors.append(
-                f"Only table, view, and incremental materializations are supported for constraints, but found '{model_node.config.materialized}'"
-            )
-
-        if str(model_node.language) != "sql":
-            errors.append(f"Language Error: Expected 'sql' but found '{model_node.language}'")
-
-        if errors:
-            raise ParsingError(
-                f"Constraint validation failed for: ({model_node.original_file_path})\n"
-                + "\n".join(errors)
-            )
+    def patch_node_properties(self, node, patch: "ParsedNodePatch"):
+        """Given a ParsedNodePatch, add the new information to the node."""
+        # explicitly pick out the parts to update so we don't inadvertently
+        # step on the model name or anything
+        # Note: config should already be updated
+        node.patch_path = patch.file_id
+        # update created_at so process_docs will run in partial parsing
+        node.created_at = time.time()
+        node.description = patch.description
+        node.columns = patch.columns
+        node.name = patch.name
+
+        if not isinstance(node, ModelNode):
+            for attr in ["latest_version", "access", "version", "constraints"]:
+                if getattr(patch, attr):
+                    warn_or_error(
+                        ValidationWarning(
+                            field_name=attr,
+                            resource_type=node.resource_type.value,
+                            node_name=patch.name,
+                        )
+                    )
 
 
 # TestablePatchParser = seeds, snapshots
 class TestablePatchParser(NodePatchParser[UnparsedNodeUpdate]):
     def get_block(self, node: UnparsedNodeUpdate) -> TestBlock:
         return TestBlock.from_yaml_block(self.yaml, node)
 
@@ -1159,47 +762,95 @@
                     columns=version_refs.column_info,
                     meta=target.meta,
                     docs=unparsed_version.docs or target.docs,
                     config=deep_merge(target.config, unparsed_version.config),
                     access=unparsed_version.access or target.access,
                     version=unparsed_version.v,
                     latest_version=latest_version,
+                    constraints=unparsed_version.constraints or target.constraints,
+                    deprecation_date=unparsed_version.deprecation_date,
                 )
                 # Node patched before config because config patching depends on model name,
                 # which may have been updated in the version patch
-                versioned_model_node.patch(versioned_model_patch)
-                # TODO: We want to do all the actual patching either in the above node.patch() call
-                # or here, but it will require some thought to the details. For now the patching is
-                # awkwardly split.
-                self.patch_constraints(
-                    versioned_model_node, unparsed_version.constraints or target.constraints
-                )
-                versioned_model_node.build_contract_checksum()
+                # versioned_model_node.patch(versioned_model_patch)
+                self.patch_node_properties(versioned_model_node, versioned_model_patch)
 
                 # Includes alias recomputation
                 self.patch_node_config(versioned_model_node, versioned_model_patch)
                 source_file.append_patch(
                     versioned_model_patch.yaml_key, versioned_model_node.unique_id
                 )
             self.manifest.rebuild_ref_lookup()
             self.manifest.rebuild_disabled_lookup()
 
     def _target_type(self) -> Type[UnparsedModelUpdate]:
         return UnparsedModelUpdate
 
+    def patch_node_properties(self, node, patch: "ParsedNodePatch"):
+        super().patch_node_properties(node, patch)
+        node.version = patch.version
+        node.latest_version = patch.latest_version
+        node.deprecation_date = patch.deprecation_date
+        if patch.access:
+            if AccessType.is_valid(patch.access):
+                node.access = AccessType(patch.access)
+            else:
+                raise InvalidAccessTypeError(
+                    unique_id=node.unique_id,
+                    field_value=patch.access,
+                )
+        self.patch_constraints(node, patch.constraints)
+        node.build_contract_checksum()
+
+    def patch_constraints(self, node, constraints):
+        contract_config = node.config.get("contract")
+        if contract_config.enforced is True:
+            self._validate_constraint_prerequisites(node)
+
+            if any(
+                c for c in constraints if "type" not in c or not ConstraintType.is_valid(c["type"])
+            ):
+                raise ParsingError(
+                    f"Invalid constraint type on model {node.name}: "
+                    f"Type must be one of {[ct.value for ct in ConstraintType]}"
+                )
+
+            node.constraints = [ModelLevelConstraint.from_dict(c) for c in constraints]
+
+    def _validate_constraint_prerequisites(self, model_node: ModelNode):
+        errors = []
+        if not model_node.columns:
+            errors.append(
+                "Constraints must be defined in a `yml` schema configuration file like `schema.yml`."
+            )
+
+        if model_node.config.materialized not in ["table", "view", "incremental"]:
+            errors.append(
+                f"Only table, view, and incremental materializations are supported for constraints, but found '{model_node.config.materialized}'"
+            )
+
+        if str(model_node.language) != "sql":
+            errors.append(f"Language Error: Expected 'sql' but found '{model_node.language}'")
+
+        if errors:
+            raise ParsingError(
+                f"Constraint validation failed for: ({model_node.original_file_path})\n"
+                + "\n".join(errors)
+            )
+
 
 class AnalysisPatchParser(NodePatchParser[UnparsedAnalysisUpdate]):
     def get_block(self, node: UnparsedAnalysisUpdate) -> TargetBlock:
         return TargetBlock.from_yaml_block(self.yaml, node)
 
     def _target_type(self) -> Type[UnparsedAnalysisUpdate]:
         return UnparsedAnalysisUpdate
 
 
-class MacroPatchParser(NonSourceParser[UnparsedMacroUpdate, ParsedMacroPatch]):
+class MacroPatchParser(PatchParser[UnparsedMacroUpdate, ParsedMacroPatch]):
     def get_block(self, node: UnparsedMacroUpdate) -> TargetBlock:
         return TargetBlock.from_yaml_block(self.yaml, node)
 
     def _target_type(self) -> Type[UnparsedMacroUpdate]:
         return UnparsedMacroUpdate
 
     def parse_patch(self, block: TargetBlock[UnparsedMacroUpdate], refs: ParserRef) -> None:
@@ -1222,263 +873,15 @@
         if not macro:
             warn_or_error(MacroNotFoundForPatch(patch_name=patch.name))
             return
         if macro.patch_path:
             package_name, existing_file_path = macro.patch_path.split("://")
             raise DuplicateMacroPatchNameError(patch, existing_file_path)
         source_file.macro_patches[patch.name] = unique_id
-        macro.patch(patch)
-
-
-class ExposureParser(YamlReader):
-    def __init__(self, schema_parser: SchemaParser, yaml: YamlBlock):
-        super().__init__(schema_parser, yaml, NodeType.Exposure.pluralize())
-        self.schema_parser = schema_parser
-        self.yaml = yaml
-
-    def parse_exposure(self, unparsed: UnparsedExposure):
-        package_name = self.project.project_name
-        unique_id = f"{NodeType.Exposure}.{package_name}.{unparsed.name}"
-        path = self.yaml.path.relative_path
-
-        fqn = self.schema_parser.get_fqn_prefix(path)
-        fqn.append(unparsed.name)
-
-        config = self._generate_exposure_config(
-            target=unparsed,
-            fqn=fqn,
-            package_name=package_name,
-            rendered=True,
-        )
-
-        config = config.finalize_and_validate()
-
-        unrendered_config = self._generate_exposure_config(
-            target=unparsed,
-            fqn=fqn,
-            package_name=package_name,
-            rendered=False,
-        )
-
-        if not isinstance(config, ExposureConfig):
-            raise DbtInternalError(
-                f"Calculated a {type(config)} for an exposure, but expected an ExposureConfig"
-            )
-
-        parsed = Exposure(
-            resource_type=NodeType.Exposure,
-            package_name=package_name,
-            path=path,
-            original_file_path=self.yaml.path.original_file_path,
-            unique_id=unique_id,
-            fqn=fqn,
-            name=unparsed.name,
-            type=unparsed.type,
-            url=unparsed.url,
-            meta=unparsed.meta,
-            tags=unparsed.tags,
-            description=unparsed.description,
-            label=unparsed.label,
-            owner=unparsed.owner,
-            maturity=unparsed.maturity,
-            config=config,
-            unrendered_config=unrendered_config,
-        )
-        ctx = generate_parse_exposure(
-            parsed,
-            self.root_project,
-            self.schema_parser.manifest,
-            package_name,
-        )
-        depends_on_jinja = "\n".join("{{ " + line + "}}" for line in unparsed.depends_on)
-        get_rendered(depends_on_jinja, ctx, parsed, capture_macros=True)
-        # parsed now has a populated refs/sources/metrics
-
-        if parsed.config.enabled:
-            self.manifest.add_exposure(self.yaml.file, parsed)
-        else:
-            self.manifest.add_disabled(self.yaml.file, parsed)
-
-    def _generate_exposure_config(
-        self, target: UnparsedExposure, fqn: List[str], package_name: str, rendered: bool
-    ):
-        generator: BaseContextConfigGenerator
-        if rendered:
-            generator = ContextConfigGenerator(self.root_project)
-        else:
-            generator = UnrenderedConfigGenerator(self.root_project)
-
-        # configs with precendence set
-        precedence_configs = dict()
-        # apply exposure configs
-        precedence_configs.update(target.config)
-
-        return generator.calculate_node_config(
-            config_call_dict={},
-            fqn=fqn,
-            resource_type=NodeType.Exposure,
-            project_name=package_name,
-            base=False,
-            patch_config_dict=precedence_configs,
-        )
-
-    def parse(self):
-        for data in self.get_key_dicts():
-            try:
-                UnparsedExposure.validate(data)
-                unparsed = UnparsedExposure.from_dict(data)
-            except (ValidationError, JSONValidationError) as exc:
-                raise YamlParseDictError(self.yaml.path, self.key, data, exc)
-
-            self.parse_exposure(unparsed)
-
-
-class MetricParser(YamlReader):
-    def __init__(self, schema_parser: SchemaParser, yaml: YamlBlock):
-        super().__init__(schema_parser, yaml, NodeType.Metric.pluralize())
-        self.schema_parser = schema_parser
-        self.yaml = yaml
-
-    def parse_metric(self, unparsed: UnparsedMetric):
-        package_name = self.project.project_name
-        unique_id = f"{NodeType.Metric}.{package_name}.{unparsed.name}"
-        path = self.yaml.path.relative_path
-
-        fqn = self.schema_parser.get_fqn_prefix(path)
-        fqn.append(unparsed.name)
-
-        config = self._generate_metric_config(
-            target=unparsed,
-            fqn=fqn,
-            package_name=package_name,
-            rendered=True,
-        )
-
-        config = config.finalize_and_validate()
-
-        unrendered_config = self._generate_metric_config(
-            target=unparsed,
-            fqn=fqn,
-            package_name=package_name,
-            rendered=False,
-        )
-
-        if not isinstance(config, MetricConfig):
-            raise DbtInternalError(
-                f"Calculated a {type(config)} for a metric, but expected a MetricConfig"
-            )
-
-        parsed = Metric(
-            resource_type=NodeType.Metric,
-            package_name=package_name,
-            path=path,
-            original_file_path=self.yaml.path.original_file_path,
-            unique_id=unique_id,
-            fqn=fqn,
-            model=unparsed.model,
-            name=unparsed.name,
-            description=unparsed.description,
-            label=unparsed.label,
-            calculation_method=unparsed.calculation_method,
-            expression=str(unparsed.expression),
-            timestamp=unparsed.timestamp,
-            dimensions=unparsed.dimensions,
-            window=unparsed.window,
-            time_grains=unparsed.time_grains,
-            filters=unparsed.filters,
-            meta=unparsed.meta,
-            tags=unparsed.tags,
-            config=config,
-            unrendered_config=unrendered_config,
-            group=config.group,
-        )
-
-        ctx = generate_parse_metrics(
-            parsed,
-            self.root_project,
-            self.schema_parser.manifest,
-            package_name,
-        )
-
-        if parsed.model is not None:
-            model_ref = "{{ " + parsed.model + " }}"
-            get_rendered(model_ref, ctx, parsed)
-
-        parsed.expression = get_rendered(
-            parsed.expression,
-            ctx,
-            node=parsed,
-        )
-
-        # if the metric is disabled we do not want it included in the manifest, only in the disabled dict
-        if parsed.config.enabled:
-            self.manifest.add_metric(self.yaml.file, parsed)
-        else:
-            self.manifest.add_disabled(self.yaml.file, parsed)
-
-    def _generate_metric_config(
-        self, target: UnparsedMetric, fqn: List[str], package_name: str, rendered: bool
-    ):
-        generator: BaseContextConfigGenerator
-        if rendered:
-            generator = ContextConfigGenerator(self.root_project)
-        else:
-            generator = UnrenderedConfigGenerator(self.root_project)
-
-        # configs with precendence set
-        precedence_configs = dict()
-        # first apply metric configs
-        precedence_configs.update(target.config)
-
-        config = generator.calculate_node_config(
-            config_call_dict={},
-            fqn=fqn,
-            resource_type=NodeType.Metric,
-            project_name=package_name,
-            base=False,
-            patch_config_dict=precedence_configs,
-        )
-        return config
-
-    def parse(self):
-        for data in self.get_key_dicts():
-            try:
-                UnparsedMetric.validate(data)
-                unparsed = UnparsedMetric.from_dict(data)
-
-            except (ValidationError, JSONValidationError) as exc:
-                raise YamlParseDictError(self.yaml.path, self.key, data, exc)
-            self.parse_metric(unparsed)
-
-
-class GroupParser(YamlReader):
-    def __init__(self, schema_parser: SchemaParser, yaml: YamlBlock):
-        super().__init__(schema_parser, yaml, NodeType.Group.pluralize())
-        self.schema_parser = schema_parser
-        self.yaml = yaml
-
-    def parse_group(self, unparsed: UnparsedGroup):
-        package_name = self.project.project_name
-        unique_id = f"{NodeType.Group}.{package_name}.{unparsed.name}"
-        path = self.yaml.path.relative_path
-
-        parsed = Group(
-            resource_type=NodeType.Group,
-            package_name=package_name,
-            path=path,
-            original_file_path=self.yaml.path.original_file_path,
-            unique_id=unique_id,
-            name=unparsed.name,
-            owner=unparsed.owner,
-        )
-
-        self.manifest.add_group(self.yaml.file, parsed)
-
-    def parse(self):
-        for data in self.get_key_dicts():
-            try:
-                UnparsedGroup.validate(data)
-                unparsed = UnparsedGroup.from_dict(data)
-            except (ValidationError, JSONValidationError) as exc:
-                raise YamlParseDictError(self.yaml.path, self.key, data, exc)
 
-            self.parse_group(unparsed)
+        # former macro.patch code
+        macro.patch_path = patch.file_id
+        macro.description = patch.description
+        macro.created_at = time.time()
+        macro.meta = patch.meta
+        macro.docs = patch.docs
+        macro.arguments = patch.arguments
```

### Comparing `dbt-core-1.6.0b1/dbt/parser/search.py` & `dbt-core-1.6.0b2/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/seeds.py` & `dbt-core-1.6.0b2/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/singular_test.py` & `dbt-core-1.6.0b2/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/snapshots.py` & `dbt-core-1.6.0b2/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/parser/sources.py` & `dbt-core-1.6.0b2/dbt/parser/sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     Time,
 )
 from dbt.events.functions import warn_or_error
 from dbt.events.types import UnusedTables
 from dbt.exceptions import DbtInternalError
 from dbt.node_types import NodeType
 
-from dbt.parser.schemas import SchemaParser, ParserRef
+from dbt.parser.common import ParserRef
+from dbt.parser.schema_generic_tests import SchemaGenericTestParser
 
 
 # An UnparsedSourceDefinition is taken directly from the yaml
 # file. It can affect multiple tables, all of which will eventually
 # have their own source node. An UnparsedSourceDefinition will
 # generate multiple UnpatchedSourceDefinition nodes (one per
 # table) in the SourceParser.add_source_definitions. The
@@ -44,15 +45,15 @@
     def __init__(
         self,
         root_project: RuntimeConfig,
         manifest: Manifest,
     ) -> None:
         self.root_project = root_project
         self.manifest = manifest
-        self.schema_parsers: Dict[str, SchemaParser] = {}
+        self.generic_test_parsers: Dict[str, SchemaGenericTestParser] = {}
         self.patches_used: Dict[SourceKey, Set[str]] = {}
         self.sources: Dict[str, SourceDefinition] = {}
 
     # This method calls the 'parse_source' method which takes
     # the UnpatchedSourceDefinitions in the manifest and combines them
     # with SourcePatches to produce SourceDefinitions.
     def construct_sources(self) -> None:
@@ -184,26 +185,26 @@
         )
 
         # relation name is added after instantiation because the adapter does
         # not provide the relation name for a UnpatchedSourceDefinition object
         parsed_source.relation_name = self._get_relation_name(parsed_source)
         return parsed_source
 
-    # This code uses the SchemaParser because it shares the '_parse_generic_test'
-    # code. It might be nice to separate out the generic test code
-    # and make it common to the schema parser and source patcher.
-    def get_schema_parser_for(self, package_name: str) -> "SchemaParser":
-        if package_name in self.schema_parsers:
-            schema_parser = self.schema_parsers[package_name]
+    # Use the SchemaGenericTestParser to parse the source tests
+    def get_generic_test_parser_for(self, package_name: str) -> "SchemaGenericTestParser":
+        if package_name in self.generic_test_parsers:
+            generic_test_parser = self.generic_test_parsers[package_name]
         else:
             all_projects = self.root_project.load_dependencies()
             project = all_projects[package_name]
-            schema_parser = SchemaParser(project, self.manifest, self.root_project)
-            self.schema_parsers[package_name] = schema_parser
-        return schema_parser
+            generic_test_parser = SchemaGenericTestParser(
+                project, self.manifest, self.root_project
+            )
+            self.generic_test_parsers[package_name] = generic_test_parser
+        return generic_test_parser
 
     def get_source_tests(self, target: UnpatchedSourceDefinition) -> Iterable[GenericTestNode]:
         for test, column in target.get_tests():
             yield self.parse_source_test(
                 target=target,
                 test=test,
                 column=column,
@@ -222,15 +223,15 @@
         if key not in self.patches_used:
             # mark the key as used
             self.patches_used[key] = set()
         if patch.get_table_named(unpatched.table.name) is not None:
             self.patches_used[key].add(unpatched.table.name)
         return patch
 
-    # This calls _parse_generic_test in the SchemaParser
+    # This calls parse_generic_test in the SchemaGenericTestParser
     def parse_source_test(
         self,
         target: UnpatchedSourceDefinition,
         test: Dict[str, Any],
         column: Optional[UnparsedColumn],
     ) -> GenericTestNode:
         column_name: Optional[str]
@@ -243,18 +244,16 @@
                 column_name = get_adapter(self.root_project).quote(column_name)
 
         tags_sources = [target.source.tags, target.table.tags]
         if column is not None:
             tags_sources.append(column.tags)
         tags = list(itertools.chain.from_iterable(tags_sources))
 
-        # TODO: make the generic_test code common so we don't need to
-        # create schema parsers to handle the tests
-        schema_parser = self.get_schema_parser_for(target.package_name)
-        node = schema_parser._parse_generic_test(
+        generic_test_parser = self.get_generic_test_parser_for(target.package_name)
+        node = generic_test_parser.parse_generic_test(
             target=target,
             test=test,
             tags=tags,
             column_name=column_name,
             schema_file_id=target.file_id,
             version=None,
         )
```

### Comparing `dbt-core-1.6.0b1/dbt/parser/sql.py` & `dbt-core-1.6.0b2/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/semver.py` & `dbt-core-1.6.0b2/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/base.py` & `dbt-core-1.6.0b2/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/build.py` & `dbt-core-1.6.0b2/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/clean.py` & `dbt-core-1.6.0b2/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/compile.py` & `dbt-core-1.6.0b2/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/debug.py` & `dbt-core-1.6.0b2/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/deps.py` & `dbt-core-1.6.0b2/dbt/task/deps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, Optional
-
+from pathlib import Path
 import dbt.utils
 import dbt.deprecations
 import dbt.exceptions
 
 from dbt.config.renderer import DbtProjectYamlRenderer
 from dbt.deps.base import downloads_directory
 from dbt.deps.resolver import resolve_packages
@@ -25,14 +25,20 @@
 from dbt.task.base import BaseTask, move_to_nearest_project_dir
 
 from dbt.config import Project
 
 
 class DepsTask(BaseTask):
     def __init__(self, args: Any, project: Project):
+        # N.B. This is a temporary fix for a bug when using relative paths via
+        # --project-dir with deps.  A larger overhaul of our path handling methods
+        # is needed to fix this the "right" way.
+        # See GH-7615
+        project.project_root = str(Path(project.project_root).resolve())
+
         move_to_nearest_project_dir(project.project_root)
         super().__init__(args=args, config=None, project=project)
         self.cli_vars = args.vars
 
     def track_package_install(
         self, package_name: str, source_type: str, version: Optional[str]
     ) -> None:
```

### Comparing `dbt-core-1.6.0b1/dbt/task/freshness.py` & `dbt-core-1.6.0b2/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/generate.py` & `dbt-core-1.6.0b2/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/init.py` & `dbt-core-1.6.0b2/dbt/task/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import copy
 import os
 from pathlib import Path
 import re
 import shutil
-import sys
 from typing import Optional
 
 import yaml
 import click
 
 import dbt.config
 import dbt.clients.system
@@ -141,25 +140,25 @@
         return dbt_project["profile"]
 
     def write_profile(self, profile: dict, profile_name: str):
         """Given a profile, write it to the current project's profiles.yml.
         This will overwrite any profile with a matching name."""
         # Create the profile directory if it doesn't exist
         profiles_filepath = Path(get_flags().PROFILES_DIR) / Path("profiles.yml")
+
+        profiles = {profile_name: profile}
+
         if profiles_filepath.exists():
-            with open(profiles_filepath, "r+") as f:
+            with open(profiles_filepath, "r") as f:
                 profiles = yaml.safe_load(f) or {}
                 profiles[profile_name] = profile
-                f.seek(0)
-                yaml.dump(profiles, f)
-                f.truncate()
-        else:
-            profiles = {profile_name: profile}
-            with open(profiles_filepath, "w") as f:
-                yaml.dump(profiles, f)
+
+        # Write the profiles dictionary to a brand-new or pre-existing file
+        with open(profiles_filepath, "w") as f:
+            yaml.dump(profiles, f)
 
     def create_profile_from_profile_template(self, profile_template: dict, profile_name: str):
         """Create and write a profile using the supplied profile_template."""
         initial_target = profile_template.get("fixed", {})
         prompts = profile_template.get("prompts", {})
         target = self.generate_target_from_input(prompts, initial_target)
         target_name = target.pop("target", "dev")
@@ -217,14 +216,18 @@
         fire_event(
             ProfileWrittenWithProjectTemplateYAML(name=profile_name, path=str(profiles_filepath))
         )
 
     def ask_for_adapter_choice(self) -> str:
         """Ask the user which adapter (database) they'd like to use."""
         available_adapters = list(_get_adapter_plugin_names())
+
+        if not available_adapters:
+            raise dbt.exceptions.NoAdaptersAvailableError()
+
         prompt_msg = (
             "Which database would you like to use?\n"
             + "\n".join([f"[{n+1}] {v}" for n, v in enumerate(available_adapters)])
             + "\n\n(Don't see the one you want? https://docs.getdbt.com/docs/available-adapters)"
             + "\n\nEnter a number"
         )
         numeric_choice = click.prompt(prompt_msg, type=click.INT)
@@ -240,30 +243,58 @@
         while not ProjectName.is_valid(name) or name in internal_package_names:
             if name:
                 click.echo(name + " is not a valid project name.")
             name = click.prompt("Enter a name for your project (letters, digits, underscore)")
 
         return name
 
+    def create_new_project(self, project_name: str):
+        self.copy_starter_repo(project_name)
+        os.chdir(project_name)
+        with open("dbt_project.yml", "r") as f:
+            content = f"{f.read()}".format(project_name=project_name, profile_name=project_name)
+        with open("dbt_project.yml", "w") as f:
+            f.write(content)
+        fire_event(
+            ProjectCreated(
+                project_name=project_name,
+                docs_url=DOCS_URL,
+                slack_url=SLACK_URL,
+            )
+        )
+
     def run(self):
         """Entry point for the init task."""
         profiles_dir = get_flags().PROFILES_DIR
         self.create_profiles_dir(profiles_dir)
 
         try:
             move_to_nearest_project_dir(self.args.project_dir)
             in_project = True
         except dbt.exceptions.DbtRuntimeError:
             in_project = False
 
         if in_project:
             # When dbt init is run inside an existing project,
             # just setup the user's profile.
-            fire_event(SettingUpProfile())
             profile_name = self.get_profile_name_from_current_project()
+        else:
+            # When dbt init is run outside of an existing project,
+            # create a new project and set up the user's profile.
+            project_name = self.get_valid_project_name()
+            project_path = Path(project_name)
+            if project_path.exists():
+                fire_event(ProjectNameAlreadyExists(name=project_name))
+                return
+            self.create_new_project(project_name)
+            profile_name = project_name
+
+        # Ask for adapter only if skip_profile_setup flag is not provided.
+        if not self.args.skip_profile_setup:
+            fire_event(SettingUpProfile())
             if not self.check_if_can_write_profile(profile_name=profile_name):
                 return
             # If a profile_template.yml exists in the project root, that effectively
             # overrides the profile_template.yml for the given target.
             profile_template_path = Path("profile_template.yml")
             if profile_template_path.exists():
                 try:
@@ -271,42 +302,7 @@
                     # so use a try: except to fall back to the default on failure
                     self.create_profile_using_project_profile_template(profile_name)
                     return
                 except Exception:
                     fire_event(InvalidProfileTemplateYAML())
             adapter = self.ask_for_adapter_choice()
             self.create_profile_from_target(adapter, profile_name=profile_name)
-            return
-
-        # When dbt init is run outside of an existing project,
-        # create a new project and set up the user's profile.
-        available_adapters = list(_get_adapter_plugin_names())
-        if not len(available_adapters):
-            print("No adapters available. Go to https://docs.getdbt.com/docs/available-adapters")
-            sys.exit(1)
-        project_name = self.get_valid_project_name()
-        project_path = Path(project_name)
-        if project_path.exists():
-            fire_event(ProjectNameAlreadyExists(name=project_name))
-            return
-
-        self.copy_starter_repo(project_name)
-        os.chdir(project_name)
-        with open("dbt_project.yml", "r+") as f:
-            content = f"{f.read()}".format(project_name=project_name, profile_name=project_name)
-            f.seek(0)
-            f.write(content)
-            f.truncate()
-
-        # Ask for adapter only if skip_profile_setup flag is not provided.
-        if not self.args.skip_profile_setup:
-            if not self.check_if_can_write_profile(profile_name=project_name):
-                return
-            adapter = self.ask_for_adapter_choice()
-            self.create_profile_from_target(adapter, profile_name=project_name)
-            fire_event(
-                ProjectCreated(
-                    project_name=project_name,
-                    docs_url=DOCS_URL,
-                    slack_url=SLACK_URL,
-                )
-            )
```

### Comparing `dbt-core-1.6.0b1/dbt/task/list.py` & `dbt-core-1.6.0b2/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/printer.py` & `dbt-core-1.6.0b2/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/run.py` & `dbt-core-1.6.0b2/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/run_operation.py` & `dbt-core-1.6.0b2/dbt/task/run_operation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from datetime import datetime
+import os
+import threading
 import traceback
+from datetime import datetime
 
 import agate
 
-from .base import ConfiguredTask
-
 import dbt.exceptions
 from dbt.adapters.factory import get_adapter
-from dbt.contracts.results import RunOperationResultsArtifact
+from dbt.contracts.files import FileHash
+from dbt.contracts.graph.nodes import HookNode
+from dbt.contracts.results import RunResultsArtifact, RunResult, RunStatus, TimingInfo
 from dbt.events.functions import fire_event
 from dbt.events.types import (
     RunningOperationCaughtError,
     RunningOperationUncaughtError,
     LogDebugStackTrace,
 )
+from dbt.node_types import NodeType
+from dbt.task.base import ConfiguredTask
+
+RESULT_FILE_NAME = "run_results.json"
 
 
 class RunOperationTask(ConfiguredTask):
     def _get_macro_parts(self):
         macro_name = self.args.macro
         if "." in macro_name:
             package_name, macro_name = macro_name.split(".", 1)
         else:
-            package_name = None
+            package_name = self.config.project_name
 
         return package_name, macro_name
 
     def _run_unsafe(self) -> agate.Table:
         adapter = get_adapter(self.config)
 
         package_name, macro_name = self._get_macro_parts()
@@ -36,15 +42,15 @@
             adapter.clear_transaction()
             res = adapter.execute_macro(
                 macro_name, project=package_name, kwargs=macro_kwargs, manifest=self.manifest
             )
 
         return res
 
-    def run(self) -> RunOperationResultsArtifact:
+    def run(self) -> RunResultsArtifact:
         start = datetime.utcnow()
         self.compile_manifest()
         try:
             self._run_unsafe()
         except dbt.exceptions.Exception as exc:
             fire_event(RunningOperationCaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
@@ -52,15 +58,55 @@
         except Exception as exc:
             fire_event(RunningOperationUncaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
             success = False
         else:
             success = True
         end = datetime.utcnow()
-        return RunOperationResultsArtifact.from_success(
+
+        package_name, macro_name = self._get_macro_parts()
+        fqn = [NodeType.Operation, package_name, macro_name]
+        unique_id = ".".join(fqn)
+
+        run_result = RunResult(
+            adapter_response={},
+            status=RunStatus.Success if success else RunStatus.Error,
+            execution_time=(end - start).total_seconds(),
+            failures=0 if success else 1,
+            message=None,
+            node=HookNode(
+                alias=macro_name,
+                checksum=FileHash.from_contents(unique_id),
+                database=self.config.credentials.database,
+                schema=self.config.credentials.schema,
+                resource_type=NodeType.Operation,
+                fqn=fqn,
+                name=macro_name,
+                unique_id=unique_id,
+                package_name=package_name,
+                path="",
+                original_file_path="",
+            ),
+            thread_id=threading.current_thread().name,
+            timing=[TimingInfo(name=macro_name, started_at=start, completed_at=end)],
+        )
+
+        results = RunResultsArtifact.from_execution_results(
             generated_at=end,
             elapsed_time=(end - start).total_seconds(),
-            success=success,
+            args={
+                k: v
+                for k, v in self.args.__dict__.items()
+                if k.islower() and type(v) in (str, int, float, bool, list, dict)
+            },
+            results=[run_result],
         )
 
+        result_path = os.path.join(self.config.target_path, RESULT_FILE_NAME)
+
+        if self.args.write_json:
+            results.write(result_path)
+
+        return results
+
     def interpret_results(self, results):
-        return results.success
+        return results.results[0].status == RunStatus.Success
```

### Comparing `dbt-core-1.6.0b1/dbt/task/runnable.py` & `dbt-core-1.6.0b2/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/seed.py` & `dbt-core-1.6.0b2/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/serve.py` & `dbt-core-1.6.0b2/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/show.py` & `dbt-core-1.6.0b2/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/snapshot.py` & `dbt-core-1.6.0b2/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/sql.py` & `dbt-core-1.6.0b2/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/task/test.py` & `dbt-core-1.6.0b2/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0b2/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/tests/util.py` & `dbt-core-1.6.0b2/dbt/tests/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     fire_event,
     capture_stdout_logs,
     stop_capture_stdout_logs,
     reset_metadata_vars,
 )
 from dbt.events.base_types import EventLevel
 from dbt.events.types import Note
+from dbt.contracts.publication import PublicationArtifact
 
 
 # =============================================================================
 # Test utilities
 #   run_dbt
 #   run_dbt_and_capture
 #   get_manifest
@@ -65,15 +66,19 @@
 # different objects depending on the command that is executed.
 # For a run command (and most other commands) it will return a list
 # of results. For the 'docs generate' command it returns a CatalogArtifact.
 # The first parameter is a list of dbt command line arguments, such as
 #   run_dbt(["run", "--vars", "seed_name: base"])
 # If the command is expected to fail, pass in "expect_pass=False"):
 #   run_dbt("test"], expect_pass=False)
-def run_dbt(args: List[str] = None, expect_pass=True):
+def run_dbt(
+    args: List[str] = None,
+    expect_pass: bool = True,
+    publications: List[PublicationArtifact] = None,
+):
     # Ignore logbook warnings
     warnings.filterwarnings("ignore", category=DeprecationWarning, module="logbook")
 
     # reset global vars
     reset_metadata_vars()
 
     # The logger will complain about already being initialized if
@@ -90,15 +95,15 @@
     profiles_dir = getattr(flags, "PROFILES_DIR", None)
     if project_dir and "--project-dir" not in args:
         args.extend(["--project-dir", project_dir])
     if profiles_dir and "--profiles-dir" not in args:
         args.extend(["--profiles-dir", profiles_dir])
 
     dbt = dbtRunner()
-    res = dbt.invoke(args)
+    res = dbt.invoke(args, publications=publications)
 
     # the exception is immediately raised to be caught in tests
     # using a pattern like `with pytest.raises(SomeException):`
     if res.exception is not None:
         raise res.exception
 
     if expect_pass is not None:
@@ -107,32 +112,47 @@
     return res.result
 
 
 # Use this if you need to capture the command logs in a test.
 # If you want the logs that are normally written to a file, you must
 # start with the "--debug" flag. The structured schema log CI test
 # will turn the logs into json, so you have to be prepared for that.
-def run_dbt_and_capture(args: List[str] = None, expect_pass=True):
+def run_dbt_and_capture(
+    args: List[str] = None,
+    expect_pass: bool = True,
+    publications: List[PublicationArtifact] = None,
+):
     try:
         stringbuf = StringIO()
         capture_stdout_logs(stringbuf)
-        res = run_dbt(args, expect_pass=expect_pass)
+        res = run_dbt(args, expect_pass=expect_pass, publications=publications)
         stdout = stringbuf.getvalue()
 
     finally:
         stop_capture_stdout_logs()
 
-    # Json logs will have lots of escape characters which will
-    # make checks for strings in the logs fail, so remove those.
-    if '{"code":' in stdout:
-        stdout = stdout.replace("\\", "")
-
     return res, stdout
 
 
+def get_logging_events(log_output, event_name):
+    logging_events = []
+    for log_line in log_output.split("\n"):
+        # skip empty lines
+        if len(log_line) == 0:
+            continue
+        # The adapter logging also shows up, so skip non-json lines
+        if not log_line.startswith("{"):
+            continue
+        if event_name in log_line:
+            log_dct = json.loads(log_line)
+            if log_dct["info"]["name"] == event_name:
+                logging_events.append(log_dct)
+    return logging_events
+
+
 # Used in test cases to get the manifest from the partial parsing file
 # Note: this uses an internal version of the manifest, and in the future
 # parts of it will not be supported for external use.
 def get_manifest(project_root):
     path = os.path.join(project_root, "target", "partial_parse.msgpack")
     if os.path.exists(path):
         with open(path, "rb") as fp:
```

### Comparing `dbt-core-1.6.0b1/dbt/tracking.py` & `dbt-core-1.6.0b2/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/ui.py` & `dbt-core-1.6.0b2/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b1/dbt/utils.py` & `dbt-core-1.6.0b2/dbt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
 
 def _deep_map_render(
     func: Callable[[Any, Tuple[Union[str, int], ...]], Any],
     value: Any,
     keypath: Tuple[Union[str, int], ...],
 ) -> Any:
-    atomic_types: Tuple[Type[Any], ...] = (int, float, str, type(None), bool)
+    atomic_types: Tuple[Type[Any], ...] = (int, float, str, type(None), bool, datetime.date)
 
     ret: Any
 
     if isinstance(value, list):
         ret = [_deep_map_render(func, v, (keypath + (idx,))) for idx, v in enumerate(value)]
     elif isinstance(value, dict):
         ret = {k: _deep_map_render(func, v, (keypath + (str(k),))) for k, v in value.items()}
```

### Comparing `dbt-core-1.6.0b1/dbt/version.py` & `dbt-core-1.6.0b2/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b1/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0b2/dbt_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b1/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0b2/dbt_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 dbt/cli/flags.py
 dbt/cli/main.py
 dbt/cli/option_types.py
 dbt/cli/options.py
 dbt/cli/params.py
 dbt/cli/requires.py
 dbt/cli/resolvers.py
+dbt/cli/types.py
 dbt/clients/__init__.py
 dbt/clients/_jinja_blocks.py
 dbt/clients/agate_helper.py
 dbt/clients/git.py
 dbt/clients/jinja.py
 dbt/clients/jinja_static.py
 dbt/clients/registry.py
@@ -125,14 +126,15 @@
 dbt/include/README.md
 dbt/include/index.html
 dbt/include/global_project/__init__.py
 dbt/include/global_project/dbt_project.yml
 dbt/include/global_project/docs/overview.md
 dbt/include/global_project/macros/adapters/apply_grants.sql
 dbt/include/global_project/macros/adapters/columns.sql
+dbt/include/global_project/macros/adapters/drop_relation.sql
 dbt/include/global_project/macros/adapters/freshness.sql
 dbt/include/global_project/macros/adapters/indexes.sql
 dbt/include/global_project/macros/adapters/metadata.sql
 dbt/include/global_project/macros/adapters/persist_docs.sql
 dbt/include/global_project/macros/adapters/relation.sql
 dbt/include/global_project/macros/adapters/schema.sql
 dbt/include/global_project/macros/adapters/timestamps.sql
@@ -206,24 +208,27 @@
 dbt/include/starter_project/models/example/schema.yml
 dbt/include/starter_project/seeds/.gitkeep
 dbt/include/starter_project/snapshots/.gitkeep
 dbt/include/starter_project/tests/.gitkeep
 dbt/parser/__init__.py
 dbt/parser/analysis.py
 dbt/parser/base.py
+dbt/parser/common.py
 dbt/parser/docs.py
 dbt/parser/generic_test.py
 dbt/parser/generic_test_builders.py
 dbt/parser/hooks.py
 dbt/parser/macros.py
 dbt/parser/manifest.py
 dbt/parser/models.py
 dbt/parser/partial.py
 dbt/parser/read_files.py
+dbt/parser/schema_generic_tests.py
 dbt/parser/schema_renderer.py
+dbt/parser/schema_yaml_readers.py
 dbt/parser/schemas.py
 dbt/parser/search.py
 dbt/parser/seeds.py
 dbt/parser/singular_test.py
 dbt/parser/snapshots.py
 dbt/parser/sources.py
 dbt/parser/sql.py
```

### Comparing `dbt-core-1.6.0b1/setup.py` & `dbt-core-1.6.0b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0b1"
+package_version = "1.6.0b2"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -65,15 +65,15 @@
         "pathspec>=0.9,<0.12",
         "protobuf>=4.0.0",
         "pytz>=2015.7",
         # the following are all to match snowflake-connector-python
         "requests<3.0.0",
         "idna>=2.5,<4",
         "cffi>=1.9,<2.0.0",
-        "pyyaml>=6.0",
+        "pyyaml>=5.3",
         "urllib3~=1.0",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
```

