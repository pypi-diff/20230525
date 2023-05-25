# Comparing `tmp/dcicsnovault-8.0.1.5b15.tar.gz` & `tmp/dcicsnovault-8.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.5b15.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.2b0.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.5b15.tar` & `dcicsnovault-8.0.2b0.tar`

### file list

```diff
@@ -1,163 +1,123 @@
--rw-r--r--   0        0        0     1135 2023-05-25 20:04:54.359383 dcicsnovault-8.0.1.5b15/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-05-25 20:04:54.359383 dcicsnovault-8.0.1.5b15/README.rst
--rw-r--r--   0        0        0     5293 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/pyproject.toml
--rw-r--r--   0        0        0     4907 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/aggregated_items.py
--rw-r--r--   0        0        0     9389 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/app.py
--rw-r--r--   0        0        0      358 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/attachment.py
--rw-r--r--   0        0        0    25502 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6876 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-05-25 20:04:54.363383 dcicsnovault-8.0.1.5b15/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5796 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/custom_embed.py
--rw-r--r--   0        0        0     7257 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30434 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/predicates.py
--rw-r--r--   0        0        0      289 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/project_defs.py
--rw-r--r--   0        0        0       95 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/resource_views.py
--rw-r--r--   0        0        0    24112 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/root.py
--rw-r--r--   0        0        0      986 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schema_graph.py
--rw-r--r--   0        0        0    14547 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-05-25 20:04:54.367384 dcicsnovault-8.0.1.5b15/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/search/search.py
--rw-r--r--   0        0        0    17915 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4443 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2433 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3186 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_util.py
--rw-r--r--   0        0        0    19246 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4620 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-05-25 20:04:54.371384 dcicsnovault-8.0.1.5b15/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5583 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/upgrader.py
--rw-r--r--   0        0        0    52343 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-05-25 20:04:54.375384 dcicsnovault-8.0.1.5b15/snovault/validators.py
--rw-r--r--   0        0        0     9195 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.5b15/PKG-INFO
+-rw-r--r--   0        0        0     1135 2021-08-05 13:09:50.965406 dcicsnovault-8.0.2b0/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2022-03-28 12:18:05.921263 dcicsnovault-8.0.2b0/README.rst
+-rw-r--r--   0        0        0     5558 2023-05-17 20:40:36.815687 dcicsnovault-8.0.2b0/pyproject.toml
+-rw-r--r--   0        0        0     4460 2023-05-17 19:23:12.027395 dcicsnovault-8.0.2b0/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2022-12-06 18:39:28.758670 dcicsnovault-8.0.2b0/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-05-17 19:23:12.027670 dcicsnovault-8.0.2b0/snovault/app.py
+-rw-r--r--   0        0        0    11879 2022-08-26 18:02:01.685022 dcicsnovault-8.0.2b0/snovault/attachment.py
+-rw-r--r--   0        0        0     6670 2022-12-06 18:39:28.759399 dcicsnovault-8.0.2b0/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2021-08-05 13:09:50.971424 dcicsnovault-8.0.2b0/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2021-08-05 13:09:50.971503 dcicsnovault-8.0.2b0/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2021-08-05 13:09:50.971588 dcicsnovault-8.0.2b0/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2021-08-05 13:09:50.971661 dcicsnovault-8.0.2b0/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     1608 2022-08-26 18:02:01.685403 dcicsnovault-8.0.2b0/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2021-08-05 13:09:50.971801 dcicsnovault-8.0.2b0/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     4350 2022-12-06 18:39:28.759780 dcicsnovault-8.0.2b0/snovault/commands/profile.py
+-rw-r--r--   0        0        0      909 2022-12-06 18:39:28.760010 dcicsnovault-8.0.2b0/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2022-12-06 18:39:28.760248 dcicsnovault-8.0.2b0/snovault/config.py
+-rw-r--r--   0        0        0     6352 2022-12-06 18:39:28.760508 dcicsnovault-8.0.2b0/snovault/connection.py
+-rw-r--r--   0        0        0    14815 2022-08-26 18:02:01.685826 dcicsnovault-8.0.2b0/snovault/crud_views.py
+-rw-r--r--   0        0        0     4282 2022-12-06 18:39:28.760742 dcicsnovault-8.0.2b0/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2022-12-06 18:39:28.760964 dcicsnovault-8.0.2b0/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-05 17:21:01.470795 dcicsnovault-8.0.2b0/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2022-12-06 18:39:28.761673 dcicsnovault-8.0.2b0/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2022-12-06 18:39:28.761963 dcicsnovault-8.0.2b0/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-05-17 19:23:12.028113 dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-01-26 21:38:09.491537 dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2022-12-06 18:39:28.762984 dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2021-08-05 13:09:50.973270 dcicsnovault-8.0.2b0/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-05-17 19:23:12.028378 dcicsnovault-8.0.2b0/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8872 2023-05-17 20:33:55.773106 dcicsnovault-8.0.2b0/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2022-12-06 18:39:28.763658 dcicsnovault-8.0.2b0/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2022-12-06 18:39:28.763921 dcicsnovault-8.0.2b0/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2021-08-05 13:09:50.973711 dcicsnovault-8.0.2b0/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-01-26 21:38:09.491890 dcicsnovault-8.0.2b0/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2022-04-05 14:53:03.078388 dcicsnovault-8.0.2b0/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2021-08-05 13:09:50.973908 dcicsnovault-8.0.2b0/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2022-12-06 18:39:28.764413 dcicsnovault-8.0.2b0/snovault/jsonld_context.py
+-rw-r--r--   0        0        0      846 2021-08-05 13:09:50.974063 dcicsnovault-8.0.2b0/snovault/predicates.py
+-rw-r--r--   0        0        0       95 2023-05-17 19:23:12.028559 dcicsnovault-8.0.2b0/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-05-17 19:23:12.028650 dcicsnovault-8.0.2b0/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-17 19:23:12.028740 dcicsnovault-8.0.2b0/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-05-17 19:23:12.028871 dcicsnovault-8.0.2b0/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0     6495 2022-12-06 18:39:28.764720 dcicsnovault-8.0.2b0/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2022-06-08 15:58:38.024771 dcicsnovault-8.0.2b0/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-05-17 19:23:12.029164 dcicsnovault-8.0.2b0/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2022-12-06 18:39:28.765415 dcicsnovault-8.0.2b0/snovault/schema_graph.py
+-rw-r--r--   0        0        0    16947 2022-12-06 18:39:28.766426 dcicsnovault-8.0.2b0/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4359 2021-08-05 13:09:50.974634 dcicsnovault-8.0.2b0/snovault/schema_views.py
+-rw-r--r--   0        0        0      522 2022-12-06 18:39:28.766731 dcicsnovault-8.0.2b0/snovault/settings.py
+-rw-r--r--   0        0        0     1498 2021-08-05 13:09:50.974777 dcicsnovault-8.0.2b0/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2022-12-06 18:39:28.766993 dcicsnovault-8.0.2b0/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-05-17 19:23:12.029649 dcicsnovault-8.0.2b0/snovault/storage.py
+-rw-r--r--   0        0        0      330 2021-08-05 13:09:50.975120 dcicsnovault-8.0.2b0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2021-08-05 13:09:50.975172 dcicsnovault-8.0.2b0/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2022-06-29 20:41:05.272414 dcicsnovault-8.0.2b0/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2021-08-05 13:09:50.975307 dcicsnovault-8.0.2b0/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2021-08-05 13:09:50.975360 dcicsnovault-8.0.2b0/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2021-08-05 13:09:50.975421 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2022-08-26 18:02:01.687677 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2021-08-05 13:09:50.975544 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2021-08-05 13:09:50.975602 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2021-08-05 13:09:50.975660 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      577 2021-08-05 13:09:50.975746 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2021-08-05 13:09:50.975798 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2021-08-05 13:09:50.975856 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2021-08-05 13:09:50.975920 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2021-08-05 13:09:50.975980 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2021-08-05 13:09:50.976042 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2021-08-05 13:09:50.976101 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2021-08-05 13:09:50.976163 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2022-08-26 18:02:01.687799 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2021-08-05 13:09:50.976215 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2021-08-05 13:09:50.976301 dcicsnovault-8.0.2b0/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0      417 2021-08-05 13:09:50.976361 dcicsnovault-8.0.2b0/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2022-12-06 18:39:28.767548 dcicsnovault-8.0.2b0/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     9899 2022-12-06 18:39:28.768136 dcicsnovault-8.0.2b0/snovault/tests/authentication.py
+-rw-r--r--   0        0        0     2068 2021-08-05 13:09:50.976620 dcicsnovault-8.0.2b0/snovault/tests/authorization.py
+-rw-r--r--   0        0        0     2210 2023-05-17 19:23:12.029857 dcicsnovault-8.0.2b0/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2022-09-08 15:16:00.868058 dcicsnovault-8.0.2b0/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0     3086 2022-12-06 18:39:28.768761 dcicsnovault-8.0.2b0/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2021-08-05 13:09:50.976822 dcicsnovault-8.0.2b0/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-05-17 19:23:12.030021 dcicsnovault-8.0.2b0/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2021-08-05 13:09:50.976953 dcicsnovault-8.0.2b0/snovault/tests/root.py
+-rw-r--r--   0        0        0    59212 2022-12-06 18:39:28.769247 dcicsnovault-8.0.2b0/snovault/tests/search.py
+-rw-r--r--   0        0        0    17312 2023-05-17 19:23:12.030264 dcicsnovault-8.0.2b0/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0     1857 2021-08-05 13:09:50.977413 dcicsnovault-8.0.2b0/snovault/tests/snowflake_hash.py
+-rw-r--r--   0        0        0    20332 2023-05-17 19:23:12.030525 dcicsnovault-8.0.2b0/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3932 2021-08-05 13:09:50.977571 dcicsnovault-8.0.2b0/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2021-08-05 13:09:50.977633 dcicsnovault-8.0.2b0/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0     8984 2022-12-06 18:39:28.769899 dcicsnovault-8.0.2b0/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     7458 2023-04-05 17:21:01.472227 dcicsnovault-8.0.2b0/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-04-05 17:21:01.472528 dcicsnovault-8.0.2b0/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2021-08-05 13:09:50.977969 dcicsnovault-8.0.2b0/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0    97622 2023-05-17 19:23:12.031394 dcicsnovault-8.0.2b0/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2022-12-06 18:39:28.771473 dcicsnovault-8.0.2b0/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     2147 2023-04-05 17:21:01.473341 dcicsnovault-8.0.2b0/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2021-08-05 13:09:50.978588 dcicsnovault-8.0.2b0/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2022-12-06 18:39:28.771707 dcicsnovault-8.0.2b0/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-04-05 17:21:01.473556 dcicsnovault-8.0.2b0/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2021-08-05 13:09:50.978758 dcicsnovault-8.0.2b0/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2022-12-06 18:39:28.772371 dcicsnovault-8.0.2b0/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2022-12-06 18:39:28.772542 dcicsnovault-8.0.2b0/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2021-08-05 13:09:50.979031 dcicsnovault-8.0.2b0/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2022-12-06 18:39:28.772775 dcicsnovault-8.0.2b0/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0      484 2021-08-05 13:09:50.979169 dcicsnovault-8.0.2b0/snovault/tests/test_snowflake_hash.py
+-rw-r--r--   0        0        0     4267 2021-08-05 13:09:50.979237 dcicsnovault-8.0.2b0/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2022-12-06 18:39:28.772892 dcicsnovault-8.0.2b0/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-05-17 19:23:12.031621 dcicsnovault-8.0.2b0/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     1291 2021-08-05 13:09:50.979377 dcicsnovault-8.0.2b0/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2022-12-06 18:39:28.773485 dcicsnovault-8.0.2b0/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2022-12-06 18:39:28.773758 dcicsnovault-8.0.2b0/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4621 2022-06-08 15:58:38.027027 dcicsnovault-8.0.2b0/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      688 2021-08-05 13:09:50.979699 dcicsnovault-8.0.2b0/snovault/tests/testing_key.py
+-rw-r--r--   0        0        0      677 2021-08-05 13:09:50.979756 dcicsnovault-8.0.2b0/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    26232 2022-12-06 18:39:28.774184 dcicsnovault-8.0.2b0/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2021-08-05 13:09:50.979967 dcicsnovault-8.0.2b0/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-05 17:21:01.473937 dcicsnovault-8.0.2b0/snovault/tools.py
+-rw-r--r--   0        0        0     7605 2021-08-05 13:09:50.980043 dcicsnovault-8.0.2b0/snovault/typeinfo.py
+-rw-r--r--   0        0        0     8124 2023-04-05 17:21:01.474208 dcicsnovault-8.0.2b0/snovault/upgrader.py
+-rw-r--r--   0        0        0    45963 2023-04-05 17:21:01.474588 dcicsnovault-8.0.2b0/snovault/util.py
+-rw-r--r--   0        0        0     5460 2022-12-06 18:39:28.774411 dcicsnovault-8.0.2b0/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2022-12-06 18:39:28.774627 dcicsnovault-8.0.2b0/snovault/validators.py
+-rw-r--r--   0        0        0     9044 1970-01-01 00:00:00.000000 dcicsnovault-8.0.2b0/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.5b15/LICENSE.txt` & `dcicsnovault-8.0.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/README.rst` & `dcicsnovault-8.0.2b0/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/pyproject.toml` & `dcicsnovault-8.0.2b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.5b15"  # to become 8.1.0
+version = "8.0.2b0"
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -19,56 +19,56 @@
     'Development Status :: 4 - Beta',
 
     # Indicate who your project is intended for
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Framework :: Pyramid',
 
+
     # Pick your license as you wish (should match "license" above)
     'License :: OSI Approved :: MIT License',
     'Topic :: Database :: Database Engines/Servers',
 
     # Specify the Python versions you support here. In particular, ensure
     # that you indicate whether you support Python 2, Python 3 or both.
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.10"
+python = ">=3.8.1,<3.9"
 aws_requests_auth = "^0.4.1"
-boto3 = "^1.26.124"  # no particular version required, but this speeds up search
-botocore = "^1.19.124"  # no particular version required, but this speeds up search
+# TODO: This is a backport of Python's statistics library for versions earlier than Python 3.4,
+#       so may no longer be needed. Something to investigate later. -kmp 20-Feb-2020
+# "backports.statistics" = "0.1.0"
+botocore = ">=1.27.36"  # no particular version required, but this speeds up search
+boto3 = ">=1.24.36"  # no particular version required, but this speeds up search
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
 elasticsearch_dsl = "^7.4.0"
-dcicutils = "7.4.4.5b21"  # "^7.0.0"
+dcicutils = "^7.0.0"
 future = ">=0.15.2,<1"
 html5lib = ">=1.1"  # experimental, should be OK now that we're not using moto server
 humanfriendly = "^1.44.9"
 jsonschema_serialize_fork = "^2.1.1"
 netaddr = ">=0.8.0,<1"
 passlib = "^1.7.4"
-pillow = "^9.5.0"
 psutil = "^5.9.0"
 psycopg2-binary = "^2.9.1"
 PyBrowserID = ">=0.10.0,<1"
-pyjwt = "^2.6.0"
 pyramid = "1.10.4"
 pyramid_localroles = ">=0.1,<1"
 pyramid-multiauth = ">=0.9.0,<1"
 pyramid-retry = "^1.0"
 pyramid-tm = "^2.5"
 pyramid-translogger = "^0.1"
 python-dateutil = "^2.8.2"
 python_magic = ">=0.4.27"
 pytz = ">=2021.3"
 rdflib = "^4.2.2"
 rdflib-jsonld = ">=0.5.0,<1.0.0"
-redis = "^4.5.1"
 rutter = ">=0.3,<1"
 simplejson = "^3.17.6"
 SPARQLWrapper = "^1.8.5"
 SQLAlchemy = "^1.4.41"  # portals pin 1.4.41, but we don't. should it matter? -kmp 6-Mar-2023
 # Our use of structlog is pretty vanilla, so we should be OK with changes across the 18-19 major version boundary.
 structlog = ">=19.2.0,<20"
 subprocess_middleware = ">=0.3,<1"
@@ -79,67 +79,62 @@
 WebOb = "^1.8.7"
 WebTest = "^2.0.35"
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
 "zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
+pytest-redis = "^2.0.0"
+redis = "^4.5.1"
 
 [tool.poetry.dev-dependencies]
-boto3-stubs = "^1.26.124"  # no particular version required, but this speeds up search
-botocore-stubs = "^1.29.124"  # no particular version required, but this speeds up search
+botocore-stubs = ">=1.27.36"  # no particular version required, but this speeds up search
+boto3-stubs = ">=1.24.36"  # no particular version required, but this speeds up search
 coverage = ">=6.2"
 codacy-coverage = ">=1.3.11"
+coveralls = ">=3.3.1"
 docutils = ">=0.16,<1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
+# moto 2.0.0 (see https://github.com/spulec/moto/blob/master/CHANGELOG.md) has incompatibilities in how it needs
+# to be configured, so will require some adaptation. moto 1.3,14 will support python 3.8, but python 3.9 support
+# needs moto 2.2.5. If we do eventually upgrade, there are some tests in test_storage.py that may be possible to
+# simplify. -kmp 5-Feb-2022
+#
+# We tried 1.3.14 but it adds stuff we don't need (until Python 3.8) and it doesn't work as well.
+# See https://github.com/spulec/moto/blob/master/CHANGELOG.md
 moto = "^4.0.3"
-PasteDeploy = "1.5.2"
-plaster = "1.0"
-plaster-pastedeploy = "0.6"
 pipdeptree = ">=2.3.3"
-# pip-licenses = ">=3.5.3"
+pip-licenses = "^3.5.3"
 # Not even sure we need an explicit dependence on Pillow, though it might help keep from searching older versions.
 # -kmp 22-Feb-2022
 Pillow = ">=6.2.2"  # later version known to work - Will 11/17/20
 # Experimental upgrade to PyTest 4.5. It may be possible to upgrade further, but I think this is an improvement.
 # -kmp 11-May-2020
 pytest = "^7.2.2"
 pytest-cov = ">=2.2.1"
 # pytest_exact_fixtures = "^0.3"
 pytest-instafail = ">=0.3.0"
 # TODO: Investigate whether a major version upgrade is allowable for 'pytest-mock'.
 pytest-mock = ">=0.11.0"
-pytest-redis = "^2.0.0"
 # TODO: Investigate whether a major version upgrade is allowable for 'pytest-runner'.
 pytest-runner = ">=4.0"
 pytest-timeout = ">=1.0.0"
 # There was no version 4 of PyYAML. We upgraded today to PyYAML 5 per compatibility info in:
 # https://github.com/yaml/pyyaml/issues/265
 # We must have 5.1 to get the new yaml.safe_load method.
 # awscli appears to add its own restrictions, but our uses are pretty simple.
 # 5.2 had soe bugs that were probably only in Python 2, but we require 5.2 here just in case.
 # Any narrowing beyond that is just to help 'poetry lock' converge faster.
 # And we only need .safe_load in testing, so we're moving this to dev dependencies. -kmp 22-Feb-2022
 PyYAML = ">=5.1,<5.5"
 "repoze.debug" = ">=1.0.2"
+# Used only by moto, not explicitly by us.
+# responses = "^0.17.0"  # 0.17.0 is the last version compliant with Python 3.6
 wheel = ">=0.29.0"
 
 [tool.poetry.scripts]
-dev-servers = "snovault.dev_servers:main"
-list-db-tables = "snovault.commands.list_db_tables:main"
-prepare-local-dev = "snovault.commands.prepare_template:prepare_local_dev_main"
 wipe-test-indices = "snovault.commands.wipe_test_indices:main"
 
-[paste.app_factory]
-main = "snovault:main"
-
-[paste.composite_factory]
-indexer = "snovault.elasticsearch.es_index_listener:composite"
-# ingester = "encoded.ingestion_listener:composite"
-
-# [paste.filter_app_factory]
-# memlimit = "encoded.memlimit:filter_app"
-
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/__init__.py` & `dcicsnovault-8.0.2b0/snovault/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,43 +17,38 @@
 from .schema_utils import load_schema  # noqa
 from .upgrader import upgrade_step  # noqa
 
 
 def includeme(config):
     config.include('pyramid_retry')
     config.include('pyramid_tm')
-    config.include('snovault.authentication')
-    config.include('snovault.util')
-    config.include('snovault.drs')
-    config.include('snovault.stats')
-    config.include('snovault.batchupgrade')
-    config.include('snovault.calculated')
-    config.include('snovault.config')
-    config.include('snovault.connection')
-    config.include('snovault.custom_embed')
-    config.include('snovault.embed')
-    config.include('snovault.json_renderer')
-    config.include('snovault.validation')
-    config.include('snovault.predicates')
-    config.include('snovault.invalidation')
-    config.include('snovault.upgrader')
-    config.include('snovault.aggregated_items')
-    config.include('snovault.storage')
-    config.include('snovault.typeinfo')
-    config.include('snovault.types')
-    config.include('snovault.resources')
-    config.include('snovault.attachment')
-    config.include('snovault.schema_graph')
-    config.include('snovault.jsonld_context')
-    config.include('snovault.schema_views')
-    config.include('snovault.crud_views')
-    config.include('snovault.indexing_views')
-    config.include('snovault.resource_views')
-    config.include('snovault.settings')
-    config.include('snovault.server_defaults')
+    config.include('.util')
+    config.include('.stats')
+    config.include('.batchupgrade')
+    config.include('.calculated')
+    config.include('.config')
+    config.include('.connection')
+    config.include('.embed')
+    config.include('.json_renderer')
+    config.include('.validation')
+    config.include('.predicates')
+    config.include('.invalidation')
+    config.include('.upgrader')
+    config.include('.aggregated_items')
+    config.include('.storage')
+    config.include('.typeinfo')
+    config.include('.resources')
+    config.include('.attachment')
+    config.include('.schema_graph')
+    config.include('.jsonld_context')
+    config.include('.schema_views')
+    config.include('.crud_views')
+    config.include('.indexing_views')
+    config.include('.resource_views')
+    config.include('.settings')
 
 
 def main(global_config, **local_config):
     """
     This function returns a Pyramid WSGI application.
     """
     settings = global_config
@@ -84,27 +79,24 @@
 
     config.include(configure_dbsession)
     config.include('snovault')
     config.commit()  # commit so search can override listing
 
     config.include('.renderers')
 
-    if settings.get('elasticsearch.server'):
-        config.include('snovault.search.search')
-        config.include('snovault.search.compound_search')
-
     # only include this stuff if we're testing
     if asbool(settings.get('testing', False)):
         config.include('snovault.tests.testing_views')
+        config.include('snovault.tests.authentication')
         config.include('snovault.tests.root')
+        if settings.get('elasticsearch.server'):
+            config.include('snovault.tests.search')
 
         # in addition, enable invalidation scope for testing - but NOT by default
         settings[INVALIDATION_SCOPE_ENABLED] = True
-    else:
-        config.include('snovault.root')
 
     if 'elasticsearch.server' in config.registry.settings:
         config.include('snovault.elasticsearch')
 
     # configure redis server in production.ini
     if 'redis.server' in config.registry.settings:
         config.include('snovault.redis')
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/aggregated_items.py` & `dcicsnovault-8.0.2b0/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/app.py` & `dcicsnovault-8.0.2b0/snovault/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import base64
 import codecs
 import hashlib
 import json
 import os
 import psycopg2
-import psycopg2.extensions
 import subprocess
 import zope.sqlalchemy
 
 from dcicutils.misc_utils import ignored, ignorable
 from pyramid.config import Configurator
 from pyramid.path import AssetResolver, caller_package
 from pyramid.session import SignedCookieSessionFactory
 from pyramid.settings import asbool
 from pyramid_localroles import LocalRolesAuthorizationPolicy
-from sqlalchemy import engine_from_config, event, orm  # , text as psql_text
+from sqlalchemy import engine_from_config, event, orm
 from webob.cookies import JSONSerializer
 
 from .interfaces import DBSESSION
 
 from .elasticsearch import APP_FACTORY
 from .json_renderer import json_renderer
 from .storage import Base
@@ -79,21 +78,15 @@
             # and we have long used that. But the real purpose of introducing
             # this coercion is to get a ValueError if a string other than a
             # representation of a number slips through, to seal out accidental injection.
             # -kmp 6-Apr-2023
             timeout_ms = int(timeout_ms)
         cursor = dbapi_connection.cursor()
         try:
-            # cursor: psycopg2.extensions.cursor
-            # This call to psycopg2.extensions.cursor.execute expects a real string. Giving it an sqlalchemy.text
-            # object will fail because something will try to do a boolean test, probably "if thing_to_execute:..."
-            # and __bool__ is not defined on sqlalchemy.txt
-            # Bottom line: Cannot wrap this string with psql_text(...) like we do elsewhere. It's not ready.
-            # Might be we could do such a wrapper if we called execute on some other object.
-            cursor.execute("SET statement_timeout = %d;" % timeout_ms)
+            cursor.execute("SET statement_timeout TO %d" % timeout_ms)
         except psycopg2.Error:
             dbapi_connection.rollback()
         finally:
             cursor.close()
             dbapi_connection.commit()
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/attachment.py` & `dcicsnovault-8.0.2b0/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/batchupgrade.py` & `dcicsnovault-8.0.2b0/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/cache.py` & `dcicsnovault-8.0.2b0/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/calculated.py` & `dcicsnovault-8.0.2b0/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.2b0/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.2b0/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.2b0/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/commands/profile.py` & `dcicsnovault-8.0.2b0/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.2b0/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/config.py` & `dcicsnovault-8.0.2b0/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/connection.py` & `dcicsnovault-8.0.2b0/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/crud_views.py` & `dcicsnovault-8.0.2b0/snovault/crud_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,16 +263,16 @@
     """
     item_uuid = str(context.uuid)
     links = request.registry[STORAGE].find_uuids_linked_to_item(item_uuid)
     request.response.status = 200
     result = {
         'status': 'success',
         '@type': ['result'],
-        'display_title': f'Links to {item_uuid}',
-        'notification': f'{item_uuid} has {len(links)} items linking to it. This may include rev_links if status != deleted',
+        'display_title': 'Links to %s' % item_uuid,
+        'notification' : '%s has %s items linking to it. This may include rev_links if status != deleted' % (item_uuid, len(links)),
         'uuids_linking_to': links
     }
     return result
 
 
 @view_config(context=Item, permission='edit', request_method='DELETE')
 @debug_log
@@ -285,48 +285,49 @@
     To purge, use ?purge=true query string
     For example: DELETE `/<item-type>/<uuid>?purge=true`
     """
     # possibly temporary fix to check if user is admin
     if hasattr(request, 'user_info'):
         user_details = request.user_info.get('details', {})
     else:
-        # used to check for admin here, now done in user_info above
-        # note that hasattr() results in a function call when referring to an @property
-        user_details = {}
+        if 'group.admin' in request.effective_principals:
+            user_details = {'groups': 'admin'}  # you can do it
+        else:
+            user_details = {}  # you cannot
     if 'admin' not in user_details.get('groups', []):
         msg = u'Must be admin to fully delete items.'
         raise ValidationFailure('body', ['userid'], msg)
 
     purge_from_database = asbool(request.GET and request.GET.get('purge'))
     uuid = str(context.uuid)
     if purge_from_database:
         # Delete entirely - WARNING USE WITH CAUTION - DELETES PERMANENTLY
         # checking of item status and links is done within purge_item()
         result = purge_item(context, request)
         if result:
             return {
                 'status': 'success',
                 '@type': ['result'],
-                'notification': f'Permanently deleted {uuid}',
+                'notification' : 'Permanently deleted ' + uuid,
                 '@graph': [uuid]
             }
     else:
         result = delete_item(context, request)
         if result:
             return {
                 'status': 'success',
                 '@type': ['result'],
-                'notification': f'Set status of {uuid} to deleted',
-                '@graph': [render_item(request, context, render)]
+                'notification' : 'Set status of ' + uuid + ' to deleted',
+                '@graph': [ render_item(request, context, render) ]
             }
 
     return {
         'status': 'failure',
         '@type': ['result'],
-        'notification': 'Deletion failed',
+        'notification' : 'Deletion failed',
         '@graph': [uuid]
     }
 
 
 @view_config(context=Item, permission='view', request_method='GET',
              name='validation-errors')
 @debug_log
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/edw_hash.py` & `dcicsnovault-8.0.2b0/snovault/tests/snowflake_hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 )
 from hashlib import sha384
 from passlib.registry import register_crypt_handler
 from passlib.utils import handlers as uh
 
 
 def includeme(config):
-    register_crypt_handler(EDWHash)
+    register_crypt_handler(SNOWHash)
 
 
-class EDWHash(uh.StaticHandler):
-    """ EDW's password hashing scheme
+class SNOWHash(uh.StaticHandler):
+    """ a special snowflake of a  password hashing scheme
 
     Cryptographic strength of the hashing function is less of a concern for
     randomly generated passwords.
     """
-    name = 'edw_hash'
+    name = 'snowflake_hash'
     checksum_chars = uh.PADDED_BASE64_CHARS
     checksum_size = 64
 
     setting_kwds = ('salt_before', 'salt_after', 'salt_base')
     salt_before = b"186ED79BAEXzeusdioIsdklnw88e86cd73"
     salt_after = b"<*#$*(#)!DSDFOUIHLjksdf"
     salt_base = b64decode(b"""\
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.2b0/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/embed.py` & `dcicsnovault-8.0.2b0/snovault/embed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 from copy import deepcopy
 from posixpath import join
+from typing import Union
 
 from pyramid.compat import (
     native_,
     unquote_bytes_to_wsgi,
 )
 from pyramid.httpexceptions import HTTPNotFound
+from pyramid.request import Request
 
 from .interfaces import CONNECTION
 
 log = logging.getLogger(__name__)
 
 
 def includeme(config):
@@ -160,24 +162,15 @@
         as_user (str/bool): involved in setting subreq.remote_user
 
     Returns:
         dict containing the result and a number of subrequest attributes
     """
     # Carl: the subrequest is 'built' here, but not actually invoked
     subreq = make_subrequest(request, path)
-    # these attributes are propogated across the subrequest
-    subreq.override_renderer = 'null_renderer'
-    subreq._indexing_view = request._indexing_view
-    subreq._aggregate_for = request._aggregate_for
-    subreq._aggregated_items = request._aggregated_items
-    subreq._sid_cache = request._sid_cache
-    if as_user is not True:
-        if 'HTTP_COOKIE' in subreq.environ:
-            del subreq.environ['HTTP_COOKIE']
-        subreq.remote_user = as_user
+    _set_subrequest_attributes(subreq, request, as_user=as_user)
     # _linked_uuids are populated in item_view_object of resource_views.py
     try:
         result = request.invoke_subrequest(subreq)
     except HTTPNotFound:
         if '@@index-data' in path:
             # the resource to index is missing; likely purged
             raise MissingIndexItemException(path)
@@ -186,14 +179,42 @@
             raise KeyError(path)
     return {'result': result, '_linked_uuids': subreq._linked_uuids,
             '_rev_linked_by_item': subreq._rev_linked_uuids_by_item,
             '_aggregated_items': subreq._aggregated_items,
             '_sid_cache': subreq._sid_cache}
 
 
+def _set_subrequest_attributes(
+    subrequest: Request, request: Request, as_user: Union[str, bool] = False
+) -> None:
+    subrequest.override_renderer = 'null_renderer'
+    _add_propagated_attributes(subrequest, request)
+    if as_user is not True:
+        _remove_http_cookie_and_set_user(subrequest, as_user)
+
+
+def _add_propagated_attributes(subrequest: Request, request: Request) -> None:
+    subrequest._indexing_view = request._indexing_view
+    subrequest._aggregate_for = request._aggregate_for
+    subrequest._aggregated_items = request._aggregated_items
+    subrequest._sid_cache = request._sid_cache
+    try:
+        subrequest._stats = request._stats
+    except AttributeError:
+        subrequest._stats = {}
+
+
+def _remove_http_cookie_and_set_user(
+    subrequest: Request, remote_user: Union[str, bool]
+) -> None:
+    if 'HTTP_COOKIE' in subrequest.environ:
+        del subrequest.environ['HTTP_COOKIE']
+    subrequest.remote_user = remote_user
+
+
 class NullRenderer:
     '''Sets result value directly as response.
     '''
     def __init__(self, info):
         pass
 
     def __call__(self, value, system):
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/etag.py` & `dcicsnovault-8.0.2b0/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/indexing_views.py` & `dcicsnovault-8.0.2b0/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/interfaces.py` & `dcicsnovault-8.0.2b0/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/invalidation.py` & `dcicsnovault-8.0.2b0/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/json_renderer.py` & `dcicsnovault-8.0.2b0/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/jsongraph.py` & `dcicsnovault-8.0.2b0/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/jsonld_context.py` & `dcicsnovault-8.0.2b0/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/predicates.py` & `dcicsnovault-8.0.2b0/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.2b0/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/resource_views.py` & `dcicsnovault-8.0.2b0/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/resources.py` & `dcicsnovault-8.0.2b0/snovault/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import logging
 from collections import Mapping
 from copy import deepcopy
 from dcicutils.misc_utils import ignored
 from pyramid.decorator import reify
 from pyramid.httpexceptions import HTTPInternalServerError
 from pyramid.security import (
-    Allow,
-    Deny,
-    ALL_PERMISSIONS,
+    # Allow,
     Everyone,
     Authenticated,
     principals_allowed_by_permission
 )
 from pyramid.traversal import (
     resource_path,
     traverse
@@ -37,43 +35,17 @@
 from .util import add_default_embeds, IndexSettings
 
 logger = logging.getLogger(__name__)
 
 
 def includeme(config):
     config.include(auth0_config)
-    config.include(recaptcha_config)
     config.scan(__name__)
 
 
-def acl_from_settings(settings):
-    # XXX Unsure if any of the demo instance still need this
-    acl = []
-    for k, v in settings.items():
-        if k.startswith('allow.'):
-            action = Allow
-            permission = k[len('allow.'):]
-            principals = v.split()
-        elif k.startswith('deny.'):
-            action = Deny
-            permission = k[len('deny.'):]
-            principals = v.split()
-        else:
-            continue
-        if permission == 'ALL_PERMISSIONS':
-            permission = ALL_PERMISSIONS
-        for principal in principals:
-            if principal == 'Authenticated':
-                principal = Authenticated
-            elif principal == 'Everyone':
-                principal = Everyone
-            acl.append((action, principal, permission))
-    return acl
-
-
 class Resource(object):
     """
     Just used to add global calculated properties
     """
     @calculated_property(name='@id', schema={
         "title": "ID",
         "type": "string",
@@ -97,27 +69,14 @@
     __parent__ = None
     properties = {}
 
     def __init__(self, registry):
         self.registry = registry
 
     @reify
-    def __acl__(self):
-        acl = acl_from_settings(self.registry.settings) + [
-            (Allow, Everyone, ['list', 'search']),
-            (Allow, 'group.admin', ALL_PERMISSIONS),
-            (Allow, 'remoteuser.EMBED', 'restricted_fields'),
-        ] + [
-                  (Allow, 'remoteuser.INDEXER', ['view', 'view_raw', 'list', 'index']),
-                  (Allow, 'remoteuser.EMBED', ['view', 'view_raw', 'expand']),
-                  (Allow, Everyone, ['visible_for_edit'])
-              ]
-        return acl
-
-    @reify
     def connection(self):
         return self.registry[CONNECTION]
 
     @reify
     def collections(self):
         return self.registry[COLLECTIONS]
 
@@ -192,39 +151,14 @@
             callback = f'{request.host_url}/callback'
             response_dict['auth0Options']['auth']['redirectUrl'] = callback
         return response_dict
 
     config.add_view(auth0_config_view, route_name='auth0-config')
 
 
-def recaptcha_config(config):
-    """ Route that exposes the recaptcha site key """
-    config.add_route(
-        'recaptcha-config',
-        '/recaptcha_config'
-    )
-    recaptcha_config_values = {  # determines which values are echoed
-        'g.recaptcha.key': 'RecaptchaKey',
-    }
-
-    def recaptcha_config_view(request):
-        response = request.response
-        response.content_type = 'application/json; charset=utf-8'
-        response_dict = {
-            'title': 'Recaptcha Config',
-        }
-        settings = config.registry.settings
-        for config_key, result_key in recaptcha_config_values.items():
-            if config_key in settings:
-                response_dict[result_key] = settings[config_key]
-        return response_dict
-
-    config.add_view(recaptcha_config_view, route_name='recaptcha-config')
-
-
 class AbstractCollection(Resource, Mapping):
     """
     Collection for a certain type of resource that stores the following info:
     - registry (pyramid registry)
     - type_info (TypeInfo for a certain item type, see snovault.typeinfo.py)
     - __acl__
     - uniqueKey for the collection (e.g. item_name:key)
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/schema_graph.py` & `dcicsnovault-8.0.2b0/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/schema_utils.py` & `dcicsnovault-8.0.2b0/snovault/schema_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import codecs
 import collections
 import uuid
 import json
+import requests
 
 from datetime import datetime
 from dcicutils.misc_utils import ignored
 from jsonschema_serialize_fork import (
     Draft4Validator,
     FormatChecker,
     RefResolver,
 )
+# TODO (C4-177): remove these imports (urlsplit, urlopen) when RefResolverOrdered is removed
+from jsonschema_serialize_fork.compat import urlsplit, urlopen
 from jsonschema_serialize_fork.exceptions import ValidationError
 from pyramid.path import AssetResolver, caller_package
 from pyramid.threadlocal import get_current_request
 from pyramid.traversal import find_resource
 from uuid import UUID
 from .util import ensurelist
 
@@ -21,27 +24,74 @@
 # to avoid a circularity. No files should refer upward to "." for imports. -kmp 9-Jun-2020
 from .resources import Item, COLLECTIONS
 
 
 SERVER_DEFAULTS = {}
 
 
-# TODO: Shouldn't this return func? Otherwise this:
-#           @server_default
-#           def foo(instance, subschema):
-#               return ...something...
-#       does (approximately):
-#           SERVER_DEFAULTS['foo'] = lambda(instance, subschema): ...something...
-#           server_default = None
-#       It feels like the function should still get defined. -kmp 17-Feb-2023
 def server_default(func):
     SERVER_DEFAULTS[func.__name__] = func
 
 
-class NoRemoteResolver(RefResolver):
+class RefResolverOrdered(RefResolver):
+    """
+    Overwrite the resolve_remote method in the RefResolver class, written
+    by lrowe. See:
+    https://github.com/lrowe/jsonschema_serialize_fork/blob/master/jsonschema_serialize_fork/validators.py
+    With python <3.6, json.loads was losing schema order for properties, facets,
+    and columns. Pass in the object_pairs_hook=collections.OrderedDict
+    argument to fix this.
+    WHEN ELASTICBEANSTALK IS RUNNING PY 3.6 WE CAN REMOVE THIS
+    """
+    # TODO (C4-177): The stated condition is now met. We are reliably in Python 3.6, so this code should be removed.
+
+    def resolve_remote(self, uri):
+        """
+        Resolve a remote ``uri``.
+        Does not check the store first, but stores the retrieved document in
+        the store if :attr:`RefResolver.cache_remote` is True.
+        .. note::
+            If the requests_ library is present, ``jsonschema`` will use it to
+            request the remote ``uri``, so that the correct encoding is
+            detected and used.
+            If it isn't, or if the scheme of the ``uri`` is not ``http`` or
+            ``https``, UTF-8 is assumed.
+        :argument str uri: the URI to resolve
+        :returns: the retrieved document
+        .. _requests: http://pypi.python.org/pypi/requests/
+        """
+        scheme = urlsplit(uri).scheme
+
+        if scheme in self.handlers:
+            result = self.handlers[scheme](uri)
+        elif (
+            scheme in ["http", "https"] and
+            # TODO (C4-177): PyCharm flagged free references to 'requests' in this file as undefined,
+            #                so I've added an import at top of file. However, that suggests this 'elif'
+            #                branch is never entered. When this tangled code is removed, I'll be happier.
+            #                Meanwhile having a definition seems safer than not. -kmp 9-Jun-2020
+            requests and
+            getattr(requests.Response, "json", None) is not None
+        ):
+            # Requests has support for detecting the correct encoding of
+            # json over http
+            if callable(requests.Response.json):
+                result = collections.OrderedDict(requests.get(uri).json())
+            else:
+                result = collections.OrderedDict(requests.get(uri).json)
+        else:
+            # Otherwise, pass off to urllib and assume utf-8
+            result = json.loads(urlopen(uri).read().decode("utf-8"), object_pairs_hook=collections.OrderedDict)
+
+        if self.cache_remote:
+            self.store[uri] = result
+        return result
+
+
+class NoRemoteResolver(RefResolverOrdered):
     def resolve_remote(self, uri):
         raise ValueError('Resolution disallowed for: %s' % uri)
 
 
 def mixinSchemas(schema, resolver, key_name='properties'):
     mixinKeyName = 'mixin' + key_name.capitalize()
     mixins = schema.get(mixinKeyName)
@@ -232,15 +282,15 @@
         schema = filename
         resolver = NoRemoteResolver.from_schema(schema)
     else:
         utf8 = codecs.getreader("utf-8")
         asset = AssetResolver(caller_package()).resolve(filename)
         schema = json.load(utf8(asset.stream()),
                            object_pairs_hook=collections.OrderedDict)
-        resolver = RefResolver('file://' + asset.abspath(), schema)
+        resolver = RefResolverOrdered('file://' + asset.abspath(), schema)
     # use mixinProperties, mixinFacets, mixinAggregations, and mixinColumns (if provided)
     schema = mixinSchemas(
         mixinSchemas(
             mixinSchemas(mixinSchemas(schema, resolver, 'properties'), resolver, 'facets'),
             resolver,
             'aggregations'
         ),
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/schema_views.py` & `dcicsnovault-8.0.2b0/snovault/schema_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
     schema = type_info.schema.copy()
     schema['@type'] = ['JSONSchema']
     jsonld_base = request.registry.settings['snovault.jsonld.terms_namespace']
     schema['rdfs:seeAlso'] = urlparse(jsonld_base).path + type_info.name
     # add links to profiles of children schemas
     schema['children'] = [
-        '/profiles/' + t_name + '.json' for t_name in type_info.child_types
+        '/profiles/' +  t_name + '.json' for t_name in type_info.child_types
     ]
 
     if type_info.factory is None:
         return schema
 
     # use first base_type that is not this type itself to handle abstract
     found_subtype = None
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.2b0/snovault/tests/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1158 +1,1435 @@
+import itertools
+import math
 import re
 import structlog
-from copy import deepcopy
+import uuid
+
 from collections import OrderedDict
+from copy import deepcopy
+from dcicutils.misc_utils import ignored
+from elasticsearch import TransportError, RequestError, ConnectionTimeout
+from elasticsearch_dsl import Search
 from pyramid.httpexceptions import HTTPBadRequest
+from pyramid.view import view_config
 from urllib.parse import urlencode
-from snovault import TYPES
-from snovault.elasticsearch.create_mapping import determine_if_is_date_field
-from .search_utils import (
-    find_nested_path,  # convert_search_to_dictionary,
-    QueryConstructionException,
-    COMMON_EXCLUDED_URI_PARAMS, QUERY, FILTER, MUST, MUST_NOT, BOOL, MATCH, SHOULD,
-    EXISTS, FIELD, NESTED, PATH, TERMS, RANGE, AGGS,  # REVERSE_NESTED,
-    STATS,
-    schema_for_field, get_query_field, search_log, MAX_FACET_COUNTS,
-)
+from webob.multidict import MultiDict
+
+from ..elasticsearch import ELASTIC_SEARCH
+from ..elasticsearch.create_mapping import determine_if_is_date_field
+from ..elasticsearch.indexer_utils import get_namespaced_index
+from ..embed import make_subrequest
+from ..interfaces import TYPES, COLLECTIONS
+from ..resources import AbstractCollection
+from ..typeinfo import AbstractTypeInfo
+from ..util import find_collection_subtypes, crawl_schema
 
 
 log = structlog.getLogger(__name__)
 
 
-class LuceneBuilder:
-    """ Collection of methods for working with Lucene queries. These operations can be used
-        independently of the SearchBuilder state. See SearchBuilder for how these are used.
-
-        Main points of entry:
-            1. build_filters (construct the search query itself)
-            2. build_facets (construct aggregations on search)
-            3. verify_search_has_permissions (to be sure we did not strip permissions while building search)
-
-        All other methods in this class are helper methods. Static methods are "leaf" operations that do
-        not require additional function calls. Class methods call other methods within the class but could
-        be "entry-point" methods as well.
-    """
-    to_from_pattern = re.compile("^(.*)[.](to|from)$")
-    RANGE_DIRECTIONS = ['gt', 'gte', 'lt', 'lte']
-    SMALLEST_NONZERO_IEEE_32 = 1.1754e-38  # smallest epsilon > 0 (estimate)
-    SMALLEST_NEGATIVE_IEEE_32 = -3.4028e38
-    # ref: http://www.cs.uwm.edu/classes/cs315/Bacon/Lecture/HTML/ch04s17.html
-    # 1.00000000000000000000001 x 2^-127 = 1.1754e-38
+def includeme(config):
+    config.add_route('search', '/search{slash:/?}')
+    config.add_route('browse', '/browse{slash:/?}')
+    config.scan(__name__)
 
-    @staticmethod
-    def apply_range_filters(range_filters, must_filters, es_mapping):
-        """
-        Applies the range filters to the 'must' subquery
-        Tuple format is required to handle nested fields that are non-range (it is discarded in this case)
-        Nested range fields must also be separated from other nested sub queries - see comment in handle_nested_filters
-        Modifies must_filters in place
-
-        :param range_filters: intermediary range_filter format to be converted to valid lucene
-        :param must_filters: must_filters from build_sub_queries, this is where range filters are applied
-        :param es_mapping: mapping of the item we searching on, as the range filter could be on a nested field
-        """
 
-        # tuple format is required to handle nested fields that are non-range (it is discarded in this case)
-        # nested range fields must also be separated from other nested sub queries - see comment in 'handle_nested_filters'
-        for range_field, range_def in range_filters.items():
-            nested_path = find_nested_path(range_field, es_mapping)
-            range_query = {RANGE: {range_field: range_def}}
-            if 'add_no_value' in range_def:
-                del range_def['add_no_value']
-                range_query = {
-                    BOOL: {
-                        SHOULD: [
-                            range_query,
-                            {BOOL: {MUST_NOT: {EXISTS: {FIELD: range_field}}}}
-                        ]
-                    }
-                }
-            if nested_path:
-                # look for existing nested sub query - must add to it if it exists
-                found = False
-                for query_part in must_filters:
-                    nested_queries = query_part.get(BOOL, {}).get(MUST, {})
-                    for query in nested_queries:
-                        if NESTED in query and query[NESTED][PATH] == nested_path:
-                            query[NESTED][QUERY][BOOL][MUST].append(range_query)
-                            found = True
-                            break  # if we found a valid path, add it here and continue
-                # if we never found a path, this is the only nested query on that path, so just add it as is
-                if not found:
-                    new_nested_query = {
-                        NESTED: {
-                            PATH: nested_path,
-                            QUERY: range_query
-                        }
-                    }
-                    must_filters.append(new_nested_query)
-            else:
-                must_filters.append(range_query)
+sanitize_search_string_re = re.compile(r'[\\\+\-\&\|\!\(\)\{\}\[\]\^\~\:\/\\\*\?]')
 
-    @staticmethod
-    def handle_should_query(field_name, options):
-        """
-        Builds a lucene 'should' subquery for every option for the given field
 
-        :param field_name: full path to field
-        :param options: list of options for that field
-            ex: field_name='embedded.files.file_size.raw', options=[20, 30, 40]
+COMMON_EXCLUDED_URI_PARAMS = [
+    'frame', 'format', 'limit', 'sort', 'from', 'field',
+    'mode', 'redirected_from', 'datastore', 'referrer',
+    'currentAction'
+]
 
-        :return: dsl-subquery that is effectively an OR of all options on the field. See SHOULD.
-        """
-        should_query = {BOOL: {SHOULD: {TERMS: {field_name: options}}}}
-        return should_query
 
-    @classmethod
-    def build_sub_queries(cls, field_filters, es_mapping):
-        """
-        Builds queries based on several things:
-            - What the query field is
-            - If that field is nested
-            - If we would like to see items who do not have a value for this field. These items will have 'No value'
-              for the relevant field.
-            - If it is a positive (must) or negative (must_not) query. This is the level by which these are separated.
-
-        :param field_filters: Intermediary format to be converted to valid lucene based on the es_mapping
-        :param es_mapping: mapping of the item we are searching on
-        :return: 4 tuple consisting of (must_filters, must_not_filters, must_filters_nested, must_not_filters_nested)
-        """
-        must_filters = []
-        must_not_filters = []
-        must_filters_nested = []
-        must_not_filters_nested = []
-
-        for query_field, filters in field_filters.items():
-            # if we are nested, we must construct the query differently than normal
-            nested_path = find_nested_path(query_field, es_mapping)
-            if nested_path is not None:
-                query_field = query_field.replace('.properties', '')
-                strip_raw = query_field.replace('.raw', '')
-
-                # if we are searching on the nested field itself, we must do something "special"
-                if nested_path == strip_raw:
-                    query_field = strip_raw
-
-                    # if searching on 'No Value' on a nested field, the query has to be written
-                    # slightly differently - note that you cannot combine a 'No value' search with
-                    # anything else on this field path
-                    if filters['add_no_value'] is True:
-                        should_arr = [{EXISTS: {FIELD: query_field}}]
-                        must_not_filters_nested.append((query_field, should_arr))
-                        continue
+@view_config(route_name='search', request_method='GET', permission='search')
+def search(context, request, search_type=None, return_generator=False, forced_type='Search', custom_aggregations=None):
+    """
+    Search view connects to ElasticSearch and returns the results
+    """
+    types = request.registry[TYPES]
+    # list of item types used from the query
+    doc_types = set_doc_types(request, types, search_type)
+    # sets request.normalized_params
+    search_base = normalize_query(request, types, doc_types)
+    # == INITIALIZE RESULT ==
+    result = {
+        '@context': request.route_path('jsonld_context'),
+        '@id': '/' + forced_type.lower() + '/' + search_base,
+        '@type': [forced_type],
+        'title': forced_type,
+        'filters': [],
+        'facets': [],
+        '@graph': [],
+        'notification': '',
+        'sort': {}
+    }
+    principals = request.effective_principals
+    es = request.registry[ELASTIC_SEARCH]
+
+    from_, size = get_pagination(request)
+
+    # get desired frame for this search
+    search_frame = request.normalized_params.get('frame', 'embedded')
+
+    # == PREPARE SEARCH TERM ==
+    prepared_terms = prepare_search_term(request)
+
+    schemas = [types[item_type].schema for item_type in doc_types]
+
+    # set ES index based on doc_type (one type per index)
+    # if doc_type is item, search all indexes by setting es_index to None
+    # If multiple, search all specified
+    namespaced_star = get_namespaced_index(request, '*')
+    if 'Item' in doc_types:
+        es_index = namespaced_star
+    else:
+        es_index = find_index_by_doc_types(request, doc_types, ['Item'])
+
+    # establish elasticsearch_dsl class that will perform the search
+    search = Search(using=es, index=es_index)
+
+    # set up clear_filters path
+    result['clear_filters'] = clear_filters_setup(request, doc_types, forced_type)
+
+    # == SET TYPE FILTERS ==
+    build_type_filters(result, request, doc_types, types)
+
+    # get the fields that will be used as source for the search
+    # currently, supports frame=raw/object but live faceting does not work
+    # this is okay because the only non-embedded access will be programmatic
+    source_fields = sorted(list_source_fields(request, doc_types, search_frame))
+
+    # == GET FILTERED QUERY ==
+    # Builds filtered query which supports multiple facet selection
+    search, string_query = build_query(search, prepared_terms, source_fields)
+
+    # == Set sort order ==
+    search = set_sort_order(request, search, prepared_terms, types, doc_types, result)
+    # TODO: implement BOOST here?
+
+    # == Set filters ==
+    search, query_filters = set_filters(request, search, result, principals, doc_types)
+
+    # == Set starting facets ==
+    facets = initialize_facets(request, doc_types, prepared_terms, schemas)
+
+    # == Adding facets, plus any optional custom aggregations. ==
+    # Uses 'size' and 'from_' to conditionally skip (no facets if from > 0; no aggs if size > 0).
+    search = set_facets(search, facets, query_filters, string_query, request, doc_types, custom_aggregations, size, from_)
+
+    # == Add preference from session, if available ==
+    search_session_id = None
+    if request.__parent__ is None and not return_generator and size != 'all':  # Probably unnecessary, but skip for non-paged, sub-reqs, etc.
+        search_session_id = request.cookies.get('searchSessionID', 'SESSION-' + str(uuid.uuid1()))
+        search = search.params(preference=search_session_id)
+
+    # == Execute the query ==
+    if size == 'all':
+        es_results = execute_search_for_all_results(search)
+    else:
+        size_search = search[from_:from_ + size]
+        es_results = execute_search(size_search)
+
+    # == Record total number of hits ==
+    result['total'] = total = es_results['hits']['total']['value']
+    result['facets'] = format_facets(es_results, facets, total, search_frame)
+    result['aggregations'] = format_extra_aggregations(es_results)
+
+    # Add batch actions
+    # TODO: figure out exactly what this does. Provide download URLs?
+    # Implement later
+    # result.update(search_result_actions(request, doc_types, es_results))
+
+    # == Add all link for collections ==
+    if size not in (None, 'all') and size < result['total']:
+        params = [(k, v) for k, v in request.normalized_params.items() if k != 'limit']
+        params.append(('limit', 'all'))
+        if context:
+            result['all'] = '%s?%s' % (request.resource_path(context), urlencode(params))
+
+    # add actions (namely 'add')
+    result['actions'] = get_collection_actions(request, types[doc_types[0]])
+
+    if not result['total']:
+        # http://googlewebmastercentral.blogspot.com/2014/02/faceted-navigation-best-and-5-of-worst.html
+        request.response.status_code = 404
+        result['notification'] = 'No results found'
+        result['@graph'] = []
+        return result if not return_generator else []
+
+    columns = build_table_columns(request, schemas, doc_types)
+    if columns:
+        result['columns'] = columns
+
+    result['notification'] = 'Success'
+
+    # == Format results for JSON-LD ==
+    graph = format_results(request, es_results['hits']['hits'], search_frame)
+
+    if request.__parent__ is not None or return_generator:
+        if return_generator:
+            return graph
+        else:
+            result['@graph'] = list(graph)
+            return result
 
-                # Build must/must_not sub-queries
-                # Example:
-                # {'bool': {'must': {'bool':
-                #   {'should': [{'match': {'embedded.hg19.hg19_hgvsg.raw': 'NC_000001.11:g.12185956del'}},
-                #               {'match': {'embedded.hg19.hg19_hgvsg.raw': 'NC_000001.11:g.11901816A>T'}}
-                #               ]}}}}
-                # This is a "normal" query that we must convert to a "nested" sub-query on nested_path
-                must_terms = cls.construct_nested_sub_queries(query_field, filters, key='must_terms')
-                must_not_terms = cls.construct_nested_sub_queries(query_field, filters, key='must_not_terms')
-
-                # XXX: In ES6, MUST -> MUST_NOT EXISTS does not work - have to use EXISTS under MUST_NOT
-                # This means you cannot search on field=value or field DNE
-                if filters['add_no_value'] is True:  # when searching on 'No Value'
-                    should_arr = [must_not_terms] if must_not_terms else []
-                    should_arr.append({BOOL: {MUST: {EXISTS: {FIELD: query_field}}}})  # field=value OR field DNE
-                    must_not_filters_nested.append((query_field, should_arr))
-                    if must_terms:
-                        must_filters_nested.append((query_field, must_terms))
-                else:  # when not searching on 'No Value'
-                    should_arr = [must_terms] if must_terms else []
-                    should_arr.append({EXISTS: {FIELD: query_field}})   # field=value OR field EXISTS
-                    must_filters_nested.append((query_field, should_arr))
-                    if must_not_terms:
-                        must_not_filters_nested.append((query_field, must_not_terms))
+    result['@graph'] = list(graph)
+    if search_session_id:  # Is 'None' if e.g. limit=all
+        request.response.set_cookie('searchSessionID', search_session_id)  # Save session ID for re-requests / subsequent pages.
+    return result
 
-            # if we are not nested, handle this with 'terms' query like usual
-            else:
-                must_terms = {TERMS: {query_field: filters['must_terms']}} if filters['must_terms'] else {}
-                must_not_terms = {TERMS: {query_field: filters['must_not_terms']}} if filters['must_not_terms'] else {}
-                if filters['add_no_value'] is True:
-                    # add to must_not in an OR case, which is equivalent to filtering on 'No value'
-                    should_arr = [must_terms] if must_terms else []
-                    should_arr.append({BOOL: {MUST_NOT: {EXISTS: {FIELD: query_field}}}})  # field=value OR field DNE
-                    must_filters.append((query_field, {BOOL: {SHOULD: should_arr}}))
-                elif filters['add_no_value'] is False:
-                    # add to must_not in an OR case, which is equivalent to filtering on '! No value'
-                    should_arr = [must_terms] if must_terms else []
-                    should_arr.append({EXISTS: {FIELD: query_field}})  # field=value OR field EXISTS
-                    must_filters.append((query_field, {BOOL: {SHOULD: should_arr}}))
-                elif must_terms:  # no filtering on 'No value'
-                    must_filters.append((query_field, must_terms))
-                if must_not_terms:
-                    must_not_filters.append((query_field, must_not_terms))
 
-        return must_filters, must_not_filters, must_filters_nested, must_not_filters_nested
+@view_config(route_name='browse', request_method='GET', permission='search')
+def browse(context, request, search_type='ExperimentSetReplicate', return_generator=False):
+    """
+    Simply use search results for browse view
+    """
+    return search(context, request, search_type, return_generator, forced_type='Browse')
 
-    @staticmethod
-    def construct_nested_sub_queries(query_field, filters, key='must_terms'):
-        """
-         Helper for build_sub_queries that constructs the base layer of sub-queries
-         Note that due to the query structure, 'must' is always needed in the base level query,
-         since at this point we have already split into 'must' or 'must_not'.
-
-        :param query_field: field that we are querying
-        :param filters: all filters
-        :param key: one of 'must' or 'must_not'
-        :return: a lucene sub-query filtering the query field based on the given filters
-        :raises: QueryConstructionException if bad params make it here
+
+@view_config(context=AbstractCollection, permission='list', request_method='GET')
+def collection_view(context, request):
+    """
+    Simply use search results for collections views (e.g./biosamples/)
+    This is a redirect directly to the search page
+    """
+    return search(context, request, context.type_info.name, False, forced_type='Search')
+
+
+def get_collection_actions(request, type_info):
+    collection = request.registry[COLLECTIONS].get(type_info.name)
+    if collection and hasattr(collection, 'actions'):
+        return collection.actions(request)
+    else:
+        return None
+
+
+def get_pagination(request):
+    """
+    Fill from_ and size parameters for search if given in the query string
+    """
+    from_ = request.normalized_params.get('from', 0)
+    size = request.normalized_params.get('limit', 25)
+    if size in ('all', ''):
+        size = "all"
+    else:
+        try:
+            size = int(size)
+        except ValueError:
+            size = 25
+        try:
+            from_ = int(from_)
+        except ValueError:
+            size = 0
+    return from_, size
+
+
+def get_all_subsequent_results(initial_search_result, search, extra_requests_needed_count, size_increment):
+    from_ = 0
+    while extra_requests_needed_count > 0:
+        # print(str(extra_requests_needed_count) + " requests left to get all results.")
+        from_ = from_ + size_increment
+        subsequent_search = search[from_:from_ + size_increment]
+        subsequent_search_result = execute_search(subsequent_search)
+        extra_requests_needed_count -= 1
+        for hit in subsequent_search_result['hits'].get('hits', []):
+            yield hit
+
+
+def execute_search_for_all_results(search):
+    size_increment = 100  # Decrease this to like 5 or 10 to test.
+
+    first_search = search[0:size_increment]  # get aggregations from here
+    es_result = execute_search(first_search)
+
+    total_results_expected = es_result['hits'].get('total', 0)
+    extra_requests_needed_count = int(math.ceil(total_results_expected / size_increment)) - 1  # Decrease by 1 (first es_result already happened)
+
+    if extra_requests_needed_count > 0:
+        es_result['hits']['hits'] = itertools.chain(es_result['hits']['hits'], get_all_subsequent_results(es_result, search, extra_requests_needed_count, size_increment))
+    return es_result
+
+
+def normalize_query(request, types, doc_types):
+    """
+    Normalize the query by calculating and setting request.normalized_params
+    (a webob MultiDict) that is derived from custom query rules and also
+    the list of doc_types specified by set_doc_types(). The normalize_param
+    helper function finds field_schema for each query parameter and enforces
+    a set of rules (see below). If the query item types differ from doc_types,
+    override with doc_types
+
+    Args:
+        request: the current Request
+        types: registry[TYPES]
+        doc_types (list): item_types to use for the search
+
+    Returns:
+        string: query string built from normalized params
+    """
+    def normalize_param(key, val):
         """
-        if key not in ['must_terms', 'must_not_terms']:
-            raise QueryConstructionException(
-                query_type='nested',
-                func='construct_nested_sub_queries',
-                msg='Tried to handle nested filter with key other than must/must_not: %s' % key
-            )
-        my_filters = filters.get(key, [])
-        if len(my_filters) == 0:
-            return {}
-        elif len(my_filters) == 1:  # see standard bool/match query
-            return {MATCH: {query_field: my_filters[0]}}
+        Process each key/val in the original query param. As part of this,
+        obtain the field schema for each parameter.
+        Current rules:
+        - for 'type', get name from types (from the registry)
+        - append '.display_title' to any terminal linkTo query field
+        """
+        # type param is a special case. use the name from TypeInfo
+        if key == 'type' and val in types:
+            return (key, types[val].name)
+
+        # find schema for field parameter and drill down into arrays/subobjects
+        field_schema = schema_for_field(key, request, doc_types)
+        while field_schema and ('items' in field_schema or 'properties' in field_schema):
+            try:
+                field_schema = field_schema['items']
+            except KeyError:
+                pass
+            try:
+                field_schema = field_schema['properties']
+            except KeyError:
+                pass
+        if field_schema and 'linkTo' in field_schema:
+            # add display_title to terminal linkTo query fields
+            if key.endswith('!'):  # handle NOT
+                return (key[:-1] + '.display_title!', val)
+            return (key + '.display_title', val)
         else:
-            sub_queries = {BOOL: {SHOULD: []}}  # combine all options under SHOULD
-            for option in my_filters:
-                sub_queries[BOOL][SHOULD].append({MATCH: {query_field: option}})
-            return sub_queries
-
-    @classmethod
-    def extract_field_from_to(cls, query_part):
-        """ Neat helper method provided by Kent to clean up a step in 'handle_range_filters'.
-            Extracts the field_name and whether it is a 'from' or 'to' query
-
-        :param query_part: query part to parse, such as "field.a.from" or "field.to". See the regexp.
-        :return: 3-tuple consisting of whether or not there was a match, the first grouping and the second grouping
-                 ie: (True, field.name, 'from')
-        """
-        match = cls.to_from_pattern.match(query_part)
-        if match is not None:
-            return bool(match), match.group(1), match.group(2)
-        return False, None, None
-
-    @classmethod
-    def canonicalize_bounds(cls, range_filter):
-        """ Canonicalizes the bounds of the range filter such that they are
-            inclusive on the lower bound and exclusive on the upper bound.
-        """
-        lower, upper = -1e38, 1e38  # very large numbers that should never be in range
-        for direction, pivot in range_filter.items():
-            pivot = float(pivot)
-            if direction == 'lte':
-                upper = pivot + cls.SMALLEST_NONZERO_IEEE_32
-            elif direction == 'lt':
-                upper = pivot
-            elif direction == 'gte':
-                lower = pivot
-            elif direction == 'gt':
-                lower = pivot - cls.SMALLEST_NONZERO_IEEE_32
-        return lower, upper
-
-    @classmethod
-    def range_includes_zero(cls, range_filter):
-        """ Returns True if the given range_filter includes the value 0. """
-        lower, upper = cls.canonicalize_bounds(range_filter)
-        return lower <= 0 <= upper
+            return (key, val)
 
-    @classmethod
-    def handle_range_filters(cls, request, result, field_filters, doc_types):
-        """
-        Constructs range_filters based on the given filters as part of the MUST sub-query
+    normalized_params = (
+        normalize_param(k, v)
+        for k, v in request.params.items()
+    )
+    # use a MultiDict to emulate request.params
+    normalized_params = MultiDict(normalized_params)
+    # overwrite 'type' if not equal to doc_types
+    if set(normalized_params.getall('type')) != set(doc_types):
+        if 'type' in normalized_params:
+            del normalized_params['type']
+        for dtype in doc_types:
+            normalized_params.add('type', dtype)
+    # add the normalized params to the request
+    # these will be used in place of request.params for the rest of search
+    setattr(request, 'normalized_params', normalized_params)
+    # the query string of the normalized search
+    qs = '?' + urlencode([
+        (k.encode('utf-8'), v.encode('utf-8'))
+        for k, v in request.normalized_params.items()
+    ])
+    return qs
 
-        :param request: current request
-        :param result: result to modify in place
-        :param field_filters: filters to look at
-        :param doc_types: types we are searching on
-        :return: constructed range_filters
-        """
-        range_filters = {}
 
-        for field, term in request.normalized_params.items():
-            not_field = False  # keep track if query is NOT (!)
-            exists_field = False  # keep track of null values
-            range_type = False  # If we determine is a range request (field.to, field.from), will be populated with string 'date' or 'numerical'
-            range_direction = None
-            field_schema = {}
-            if field == 'q' or field in COMMON_EXCLUDED_URI_PARAMS:
-                continue
-            elif field == 'type' and term != 'Item':
-                continue
-            elif term == 'No value':
-                exists_field = True
+def clear_filters_setup(request, doc_types, forced_type):
+    """
+    Clear Filters URI path
 
-            # Check for date or numerical range filters
-            is_range, f_field, which = cls.extract_field_from_to(field)
-            if is_range:
-                if which == 'to':
-                    range_direction = 'lte'
-                else:
-                    range_direction = 'gte'
+    Make a URI path that clears all non-datatype filters
+    and leaves in `q` (search query) params, if present.
+    Also preserves currentAction=selection, if is set.
+
+    Returns:
+        A URL path
+    """
+    seach_query_specs = request.normalized_params.getall('q')
+    seach_query_url = urlencode([("q", seach_query) for seach_query in seach_query_specs])
+    # types_url will always be present (always >=1 doc_type)
+    types_url = urlencode([("type", typ) for typ in doc_types])
+    current_action = request.normalized_params.get('currentAction')
+
+    clear_qs = types_url or ''
+    if seach_query_url:
+        clear_qs += '&' + seach_query_url
+    if current_action == 'selection':
+        clear_qs += '&currentAction=selection'
+    current_search_sort = request.normalized_params.getall('sort')
+    current_search_sort_url = urlencode([("sort", s) for s in current_search_sort])
+    if current_search_sort_url:
+        clear_qs += '&' + current_search_sort_url
+    return request.route_path(forced_type.lower(), slash='/') + (('?' + clear_qs) if clear_qs else '')
 
-                # If schema for field is not found (and range_type thus not set),
-                # then treated as ordinary term filter (likely will get 0 results)
-                field_schema = schema_for_field(f_field, request, doc_types)
-                if field_schema:
-                    range_type = 'date' if determine_if_is_date_field(f_field, field_schema) else 'numerical'
 
-            # Add filter to result
+def build_type_filters(result, request, doc_types, types):
+    """
+    Set the type filters for the search. If no doc_types, default to Item
+    """
+    if not doc_types:
+        doc_types = ['Item']
+    else:
+        for item_type in doc_types:
+            ti = types[item_type]
             qs = urlencode([
                 (k.encode('utf-8'), v.encode('utf-8'))
-                for k, v in request.normalized_params.items()
-                if k != "limit" and k != "from" and not (k == field and v == term)
+                for k, v in request.normalized_params.items() if not (k == 'type' and types.all.get('Item' if v == '*' else v) is ti)
             ])
-            remove_path = '{}?{}'.format(request.path, qs)
-
-            # default to searching type=Item rather than empty filter path
-            if remove_path[-1] == '?':
-                remove_path += 'type=Item'
-
             result['filters'].append({
-                'field': field,
-                'term': term,
-                'remove': remove_path
+                'field': 'type',
+                'term': ti.name,
+                'remove': '{}?{}'.format(request.path, qs)
             })
 
-            # handle NOT
-            if field.endswith('!'):
-                field = field[:-1]
-                not_field = True
-
-            # Add filter to query
-            if range_type and f_field and range_type in ('date', 'numerical'):
-                query_field = 'embedded.' + f_field
-            elif field.startswith('validation_errors') or field.startswith('aggregated_items'):
-                query_field = field + '.raw'
-            elif field == 'type':
-                query_field = 'embedded.@type.raw'
+
+def prepare_search_term(request):
+    """
+    Prepares search terms by making a dictionary where the keys are fields
+    and the values are arrays of query strings
+    Ignore certain keywords, such as type, format, and field
+    """
+    prepared_terms = {}
+    # prepared_vals = []
+    # In case it helps, I think request.normalized_params is a MultiDict. -kmp 7-Aug-2022
+    for field, val in request.normalized_params.items():  # was .iteritems(), but that went away in Python 3
+        if field.startswith('validation_errors') or field.startswith('aggregated_items'):
+            continue
+        elif field == 'q':  # searched string has field 'q'
+            # people shouldn't provide multiple queries, but if they do,
+            # combine them with AND logic
+            if 'q' in prepared_terms:
+                join_list = [prepared_terms['q'], val]
+                prepared_terms['q'] = ' AND '.join(join_list)
             else:
-                query_field = 'embedded.' + field + '.raw'
+                prepared_terms['q'] = val
+        elif field not in COMMON_EXCLUDED_URI_PARAMS + ['type']:
+            if 'embedded.' + field not in prepared_terms.keys():
+                prepared_terms['embedded.' + field] = []
+            prepared_terms['embedded.' + field].append(val)
+    return prepared_terms
 
-            if range_type:
-                if query_field not in range_filters:
-                    range_filters[query_field] = {}
-                    if range_type == 'date':
-                        range_filters[query_field]['format'] = 'yyyy-MM-dd HH:mm'
-
-                if range_direction in cls.RANGE_DIRECTIONS:
-                    if range_type == "date" and len(term) == 10:  # TODO: refactor to use regex -Will 06/24/2020
-                        # Correct term to have hours, e.g. 00:00 or 23:59, if not otherwise supplied.
-                        if range_direction == 'gt' or range_direction == 'lte':
-                            term += ' 23:59'
-                        elif range_direction == 'gte' or range_direction == 'lt':
-                            term += ' 00:00'
 
-                    if range_filters[query_field].get(range_direction) is None:
-                        range_filters[query_field][range_direction] = term
-                    else:
-                        # If have a value already (e.g. multiple ranges selected), choose the widening option.
-                        if range_direction == 'gt' or range_direction == 'gte':
-                            if term < range_filters[query_field][range_direction]:
-                                range_filters[query_field][range_direction] = term
-                        elif range_direction == 'lt' or range_direction == 'lte':
-                            if term > range_filters[query_field][range_direction]:
-                                range_filters[query_field][range_direction] = term
-
-                # Check if schema requests no value
-                if 'items' in field_schema:  # we are searching on an array of numerics
-                    field_schema = field_schema['items']
-                if field_schema.get('add_no_value', False) and cls.range_includes_zero(range_filters[query_field]):
-                    range_filters[query_field]['add_no_value'] = True
+def set_doc_types(request, types, search_type):
+    """
+    Set the type of documents resulting from the search; order and check for
+    invalid types as well. If a forced search_type is enforced, use that;
+    otherwise, set types from the query params. Default to Item if none set.
+
+    Args:
+        request: the current Request
+        types: registry[TYPES]
+        search_type (str): forced search item type
 
-            # add these to field_filters directly, handle later with build_sub_queries
-            else:
-                if query_field not in field_filters:
-                    field_filters[query_field] = {
-                        'must_terms': [],
-                        'must_not_terms': [],
-                        'add_no_value': None
-                    }
+    Returns:
+        list: the string item types to use for the search
 
-                # handle case of filtering for null values
-                if exists_field:
-                    # the value below is True when we want to include 'No value' as a filter
-                    field_filters[query_field]['add_no_value'] = False if not_field else True
-                    continue
+    Raises:
+        HTTPBadRequest: if an invalid item type is supplied
+    """
+    doc_types = []
+    if search_type is None:
+        doc_types = request.params.getall('type')
+        if '*' in doc_types:
+            doc_types = ['Item']
+    else:
+        doc_types = [search_type]
+    # Normalize to item_type
+    try:
+        doc_types = sorted({types[name].name for name in doc_types})
+    except KeyError:
+        # Check for invalid types
+        bad_types = [t for t in doc_types if t not in types]
+        msg = "Invalid type: {}".format(', '.join(bad_types))
+        raise HTTPBadRequest(explanation=msg)
+    if len(doc_types) == 0:
+        doc_types = ['Item']
+    return doc_types
 
-                if not_field:
-                    field_filters[query_field]['must_not_terms'].append(term)
-                else:
-                    field_filters[query_field]['must_terms'].append(term)
 
-        return range_filters
+def get_search_fields(request, doc_types):
+    """
+    Returns set of columns that are being searched and highlights
+    """
+    fields = {'uuid'}
+    highlights = {}
+    types = request.registry[TYPES]
+    for doc_type in doc_types:
+        type_info = types[doc_type]
+        for value in type_info.schema.get('boost_values', ()):
+            fields.add('embedded.' + value)
+            highlights['embedded.' + value] = {}
+    return fields, highlights
 
-    @staticmethod
-    def initialize_field_filters(request, principals, doc_types):
-        """ Helper function for build_filters
-            Initializes field filters with filters that exist on all searches, does some basic updates
-        """
-        field_filters = {
-            'principals_allowed.view': {
-                'must_terms': principals,
-                'must_not_terms': [],
-                'add_no_value': None
-            },
-            'embedded.@type.raw': {
-                'must_terms': doc_types,
-                'must_not_terms': [],
-                'add_no_value': None
-            },
-            'embedded.status.raw': {
-                'must_terms': [],
-                'must_not_terms': [],
-                'add_no_value': None
-            }
-        }
 
-        # Exclude status=deleted Items unless explicitly requested/filtered-in.
-        if 'deleted' not in request.normalized_params.getall('status'):
-            field_filters['embedded.status.raw']['must_not_terms'].append('deleted')
-        if 'replaced' not in request.normalized_params.getall('status'):
-            field_filters['embedded.status.raw']['must_not_terms'].append('replaced')
-
-        # Exclude type=TrackingItem and type=OntologyTerm from results unless are explictly specified
-        if 'TrackingItem' not in doc_types:
-            field_filters['embedded.@type.raw']['must_not_terms'].append('TrackingItem')
-        if 'OntologyTerm' not in doc_types:
-            field_filters['embedded.@type.raw']['must_not_terms'].append('OntologyTerm')
-
-        return field_filters
-
-    @staticmethod
-    def build_nested_query(nested_path, query):
-        """ Takes the given query and converts it into a nested query on the
-            given path.
-        """
-        return {
-            NESTED: {
-                PATH: nested_path,
-                QUERY: query
+def list_source_fields(request, doc_types, frame):
+    """
+    Returns set of fields that are requested by user or default fields.
+    These fields are used to further limit the results from the search.
+    Note that you must provide the full fieldname with embeds, such as:
+    'field=biosample.biosource.individual.organism.name' and not just
+    'field=name'
+    """
+    fields_requested = request.normalized_params.getall('field')
+    if fields_requested:
+        fields = ['embedded.@id', 'embedded.@type']
+        for field in fields_requested:
+            fields.append('embedded.' + field)
+    elif frame in ['embedded', 'object', 'raw']:
+        if frame != 'embedded':
+            # frame=raw corresponds to 'properties' in ES
+            if frame == 'raw':
+                frame = 'properties'
+            # let embedded be searched as well (for faceting)
+            fields = ['embedded.*', frame + '.*']
+        else:
+            fields = [frame + '.*']
+    else:
+        fields = ['embedded.*']
+    return fields
+
+
+def build_query(search, prepared_terms, source_fields):
+    """
+    Prepare the query within the Search object.
+    """
+    query_info = {}
+    string_query = None
+    # set _source fields for the search
+    search = search.source(list(source_fields))
+    # prepare the query from prepared_terms
+    for field, value in prepared_terms.items():
+        if field == 'q':
+            query_info['query'] = value
+            query_info['lenient'] = True
+            query_info['default_operator'] = 'AND'
+            query_info['fields'] = ['_all']
+            break
+    if query_info != {}:
+        string_query = {'must': {'simple_query_string': query_info}}
+        query_dict = {'query': {'bool': string_query}}
+    else:
+        query_dict = {'query': {'bool': {}}}
+    search.update_from_dict(query_dict)
+    return search, string_query
+
+
+def set_sort_order(request, search, search_term, types, doc_types, result):
+    """
+    sets sort order for elasticsearch results
+    example: /search/?type=Biosource&sort=display_title
+    will sort by display_title in ascending order. To set descending order,
+    use the "-" flag: sort_by=-date_created.
+    Sorting is done alphatbetically, case sensitive by default.
+    TODO: add a schema flag for case sensitivity/insensitivity?
+
+    ES5: simply pass in the sort OrderedDict into search.sort
+    """
+    sort = OrderedDict()
+    result_sort = OrderedDict()
+    if len(doc_types) == 1:
+        type_schema = types[doc_types[0]].schema
+    else:
+        type_schema = None
+
+    def add_to_sort_dict(requested_sort):
+        if requested_sort.startswith('-'):
+            name = requested_sort[1:]
+            order = 'desc'
+        else:
+            name = requested_sort
+            order = 'asc'
+        sort_schema = type_schema.get('properties', {}).get(name) if type_schema else None
+        if sort_schema:
+            sort_type = sort_schema.get('type')
+        else:
+            sort_type = 'string'
+
+        # ES type != schema types
+        if sort_type == 'integer':
+            sort['embedded.' + name] = result_sort[name] = {
+                'order': order,
+                'unmapped_type': 'long',
+                'missing': '_last'
+            }
+        elif sort_type == 'number':
+            sort['embedded.' + name] = result_sort[name] = {
+                'order': order,
+                'unmapped_type': 'float',
+                'missing': '_last'
+            }
+        else:
+            # fallback case, applies to all string type:string fields
+            sort['embedded.' + name + '.lower_case_sort'] = result_sort[name] = {
+                'order': order,
+                'unmapped_type': 'keyword',
+                'missing': '_last'
             }
-        }
 
-    @classmethod
-    def handle_nested_filters_v2(cls, must_nested_filters, must_not_nested_filters, es_mapping):
-        """ This function implements nested query construction.
-
-            When building a nested query, unlike with traditional queries, selections on the same
-            field must occur in the same nested sub-query in order to be applied as an intersect
-            condition on the object field. Previously we would create separate nested sub-queries
-            per field selection, which causes them to be OR'd.
-
-            :param must_nested_filters: conditions filtered on in the affirmative
-            :param must_not_nested_filters: conditions filtered on in the negative
-            :param es_mapping: the ES mapping of the type we are searching on
-            :returns: a nested sub-query that can be added directly to the parent query
-        """
-        # Build base query structure
-        # always use MUST + sub queries for MUST_NOT
-        nested_query = {
-            BOOL: {
-                MUST: [],
-                MUST_NOT: [],
+    # Prefer sort order specified in request, if any
+    requested_sorts = request.normalized_params.getall('sort')
+    if requested_sorts:
+        for rs in requested_sorts:
+            add_to_sort_dict(rs)
+
+    text_search = search_term.get('q')
+
+    # Otherwise we use a default sort only when there's no text search to be ranked
+    if not sort and (text_search == '*' or not text_search):
+        # If searching for a single type, look for sort options in its schema
+        if type_schema:
+            if 'sort_by' in type_schema:
+                for k, v in type_schema['sort_by'].items():
+                    # Should always sort on raw field rather than analyzed field
+                    # OR search on lower_case_sort for case insensitive results
+                    sort['embedded.' + k + '.lower_case_sort'] = result_sort[k] = v
+        # Default is most recent first, then alphabetical by label
+        if not sort:
+            sort['embedded.date_created.raw'] = result_sort['date_created'] = {
+                'order': 'desc',
+                'unmapped_type': 'keyword',
             }
+            sort['embedded.label.raw'] = result_sort['label'] = {
+                'order': 'asc',
+                'missing': '_last',
+                'unmapped_type': 'keyword',
+            }
+    elif not sort and text_search and text_search != '*':
+        search = search.sort(                   # Multi-level sort. See http://www.elastic.co/guide/en/elasticsearch/guide/current/_sorting.html#_multilevel_sorting & https://stackoverflow.com/questions/46458803/python-elasticsearch-dsl-sorting-with-multiple-fields
+            {'_score': {"order": "desc"}},
+            {'embedded.date_created.raw': {'order': 'desc', 'unmapped_type': 'keyword'},
+             'embedded.label.raw': {'order': 'asc', 'unmapped_type': 'keyword', 'missing': '_last'}},
+            {'_uid': {'order': 'asc'}}  # 'embedded.uuid.raw' (instd of _uid) sometimes results in 400 bad request : 'org.elasticsearch.index.query.QueryShardException: No mapping found for [embedded.uuid.raw] in order to sort on'
+        )
+        result['sort'] = result_sort = {'_score': {"order": "desc"}}
+        return search
+
+    if sort and result_sort:
+        result['sort'] = result_sort
+        search = search.sort(sort)
+    return search
+
+
+def set_filters(request, search, result, principals, doc_types):
+    """
+    Sets filters in the query
+    """
+
+    # these next two dictionaries should each have keys equal to query_field
+    # and values: must_terms: [<list of terms>], must_not_terms: [<list of terms>], add_no_value: True/False/None
+    field_filters = {
+        'principals_allowed.view': {
+            'must_terms': principals,
+            'must_not_terms': [],
+            'add_no_value': None
+        },
+        'embedded.@type.raw': {
+            'must_terms': doc_types,
+            'must_not_terms': [],
+            'add_no_value': None
+        },
+        'embedded.status.raw': {
+            'must_terms': [],
+            'must_not_terms': [],
+            'add_no_value': None
         }
+    }
 
-        # Maps a nested path to a 2-tuple of it's key (must/must_not) and index
-        nested_path_to_index_map = {}
+    range_filters = {}
 
-        # Build array of key, (field, query) so we can process the filters in a single pass
-        # note that MUST queries are always processed first
-        filters_to_work_on = []
-        if must_nested_filters:
-            filters_to_work_on += zip([MUST] * len(must_nested_filters), must_nested_filters)
-        if must_not_nested_filters:
-            filters_to_work_on += zip([MUST_NOT] * len(must_not_nested_filters), must_not_nested_filters)
-
-        # Process key (must/must_not), field (target of search), query (condition)
-        # iteratively building nested_query
-        for key, (field, query) in filters_to_work_on:
-            nested_path = find_nested_path(field, es_mapping)
-
-            # if we've never seen this path before, bootstrap a sub-query for it
-            if nested_path not in nested_path_to_index_map:
-
-                # set in tracking, note it is order dependent
-                new_index = len(nested_query[BOOL][key])
-                nested_path_to_index_map[nested_path] = (key, new_index)
-
-                # this nested path could have more filters (under differing keys)
-                # bootstrap an entire sub-query for this path
-                combined_query = {
-                    BOOL: {
-                        MUST: [],
-                        MUST_NOT: []
-                    }
+    # Exclude status=deleted Items unless explicitly requested/filtered-in.
+    if 'deleted' not in request.normalized_params.getall('status'):
+        field_filters['embedded.status.raw']['must_not_terms'].append('deleted')
+    if 'replaced' not in request.normalized_params.getall('status'):
+        field_filters['embedded.status.raw']['must_not_terms'].append('replaced')
+
+    # Exclude type=TrackingItem and type=OntologyTerm from results unless are explictly specified
+    if 'TrackingItem' not in doc_types:
+        field_filters['embedded.@type.raw']['must_not_terms'].append('TrackingItem')
+    if 'OntologyTerm' not in doc_types:
+        field_filters['embedded.@type.raw']['must_not_terms'].append('OntologyTerm')
+
+    for field, term in request.normalized_params.items():
+        not_field = False  # keep track if query is NOT (!)
+        exists_field = False  # keep track of null values
+        range_type = False  # If we determine is a range request (field.to, field.from), will be populated with string 'date' or 'numerical'
+        range_direction = None
+        if field in COMMON_EXCLUDED_URI_PARAMS + ['q']:
+            continue
+        elif field == 'type' and term != 'Item':
+            continue
+        elif term == 'No value':
+            exists_field = True
+
+        # Check for date or numerical range filters
+        if (len(field) > 3 and field[-3:] == '.to') or (len(field) > 5 and field[-5:] == '.from'):
+            if field[-3:] == '.to':
+                f_field = field[:-3]
+                range_direction = "lte"
+            else:
+                f_field = field[:-5]
+                range_direction = "gte"
+
+            # If schema for field is not found (and range_type thus not set),
+            # then treated as ordinary term filter (likely will get 0 results)
+            field_schema = schema_for_field(f_field, request, doc_types)
+            if field_schema:
+                range_type = 'date' if determine_if_is_date_field(f_field, field_schema) else 'numerical'
+
+        # Add filter to result
+        qs = urlencode([
+            (k.encode('utf-8'), v.encode('utf-8'))
+            for k, v in request.normalized_params.items()
+            if (k != field or v != term)
+        ])
+        remove_path = '{}?{}'.format(request.path, qs)
+
+        # default to searching type=Item rather than empty filter path
+        if remove_path[-1] == '?':
+            remove_path += 'type=Item'
+
+        result['filters'].append({
+            'field': field,
+            'term': term,
+            'remove': remove_path
+        })
+
+        # handle NOT
+        if field.endswith('!'):
+            field = field[:-1]
+            not_field = True
+
+        # Add filter to query
+        if range_type and f_field and range_type in ('date', 'numerical'):
+            query_field = 'embedded.' + f_field
+        elif field.startswith('validation_errors') or field.startswith('aggregated_items'):
+            query_field = field + '.raw'
+        elif field == 'type':
+            query_field = 'embedded.@type.raw'
+        else:
+            query_field = 'embedded.' + field + '.raw'
+
+        if range_type:
+            if query_field not in range_filters:
+                range_filters[query_field] = {}
+                if range_type == 'date':
+                    range_filters[query_field]['format'] = 'yyyy-MM-dd HH:mm'
+
+            if range_direction in ('gt', 'gte', 'lt', 'lte'):
+                if len(term) == 10:
+                    # Correct term to have hours, e.g. 00:00 or 23:59, if not otherwise supplied.
+                    if range_direction == 'gt' or range_direction == 'lte':
+                        term += ' 23:59'
+                    elif range_direction == 'gte' or range_direction == 'lt':
+                        term += ' 00:00'
+
+                if range_filters[query_field].get(range_direction) is None:
+                    range_filters[query_field][range_direction] = term
+                else:
+                    # If have a value already (e.g. multiple ranges selected), choose the widening option.
+                    if range_direction == 'gt' or range_direction == 'gte':
+                        if term < range_filters[query_field][range_direction]:
+                            range_filters[query_field][range_direction] = term
+                    elif range_direction == 'lt' or range_direction == 'lte':
+                        if term > range_filters[query_field][range_direction]:
+                            range_filters[query_field][range_direction] = term
+        else:
+            if query_field not in field_filters:
+                field_filters[query_field] = {
+                    'must_terms': [],
+                    'must_not_terms': [],
+                    'add_no_value': None
                 }
-                for sub_query in query:
-                    # Special case for EXISTS, since we cannot construct these like normal
-                    # queries - add DOES NOT EXIST queries to MUST branches, as these are
-                    # automatically added to MUST_NOT branch
-                    if EXISTS in sub_query and key == MUST_NOT:
-                        combined_query[BOOL][MUST].append(sub_query)
-                    elif sub_query.get(BOOL, {}).get(MUST, {}).get(EXISTS, None):
-                        combined_query[BOOL][MUST].append(sub_query)
-                    else:
-                        combined_query[BOOL][key].append(sub_query)
 
-                # add the combined_query for this nested path to the global nested query
-                nested_query[BOOL][key].append(cls.build_nested_query(nested_path, combined_query))
+            # handle case of filtering for null values
+            if exists_field:
+                # the value below is True when we want to include 'No value' as a filter
+                field_filters[query_field]['add_no_value'] = False if not_field else True
+                continue
 
-            # We have seen this nested_path before, so in order to achieve proper intersect
-            # behavior all conditions must be present on the same nested sub-query
+            if not_field:
+                field_filters[query_field]['must_not_terms'].append(term)
             else:
+                field_filters[query_field]['must_terms'].append(term)
 
-                # extract the location of the nested query we would like to add to
-                # note that the key under which the previous query was added could differ
-                # from the key we are seeing now ie: EXIST (must) combined with != (must_not)
-                prev_key, path_index = nested_path_to_index_map[nested_path]
-                leaf_query = nested_query[BOOL][prev_key][path_index][NESTED][QUERY][BOOL][key]
-
-                # leaf_query is the sub-query we want to build off of
-                # its possible our current query contains multiple conditions
-                if isinstance(query, list):
-                    leaf_query += query
-                elif isinstance(query, dict):
-                    leaf_query.append(query)
-                else:
-                    raise QueryConstructionException(
-                        query_type='nested',
-                        func='handle_nested_filters_v2',
-                        msg='passed a query with a bad type: %s' % query
-                    )
+    must_filters = []
+    must_not_filters = []
+    for query_field, filters in field_filters.items():
+        must_terms = {'terms': {query_field: filters['must_terms']}} if filters['must_terms'] else {}
+        must_not_terms = {'terms': {query_field: filters['must_not_terms']}} if filters['must_not_terms'] else {}
+        if filters['add_no_value'] is True:
+            # add to must_not in an OR case, which is equivalent to filtering on 'No value'
+            should_arr = [must_terms] if must_terms else []
+            should_arr.append({'bool': {'must_not': {'exists': {'field': query_field}}}})
+            must_filters.append({'bool': {'should': should_arr}})
+        elif filters['add_no_value'] is False:
+            # add to must_not in an OR case, which is equivalent to filtering on '! No value'
+            should_arr = [must_terms] if must_terms else []
+            should_arr.append({'exists': {'field': query_field}})
+            must_filters.append({'bool': {'should': should_arr}})
+        else:  # no filtering on 'No value'
+            if must_terms:
+                must_filters.append(must_terms)
+        if must_not_terms:
+            must_not_filters.append(must_not_terms)
+
+    # lastly, add range limits to filters if given
+    for range_field, range_def in range_filters.items():
+        must_filters.append({
+            'range': {range_field: range_def}
+        })
+
+    # To modify filters of elasticsearch_dsl Search, must call to_dict(),
+    # modify that, then update from the new dict
+    prev_search = search.to_dict()
+    # initialize filter hierarchy
+    final_filters = {'bool': {'must': must_filters, 'must_not': must_not_filters}}
+    prev_search['query']['bool']['filter'] = final_filters
+    search.update_from_dict(prev_search)
 
-        return nested_query
+    return search, final_filters
 
-    @classmethod
-    def build_filters(cls, request, query, result, principals, doc_types, es_mapping):
-        """
-        This function builds the Elasticsearch query based on the request. The structure of the query
-        is approximately represented below. 'Approximate' because you could not copy-paste directly into
-        Lucene, but should illustrate enough so it is comprehensible. Note the 'nested' nature of the query.
-
-        QUERY HIERARCHY ('approximate' lucene syntax):
-            {
-                'query': {
-                    'bool': {
-                        'filter': {
-                            'bool': {
-                                'must': {
-                                    <positive+range sub-queries>
-                                    +
-                                    'bool': {
-                                        'should': { option1, option2 ... }
-                                    }
-                                },
-                                'must_not': {
-                                    <negative sub-queries>
-                                    +
-                                    'bool': {
-                                        'should': { option1, option2 ...
-                                }}}}}
-            }
-        There are several different sub-queries, but most of them are built using 'bool' -> 'must'.
-        A brief overview follows.
-            * nested data type sub-queries have a special format. See 'handle_nested_filters'.
-            * range filter sub-queries also have their own special format. See 'apply_range_filters'. Note that
-                the format is extra special when you're applying a range filter to a nested data type.
-            * 'terms' filters are what we 'normally' use.
-
-        :param request: Current request
-        :param query: Current search query body
-        :param result: Response to be returned from the view ('/search')
-        :param principals: Active user roles
-        :param doc_types: Document type we are searching on
-        :param es_mapping: Elasticsearch mapping of the document type we're searching on
-        :returns: 2-tuple containing the updated search based on the request parameters and
-                  information on the filters used in the query.
-        """
 
-        # these next two dictionaries should each have keys equal to query_field
-        # and values: must_terms: [<list of terms>], must_not_terms: [<list of terms>], add_no_value: True/False/None
-        field_filters = cls.initialize_field_filters(request, principals, doc_types)
-        range_filters = cls.handle_range_filters(request, result, field_filters, doc_types)
-
-        # construct queries
-        must_filters, must_not_filters, \
-        must_filters_nested, must_not_filters_nested = cls.build_sub_queries(field_filters, es_mapping)
-
-        # initialize filter hierarchy
-        final_filters = {BOOL: {MUST: [f for _, f in must_filters], MUST_NOT: [f for _, f in must_not_filters]}}
-
-        # Build nested queries
-        final_nested_query = cls.handle_nested_filters_v2(must_filters_nested, must_not_filters_nested, es_mapping)
-        final_filters[BOOL][MUST].append(final_nested_query)
-
-        # add range filters after (so nested ranges can be applied with existing nested queries)
-        cls.apply_range_filters(range_filters, final_filters[BOOL][MUST], es_mapping)
-
-        # at this point, final_filters is valid lucene and can be dropped into the query directly
-        query[QUERY][BOOL][FILTER] = final_filters
-        return query, final_filters
-
-    @staticmethod
-    def _check_and_remove(compare_field, facet_filters, active_filter, query_field, filter_type):
-        """ Does the actual 'check and removal' since this code is duplicated throughout. """
-        if compare_field == query_field:
-            facet_filters[filter_type].remove(active_filter)
-            return True
-        return False
-
-    @classmethod
-    def _check_and_remove_terms(cls, facet_filters, active_filter, query_field, filter_type):
-        """ Helper function for _remove_from_active_filters that handles filter removal for terms query """
-        # there should only be one key here
-        for compare_field in active_filter[TERMS].keys():
-            # remove filter for a given field for that facet
-            # skip this for type facet (field = 'type')
-            # since we always want to include that filter.
-            if (query_field != 'embedded.@type.raw' and  # this evaluation order MUST be preserved!
-                    cls._check_and_remove(compare_field, facet_filters, active_filter, query_field, filter_type)):
-                break
+def initialize_facets(request, doc_types, prepared_terms, schemas):
+    """
+    Initialize the facets used for the search. If searching across multiple
+    doc_types, only use the default 'Data Type' and 'Status' facets.
+    Add facets for custom url filters whether or not they're in the schema
+
+    Args:
+        doc_types (list): Item types (@type) for which we are performing a search for.
+        prepared_terms (dict): terms to match in ES, keyed by ES field name.
+        schemas (list): List of OrderedDicts of schemas for doc_types.
 
-    @classmethod
-    def _check_and_remove_range(cls, facet_filters, active_filter, query_field, filter_type):
-        """ Helper function for _remove_from_active_filters that handles filter removal for terms query """
-        for compare_field in active_filter[RANGE].keys():
-            if cls._check_and_remove(compare_field, facet_filters, active_filter, query_field, filter_type):
-                break
+    Returns:
+        list: tuples containing (0) ElasticSearch-formatted field name (e.g. `embedded.status`) and (1) list of terms for it.
+    """
 
-    @classmethod
-    def _check_and_remove_bool_should(cls, facet_filters, active_filter, query_field, filter_type):
-        """ Helper function for _remove_from_active_filters that handles filter removal for boolean queries that
-            have multiple options (inner SHOULD query)
-        """
-        # handle No value case
-        inner_bool = None
-        inner_should = active_filter.get(BOOL).get(SHOULD, [])
-        for or_term in inner_should:
-            # this may be naive, but assume first non-terms
-            # filter is the No value query
-            if TERMS in or_term or RANGE in or_term:
-                continue
+    facets = [
+        # More facets will be appended to this list from item schema plus from any currently-active filters (as requested in URI params).
+        ('type', {'title': 'Data Type'})
+    ]
+    append_facets = [
+        # Facets which will be appended after those which are in & added to `facets`
+        ('status', {'title': 'Status'}),
+
+        # TODO: Re-enable below line if/when 'range' URI param queries for date & numerical fields are implemented.
+        # ('date_created', {'title': 'Date Created', 'hide_from_view' : True, 'aggregation_type' : 'date_histogram' })
+    ]
+    validation_error_facets = [
+        ('validation_errors.name', {'title': 'Validation Errors', 'order': 999})
+    ]
+    # hold disabled facets from schema; we also want to remove these from the prepared_terms facets
+    disabled_facets = []
+
+    # Add facets from schema if one Item type is defined.
+    # Also, conditionally add extra appendable facets if relevant for type from schema.
+    if len(doc_types) == 1 and doc_types[0] != 'Item':
+        current_type_schema = request.registry[TYPES][doc_types[0]].schema
+        if 'facets' in current_type_schema:
+            schema_facets = OrderedDict(current_type_schema['facets'])
+            for schema_facet in schema_facets.items():
+                if schema_facet[1].get('disabled', False):
+                    disabled_facets.append(schema_facet[0])
+                    continue  # Skip disabled facets.
+                facets.append(schema_facet)
+
+    # == Add facets for any non-schema ?field=value filters requested in the search (unless already set) ==
+    used_facets = [facet[0] for facet in facets + append_facets]
+    used_facet_titles = [facet[1]['title']
+                         for facet in facets + append_facets
+                         if 'title' in facet[1]]
+    for field in prepared_terms:
+        if field.startswith('embedded'):
+            split_field = field.strip().split('.')  # Will become, e.g. ['embedded', 'experiments_in_set', 'files', 'file_size', 'from']
+            use_field = '.'.join(split_field[1:])
+
+            # 'terms' is the default per-term bucket aggregation for all non-schema facets
+            aggregation_type = 'terms'
+
+            # Use the last part of the split field to get the field title
+            title_field = split_field[-1]
+
+            # if searching for a display_title, use the title of parent object
+            # use `is_object_title` to keep track of this
+            if title_field == 'display_title' and len(split_field) > 1:
+                title_field = split_field[-2]
+                is_object_title = True
             else:
-                inner_bool = or_term
-                break
-        if EXISTS in inner_bool:
-            compare_field = inner_bool[EXISTS].get(FIELD)
-        else:
-            # attempt to get the field from the alternative No value syntax
-            compare_field = inner_bool.get(BOOL, {}).get(MUST_NOT, {}).get(EXISTS, {}).get(FIELD)
-        if query_field != 'embedded.@type.raw':
-            cls._check_and_remove(compare_field, facet_filters, active_filter, query_field, filter_type)
-
-    @classmethod
-    def _check_and_remove_match_from_should(cls, query_options, facet_filters, active_filter, query_field,
-                                            filter_type):
-        """ Helper function that searches a MATCH query for the given query_field, removing the
-            active filter if found.
-        """
-        for inner_query in query_options:
-            if MATCH in inner_query:
-                for field in inner_query.get(MATCH, {}).keys():  # should be only one per block
-                    if cls._check_and_remove(field, facet_filters, active_filter, query_field,
-                                             filter_type):
-                        return
+                is_object_title = False
+
+            if title_field in used_facets or title_field in disabled_facets:
+                # Cancel if already in facets or is disabled
+                continue
+
+            # If we have a range filter in the URL,
+            if title_field == 'from' or title_field == 'to':
+                if len(split_field) == 3:
+                    f_field = split_field[-2]
+                    field_schema = schema_for_field(f_field, request, doc_types)
+                    if field_schema:
+                        title_field = f_field
+                        use_field = '.'.join(split_field[1:-1])
+                        aggregation_type = 'stats'
+
+            for schema in schemas:
+                if title_field in schema['properties']:
+                    title_field = schema['properties'][title_field].get('title', title_field)
+                    # see if the title field conflicts for is_object_title facets
+                    if is_object_title and title_field in used_facet_titles:
+                        title_field += ' (Title)'
+                    break
+
+            facet_tuple = (use_field, {'title': title_field, 'aggregation_type': aggregation_type})
+
+            # At moment is equivalent to `if aggregation_type == 'stats'`` until/unless more agg types are added for _facets_.
+            if aggregation_type != 'terms':
+                facet_tuple[1]['hide_from_view'] = True  # Temporary until we handle these better on front-end.
+                # Facet would be otherwise added twice if both `.from` and `.to` are requested.
+                if facet_tuple in facets:
+                    continue
+
+            facets.append(facet_tuple)
+
+    # Append additional facets (status, validation_errors, ...) at the end of
+    # list unless were already added via schemas, etc.
+    used_facets = [facet[0] for facet in facets]  # Reset this var
+    for ap_facet in append_facets + validation_error_facets:
+        if ap_facet[0] not in used_facets:
+            facets.append(ap_facet)
+        else:  # Update with better title if not already defined from e.g. requested filters.
+            existing_facet_index = used_facets.index(ap_facet[0])
+            if facets[existing_facet_index][1].get('title') in (None, facets[existing_facet_index][0]):
+                facets[existing_facet_index][1]['title'] = ap_facet[1]['title']
+
+    return facets
+
+
+def schema_for_field(field, request, doc_types, should_log=False):
+    """
+    Find the schema for the given field (in embedded '.' format). Uses
+    ff_utils.crawl_schema from snovault and logs any cases where there is an
+    error finding the field from the schema
+
+    Args:
+        field (string): embedded field path, separated by '.'
+        request: current Request object
+        doc_types (list): @types for the search
+        should_log (bool): logging will only occur if set to True
+
+    Returns:
+        Dictionary schema for the field, or None if not found
+    """
+    types = request.registry[TYPES]
+    schemas = [types[dt].schema
+               for dt in doc_types]
+
+    # We cannot hash dict by list (of doc_types) so we convert to unique ordered string
+    doc_type_string = ','.join(doc_types)
+
+    cache = getattr(request, '_field_schema_cache', {})
+    if (field, doc_type_string) in cache:
+        return cache[(field, doc_type_string)]
+
+    field_schema = None
+
+    # for 'validation_errors.*' and 'aggregated_items.*',
+    # schema will never be found and logging isn't helpful
+    if (schemas
+            and not field.startswith('validation_errors.')
+            and not field.startswith('aggregated_items.')):
+        # 'type' field is really '@type' in the schema
+        use_field = '@type' if field == 'type' else field
+        # eliminate '!' from not fields
+        use_field = use_field[:-1] if use_field.endswith('!') else use_field
+        for schema in schemas:
+            try:
+                field_schema = crawl_schema(types, use_field, schema)
+            except Exception as exc:  # cannot find schema. Log and Return None
+                if should_log:
+                    log.warning(f'Cannot find schema in search.py. Type: {doc_types[0]}. Field: {field}',
+                                field=field, error=str(exc))
             else:
-                search_log(log_handler=log, msg='Encountered a unexpected nested structure in '
-                                                'query: %s' % inner_query)
+                if field_schema is not None:
+                    break
 
-    @classmethod
-    def _check_and_remove_nested(cls, facet_filters, active_filter, query_field, filter_type):
-        """ Helper function for _remove_from_active_filters that handles filter removal for nested query
-            Reminder that this code is responsible for constructing the aggregation filter, hence the desire
-            to omit selections on the field we are aggregating on.
-        """
-        nested_sub_query = active_filter[NESTED][QUERY]
+    # Cache result, even if not found, for this request.
+    cache[(field, doc_type_string)] = field_schema
+    if not hasattr(request, '_field_schema_cache'):
+        setattr(request, '_field_schema_cache', cache)
+
+    return field_schema
 
-        # For No value searches
-        if EXISTS in nested_sub_query:
-            field = nested_sub_query.get(EXISTS, {}).get(FIELD)
-            cls._check_and_remove(field, facet_filters, active_filter, query_field, filter_type)
-
-        # For all other searches
-        elif BOOL in nested_sub_query:
-            for inner_filter_type in [MUST, MUST_NOT]:
-                for nested_option in nested_sub_query[BOOL].get(inner_filter_type, []):
-                    if isinstance(nested_option, dict):
-
-                        # For structure like this:
-                        #   {'bool': {'must': [{'match': {'embedded.hg19.hg19_hgvsg.raw': 'NC_000001.11:g.12185956del'}]
-                        if MATCH in nested_option:
-                            for field in nested_option.get(MATCH, {}).keys():  # should only be one per block
-                                if cls._check_and_remove(field, facet_filters, active_filter, query_field, filter_type):
-                                    break
-
-                        # For structure like this:
-                        # {'bool': {'should':
-                        # [{'match': {'embedded.variant.genes.genes_most_severe_consequence.coding_effect.raw':
-                        #       'Missense'}},
-                        # {'match': {'embedded.variant.genes.genes_most_severe_consequence.coding_effect.raw':
-                        #       'Synonymous'}}]}}
-                        elif BOOL in nested_option:
-                            inner_inner_bool = nested_option[BOOL]
-                            if SHOULD in inner_inner_bool:
-                                cls._check_and_remove_match_from_should(inner_inner_bool[SHOULD], facet_filters,
-                                                                        active_filter,
-                                                                        query_field, filter_type)
-
-                    # For structure like this:
-                    #   {'bool': {'must': {'bool': {'should':
-                    #       [{'match': {'embedded.hg19.hg19_hgvsg.raw': 'NC_000001.11:g.12185956del'}},
-                    #       {'match': {'embedded.hg19.hg19_hgvsg.raw': 'NC_000001.11:g.11901816A>T'}}]}}}}
-                    elif isinstance(nested_option, str):
-                        inner_bool = nested_sub_query[BOOL].get(inner_filter_type, {})
-                        if SHOULD in inner_bool:
-                            cls._check_and_remove_match_from_should(inner_bool[SHOULD], facet_filters, active_filter,
-                                                                    query_field, filter_type)
-
-                        # For structure like this:
-                        # {'bool': {'should': [
-                        #    {'match': {'embedded.variant.genes.genes_most_severe_consequence.impact.raw': 'MODIFIER'}},
-                        #    {'match': {'embedded.variant.genes.genes_most_severe_consequence.impact.raw': 'LOW'}}]}}
-                        elif BOOL in inner_bool:
-                            inner_inner_bool = inner_bool[BOOL]
-                            if SHOULD in inner_inner_bool:
-                                cls._check_and_remove_match_from_should(inner_inner_bool[SHOULD], facet_filters, active_filter,
-                                                                        query_field, filter_type)
 
+def is_linkto_or_object_array_root_field(field, types, doc_types):
+    """Not used currently. May be useful for if we want to enabled "type" : "nested" mappings on lists of dictionaries"""
+    schema = types[doc_types[0]].schema
+    field_root = field.split('.')[0]
+    fr_schema = (schema and schema.get('properties', {}).get(field_root, None)) or None
+    if fr_schema and fr_schema['type'] == 'array' and (fr_schema['items'].get('linkTo') is not None or fr_schema['items']['type'] == 'object'):
+        return True
+    return False
+
+
+def generate_filters_for_terms_agg_from_search_filters(query_field, search_filters, string_query):
+    """
+    We add a copy of our filters to each facet, minus that of
+    facet's field itself so that we can get term counts for other terms filters.
+    And be able to filter w/ it.
+
+    Remove filters from fields they apply to.
+    For example, the 'biosource_type' aggs should not have any
+    biosource_type filter in place.
+    Handle 'must' and 'must_not' filters separately
+
+    Returns
+        Copy of search_filters, minus filter for current query_field (if one set).
+    """
+
+    facet_filters = deepcopy(search_filters['bool'])
+
+    for filter_type in ['must', 'must_not']:
+        if not search_filters['bool'][filter_type]:
+            continue
+        for active_filter in search_filters['bool'][filter_type]:  # active_filter => e.g. { 'terms' : { 'embedded.@type.raw': ['ExperimentSetReplicate'] } }
+            if 'bool' in active_filter and 'should' in active_filter['bool']:
+                # handle No value case
+                inner_bool = None
+                inner_should = active_filter.get('bool').get('should', [])
+                for or_term in inner_should:
+                    # this may be naive, but assume first non-terms
+                    # filter is the No value quqery
+                    if 'terms' in or_term:
+                        continue
                     else:
-                        search_log(log_handler=log, msg='Encountered a unexpected nested structure at top level: %s'
-                                                        % nested_sub_query[BOOL])
+                        inner_bool = or_term
+                        break
+                if 'exists' in inner_bool:
+                    compare_field = inner_bool['exists'].get('field')
+                else:
+                    # attempt to get the field from the alternative No value syntax
+                    compare_field = inner_bool.get('bool', {}).get('must_not', {}).get('exists', {}).get('field')
+                if compare_field == query_field and query_field != 'embedded.@type.raw':
+                    facet_filters[filter_type].remove(active_filter)
+
+            if 'terms' in active_filter:
+                # there should only be one key here
+                for compare_field in active_filter['terms'].keys():
+                    # remove filter for a given field for that facet
+                    # skip this for type facet (field = 'type')
+                    # since we always want to include that filter.
+                    if compare_field == query_field and query_field != 'embedded.@type.raw':
+                        facet_filters[filter_type].remove(active_filter)
+
+            elif 'range' in active_filter:
+                for compare_field in active_filter['range'].keys():
+                    # Do same as for terms
+                    if compare_field == query_field:
+                        facet_filters[filter_type].remove(active_filter)
+
+    # add the string_query, if present, to the bool term with facet_filters
+    if string_query and string_query['must']:
+        # combine statements within 'must' for each
+        facet_filters['must'].append(string_query['must'])
 
-    @classmethod
-    def _remove_from_active_filters(cls, facet_filters, query_field, active_filter, filter_type):
-        """ Helper function for generate_filters_for_terms_agg_from_search_filters
-            Modifies facet_filters in place to remove the active_filter if it matches
-            the given query field.
-            This function is intended to be called on every "sub part" of the base query
-            for every aggregation.
-
-            TODO: Optimize this - it is inefficient application side regardless of the dominating ES cost
-
-            :param facet_filters: intended filter block to be used on the aggregation
-            :param query_field: field that we are aggregating on
-            :param active_filter: which "sub part" of the facet filters we are examining
-            :param filter_type: one of MUST or MUST_NOT
-        """
-        if BOOL in active_filter and SHOULD in active_filter[BOOL]:
-            cls._check_and_remove_bool_should(facet_filters, active_filter, query_field, filter_type)
-        elif TERMS in active_filter:
-            cls._check_and_remove_terms(facet_filters, active_filter, query_field, filter_type)
-        elif RANGE in active_filter:
-            cls._check_and_remove_range(facet_filters, active_filter, query_field, filter_type)
-        elif NESTED in active_filter:
-            cls._check_and_remove_nested(facet_filters, active_filter, query_field, filter_type)
+    return facet_filters
 
-    @classmethod
-    def generate_filters_for_terms_agg_from_search_filters(cls, query_field, search_filters, string_query):
-        """
-        We add a copy of our filters to each facet, minus that of
-        facet's field itself so that we can get term counts for other terms filters.
-        And be able to filter w/ it.
-        Remove filters from fields they apply to.
-        For example, the 'biosource_type' aggs should not have any
-        biosource_type filter in place.
-        Handle 'must' and 'must_not' filters separately
-
-        :param query_field: field terms agg is on
-        :param search_filters: intermediary format prior to any valid lucene representing the search_filters
-                               from the front-end
-        :param string_query: query string if provided
-        :return: Copy of search_filters, minus filter for current query_field (if one set).
-        """
-        if not search_filters or BOOL not in search_filters:  # a sane default if this happens -Will 11/17/20
-            log.error('Encountered an unexpected query format: %s' % search_filters)
-            return {BOOL: {MUST: [{TERMS: {'principals_allowed.view': ['system.Everyone']}}]}}
-
-        facet_filters = deepcopy(search_filters[BOOL])
-
-        for filter_type in [MUST, MUST_NOT]:
-            # active_filter => e.g. { 'terms' : { 'embedded.@type.raw': ['ExperimentSetReplicate'] } }
-            for active_filter in search_filters[BOOL][filter_type]:
-                cls._remove_from_active_filters(facet_filters, query_field, active_filter, filter_type)
-
-        # add the string_query, if present, to the bool term with facet_filters
-        if string_query and string_query[MUST]:
-            # combine statements within 'must' for each
-            facet_filters[MUST].append(string_query[MUST])
 
-        return {BOOL: facet_filters}
+def set_facets(search, facets, search_filters, string_query, request, doc_types, custom_aggregations=None,
+               size=25, from_=0):
+    """
+    Sets facets in the query as ElasticSearch aggregations, with each aggregation to be
+    filtered by search_filters minus filter affecting facet field in order to get counts
+    for other facet term options.
+    ES5 - simply sets aggs by calling update_from_dict after adding them in
+
+        :param facets:         Facet field (0) in object dot notation, and a dict or OrderedDict with title property (1).
+        :type  facets:         List of tuples.
+        :param search_filters: Dict of filters which are set for the ES query in set_filters
+        :param string_query:   Dict holding the query_string used in the search
+    """
 
-    @staticmethod
-    def set_additional_aggregations(search_as_dict, request, doc_types, extra_aggregations=None):
-        """
-        Per-type aggregations may be defined in schemas. Apply them OUTSIDE of globals so they act on our
-        current search filters. Warning: `search_as_dict` is modified IN PLACE.
+    if from_ != 0:
+        return search
 
-        :param search_as_dict: elasticsearch_dsl object converted to_dict()
-        :param request: current request
-        :param doc_types: types we are searching on
-        :param extra_aggregations: aggregations to add
-        :return: search_as_dict, same as originally passed in, but modified in this function
-        """
+    aggs = OrderedDict()
 
-        types = request.registry[TYPES]
-        schema = types[doc_types[0]].schema
+    for field, facet in facets:  # E.g. 'type','experimentset_type','experiments_in_set.award.project', ...
+        field_schema = schema_for_field(field, request, doc_types, should_log=True)
+        is_date_field = field_schema and determine_if_is_date_field(field, field_schema)
+        is_numerical_field = field_schema and field_schema['type'] in ("integer", "float", "number")
 
-        if schema.get('aggregations'):
-            for schema_agg_name in schema['aggregations'].keys():
-                if schema_agg_name == 'all_items':
-                    raise QueryConstructionException(
-                        query_type='aggregations',
-                        func='set_additional_aggregations',
-                        msg='all_items is a reserved agg name and not allowed as an extra aggregation name.')
-                search_as_dict['aggs'][schema_agg_name] = schema['aggregations'][schema_agg_name]
-
-        if extra_aggregations:
-            for extra_agg_name in extra_aggregations.keys():
-                if extra_agg_name == 'all_items':
-                    raise QueryConstructionException(
-                        query_type='extra_aggregations',
-                        func='set_additional_aggregations',
-                        msg='all_items is a reserved agg name and not allowed as an extra aggregation name.')
-                search_as_dict['aggs'][extra_agg_name] = extra_aggregations[extra_agg_name]
-
-        return search_as_dict
-
-    @staticmethod
-    def _build_nested_aggregation(sub_query, nested_path, requested=None):
-        """ Builds a nested aggregation.
-
-            :param sub_query: query to use as the 'primary_agg'
-            :param nested_path: path to nested object we are searching on
-            :param requested: requested agg, if any
-            :returns: the nested form of sub_query
-        """
-        if requested:
-            return {
-                NESTED: {
-                    PATH: nested_path
-                },
-                AGGS: {
-                    'primary_agg': sub_query,
-                    'requested_agg': requested
-                }
-            }
+        if field == 'type':
+            query_field = 'embedded.@type.raw'
+        elif field.startswith('validation_errors') or field.startswith('aggregated_items'):
+            query_field = field + '.raw'
+        elif facet.get('aggregation_type') in ('stats', 'date_histogram', 'histogram', 'range'):
+            query_field = 'embedded.' + field
         else:
-            return {
-                NESTED: {
-                    PATH: nested_path
+            query_field = 'embedded.' + field + '.raw'
+
+        # Create the aggregation itself, extend facet with info to pass down to front-end
+        agg_name = field.replace('.', '-')
+
+        if facet.get('aggregation_type') == 'stats':
+
+            if is_date_field:
+                facet['field_type'] = 'date'
+            elif is_numerical_field:
+                facet['field_type'] = 'number'
+
+            aggs[facet['aggregation_type'] + ":" + agg_name] = {
+                'aggs': {
+                    "primary_agg": {
+                        'stats': {
+                            'field': query_field
+                        }
+                    }
                 },
-                AGGS: {
-                    'primary_agg': sub_query
-                }
+                'filter': search_filters
             }
 
-    @classmethod
-    def _add_stats_aggregation(cls, field, facet, field_schema, query_field, search_filters, string_query,
-                               nested_path, aggs, agg_name):
-        """ Builds a stats aggregation, adding it to the given aggs.
-
-            :param field: raw field name we are searching on (ex: AF)
-            :param facet: facet metadata
-            :param field_schema: schema for the field we are searching on
-            :param query_field: ES document field we are searching on (ex: embedded.AF)
-            :param search_filters: filters we are searching on
-            :param string_query: simple query string if specified
-            :param nested_path: path to nested object we are aggregating on
-            :param aggs: the aggregation object we are building
-            :param agg_name: name of the aggregation we are building
-        """
-        is_date_field = field_schema and determine_if_is_date_field(field, field_schema)
-        is_numerical_field = field_schema and field_schema['type'] in ("integer", "float", "number")
-        if is_date_field:
-            facet['field_type'] = 'date'
-        elif is_numerical_field:
-            facet["field_type"] = field_schema['type'] or "number"
-            if "number_step" not in facet:
-                if "number_step" in field_schema:
-                    facet["number_step"] = field_schema['number_step']
-                elif facet["field_type"] == "integer":
-                    facet["number_step"] = 1
-                else:  # Default
-                    facet["number_step"] = "any"
-        facet_filters = cls.generate_filters_for_terms_agg_from_search_filters(query_field, search_filters,
-                                                                               string_query)
-        # stats aggregations could be nested too
-        stats_agg = {
-            STATS: {
-                'field': query_field
-            }
-        }
-        if nested_path:
-            facet['aggregation_type'] = 'nested:stats'
-            aggs[facet['aggregation_type'] + ':' + agg_name] = {
-                AGGS: {
-                    'primary_agg': cls._build_nested_aggregation(stats_agg, nested_path)
-                },
-                FILTER: facet_filters
+        else:  # Default -- facetable terms
+
+            facet['aggregation_type'] = 'terms'
+            facet_filters = generate_filters_for_terms_agg_from_search_filters(query_field, search_filters, string_query)
+            term_aggregation = {
+                "terms": {
+                    'size': 100,            # Maximum terms returned (default=10); see https://github.com/10up/ElasticPress/wiki/Working-with-Aggregations
+                    'field': query_field,
+                    'missing': facet.get("missing_value_replacement", "No value")
+                }
             }
 
-        else:
             aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                AGGS: {
-                    'primary_agg': stats_agg
+                'aggs': {
+                    "primary_agg": term_aggregation
                 },
-                FILTER: facet_filters
+                'filter': {'bool': facet_filters},
             }
 
-    @classmethod
-    def _build_range_aggregation(cls, query_field, ranges):
-        """ Builds a range aggregation.
-            Detects when 0-0 range is specified and replaces 'to' with the
-            smallest IEEE 32 value such that the bucket effectively only captures
-            the value 0.
-        """
-        for r in ranges:
-            if 'from' in r and 'to' in r:
-                if r['from'] == 0 and r['to'] == 0:
-                    r['to'] = cls.SMALLEST_NONZERO_IEEE_32
-            if 'to' in r and r['to'] != cls.SMALLEST_NONZERO_IEEE_32:
-                r['to'] += cls.SMALLEST_NONZERO_IEEE_32
-        return {
-            RANGE: {
-                FIELD: query_field,
-                'ranges': ranges
-            }
+        # Update facet with title, description from field_schema, if missing.
+        if facet.get('title') is None and field_schema and 'title' in field_schema:
+            facet['title'] = field_schema['title']
+        if facet.get('description') is None and field_schema and 'description' in field_schema:
+            facet['description'] = field_schema['description']
+
+    # to achieve OR behavior within facets, search among GLOBAL results,
+    # not just returned ones. to do this, wrap aggs in ['all_items']
+    # and add "global": {} to top level aggs query
+    # see elasticsearch global aggs for documentation (should be ES5 compliant)
+    search_as_dict = search.to_dict()
+    search_as_dict['aggs'] = {
+        'all_items': {
+            'global': {},
+            'aggs': aggs
         }
+    }
 
-    @classmethod
-    def _add_range_aggregation(cls, facet, query_field, search_filters, string_query, nested_path, aggs, agg_name):
-        """ Builds a range aggregation utilizing the ranges defined on schema facet, adding it to the given aggs.
-
-            :param facet: facet metadata
-            :param query_field: field we are searching on.
-            :param search_filters: filters we are searching on
-            :param string_query: simple query string if specified
-            :param nested_path: path to nested object we are aggregating on
-            :param aggs: the aggregation object we are building
-            :param agg_name: name of the aggregation we are building
-        """
-        facet_filters = cls.generate_filters_for_terms_agg_from_search_filters(query_field, search_filters,
-                                                                               string_query)
-        ranges = [{k: v for k, v in r.items() if k in ['from', 'to']} for r in facet['ranges']]
-        range_agg = cls._build_range_aggregation(query_field, ranges)
-        if nested_path:
-            facet['aggregation_type'] = 'nested:range'
-            field = facet['aggregation_type'] + ':' + agg_name
-            range_agg = cls._build_nested_aggregation(range_agg, nested_path)
-        else:
-            facet['aggregation_type'] = RANGE
-            field = facet['aggregation_type'] + ':' + agg_name
-        aggs[field] = {
-            AGGS: {
-                'primary_agg': range_agg
-            },
-            FILTER: facet_filters
-        }
+    if size == 0:
+        # Only perform aggs if size==0 requested, to improve performance for search page queries.
+        # We do currently have (hidden) monthly date histogram facets which may yet to be utilized for common size!=0 agg use cases.
+        set_additional_aggregations(search_as_dict, request, doc_types, custom_aggregations)
 
-    @staticmethod
-    def _build_terms_aggregation(query_field, facet, requested_values=None, nested=False):
-        """ Builds a terms aggregation, specifically requesting counts for any selected values. """
-        agg = {
-            TERMS: {
-                'size': MAX_FACET_COUNTS,
-                'field': query_field,
-                'missing': facet.get('missing_value_replacement', 'No value')
-            }
-        }
-        if requested_values:  # getall returns [], not None
-            agg[TERMS]['include'] = requested_values
-        if nested:
-            agg[AGGS] = {
-                'primary_agg_reverse_nested': {
-                    'reverse_nested': {}
-                }
-            }
-        return agg
+    search.update_from_dict(search_as_dict)
+    return search
 
-    @classmethod
-    def _add_terms_aggregation(cls, facet, query_field, search_filters, string_query, nested_path, aggs, agg_name,
-                               requested_values):
-        """ Builds a standard terms aggregation, setting a nested identifier to be repaired later
-            by elasticsearch_dsl, adding it to the given aggs.
-
-            :param facet: facet metadata
-            :param query_field: field we are searching on.
-            :param search_filters: filters we are searching on
-            :param string_query: simple query string if specified
-            :param nested_path: path to nested object we are aggregating on
-            :param aggs: the aggregation object we are building
-            :param agg_name: name of the aggregation we are building
-            :param requested_values: values for this terms agg we requested (to be explicitly included)
-        """
-        is_nested = nested_path is not None
-        if is_nested:
-            facet['aggregation_type'] = NESTED  # special in that it is used to identify (broken) facets - Will 11/17/20
-        else:
-            facet['aggregation_type'] = TERMS
 
-        facet_filters = cls.generate_filters_for_terms_agg_from_search_filters(query_field, search_filters,
-                                                                               string_query)
-        terms_aggregation = cls._build_terms_aggregation(query_field, facet, None, is_nested)
-
-        # NOTE: if we requested values for this field, we must expand to do two aggregations
-        # Unfortunately when you pass "include" to a terms aggregation it acts as a hard filter,
-        # not a "force bucket", which makes implementing this very tricky. To get around this we
-        # expand to 2 aggregations - one for the requested field and one for the remaining top fields
-        if requested_values:
-            terms_aggregation_requested = cls._build_terms_aggregation(query_field, facet, requested_values,
-                                                                       is_nested)
-            if nested_path:
-                aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                    AGGS: {'primary_agg':
-                               cls._build_nested_aggregation(terms_aggregation, nested_path,
-                                                             terms_aggregation_requested),
-                    },
-                    FILTER: facet_filters,
-                }
-            else:
-                aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                    AGGS: {
-                        'primary_agg': terms_aggregation_requested,
-                        'requested_agg': terms_aggregation
-                    },
-                    FILTER: facet_filters,
-                }
+def set_additional_aggregations(search_as_dict, request, doc_types, extra_aggregations=None):
+    """
+    Per-type aggregations may be defined in schemas. Apply them OUTSIDE of globals so they act on our current search filters.
+    Warning: `search_as_dict` is modified IN PLACE.
+    """
+
+    types = request.registry[TYPES]
+    schema = types[doc_types[0]].schema
 
+    if schema.get('aggregations'):
+        for schema_agg_name in schema['aggregations'].keys():
+            if schema_agg_name == 'all_items':
+                raise Exception('all_items is a reserved agg name and not allowed as an extra aggregation name.')
+            search_as_dict['aggs'][schema_agg_name] = schema['aggregations'][schema_agg_name]
+
+    if extra_aggregations:
+        for extra_agg_name in extra_aggregations.keys():
+            if extra_agg_name == 'all_items':
+                raise Exception('all_items is a reserved agg name and not allowed as an extra aggregation name.')
+            search_as_dict['aggs'][extra_agg_name] = extra_aggregations[extra_agg_name]
+
+    return search_as_dict
+
+
+def execute_search(search):
+    """
+    Execute the given Elasticsearch-dsl search. Raise HTTPBadRequest for any
+    exceptions that arise.
+    Args:
+        search: the Elasticsearch-dsl prepared in the search() function
+    Returns:
+        Dictionary search results
+    """
+    err_exp = None
+    try:
+        es_results = search.execute().to_dict()
+    except ConnectionTimeout as exc:
+        ignored(exc)
+        err_exp = 'The search failed due to a timeout. Please try a different query.'
+    except RequestError as exc:
+        # try to get a specific error message. May fail in some cases
+        try:
+            err_detail = str(exc.info['error']['root_cause'][0]['reason'])
+        except Exception:
+            err_detail = str(exc)
+        err_exp = 'The search failed due to a request error: ' + err_detail
+    except TransportError as exc:
+        # most general exception
+        exc_status = getattr(exc, 'status_code')
+        if exc_status == 'TIMEOUT':
+            err_exp = 'The search failed due to a timeout. Please try a different query.'
         else:
-            if nested_path:
-                aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                    AGGS: {'primary_agg':
-                               cls._build_nested_aggregation(terms_aggregation, nested_path),
-                    },
-                    FILTER: facet_filters,
-                }
-            else:
-                aggs[facet['aggregation_type'] + ":" + agg_name] = {
-                    AGGS: {
-                        'primary_agg': terms_aggregation
-                    },
-                    FILTER: facet_filters,
-                }
+            err_exp = 'The search failed due to a transport error: ' + str(exc)
+    except Exception as exc:
+        ignored(exc)
+        err_exp = 'The search failed. The DCIC team has been notified.'
+    if err_exp:
+        raise HTTPBadRequest(explanation=err_exp)
+    return es_results  # noQA - PyCharm wrongly worries this might not have been set.
 
-    @classmethod
-    def build_facets(cls, query, facets, search_filters, string_query, request, doc_types,
-                     custom_aggregations=None, size=25, from_=0, es_mapping=None):
-        """
-        Sets facets in the query as ElasticSearch aggregations, with each aggregation to be
-        filtered by search_filters minus filter affecting facet field in order to get counts
-        for other facet term options.
-        ES5 - simply sets aggs by calling update_from_dict after adding them in
-            :param facets:         Facet field (0) in object dot notation, and a dict or OrderedDict with title property (1).
-            :type  facets:         List of tuples.
-            :param search_filters: Dict of filters which are set for the ES query in build_filters
-            :param string_query:   Dict holding the query_string used in the search
-        """
-        if from_ != 0:
-            return query
 
-        aggs = OrderedDict()
-        for field, facet in facets:  # E.g. 'type','experimentset_type','experiments_in_set.award.project', ...
-            field_schema = schema_for_field(field, request, doc_types, should_log=True)
-            query_field = get_query_field(field, facet)
-            nested_path = find_nested_path(query_field, es_mapping)
-            requested_values = request.params.getall(field)
-
-            # Build the aggregation based on its type (by side-effect) - stats, range or terms
-            agg_name = field.replace('.', '-')
-            facet_type = facet.get('aggregation_type')
-            if facet_type in ['stats', 'nested:stats']:
-                cls._add_stats_aggregation(field, facet, field_schema, query_field, search_filters, string_query,
-                                           nested_path, aggs, agg_name)
-            elif facet_type in ['range', 'nested:range']:
-                cls._add_range_aggregation(facet, query_field, search_filters, string_query, nested_path,
-                                           aggs, agg_name)
-            else:  # assume terms
-                cls._add_terms_aggregation(facet, query_field, search_filters, string_query, nested_path,
-                                           aggs, agg_name, requested_values)
-
-            # Update facet with title, description from field_schema, if missing.
-            if facet.get('title') is None and field_schema and 'title' in field_schema:
-                facet['title'] = field_schema['title']
-            if facet.get('description') is None and field_schema and 'description' in field_schema:
-                facet['description'] = field_schema['description']
-
-        # to achieve OR behavior within facets, search among GLOBAL results,
-        # not just returned ones. to do this, wrap aggs in ['all_items']
-        # and add "global": {} to top level aggs query
-        # see elasticsearch global aggs for documentation (should be ES5 compliant)
-        query['aggs'] = {
-            'all_items': {
-                'global': {},
-                'aggs': aggs
-            }
+def format_facets(es_results, facets, total, search_frame='embedded'):
+    """
+    Format the facets for the final results based on the es results.
+    Sort based off of the 'order' of the facets
+    These are stored within 'aggregations' of the result.
+
+    If the frame for the search != embedded, return no facets
+    """
+    ignored(total)
+    result = []
+    if search_frame != 'embedded':
+        return result
+
+    # Loading facets in to the results
+    if 'aggregations' not in es_results:
+        return result
+
+    aggregations = es_results['aggregations']['all_items']
+    used_facets = set()
+
+    # Sort facets by order (ascending).
+    # If no order is provided, assume 0 to
+    # retain order of non-explicitly ordered facets
+    for field, facet in sorted(facets, key=lambda fct: fct[1].get('order', 0)):
+        result_facet = {
+            'field': field,
+            'title': facet.get('title', field),
+            'total': 0
+            # To be added depending on facet['aggregation_type']: 'terms', 'min', 'max', 'min_as_string', 'max_as_string', ...
         }
 
-        if size == 0:
-            # Only perform aggs if size==0 requested, to improve performance for search page queries.
-            # We do currently have (hidden) monthly date histogram facets which may yet to be utilized for common size!=0 agg use cases.
-            cls.set_additional_aggregations(query, request, doc_types, custom_aggregations)
+        result_facet.update({k: v
+                             for k, v in facet.items()
+                             if k not in result_facet.keys()})
+        used_facets.add(field)
+        field_agg_name = field.replace('.', '-')
+        full_agg_name = facet['aggregation_type'] + ':' + field_agg_name
+
+        if full_agg_name in aggregations:
+            if facet['aggregation_type'] == 'stats':
+                result_facet['total'] = aggregations[full_agg_name]['doc_count']
+                # Used for fields on which can do range filter on, to provide min + max bounds
+                for k in aggregations[full_agg_name]["primary_agg"].keys():
+                    result_facet[k] = aggregations[full_agg_name]["primary_agg"][k]
+            else:  # 'terms' assumed.
+                # Default - terms, range, or histogram buckets. Buckets may not be present
+                result_facet['terms'] = aggregations[full_agg_name]["primary_agg"]["buckets"]
+                # Choosing to show facets with one term for summary info on search it provides
+                if len(result_facet.get('terms', [])) < 1:
+                    continue
 
-        return query
+            if len(aggregations[full_agg_name].keys()) > 2:
+                result_facet['extra_aggs'] = {k: v
+                                              for k, v in aggregations[field_agg_name].items()
+                                              if k not in ('doc_count', "primary_agg")}
 
-    @staticmethod
-    def verify_search_has_permissions(request, query):
-        """
-        Inspects the search object to ensure permissions are still present on the query
-        This method depends on the query structure defined in 'build_filters'.
+        result.append(result_facet)
 
-        :param request: the current request
-        :param query: search query object to inspect
-        :raises: HTTPBadRequest if permissions not present
-        """
-        effective_principals_on_query = None
-        found = False  # set to True if we found valid 'principals_allowed.view'
-        try:
-            for boolean_clause in [query['query']['bool']['filter']]:  # should always be present
-                if 'bool' in boolean_clause and 'must' in boolean_clause['bool']:  # principals_allowed.view is on 'must'
-                    possible_permission_block = boolean_clause['bool']['must']
-                    for entry in possible_permission_block:
-                        if 'terms' in entry:
-                            if 'principals_allowed.view' in entry['terms']:
-                                effective_principals_on_query = entry['terms']['principals_allowed.view']
-                                if effective_principals_on_query != request.effective_principals:
-                                    raise QueryConstructionException(
-                                        query_type='principals',
-                                        func='verify_search_has_permissions',
-                                        msg='principals_allowed was modified - see application logs')
-                                else:
-                                    found = True
-                                    break
-        except QueryConstructionException:
-            search_log(log_handler=log, msg='Detected URL query param manipulation, principals_allowed.view was'
-                                            ' modified from %s to %s' % (request.effective_principals,
-                                                                         effective_principals_on_query))
-            raise HTTPBadRequest('The search failed - the DCIC team has been notified.')
-        except KeyError:
-            search_log(log_handler=log, msg='Malformed query detected while checking for principals_allowed')
-            raise HTTPBadRequest('The search failed - the DCIC team has been notified.')
-        if not found:
-            search_log(log_handler=log, msg='Did not locate principals_allowed.view on search query body: %s'
-                                            % query)
-            raise HTTPBadRequest('The search failed - the DCIC team has been notified.')
-
-    @classmethod
-    def compound_search(cls, sub_queries, intersect=False):
-        """  Takes an array of sub-queries and merges them into one query
-
-        :param sub_queries: list of query to be combined, typically starting with "bool"
-        :param intersect: whether or not to intersect the sub-queries
-        :return: lucene query combining the sub_queries with OR
-        """
-        if not intersect:
-            key = SHOULD
+    return result
+
+
+def format_extra_aggregations(es_results):
+    if 'aggregations' not in es_results:
+        return {}
+    return {k: v
+            for k, v in es_results['aggregations'].items()
+            if k != 'all_items'}
+
+
+def format_results(request, hits, search_frame):
+    """
+    Loads results to pass onto UI
+    Will retrieve the desired frame from the search hits and automatically
+    add 'validation_errors' and 'aggregated_items' frames if they are present
+    """
+    fields_requested = request.normalized_params.getall('field')
+    if fields_requested:
+        frame = 'embedded'
+    elif search_frame:
+        frame = search_frame
+    else:
+        frame = 'embedded'
+
+    if frame in ['embedded', 'object', 'raw']:
+        # transform 'raw' to 'properties', which is what is stored in ES
+        if frame == 'raw':
+            frame = 'properties'
+        for hit in hits:
+            frame_result = hit['_source'][frame]
+            if 'validation_errors' in hit['_source'] and 'validation_errors' not in frame_result:
+                frame_result['validation_errors'] = hit['_source']['validation_errors']
+            if 'aggregated_items' in hit['_source'] and 'aggregated_items' not in frame_result:
+                frame_result['aggregated_items'] = hit['_source']['aggregated_items']
+            yield frame_result
+        return
+
+
+def find_index_by_doc_types(request, doc_types, ignore):
+    """
+    Find the correct index(es) to be search given a list of doc_types.
+    The types in doc_types are the item class names, formatted like
+    'Experiment HiC' and index names are the item types, formatted like
+    'experiment_hi_c'.
+    Ignore any collection names provided in the ignore param, an array.
+    Formats output indexes as a string usable by elasticsearch
+    """
+    indexes = []
+    for doc_type in doc_types:
+        if doc_type in ignore:
+            continue
         else:
-            key = MUST
+            result = find_collection_subtypes(request.registry, doc_type)
+            namespaced_results = map(lambda t: get_namespaced_index(request, t), result)
+            indexes.extend(namespaced_results)
+    # remove any duplicates
+    indexes = list(set(indexes))
+    index_string = ','.join(indexes)
+    return index_string
+
+
+def make_search_subreq(request, path):
+    subreq = make_subrequest(request, path)
+    if hasattr(request, "_stats"):
+        subreq._stats = request._stats
+    subreq.registry = request.registry
+    if hasattr(request, "context"):
+        subreq.context = request.context
+    else:
+        subreq.context = None
+    subreq.headers['Accept'] = 'application/json'
+    return subreq
+
+
+DEFAULT_BROWSE_PARAM_LISTS = {
+    'type': ["ExperimentSetReplicate"],
+    'experimentset_type': ['replicate'],
+    'award.project': ['4DN']
+}
 
-        query = {
-            'query': {
-                'bool': {
-                    key: []
-                }
-            }
+
+def get_iterable_search_results(request, search_path='/search/', param_lists=None, **kwargs):
+    """
+    Loops through search results, returns 100 (or search_results_chunk_row_size) results at a time.
+    Pass it through itertools.chain.from_iterable to get one big iterable of results.
+    TODO: Maybe make 'limit=all', and instead of calling invoke_subrequest(subrequest), instead call iter_search_results!
+
+    :param request: Only needed to pass to do_subreq to make a subrequest with.
+    :param search_path: Root path to call, defaults to /search/ (can also use /browse/).
+    :param param_lists: Dictionary of param:lists_of_vals which is converted to URL query.
+    :param search_results_chunk_row_size: Amount of results to get per chunk. Default should be fine.
+    """
+    if param_lists is None:
+        param_lists = deepcopy(DEFAULT_BROWSE_PARAM_LISTS)
+    else:
+        param_lists = deepcopy(param_lists)
+    param_lists['limit'] = ['all']
+    param_lists['from'] = [0]  # TODO: Should be ['0'] ??
+    param_lists['sort'] = param_lists.get('sort', 'uuid')  # TODO: Default should be ['uuid'] ??
+    subreq = make_search_subreq(request, f'{search_path}?{urlencode(param_lists, True)}')
+    return iter_search_results(None, subreq, **kwargs)
+
+
+# Update? used in ./batch_download.py
+def iter_search_results(context, request, **kwargs):
+    return search(context, request, return_generator=True, **kwargs)
+
+
+def build_table_columns(request, schemas, doc_types):
+
+    any_abstract_types = 'Item' in doc_types
+    if not any_abstract_types:  # Check explictly-defined types to see if any are abstract.
+        type_infos = [request.registry[TYPES][type] for type in doc_types if type != 'Item']
+        for ti in type_infos:
+            # We use `type` instead of `isinstance` since we don't want to catch subclasses.
+            if type(ti) == AbstractTypeInfo:
+                any_abstract_types = True
+                break
+
+    columns = OrderedDict()
+
+    # Add title column, at beginning always
+    columns['display_title'] = {
+        "title": "Title",
+        "order": -100
+    }
+
+    # Add type column if any abstract types in search
+    if any_abstract_types and request.normalized_params.get('currentAction') != 'selection':
+        columns['@type'] = {
+            "title": "Item Type",
+            "colTitle": "Type",
+            "order": -80,
+            "description": "Type or category of Item",
+            # Alternative below, if we want type column to be available but hidden by default in selection mode:
+            # "default_hidden": request.normalized_params.get('currentAction') == 'selection'
+        }
+
+    for schema in schemas:
+        if 'columns' in schema:
+            schema_columns = OrderedDict(schema['columns'])
+            # Add all columns defined in schema
+            for name, obj in schema_columns.items():
+                if name not in columns:
+                    columns[name] = obj
+                else:
+                    # If @type or display_title etc. column defined in schema, then override defaults.
+                    for prop in schema_columns[name]:
+                        columns[name][prop] = schema_columns[name][prop]
+                # Add description from field schema, if none otherwise.
+                if not columns[name].get('description'):
+                    field_schema = schema_for_field(name, request, doc_types)
+                    if field_schema:
+                        if field_schema.get('description') is not None:
+                            columns[name]['description'] = field_schema['description']
+
+    # Add status column, if not present, at end.
+    if 'status' not in columns:
+        columns['status'] = {
+            "title": "Status",
+            "default_hidden": True,
+            "order": 501
         }
-        for q in sub_queries:
-            query['query']['bool'][key].append(q)
-        return query
+    # Add date column, if not present, at end.
+    if 'date_created' not in columns:
+        columns['date_created'] = {
+            "title": "Date Created",
+            "colTitle": "Created",
+            "default_hidden": True,
+            "order": 510
+        }
+    return columns
+
+
+_ASSEMBLY_MAPPER = {
+    'GRCh38-minimal': 'hg38',
+    'GRCh38': 'hg38',
+    'GRCh37': 'hg19',
+    'GRCm38': 'mm10',
+    'GRCm37': 'mm9',
+    'BDGP6': 'dm4',
+    'BDGP5': 'dm3',
+    'WBcel235': 'WBcel235'
+}
+
+hgConnect = ''.join([
+    'http://genome.ucsc.edu/cgi-bin/hgTracks',
+    '?hubClear=',
+])
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/settings.py` & `dcicsnovault-8.0.2b0/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/standalone_dev.py` & `dcicsnovault-8.0.2b0/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/stats.py` & `dcicsnovault-8.0.2b0/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/storage.py` & `dcicsnovault-8.0.2b0/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingDownload.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {'delete': "['mixinProperties']"}*

```diff
@@ -1,16 +1,8 @@
 {
-    "mixinProperties": [
-        {
-            "$ref": "mixins.json#/status"
-        },
-        {
-            "$ref": "mixins.json#/submitted"
-        }
-    ],
     "properties": {
         "attachment": {
             "attachment": true,
             "properties": {
                 "type": {
                     "enum": [
                         "image/png"
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.2b0/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/conftest.py` & `dcicsnovault-8.0.2b0/snovault/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import logging
+# import os
+# import time
+# import tempfile
 import pytest
+import logging
+# import subprocess
 
-from ..project_defs import C4ProjectRegistry
 from ..elasticsearch.indexer_queue import QueueManager
 
 
-# This might not be needed because it should demand-initialize, but there's a chance that the
-# demand-initialization would happen in some weird state of mocking, so rather than risk that,
-# we force it here.
-C4ProjectRegistry.initialize()
-
-
 # required so that db transactions are properly rolled back in tests
 @pytest.fixture(autouse=True)
 def autouse_external_tx(external_tx):
     pass
 
 
 # def _check_server_is_up(output):
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.2b0/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.2b0/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.2b0/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/root.py` & `dcicsnovault-8.0.2b0/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.2b0/snovault/tests/serverfixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     # SNOVAULT_DB_TEST_PORT,
     make_snovault_db_test_url,
 )
 
 
 NO_SERVER_FIXTURES = environ_bool("NO_SERVER_FIXTURES")
 
-
 def pytest_configure():
     logging.basicConfig(format='')
     logging.getLogger('sqlalchemy.engine').setLevel(logging.WARNING)
 
     class Shorten(logging.Filter):
         max_len = 500
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from pyramid.interfaces import IAuthenticationPolicy
 from pyramid.security import Authenticated, Everyone
 from pyramid.testing import DummyRequest
 from zope.interface.verify import verifyObject, verifyClass
-from ..authentication import NamespacedAuthenticationPolicy
+from .authentication import NamespacedAuthenticationPolicy
 
 
 class TestNamespacedAuthenticationPolicy(unittest.TestCase):
     """ This is a modified version of TestRemoteUserAuthenticationPolicy
     """
     def _getTargetClass(self):
         return NamespacedAuthenticationPolicy
@@ -27,47 +27,47 @@
 
     def test_unauthenticated_userid_returns_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.unauthenticated_userid(request), None)
 
     def test_unauthenticated_userid(self):
-        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
+        request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.unauthenticated_userid(request), 'user.fred')
 
     def test_authenticated_userid_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.authenticated_userid(request), None)
 
     def test_authenticated_userid(self):
-        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
+        request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.authenticated_userid(request), 'user.fred')
 
     def test_effective_principals_None(self):
         request = DummyRequest(environ={})
         policy = self._makeOne()
         self.assertEqual(policy.effective_principals(request), [Everyone])
 
     def test_effective_principals(self):
-        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
+        request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         self.assertEqual(policy.effective_principals(request),
                          [Everyone, Authenticated, 'user.fred'])
 
     def test_remember(self):
         request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         result = policy.remember(request, 'fred')
         self.assertEqual(result, [])
 
     def test_forget(self):
-        request = DummyRequest(environ={'REMOTE_USER': 'fred'})
+        request = DummyRequest(environ={'REMOTE_USER':'fred'})
         policy = self._makeOne()
         result = policy.forget(request)
         self.assertEqual(result, [])
 
     # From TestSessionAuthenticationPolicy
 
     def test_session_remember(self):
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_embed_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,15 @@
         for emb in expected_embeds
     ]
     embs_to_add, _ = expand_embedded_list('EmbeddingTest', registry[TYPES], dummy_emb_list, schema_props, set())
     expected_to_add = [
         'attachment',
         'attachment.attachment.*',
         'attachment.attachment2.*',
-        'attachment.principals_allowed.*',
-        'attachment.submitted_by'
+        'attachment.principals_allowed.*'
     ]
     assert set(embs_to_add) == set(expected_to_add)
 
     # add default embeds for all items 'attachment'
     test_embed = ['attachment.attachment.*']
     embs_to_add2, _ = expand_embedded_list('EmbeddingTest', registry[TYPES], test_embed, schema_props, set())
     expected_to_add2 = ['attachment']
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_indexing.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,21 +50,19 @@
 
 from .testing_views import TestingLinkSourceSno
 
 
 notice_pytest_fixtures(TestingLinkSourceSno)
 
 
-pytestmark = [pytest.mark.indexing, pytest.mark.es]
+pytestmark = [pytest.mark.indexing]
 
 
 TEST_COLL = '/testing-post-put-patch-sno/'
 TEST_TYPE = 'testing_post_put_patch_sno'  # use one collection for testing
-TEST_TYPE_HIDDEN_FACETS = 'testing_hidden_facets'
-TEST_TYPE_BUCKET_RANGE = 'testing_bucket_range_facets'
 
 # we just need single shard for these tests
 # XXX: use new type
 create_mapping.NUM_SHARDS = 1
 
 
 @pytest.fixture(scope='session')
@@ -92,15 +90,15 @@
     INDEXER_APP_PARAMS = [False]
 elif INDEXER_MODE == "BOTH":
     INDEXER_APP_PARAMS = [False, True]
 else:
     raise Exception("Bad value of INDEXER_MODE: %s. Possible values are MPINDEX, INDEX, and BOTH." % INDEXER_MODE)
 
 
-@pytest.fixture(scope='session', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
+@pytest.fixture(scope='module', params=INDEXER_APP_PARAMS)  # must happen AFTER scope='session' moto setup
 def app(app_settings, request):
     old_mpindexer = app_settings['mpindexer']
     with override_dict(app_settings, mpindexer=old_mpindexer):  # we plan to set it inside here
         if request.param:  # run tests both with and without mpindexer
             print("TEMPORARILY SETTING mpindexer=True in app_settings")
             app_settings['mpindexer'] = True  # This will get cleaned up by the override_dict
         app = main({}, **app_settings)
@@ -111,26 +109,24 @@
         try:
             DBSession.bind.pool.dispose()
         except AttributeError:
             # TODO: The .bind may be a connection, which doesn't have a .pool, so maybe sometime try this instead?
             #       DBSession.bind.engine.pool.dispose()
             pass
 
-
 # XXX C4-312: refactor tests so this can be module scope.
 # Having to have to drop DB tables and re-run create_mapping for every test is slow.
 @pytest.fixture(scope='function', autouse=True)
 def setup_and_teardown(app):
     """
     Run create mapping and purge queue before tests and clear out the
     DB tables after the test
     """
-    # BEFORE THE TEST - just run CM for the TEST_TYPEs above by default
-    create_mapping.run(app, collections=[TEST_TYPE, TEST_TYPE_HIDDEN_FACETS, TEST_TYPE_BUCKET_RANGE],
-                       skip_indexing=True, purge_queue=True)
+    # BEFORE THE TEST - just run CM for the TEST_TYPE by default
+    create_mapping.run(app, collections=[TEST_TYPE], skip_indexing=True, purge_queue=True)
 
     yield  # run the test
 
     # AFTER THE TEST
     session = app.registry[DBSESSION]
     connection = session.connection()  # was session.connection().connect(), rewritten for SA2.0
     # The reflect=True argument to MetaData was deprecated. Instead, one is supposed to call the .reflect()
@@ -210,15 +206,15 @@
         raw_idx = indexer_utils.get_namespaced_index(app, TEST_TYPE)
         star_idx = indexer_utils.get_namespaced_index(app.registry, '*')  # registry should work as well
         assert raw_idx == TEST_TYPE
         assert star_idx == '*'
         # app.registry.settings['indexer.namespace'] = indexer_namespace  # reset indexer_namespace
 
 
-# @pytest.mark.es - Specified at top of file for whole file
+@pytest.mark.es
 def test_indexer_queue_adds_telemetry_id(app):
     indexer_queue = app.registry[INDEXER_QUEUE]
     indexer_queue.clear_queue()
     test_message = 'abc123'
     telem = 'test_telemetry_id'
     to_index, failed = indexer_queue.add_uuids(app.registry, [test_message], strict=True,
                                                telemetry_id=telem)
@@ -232,15 +228,15 @@
     assert msg_body['strict'] is True
     assert msg_body['telemetry_id'] == telem
 
     # finally, delete
     indexer_queue.delete_messages(received)
 
 
-# @pytest.mark.es - Specified at top of file for whole file
+@pytest.mark.es
 @pytest.mark.flaky
 def test_indexer_queue(app):
     indexer_queue_mirror = app.registry[INDEXER_QUEUE_MIRROR]
     # An indexing queue mirror would only be set up for production servers.
     assert indexer_queue_mirror is None
 
     indexer_queue = app.registry[INDEXER_QUEUE]
@@ -1953,372 +1949,14 @@
     ])
     def test_invalidation_scope_view_error(self, indexer_testapp, req):
         """ Test failure cases """
         with pytest.raises(webtest.AppError):
             indexer_testapp.post_json('/compute_invalidation_scope', req)
 
 
-@pytest.fixture(scope='session')
-def hidden_facet_data_one():
-    """ Sample TestingHiddenFacets object we are going to facet on """
-    return {
-        'first_name': 'John',
-        'last_name': 'Doe',
-        'sid': 1,
-        'status': 'current',
-        'unfaceted_string': 'hello',
-        'unfaceted_integer': 123,
-        'disabled_string': 'orange',
-        'disabled_integer': 789,
-        'unfaceted_object': {
-            'mother': 'Anne',
-            'father': 'Bob'
-        },
-        'unfaceted_array_of_objects': [
-            {
-                'fruit': 'orange',
-                'color': 'orange',
-                'uid': 1
-            },
-            {
-                'fruit': 'banana',
-                'color': 'yellow',
-                'uid': 2
-            },
-        ]
-    }
-
-
-@pytest.fixture(scope='session')
-def hidden_facet_data_two():
-    """ A second sample TestingHiddenFacets object we are going to facet on """
-    return {
-        'first_name': 'Boston',
-        'last_name': 'Bruins',
-        'sid': 2,
-        'status': 'current',
-        'unfaceted_string': 'world',
-        'unfaceted_integer': 456,
-        'disabled_string': 'apple',
-        'disabled_integer': 101112,
-        'unfaceted_object': {
-            'mother': 'Candice',
-            'father': 'Doug'
-        },
-        'unfaceted_array_of_objects': [
-            {
-                'fruit': 'blueberry',
-                'color': 'blue',
-                'uid': 3
-            },
-            {
-                'fruit': 'mango',
-                'color': 'yellow',
-                'uid': 4
-            },
-        ]
-    }
-
-
-@pytest.fixture(scope='function')
-def hidden_facet_test_data(testapp, hidden_facet_data_one, hidden_facet_data_two):
-    testapp.post_json('/TestingHiddenFacets', hidden_facet_data_one, status=201)
-    testapp.post_json('/TestingHiddenFacets', hidden_facet_data_two, status=201)
-    index_n_items_for_testing(testapp, 2)
-
-
-class TestSearchHiddenAndAdditionalFacets:
-    """ Encapsulates tests meant for testing behavior associated with default_hidden, hidden
-        and additional_facets
-    """
-    DEFAULT_FACETS = ['first_name']  # 'validation_errors.name'
-    DEFAULT_HIDDEN_FACETS = ['last_name', 'sid']
-    ADDITIONAL_FACETS = ['unfaceted_string', 'unfaceted_integer']
-    DISABLED_FACETS = ['disabled_string', 'disabled_integer']
-
-    @staticmethod
-    def check_and_verify_result(facets, desired_facet, number_expected):
-        """ Helper method for later tests that checks terms count and average. """
-        for facet in facets:
-            field = facet['field']
-            if field == desired_facet and 'terms' in facet:
-                assert len(facet['terms']) == number_expected
-            elif field == facet and 'avg' in facet:
-                assert facet['avg'] == number_expected
-            else:
-                continue
-            break
-
-    @staticmethod
-    def assert_facet_set_equal(expected, facets):
-        """ Takes list of expect results and raw facet response and checks that they
-            are identical. """
-        assert sorted(expected) == sorted([facet['field'] for facet in facets])
-
-    def test_search_default_hidden_facets_dont_show(self, testapp, hidden_facet_test_data):
-        facets = testapp.get('/search/?type=TestingHiddenFacets').json['facets']
-        self.assert_facet_set_equal(self.DEFAULT_FACETS, facets)
-
-    @pytest.mark.parametrize('facet', ADDITIONAL_FACETS)
-    def test_search_one_additional_facet(self, testapp, hidden_facet_test_data, facet):
-        """ Tests that specifying each of the 'additional' facets works correctly """
-        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % facet).json['facets']
-        expected = self.DEFAULT_FACETS + [facet]
-        self.assert_facet_set_equal(expected, facets)
-
-    def test_search_multiple_additional_facets(self, testapp, hidden_facet_test_data):
-        """ Tests that enabling multiple additional facets works """
-        facets = testapp.get('/search/?type=TestingHiddenFacets'
-                                '&additional_facet=unfaceted_string'
-                                '&additional_facet=unfaceted_integer').json['facets']
-        expected = self.DEFAULT_FACETS + self.ADDITIONAL_FACETS
-        self.assert_facet_set_equal(expected, facets)
-        for facet in facets:  # verify facet type
-            if facet['field'] == 'unfaceted_integer':
-                assert facet['aggregation_type'] == 'stats'
-            else:  # facet['field'] == 'unfaceted_string'
-                assert facet['aggregation_type'] == 'terms'
-
-    @pytest.mark.parametrize('facet', DEFAULT_HIDDEN_FACETS)
-    def test_search_one_additional_default_hidden_facet(self, testapp, hidden_facet_test_data, facet):
-        """ Tests that passing default_hidden facets to additional_facets works correctly """
-        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % facet).json['facets']
-        expected = self.DEFAULT_FACETS + [facet]
-        self.assert_facet_set_equal(expected, facets)
-
-    def test_search_multiple_additional_default_hidden_facets(self, testapp, hidden_facet_test_data):
-        """ Tests that passing multiple hidden_facets as additionals works correctly """
-        facets = testapp.get('/search/?type=TestingHiddenFacets'
-                                '&additional_facet=last_name'
-                                '&additional_facet=sid').json['facets']
-        expected = self.DEFAULT_FACETS + self.DEFAULT_HIDDEN_FACETS
-        self.assert_facet_set_equal(expected, facets)
-        for facet in facets:
-            if facet['field'] == 'sid':
-                assert facet['aggregation_type'] == 'stats'
-            else:
-                assert facet['aggregation_type'] == 'terms'
-
-    @pytest.mark.parametrize('_facets', [
-        ['last_name', 'unfaceted_integer'],  # second slot holds number field
-        ['unfaceted_string', 'sid']
-    ])
-    def test_search_mixing_additional_and_default_hidden(self, testapp, hidden_facet_test_data, _facets):
-        """ Tests that we can mix additional_facets with those both on and off schema """
-        facets = testapp.get('/search/?type=TestingHiddenFacets'
-                                '&additional_facet=%s'
-                                '&additional_facet=%s' % (_facets[0], _facets[1])).json['facets']
-        expected = self.DEFAULT_FACETS + _facets
-        self.assert_facet_set_equal(expected, facets)
-        for facet in facets:
-            if facet['field'] == _facets[1]:  # second slot holds number field
-                assert facet['aggregation_type'] == 'stats'
-            else:
-                assert facet['aggregation_type'] == 'terms'
-
-    @pytest.mark.parametrize('_facet', DISABLED_FACETS)
-    def test_search_disabled_overrides_additional(self, testapp, hidden_facet_test_data, _facet):
-        """ Hidden facets should NEVER be faceted on """
-        facets = testapp.get('/search/?type=TestingHiddenFacets&additional_facet=%s' % _facet).json['facets']
-        field_names = [facet['field'] for facet in facets]
-        assert _facet not in field_names  # always hidden should not be here, even if specified
-
-    @pytest.mark.parametrize('_facets', [
-        ('last_name', 'unfaceted_integer', 'disabled_integer'),  # default_hidden second
-        ('sid', 'unfaceted_string', 'disabled_string')  # disabled always last
-    ])
-    def test_search_additional_mixing_disabled_default_hidden(self, testapp, hidden_facet_test_data, _facets):
-        """ Tests that supplying multiple additional facets combined with hidden still respects the
-            hidden restriction. """
-        facets = testapp.get('/search/?type=TestingHiddenFacets'
-                                '&additional_facet=%s'
-                                '&additional_facet=%s' 
-                                '&additional_facet=%s' % (_facets[0], _facets[1], _facets[2])).json['facets']
-        expected = self.DEFAULT_FACETS + [_facets[0], _facets[1]]  # first two should show
-        self.assert_facet_set_equal(expected, facets)
-
-    @pytest.mark.parametrize('_facet', [
-        'unfaceted_object.mother',
-        'unfaceted_object.father'
-    ])
-    def test_search_additional_object_facets(self, testapp, hidden_facet_test_data, _facet):
-        """ Tests that specifying an object field as an additional_facet works correctly """
-        facets = testapp.get('/search/?type=TestingHiddenFacets'
-                                '&additional_facet=%s' % _facet).json['facets']
-        expected = self.DEFAULT_FACETS + [_facet]
-        self.assert_facet_set_equal(expected, facets)
-
-    @pytest.mark.parametrize('_facet, n_expected', [
-        ('unfaceted_array_of_objects.fruit', 4),
-        ('unfaceted_array_of_objects.color', 3),
-        ('unfaceted_array_of_objects.uid', 2.5)  # stats avg
-    ])
-    def test_search_additional_nested_facets(self, testapp, hidden_facet_test_data, _facet, n_expected):
-        """ Tests that specifying an array of object field mapped with nested as an additional_facet
-            works correctly. """
-        [desired_facet] = [facet for facet in testapp.get('/search/?type=TestingHiddenFacets'
-                                                             '&additional_facet=%s' % _facet).json['facets']
-                           if facet['field'] == _facet]
-        if 'terms' in desired_facet:
-            assert len(desired_facet['terms']) == n_expected
-        else:
-            assert desired_facet['avg'] == n_expected
-
-    @pytest.fixture
-    def many_non_nested_facets(self, testapp, hidden_facet_test_data):
-        return testapp.get('/search/?type=TestingHiddenFacets'  
-                              '&additional_facet=non_nested_array_of_objects.fruit'
-                              '&additional_facet=non_nested_array_of_objects.color'
-                              '&additional_facet=non_nested_array_of_objects.uid').json['facets']
-
-    @pytest.mark.parametrize('_facet, n_expected', [
-        ('unfaceted_array_of_objects.fruit', 4),
-        ('unfaceted_array_of_objects.color', 3),
-        ('unfaceted_array_of_objects.uid', 2.5)  # stats avg
-    ])
-    def test_search_additional_non_nested_facets(self, many_non_nested_facets, _facet, n_expected):
-        """ Tests trying to facet on an array of objects field that is not nested, requesting
-            all at the same time.
-        """
-        self.check_and_verify_result(many_non_nested_facets, _facet, n_expected)
-
-
-@pytest.fixture(scope='session')
-def bucket_range_data_raw():
-    """ 9 objects with a numerical field we will bucket on.
-            'special_integer' has i in it.
-            'special_object_that_holds_integer' holds a single integer field with i as well
-            'array_of_objects_that_holds_integer' holds 2 objects that are mirrors of one another
-        +
-        1 object with a value for no_value_integer, to test that filtering on a field that sets
-        'add_no_value' to True will not filter documents with 'No value'.
-    """
-    entries = [{
-        'special_integer': i,
-        'special_object_that_holds_integer': {
-            'embedded_integer': i
-        },
-        'array_of_objects_that_holds_integer': [
-            {
-                'embedded_identifier': 'forward',
-                'embedded_integer': 0 if i < 5 else 9
-            },
-            {
-                'embedded_identifier': 'reverse',
-                'embedded_integer': 9 if i < 5 else 0
-            },
-        ]
-    } for i in range(10)]
-    # set no value int on the last element
-    entries[-1]['no_value_integer'] = 8
-    entries[-1]['no_value_integer_array'] = [8]
-    return entries
-
-
-@pytest.fixture(scope='function')
-def bucket_range_data(testapp, bucket_range_data_raw):
-    for entry in bucket_range_data_raw:
-        testapp.post_json('/TestingBucketRangeFacets', entry, status=201)
-    index_n_items_for_testing(testapp, 10)
-
-
-class TestSearchBucketRangeFacets:
-    """ Class that encapsulates tests for BucketRanges """
-
-    @staticmethod
-    def verify_facet_counts(facets, expected_fields, expected_cardinality, expected_count):
-        """ Checks for given expected facets, checking bucket cardinality and document count
-            Note that the actual range properties are trivial (we are not testing elasticsearch)
-        """
-        for facet in facets:
-            if facet['field'] in expected_fields:
-                assert len(facet['ranges']) == expected_cardinality
-                for bucket in facet['ranges']:
-                    assert bucket['doc_count'] == expected_count
-
-    @staticmethod
-    def verify_counts(response, expected_count):
-        assert len(response['@graph']) == expected_count
-
-    @staticmethod
-    def select_facet(facets, facet_name):
-        result = None
-        for facet in facets:
-            if facet['field'] == facet_name:
-                result = facet
-                break
-        return result
-
-    @pytest.mark.parametrize('expected_fields, expected_counts', [
-        (['special_integer'], 5),
-        (['special_object_that_holds_integer.embedded_integer'], 5),
-        (['array_of_objects_that_holds_integer.embedded_integer'], 10)
-    ])
-    def test_search_bucket_range_simple(self, testapp, bucket_range_data, expected_fields, expected_counts):
-        """ Tests searching a collection of documents with varying integer field types that
-            have the same distribution - all of which should give the same results. """
-        res = testapp.get('/search/?type=TestingBucketRangeFacets').json['facets']
-        self.verify_facet_counts(res, expected_fields, 2, expected_counts)
-
-    # XXX: The following 2 tests don't function correctly because the facet doesn't utilize reverse_nested
-    @pytest.mark.parametrize('identifier', [
-        'reverse', 'forward'
-    ])
-    def test_search_bucket_range_nested_qualifier(self, testapp, bucket_range_data, identifier):
-        """ Tests aggregating on a nested field while selecting for a field within the nested object. """
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&array_of_objects_that_holds_integer.embedded_identifier=%s' % identifier).json['facets']
-        self.verify_facet_counts(res, ['array_of_objects_that_holds_integer.embedded_integer'],
-                                 2, 10)
-
-    @pytest.mark.parametrize('identifier', [
-        'reverse', 'forward'
-    ])
-    def test_search_bucket_range_nested_qualifier_multiple(self, testapp, bucket_range_data, identifier):
-        """ Tests aggregating on a nested field while selecting for a field within the nested object (no change). """
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&array_of_objects_that_holds_integer.embedded_integer.from=6'
-                             '&array_of_objects_that_holds_integer.embedded_identifier=%s' % identifier).json['facets']
-        self.verify_facet_counts(res, ['array_of_objects_that_holds_integer.embedded_integer'],
-                                 2, 10)
-        facet_with_labels = self.select_facet(res, 'array_of_objects_that_holds_integer.embedded_integer')
-        for r in facet_with_labels['ranges']:
-            assert 'label' in r
-            assert r['label'] in ['Low', 'High']
-
-    def test_search_bucket_range_add_no_value(self, testapp, bucket_range_data):
-        """ Tests that providing a range filter on a field that specifies 'add_no_value' does not
-            filter documents that have no value for that field.
-        """
-        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=0').json  # should detect
-        self.verify_counts(res, 10)
-        testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=10', status=404)  # should not detect
-        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.to=10').json  # should detect
-        self.verify_counts(res, 10)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets&no_value_integer.from=0'
-                             '&no_value_integer.to=10').json  # should detect
-        self.verify_counts(res, 10)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&no_value_integer_array.from=0').json  # should detect
-        self.verify_counts(res, 10)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&no_value_integer_array.from=8').json  # should detect
-        self.verify_counts(res, 1)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&no_value_integer_array.from=0&no_value_integer_array.to=7').json  # should detect
-        self.verify_counts(res, 9)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&no_value_integer_array.from=-1&no_value_integer_array.to=7').json  # should detect
-        self.verify_counts(res, 9)
-        res = testapp.get('/search/?type=TestingBucketRangeFacets'
-                             '&no_value_integer_array.from=-1&no_value_integer_array.to=9').json  # should detect
-        self.verify_counts(res, 10)
-
-
-
 def test_assert_transactions_table_is_gone(app):
     """
     A bit of a strange location for this test, but we need the app and
     serverfixtures to be established (used for indexing)
     """
     session = app.registry[DBSESSION]
     conn = session.connection()
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_key.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 
 from dcicutils.qa_utils import notice_pytest_fixtures
+from pyramid.config import Configurator
+from ..interfaces import DBSESSION
 
 
 # Test for storage.keys
 
 items = [
     {'name': 'one', 'accession': 'TEST1'},
     {'name': 'two', 'accession': 'TEST2'},
@@ -12,14 +14,24 @@
 
 bad_items = [
     {'name': 'one', 'accession': 'BAD1'},
     {'name': 'bad', 'accession': 'TEST1'},
 ]
 
 
+@pytest.fixture(scope='session')
+def app(DBSession):
+    notice_pytest_fixtures(DBSession)
+    config = Configurator()
+    config.registry[DBSESSION] = DBSession
+    config.include('snovault')
+    config.include('.testing_key')
+    return config.make_wsgi_app()
+
+
 @pytest.fixture
 def content(testapp):
     notice_pytest_fixtures(testapp)
     url = '/testing-keys/'
     for item in items:
         testapp.post_json(url, item, status=201)
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_link.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_logging.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_misc.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_stats.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_storage.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_util.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/test_views.py` & `dcicsnovault-8.0.2b0/snovault/tests/test_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -429,23 +429,7 @@
     """ Tests that acquiring auth0 config gives the expected values from settings for admins. """
     _test_auth_config(testapp, registry)
 
 
 def test_auth0_config_anon(anontestapp, registry):
     """ Tests that acquiring auth0 config gives the expected values from settings for anonymous users. """
     _test_auth_config(anontestapp, registry)
-
-
-def _test_recaptcha_config(testapp, registry):
-    cfg = testapp.get('/recaptcha_config').json
-    assert cfg['title'] == 'Recaptcha Config'
-    assert cfg['RecaptchaKey'] == registry.settings['g.recaptcha.key']
-
-
-def test_recaptcha_config_admin(testapp, registry):
-    """ Tests that acquiring recaptcha config gives the expected values from settings for admins. """
-    _test_recaptcha_config(testapp, registry)
-
-
-def test_recaptcha_config_anon(anontestapp, registry):
-    """ Tests that acquiring recaptcha config gives the expected values from settings for anonymous users. """
-    _test_recaptcha_config(anontestapp, registry)
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.2b0/snovault/tests/testappfixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     'testing': True,
     'mpindexer': False,
     'pyramid.debug_authorization': True,
     'postgresql.statement_timeout': 20,
     'retry.attempts': 3,
     'production': True,
     'structlog.dir': '/tmp/',
-    'g.recaptcha.key': 'dummy-recaptcha',
     'auth0.client': 'dummy-client',
     'auth0.domain': 'dummy.domain',
     'auth0.options': {
         'auth': {
             'sso': False,
             'redirect': False,
             'responseType': 'token',
@@ -29,29 +28,29 @@
                 'prompt': 'select_account'
             }
         },
         'allowedConnections': [
             'github', 'google-oauth2', 'partners'
         ]
     },
-    'multiauth.policies': 'session remoteuser accesskey auth0',
-    'multiauth.groupfinder': 'snovault.authorization.groupfinder',
-    'multiauth.policy.session.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policies': 'session remoteuser accesskey webuser',
+    'multiauth.groupfinder': 'snovault.tests.authorization.groupfinder',
+    'multiauth.policy.session.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.session.base': 'pyramid.authentication.SessionAuthenticationPolicy',
     'multiauth.policy.session.namespace': 'mailto',
-    'multiauth.policy.remoteuser.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.remoteuser.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.remoteuser.namespace': 'remoteuser',
     'multiauth.policy.remoteuser.base': 'pyramid.authentication.RemoteUserAuthenticationPolicy',
-    'multiauth.policy.accesskey.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.accesskey.use': 'snovault.tests.authentication.NamespacedAuthenticationPolicy',
     'multiauth.policy.accesskey.namespace': 'accesskey',
-    'multiauth.policy.accesskey.base': 'snovault.authentication.BasicAuthAuthenticationPolicy',
-    'multiauth.policy.accesskey.check': 'snovault.authentication.basic_auth_check',
-    'multiauth.policy.auth0.use': 'snovault.authentication.NamespacedAuthenticationPolicy',
-    'multiauth.policy.auth0.namespace': 'auth0',
-    'multiauth.policy.auth0.base': 'snovault.authentication.Auth0AuthenticationPolicy',
+    'multiauth.policy.accesskey.base': 'snovault.tests.authentication.BasicAuthAuthenticationPolicy',
+    'multiauth.policy.accesskey.check': 'snovault.tests.authentication.basic_auth_check',
+    'multiauth.policy.webuser.use':  'snovault.tests.authentication.NamespacedAuthenticationPolicy',
+    'multiauth.policy.webuser.namespace': 'webuser',
+    'multiauth.policy.webuser.base': 'snovault.tests.authentication.WebUserAuthenticationPolicy'
 }
 
 
 @pytest.fixture(scope="session")
 def basic_app_settings():
     return _app_settings.copy()
 
@@ -90,15 +89,15 @@
     environ = {
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     return webtest.TestApp(encrypted_app, environ)
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture
 def testapp(app):
     """ TestApp with JSON accept header. """
     environ = {
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     return webtest.TestApp(app, environ)
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.2b0/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/testing_views.py` & `dcicsnovault-8.0.2b0/snovault/tests/testing_views.py`

 * *Files 22% similar despite different names*

```diff
@@ -424,46 +424,14 @@
     },
 )
 class TestingDownload(ItemWithAttachment):
     item_type = 'testing_download'
     schema = load_schema('snovault:test_schemas/TestingDownload.json')
 
 
-@view_config(name='drs', context=TestingDownload, request_method='GET',
-             permission='view', subpath_segments=[0, 1])
-def drs(context, request):
-    """ Example DRS object implementation. Write this for all object classes that
-        you want to render a DRS object. This structure is minimally validated by the
-        downstream API (see drs.py).
-    """
-    rendered_object = request.embed(str(context.uuid), '@@object', as_user=True)
-    drs_object = {
-        'id': rendered_object['@id'],
-        'created_time': rendered_object['date_created'],
-        'drs_id': rendered_object['uuid'],
-        'self_uri': f'drs://{request.host}{request.path}',
-        'size': 0,
-        'checksums': [
-            {
-                'checksum': 'something',
-                'type': 'md5'
-            }
-        ],
-        'access_methods': [
-            {
-                'access_url': {
-                    'url': f'http://{request.host}/{context.uuid}/@@download'
-                },
-                'type': 'http'
-            },
-        ]
-    }
-    return drs_object
-
-
 @collection('testing-link-sources-sno', unique_key='testing_link_sources-sno:name')
 class TestingLinkSourceSno(Item):
     item_type = 'testing_link_source_sno'
     schema = load_schema('snovault:test_schemas/TestingLinkSourceSno.json')
     embedded_list = ['target_es.status', 'target.status']
 
 
@@ -834,230 +802,7 @@
     name_key = 'name'
     schema = load_schema('snovault:test_schemas/TestingBiogroupSno.json')
     embedded_list = [
         'sources.counter',  # get the counter
         'sources.samples.*',  # embed everything at top level
         'sources.contributor.*'
     ]
-
-
-@collection(
-    'testing-keys',
-    properties={
-        'title': 'Test keys',
-        'description': 'Testing. Testing. 1, 2, 3.',
-    },
-    unique_key='testing_accession',
-)
-class TestingKey(Item):
-    item_type = 'testing_key'
-    schema = {
-        'type': 'object',
-        'properties': {
-            'name': {
-                'type': 'string',
-                'uniqueKey': True,
-            },
-            'accession': {
-                'type': 'string',
-                'uniqueKey': 'testing_accession',
-            },
-        }
-    }
-
-
-@collection('testing-hidden-facets')
-class TestingHiddenFacets(Item):
-    """ Collection designed to test searching with hidden facets. Yes this is large, but this is a complex feature
-        with many possible cases. """
-    item_type = 'testing_hidden_facets'
-    schema = {
-        'type': 'object',
-        'properties': {
-            'first_name': {
-                'type': 'string'
-            },
-            'last_name': {
-                'type': 'string'
-            },
-            'sid': {
-                'type': 'integer'
-            },
-            'unfaceted_string': {
-                'type': 'string'
-            },
-            'unfaceted_integer': {
-                'type': 'integer'
-            },
-            'disabled_string': {
-                'type': 'string',
-            },
-            'disabled_integer': {
-                'type': 'integer',
-            },
-            'unfaceted_object': {
-                'type': 'object',
-                'properties': {
-                    'mother': {
-                        'type': 'string'
-                    },
-                    'father': {
-                        'type': 'string'
-                    }
-                }
-            },
-            'unfaceted_array_of_objects': {
-                'type': 'array',
-                'enable_nested': True,
-                'items': {
-                    'type': 'object',
-                    'properties': {
-                        'fruit': {
-                            'type': 'string'
-                        },
-                        'color': {
-                            'type': 'string'
-                        },
-                        'uid': {
-                            'type': 'integer'
-                        }
-                    }
-                }
-            }
-        },
-        'facets': {
-            'first_name': {
-                'title': 'First Name'
-            },
-            'last_name': {
-                'default_hidden': True,
-                'title': 'Last Name'
-            },
-            'sid': {
-                'default_hidden': True,
-                'title': 'SID',
-                'aggregation_type': 'stats',
-                'number_step': 1
-            },
-            'disabled_string': {
-                'disabled': True
-            },
-            'disabled_integer': {
-                'disabled': True
-            }
-        }
-    }
-
-    @calculated_property(schema={
-        'type': 'array',
-        'items': {
-            'type': 'object',
-            'properties': {
-                'fruit': {
-                    'type': 'string'
-                },
-                'color': {
-                    'type': 'string'
-                },
-                'uid': {
-                    'type': 'integer'
-                }
-            }
-        }
-    })
-    def non_nested_array_of_objects(self, unfaceted_array_of_objects):
-        """ Non-nested view of the unfaceted_array_of_objects field """
-        return unfaceted_array_of_objects
-
-
-@collection('testing-bucket-range-facets')
-class TestingBucketRangeFacets(Item):
-    """ Collection for testing BucketRange facets.
-        Also tests 'add_no_value' schema param behavior.
-    """
-    item_type = 'testing_bucket_range_facets'
-    schema = {
-        'type': 'object',
-        'properties': {
-            'no_value_integer': {
-                'type': 'integer',
-                'add_no_value': True  # if a range query is specified on this field, include documents that
-                                      # have 'No value' for the field
-            },
-            'no_value_integer_array': {
-                'type': 'array',
-                'items': {
-                    'type': 'integer',
-                    'add_no_value': True
-                }
-            },
-            'special_integer': {
-                'type': 'integer'
-            },
-            'special_object_that_holds_integer': {
-                'type': 'object',
-                'properties': {
-                    'embedded_integer': {
-                        'type': 'integer'
-                    }
-                }
-            },
-            'array_of_objects_that_holds_integer': {
-                'type': 'array',
-                'items': {
-                    'type': 'object',
-                    'enable_nested': False,
-                    'properties': {
-                        'embedded_identifier': {
-                            'type': 'string'
-                        },
-                        'embedded_integer': {
-                            'type': 'integer'
-                        }
-                    }
-                }
-            }
-        },
-        'facets': {
-            'no_value_integer': {
-                'title': 'No value integer',
-                'aggregation_type': 'range',
-                'ranges': [
-                    {'from': 0, 'to': 5},
-                    {'from': 5, 'to': 10}
-                ]
-            },
-            'no_value_integer_array': {
-                'title': 'No value integer array',
-                'aggregation_type': 'range',
-                'ranges': [
-                    {'from': 0, 'to': 0},  # test zero range faceting behavior
-                    {'from': 0, 'to': 5},
-                    {'from': 5, 'to': 10}
-                ]
-            },
-            'special_integer': {
-                'title': 'Special Integer',
-                'aggregation_type': 'range',
-                'ranges': [
-                    {'from': 0, 'to': 5},
-                    {'from': 5, 'to': 10}
-                ]
-            },
-            'special_object_that_holds_integer.embedded_integer': {
-                'title': 'Single Object Embedded Integer',
-                'aggregation_type': 'range',
-                'ranges': [
-                    {'from': 0, 'to': 5},
-                    {'from': 5, 'to': 10}
-                ]
-            },
-            'array_of_objects_that_holds_integer.embedded_integer': {
-                'title': 'Array of Objects Embedded Integer',
-                'aggregation_type': 'range',
-                'ranges': [
-                    {'from': 0, 'to': 5, 'label': 'Low'},
-                    {'from': 5, 'to': 10, 'label': 'High'}
-                ]
-            }
-        }
-    }
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.2b0/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/tools.py` & `dcicsnovault-8.0.2b0/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/typeinfo.py` & `dcicsnovault-8.0.2b0/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/upgrader.py` & `dcicsnovault-8.0.2b0/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/util.py` & `dcicsnovault-8.0.2b0/snovault/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import contextlib
 import datetime as datetime_module
 import functools
 import json
 import os
 import structlog
 import sys
-import re
-import boto3
 
-from botocore.client import Config
 from copy import copy
 from datetime import datetime, timedelta
 from pyramid.httpexceptions import HTTPForbidden
 from pyramid.threadlocal import manager as threadlocal_manager
-from dcicutils.secrets_utils import assume_identity
-from dcicutils.ecs_utils import ECSUtils
 
 from .interfaces import CONNECTION, STORAGE, TYPES
 from .settings import Settings
 
 
 log = structlog.getLogger(__name__)
 
@@ -1065,177 +1060,7 @@
         return "%s-test-%s-" % (prefix, test_job_id)
     else:
         # We've experimentally determined that it works pretty well to just use the timestamp.
         return "%s-test-%s-" % (prefix, int(datetime_module.datetime.now().timestamp() * 1000000))
 
 
 INDEXER_NAMESPACE_FOR_TESTING = generate_indexer_namespace_for_testing()
-
-
-def is_admin_request(request):
-    """ Checks for 'group.admin' in effective_principals on request - if present we know this
-        request was submitted by an admin
-    """
-    return 'group.admin' in request.effective_principals
-
-
-def get_item_or_none(request, value, itype=None, frame='object'):
-    """
-    Return the view of an item with given frame. Can specify different types
-    of `value` for item lookup
-
-    Args:
-        request: the current Request
-        value (str): String item identifier or a dict containing @id/uuid
-        itype (str): Optional string collection name for the item (e.g. /file-formats/)
-        frame (str): Optional frame to return. Defaults to 'object'
-
-    Returns:
-        dict: given view of the item or None on failure
-    """
-    item = None
-
-    if isinstance(value, dict):
-        if 'uuid' in value:
-            value = value['uuid']
-        elif '@id' in value:
-            value = value['@id']
-
-    svalue = str(value)
-
-    # Below case is for UUIDs & unique_keys such as accessions, but not @ids
-    if not svalue.startswith('/') and not svalue.endswith('/'):
-        svalue = '/' + svalue + '/'
-        if itype is not None:
-            svalue = '/' + itype + svalue
-
-    # Request.embed will attempt to get from ES for frame=object/embedded
-    # If that fails, get from DB. Use '@@' syntax instead of 'frame=' because
-    # these paths are cached in indexing
-    try:
-        item = request.embed(svalue, '@@' + frame)
-    except Exception:
-        pass
-
-    # could lead to unexpected errors if == None
-    return item
-
-
-CONTENT_TYPE_SPECIAL_CASES = {
-    'application/x-www-form-urlencoded': [
-        # Single legacy special case to allow us to POST to metadata TSV requests via form submission.
-        # All other special case values should be added using register_path_content_type.
-        '/metadata/',
-        '/variant-sample-search-spreadsheet/',
-        re.compile(r'/variant-sample-lists/[\da-z-]+/@@spreadsheet/'),
-    ]
-}
-
-
-def register_path_content_type(*, path, content_type):
-    """
-    Registers that endpoints that begin with the specified path use the indicated content_type.
-
-    This is part of an inelegant workaround for an issue in renderers.py that maybe we can make go away in the future.
-    See the 'implementation note' in ingestion/common.py for more details.
-    """
-    exceptions = CONTENT_TYPE_SPECIAL_CASES.get(content_type, None)
-    if exceptions is None:
-        CONTENT_TYPE_SPECIAL_CASES[content_type] = exceptions = []
-    if path not in exceptions:
-        exceptions.append(path)
-
-
-compiled_regexp_class = type(re.compile("foo.bar"))  # Hides that it's _sre.SRE_Pattern in 3.6, but re.Pattern in 3.7
-
-
-def content_type_allowed(request):
-    """
-    Returns True if the current request allows the requested content type.
-
-    This is part of an inelegant workaround for an issue in renderers.py that maybe we can make go away in the future.
-    See the 'implementation note' in ingestion/common.py for more details.
-    """
-    if request.content_type == "application/json":
-        # For better or worse, we always allow this.
-        return True
-
-    exceptions = CONTENT_TYPE_SPECIAL_CASES.get(request.content_type)
-
-    if exceptions:
-        for path_condition in exceptions:
-            if isinstance(path_condition, str):
-                if path_condition in request.path:
-                    return True
-            elif isinstance(path_condition, compiled_regexp_class):
-                if path_condition.match(request.path):
-                    return True
-            else:
-                raise NotImplementedError(f"Unrecognized path_condition: {path_condition}")
-
-    return False
-
-
-def check_user_is_logged_in(request):
-    """ Raises HTTPForbidden if the request did not come from a logged in user. """
-    for principal in request.effective_principals:
-        if principal.startswith('userid.') or principal == 'group.admin':  # allow if logged in OR has admin
-            break
-    else:
-        raise HTTPForbidden(title="Not logged in.")
-
-
-def make_s3_client():
-    s3_client_extra_args = {}
-    if 'IDENTITY' in os.environ:
-        identity = assume_identity()
-        s3_client_extra_args['aws_access_key_id'] = key_id = identity.get('S3_AWS_ACCESS_KEY_ID')
-        s3_client_extra_args['aws_secret_access_key'] = identity.get('S3_AWS_SECRET_ACCESS_KEY')
-        s3_client_extra_args['region_name'] = ECSUtils.REGION
-        log.warning(f"make_s3_client using S3 entity ID {key_id[:10]} arguments in `boto3 client creation call.")
-        if 'ENCODED_S3_ENCRYPT_KEY_ID' in identity:
-            # This setting is required when testing locally and encrypted buckets need to be accessed.
-            s3_client_extra_args['config'] = Config(signature_version='s3v4')
-    else:
-        log.warning(f'make_s3_client called with no identity')
-
-    s3_client = boto3.client('s3', **s3_client_extra_args)
-    return s3_client
-
-
-def build_s3_presigned_get_url(*, params):
-    """ Helper function that builds a presigned URL. """
-    s3_client = make_s3_client()
-    return s3_client.generate_presigned_url(
-        ClientMethod='get_object',
-        Params=params,
-        ExpiresIn=36 * 60 * 60
-    )
-
-
-class SettingsKey:
-    APPLICATION_BUCKET_PREFIX = 'application_bucket_prefix'
-    BLOB_BUCKET = 'blob_bucket'
-    EB_APP_VERSION = 'eb_app_version'
-    ELASTICSEARCH_SERVER = 'elasticsearch.server'
-    ENCODED_VERSION = 'encoded_version'
-    FILE_UPLOAD_BUCKET = 'file_upload_bucket'
-    FILE_WFOUT_BUCKET = 'file_wfout_bucket'
-    FOURSIGHT_BUCKET_PREFIX = 'foursight_bucket_prefix'
-    IDENTITY = 'identity'
-    INDEXER = 'indexer'
-    INDEXER_NAMESPACE = 'indexer.namespace'
-    INDEX_SERVER = 'index_server'
-    LOAD_TEST_DATA = 'load_test_data'
-    METADATA_BUNDLES_BUCKET = 'metadata_bundles_bucket'
-    S3_ENCRYPT_KEY_ID = 's3_encrypt_key_id'
-    SNOVAULT_VERSION = 'snovault_version'
-    SQLALCHEMY_URL = 'sqlalchemy.url'
-    SYSTEM_BUCKET = 'system_bucket'
-    TIBANNA_CWLS_BUCKET = 'tibanna_cwls_bucket'
-    TIBANNA_OUTPUT_BUCKET = 'tibanna_output_bucket'
-    UTILS_VERSION = 'utils_version'
-
-
-class ExtraArgs:
-    SERVER_SIDE_ENCRYPTION = "ServerSideEncryption"
-    SSE_KMS_KEY_ID = "SSEKMSKeyId"
```

### Comparing `dcicsnovault-8.0.1.5b15/snovault/validation.py` & `dcicsnovault-8.0.2b0/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/snovault/validators.py` & `dcicsnovault-8.0.2b0/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.5b15/PKG-INFO` & `dcicsnovault-8.0.2b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.5b15
+Version: 8.0.2b0
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
-Requires-Python: >=3.8.1,<3.10
+Requires-Python: >=3.8.1,<3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pyramid
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyBrowserID (>=0.10.0,<1)
 Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: aws_requests_auth (>=0.4.1,<0.5.0)
-Requires-Dist: boto3 (>=1.26.124,<2.0.0)
-Requires-Dist: botocore (>=1.19.124,<2.0.0)
-Requires-Dist: dcicutils (==7.4.4.5b21)
+Requires-Dist: boto3 (>=1.24.36)
+Requires-Dist: botocore (>=1.27.36)
+Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch_dsl (>=7.4.0,<8.0.0)
 Requires-Dist: future (>=0.15.2,<1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: netaddr (>=0.8.0,<1)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
-Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pyramid-multiauth (>=0.9.0,<1)
 Requires-Dist: pyramid-retry (>=1.0,<2.0)
 Requires-Dist: pyramid-tm (>=2.5,<3.0)
 Requires-Dist: pyramid-translogger (>=0.1,<0.2)
 Requires-Dist: pyramid_localroles (>=0.1,<1)
+Requires-Dist: pytest-redis (>=2.0.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python_magic (>=0.4.27)
 Requires-Dist: pytz (>=2021.3)
 Requires-Dist: rdflib (>=4.2.2,<5.0.0)
 Requires-Dist: rdflib-jsonld (>=0.5.0,<1.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: rutter (>=0.3,<1)
```

