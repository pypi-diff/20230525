# Comparing `tmp/langflow-0.0.76.tar.gz` & `tmp/langflow-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.0.76.tar", max compression
+gzip compressed data, was "langflow-0.0.78.tar", max compression
```

## Comparing `langflow-0.0.76.tar` & `langflow-0.0.78.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1065 2023-05-23 15:35:39.333321 langflow-0.0.76/LICENSE
--rw-r--r--   0        0        0    10199 2023-05-23 15:35:39.333321 langflow-0.0.76/README.md
--rw-r--r--   0        0        0     1888 2023-05-23 15:35:39.361321 langflow-0.0.76/pyproject.toml
--rw-r--r--   0        0        0      152 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     3726 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0     2032 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/base.py
--rw-r--r--   0        0        0     1124 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/callback.py
--rw-r--r--   0        0        0      776 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/chat.py
--rw-r--r--   0        0        0     8492 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/chat_manager.py
--rw-r--r--   0        0        0     1246 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/endpoints.py
--rw-r--r--   0        0        0     1443 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/schemas.py
--rw-r--r--   0        0        0     1765 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/api/validate.py
--rw-r--r--   0        0        0       57 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     4333 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4478 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     2369 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0      988 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0     2521 2023-05-23 15:36:46.921496 langflow-0.0.76/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
--rw-r--r--   0        0        0    11568 2023-05-23 15:36:46.921496 langflow-0.0.76/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
--rw-r--r--   0        0        0    80491 2023-05-23 15:36:46.921496 langflow-0.0.76/src/backend/langflow/frontend/assets/index-d5403acc.css
--rw-r--r--   0        0        0  4001839 2023-05-23 15:36:46.925496 langflow-0.0.76/src/backend/langflow/frontend/assets/index-e39661aa.js
--rw-r--r--   0        0        0     4310 2023-05-23 15:36:46.921496 langflow-0.0.76/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-05-23 15:36:46.921496 langflow-0.0.76/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      622 2023-05-23 15:36:46.925496 langflow-0.0.76/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      119 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0    11350 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/base.py
--rw-r--r--   0        0        0       72 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/constants.py
--rw-r--r--   0        0        0     6217 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/graph.py
--rw-r--r--   0        0        0     5884 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/nodes.py
--rw-r--r--   0        0        0      420 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10100 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     2733 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     1993 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4084 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0     2428 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     5592 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1412 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     4811 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0     1668 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1342 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0    13226 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/loading.py
--rw-r--r--   0        0        0       88 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0       87 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2443 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2618 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0    10020 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     2309 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2447 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5353 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      823 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0      811 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     1813 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     1343 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     1488 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.361321 langflow-0.0.76/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1872 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      362 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0      816 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/main.py
--rw-r--r--   0        0        0      579 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/server.py
--rw-r--r--   0        0        0     2131 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0     7763 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/template/base.py
--rw-r--r--   0        0        0      683 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/template/constants.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/template/fields.py
--rw-r--r--   0        0        0    18579 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/template/nodes.py
--rw-r--r--   0        0        0        0 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0      364 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      914 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0    10101 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     5311 2023-05-23 15:35:39.365321 langflow-0.0.76/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    12271 1970-01-01 00:00:00.000000 langflow-0.0.76/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-25 13:43:13.892536 langflow-0.0.78/LICENSE
+-rw-r--r--   0        0        0    10199 2023-05-25 13:43:13.892536 langflow-0.0.78/README.md
+-rw-r--r--   0        0        0     1888 2023-05-25 13:43:13.908536 langflow-0.0.78/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     3726 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0     2032 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/base.py
+-rw-r--r--   0        0        0     1124 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/callback.py
+-rw-r--r--   0        0        0      776 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/chat.py
+-rw-r--r--   0        0        0     8492 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/chat_manager.py
+-rw-r--r--   0        0        0     1246 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/endpoints.py
+-rw-r--r--   0        0        0     1443 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/schemas.py
+-rw-r--r--   0        0        0     1765 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/api/validate.py
+-rw-r--r--   0        0        0       57 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     4333 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4478 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     2369 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0      988 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0     2521 2023-05-25 13:44:14.544752 langflow-0.0.78/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
+-rw-r--r--   0        0        0    11568 2023-05-25 13:44:14.544752 langflow-0.0.78/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
+-rw-r--r--   0        0        0    80491 2023-05-25 13:44:14.544752 langflow-0.0.78/src/backend/langflow/frontend/assets/index-d5403acc.css
+-rw-r--r--   0        0        0  4001839 2023-05-25 13:44:14.548753 langflow-0.0.78/src/backend/langflow/frontend/assets/index-e39661aa.js
+-rw-r--r--   0        0        0     4310 2023-05-25 13:44:14.544752 langflow-0.0.78/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-05-25 13:44:14.544752 langflow-0.0.78/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      622 2023-05-25 13:44:14.548753 langflow-0.0.78/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      119 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0    11350 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/base.py
+-rw-r--r--   0        0        0       72 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/constants.py
+-rw-r--r--   0        0        0     6217 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/graph.py
+-rw-r--r--   0        0        0     6470 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/nodes.py
+-rw-r--r--   0        0        0      420 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10100 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     2733 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     1993 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4084 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0     2428 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     5592 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1412 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     4811 2023-05-25 13:43:13.908536 langflow-0.0.78/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0     1668 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1342 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0    13447 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/loading.py
+-rw-r--r--   0        0        0       88 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0       87 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2443 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2618 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0    10020 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     2309 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2447 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5353 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      823 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0      811 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     1813 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     1343 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     1488 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1872 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      362 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0      816 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/main.py
+-rw-r--r--   0        0        0      579 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     2131 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0     7763 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/template/base.py
+-rw-r--r--   0        0        0      683 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/template/constants.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/template/fields.py
+-rw-r--r--   0        0        0    18579 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/template/nodes.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0      364 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      914 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0    10101 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     5311 2023-05-25 13:43:13.912536 langflow-0.0.78/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    12271 1970-01-01 00:00:00.000000 langflow-0.0.78/PKG-INFO
```

### Comparing `langflow-0.0.76/LICENSE` & `langflow-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/README.md` & `langflow-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/pyproject.toml` & `langflow-0.0.78/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.0.76"
+version = "0.0.78"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Ibis Prevedello <ibiscp@gmail.com>",
     "Lucas Eduoli <lucaseduoli@gmail.com>",
     "Otávio Anovazzi <otavio2204@gmail.com>",
```

### Comparing `langflow-0.0.76/src/backend/langflow/__main__.py` & `langflow-0.0.78/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/base.py` & `langflow-0.0.78/src/backend/langflow/api/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/callback.py` & `langflow-0.0.78/src/backend/langflow/api/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/chat.py` & `langflow-0.0.78/src/backend/langflow/api/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/chat_manager.py` & `langflow-0.0.78/src/backend/langflow/api/chat_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         chat_message = ChatMessage(message=chat_message)
         self.chat_history.add_message(client_id, chat_message)
 
         graph_data = payload
         start_resp = ChatResponse(message=None, type="start", intermediate_steps="")
         await self.send_json(client_id, start_resp)
 
-        is_first_message = len(self.chat_history.get_history(client_id=client_id)) == 0
+        is_first_message = len(self.chat_history.get_history(client_id=client_id)) <= 1
         # Generate result and thought
         try:
             logger.debug("Generating result and thought")
 
             result, intermediate_steps = await process_graph(
                 graph_data=graph_data,
                 is_first_message=is_first_message,
```

### Comparing `langflow-0.0.76/src/backend/langflow/api/endpoints.py` & `langflow-0.0.78/src/backend/langflow/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/schemas.py` & `langflow-0.0.78/src/backend/langflow/api/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/api/validate.py` & `langflow-0.0.78/src/backend/langflow/api/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/cache/base.py` & `langflow-0.0.78/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/cache/manager.py` & `langflow-0.0.78/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/config.yaml` & `langflow-0.0.78/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/custom/customs.py` & `langflow-0.0.78/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg` & `langflow-0.0.78/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/assets/froze-flow-494453cf.png` & `langflow-0.0.78/src/backend/langflow/frontend/assets/froze-flow-494453cf.png`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/assets/index-d5403acc.css` & `langflow-0.0.78/src/backend/langflow/frontend/assets/index-d5403acc.css`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/assets/index-e39661aa.js` & `langflow-0.0.78/src/backend/langflow/frontend/assets/index-e39661aa.js`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.0.78/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/favicon.ico` & `langflow-0.0.78/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/frontend/index.html` & `langflow-0.0.78/src/backend/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/graph/base.py` & `langflow-0.0.78/src/backend/langflow/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/graph/graph.py` & `langflow-0.0.78/src/backend/langflow/graph/graph.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/graph/nodes.py` & `langflow-0.0.78/src/backend/langflow/graph/nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 chain_node.build(tools=self.tools)
 
             self._build()
 
         #! Cannot deepcopy VectorStore, VectorStoreRouter, or SQL agents
         if self.node_type in ["VectorStoreAgent", "VectorStoreRouterAgent", "SQLAgent"]:
             return self._built_object
-        return deepcopy(self._built_object)
+        return self._built_object
 
 
 class ToolNode(Node):
     def __init__(self, data: Dict):
         super().__init__(data, base_type="tools")
 
 
@@ -77,15 +77,15 @@
             for param in prompt_params:
                 prompt_text = self.params[param]
                 variables = extract_input_variables_from_prompt(prompt_text)
                 self.params["input_variables"].extend(variables)
             self.params["input_variables"] = list(set(self.params["input_variables"]))
 
             self._build()
-        return deepcopy(self._built_object)
+        return self._built_object
 
 
 class ChainNode(Node):
     def __init__(self, data: Dict):
         super().__init__(data, base_type="chains")
 
     def build(
@@ -101,21 +101,37 @@
                     self.params[key] = value.build(tools=tools, force=force)
 
             self._build()
 
         #! Cannot deepcopy SQLDatabaseChain
         if self.node_type in ["SQLDatabaseChain"]:
             return self._built_object
-        return deepcopy(self._built_object)
+        return self._built_object
 
 
 class LLMNode(Node):
+    built_node_type = None
+    class_built_object = None
+
     def __init__(self, data: Dict):
         super().__init__(data, base_type="llms")
 
+    def build(self, force: bool = False) -> Any:
+        # LLM is different because some models might take up too much memory
+        # or time to load. So we only load them when we need them.ß
+        if self.node_type == self.built_node_type:
+            return self.class_built_object
+        if not self._built or force:
+            self._build()
+            self.built_node_type = self.node_type
+            self.class_built_object = self._built_object
+        # Avoid deepcopying the LLM
+        # that are loaded from a file
+        return self._built_object
+
 
 class ToolkitNode(Node):
     def __init__(self, data: Dict):
         super().__init__(data, base_type="toolkits")
 
 
 class FileToolNode(ToolNode):
@@ -128,15 +144,15 @@
         super().__init__(data, base_type="wrappers")
 
     def build(self, force: bool = False) -> Any:
         if not self._built or force:
             if "headers" in self.params:
                 self.params["headers"] = eval(self.params["headers"])
             self._build()
-        return deepcopy(self._built_object)
+        return self._built_object
 
 
 class DocumentLoaderNode(Node):
     def __init__(self, data: Dict):
         super().__init__(data, base_type="documentloaders")
 
     def _built_object_repr(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `langflow-0.0.76/src/backend/langflow/interface/agents/base.py` & `langflow-0.0.78/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/agents/custom.py` & `langflow-0.0.78/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.0.78/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/base.py` & `langflow-0.0.78/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/chains/base.py` & `langflow-0.0.78/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/chains/custom.py` & `langflow-0.0.78/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/custom_lists.py` & `langflow-0.0.78/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.0.78/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.0.78/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/importing/utils.py` & `langflow-0.0.78/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/listing.py` & `langflow-0.0.78/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/llms/base.py` & `langflow-0.0.78/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/loading.py` & `langflow-0.0.78/src/backend/langflow/interface/loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,21 @@
 
 
 def instantiate_documentloader(class_object, params):
     return class_object(**params).load()
 
 
 def instantiate_textsplitter(class_object, params):
-    documents = params.pop("documents")
+    try:
+        documents = params.pop("documents")
+    except KeyError as e:
+        raise ValueError(
+            "The source you provided did not load correctly or was empty."
+            "Try changing the chunk_size of the Text Splitter."
+        ) from e
     text_splitter = class_object(**params)
     return text_splitter.split_documents(documents)
 
 
 def instantiate_utility(node_type, class_object, params):
     if node_type == "SQLDatabase":
         return class_object.from_uri(params.pop("uri"))
```

### Comparing `langflow-0.0.76/src/backend/langflow/interface/memories/base.py` & `langflow-0.0.78/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/prompts/base.py` & `langflow-0.0.78/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.0.78/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/run.py` & `langflow-0.0.78/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.0.78/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.0.78/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/tools/base.py` & `langflow-0.0.78/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/tools/constants.py` & `langflow-0.0.78/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/tools/custom.py` & `langflow-0.0.78/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/tools/util.py` & `langflow-0.0.78/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/types.py` & `langflow-0.0.78/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/utilities/base.py` & `langflow-0.0.78/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/utils.py` & `langflow-0.0.78/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.0.78/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.0.78/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/main.py` & `langflow-0.0.78/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/server.py` & `langflow-0.0.78/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/settings.py` & `langflow-0.0.78/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/template/base.py` & `langflow-0.0.78/src/backend/langflow/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/template/constants.py` & `langflow-0.0.78/src/backend/langflow/template/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/template/nodes.py` & `langflow-0.0.78/src/backend/langflow/template/nodes.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/utils/logger.py` & `langflow-0.0.78/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/utils/payload.py` & `langflow-0.0.78/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/utils/util.py` & `langflow-0.0.78/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/src/backend/langflow/utils/validate.py` & `langflow-0.0.78/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.0.76/PKG-INFO` & `langflow-0.0.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.0.76
+Version: 0.0.78
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Gabriel Almeida
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.0.76 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.0.78 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Gabriel Almeida Maintainer-email:
 gabriel@logspace.ai Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

