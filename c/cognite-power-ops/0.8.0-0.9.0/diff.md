# Comparing `tmp/cognite_power_ops-0.8.0.tar.gz` & `tmp/cognite_power_ops-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.8.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.9.0.tar", max compression
```

## Comparing `cognite_power_ops-0.8.0.tar` & `cognite_power_ops-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,53 @@
--rw-r--r--   0        0        0    10758 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/LICENSE
--rw-r--r--   0        0        0      250 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/README.md
--rw-r--r--   0        0        0      192 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10526 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0       23 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/case/__init__.py
--rw-r--r--   0        0        0     3869 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/case/case.py
--rw-r--r--   0        0        0       65 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6202 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2037 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0     1883 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/dm_apis.py
--rw-r--r--   0        0        0     2281 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0     2990 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/client/shop_api.py
--rw-r--r--   0        0        0    27627 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0     3057 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0     2361 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/generator.py
--rw-r--r--   0        0        0     1482 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16336 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0     1609 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0      163 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2171 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1323 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     5039 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    12598 2023-05-24 10:09:23.194885 cognite_power_ops-0.8.0/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-24 10:09:23.198885 cognite_power_ops-0.8.0/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-24 10:09:23.198885 cognite_power_ops-0.8.0/cognite/powerops/version.py
--rw-r--r--   0        0        0     1516 2023-05-24 10:09:23.198885 cognite_power_ops-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/README.md
+-rw-r--r--   0        0        0      192 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10348 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       23 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/case/__init__.py
+-rw-r--r--   0        0        0     3869 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/case/case.py
+-rw-r--r--   0        0        0       65 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6202 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1883 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2281 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     2990 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    33657 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0    13238 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0     2361 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/generator.py
+-rw-r--r--   0        0        0    16336 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0      163 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2171 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1323 2023-05-25 07:05:41.038268 cognite_power_ops-0.9.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     5039 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    12598 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1516 2023-05-25 07:05:41.042268 cognite_power_ops-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.9.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.8.0/LICENSE` & `cognite_power_ops-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.9.0/cognite/powerops/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import os
 from pathlib import Path
 from typing import List, Optional
 
 from cognite.client import CogniteClient
 
 from cognite.powerops.config import (
+    BenchmarkingConfig,
     BidMatrixGeneratorConfig,
     BidProcessConfig,
     BootstrapConfig,
     PriceScenario,
+    RKOMBidCombinationConfig,
     RKOMBidProcessConfig,
+    RkomMarketConfig,
     WatercourseConfig,
 )
-from cognite.powerops.data_classes.benchmarking_config import BenchmarkingConfig
 from cognite.powerops.data_classes.cdf_resource_collection import BootstrapResourceCollection
-from cognite.powerops.data_classes.rkom_bid_combination_config import RKOMBidCombinationConfig
-from cognite.powerops.data_classes.rkom_market_config import RkomMarketConfig
 from cognite.powerops.data_classes.shop_file_config import ShopFileConfig, ShopFileConfigs
 from cognite.powerops.data_classes.shop_output_definition import ShopOutputConfig
 from cognite.powerops.data_classes.time_series_mapping import TimeSeriesMapping, write_mapping_to_sequence
 from cognite.powerops.utils.cdf_auth import get_client
 from cognite.powerops.utils.files import process_yaml_file
 from cognite.powerops.utils.labels import create_labels
 from cognite.powerops.utils.powerops_asset_hierarchy import create_skeleton_asset_hierarchy
```

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/case/case.py` & `cognite_power_ops-0.9.0/cognite/powerops/case/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/asset_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.9.0/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/dm_apis.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/dm_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/client/shop_api.py` & `cognite_power_ops-0.9.0/cognite/powerops/client/shop_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/config.py` & `cognite_power_ops-0.9.0/cognite/powerops/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import ClassVar, Dict, Generator, List, Optional, Tuple
 
 from cognite.client.data_classes import Asset, Label, Sequence
 from pydantic import BaseModel, Field, root_validator, validator
 
-from cognite.powerops.data_classes.benchmarking_config import BenchmarkingConfig
 from cognite.powerops.data_classes.cdf_resource_collection import (
     BootstrapResourceCollection,
     SequenceContent,
     SequenceRows,
 )
 from cognite.powerops.data_classes.common import AggregationMethod, CommonConstants, RelativeTime, RetrievalType
 from cognite.powerops.data_classes.config_model import Configuration
-from cognite.powerops.data_classes.market_config import MarketConfig
 from cognite.powerops.data_classes.reserve_scenario import Auction, Block, Product, ReserveScenario
-from cognite.powerops.data_classes.rkom_bid_combination_config import RKOMBidCombinationConfig
-from cognite.powerops.data_classes.rkom_market_config import RkomMarketConfig
 from cognite.powerops.data_classes.time_series_mapping import (
     TimeSeriesMapping,
     TimeSeriesMappingEntry,
     write_mapping_to_sequence,
 )
 from cognite.powerops.data_classes.transformation import Transformation, TransformationType
 from cognite.powerops.utils.cdf_utils import simple_relationship
@@ -212,14 +208,190 @@
             label_external_id=RelationshipLabels.BID_MATRIX_GENERATOR_CONFIG_SEQUENCE,
         )
         bootstrap_resource_collection.add(relationship)
 
         return bootstrap_resource_collection
 
 
+class RkomMarketConfig(BaseModel):
+    external_id: str
+    name: str
+    timezone: str
+    start_of_week: int
+    parent_external_id: ClassVar[str] = "market_configurations"
+
+    @property
+    def metadata(self) -> dict:
+        return {
+            "timezone": self.timezone,
+            "start_of_week": self.start_of_week,
+        }
+
+    @property
+    def cdf_asset(self) -> Asset:
+        return Asset(
+            external_id=self.external_id,
+            name=self.name,
+            metadata=self.metadata,
+            parent_external_id=self.parent_external_id,
+            labels=["market"],
+        )
+
+    @staticmethod
+    def default() -> "RkomMarketConfig":
+        return RkomMarketConfig(
+            external_id="market_configuration_statnett_rkom_weekly",
+            name="RKOM weekly (Statnett)",
+            timezone="Europe/Oslo",
+            start_of_week=1,
+        )
+
+
+class RKOMBidCombinationConfig(Configuration):
+    auction: Auction = Field(alias="bid_auction")
+    name: str = Field("default", alias="bid_combination_name")
+    rkom_bid_config_external_ids: List[str] = Field(alias="bid_rkom_bid_configs")
+    parent_external_id: ClassVar[str] = "rkom_bid_combination_configurations"
+
+    @validator("auction", pre=True)
+    def to_enum(cls, value):
+        return Auction[value] if isinstance(value, str) else value
+
+    @validator("rkom_bid_config_external_ids", pre=True)
+    def parse_string(cls, value):
+        return [external_id for external_id in ast.literal_eval(value)] if isinstance(value, str) else value
+
+    @property
+    def cdf_asset(self) -> Asset:
+        sequence_external_id = f"RKOM_bid_combination_configuration_{self.auction.value}_{self.name}"
+
+        return Asset(
+            name=sequence_external_id.replace("_", " "),
+            description="Defining which RKOM bid methods should be combined (into the total bid form)",
+            external_id=sequence_external_id,
+            metadata={
+                "bid:auction": self.auction.value,
+                "bid:combination_name": self.name,
+                "bid:rkom_bid_configs": json.dumps(self.rkom_bid_config_external_ids),
+            },
+            parent_external_id=self.parent_external_id,
+        )
+
+
+class BenchmarkingConfig(Configuration):
+    bid_date: RelativeTime
+    shop_start: RelativeTime = Field(alias="shop_starttime")
+    shop_end: RelativeTime = Field(alias="shop_endtime")
+    production_plan_time_series: Optional[Dict[str, List[str]]]
+    market_config_external_id: str = Field(alias="bid_market_config_external_id")
+    relevant_shop_objective_metrics: Dict[str, str] = {
+        "grand_total": "Grand Total",
+        "total": "Total",
+        "sum_penalties": "Sum Penalties",
+        "major_penalties": "Major Penalties",
+        "minor_penalties": "Minor Penalties",
+        "load_value": "Load Value",
+        "market_sale_buy": "Market Sale Buy",
+        "rsv_end_value_relative": "RSV End Value Relative",
+        "startup_costs": "Startup Costs",
+        "vow_in_transit": "Vow in Transit",
+        "sum_feeding_fee": "Sum Feeding Fee",
+        "rsv_tactical_penalty": "RSV Tactical Penalty",
+        "rsv_end_value": "RSV End Value",
+        "bypass_cost": "Bypass Cost",
+        "gate_discharge_cost": "Gate Discharge Cost",
+        "reserve_violation_penalty": "Reserve Violation Penalty",
+        "load_penalty": "Load Penalty",
+    }  # Pydantic handles mutable defaults such that this is OK:
+    # https://stackoverflow.com/questions/63793662/how-to-give-a-pydantic-list-field-a-default-value/63808835#63808835
+    # TODO: Consider adding relationships to bid process config
+    #  assets (or remove the optional part that uses those relationships in power-ops-functions)
+
+    @validator("shop_start", "shop_end", "bid_date", pre=True)
+    def json_loads(cls, value):
+        return {"operations": json.loads(value)} if isinstance(value, str) else value
+
+    @property
+    def metadata(self) -> dict:
+        metadata = {
+            "bid:date": str(self.bid_date),
+            "shop:starttime": str(self.shop_start),
+            "shop:endtime": str(self.shop_end),
+            "bid:market_config_external_id": self.market_config_external_id,
+            "benchmarking_metrics": json.dumps(self.relevant_shop_objective_metrics),
+        }
+        if self.production_plan_time_series:
+            metadata["benchmark:production_plan_time_series"] = json.dumps(
+                self.production_plan_time_series, ensure_ascii=False
+            )  # ensure_ascii=False to treat Nordic letters properly
+        return metadata
+
+    @property
+    def cdf_asset(self) -> Asset:
+        return Asset(
+            external_id="POWEROPS_dayahead_bidding_benchmarking_config",
+            name="Benchmarking config DA",
+            description="Configuration for benchmarking of day-ahead bidding",
+            metadata=self.metadata,
+            parent_external_id="benchmarking_configurations",
+            labels=["dayahead_bidding_benchmarking_config"],
+        )
+
+
+class MarketConfig(Configuration):
+    external_id: str
+    name: str
+    max_price: float = None
+    min_price: float = None
+    time_unit: str = None
+    timezone: str
+    tick_size: float = None
+    trade_lot: float = None
+    price_steps: int = None
+    parent_external_id: ClassVar[str] = "market_configurations"
+    price_unit: str = None
+
+    @property
+    def metadata(self) -> dict:
+        return {
+            "min_price": self.min_price,
+            "max_price": self.max_price,
+            "timezone": self.timezone,
+            "time_unit": self.time_unit,
+            "tick_size": self.tick_size,
+            "trade_lot": self.trade_lot,
+            "price_steps": self.price_steps,
+            "price_unit": self.price_unit,
+        }
+
+    @property
+    def cdf_asset(self) -> Asset:
+        return Asset(
+            external_id=self.external_id,
+            name=self.name,
+            metadata=self.metadata,
+            parent_external_id=self.parent_external_id,
+            labels=["market"],
+        )
+
+
+MARKET_CONFIG_NORDPOOL_DAYAHEAD = MarketConfig(
+    external_id="market_configuration_nordpool_dayahead",
+    name="Nord Pool Day-ahead",
+    max_price=4000,
+    min_price=-500,
+    time_unit="1h",
+    timezone="Europe/Oslo",
+    tick_size=0.1,
+    trade_lot=0.1,
+    price_steps=200,
+    price_unit="EUR/MWh",
+)
+
+
 class BidProcessConfig(Configuration):
     name: str
     price_area_name: str = Field(alias="bid_price_area")
     price_scenarios: List[PriceScenarioID] = Field(alias="bid_price_scenarios")
     main_scenario: str = Field(alias="bid_main_scenario")
     bid_date: Optional[RelativeTime] = None
     shop_start: Optional[RelativeTime] = Field(None, alias="shop_starttime")
```

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/generator.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.9.0/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/logger.py` & `cognite_power_ops-0.9.0/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/main.py` & `cognite_power_ops-0.9.0/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/common.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/files.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.9.0/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.8.0/pyproject.toml` & `cognite_power_ops-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.8.0"
+version = "0.9.0"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
```

### Comparing `cognite_power_ops-0.8.0/PKG-INFO` & `cognite_power_ops-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.8.0
+Version: 0.9.0
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

